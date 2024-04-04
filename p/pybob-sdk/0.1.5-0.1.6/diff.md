# Comparing `tmp/pybob_sdk-0.1.5.tar.gz` & `tmp/pybob_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybob_sdk-0.1.5.tar", max compression
+gzip compressed data, was "pybob_sdk-0.1.6.tar", max compression
```

## Comparing `pybob_sdk-0.1.5.tar` & `pybob_sdk-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1091 2024-03-29 14:24:07.195425 pybob_sdk-0.1.5/LICENCE.md
--rw-r--r--   0        0        0     1529 2024-03-30 19:12:40.256434 pybob_sdk-0.1.5/README.md
--rw-r--r--   0        0        0       21 2024-03-30 19:00:08.784442 pybob_sdk-0.1.5/pybob_sdk/__init__.py
--rw-r--r--   0        0        0     2067 2024-03-30 18:52:09.612447 pybob_sdk-0.1.5/pybob_sdk/bob.py
--rw-r--r--   0        0        0     2928 2024-03-30 19:00:08.904442 pybob_sdk-0.1.5/pybob_sdk/bob_client.py
--rw-r--r--   0        0        0        0 2024-03-29 14:51:46.611408 pybob_sdk-0.1.5/pybob_sdk/v1/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-30 18:14:24.360470 pybob_sdk-0.1.5/pybob_sdk/v1/attendance.py
--rw-r--r--   0        0        0       80 2024-03-30 18:14:24.356470 pybob_sdk-0.1.5/pybob_sdk/v1/base.py
--rw-r--r--   0        0        0       24 2024-03-30 18:14:24.356470 pybob_sdk-0.1.5/pybob_sdk/v1/company.py
--rw-r--r--   0        0        0     4239 2024-03-30 18:14:24.532470 pybob_sdk-0.1.5/pybob_sdk/v1/documents.py
--rw-r--r--   0        0        0     2026 2024-03-30 18:14:24.444470 pybob_sdk-0.1.5/pybob_sdk/v1/hiring.py
--rw-r--r--   0        0        0     7125 2024-03-30 18:55:26.596445 pybob_sdk-0.1.5/pybob_sdk/v1/metadata.py
--rw-r--r--   0        0        0      231 2024-03-30 18:14:24.212470 pybob_sdk-0.1.5/pybob_sdk/v1/models/Bob.py
--rw-r--r--   0        0        0      537 2024-03-30 18:14:24.268470 pybob_sdk-0.1.5/pybob_sdk/v1/models/Metadata.py
--rw-r--r--   0        0        0      682 2024-03-30 18:14:24.316470 pybob_sdk-0.1.5/pybob_sdk/v1/models/Payroll.py
--rw-r--r--   0        0        0      802 2024-03-30 18:14:24.324470 pybob_sdk-0.1.5/pybob_sdk/v1/models/People.py
--rw-r--r--   0        0        0      138 2024-03-30 18:14:24.328470 pybob_sdk-0.1.5/pybob_sdk/v1/models/Reports.py
--rw-r--r--   0        0        0      497 2024-03-30 18:14:24.352470 pybob_sdk-0.1.5/pybob_sdk/v1/models/Tasks.py
--rw-r--r--   0        0        0        0 2024-03-29 14:51:49.343408 pybob_sdk-0.1.5/pybob_sdk/v1/models/__init__.py
--rw-r--r--   0        0        0      908 2024-03-30 18:14:24.548470 pybob_sdk-0.1.5/pybob_sdk/v1/objects.py
--rw-r--r--   0        0        0      238 2024-03-30 18:14:24.556470 pybob_sdk-0.1.5/pybob_sdk/v1/onboarding.py
--rw-r--r--   0        0        0      770 2024-03-30 18:14:24.576470 pybob_sdk-0.1.5/pybob_sdk/v1/payroll.py
--rw-r--r--   0        0        0    36350 2024-03-30 18:55:33.020445 pybob_sdk-0.1.5/pybob_sdk/v1/people.py
--rw-r--r--   0        0        0     3963 2024-03-30 18:55:36.240445 pybob_sdk-0.1.5/pybob_sdk/v1/reports.py
--rw-r--r--   0        0        0     3386 2024-03-30 18:14:24.752470 pybob_sdk-0.1.5/pybob_sdk/v1/tables.py
--rw-r--r--   0        0        0     2776 2024-03-30 18:55:38.484445 pybob_sdk-0.1.5/pybob_sdk/v1/tasks.py
--rw-r--r--   0        0        0    17466 2024-03-30 18:14:25.084470 pybob_sdk-0.1.5/pybob_sdk/v1/timeoff.py
--rw-r--r--   0        0        0      462 2024-03-30 19:14:03.312433 pybob_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 pybob_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-03-29 14:24:07.195425 pybob_sdk-0.1.6/LICENCE.md
+-rw-r--r--   0        0        0     1529 2024-03-30 19:12:40.256434 pybob_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0       21 2024-03-30 19:00:08.784442 pybob_sdk-0.1.6/pybob_sdk/__init__.py
+-rw-r--r--   0        0        0     2067 2024-03-30 18:52:09.612447 pybob_sdk-0.1.6/pybob_sdk/bob.py
+-rw-r--r--   0        0        0     2928 2024-03-30 19:00:08.904442 pybob_sdk-0.1.6/pybob_sdk/bob_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 14:51:46.611408 pybob_sdk-0.1.6/pybob_sdk/v1/__init__.py
+-rw-r--r--   0        0        0     1408 2024-03-30 18:14:24.360470 pybob_sdk-0.1.6/pybob_sdk/v1/attendance.py
+-rw-r--r--   0        0        0       80 2024-03-30 18:14:24.356470 pybob_sdk-0.1.6/pybob_sdk/v1/base.py
+-rw-r--r--   0        0        0       24 2024-03-30 18:14:24.356470 pybob_sdk-0.1.6/pybob_sdk/v1/company.py
+-rw-r--r--   0        0        0     4238 2024-04-04 22:17:14.068996 pybob_sdk-0.1.6/pybob_sdk/v1/documents.py
+-rw-r--r--   0        0        0     2026 2024-03-30 18:14:24.444470 pybob_sdk-0.1.6/pybob_sdk/v1/hiring.py
+-rw-r--r--   0        0        0     7125 2024-03-30 18:55:26.596445 pybob_sdk-0.1.6/pybob_sdk/v1/metadata.py
+-rw-r--r--   0        0        0      231 2024-03-30 18:14:24.212470 pybob_sdk-0.1.6/pybob_sdk/v1/models/Bob.py
+-rw-r--r--   0        0        0      537 2024-03-30 18:14:24.268470 pybob_sdk-0.1.6/pybob_sdk/v1/models/Metadata.py
+-rw-r--r--   0        0        0      682 2024-03-30 18:14:24.316470 pybob_sdk-0.1.6/pybob_sdk/v1/models/Payroll.py
+-rw-r--r--   0        0        0      802 2024-03-30 18:14:24.324470 pybob_sdk-0.1.6/pybob_sdk/v1/models/People.py
+-rw-r--r--   0        0        0      138 2024-03-30 18:14:24.328470 pybob_sdk-0.1.6/pybob_sdk/v1/models/Reports.py
+-rw-r--r--   0        0        0      497 2024-03-30 18:14:24.352470 pybob_sdk-0.1.6/pybob_sdk/v1/models/Tasks.py
+-rw-r--r--   0        0        0        0 2024-03-29 14:51:49.343408 pybob_sdk-0.1.6/pybob_sdk/v1/models/__init__.py
+-rw-r--r--   0        0        0      908 2024-03-30 18:14:24.548470 pybob_sdk-0.1.6/pybob_sdk/v1/objects.py
+-rw-r--r--   0        0        0      238 2024-03-30 18:14:24.556470 pybob_sdk-0.1.6/pybob_sdk/v1/onboarding.py
+-rw-r--r--   0        0        0      770 2024-03-30 18:14:24.576470 pybob_sdk-0.1.6/pybob_sdk/v1/payroll.py
+-rw-r--r--   0        0        0    36350 2024-03-30 18:55:33.020445 pybob_sdk-0.1.6/pybob_sdk/v1/people.py
+-rw-r--r--   0        0        0     3963 2024-03-30 18:55:36.240445 pybob_sdk-0.1.6/pybob_sdk/v1/reports.py
+-rw-r--r--   0        0        0     3386 2024-03-30 18:14:24.752470 pybob_sdk-0.1.6/pybob_sdk/v1/tables.py
+-rw-r--r--   0        0        0     2776 2024-03-30 18:55:38.484445 pybob_sdk-0.1.6/pybob_sdk/v1/tasks.py
+-rw-r--r--   0        0        0    17466 2024-03-30 18:14:25.084470 pybob_sdk-0.1.6/pybob_sdk/v1/timeoff.py
+-rw-r--r--   0        0        0      462 2024-04-04 22:18:18.508997 pybob_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 pybob_sdk-0.1.6/PKG-INFO
```

### Comparing `pybob_sdk-0.1.5/LICENCE.md` & `pybob_sdk-0.1.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/README.md` & `pybob_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/bob.py` & `pybob_sdk-0.1.6/pybob_sdk/bob.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/bob_client.py` & `pybob_sdk-0.1.6/pybob_sdk/bob_client.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/attendance.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/attendance.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/documents.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base import BobEndpoint
 from typing import Optional, List
