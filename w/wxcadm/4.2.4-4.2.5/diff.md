# Comparing `tmp/wxcadm-4.2.4.tar.gz` & `tmp/wxcadm-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxcadm-4.2.4.tar", last modified: Thu Mar 28 14:03:59 2024, max compression
+gzip compressed data, was "wxcadm-4.2.5.tar", last modified: Fri Apr  5 18:09:55 2024, max compression
```

## Comparing `wxcadm-4.2.4.tar` & `wxcadm-4.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:03:59.408898 wxcadm-4.2.4/
--rw-rw-rw-   0        0        0    35823 2022-08-15 14:34:57.000000 wxcadm-4.2.4/LICENSE
--rw-rw-rw-   0        0        0       25 2022-08-15 14:34:57.000000 wxcadm-4.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2938 2024-03-28 14:03:59.398772 wxcadm-4.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2372 2022-08-15 14:34:57.000000 wxcadm-4.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-03-28 14:03:59.408898 wxcadm-4.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-03-28 14:03:56.000000 wxcadm-4.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:03:59.014864 wxcadm-4.2.4/tests/
--rw-rw-rw-   0        0        0     5241 2024-03-25 13:44:31.000000 wxcadm-4.2.4/tests/test_dect.py
--rw-rw-rw-   0        0        0     3201 2024-02-15 19:03:07.000000 wxcadm-4.2.4/tests/test_device.py
--rw-rw-rw-   0        0        0     1398 2023-10-03 17:16:17.000000 wxcadm-4.2.4/tests/test_jobs.py
--rw-rw-rw-   0        0        0     3256 2023-12-05 19:27:28.000000 wxcadm-4.2.4/tests/test_redsky.py
--rw-rw-rw-   0        0        0      906 2024-03-28 13:55:43.000000 wxcadm-4.2.4/tests/test_reports.py
--rw-rw-rw-   0        0        0     1881 2023-10-03 17:16:17.000000 wxcadm-4.2.4/tests/test_webex.py
--rw-rw-rw-   0        0        0     1726 2023-10-03 17:16:17.000000 wxcadm-4.2.4/tests/test_workspaces.py
--rw-rw-rw-   0        0        0     4609 2023-10-03 17:16:17.000000 wxcadm-4.2.4/tests/test_xsi.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:03:59.351691 wxcadm-4.2.4/wxcadm/
--rw-rw-rw-   0        0        0      516 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/__init__.py
--rw-rw-rw-   0        0        0     8184 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/announcements.py
--rw-rw-rw-   0        0        0     8898 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/applications.py
--rw-rw-rw-   0        0        0     8501 2024-02-26 21:14:56.000000 wxcadm-4.2.4/wxcadm/auto_attendant.py
--rw-rw-rw-   0        0        0     2048 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/bifrost.py
--rw-rw-rw-   0        0        0    12160 2024-02-26 20:04:26.000000 wxcadm-4.2.4/wxcadm/call_queue.py
--rw-rw-rw-   0        0        0    13342 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/call_routing.py
--rw-rw-rw-   0        0        0     3321 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/calls.py
--rw-rw-rw-   0        0        0    17483 2024-03-20 13:55:43.000000 wxcadm-4.2.4/wxcadm/common.py
--rw-rw-rw-   0        0        0    13789 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/cpapi.py
--rw-rw-rw-   0        0        0    21656 2024-03-27 20:35:21.000000 wxcadm-4.2.4/wxcadm/dect.py
--rw-rw-rw-   0        0        0    29976 2024-01-12 16:42:37.000000 wxcadm-4.2.4/wxcadm/device.py
--rw-rw-rw-   0        0        0     1369 2022-08-23 16:22:45.000000 wxcadm-4.2.4/wxcadm/exceptions.py
--rw-rw-rw-   0        0        0     9438 2024-02-26 21:14:56.000000 wxcadm-4.2.4/wxcadm/hunt_group.py
--rw-rw-rw-   0        0        0    15413 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/jobs.py
--rw-rw-rw-   0        0        0    24659 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/location.py
--rw-rw-rw-   0        0        0    14181 2024-02-22 15:04:44.000000 wxcadm-4.2.4/wxcadm/location_features.py
--rw-rw-rw-   0        0        0    21777 2023-12-04 17:13:09.000000 wxcadm-4.2.4/wxcadm/meraki.py
--rw-rw-rw-   0        0        0      307 2023-02-16 15:26:30.000000 wxcadm-4.2.4/wxcadm/number.py
--rw-rw-rw-   0        0        0    31121 2024-03-28 13:37:50.000000 wxcadm-4.2.4/wxcadm/org.py
--rw-rw-rw-   0        0        0    72125 2024-02-15 19:21:13.000000 wxcadm-4.2.4/wxcadm/person.py
--rw-rw-rw-   0        0        0     3205 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/pickup_group.py
--rw-rw-rw-   0        0        0     1334 2023-11-03 19:56:29.000000 wxcadm-4.2.4/wxcadm/realtime.py
--rw-rw-rw-   0        0        0     2972 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/recording.py
--rw-rw-rw-   0        0        0    47269 2023-12-21 19:53:27.000000 wxcadm-4.2.4/wxcadm/redsky.py
--rw-rw-rw-   0        0        0    12133 2024-03-28 13:47:40.000000 wxcadm-4.2.4/wxcadm/reports.py
--rw-rw-rw-   0        0        0     1303 2023-10-03 17:16:17.000000 wxcadm-4.2.4/wxcadm/terminus.py
--rw-rw-rw-   0        0        0    14058 2023-12-21 20:08:03.000000 wxcadm-4.2.4/wxcadm/virtual_line.py
--rw-rw-rw-   0        0        0    12779 2024-03-28 13:39:44.000000 wxcadm-4.2.4/wxcadm/webex.py
--rw-rw-rw-   0        0        0     8968 2022-08-23 16:22:45.000000 wxcadm-4.2.4/wxcadm/webhooks.py
--rw-rw-rw-   0        0        0     6002 2023-12-04 17:13:10.000000 wxcadm-4.2.4/wxcadm/wholesale.py
--rw-rw-rw-   0        0        0    23279 2024-02-26 20:16:18.000000 wxcadm-4.2.4/wxcadm/workspace.py
--rw-rw-rw-   0        0        0    73491 2023-10-10 13:52:08.000000 wxcadm-4.2.4/wxcadm/xsi.py
--rw-rw-rw-   0        0        0     1040 2022-08-23 16:22:45.000000 wxcadm-4.2.4/wxcadm/xsi_response.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:03:59.386728 wxcadm-4.2.4/wxcadm.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-03-28 14:03:58.000000 wxcadm-4.2.4/wxcadm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-03-28 14:03:58.000000 wxcadm-4.2.4/wxcadm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:03:58.000000 wxcadm-4.2.4/wxcadm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2024-03-28 14:03:58.000000 wxcadm-4.2.4/wxcadm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-28 14:03:58.000000 wxcadm-4.2.4/wxcadm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 18:09:55.581372 wxcadm-4.2.5/
+-rw-rw-rw-   0        0        0    35823 2022-08-15 14:34:57.000000 wxcadm-4.2.5/LICENSE
+-rw-rw-rw-   0        0        0       25 2022-08-15 14:34:57.000000 wxcadm-4.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2938 2024-04-05 18:09:55.576934 wxcadm-4.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2372 2022-08-15 14:34:57.000000 wxcadm-4.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:09:55.582706 wxcadm-4.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-05 18:09:15.000000 wxcadm-4.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:09:55.346216 wxcadm-4.2.5/tests/
+-rw-rw-rw-   0        0        0     5241 2024-03-28 14:06:55.000000 wxcadm-4.2.5/tests/test_dect.py
+-rw-rw-rw-   0        0        0     3201 2024-03-28 14:06:55.000000 wxcadm-4.2.5/tests/test_device.py
+-rw-rw-rw-   0        0        0     1398 2023-10-03 17:16:17.000000 wxcadm-4.2.5/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     3256 2024-03-28 14:06:55.000000 wxcadm-4.2.5/tests/test_redsky.py
+-rw-rw-rw-   0        0        0      906 2024-03-28 14:06:55.000000 wxcadm-4.2.5/tests/test_reports.py
+-rw-rw-rw-   0        0        0     1881 2023-10-03 17:16:17.000000 wxcadm-4.2.5/tests/test_webex.py
+-rw-rw-rw-   0        0        0     1726 2023-10-03 17:16:17.000000 wxcadm-4.2.5/tests/test_workspaces.py
+-rw-rw-rw-   0        0        0     4609 2023-10-03 17:16:17.000000 wxcadm-4.2.5/tests/test_xsi.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:09:55.546734 wxcadm-4.2.5/wxcadm/
+-rw-rw-rw-   0        0        0      516 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/__init__.py
+-rw-rw-rw-   0        0        0     8184 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/announcements.py
+-rw-rw-rw-   0        0        0     8898 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/applications.py
+-rw-rw-rw-   0        0        0     8501 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/auto_attendant.py
+-rw-rw-rw-   0        0        0     2048 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/bifrost.py
+-rw-rw-rw-   0        0        0    12160 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/call_queue.py
+-rw-rw-rw-   0        0        0    13342 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/call_routing.py
+-rw-rw-rw-   0        0        0     3321 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/calls.py
+-rw-rw-rw-   0        0        0    17483 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/common.py
+-rw-rw-rw-   0        0        0    13789 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/cpapi.py
+-rw-rw-rw-   0        0        0    21656 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/dect.py
+-rw-rw-rw-   0        0        0    35696 2024-04-05 15:31:11.000000 wxcadm-4.2.5/wxcadm/device.py
+-rw-rw-rw-   0        0        0     1369 2022-08-23 16:22:45.000000 wxcadm-4.2.5/wxcadm/exceptions.py
+-rw-rw-rw-   0        0        0     9438 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/hunt_group.py
+-rw-rw-rw-   0        0        0    15413 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/jobs.py
+-rw-rw-rw-   0        0        0    24659 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/location.py
+-rw-rw-rw-   0        0        0    14181 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/location_features.py
+-rw-rw-rw-   0        0        0    21777 2023-12-04 17:13:09.000000 wxcadm-4.2.5/wxcadm/meraki.py
+-rw-rw-rw-   0        0        0      307 2023-02-16 15:26:30.000000 wxcadm-4.2.5/wxcadm/number.py
+-rw-rw-rw-   0        0        0    31121 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/org.py
+-rw-rw-rw-   0        0        0    74442 2024-04-05 17:03:26.000000 wxcadm-4.2.5/wxcadm/person.py
+-rw-rw-rw-   0        0        0     3205 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/pickup_group.py
+-rw-rw-rw-   0        0        0     1334 2023-11-03 19:56:29.000000 wxcadm-4.2.5/wxcadm/realtime.py
+-rw-rw-rw-   0        0        0     2972 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/recording.py
+-rw-rw-rw-   0        0        0    47269 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/redsky.py
+-rw-rw-rw-   0        0        0    12133 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/reports.py
+-rw-rw-rw-   0        0        0     1303 2023-10-03 17:16:17.000000 wxcadm-4.2.5/wxcadm/terminus.py
+-rw-rw-rw-   0        0        0    14058 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/virtual_line.py
+-rw-rw-rw-   0        0        0    12779 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/webex.py
+-rw-rw-rw-   0        0        0     8968 2022-08-23 16:22:45.000000 wxcadm-4.2.5/wxcadm/webhooks.py
+-rw-rw-rw-   0        0        0     6002 2023-12-04 17:13:10.000000 wxcadm-4.2.5/wxcadm/wholesale.py
+-rw-rw-rw-   0        0        0    23279 2024-03-28 14:06:55.000000 wxcadm-4.2.5/wxcadm/workspace.py
+-rw-rw-rw-   0        0        0    73491 2023-10-10 13:52:08.000000 wxcadm-4.2.5/wxcadm/xsi.py
+-rw-rw-rw-   0        0        0     1040 2022-08-23 16:22:45.000000 wxcadm-4.2.5/wxcadm/xsi_response.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:09:55.572935 wxcadm-4.2.5/wxcadm.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-05 18:09:55.000000 wxcadm-4.2.5/wxcadm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-04-05 18:09:55.000000 wxcadm-4.2.5/wxcadm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:09:55.000000 wxcadm-4.2.5/wxcadm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-04-05 18:09:55.000000 wxcadm-4.2.5/wxcadm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 18:09:55.000000 wxcadm-4.2.5/wxcadm.egg-info/top_level.txt
```

### Comparing `wxcadm-4.2.4/LICENSE` & `wxcadm-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/PKG-INFO` & `wxcadm-4.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxcadm
-Version: 4.2.4
+Version: 4.2.5
 Summary: A Python 3 Library for Webex Calling Administrators
 Home-page: https://github.com/kctrey/wxcadm
 Author: Trey Hilyard
 Author-email: kctrey@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `wxcadm-4.2.4/README.md` & `wxcadm-4.2.5/README.md`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/setup.py` & `wxcadm-4.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='wxcadm',
