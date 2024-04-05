# Comparing `tmp/tracebloc_package-dev-0.5.8.tar.gz` & `tmp/tracebloc_package-dev-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.8.tar", last modified: Mon Aug 14 06:24:59 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.9.tar", last modified: Thu Aug 17 13:15:26 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.8.tar` & `tracebloc_package-dev-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-14 06:24:59.588038 tracebloc_package-dev-0.5.8/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.8/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-08-14 06:24:59.588144 tracebloc_package-dev-0.5.8/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.8/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-08-14 06:24:59.588482 tracebloc_package-dev-0.5.8/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-08-14 06:24:22.000000 tracebloc_package-dev-0.5.8/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-14 06:24:59.586472 tracebloc_package-dev-0.5.8/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-08-02 14:09:41.000000 tracebloc_package-dev-0.5.8/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.8/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    29608 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.8/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    58420 2023-08-14 06:22:57.000000 tracebloc_package-dev-0.5.8/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.8/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    11477 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.8/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-08-08 10:31:00.000000 tracebloc_package-dev-0.5.8/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6860 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.8/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.8/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-14 06:24:59.587843 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-08-14 06:24:59.000000 tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-17 13:15:26.794716 tracebloc_package-dev-0.5.9/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.9/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      558 2023-08-17 13:15:26.794782 tracebloc_package-dev-0.5.9/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.9/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-08-17 13:15:26.795100 tracebloc_package-dev-0.5.9/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-08-17 13:14:49.000000 tracebloc_package-dev-0.5.9/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-17 13:15:26.793720 tracebloc_package-dev-0.5.9/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-08-02 14:09:41.000000 tracebloc_package-dev-0.5.9/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.9/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    29608 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.9/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    58884 2023-08-17 13:13:10.000000 tracebloc_package-dev-0.5.9/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.9/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    11477 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.9/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-08-08 10:31:00.000000 tracebloc_package-dev-0.5.9/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     6860 2023-08-11 06:06:02.000000 tracebloc_package-dev-0.5.9/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.9/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-08-17 13:15:26.794603 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      558 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-08-17 13:15:26.000000 tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.8/LICENSE.txt` & `tracebloc_package-dev-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/PKG-INFO` & `tracebloc_package-dev-0.5.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.8
+Version: 0.5.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.8/setup.py` & `tracebloc_package-dev-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.8",
+    version="0.5.9",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,18 @@
         images = int(self.__total_images[edge_min])
         # check for no of batches
         if type(batchSize) == int:
             if images // batchSize < 3 and self.__framework == TENSORFLOW_FRAMEWORK:
                 error_msg = "Please choose smaller batch size as dataset selected have less images\n"
                 self.__print_error(error_msg)
                 return
+            elif batchSize < self.__num_classes:
+                error_msg = "Please choose higher batch size than num of classes in dataset provided\n"
+                self.__print_error(error_msg)
+                return
             self.__batchSize = batchSize
             self.__remove_error_method()
         else:
             error_msg = "Invalid input type given for batchSize\n"
             self.__print_error(error_msg)
 
     def __default_validation_split(self):
@@ -946,15 +950,19 @@
 
     def channel_shift_range(self, channel_shift_range: float):
         """
         Float. Range for random channel shifts.
         example: trainingObject.channel_shift_range(0.4)
         default: 0.0
         """
-        if type(channel_shift_range) == float:
+        if self.__framework == PYTORCH_FRAMEWORK and self.__image_type is not "rgb":
+            error_msg = "You can not set channel_shift_range if image type is not rgb\n"
+            self.__print_error(error_msg)
+            return None
+        elif type(channel_shift_range) == float:
             self.__channel_shift_range = channel_shift_range
             self.__remove_error_method()
         else:
             error_msg = "Invalid input type given for channel_shift_range\n"
             self.__print_error(error_msg)
 
     def fill_mode(self, fill_mode: str):
```

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.9/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.8
+Version: 0.5.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.8/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.9/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

