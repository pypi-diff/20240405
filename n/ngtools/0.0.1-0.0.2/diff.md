# Comparing `tmp/ngtools-0.0.1.tar.gz` & `tmp/ngtools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngtools-0.0.1.tar", last modified: Fri Apr  5 16:32:48 2024, max compression
+gzip compressed data, was "ngtools-0.0.2.tar", last modified: Fri Apr  5 19:51:47 2024, max compression
```

## Comparing `ngtools-0.0.1.tar` & `ngtools-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:32:48.790694 ngtools-0.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-05 16:32:40.000000 ngtools-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 16:32:48.790694 ngtools-0.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4820 2024-04-05 16:32:40.000000 ngtools-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:32:48.790694 ngtools-0.0.1/ngtools/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 16:32:48.790694 ngtools-0.0.1/ngtools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:32:48.790694 ngtools-0.0.1/ngtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:32:48.000000 ngtools-0.0.1/ngtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 16:32:40.000000 ngtools-0.0.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1207 2024-04-05 16:32:48.790694 ngtools-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-05 16:32:40.000000 ngtools-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-05 16:32:40.000000 ngtools-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-05 19:51:38.000000 ngtools-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 19:51:47.537914 ngtools-0.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4820 2024-04-05 19:51:38.000000 ngtools-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/ngtools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 19:51:47.541914 ngtools-0.0.2/ngtools/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   140462 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/cmdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14653 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/dandifs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      705 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/drawroi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/fileserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1832 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/nglocal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3572 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/opener.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13130 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/parserapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8131 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/shaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16603 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/spaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12225 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/tracts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2434 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1678 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64294 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17750 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/ngtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 19:51:38.000000 ngtools-0.0.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1207 2024-04-05 19:51:47.541914 ngtools-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-05 19:51:38.000000 ngtools-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-05 19:51:38.000000 ngtools-0.0.2/versioneer.py
```

### Comparing `ngtools-0.0.1/LICENSE` & `ngtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.1/PKG-INFO` & `ngtools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tracts visualization and annotation in neuroglancer
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: ybalbastre@mgh.harvard.edu
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/ngtools
 Project-URL: Homepage, https://github.com/balbasty/ngtools
```

### Comparing `ngtools-0.0.1/README.md` & `ngtools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.1/ngtools.egg-info/PKG-INFO` & `ngtools-0.0.2/ngtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tracts visualization and annotation in neuroglancer
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: ybalbastre@mgh.harvard.edu
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/ngtools
 Project-URL: Homepage, https://github.com/balbasty/ngtools
```

### Comparing `ngtools-0.0.1/setup.cfg` & `ngtools-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.1/setup.py` & `ngtools-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 except ImportError:
     # see https://github.com/warner/python-versioneer/issues/192
     print("WARNING: failed to import versioneer, "
           "falling back to no version for now")
     setup_kw = {}
 
 if __name__ == "__main__":
-    setup(name="ngtools", **setup_kw)
+    setup(packages=["ngtools"], **setup_kw)
```

### Comparing `ngtools-0.0.1/versioneer.py` & `ngtools-0.0.2/versioneer.py`

 * *Files identical despite different names*

