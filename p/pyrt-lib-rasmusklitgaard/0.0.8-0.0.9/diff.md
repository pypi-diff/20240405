# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.0.8.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.0.9.tar.gz`

## Comparing `pyrt_lib_rasmusklitgaard-0.0.8.tar` & `pyrt_lib_rasmusklitgaard-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/__init__.py
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/helpers.py
--rw-r--r--   0        0        0    12165 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-r--r--   0        0        0    28088 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/patient.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/select_structures.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/.gitignore
--rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/LICENSE
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/README.md
--rwxr-xr-x   0        0        0     1041 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-r--r--   0        0        0    12165 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-r--r--   0        0        0    28088 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/patient.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/select_structures.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/LICENSE
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/README.md
+-rwxr-xr-x   0        0        0     1041 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrt_lib_rasmusklitgaard-0.0.9/PKG-INFO
```

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.0.9/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/LICENSE` & `pyrt_lib_rasmusklitgaard-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/README.md` & `pyrt_lib_rasmusklitgaard-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
-name = "pyrt-lib_rasmusklitgaard"
-version = "0.0.8"
+name = "pyrt_lib_rasmusklitgaard"
+version = "0.0.9"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.0.8/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyrt-lib_rasmusklitgaard
-Version: 0.0.8
+Name: pyrt_lib_rasmusklitgaard
+Version: 0.0.9
 Summary: PYthon RadioTherapy library
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

