# Comparing `tmp/fave_measurement_point-0.1.1.tar.gz` & `tmp/fave_measurement_point-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fave_measurement_point-0.1.1.tar", max compression
+gzip compressed data, was "fave_measurement_point-0.1.2.tar", max compression
```

## Comparing `fave_measurement_point-0.1.1.tar` & `fave_measurement_point-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-04 15:12:45.453135 fave_measurement_point-0.1.1/LICENSE
--rw-r--r--   0        0        0      101 2024-04-04 15:12:45.453270 fave_measurement_point-0.1.1/README.md
--rw-r--r--   0        0        0      629 2024-04-05 16:08:23.132212 fave_measurement_point-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 15:23:27.622070 fave_measurement_point-0.1.1/src/fave_measurement_point/__init__.py
--rw-r--r--   0        0        0     6447 2024-04-05 16:07:35.588223 fave_measurement_point-0.1.1/src/fave_measurement_point/formants.py
--rw-r--r--   0        0        0     3744 2024-04-05 15:27:41.270812 fave_measurement_point-0.1.1/src/fave_measurement_point/heuristic.py
--rw-r--r--   0        0        0     3027 2024-04-05 15:20:21.533479 fave_measurement_point-0.1.1/src/fave_measurement_point/processor.py
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 fave_measurement_point-0.1.1/setup.py
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 fave_measurement_point-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-04 15:12:45.453135 fave_measurement_point-0.1.2/LICENSE
+-rw-r--r--   0        0        0      101 2024-04-04 15:12:45.453270 fave_measurement_point-0.1.2/README.md
+-rw-r--r--   0        0        0      629 2024-04-05 16:12:12.206101 fave_measurement_point-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 15:23:27.622070 fave_measurement_point-0.1.2/src/fave_measurement_point/__init__.py
+-rw-r--r--   0        0        0     6443 2024-04-05 16:11:53.865566 fave_measurement_point-0.1.2/src/fave_measurement_point/formants.py
+-rw-r--r--   0        0        0     3744 2024-04-05 15:27:41.270812 fave_measurement_point-0.1.2/src/fave_measurement_point/heuristic.py
+-rw-r--r--   0        0        0     3027 2024-04-05 15:20:21.533479 fave_measurement_point-0.1.2/src/fave_measurement_point/processor.py
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 fave_measurement_point-0.1.2/setup.py
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 fave_measurement_point-0.1.2/PKG-INFO
```

### Comparing `fave_measurement_point-0.1.1/LICENSE` & `fave_measurement_point-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fave_measurement_point-0.1.1/pyproject.toml` & `fave_measurement_point-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fave-measurement-point"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library for defining and evaluating formant measurement point heuristics."
 authors = ["JoFrhwld <JoFrhwld@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "fave_measurement_point", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fave_measurement_point-0.1.1/src/fave_measurement_point/formants.py` & `fave_measurement_point-0.1.2/src/fave_measurement_point/formants.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             The shape of the formant
         max (Point):
             A Point for the formant maximum
         min (Point):
             A Point for the formant minimum
     """
     track: NDArray
-    time: NDArray = field(default_factory=lambda x: np.array([]))
+    time: NDArray = field(default_factory=lambda: np.array([]))
 
     def __post_init__(self):
         if self.time.size == 0:
             idx_time = np.arange(self.track.size)
             self.time = idx_time/idx_time.max()
         
         self.rel_time = self.time - self.time.min()
@@ -137,15 +137,15 @@
         prop_time:
             The proportional time domain
         f[1, 2, 3, ...] (np.array):
             Specific formant tracks.
 
     """
     array: NDArray
-    time: NDArray = field(default_factory=lambda x: np.array([]))
+    time: NDArray = field(default_factory=lambda: np.array([]))
 
     def __post_init__(self):
         if self.time.size == 0:
             idx_time = np.arange(self.array.shape[1])
             self.time = idx_time/idx_time.max()
         
         assert self.time.size == self.array.shape[1], \
```

### Comparing `fave_measurement_point-0.1.1/src/fave_measurement_point/heuristic.py` & `fave_measurement_point-0.1.2/src/fave_measurement_point/heuristic.py`

 * *Files identical despite different names*

### Comparing `fave_measurement_point-0.1.1/src/fave_measurement_point/processor.py` & `fave_measurement_point-0.1.2/src/fave_measurement_point/processor.py`

 * *Files identical despite different names*

### Comparing `fave_measurement_point-0.1.1/setup.py` & `fave_measurement_point-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['nptyping>=2.5.0,<3.0.0', 'numpy>=1.26.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'fave-measurement-point',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A library for defining and evaluating formant measurement point heuristics.',
     'long_description': '# fave-measurement-point\nA library for defining and evaluating formant measurement point heuristics.\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fave_measurement_point-0.1.1/PKG-INFO` & `fave_measurement_point-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fave-measurement-point
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for defining and evaluating formant measurement point heuristics.
 License: GPLv3
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

