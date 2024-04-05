# Comparing `tmp/crosslab_soa_service_electrical-0.2.6.tar.gz` & `tmp/crosslab_soa_service_electrical-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_electrical-0.2.6.tar", last modified: Thu Feb  8 15:26:18 2024, max compression
+gzip compressed data, was "crosslab_soa_service_electrical-0.2.7.tar", last modified: Fri Apr  5 09:17:07 2024, max compression
```

## Comparing `crosslab_soa_service_electrical-0.2.6.tar` & `crosslab_soa_service_electrical-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      585 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      256 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5236 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/electrical_connection_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      745 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      614 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interface.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interfaces/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3001 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-02-08 15:26:18.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      770 2024-02-08 15:26:18.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-08 15:26:18.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-02-08 15:26:18.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-02-08 15:26:18.000000 crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-08 15:26:18.284196 crosslab_soa_service_electrical-0.2.6/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/tests/test_gpio.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.6/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      585 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      256 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5236 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/electrical_connection_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      745 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      614 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interface.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3001 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      770 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/tests/test_gpio.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/tests/test_standard.py
```

### Comparing `crosslab_soa_service_electrical-0.2.6/setup.cfg` & `crosslab_soa_service_electrical-0.2.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_electrical
-version = 0.2.6
+version = 0.2.7
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Electrical Service
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/electrical_connection_service.py` & `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/electrical_connection_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/messages.py` & `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interface.py` & `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interface.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py` & `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt` & `crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/tests/test_gpio.py` & `crosslab_soa_service_electrical-0.2.7/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.6/tests/test_standard.py` & `crosslab_soa_service_electrical-0.2.7/tests/test_standard.py`

 * *Files identical despite different names*