-    version='4.2.4',
+    version='4.2.5',
     packages=packages,
     url='https://github.com/kctrey/wxcadm',
     license='GPL-3.0',
     author='Trey Hilyard',
     author_email='kctrey@gmail.com',
     description='A Python 3 Library for Webex Calling Administrators',
     long_description=readme,
```

### Comparing `wxcadm-4.2.4/tests/test_dect.py` & `wxcadm-4.2.5/tests/test_dect.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_device.py` & `wxcadm-4.2.5/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_jobs.py` & `wxcadm-4.2.5/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_redsky.py` & `wxcadm-4.2.5/tests/test_redsky.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_reports.py` & `wxcadm-4.2.5/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_webex.py` & `wxcadm-4.2.5/tests/test_webex.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_workspaces.py` & `wxcadm-4.2.5/tests/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/tests/test_xsi.py` & `wxcadm-4.2.5/tests/test_xsi.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/__init__.py` & `wxcadm-4.2.5/wxcadm/__init__.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/announcements.py` & `wxcadm-4.2.5/wxcadm/announcements.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/applications.py` & `wxcadm-4.2.5/wxcadm/applications.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/auto_attendant.py` & `wxcadm-4.2.5/wxcadm/auto_attendant.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/bifrost.py` & `wxcadm-4.2.5/wxcadm/bifrost.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/call_queue.py` & `wxcadm-4.2.5/wxcadm/call_queue.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/call_routing.py` & `wxcadm-4.2.5/wxcadm/call_routing.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/calls.py` & `wxcadm-4.2.5/wxcadm/calls.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/common.py` & `wxcadm-4.2.5/wxcadm/common.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/cpapi.py` & `wxcadm-4.2.5/wxcadm/cpapi.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/dect.py` & `wxcadm-4.2.5/wxcadm/dect.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/device.py` & `wxcadm-4.2.5/wxcadm/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                 'port': entry.port,
                 'id': entry.id,
                 'primaryOwner': entry.primary_owner,
                 'lineType': entry.line_type,
                 'lineWeight': entry.line_weight,
                 'hotlineEnabled': entry.hotline_enabled,
                 'hotlineDestination': entry.hotline_destination,
