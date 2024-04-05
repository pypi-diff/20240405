# Comparing `tmp/marqo-3.2.0.tar.gz` & `tmp/marqo-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-3.2.0.tar", last modified: Tue Mar 12 04:28:32 2024, max compression
+gzip compressed data, was "marqo-3.2.1.tar", last modified: Fri Apr  5 04:18:49 2024, max compression
```

## Comparing `marqo-3.2.0.tar` & `marqo-3.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:32.662626 marqo-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-12 04:28:26.000000 marqo-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-03-12 04:28:32.662626 marqo-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-03-12 04:28:26.000000 marqo-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-12 04:28:26.000000 marqo-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 04:28:32.662626 marqo-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-12 04:28:26.000000 marqo-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:32.654626 marqo-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:32.658626 marqo-3.2.0/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/cloud_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/default_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    35873 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/marqo_cloud_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/marqo_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:32.658626 marqo-3.2.0/src/marqo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/create_index_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/marqo_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/marqo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/marqo_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/models/search_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-12 04:28:26.000000 marqo-3.2.0/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:28:32.658626 marqo-3.2.0/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-03-12 04:28:32.000000 marqo-3.2.0/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-12 04:28:32.000000 marqo-3.2.0/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 04:28:32.000000 marqo-3.2.0/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-12 04:28:32.000000 marqo-3.2.0/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 04:28:32.000000 marqo-3.2.0/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.196438 marqo-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-05 04:18:40.000000 marqo-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-05 04:18:49.192438 marqo-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-05 04:18:40.000000 marqo-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 04:18:40.000000 marqo-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:18:49.196438 marqo-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 04:18:40.000000 marqo-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.188438 marqo-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/cloud_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/default_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35873 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/marqo_cloud_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/marqo_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/create_index_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/search_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-3.2.0/LICENSE` & `marqo-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/PKG-INFO` & `marqo-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.2.0
+Version: 3.2.1
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.2.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.2.1 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.2.0/README.md` & `marqo-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/setup.py` & `marqo-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="3.2.0",
+    version="3.2.1",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-3.2.0/src/marqo/_httprequests.py` & `marqo-3.2.1/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/client.py` & `marqo-3.2.1/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/cloud_helpers.py` & `marqo-3.2.1/src/marqo/cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/config.py` & `marqo-3.2.1/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/default_instance_mappings.py` & `marqo-3.2.1/src/marqo/default_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/errors.py` & `marqo-3.2.1/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/index.py` & `marqo-3.2.1/src/marqo/index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/instance_mappings.py` & `marqo-3.2.1/src/marqo/instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/marqo_cloud_instance_mappings.py` & `marqo-3.2.1/src/marqo/marqo_cloud_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/models/create_index_settings.py` & `marqo-3.2.1/src/marqo/models/create_index_settings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/models/marqo_cloud.py` & `marqo-3.2.1/src/marqo/models/marqo_cloud.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/models/marqo_index.py` & `marqo-3.2.1/src/marqo/models/marqo_index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/models/marqo_models.py` & `marqo-3.2.1/src/marqo/models/marqo_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/models/search_models.py` & `marqo-3.2.1/src/marqo/models/search_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/utils.py` & `marqo-3.2.1/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.0/src/marqo/version.py` & `marqo-3.2.1/src/marqo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__marqo_version__ = "2.3.0"
+__marqo_version__ = "2.4.0"
 __marqo_release_page__ = f"https://github.com/marqo-ai/marqo/releases/tag/{__marqo_version__}"
 
 __minimum_supported_marqo_version__ = "2.0"
 
 
 def supported_marqo_version() -> str:
     return f"This Marqo Python client is built for Marqo release ({__marqo_version__}) \n" \
```

### Comparing `marqo-3.2.0/src/marqo.egg-info/PKG-INFO` & `marqo-3.2.1/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.2.0
+Version: 3.2.1
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.2.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.2.1 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.2.0/src/marqo.egg-info/SOURCES.txt` & `marqo-3.2.1/src/marqo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

