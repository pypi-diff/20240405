# Comparing `tmp/lookml_zenml-0.1.5.tar.gz` & `tmp/lookml_zenml-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookml_zenml-0.1.5.tar", max compression
+gzip compressed data, was "lookml_zenml-0.1.6.tar", max compression
```

## Comparing `lookml_zenml-0.1.5.tar` & `lookml_zenml-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.5/LICENSE
--rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.5/README.md
--rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.5/lookml_zenml/__init__.py
--rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.5/lookml_zenml/cli.py
--rw-r--r--   0        0        0    28081 2024-03-30 16:01:51.145265 lookml_zenml-0.1.5/lookml_zenml/lookml_project.py
--rw-r--r--   0        0        0      581 2024-03-29 23:58:11.328924 lookml_zenml-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.6/README.md
+-rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.6/lookml_zenml/__init__.py
+-rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.6/lookml_zenml/cli.py
+-rw-r--r--   0        0        0    29505 2024-04-05 04:59:10.886590 lookml_zenml-0.1.6/lookml_zenml/lookml_project.py
+-rw-r--r--   0        0        0      581 2024-04-05 05:01:45.882475 lookml_zenml-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.6/PKG-INFO
```

### Comparing `lookml_zenml-0.1.5/LICENSE` & `lookml_zenml-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.5/README.md` & `lookml_zenml-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.5/lookml_zenml/cli.py` & `lookml_zenml-0.1.6/lookml_zenml/cli.py`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.5/lookml_zenml/lookml_project.py` & `lookml_zenml-0.1.6/lookml_zenml/lookml_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import os
 import lkml
+import json
 from ruamel.yaml import YAML
 import uuid
 from collections import defaultdict
 
 FIELD_KEY_ORDER = ["name", "field_type", "type", "description", "timeframes", "sql"]
 yaml = YAML()
 yaml.indent(sequence=4, offset=2)
@@ -15,14 +16,15 @@
     def __init__(self, in_directory: str = None, out_directory: str = None):
         self.in_directory = in_directory
         self.out_directory = out_directory
         self.field_mappings = []
         self._views = []
         self._models = []
         self._explore_from_mapping = {}
+        self._default_model_name = None
 
     def convert(self):
         if not self.in_directory:
             raise ValueError(
                 "You must pass the in_directory argument to the class to use this function. "
                 "If you want to convert dict -> dict use the convert_project function in this class"
             )
@@ -46,21 +48,21 @@
             self._explore_from_mapping[model["name"]] = model_view_metadata["explore_from_mapping"]
             view_metadata.update(model_view_metadata["graph"])
             for view_name in set(model_view_metadata["graph"].keys()):
                 views_to_models[view_name] = model["name"]
             models.append(model)
         self._models = models
 
-        default_model_name = models[0]["name"]
+        self._default_model_name = models[0]["name"]
         for raw_view in lookml_project["views"]:
             # We don't currently get access filters from the explores
             # because they vary across explores for the same view
             view = self.convert_view(
                 raw_view,
-                views_to_models.get(raw_view["name"], default_model_name),
+                views_to_models.get(raw_view["name"], self._default_model_name),
                 access_filters=[],
                 joins=view_metadata.get(raw_view["name"], []),
             )
             views.append(view)
         self._views = views
 
         for raw_dashboard in lookml_project["dashboards"]:
@@ -290,14 +292,22 @@
             "name": dashboard["dashboard"],
             "label": dashboard["title"],
             "elements": [],
         }
         if "description" in dashboard:
             zenml_data["description"] = dashboard["description"]
 
+        if "filters" in dashboard:
+            zenml_data["filters"] = []
+            for f in dashboard["filters"]:
+                field = self._get_field(
+                    f["field"], self._views, model_name=f.get("model"), explore_name=f.get("explore")
+                )
+                zenml_data["filters"].append({"field": field["id"], "value": f.get("default_value")})
+
         for element in dashboard["elements"]:
             zenml_element = self._translate_dashboard_element(element)
             if zenml_element:
                 zenml_data["elements"].append(zenml_element)
 
         return zenml_data
 
@@ -305,17 +315,37 @@
         if "merged_queries" in element:
             return self._translate_merged_queries_element(element)
         return self._translate_vanilla_element(element)
 
     def _translate_vanilla_element(self, element: dict):
         # We do not support conditional formatting in dashboards
         # We do not support non-query elements yet, either
-        if "model" not in element:
+        if "model" not in element and element.get("type") not in {"button", "text"}:
             return None
 
+        elif element.get("type") == "text":
+            model_name = self._default_model_name if self._default_model_name else "todo"
+            zenml_element = {"model": model_name, "type": "markdown", "size": "quarter"}
+            zenml_element["content"] = element.get("body_text", "")
+            return zenml_element
+
+        elif element.get("type") == "button":
+            model_name = self._default_model_name if self._default_model_name else "todo"
+            zenml_element = {"model": model_name, "type": "markdown", "size": "quarter"}
+            content_json = json.loads(element.get("rich_content_json", "{}"))
+            link_url = content_json.get("href", "")
+
+            if link_text := content_json.get("text", ""):
+                content = f"[{link_text}]({link_url})"
+            else:
+                content = link_url
+
+            zenml_element["content"] = content
+            return zenml_element
+
         zenml_element = {"model": element["model"], "metrics": [], "slice_by": []}
         if "title" in element:
             zenml_element["title"] = element["title"]
 
         # Add fields
         if "fields" not in element:
             return None
```

### Comparing `lookml_zenml-0.1.5/pyproject.toml` & `lookml_zenml-0.1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lookml-zenml"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Paul Blankley <paul@zenlytic.com>"]
 readme = "README.md"
 packages = [{include = "lookml_zenml"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <3.12"
```

### Comparing `lookml_zenml-0.1.5/PKG-INFO` & `lookml_zenml-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookml-zenml
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Paul Blankley
 Author-email: paul@zenlytic.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