-                'allowCallDeclineEnabled': entry.allow_call_decline,
+                'allowCallDeclineEnabled': entry.call_decline_all,
             }
             # lineLabel is weird, so we have to only add it back when it is not None
             if entry.line_label is not None:
                 new_entry['lineLabel'] = entry.line_label
             json_list.append(new_entry)
         return json_list
 
@@ -321,36 +321,160 @@
         for member in self.data:
             log.debug("Starting loop")
             for p in range(member.port, member.port + member.line_weight, 1):
                 log.debug(f"In Loop: {p}")
                 port_map[p] = member
         return port_map
 
+    def get(self, person: Optional[Person] = None, workspace: Optional[Workspace] = None):
+        if person is not None and workspace is not None:
+            raise ValueError('Only person or workspace is accepted, not both')
+        if person is not None:
+            member_instance = person
+        if workspace is not None:
+            member_instance = workspace
+        for member in self.data:
+            if member.id is not None and (member.id == member_instance.id):
+                return member
+        return None
+
 
 class DeviceMember:
     def __init__(self, device: Device, member_info: dict):
         self.device: Device = device
         self.member_type: str = member_info['memberType']
         self.id: str = member_info['id']
         self.port: int = member_info['port']
         self.primary_owner: bool = member_info['primaryOwner']
         self.line_type: str = member_info['lineType']
         self.line_weight: int = member_info['lineWeight']
         self.hotline_enabled: bool = member_info['hotlineEnabled']
         self.hotline_destination: str = member_info.get('hotlineDestination', None)
