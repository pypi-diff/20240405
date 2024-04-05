# Comparing `tmp/civilpy-0.0.77.tar.gz` & `tmp/civilpy-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.77.tar", last modified: Wed Mar 27 13:30:48 2024, max compression
+gzip compressed data, was "civilpy-0.0.78.tar", last modified: Fri Apr  5 13:49:11 2024, max compression
```

## Comparing `civilpy-0.0.77.tar` & `civilpy-0.0.78.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.275956 civilpy-0.0.77/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.77/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6682 2024-03-27 13:30:48.275956 civilpy-0.0.77/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.77/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 13:30:48.275956 civilpy-0.0.77/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3028 2024-03-27 10:49:10.000000 civilpy-0.0.77/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.77/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.267956 civilpy-0.0.77/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.271956 civilpy-0.0.77/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.271956 civilpy-0.0.77/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 13:30:21.000000 civilpy-0.0.77/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14159 2024-03-27 10:49:10.000000 civilpy-0.0.77/src/civilpy/structural/arema.py
--rw-rw-rw-   0 root         (0) root         (0)    20861 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)     8479 2024-03-27 12:42:27.000000 civilpy-0.0.77/src/civilpy/structural/midas.py
--rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/structural/rail_tpg_design.py
--rw-rw-rw-   0 root         (0) root         (0)    15183 2024-03-08 15:32:48.000000 civilpy-0.0.77/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.271956 civilpy-0.0.77/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.271956 civilpy-0.0.77/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.77/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:30:48.271956 civilpy-0.0.77/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6682 2024-03-27 13:30:48.000000 civilpy-0.0.77/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1253 2024-03-27 13:30:48.000000 civilpy-0.0.77/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 13:30:48.000000 civilpy-0.0.77/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      719 2024-03-27 13:30:48.000000 civilpy-0.0.77/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-27 13:30:48.000000 civilpy-0.0.77/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.162531 civilpy-0.0.78/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.78/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-04-05 13:49:11.162531 civilpy-0.0.78/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.78/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 13:49:11.162531 civilpy-0.0.78/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-04 19:12:50.000000 civilpy-0.0.78/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.154531 civilpy-0.0.78/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.78/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 13:48:41.000000 civilpy-0.0.78/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.78/src/civilpy/structural/arema.py
+-rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.78/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)     8479 2024-03-27 12:42:27.000000 civilpy-0.0.78/src/civilpy/structural/midas.py
+-rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/structural/rail_tpg_design.py
+-rw-rw-rw-   0 root         (0) root         (0)    15183 2024-03-08 15:32:48.000000 civilpy-0.0.78/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.78/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:49:11.158531 civilpy-0.0.78/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1253 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      719 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-05 13:49:11.000000 civilpy-0.0.78/src/civilpy.egg-info/top_level.txt
```

### Comparing `civilpy-0.0.77/LICENSE` & `civilpy-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/PKG-INFO` & `civilpy-0.0.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.77
+Version: 0.0.78
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.77 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.78 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
-Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
-MIT License Classifier: Environment :: Console :: Curses Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: numpy>=1.14.5
-Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5 Requires-Dist:
-Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist: coverage>=7.1.0
-Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-selenium-
-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist: PyPDF2>=3.0.1
-Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist: sympy>=1.10.0 Requires-
-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0 Requires-Dist:
-icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist: geopandas>=0.6.2
-Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7 Requires-Dist:
-natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist: requests>=2.28.2
-Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2 Requires-Dist:
-tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist: pytest>=7.4.1
-Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-Dist:
-matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0; extra ==
-"full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full" Requires-
-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6; extra ==
-"full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full" Requires-Dist:
-sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0; extra == "full"
-Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist: earthpy>=0.9.4;
-extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full" Requires-Dist:
-pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1; extra == "full"
-Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist: tox>=4.11.1; extra
-== "full" # CivilPy ![PyPI - License](https://img.shields.io/pypi/l/civilpy)
-[Project badge][PyPI - Python Version][Project badge]![PyPI - Downloads](https:
-//img.shields.io/pypi/dm/CivilPy) Code snippets for Civil Engineering related
-tasks ## About (Skip to the "Installation" section to start running code)
-Welcome to the CivilPy repository. This is a simple software package to give
-civil engineers cleaner access to some of the packages from the python
-ecosystem. The package is focused on civil engineering related tasks such as
-file management, pdf data extraction, image manipulation mapping and unit
-conversions. I did my best to make the user interface obvious to use and tried
-to keep the functionality compatible with tools available to the average Civil
-engineer. ## Intro This repository was created in order for me to gain a better
-understanding of software development work flows and how they can be re-
-purposed for civil engineering related tasks. This is by no means a
-comprehensive or even functional repository but is more a way for me to track
-my progress while learning more about another industry. There may occasionally
-be how-tos and other code posted here but this repository is not meant as
-tutorial or in depth explanation for how coding works. For those types of
-things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or _S_t_a_c_k
-_O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
+Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Environment :: Console :: Curses
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
+Requires-Dist: Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
+coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
+selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
+PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
+sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
+Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
+geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
+Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
+requests>=2.28.2 Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist:
+pytest>=7.4.1 Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-
+Dist: matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0;
+extra == "full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full"
+Requires-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6;
+extra == "full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full"
+Requires-Dist: sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0;
+extra == "full" Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist:
+earthpy>=0.9.4; extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full"
+Requires-Dist: pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1;
+extra == "full" Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist:
+tox>=4.11.1; extra == "full" # CivilPy ![PyPI - License](https://
+img.shields.io/pypi/l/civilpy) [Project badge][PyPI - Python Version][Project
+badge]![PyPI - Downloads](https://img.shields.io/pypi/dm/CivilPy) Code snippets
+for Civil Engineering related tasks ## About (Skip to the "Installation"
+section to start running code) Welcome to the CivilPy repository. This is a
+simple software package to give civil engineers cleaner access to some of the
+packages from the python ecosystem. The package is focused on civil engineering
+related tasks such as file management, pdf data extraction, image manipulation
+mapping and unit conversions. I did my best to make the user interface obvious
+to use and tried to keep the functionality compatible with tools available to
+the average Civil engineer. ## Intro This repository was created in order for
+me to gain a better understanding of software development work flows and how
+they can be re-purposed for civil engineering related tasks. This is by no
+means a comprehensive or even functional repository but is more a way for me to
+track my progress while learning more about another industry. There may
+occasionally be how-tos and other code posted here but this repository is not
+meant as tutorial or in depth explanation for how coding works. For those types
+of things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or
+_S_t_a_c_k_ _O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
 _C_h_a_n_n_e_l for conceptual level programming lessons or _C_o_r_e_y_M_S_'_s_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l
 for lessons in practical uses of programming. For an interesting somewhat
 working examples see the files `Useful Tricks and Tools.ipynb` and `NBI
 STandards - Conversion` files to have a better understanding of what function
 the DOT/SNBI files are performing. ## Installation Run the following code to
 install the package: ```bash $ pip install civilpy ``` ## Usage to check the
 package installed correctly, run: ```python from civilpy.structural.steel
```

