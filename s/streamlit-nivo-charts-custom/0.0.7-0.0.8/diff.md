# Comparing `tmp/streamlit-nivo-charts-custom-0.0.7.tar.gz` & `tmp/streamlit-nivo-charts-custom-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nivo-charts-custom-0.0.7.tar", last modified: Tue Mar 26 15:48:33 2024, max compression
+gzip compressed data, was "streamlit-nivo-charts-custom-0.0.8.tar", last modified: Fri Apr  5 08:24:24 2024, max compression
```

## Comparing `streamlit-nivo-charts-custom-0.0.7.tar` & `streamlit-nivo-charts-custom-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:33.740533 streamlit-nivo-charts-custom-0.0.7/
--rw-rw-rw-   0        0        0     1082 2024-02-28 13:18:47.000000 streamlit-nivo-charts-custom-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       57 2024-02-29 10:29:02.000000 streamlit-nivo-charts-custom-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      210 2024-03-26 15:48:33.726405 streamlit-nivo-charts-custom-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-02-28 13:18:47.000000 streamlit-nivo-charts-custom-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:32.398555 streamlit-nivo-charts-custom-0.0.7/all_charts_component/
--rw-rw-rw-   0        0        0     1561 2024-03-26 15:47:10.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/__init__.py
--rw-rw-rw-   0        0        0     9452 2024-03-26 13:36:07.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/example.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:32.146751 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:32.588450 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/
--rw-rw-rw-   0        0        0      374 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-02-28 13:18:47.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      553 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:32.154320 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:32.656410 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/css/
--rw-rw-rw-   0        0        0      161 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/css/main.8529466c.css
--rw-rw-rw-   0        0        0      647 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/css/main.8529466c.css.map
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:33.375169 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0  1210734 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/js/main.907b3ec8.js
--rw-rw-rw-   0        0        0     1293 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/js/main.907b3ec8.js.LICENSE.txt
--rw-rw-rw-   0        0        0  4917540 2024-03-26 15:45:38.000000 streamlit-nivo-charts-custom-0.0.7/all_charts_component/frontend/build/static/js/main.907b3ec8.js.map
--rw-rw-rw-   0        0        0       42 2024-03-26 15:48:33.741563 streamlit-nivo-charts-custom-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-03-26 15:48:07.000000 streamlit-nivo-charts-custom-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:48:33.716842 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/
--rw-rw-rw-   0        0        0      210 2024-03-26 15:48:30.000000 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2024-03-26 15:48:31.000000 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 15:48:30.000000 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-03-26 15:48:30.000000 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-03-26 15:48:30.000000 streamlit-nivo-charts-custom-0.0.7/streamlit_nivo_charts_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 08:24:24.035085 streamlit-nivo-charts-custom-0.0.8/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-05 08:10:07.000000 streamlit-nivo-charts-custom-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      210 2024-04-05 08:24:24.028075 streamlit-nivo-charts-custom-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-05 07:04:07.000000 streamlit-nivo-charts-custom-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 08:24:23.774805 streamlit-nivo-charts-custom-0.0.8/all_charts_component/
+-rw-rw-rw-   0        0        0     1186 2024-04-05 08:11:00.000000 streamlit-nivo-charts-custom-0.0.8/all_charts_component/__init__.py
+-rw-rw-rw-   0        0        0    11156 2024-04-05 08:04:52.000000 streamlit-nivo-charts-custom-0.0.8/all_charts_component/example.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 08:24:24.036080 streamlit-nivo-charts-custom-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-04-05 08:09:51.000000 streamlit-nivo-charts-custom-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 08:24:24.019082 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-04-05 08:24:22.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-05 08:24:21.000000 streamlit-nivo-charts-custom-0.0.8/streamlit_nivo_charts_custom.egg-info/top_level.txt
```

### Comparing `streamlit-nivo-charts-custom-0.0.7/LICENSE` & `streamlit-nivo-charts-custom-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-nivo-charts-custom-0.0.7/all_charts_component/__init__.py` & `streamlit-nivo-charts-custom-0.0.8/all_charts_component/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import streamlit.components.v1 as components
 
-_RELEASE = True  
+_RELEASE = True   
 
 if not _RELEASE:
     _chart_to_display = components.declare_component(
         
         "chart_to_display",
 
         url="http://localhost:3001",
@@ -14,34 +14,26 @@
 
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _chart_to_display = components.declare_component("chart_to_display", path=build_dir)
 
 def chart_to_display(
         chartType="pieChart", 
-        barChartCustomComponent=None,
-        barChartCustomColor=None,
-        barChartCustomColorsToSet=None,
-        customChartTextLayout=None,
         chartData=None, 
         styles=None, 
         chartLayout=None, 
         scatterPlotCustom={ "customComponent": True, "customTooltip": False }, 
         customNodeSize=None,
         scatterToolTipStyle=None,
         key=None, 
         default=None
         ):
     
     component_value = _chart_to_display(
         chartType=chartType, 
-        barChartCustomComponent=barChartCustomComponent,
-        barChartCustomColor=barChartCustomColor,
-        barChartCustomColorsToSet=barChartCustomColorsToSet,
-        customChartTextLayout=customChartTextLayout,
         chartData=chartData, 
         chartLayout=chartLayout, 
         styles=styles, 
         scatterPlotCustom=scatterPlotCustom, 
         customNodeSize=customNodeSize,
         scatterToolTipStyle=scatterToolTipStyle,
         key=key,
```

### Comparing `streamlit-nivo-charts-custom-0.0.7/setup.py` & `streamlit-nivo-charts-custom-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 # long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-nivo-charts-custom",
-    version="0.0.7",
+    version="0.0.8",
     author="John Smith",
     author_email="john@example.com",
     # description="",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

