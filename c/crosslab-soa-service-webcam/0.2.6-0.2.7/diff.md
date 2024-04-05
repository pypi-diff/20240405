# Comparing `tmp/crosslab_soa_service_webcam-0.2.6.tar.gz` & `tmp/crosslab_soa_service_webcam-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_webcam-0.2.6.tar", last modified: Thu Feb  8 15:27:56 2024, max compression
+gzip compressed data, was "crosslab_soa_service_webcam-0.2.7.tar", last modified: Fri Apr  5 09:17:20 2024, max compression
```

## Comparing `crosslab_soa_service_webcam-0.2.6.tar` & `crosslab_soa_service_webcam-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      578 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1165 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/media.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      151 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/webcam_service.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2024-02-08 15:27:56.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2024-02-08 15:27:56.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:27:56.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-02-08 15:27:56.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:27:56.000000 crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:27:56.340611 crosslab_soa_service_webcam-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      668 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.6/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.766627 crosslab_soa_service_webcam-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2024-04-05 09:17:20.766627 crosslab_soa_service_webcam-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      578 2024-04-05 09:17:20.766627 crosslab_soa_service_webcam-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.762627 crosslab_soa_service_webcam-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.762627 crosslab_soa_service_webcam-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.762627 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.762627 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1165 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/media.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      151 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/webcam_service.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.766627 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2024-04-05 09:17:20.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2024-04-05 09:17:20.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:20.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:20.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:20.000000 crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:20.766627 crosslab_soa_service_webcam-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      668 2023-11-08 12:05:40.000000 crosslab_soa_service_webcam-0.2.7/tests/test_standard.py
```

### Comparing `crosslab_soa_service_webcam-0.2.6/setup.cfg` & `crosslab_soa_service_webcam-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_webcam
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Webcam Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/media.py` & `crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/media.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.6/src/crosslab/soa_services/webcam/webcam_service.py` & `crosslab_soa_service_webcam-0.2.7/src/crosslab/soa_services/webcam/webcam_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.6/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt` & `crosslab_soa_service_webcam-0.2.7/src/crosslab_soa_service_webcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_webcam-0.2.6/tests/test_standard.py` & `crosslab_soa_service_webcam-0.2.7/tests/test_standard.py`

 * *Files identical despite different names*

