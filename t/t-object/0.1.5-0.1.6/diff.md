# Comparing `tmp/t_object-0.1.5.tar.gz` & `tmp/t_object-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-yza8jpkq/t_object-0.1.5.tar", last modified: Thu Mar 28 15:46:39 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-9azii37_/t_object-0.1.6.tar", last modified: Fri Apr  5 17:12:10 2024, max compression
```

## Comparing `t_object-0.1.5.tar` & `t_object-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 15:46:39.767207 t_object-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-28 15:46:12.000000 t_object-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4291 2024-03-28 15:46:39.767207 t_object-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3871 2024-03-28 15:46:12.000000 t_object-0.1.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-28 15:46:12.000000 t_object-0.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-03-28 15:46:12.000000 t_object-0.1.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-03-28 15:46:39.771207 t_object-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-28 15:46:12.000000 t_object-0.1.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 15:46:39.767207 t_object-0.1.5/t_object/
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-28 15:46:12.000000 t_object-0.1.5/t_object/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7893 2024-03-28 15:46:12.000000 t_object-0.1.5/t_object/base_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8633 2024-03-28 15:46:12.000000 t_object-0.1.5/t_object/builder.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-03-28 15:46:12.000000 t_object-0.1.5/t_object/config_enums.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-03-28 15:46:12.000000 t_object-0.1.5/t_object/t_object.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 15:46:39.767207 t_object-0.1.5/t_object.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4291 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-03-28 15:46:39.000000 t_object-0.1.5/t_object.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 15:46:39.767207 t_object-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2734 2024-03-28 15:46:12.000000 t_object-0.1.5/tests/test_t_object.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 17:12:10.750604 t_object-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-05 17:11:47.000000 t_object-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4291 2024-04-05 17:12:10.750604 t_object-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3871 2024-04-05 17:11:47.000000 t_object-0.1.6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-05 17:11:47.000000 t_object-0.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-05 17:11:47.000000 t_object-0.1.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-05 17:12:10.754604 t_object-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-05 17:11:47.000000 t_object-0.1.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 17:12:10.750604 t_object-0.1.6/t_object/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-05 17:11:47.000000 t_object-0.1.6/t_object/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7956 2024-04-05 17:11:47.000000 t_object-0.1.6/t_object/base_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8633 2024-04-05 17:11:47.000000 t_object-0.1.6/t_object/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-05 17:11:47.000000 t_object-0.1.6/t_object/config_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-05 17:11:47.000000 t_object-0.1.6/t_object/t_object.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 17:12:10.750604 t_object-0.1.6/t_object.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4291 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-05 17:12:10.000000 t_object-0.1.6/t_object.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 17:12:10.750604 t_object-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2024-04-05 17:11:47.000000 t_object-0.1.6/tests/test_t_object.py
```

### Comparing `t_object-0.1.5/PKG-INFO` & `t_object-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_object
-Version: 0.1.5
+Version: 0.1.6
 Summary: t_object
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_object
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_object-0.1.5/README.rst` & `t_object-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `t_object-0.1.5/setup.py` & `t_object-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     description="t_object",
     long_description=readme,
     keywords="t_object",
     name="t_object",
     packages=find_packages(include=["t_object", "t_object.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.1.5",
+    version="0.1.6",
     zip_safe=False,
     install_requires=install_requirements,
 )
```

### Comparing `t_object-0.1.5/t_object/base_object.py` & `t_object-0.1.6/t_object/base_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         if extension != ".json":
             raise ValueError(f"File extension must be .json, not {extension}")
 
         with open(file_path, "w") as file:
             file.write(self.convert_to_json_string())
         return file_path
 
+    def __dict__(self):
+        return self.convert_to_dict()
+
     def save_to_pickle_file(self, file_path: str) -> str:
         """Save an object to a pickle file.
 
         Args:
             file_path (str): The path to the file.
         """
         file_path = file_path or self.model_config.get("pickle_file_name")
```

### Comparing `t_object-0.1.5/t_object/builder.py` & `t_object-0.1.6/t_object/builder.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.5/t_object/config_enums.py` & `t_object-0.1.6/t_object/config_enums.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.5/t_object/t_object.py` & `t_object-0.1.6/t_object/t_object.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.5/t_object.egg-info/PKG-INFO` & `t_object-0.1.6/t_object.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_object
-Version: 0.1.5
+Version: 0.1.6
 Summary: t_object
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_object
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_object-0.1.5/tests/test_t_object.py` & `t_object-0.1.6/tests/test_t_object.py`

 * *Files identical despite different names*

