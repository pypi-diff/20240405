# Comparing `tmp/dustgoggles-0.7.4.tar.gz` & `tmp/dustgoggles-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustgoggles-0.7.4.tar", last modified: Tue Oct  3 20:39:53 2023, max compression
+gzip compressed data, was "dustgoggles-0.7.5.tar", last modified: Fri Apr  5 04:03:03 2024, max compression
```

## Comparing `dustgoggles-0.7.4.tar` & `dustgoggles-0.7.5.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-10-03 20:39:53.500585 dustgoggles-0.7.4/
--rw-r--r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/LICENSE
--rw-r--r--   0 sierra    (1000) sierra    (1000)      588 2023-10-03 20:39:53.496585 dustgoggles-0.7.4/PKG-INFO
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-10-03 20:39:53.496585 dustgoggles-0.7.4/dustgoggles/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       22 2023-10-03 20:38:18.000000 dustgoggles-0.7.4/dustgoggles/__init__.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-10-03 20:39:53.496585 dustgoggles-0.7.4/dustgoggles/codex/
--rw-r--r--   0 sierra    (1000) sierra    (1000)        0 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/codex/__init__.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3518 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/codex/_array_holding_area.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     5794 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/codex/codecs.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)    33342 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/codex/implements.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3351 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/codex/memutilz.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10599 2023-10-03 17:13:27.000000 dustgoggles-0.7.4/dustgoggles/composition.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6441 2023-10-03 17:13:27.000000 dustgoggles-0.7.4/dustgoggles/dynamic.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3738 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/func.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     5422 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/mosaic.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8901 2023-08-03 13:29:28.000000 dustgoggles-0.7.4/dustgoggles/pivot.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     4035 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/scrape.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)    13514 2023-05-30 13:53:39.000000 dustgoggles-0.7.4/dustgoggles/structures.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-10-03 20:39:53.496585 dustgoggles-0.7.4/dustgoggles/test_utils/
--rw-r--r--   0 sierra    (1000) sierra    (1000)       20 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/test_utils/__init__.py
--rw-r--r--   0 sierra    (1000) sierra    (1000)     2519 2023-05-30 13:48:19.000000 dustgoggles-0.7.4/dustgoggles/test_utils/core.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2653 2023-10-03 17:13:27.000000 dustgoggles-0.7.4/dustgoggles/tracker.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-10-03 20:39:53.496585 dustgoggles-0.7.4/dustgoggles.egg-info/
--rw-r--r--   0 sierra    (1000) sierra    (1000)      588 2023-10-03 20:39:53.000000 dustgoggles-0.7.4/dustgoggles.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      625 2023-10-03 20:39:53.000000 dustgoggles-0.7.4/dustgoggles.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-10-03 20:39:53.000000 dustgoggles-0.7.4/dustgoggles.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      102 2023-10-03 20:39:53.000000 dustgoggles-0.7.4/dustgoggles.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       12 2023-10-03 20:39:53.000000 dustgoggles-0.7.4/dustgoggles.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-10-03 20:39:53.500585 dustgoggles-0.7.4/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-10-03 20:32:21.000000 dustgoggles-0.7.4/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-04-05 04:03:03.740999 dustgoggles-0.7.5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1524 2022-03-27 01:26:54.000000 dustgoggles-0.7.5/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      588 2024-04-05 04:03:03.740999 dustgoggles-0.7.5/PKG-INFO
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-04-05 04:03:03.732999 dustgoggles-0.7.5/dustgoggles/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       22 2024-04-05 03:59:46.000000 dustgoggles-0.7.5/dustgoggles/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-10-20 19:34:46.000000 dustgoggles-0.7.5/dustgoggles/arg_scratch.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-04-05 04:03:03.736999 dustgoggles-0.7.5/dustgoggles/codex/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-04-23 02:19:26.000000 dustgoggles-0.7.5/dustgoggles/codex/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3518 2022-04-24 14:14:11.000000 dustgoggles-0.7.5/dustgoggles/codex/_array_holding_area.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5794 2022-06-12 19:14:57.000000 dustgoggles-0.7.5/dustgoggles/codex/codecs.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    33342 2022-06-12 19:14:57.000000 dustgoggles-0.7.5/dustgoggles/codex/implements.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28456 2022-06-01 04:16:49.000000 dustgoggles-0.7.5/dustgoggles/codex/implements_bak_scratch.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3351 2022-06-04 23:42:20.000000 dustgoggles-0.7.5/dustgoggles/codex/memutilz.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4103 2022-06-01 13:46:38.000000 dustgoggles-0.7.5/dustgoggles/codex_bounce_noreturn_scratch.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3740 2022-06-01 14:25:04.000000 dustgoggles-0.7.5/dustgoggles/codex_bounce_scratch.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10599 2023-09-29 19:14:25.000000 dustgoggles-0.7.5/dustgoggles/composition.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6574 2023-11-10 05:44:39.000000 dustgoggles-0.7.5/dustgoggles/dynamic.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3738 2023-05-09 18:50:18.000000 dustgoggles-0.7.5/dustgoggles/func.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5422 2023-02-09 17:53:03.000000 dustgoggles-0.7.5/dustgoggles/mosaic.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8923 2024-01-09 18:24:48.000000 dustgoggles-0.7.5/dustgoggles/pivot.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4035 2022-04-13 15:12:54.000000 dustgoggles-0.7.5/dustgoggles/scrape.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13514 2023-06-15 03:40:25.000000 dustgoggles-0.7.5/dustgoggles/structures.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-04-05 04:03:03.736999 dustgoggles-0.7.5/dustgoggles/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)       20 2022-04-13 15:12:54.000000 dustgoggles-0.7.5/dustgoggles/test_utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2519 2022-04-25 14:47:21.000000 dustgoggles-0.7.5/dustgoggles/test_utils/core.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2653 2023-09-29 19:52:36.000000 dustgoggles-0.7.5/dustgoggles/tracker.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-04-05 04:03:03.736999 dustgoggles-0.7.5/dustgoggles.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)      588 2024-04-05 04:03:03.000000 dustgoggles-0.7.5/dustgoggles.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      777 2024-04-05 04:03:03.000000 dustgoggles-0.7.5/dustgoggles.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2024-04-05 04:03:03.000000 dustgoggles-0.7.5/dustgoggles.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      102 2024-04-05 04:03:03.000000 dustgoggles-0.7.5/dustgoggles.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       12 2024-04-05 04:03:03.000000 dustgoggles-0.7.5/dustgoggles.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-04-05 04:03:03.740999 dustgoggles-0.7.5/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)      512 2024-04-05 03:59:25.000000 dustgoggles-0.7.5/setup.py
```

### Comparing `dustgoggles-0.7.4/LICENSE` & `dustgoggles-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/PKG-INFO` & `dustgoggles-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustgoggles
-Version: 0.7.4
+Version: 0.7.5
 Home-page: https://github.com/millionconcepts/dustgoggles.git
 Author: Million Concepts
 Author-email: mstclair@millionconcepts.com
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
```

### Comparing `dustgoggles-0.7.4/dustgoggles/codex/_array_holding_area.py` & `dustgoggles-0.7.5/dustgoggles/codex/_array_holding_area.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/codex/codecs.py` & `dustgoggles-0.7.5/dustgoggles/codex/codecs.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/codex/implements.py` & `dustgoggles-0.7.5/dustgoggles/codex/implements.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/codex/memutilz.py` & `dustgoggles-0.7.5/dustgoggles/codex/memutilz.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/composition.py` & `dustgoggles-0.7.5/dustgoggles/composition.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/dynamic.py` & `dustgoggles-0.7.5/dustgoggles/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,19 @@
         return {}
     tb = exc.__traceback__
     exc = exc if stringify_exception is False else f"{type(exc)}: {exc}"
     report = {'exception': exc, 'lineno': [], 'name': [], 'filename': []}
     while tb is not None:
         fr = tb.tb_frame
         if (module := getmodule(fr)) is not None:
-            report['name'].append(f'{module.__name__}.{fr.f_code.co_qualname}')
+            try:
+                codename = fr.f_code.co_qualname
+            except AttributeError:
+                codename = fr.f_code.co_name
+            report['name'].append(f'{module.__name__}.{codename}')
         else:
             report['name'].append(fr.f_code.co_name)
         report['lineno'].append(tb.tb_lineno)
         report['filename'].append(fr.f_code.co_filename)
         del fr  # taking excessive care here
         tb = tb.tb_next
     return report
```

### Comparing `dustgoggles-0.7.4/dustgoggles/func.py` & `dustgoggles-0.7.5/dustgoggles/func.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/mosaic.py` & `dustgoggles-0.7.5/dustgoggles/mosaic.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/pivot.py` & `dustgoggles-0.7.5/dustgoggles/pivot.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         constant_indices = pd.Series(False, df.columns)
     else:
         constant_indices = pd.Series(False, df.index)
     try:
         method = "iterrows" if how == "columns" else "items"
         for ix, series in getattr(df, method)():
             series = series if dropna is False else series.dropna()
-            if (series == series.iloc[0]).all():
+            if (len(series) == 0) or (series == series.iloc[0]).all():
                 constant_indices.loc[ix] = True
     except TypeError:
         # TODO: still necessary?
         if how == "columns":
             raise NotImplementedError("nested fields not supported columnwise")
         for c in df.columns:
             if isinstance(df[c].iloc[0], list):
```

### Comparing `dustgoggles-0.7.4/dustgoggles/scrape.py` & `dustgoggles-0.7.5/dustgoggles/scrape.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/structures.py` & `dustgoggles-0.7.5/dustgoggles/structures.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/test_utils/core.py` & `dustgoggles-0.7.5/dustgoggles/test_utils/core.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles/tracker.py` & `dustgoggles-0.7.5/dustgoggles/tracker.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.4/dustgoggles.egg-info/PKG-INFO` & `dustgoggles-0.7.5/dustgoggles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustgoggles
-Version: 0.7.4
+Version: 0.7.5
 Home-page: https://github.com/millionconcepts/dustgoggles.git
 Author: Million Concepts
 Author-email: mstclair@millionconcepts.com
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
```

### Comparing `dustgoggles-0.7.4/setup.py` & `dustgoggles-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dustgoggles",
-    version="0.7.4",
+    version="0.7.5",
     url="https://github.com/millionconcepts/dustgoggles.git",
     author="Million Concepts",
     author_email="mstclair@millionconcepts.com",
     packages=find_packages(),
     python_requires=">=3.9",
     install_requires=["cytoolz", "more-itertools"],
     extras_require={
```

