# Comparing `tmp/streamlit-nivo-charts-custom-0.0.8.tar.gz` & `tmp/streamlit-nivo-charts-custom-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nivo-charts-custom-0.0.8.tar", last modified: Fri Apr  5 08:24:24 2024, max compression
+gzip compressed data, was "streamlit-nivo-charts-custom-0.0.9.tar", last modified: Fri Apr  5 08:47:13 2024, max compression
```

## Comparing `streamlit-nivo-charts-custom-0.0.8.tar` & `streamlit-nivo-charts-custom-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:24:24.035085 streamlit-nivo-charts-custom-0.0.8/
--rw-rw-rw-   0        0        0     1082 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-05 08:10:07.000000 streamlit-nivo-charts-custom-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      210 2024-04-05 08:24:24.028075 streamlit-nivo-charts-custom-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 08:24:23.774805 streamlit-nivo-charts-custom-0.0.8/all_charts_component/
--rw-rw-rw-   0        0        0     1186 2024-04-05 08:11:00.000000 streamlit-nivo-charts-custom-0.0.8/all_charts_component/__init__.py
--rw-rw-rw-   0        0        0    11156 2024-04-05 08:04:52.000000 streamlit-nivo-charts-custom-0.0.8/all_charts_component/example.py
--rw-rw-rw-   0        0        0       42 2024-04-05 08:24:24.036080 streamlit-nivo-charts-custom-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-04-05 08:09:51.000000 streamlit-nivo-charts-custom-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:24:24.019082 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/
--rw-rw-rw-   0        0        0      210 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-05 08:24:22.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:13.299647 streamlit-nivo-charts-custom-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       57 2024-04-05 08:46:05.000000 streamlit-nivo-charts-custom-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      210 2024-04-05 08:47:13.295648 streamlit-nivo-charts-custom-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:12.580285 streamlit-nivo-charts-custom-0.0.9/all_charts_component/
+-rw-rw-rw-   0        0        0     1186 2024-04-05 08:11:00.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/__init__.py
+-rw-rw-rw-   0        0        0    11209 2024-04-05 08:45:43.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/example.py
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:12.493278 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:12.813277 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/
+-rw-rw-rw-   0        0        0      374 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      553 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:12.504275 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:12.886283 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/css/
+-rw-rw-rw-   0        0        0      162 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/css/main.e68b0f0c.css
+-rw-rw-rw-   0        0        0      648 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/css/main.e68b0f0c.css.map
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:13.034290 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   866998 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/js/main.95fa7223.js
+-rw-rw-rw-   0        0        0     1293 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/js/main.95fa7223.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  3727348 2024-04-05 08:16:12.000000 streamlit-nivo-charts-custom-0.0.9/all_charts_component/frontend/build/static/js/main.95fa7223.js.map
+-rw-rw-rw-   0        0        0       42 2024-04-05 08:47:13.300651 streamlit-nivo-charts-custom-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-04-05 08:46:54.000000 streamlit-nivo-charts-custom-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 08:47:13.288651 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-04-05 08:47:10.000000 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2024-04-05 08:47:11.000000 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 08:47:10.000000 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-05 08:47:10.000000 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-05 08:47:10.000000 streamlit-nivo-charts-custom-0.0.9/streamlit_nivo_charts_custom.egg-info/top_level.txt
```

### Comparing `streamlit-nivo-charts-custom-0.0.8/LICENSE` & `streamlit-nivo-charts-custom-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-nivo-charts-custom-0.0.8/all_charts_component/__init__.py` & `streamlit-nivo-charts-custom-0.0.9/all_charts_component/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nivo-charts-custom-0.0.8/all_charts_component/example.py` & `streamlit-nivo-charts-custom-0.0.9/all_charts_component/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import streamlit as st
-from __init__ import chart_to_display
+# from __init__ import chart_to_display
+from all_charts_component import chart_to_display
 
 st.set_page_config(layout="wide")
 
 chartData = [
   {
     "damageType": "Final Skill Damage",
     "Physical": 84,
```

### Comparing `streamlit-nivo-charts-custom-0.0.8/setup.py` & `streamlit-nivo-charts-custom-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 # long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-nivo-charts-custom",
-    version="0.0.8",
+    version="0.0.9",
     author="John Smith",
     author_email="john@example.com",
     # description="",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