-        self.allow_call_decline: bool = member_info['allowCallDeclineEnabled']
+        self.call_decline_all: bool = member_info['allowCallDeclineEnabled']
         self.line_label: Optional[str] = member_info.get('lineLabel', None)
         self.first_name: Optional[str] = member_info.get('firstName', None)
         self.last_name: Optional[str] = member_info.get('lastName', None)
         self.phone_number: Optional[str] = member_info.get('phoneNumber', None)
         self.extension: Optional[str] = member_info.get('extension', None)
         self.host_ip: Optional[str] = member_info.get('hostIP', None)
         self.remote_ip: Optional[str] = member_info.get('remoteIP', None)
         self.line_port: Optional[str] = member_info.get('linePort', None)
 
+    def set_line_label(self, label: str) -> DeviceMember:
+        """ Set/update the Line Label on the device
+
+        Args:
+            label (str): The new line label
+
+        Returns:
+            DeviceMember: The updated DeviceMember instance
+
+        """
+        # Rather than rebuild the member list from what we already have, it's quicker to just pull a fresh copy
+        old_member_list = webex_api_call('get', f'v1/telephony/config/devices/{self.device.id}/members')
+        new_member_list = []
+        for member in old_member_list['members']:
+            if member['id'] == self.id:
+                member['lineLabel'] = label
+            # The PUT doesn't take all the fields that the GET has so we have to clean up
+            member.pop('remoteIP', None)
+            member.pop('linePort', None)
+            member.pop('firstName', None)
+            member.pop('lastName', None)
+            member.pop('phoneNumber', None)
+            member.pop('extension', None)
+            member.pop('hostIP', None)
+            member.pop('location', None)
+
+            new_member_list.append(member)
+
+        # Once we have rebuilt the list, just PUT it back
+        webex_api_call('put', f'v1/telephony/config/devices/{self.device.id}/members',
+                       payload={'members': new_member_list})
+        self.line_label = label
+        return self
+
+    def set_hotline(self, enabled: bool, destination: Optional[str] = None) -> DeviceMember:
+        """ Enable or disable Hotline for the Device Member
+
+        Args:
+            enabled (bool): True for Enabled, False for Disabled
+            destination (str, optional): The Hotline destination
+
+        Returns:
+            DeviceMember: The updated DeviceMember instance
+
+        """
+        # Rather than rebuild the member list from what we already have, it's quicker to just pull a fresh copy
+        old_member_list = webex_api_call('get', f'v1/telephony/config/devices/{self.device.id}/members')
+        new_member_list = []
+        for member in old_member_list['members']:
+            if member['id'] == self.id:
+                member['hotlineEnabled'] = enabled
+                if destination is not None:
+                    member['hotlineDestination'] = destination
+
+            # The PUT doesn't take all the fields that the GET has so we have to clean up
+            member.pop('remoteIP', None)
+            member.pop('linePort', None)
+            member.pop('firstName', None)
+            member.pop('lastName', None)
+            member.pop('phoneNumber', None)
+            member.pop('extension', None)
+            member.pop('hostIP', None)
+            member.pop('location', None)
+
+            new_member_list.append(member)
+
+        # Once we have rebuilt the list, just PUT it back
+        webex_api_call('put', f'v1/telephony/config/devices/{self.device.id}/members',
+                       payload={'members': new_member_list})
+        self.hotline_enabled = enabled
+        if destination is not None:
+            self.hotline_destination = destination
+        return self
+
+    def set_call_decline_all(self, enabled: bool):
+        """ Set or change the Call Decline behavior of the Device Member.
+
+        When set to True, declining the call on the device will decline the call on all devices. When set to False,
+        declining the call on the device will only silence the device and allow other devices to keep ringing.
+
+        Args:
+            enabled (bool): True to decline on all devices, False to decline on this device
+
+        Returns:
+            DeviceMember: The updated DeviceMember instance
+
+        """
+        # Rather than rebuild the member list from what we already have, it's quicker to just pull a fresh copy
+        old_member_list = webex_api_call('get', f'v1/telephony/config/devices/{self.device.id}/members')
+        new_member_list = []
+        for member in old_member_list['members']:
+            if member['id'] == self.id:
+                member['allowCallDeclineEnabled'] = enabled
+
+            # The PUT doesn't take all the fields that the GET has so we have to clean up
+            member.pop('remoteIP', None)
+            member.pop('linePort', None)
+            member.pop('firstName', None)
+            member.pop('lastName', None)
+            member.pop('phoneNumber', None)
+            member.pop('extension', None)
+            member.pop('hostIP', None)
+            member.pop('location', None)
+
+            new_member_list.append(member)
+
+        # Once we have rebuilt the list, just PUT it back
+        webex_api_call('put', f'v1/telephony/config/devices/{self.device.id}/members',
+                       payload={'members': new_member_list})
+        self.call_decline_all = enabled
+        return self
+
 
 class DeviceList(UserList):
     _endpoint = "v1/devices"
     _endpoint_items_key = None
     _item_endpoint = "v1/devices/{item_id}"
     _item_class = Device
 
