# Comparing `tmp/utilities_dunningrb-0.8.1.tar.gz` & `tmp/utilities_dunningrb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilities_dunningrb-0.8.1.tar", last modified: Sat Mar  9 04:12:09 2024, max compression
+gzip compressed data, was "utilities_dunningrb-0.9.0.tar", last modified: Sun Mar 10 17:16:26 2024, max compression
```

## Comparing `utilities_dunningrb-0.8.1.tar` & `utilities_dunningrb-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-09 04:12:09.980576 utilities_dunningrb-0.8.1/
--rw-r--r--   0 rodneydunning   (501) staff       (20)      668 2024-03-09 04:12:09.979723 utilities_dunningrb-0.8.1/PKG-INFO
--rw-r--r--   0 rodneydunning   (501) staff       (20)      113 2024-02-02 20:19:29.000000 utilities_dunningrb-0.8.1/README.md
--rw-r--r--   0 rodneydunning   (501) staff       (20)      612 2024-03-09 04:12:03.000000 utilities_dunningrb-0.8.1/pyproject.toml
--rw-r--r--   0 rodneydunning   (501) staff       (20)       38 2024-03-09 04:12:09.980857 utilities_dunningrb-0.8.1/setup.cfg
-drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-09 04:12:09.974236 utilities_dunningrb-0.8.1/utilities/
--rw-r--r--   0 rodneydunning   (501) staff       (20)        0 2024-02-02 20:29:26.000000 utilities_dunningrb-0.8.1/utilities/__init__.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     1960 2024-02-26 22:34:03.000000 utilities_dunningrb-0.8.1/utilities/classutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     3066 2024-03-05 19:02:15.000000 utilities_dunningrb-0.8.1/utilities/dateutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     1755 2024-03-08 03:12:21.000000 utilities_dunningrb-0.8.1/utilities/decorators.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     6917 2024-02-18 00:36:22.000000 utilities_dunningrb-0.8.1/utilities/dictutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)      786 2024-02-02 19:45:12.000000 utilities_dunningrb-0.8.1/utilities/genutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)      451 2024-03-09 03:50:43.000000 utilities_dunningrb-0.8.1/utilities/gitutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     4468 2024-02-26 17:58:42.000000 utilities_dunningrb-0.8.1/utilities/listutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)    13165 2024-03-09 03:51:04.000000 utilities_dunningrb-0.8.1/utilities/mathutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     2981 2024-03-09 03:50:43.000000 utilities_dunningrb-0.8.1/utilities/pathutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     3118 2024-02-26 22:34:03.000000 utilities_dunningrb-0.8.1/utilities/pyplotutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)    22989 2024-03-09 04:11:44.000000 utilities_dunningrb-0.8.1/utilities/rwutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     3124 2024-02-26 22:34:03.000000 utilities_dunningrb-0.8.1/utilities/stringutils.py
--rw-r--r--   0 rodneydunning   (501) staff       (20)     2238 2024-02-02 19:50:33.000000 utilities_dunningrb-0.8.1/utilities/uiutils.py
-drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-09 04:12:09.978798 utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/
--rw-r--r--   0 rodneydunning   (501) staff       (20)      668 2024-03-09 04:12:09.000000 utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/PKG-INFO
--rw-r--r--   0 rodneydunning   (501) staff       (20)      517 2024-03-09 04:12:09.000000 utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/SOURCES.txt
--rw-r--r--   0 rodneydunning   (501) staff       (20)        1 2024-03-09 04:12:09.000000 utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/dependency_links.txt
--rw-r--r--   0 rodneydunning   (501) staff       (20)       10 2024-03-09 04:12:09.000000 utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/top_level.txt
+drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-10 17:16:26.940715 utilities_dunningrb-0.9.0/
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      668 2024-03-10 17:16:26.939203 utilities_dunningrb-0.9.0/PKG-INFO
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      113 2024-02-02 20:19:29.000000 utilities_dunningrb-0.9.0/README.md
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      612 2024-03-10 17:16:18.000000 utilities_dunningrb-0.9.0/pyproject.toml
+-rw-r--r--   0 rodneydunning   (501) staff       (20)       38 2024-03-10 17:16:26.941183 utilities_dunningrb-0.9.0/setup.cfg
+drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-10 17:16:26.929698 utilities_dunningrb-0.9.0/utilities/
+-rw-r--r--   0 rodneydunning   (501) staff       (20)        0 2024-02-02 20:29:26.000000 utilities_dunningrb-0.9.0/utilities/__init__.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     1960 2024-02-26 22:34:03.000000 utilities_dunningrb-0.9.0/utilities/classutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     3066 2024-03-05 19:02:15.000000 utilities_dunningrb-0.9.0/utilities/dateutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     1755 2024-03-08 03:12:21.000000 utilities_dunningrb-0.9.0/utilities/decorators.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     6917 2024-02-18 00:36:22.000000 utilities_dunningrb-0.9.0/utilities/dictutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      786 2024-02-02 19:45:12.000000 utilities_dunningrb-0.9.0/utilities/genutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      451 2024-03-09 03:50:43.000000 utilities_dunningrb-0.9.0/utilities/gitutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     4468 2024-02-26 17:58:42.000000 utilities_dunningrb-0.9.0/utilities/listutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)    13344 2024-03-10 17:15:56.000000 utilities_dunningrb-0.9.0/utilities/mathutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     2981 2024-03-09 03:50:43.000000 utilities_dunningrb-0.9.0/utilities/pathutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     3118 2024-02-26 22:34:03.000000 utilities_dunningrb-0.9.0/utilities/pyplotutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)    22989 2024-03-09 04:11:44.000000 utilities_dunningrb-0.9.0/utilities/rwutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     3124 2024-02-26 22:34:03.000000 utilities_dunningrb-0.9.0/utilities/stringutils.py
+-rw-r--r--   0 rodneydunning   (501) staff       (20)     2238 2024-02-02 19:50:33.000000 utilities_dunningrb-0.9.0/utilities/uiutils.py
+drwxr-xr-x   0 rodneydunning   (501) staff       (20)        0 2024-03-10 17:16:26.937774 utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      668 2024-03-10 17:16:26.000000 utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/PKG-INFO
+-rw-r--r--   0 rodneydunning   (501) staff       (20)      517 2024-03-10 17:16:26.000000 utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/SOURCES.txt
+-rw-r--r--   0 rodneydunning   (501) staff       (20)        1 2024-03-10 17:16:26.000000 utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/dependency_links.txt
+-rw-r--r--   0 rodneydunning   (501) staff       (20)       10 2024-03-10 17:16:26.000000 utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/top_level.txt
```

### Comparing `utilities_dunningrb-0.8.1/PKG-INFO` & `utilities_dunningrb-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities_dunningrb
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library of utility modules.
 Author-email: Rodney Dunning <dunningrb@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/dunningrb/utilities
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `utilities_dunningrb-0.8.1/pyproject.toml` & `utilities_dunningrb-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "utilities_dunningrb"
-version = "0.8.1"
+version = "0.9.0"
 authors = [
   { name="Rodney Dunning", email="dunningrb@gmail.com" },
 ]
 description = "A library of utility modules."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `utilities_dunningrb-0.8.1/utilities/classutils.py` & `utilities_dunningrb-0.9.0/utilities/classutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/dateutils.py` & `utilities_dunningrb-0.9.0/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/decorators.py` & `utilities_dunningrb-0.9.0/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/dictutils.py` & `utilities_dunningrb-0.9.0/utilities/dictutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/genutils.py` & `utilities_dunningrb-0.9.0/utilities/genutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/listutils.py` & `utilities_dunningrb-0.9.0/utilities/listutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/mathutils.py` & `utilities_dunningrb-0.9.0/utilities/mathutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,20 @@
 def get_random_number_list(size: int) -> list[float]:
     """Return a list of random numbers each in the range [0, 1]. Makes a call to get_random_number,
     which see.
     """
     return [get_random_number() for _ in range(size)]
 
 
