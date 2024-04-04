# Comparing `tmp/groups-local-0.0.8.tar.gz` & `tmp/groups-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groups-local-0.0.8.tar", last modified: Sun Mar 24 04:50:36 2024, max compression
+gzip compressed data, was "groups-local-0.0.9.tar", last modified: Fri Mar 29 13:21:41 2024, max compression
```

## Comparing `groups-local-0.0.8.tar` & `groups-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:50:36.923535 groups-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-24 04:50:36.923535 groups-local-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:50:36.919535 groups-local-0.0.8/groups_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:50:36.923535 groups-local-0.0.8/groups_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 04:50:13.000000 groups-local-0.0.8/groups_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-03-24 04:50:13.000000 groups-local-0.0.8/groups_local/src/groups_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-24 04:50:13.000000 groups-local-0.0.8/groups_local/src/groups_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:50:36.923535 groups-local-0.0.8/groups_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-24 04:50:36.000000 groups-local-0.0.8/groups_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-24 04:50:36.000000 groups-local-0.0.8/groups_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:50:36.000000 groups-local-0.0.8/groups_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-24 04:50:36.000000 groups-local-0.0.8/groups_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 04:50:36.000000 groups-local-0.0.8/groups_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-24 04:50:13.000000 groups-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:50:36.923535 groups-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-24 04:50:13.000000 groups-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:41.351167 groups-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 13:21:41.351167 groups-local-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:41.347167 groups-local-0.0.9/groups_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:41.351167 groups-local-0.0.9/groups_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:19.000000 groups-local-0.0.9/groups_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-03-29 13:21:19.000000 groups-local-0.0.9/groups_local/src/groups_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-29 13:21:19.000000 groups-local-0.0.9/groups_local/src/groups_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:41.351167 groups-local-0.0.9/groups_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 13:21:41.000000 groups-local-0.0.9/groups_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-29 13:21:41.000000 groups-local-0.0.9/groups_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:41.000000 groups-local-0.0.9/groups_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-29 13:21:41.000000 groups-local-0.0.9/groups_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 13:21:41.000000 groups-local-0.0.9/groups_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-29 13:21:19.000000 groups-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:41.351167 groups-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-29 13:21:19.000000 groups-local-0.0.9/setup.py
```

### Comparing `groups-local-0.0.8/PKG-INFO` & `groups-local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groups-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles groups-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `groups-local-0.0.8/groups_local/src/groups_local.py` & `groups-local-0.0.9/groups_local/src/groups_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
             )
             group_ml_ids_list = [group_ml_id]
         upsert_information = {
             "group_id": group_id,
             "group_ml_ids_list": group_ml_ids_list
         }
 
+        # TODO Shall we add upsert_informaiton to the logger.end()?
         logger.end(object={'group_id': group_id, 'group_ml_ids_list': group_ml_ids_list})
         return upsert_information
 
     def update_group(self, group_id: int, group_dict: Dict[str, any], lang_code: LangCode = None) -> None:
         logger.start(object={'group_id': group_id, 'data': str(group_dict)})
         group_data_json = {
             "name": group_dict.get('name'),
```

### Comparing `groups-local-0.0.8/groups_local/src/groups_local_constants.py` & `groups-local-0.0.9/groups_local/src/groups_local_constants.py`

 * *Files identical despite different names*

### Comparing `groups-local-0.0.8/groups_local.egg-info/PKG-INFO` & `groups-local-0.0.9/groups_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groups-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles groups-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `groups-local-0.0.8/setup.py` & `groups-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "groups-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/groups-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles groups-local Python",
     long_description="PyPI Package for Circles groups-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