@@ -401,45 +525,51 @@
         """
         self.data = self._get_data()
         return True
 
     def get(self,
             id: Optional[str] = None,
             name: Optional[str] = None,
+            mac_address: Optional[str] = None,
             spark_id: Optional[str] = None,
             connection_status: Optional[str] = None):
         """ Get the instance associated with a given ID, Name, or Spark ID
 
         Only one parameter should be supplied in normal cases. If multiple arguments are provided, the Locations will be
         searched in order by ID, Name, and finally Spark ID. If no arguments are provided, the method will raise an
         Exception.
 
         Args:
-            id (str, optional): The Call Queue ID to find
-            name (str, optional): The Call Queue Name to find. Case-insensitive.
+            id (str, optional): The Device ID to find
+            name (str, optional): The Device Name to find. Case-insensitive.
+            mac_address (str, optional): The Device MAC address
             spark_id (str, optional): The Spark ID to find
             connection_status(str, optional): The connection status of the device (e.g. "disconnected", "connected")
 
         Returns:
             Device: The Device instance, or list of instances correlating to the given search argument.
 
         Raises:
             ValueError: Raised when the method is called with no arguments
 
         """
-        if id is None and name is None and spark_id is None and connection_status is None:
+        if id is None and name is None and mac_address is None and spark_id is None and connection_status is None:
             raise ValueError("A search argument must be provided")
         if id is not None:
             for item in self.data:
                 if item.id == id:
                     return item
         if name is not None:
             for item in self.data:
                 if item.display_name.lower() == name.lower():
                     return item
+        if mac_address is not None:
+            for item in self.data:
+                if item.mac == mac_address.upper().replace(':', '').replace('-', ''):
+                    return item
         if spark_id is not None:
             for item in self.data:
                 if item.spark_id == spark_id:
                     return item
         if connection_status is not None:
             item_list: list = []
             for item in self.data:
```

### Comparing `wxcadm-4.2.4/wxcadm/exceptions.py` & `wxcadm-4.2.5/wxcadm/exceptions.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/hunt_group.py` & `wxcadm-4.2.5/wxcadm/hunt_group.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/jobs.py` & `wxcadm-4.2.5/wxcadm/jobs.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/location.py` & `wxcadm-4.2.5/wxcadm/location.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/location_features.py` & `wxcadm-4.2.5/wxcadm/location_features.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/meraki.py` & `wxcadm-4.2.5/wxcadm/meraki.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/org.py` & `wxcadm-4.2.5/wxcadm/org.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/person.py` & `wxcadm-4.2.5/wxcadm/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,28 @@
         """A list of the Call Queue instances that this user is an Agent for"""
         self.outgoing_permission: dict = {}
         """Dictionary of Outgoing Permission config returned by Webex API
         with :meth:`get_outgoing_permission()`"""
         self.applications_settings = None
         """ The Application Services Settings for this Person"""
         self.executive_assistant = None
+        self.avatar: Optional[str] = None
+        """ The URL of the Person's avatar """
+        self.department: Optional[str] = None
+        """ The department the Person belongs to """
+        self.manager: Optional[str] = None
+        """ The Person's manager """
+        self.manager_id: Optional[str] = None
+        """ The Person ID of the manager """
+        self.title: Optional[str] = None
+        """ The Person's title """
+        self.addresses: Optional[list] = None
+        """ A list of addresses for the Person """
+        self.status: Optional[str] = None
+        """ The current presence status of the Person """
         self._devices: Optional[DeviceList] = None
 
         # API-related attributes
         self._headers = parent._headers
         self._params = {"orgId": parent.id, "callingData": "true"}
 
         # If the config was passed, process it. If not, make the API call for the Person ID and then process
