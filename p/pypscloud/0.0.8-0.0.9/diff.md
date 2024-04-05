# Comparing `tmp/pypscloud-0.0.8.tar.gz` & `tmp/pypscloud-0.0.9.tar.gz`

## Comparing `pypscloud-0.0.8.tar` & `pypscloud-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypscloud-0.0.8/build_pkg.ps1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypscloud-0.0.8/pypscloud/__ init __.py
--rw-r--r--   0        0        0    15640 2020-02-02 00:00:00.000000 pypscloud-0.0.8/pypscloud/pypscloud.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pypscloud-0.0.8/tests/main.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pypscloud-0.0.8/tests/test1.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 pypscloud-0.0.8/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pypscloud-0.0.8/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pypscloud-0.0.8/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pypscloud-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pypscloud-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypscloud-0.0.9/build_pkg.ps1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypscloud-0.0.9/pypscloud/__ init __.py
+-rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pypscloud-0.0.9/pypscloud/pypscloud.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pypscloud-0.0.9/tests/main.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypscloud-0.0.9/tests/test1.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 pypscloud-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pypscloud-0.0.9/LICENSE
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 pypscloud-0.0.9/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pypscloud-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pypscloud-0.0.9/PKG-INFO
```

### Comparing `pypscloud-0.0.8/pypscloud/pypscloud.py` & `pypscloud-0.0.9/pypscloud/pypscloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 global g_s3_data_bucket_upload
 global g_exec_t
 
 class PSCommon:
     def __init__(self, env):
         self.env = env
         ps_set_env(env)
-        self.set_working_dir('./tmp')
 
     def __str__(self):
         return  self.env
 
     def login(self):
         ps_login()
 
@@ -182,14 +181,15 @@
     if response.status_code == 200:
         accounts = response.json()
     else:
         print(response)
 
     return accounts
 
+
 def ps_get_all_mp_from_account(account):
     '''
     Measurement Point
     {'accountId': 252, 'accountName': 'Dominion Energy', 'partnerId': 252, 'partnerName': 'Dominion Energy', 'measurementPointId': 15802, 'measurementPointTypeId': 1, 'measurementPointStatusId': 8, 'measurementPointTypeName': 'QubeScan', 'measurementPointStatusName': 'commissioned', 'mainImageId': None, 'commissionedWhen': '2023-01-30T20:35:00.000Z', 'lastCommunicationTime': '2023-10-04T18:20:00.000Z', 'isLocked': 1, 'mpId': 'Afton Chemical 2.5', 'serialNumber': 'P3018306', 'pqubeModel': 'PQube3', 'notes': '', 'locationId': 1895, 'createdWhen': '2023-01-30T20:34:53.000Z', 'locationName': 'Afton Chemical', 'locationShortname': 'Afton Chemical', 'address1': '500 Spring Street', 'address2': '', 'city': 'Richmond', 'state': 'VA', 'zipCode': '23219', 'country': 'United States', 'latitude': 37.541115523, 'longitude': -77.44778955, 'siteInformation': None, 'timezone': 'America/New_York', 'summaryKpi': '#FF0000', 'acInputKpi': '#FF0000', 'psuKpi': '#4BB050', 'dcBusKpi': '#4BB050', 'acOutputKpi': '#4BB050', 'severeEventCount': 3}
     '''
     mps = []
     if type(account) is dict:
```

### Comparing `pypscloud-0.0.8/.gitignore` & `pypscloud-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pypscloud-0.0.8/LICENSE` & `pypscloud-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypscloud-0.0.8/pyproject.toml` & `pypscloud-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "pypscloud"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Louis Marchand", email="louis.marchand@powerside.com" },
 ]
 description = "Common wrappers and tools for the Powerside Cloud API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

