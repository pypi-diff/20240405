# Comparing `tmp/crosslab_soa_service_file-0.2.6.tar.gz` & `tmp/crosslab_soa_service_file-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_file-0.2.6.tar", last modified: Thu Feb  8 15:28:39 2024, max compression
+gzip compressed data, was "crosslab_soa_service_file-0.2.7.tar", last modified: Fri Apr  5 09:17:29 2024, max compression
```

## Comparing `crosslab_soa_service_file-0.2.6.tar` & `crosslab_soa_service_file-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      574 2024-02-08 15:28:39.504793 crosslab_soa_service_file-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      192 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2551 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/file_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      222 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/py.typed
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-02-08 15:28:39.000000 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2024-02-08 15:28:39.000000 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:28:39.000000 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-02-08 15:28:39.000000 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:28:39.000000 crosslab_soa_service_file-0.2.6/src/crosslab_soa_service_file.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:28:39.500793 crosslab_soa_service_file-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      898 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.6/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      574 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      192 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2551 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/file_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      222 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/py.typed
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:29.000000 crosslab_soa_service_file-0.2.7/src/crosslab_soa_service_file.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:29.974671 crosslab_soa_service_file-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      898 2023-11-08 12:05:40.000000 crosslab_soa_service_file-0.2.7/tests/test_standard.py
```

### Comparing `crosslab_soa_service_file-0.2.6/setup.cfg` & `crosslab_soa_service_file-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_file
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA file Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_file-0.2.6/src/crosslab/soa_services/file/file_service.py` & `crosslab_soa_service_file-0.2.7/src/crosslab/soa_services/file/file_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_file-0.2.6/tests/test_standard.py` & `crosslab_soa_service_file-0.2.7/tests/test_standard.py`

 * *Files identical despite different names*