@@ -341,14 +355,21 @@
         """
         self.email = data.get('emails', [''])[0]
         self.extension = data.get("extension", "")
         self.location = data.get("locationId", "")
         self.display_name = data.get("displayName", "")
         self.first_name = data.get("firstName", "")
         self.last_name = data.get("lastName", "")
+        self.avatar = data.get('avatar', None)
+        self.department = data.get('department', None)
+        self.manager = data.get('manager', None)
+        self.manager_id = data.get('managerId', None)
+        self.title = data.get('title', None)
+        self.addresses = data.get('addresses', None)
+        self.status = data.get('status', None)
         self.roles = data.get("roles", [])
         self.numbers = data.get("phoneNumbers", [])
         self.licenses = data.get("licenses", [])
         for license in self.licenses:
             if license in self._parent.wxc_licenses:
                 self.wxc = True
 
@@ -1283,15 +1304,21 @@
                       numbers=None,
                       extension=None,
                       location=None,
                       display_name=None,
                       first_name=None,
                       last_name=None,
                       roles=None,
-                      licenses=None):
+                      licenses=None,
+                      avatar: Optional[str] = None,
+                      department: Optional[str] = None,
+                      title: Optional[str] = None,
+                      manager: Optional[str] = None,
+                      manager_id: Optional[str] = None,
+                      addresses: Optional[list] = None):
         """Update the Person in Webex.
 
         Pass only the arguments that you want to change. Other attributes will be populated
         with the existing values from the instance. *Note:* This allows changes directly to the instance attrs to
         be pushed to Webex. For example, changing :py:attr:`Person.extension` and then calling `update_person()` with no
         arguments will still push the extension change. This allows for a lot of flexibility if a method does not
         exist to change the desired value. It is also the method other methods use to push their changes to Webex.
