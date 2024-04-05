# Comparing `tmp/saphira-0.0.4.tar.gz` & `tmp/saphira-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.4.tar", last modified: Tue Apr  2 00:56:14 2024, max compression
+gzip compressed data, was "saphira-0.0.5.tar", last modified: Fri Apr  5 02:24:30 2024, max compression
```

## Comparing `saphira-0.0.4.tar` & `saphira-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-02 00:56:14.129373 saphira-0.0.4/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.4/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-02 00:56:14.127653 saphira-0.0.4/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.4/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-02 00:55:53.000000 saphira-0.0.4/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-02 00:56:14.129724 saphira-0.0.4/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-02 00:56:14.113009 saphira-0.0.4/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-02 00:56:14.115852 saphira-0.0.4/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-02 00:55:48.000000 saphira-0.0.4/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1914 2024-04-02 00:47:42.000000 saphira-0.0.4/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-02 00:56:14.125701 saphira-0.0.4/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-02 00:56:14.000000 saphira-0.0.4/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-02 00:56:14.000000 saphira-0.0.4/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-02 00:56:14.000000 saphira-0.0.4/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-02 00:56:14.000000 saphira-0.0.4/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-02 00:56:14.000000 saphira-0.0.4/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-02 00:56:14.124102 saphira-0.0.4/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1717 2024-04-02 00:37:44.000000 saphira-0.0.4/tests/test_battery_capacity.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.4/tests/test_jama_server.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.214252 saphira-0.0.5/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.5/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-05 02:24:30.213420 saphira-0.0.5/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.5/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-05 02:24:11.000000 saphira-0.0.5/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-05 02:24:30.214415 saphira-0.0.5/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.191949 saphira-0.0.5/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.196138 saphira-0.0.5/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-05 02:23:59.000000 saphira-0.0.5/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2040 2024-04-05 02:04:14.000000 saphira-0.0.5/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.211651 saphira-0.0.5/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.209679 saphira-0.0.5/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1845 2024-04-05 02:18:35.000000 saphira-0.0.5/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.5/tests/test_jama_server.py
```

### Comparing `saphira-0.0.4/LICENSE` & `saphira-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.4/PKG-INFO` & `saphira-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.4
+Version: 0.0.5
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.4/pyproject.toml` & `saphira-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.4"
+version = "0.0.5"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saphira-0.0.4/src/saphira/saphira.py` & `saphira-0.0.5/src/saphira/saphira.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,12 +37,14 @@
             t = multiprocessing.Process(target=loop)
             t.start()
         else:
             # TODO: Perform proper dependency tracing to also upload any other linked files and build a Pipfile for execution
             upload_url = f'{SAPHIRA_URL}/upload?project={datasource}&requirement={name}'
             stack = inspect.stack()
             dir_contents = os.listdir()
-            files = {f'file{i}': open(stack[1 + i].filename, 'rb') for i in range(len(stack) - 1) if stack[1 + i].filename in dir_contents}
+            files = {f'file{i}': open(stack[1 + i].filename, 'rb') for i in range(len(stack) - 1) if stack[1 + i].filename.split('/')[-1] in dir_contents}
             upload_resp = requests.post(upload_url, files=files)
             print(f"{upload_url} responded with status code {upload_resp.status_code}")
+            if upload_resp.status_code != 200:
+                print(f"Upload failed with {upload_resp.text}")
 
     return result
```

### Comparing `saphira-0.0.4/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.5/src/saphira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.4
+Version: 0.0.5
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.4/tests/test_battery_capacity.py` & `saphira-0.0.5/tests/test_battery_capacity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import unittest
-import os
-os.environ['SAPHIRA_URL'] = 'http://localhost:8081'
+# import os
+# os.environ['SAPHIRA_URL'] = 'http://localhost:8081'
 import requests
 import saphira
 
+PROJECT = '83092519-da63-4882-a899-297e3e62b65d.json'
+REQ = 'BattRef-0001'
+
 class BatteryCapacityTest(unittest.TestCase):
     def test_electric_range(self):
         energy_density = 250  # Wh/kg
-        minimum_range = int(saphira.get_param('83092519-da63-4882-a899-297e3e62b65d.json', 'BattRef-0001'))  # kilometers
+        minimum_range = int(saphira.get_param(PROJECT, REQ))  # kilometers
         print(minimum_range)
         efficiency_factor = 0.9  # Efficiency factor to account for losses
         
         # Assuming battery weight in kilograms
         battery_weight = minimum_range / (energy_density * efficiency_factor)
         
         # Calculate the minimum required battery capacity in kWh
@@ -23,11 +26,13 @@
         self.assertTrue(battery_weight < 500, "Battery weight should be reasonable (< 500 kg)")
         self.assertTrue(min_battery_capacity_kWh >= 225, "Minimum battery capacity should support at least 675 km range, is " + str(min_battery_capacity_kWh))
         self.assertTrue(min_battery_capacity_kWh <= 250, "Minimum battery capacity should not exceed required energy density")
 
 if __name__ == '__main__':
     try:
         unittest.main()
-        requests.post('http://localhost:8081/update_status', {'key': 'BattRef-0001', 'status': 'Validated'})
+        # TODO: Migrate to saphira package
+        resp = requests.post(f'{saphira.SAPHIRA_URL}/update_status', {'key': REQ, 'status': 'Validated', 'project': PROJECT})
+        print(resp.text)
     except:
-        resp = requests.post('http://localhost:8081/update_status', json={'key': 'BattRef-0001', 'status': 'Unvalidated'})
+        resp = requests.post(f'{saphira.SAPHIRA_URL}/update_status', json={'key': REQ, 'status': 'Unvalidated', 'project': PROJECT})
         print(resp.text)
```

### Comparing `saphira-0.0.4/tests/test_jama_server.py` & `saphira-0.0.5/tests/test_jama_server.py`

 * *Files identical despite different names*

