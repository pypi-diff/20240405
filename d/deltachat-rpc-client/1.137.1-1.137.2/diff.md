# Comparing `tmp/deltachat-rpc-client-1.137.1.tar.gz` & `tmp/deltachat-rpc-client-1.137.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-client-1.137.1.tar", last modified: Wed Apr  3 01:31:29 2024, max compression
+gzip compressed data, was "deltachat-rpc-client-1.137.2.tar", last modified: Fri Apr  5 14:31:43 2024, max compression
```

## Comparing `deltachat-rpc-client-1.137.1.tar` & `deltachat-rpc-client-1.137.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:31:29.445455 deltachat-rpc-client-1.137.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-03 01:31:29.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-03 01:31:29.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:31:29.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 01:31:29.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 01:31:29.000000 deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:31:29.449455 deltachat-rpc-client-1.137.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-03 01:31:21.000000 deltachat-rpc-client-1.137.1/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.432152 deltachat-rpc-client-1.137.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_webxdc.py
```

### Comparing `deltachat-rpc-client-1.137.1/LICENSE` & `deltachat-rpc-client-1.137.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/PKG-INFO` & `deltachat-rpc-client-1.137.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.1
+Version: 1.137.2
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat-rpc-client-1.137.1/README.md` & `deltachat-rpc-client-1.137.2/README.md`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/pyproject.toml` & `deltachat-rpc-client-1.137.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.137.1"
+version = "1.137.2"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/__init__.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/_utils.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/account.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/account.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/chat.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/client.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/const.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/contact.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/deltachat.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/events.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/message.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/pytestplugin.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client/rpc.py` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.1
+Version: 1.137.2
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat-rpc-client-1.137.1/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/tests/test_securejoin.py` & `deltachat-rpc-client-1.137.2/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/tests/test_something.py` & `deltachat-rpc-client-1.137.2/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.1/tests/test_webxdc.py` & `deltachat-rpc-client-1.137.2/tests/test_webxdc.py`

 * *Files identical despite different names*