@@ -1302,14 +1329,20 @@
             extension (str): The user's extension
             location (str): The Location ID for the user. Note that this can't actually be changed yet.
             display_name (str): The Display Name for the Person
             first_name (str): The Person's first name
             last_name (str): The Person's last name
             roles (list): List of Role IDs
             licenses (list): List of License IDs
+            avatar (str): The URL of the Person's avatar
+            department (str): The Person's department
+            title (str): The Person's title
+            manager (str): The Person's manager
+            manager_id (str): The Person ID of the manager
+            addresses (list): A list of addresses, each defined as a dict
 
         Returns:
             bool: True if successful. False if not.
 
         """
         # Build the payload using the arguments and the instance attrs
         payload = {}
@@ -1337,14 +1370,32 @@
         payload['lastName'] = last_name
         if roles is None:
             roles = self.roles
         payload['roles'] = roles
         if licenses is None:
             licenses = self.licenses
         payload['licenses'] = licenses
+        if avatar is None:
+            avatar = self.avatar
+        payload['avatar'] = avatar
+        if department is None:
+            department = self.department
+        payload['department'] = department
+        if title is None:
+            title = self.title
+        payload['title'] = title
+        if manager is None:
+            manager = self.manager
+        payload['manager'] = manager
+        if manager_id is None:
+            manager_id = self.manager_id
+        payload['managerId'] = manager_id
+        if addresses is None:
+            addresses = self.addresses
+        payload['addresses'] = addresses
 
         params = {"callingData": "true"}
         response = webex_api_call('put', f'v1/people/{self.id}', payload=payload, params=params)
         if response:
             self.refresh_person()
             return True
         else:
```

### Comparing `wxcadm-4.2.4/wxcadm/pickup_group.py` & `wxcadm-4.2.5/wxcadm/pickup_group.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/realtime.py` & `wxcadm-4.2.5/wxcadm/realtime.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/recording.py` & `wxcadm-4.2.5/wxcadm/recording.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/redsky.py` & `wxcadm-4.2.5/wxcadm/redsky.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/reports.py` & `wxcadm-4.2.5/wxcadm/reports.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/terminus.py` & `wxcadm-4.2.5/wxcadm/terminus.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/virtual_line.py` & `wxcadm-4.2.5/wxcadm/virtual_line.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/webex.py` & `wxcadm-4.2.5/wxcadm/webex.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/webhooks.py` & `wxcadm-4.2.5/wxcadm/webhooks.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/wholesale.py` & `wxcadm-4.2.5/wxcadm/wholesale.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/workspace.py` & `wxcadm-4.2.5/wxcadm/workspace.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/xsi.py` & `wxcadm-4.2.5/wxcadm/xsi.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm/xsi_response.py` & `wxcadm-4.2.5/wxcadm/xsi_response.py`

 * *Files identical despite different names*

### Comparing `wxcadm-4.2.4/wxcadm.egg-info/PKG-INFO` & `wxcadm-4.2.5/wxcadm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxcadm
-Version: 4.2.4
+Version: 4.2.5
 Summary: A Python 3 Library for Webex Calling Administrators
 Home-page: https://github.com/kctrey/wxcadm
 Author: Trey Hilyard
 Author-email: kctrey@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `wxcadm-4.2.4/wxcadm.egg-info/SOURCES.txt` & `wxcadm-4.2.5/wxcadm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