+def get_transpose(m: list[list]) -> list[list]:
+    """Return the transpose of the given matrix.
+    """
+    return [[m[j][i] for j in range(len(m))] for i in range(len(m[0]))]
+
+
 def get_zscore_from_pvalue(p: float) -> float:
     """Given a p-value return the z-score.
     """
     return statistics.NormalDist().inv_cdf((1 + p) / 2.0)
 
 
 def is_normalized(table: dict, *, tol: float = 1e-5) -> bool:
```

### Comparing `utilities_dunningrb-0.8.1/utilities/pathutils.py` & `utilities_dunningrb-0.9.0/utilities/pathutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/pyplotutils.py` & `utilities_dunningrb-0.9.0/utilities/pyplotutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/rwutils.py` & `utilities_dunningrb-0.9.0/utilities/rwutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/stringutils.py` & `utilities_dunningrb-0.9.0/utilities/stringutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities/uiutils.py` & `utilities_dunningrb-0.9.0/utilities/uiutils.py`

 * *Files identical despite different names*

### Comparing `utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/PKG-INFO` & `utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities_dunningrb
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library of utility modules.
 Author-email: Rodney Dunning <dunningrb@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/dunningrb/utilities
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `utilities_dunningrb-0.8.1/utilities_dunningrb.egg-info/SOURCES.txt` & `utilities_dunningrb-0.9.0/utilities_dunningrb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

