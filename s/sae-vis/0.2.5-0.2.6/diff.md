# Comparing `tmp/sae-vis-0.2.5.tar.gz` & `tmp/sae-vis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae-vis-0.2.5.tar", last modified: Mon Apr  1 10:11:25 2024, max compression
+gzip compressed data, was "sae-vis-0.2.6.tar", last modified: Fri Apr  5 11:44:23 2024, max compression
```

## Comparing `sae-vis-0.2.5.tar` & `sae-vis-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.310586 sae-vis-0.2.5/
--rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      361 2024-04-01 10:11:25.310586 sae-vis-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.245586 sae-vis-0.2.5/sae_vis/
--rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.5/sae_vis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.279586 sae-vis-0.2.5/sae_vis/__pycache__/
--rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.5/sae_vis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    23307 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
--rw-rw-rw-   0        0        0    48089 2024-03-31 11:17:20.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    57756 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13155 2024-03-30 20:39:51.000000 sae-vis-0.2.5/sae_vis/__pycache__/html_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13355 2024-03-30 10:24:03.000000 sae-vis-0.2.5/sae_vis/__pycache__/model_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    46162 2024-03-31 15:33:46.000000 sae-vis-0.2.5/sae_vis/__pycache__/utils_fns.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.283586 sae-vis-0.2.5/sae_vis/css/
--rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.5/sae_vis/css/dropdown.css
--rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.5/sae_vis/css/general.css
--rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.5/sae_vis/css/sequences.css
--rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.5/sae_vis/css/tables.css
--rw-rw-rw-   0        0        0    17143 2024-03-30 20:16:23.000000 sae-vis-0.2.5/sae_vis/data_config_classes.py
--rw-rw-rw-   0        0        0    47062 2024-03-31 11:16:12.000000 sae-vis-0.2.5/sae_vis/data_fetching_fns.py
--rw-rw-rw-   0        0        0    50059 2024-03-30 20:35:07.000000 sae-vis-0.2.5/sae_vis/data_storing_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.290587 sae-vis-0.2.5/sae_vis/html/
--rw-rw-rw-   0        0        0      137 2024-03-17 17:41:09.000000 sae-vis-0.2.5/sae_vis/html/acts_histogram_template.html
--rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.5/sae_vis/html/feature_tables_template.html
--rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.5/sae_vis/html/logits_histogram_template.html
--rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.5/sae_vis/html/logits_table_template.html
--rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.5/sae_vis/html/sequences_group_template.html
--rw-rw-rw-   0        0        0    13674 2024-04-01 09:31:33.000000 sae-vis-0.2.5/sae_vis/html_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.309586 sae-vis-0.2.5/sae_vis/js/
--rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.5/sae_vis/js/_createDropdownsScript.js
--rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.5/sae_vis/js/actsHistogramScript.js
--rw-rw-rw-   0        0        0     2961 2024-03-17 16:48:44.000000 sae-vis-0.2.5/sae_vis/js/featureTablesScript.js
--rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.5/sae_vis/js/gridColumnTitlesScript.js
--rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.5/sae_vis/js/logitsHistogramScript.js
--rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.5/sae_vis/js/logitsTableScript.js
--rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.5/sae_vis/js/tokenScript.js
--rw-rw-rw-   0        0        0     8967 2024-04-01 10:10:41.000000 sae-vis-0.2.5/sae_vis/model_fns.py
--rw-rw-rw-   0        0        0    34980 2024-03-31 15:17:59.000000 sae-vis-0.2.5/sae_vis/utils_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:11:25.268605 sae-vis-0.2.5/sae_vis.egg-info/
--rw-rw-rw-   0        0        0      361 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 10:11:25.000000 sae-vis-0.2.5/sae_vis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 10:11:25.310586 sae-vis-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      849 2024-04-01 10:11:14.000000 sae-vis-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.802348 sae-vis-0.2.6/
+-rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      361 2024-04-05 11:44:23.802348 sae-vis-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.599927 sae-vis-0.2.6/sae_vis/
+-rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.6/sae_vis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.640377 sae-vis-0.2.6/sae_vis/__pycache__/
+-rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.6/sae_vis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23307 2024-03-30 20:39:51.000000 sae-vis-0.2.6/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
+-rw-rw-rw-   0        0        0    48089 2024-03-31 11:17:20.000000 sae-vis-0.2.6/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    57756 2024-03-30 20:39:51.000000 sae-vis-0.2.6/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13155 2024-03-30 20:39:51.000000 sae-vis-0.2.6/sae_vis/__pycache__/html_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13355 2024-03-30 10:24:03.000000 sae-vis-0.2.6/sae_vis/__pycache__/model_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    46162 2024-03-31 15:33:46.000000 sae-vis-0.2.6/sae_vis/__pycache__/utils_fns.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.672745 sae-vis-0.2.6/sae_vis/css/
+-rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.6/sae_vis/css/dropdown.css
+-rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.6/sae_vis/css/general.css
+-rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.6/sae_vis/css/sequences.css
+-rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.6/sae_vis/css/tables.css
+-rw-rw-rw-   0        0        0    17143 2024-03-30 20:16:23.000000 sae-vis-0.2.6/sae_vis/data_config_classes.py
+-rw-rw-rw-   0        0        0    47062 2024-03-31 11:16:12.000000 sae-vis-0.2.6/sae_vis/data_fetching_fns.py
+-rw-rw-rw-   0        0        0    50059 2024-03-30 20:35:07.000000 sae-vis-0.2.6/sae_vis/data_storing_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.713458 sae-vis-0.2.6/sae_vis/html/
+-rw-rw-rw-   0        0        0      137 2024-03-17 17:41:09.000000 sae-vis-0.2.6/sae_vis/html/acts_histogram_template.html
+-rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.6/sae_vis/html/feature_tables_template.html
+-rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.6/sae_vis/html/logits_histogram_template.html
+-rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.6/sae_vis/html/logits_table_template.html
+-rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.6/sae_vis/html/sequences_group_template.html
+-rw-rw-rw-   0        0        0    13674 2024-04-01 09:31:33.000000 sae-vis-0.2.6/sae_vis/html_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.794351 sae-vis-0.2.6/sae_vis/js/
+-rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.6/sae_vis/js/_createDropdownsScript.js
+-rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.6/sae_vis/js/actsHistogramScript.js
+-rw-rw-rw-   0        0        0     2961 2024-03-17 16:48:44.000000 sae-vis-0.2.6/sae_vis/js/featureTablesScript.js
+-rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.6/sae_vis/js/gridColumnTitlesScript.js
+-rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.6/sae_vis/js/logitsHistogramScript.js
+-rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.6/sae_vis/js/logitsTableScript.js
+-rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.6/sae_vis/js/tokenScript.js
+-rw-rw-rw-   0        0        0     8967 2024-04-01 10:10:41.000000 sae-vis-0.2.6/sae_vis/model_fns.py
+-rw-rw-rw-   0        0        0    34976 2024-04-05 11:44:02.000000 sae-vis-0.2.6/sae_vis/utils_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:44:23.624363 sae-vis-0.2.6/sae_vis.egg-info/
+-rw-rw-rw-   0        0        0      361 2024-04-05 11:44:23.000000 sae-vis-0.2.6/sae_vis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2024-04-05 11:44:23.000000 sae-vis-0.2.6/sae_vis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:44:23.000000 sae-vis-0.2.6/sae_vis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-05 11:44:23.000000 sae-vis-0.2.6/sae_vis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 11:44:23.000000 sae-vis-0.2.6/sae_vis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:44:23.802348 sae-vis-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      849 2024-04-05 11:44:12.000000 sae-vis-0.2.6/setup.py
```

### Comparing `sae-vis-0.2.5/README.md` & `sae-vis-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/data_config_classes.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/data_config_classes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/html_fns.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/html_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/model_fns.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/model_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/__pycache__/utils_fns.cpython-311.pyc` & `sae-vis-0.2.6/sae_vis/__pycache__/utils_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/css/dropdown.css` & `sae-vis-0.2.6/sae_vis/css/dropdown.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/css/general.css` & `sae-vis-0.2.6/sae_vis/css/general.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/css/sequences.css` & `sae-vis-0.2.6/sae_vis/css/sequences.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/css/tables.css` & `sae-vis-0.2.6/sae_vis/css/tables.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/data_config_classes.py` & `sae-vis-0.2.6/sae_vis/data_config_classes.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/data_fetching_fns.py` & `sae-vis-0.2.6/sae_vis/data_fetching_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/data_storing_fns.py` & `sae-vis-0.2.6/sae_vis/data_storing_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/html_fns.py` & `sae-vis-0.2.6/sae_vis/html_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/_createDropdownsScript.js` & `sae-vis-0.2.6/sae_vis/js/_createDropdownsScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/actsHistogramScript.js` & `sae-vis-0.2.6/sae_vis/js/actsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/featureTablesScript.js` & `sae-vis-0.2.6/sae_vis/js/featureTablesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/gridColumnTitlesScript.js` & `sae-vis-0.2.6/sae_vis/js/gridColumnTitlesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/logitsHistogramScript.js` & `sae-vis-0.2.6/sae_vis/js/logitsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/logitsTableScript.js` & `sae-vis-0.2.6/sae_vis/js/logitsTableScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/js/tokenScript.js` & `sae-vis-0.2.6/sae_vis/js/tokenScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/model_fns.py` & `sae-vis-0.2.6/sae_vis/model_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/sae_vis/utils_fns.py` & `sae-vis-0.2.6/sae_vis/utils_fns.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
     "(": "&#40;",
     "[": "&#91;",
     "]": "&#93;",
     "{": "&#123;",
     "}": "&#125;",
 }
 HTML_ANOMALIES = {
-    # "âĢĶ": "&ndash;",
-    # "âĢĻ": "&rsquo;",
+    "âĢĶ": "&ndash;",
+    "âĢĻ": "&rsquo;",
     "âĢĭ": "&#8203;",
     "Ġ": "&nbsp;",
     "Ċ": "&bsol;n",
     "ĉ": "&bsol;t",
 }
 HTML_QUOTES = {
     "'": "&apos;",
```

### Comparing `sae-vis-0.2.5/sae_vis.egg-info/SOURCES.txt` & `sae-vis-0.2.6/sae_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.5/setup.py` & `sae-vis-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sae-vis',
-    version = '0.2.5',
+    version = '0.2.6',
     packages = find_packages(),
     install_requires = [
         'torch',
         'einops',
         'datasets',
         'dataclasses-json',
         'jaxtyping',
```

