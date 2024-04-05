# Comparing `tmp/input_field_component-0.0.1.tar.gz` & `tmp/input_field_component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input_field_component-0.0.1.tar", last modified: Thu Nov 23 17:32:53 2023, max compression
+gzip compressed data, was "input_field_component-0.0.2.tar", last modified: Fri Apr  5 16:42:04 2024, max compression
```

## Comparing `input_field_component-0.0.1.tar` & `input_field_component-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.977203 input_field_component-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-09-06 18:19:28.000000 input_field_component-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       58 2023-11-23 15:15:45.000000 input_field_component-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1020 2023-11-23 17:32:53.976203 input_field_component-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-09-09 11:52:15.000000 input_field_component-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.931582 input_field_component-0.0.1/input_field_component/
--rw-rw-rw-   0        0        0     2957 2023-11-23 15:15:38.000000 input_field_component-0.0.1/input_field_component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.925577 input_field_component-0.0.1/input_field_component/frontend/
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.946175 input_field_component-0.0.1/input_field_component/frontend/build/
--rw-rw-rw-   0        0        0      221 2023-11-23 15:18:13.000000 input_field_component-0.0.1/input_field_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-09-06 18:19:28.000000 input_field_component-0.0.1/input_field_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2023-11-23 15:18:13.000000 input_field_component-0.0.1/input_field_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.926578 input_field_component-0.0.1/input_field_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.973199 input_field_component-0.0.1/input_field_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   380246 2023-11-23 15:18:13.000000 input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js
--rw-rw-rw-   0        0        0     1443 2023-11-23 15:18:13.000000 input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1351058 2023-11-23 15:18:13.000000 input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js.map
-drwxrwxrwx   0        0        0        0 2023-11-23 17:32:53.937165 input_field_component-0.0.1/input_field_component.egg-info/
--rw-rw-rw-   0        0        0     1020 2023-11-23 17:32:53.000000 input_field_component-0.0.1/input_field_component.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2023-11-23 17:32:53.000000 input_field_component-0.0.1/input_field_component.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 17:32:53.000000 input_field_component-0.0.1/input_field_component.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-11-23 17:32:53.000000 input_field_component-0.0.1/input_field_component.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-11-23 17:32:53.000000 input_field_component-0.0.1/input_field_component.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-23 17:32:53.977203 input_field_component-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-11-23 17:28:06.000000 input_field_component-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.068389 input_field_component-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-09-06 18:19:28.000000 input_field_component-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-11-23 15:15:45.000000 input_field_component-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1020 2024-04-05 16:42:04.068389 input_field_component-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-09-09 11:52:15.000000 input_field_component-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.053375 input_field_component-0.0.2/input_field_component/
+-rw-rw-rw-   0        0        0     1268 2024-04-05 16:41:43.000000 input_field_component-0.0.2/input_field_component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.047370 input_field_component-0.0.2/input_field_component/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.060382 input_field_component-0.0.2/input_field_component/frontend/build/
+-rw-rw-rw-   0        0        0      221 2023-11-23 15:18:13.000000 input_field_component-0.0.2/input_field_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-09-06 18:19:28.000000 input_field_component-0.0.2/input_field_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2023-11-23 15:18:13.000000 input_field_component-0.0.2/input_field_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.048370 input_field_component-0.0.2/input_field_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.064385 input_field_component-0.0.2/input_field_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   380246 2023-11-23 15:18:13.000000 input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js
+-rw-rw-rw-   0        0        0     1443 2023-11-23 15:18:13.000000 input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1351058 2023-11-23 15:18:13.000000 input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js.map
+drwxrwxrwx   0        0        0        0 2024-04-05 16:42:04.066387 input_field_component-0.0.2/input_field_component.egg-info/
+-rw-rw-rw-   0        0        0     1020 2024-04-05 16:42:03.000000 input_field_component-0.0.2/input_field_component.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2024-04-05 16:42:04.000000 input_field_component-0.0.2/input_field_component.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:42:03.000000 input_field_component-0.0.2/input_field_component.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-05 16:42:03.000000 input_field_component-0.0.2/input_field_component.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-05 16:42:03.000000 input_field_component-0.0.2/input_field_component.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:42:04.068389 input_field_component-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2024-04-05 16:40:12.000000 input_field_component-0.0.2/setup.py
```

### Comparing `input_field_component-0.0.1/LICENSE` & `input_field_component-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/PKG-INFO` & `input_field_component-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input_field_component
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to create sentence with input field
 Home-page: 
 Author: Timonin Danila
 Author-email: dantimonin@zoho.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `input_field_component-0.0.1/input_field_component/frontend/build/bootstrap.min.css` & `input_field_component-0.0.2/input_field_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js` & `input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js.LICENSE.txt` & `input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/input_field_component/frontend/build/static/js/main.89ba5e0b.js.map` & `input_field_component-0.0.2/input_field_component/frontend/build/static/js/main.89ba5e0b.js.map`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/input_field_component.egg-info/PKG-INFO` & `input_field_component-0.0.2/input_field_component.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: input-field-component
-Version: 0.0.1
+Name: input_field_component
+Version: 0.0.2
 Summary: Streamlit component that allows you to create sentence with input field
 Home-page: 
 Author: Timonin Danila
 Author-email: dantimonin@zoho.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `input_field_component-0.0.1/input_field_component.egg-info/SOURCES.txt` & `input_field_component-0.0.2/input_field_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `input_field_component-0.0.1/setup.py` & `input_field_component-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="input_field_component",
-    version="0.0.1",
+    version="0.0.2",
     author="Timonin Danila",
     author_email="dantimonin@zoho.com",
     description="Streamlit component that allows you to create sentence with input field",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