-import mimetypes
+import filetypes
 
 
 class Documents(BobEndpoint):
     def upload_document(
         self,
         employeeId: str,
         folderId: str = "shared",
@@ -74,18 +74,18 @@
             case "shared":
                 endpoint = endpoint
             case "confidential":
                 endpoint = f"docs/people/{employeeId}/confidential/upload"
             case _:
                 endpoint = f"docs/people/{employeeId}/folders/{folderId}/upload"
 
-        mime_type, _ = mimetypes.guess_type(file)
+        file_type, _ = filetype.guess(file)
 
         return self.client.post(
-            endpoint, files={"file": (file, open(file, "rb"), mime_type)}
+            endpoint, files={"file": (file, open(file, "rb"), file_type.mime)}
         )
 
     def delete_document(self, employeeId: str, docId: str, folderId: str):
         """
         Delete a specific document from the employee's shared folder.
 
         Args:
```

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/hiring.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/hiring.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/metadata.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/metadata.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/models/Metadata.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/models/Metadata.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/models/Payroll.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/models/Payroll.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/models/People.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/models/People.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/objects.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/objects.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/payroll.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/payroll.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/people.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/people.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/reports.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/reports.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/tables.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/tables.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/tasks.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/pybob_sdk/v1/timeoff.py` & `pybob_sdk-0.1.6/pybob_sdk/v1/timeoff.py`

 * *Files identical despite different names*

### Comparing `pybob_sdk-0.1.5/PKG-INFO` & `pybob_sdk-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybob-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: An unofficial python SDK for the Bob HR platform.
 License: MIT
 Author: Kurtis Massey
 Author-email: 55586356+kurtismassey@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

