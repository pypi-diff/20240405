# Comparing `tmp/flowpyter-task-1.1.3.post0.dev3.tar.gz` & `tmp/flowpyter-task-1.1.3.post0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowpyter-task-1.1.3.post0.dev3.tar", last modified: Thu Feb  1 12:44:36 2024, max compression
+gzip compressed data, was "flowpyter-task-1.1.3.post0.dev5.tar", last modified: Thu Apr  4 14:19:59 2024, max compression
```

## Comparing `flowpyter-task-1.1.3.post0.dev3.tar` & `flowpyter-task-1.1.3.post0.dev5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2297 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.721513 flowpyter-task-1.1.3.post0.dev3/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/flowpytertask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/plugins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/plugins/base64_jinja.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-01 12:44:36.725513 flowpyter-task-1.1.3.post0.dev3/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/tests/test_flowpyter_operator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7719 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/tests/test_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-02-01 12:44:36.000000 flowpyter-task-1.1.3.post0.dev3/versioneer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2297 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.179819 flowpyter-task-1.1.3.post0.dev5/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-04 14:19:59.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/flowpytertask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/plugins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/plugins/base64_jinja.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-04 14:19:59.183819 flowpyter-task-1.1.3.post0.dev5/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/tests/test_flowpyter_operator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7708 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/tests/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-04-04 14:19:58.000000 flowpyter-task-1.1.3.post0.dev5/versioneer.py
```

### Comparing `flowpyter-task-1.1.3.post0.dev3/LICENSE` & `flowpyter-task-1.1.3.post0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/PKG-INFO` & `flowpyter-task-1.1.3.post0.dev5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.3.post0.dev3
+Version: 1.1.3.post0.dev5
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `flowpyter-task-1.1.3.post0.dev3/README.md` & `flowpyter-task-1.1.3.post0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/setup.py` & `flowpyter-task-1.1.3.post0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/PKG-INFO` & `flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.3.post0.dev3
+Version: 1.1.3.post0.dev5
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `flowpyter-task-1.1.3.post0.dev3/src/flowpyter_task.egg-info/SOURCES.txt` & `flowpyter-task-1.1.3.post0.dev5/src/flowpyter_task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/src/flowpytertask/flowpytertask.py` & `flowpyter-task-1.1.3.post0.dev5/src/flowpytertask/flowpytertask.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/tests/test_flowpyter_operator.py` & `flowpyter-task-1.1.3.post0.dev5/tests/test_flowpyter_operator.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.3.post0.dev3/tests/test_integration.py` & `flowpyter-task-1.1.3.post0.dev5/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     out["HOST_DAGRUN_DATA_DIR"] = str(session_dagrun_data_dir)
     out["HOST_SHARED_DATA_DIR"] = str(session_shared_data_dir)
     out["HOST_DAGS_DIR"] = str(Path(__file__).parent / "dags")
     out["HOST_NOTEBOOK_DIR"] = str(Path(__file__).parent / "notebooks")
     out["HOST_TEMPLATES_DIR"] = str(Path(__file__).parent / "templates")
     out["HOST_STATIC_DIR"] = str(Path(__file__).parent / "static")
     out["NOTEBOOK_UID"] = str(os.getuid())
-    out["NOTEBOOK_GID"] = str(os.getgid())
+    out["NOTEBOOK_GID"] = "100"
     out["FLOWAPI_TOKEN"] = test_jwt_token
     yield out
 
 
 @pytest.fixture(scope="session")
 def tmp_env_file(tmp_env_vars, base_env_vars, tmp_path_factory):
     combined_vars = base_env_vars.copy()
```

### Comparing `flowpyter-task-1.1.3.post0.dev3/versioneer.py` & `flowpyter-task-1.1.3.post0.dev5/versioneer.py`

 * *Files identical despite different names*