### Comparing `civilpy-0.0.77/README.md` & `civilpy-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/setup.py` & `civilpy-0.0.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.77',
+    version='0.0.78',
     packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
+    license='MIT',
     py_modules=[
         "civilpy.state.ohio.dot",
         "civilpy.state.ohio.snbi",
         "civilpy.general.database_tools",
         "civilpy.general.gis",
         "civilpy.general.kml_tools",
         "civilpy.general.math",
```

### Comparing `civilpy-0.0.77/src/civilpy/general/database_tools.py` & `civilpy-0.0.78/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/general/microstation.py` & `civilpy-0.0.78/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/general/photos.py` & `civilpy-0.0.78/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.78/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.78/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.78/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.78/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/structural/arema.py` & `civilpy-0.0.78/src/civilpy/structural/arema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from civilpy.structural.midas import get_elements_by_section_index, get_api_key, midas_api
 from civilpy.general import pint, units
 
-from civilpy.general import PrintColors
-from civilpy.structural.midas import analysis_results_request
+from src.civilpy.general import PrintColors
+from src.civilpy.structural.midas import analysis_results_request
 
 from pathlib import Path
 import pandas as pd
 import numpy as np
 import os
 
 future_ballast_depth = 6 * units('in')
```

### Comparing `civilpy-0.0.77/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.78/src/civilpy/structural/beam_bending.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         self.plot_bending_moment(ax4)
 
         return fig
 
     def plot_beam_diagram(self, ax=None):
         """Returns a schematic of the beam and all the loads applied on it.
         """
-        plot01_params = {'ylabel': "Beam loads", 'yunits': r'kN / m',
+        plot01_params = {'ylabel': "Beam loads", 'yunits': r'kip / ft',
                          # 'xlabel':"Beam axis", 'xunits':"m",
                          'color': "g",
                          'inverted': True}
         if ax is None:
             ax = plt.figure(figsize=(6, 2.5)).add_subplot(1, 1, 1)
         ax.set_title("Loaded beam diagram")
         self._plot_analytical(ax, sum(self._distributed_forces_y), **plot01_params)
```

### Comparing `civilpy-0.0.77/src/civilpy/structural/midas.py` & `civilpy-0.0.78/src/civilpy/structural/midas.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/structural/rail_tpg_design.py` & `civilpy-0.0.78/src/civilpy/structural/rail_tpg_design.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/structural/steel.py` & `civilpy-0.0.78/src/civilpy/structural/steel.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.78/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.78/src/civilpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.77
+Version: 0.0.78
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.77 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.78 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
-Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
-MIT License Classifier: Environment :: Console :: Curses Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: numpy>=1.14.5
-Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5 Requires-Dist:
-Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist: coverage>=7.1.0
-Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-selenium-
-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist: PyPDF2>=3.0.1
-Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist: sympy>=1.10.0 Requires-
-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0 Requires-Dist:
-icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist: geopandas>=0.6.2
-Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7 Requires-Dist:
-natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist: requests>=2.28.2
-Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2 Requires-Dist:
-tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist: pytest>=7.4.1
-Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-Dist:
-matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0; extra ==
-"full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full" Requires-
-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6; extra ==
-"full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full" Requires-Dist:
-sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0; extra == "full"
-Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist: earthpy>=0.9.4;
-extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full" Requires-Dist:
-pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1; extra == "full"
-Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist: tox>=4.11.1; extra
-== "full" # CivilPy ![PyPI - License](https://img.shields.io/pypi/l/civilpy)
-[Project badge][PyPI - Python Version][Project badge]![PyPI - Downloads](https:
-//img.shields.io/pypi/dm/CivilPy) Code snippets for Civil Engineering related
-tasks ## About (Skip to the "Installation" section to start running code)
-Welcome to the CivilPy repository. This is a simple software package to give
-civil engineers cleaner access to some of the packages from the python
-ecosystem. The package is focused on civil engineering related tasks such as
-file management, pdf data extraction, image manipulation mapping and unit
-conversions. I did my best to make the user interface obvious to use and tried
-to keep the functionality compatible with tools available to the average Civil
-engineer. ## Intro This repository was created in order for me to gain a better
-understanding of software development work flows and how they can be re-
-purposed for civil engineering related tasks. This is by no means a
-comprehensive or even functional repository but is more a way for me to track
-my progress while learning more about another industry. There may occasionally
-be how-tos and other code posted here but this repository is not meant as
-tutorial or in depth explanation for how coding works. For those types of
-things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or _S_t_a_c_k
-_O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
+Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Environment :: Console :: Curses
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
+Requires-Dist: Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
+coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
+selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
+PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
+sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
+Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
+geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
+Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
+requests>=2.28.2 Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist:
+pytest>=7.4.1 Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-
+Dist: matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0;
+extra == "full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full"
+Requires-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6;
+extra == "full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full"
+Requires-Dist: sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0;
+extra == "full" Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist:
+earthpy>=0.9.4; extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full"
+Requires-Dist: pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1;
+extra == "full" Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist:
+tox>=4.11.1; extra == "full" # CivilPy ![PyPI - License](https://
+img.shields.io/pypi/l/civilpy) [Project badge][PyPI - Python Version][Project
+badge]![PyPI - Downloads](https://img.shields.io/pypi/dm/CivilPy) Code snippets
+for Civil Engineering related tasks ## About (Skip to the "Installation"
+section to start running code) Welcome to the CivilPy repository. This is a
+simple software package to give civil engineers cleaner access to some of the
+packages from the python ecosystem. The package is focused on civil engineering
+related tasks such as file management, pdf data extraction, image manipulation
+mapping and unit conversions. I did my best to make the user interface obvious
+to use and tried to keep the functionality compatible with tools available to
+the average Civil engineer. ## Intro This repository was created in order for
+me to gain a better understanding of software development work flows and how
+they can be re-purposed for civil engineering related tasks. This is by no
+means a comprehensive or even functional repository but is more a way for me to
+track my progress while learning more about another industry. There may
+occasionally be how-tos and other code posted here but this repository is not
+meant as tutorial or in depth explanation for how coding works. For those types
+of things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or
+_S_t_a_c_k_ _O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
 _C_h_a_n_n_e_l for conceptual level programming lessons or _C_o_r_e_y_M_S_'_s_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l
 for lessons in practical uses of programming. For an interesting somewhat
 working examples see the files `Useful Tricks and Tools.ipynb` and `NBI
 STandards - Conversion` files to have a better understanding of what function
 the DOT/SNBI files are performing. ## Installation Run the following code to
 install the package: ```bash $ pip install civilpy ``` ## Usage to check the
 package installed correctly, run: ```python from civilpy.structural.steel
```

### Comparing `civilpy-0.0.77/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.78/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.77/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.78/src/civilpy.egg-info/requires.txt`

 * *Files identical despite different names*

