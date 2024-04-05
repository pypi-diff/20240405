# Comparing `tmp/weavel-0.4.0.tar.gz` & `tmp/weavel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavel-0.4.0.tar", last modified: Thu Apr  4 12:08:44 2024, max compression
+gzip compressed data, was "weavel-0.4.1.tar", last modified: Fri Apr  5 02:57:23 2024, max compression
```

## Comparing `weavel-0.4.0.tar` & `weavel-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,57 @@
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.313794 weavel-0.4.0/
--rw-r--r--   0 aschung    (501) staff       (20)        0 2024-01-18 05:08:39.000000 weavel-0.4.0/LICENSE
--rw-r--r--   0 aschung    (501) staff       (20)      830 2024-04-04 12:08:44.313587 weavel-0.4.0/PKG-INFO
--rw-r--r--   0 aschung    (501) staff       (20)       15 2024-01-18 05:08:39.000000 weavel-0.4.0/README.md
--rw-r--r--   0 aschung    (501) staff       (20)       38 2024-04-04 12:08:44.313952 weavel-0.4.0/setup.cfg
--rw-r--r--   0 aschung    (501) staff       (20)     1244 2024-04-04 12:08:16.000000 weavel-0.4.0/setup.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.310125 weavel-0.4.0/weavel/
--rw-r--r--   0 aschung    (501) staff       (20)      107 2024-04-04 12:08:29.000000 weavel-0.4.0/weavel/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     6063 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/_api_client.py
--rw-r--r--   0 aschung    (501) staff       (20)     1692 2024-04-04 11:41:46.000000 weavel-0.4.0/weavel/_buffer_storage.py
--rw-r--r--   0 aschung    (501) staff       (20)      211 2024-03-12 07:47:26.000000 weavel-0.4.0/weavel/_constants.py
--rw-r--r--   0 aschung    (501) staff       (20)     9433 2024-04-04 11:46:25.000000 weavel-0.4.0/weavel/_worker.py
--rw-r--r--   0 aschung    (501) staff       (20)     5404 2024-04-04 11:47:30.000000 weavel-0.4.0/weavel/client.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.312078 weavel-0.4.0/weavel/poe/
--rw-r--r--   0 aschung    (501) staff       (20)       58 2024-03-12 07:47:26.000000 weavel-0.4.0/weavel/poe/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     1749 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/_poe_buffer_storage.py
--rw-r--r--   0 aschung    (501) staff       (20)     4756 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/_poe_worker.py
--rw-r--r--   0 aschung    (501) staff       (20)     1278 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/poe_client.py
--rw-r--r--   0 aschung    (501) staff       (20)     2431 2024-04-04 11:42:13.000000 weavel-0.4.0/weavel/types.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.312909 weavel-0.4.0/weavel/utils/
--rw-r--r--   0 aschung    (501) staff       (20)       43 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/__init__.py
--rw-r--r--   0 aschung    (501) staff       (20)     1134 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/crypto.py
--rw-r--r--   0 aschung    (501) staff       (20)      679 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/logger.py
-drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.313255 weavel-0.4.0/weavel.egg-info/
--rw-r--r--   0 aschung    (501) staff       (20)      830 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/PKG-INFO
--rw-r--r--   0 aschung    (501) staff       (20)      493 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/SOURCES.txt
--rw-r--r--   0 aschung    (501) staff       (20)        1 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/dependency_links.txt
--rw-r--r--   0 aschung    (501) staff       (20)      184 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/requires.txt
--rw-r--r--   0 aschung    (501) staff       (20)        7 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/top_level.txt
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145640 weavel-0.4.1/
+-rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.4.1/LICENSE
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-04-05 02:57:23.145516 weavel-0.4.1/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.4.1/README.md
+-rw-r--r--   0 jypark     (501) staff       (20)       38 2024-04-05 02:57:23.145685 weavel-0.4.1/setup.cfg
+-rw-r--r--   0 jypark     (501) staff       (20)     1244 2024-04-05 02:54:59.000000 weavel-0.4.1/setup.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.139823 weavel-0.4.1/testapp/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.140324 weavel-0.4.1/testapp/daily_dialog/
+-rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.4.1/testapp/daily_dialog/run_qa_extractor.py
+-rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.4.1/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.4.1/testapp/daily_dialog/save_to_db.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1298 2024-03-21 06:59:25.000000 weavel-0.4.1/testapp/demo.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.140762 weavel-0.4.1/testapp/py_files/
+-rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.4.1/testapp/py_files/duplicate_log_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.4.1/testapp/py_files/poe_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.4.1/testapp/py_files/save_mock_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.4.1/testapp/py_files/save_mock_retention_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)    43795 2024-03-22 07:15:41.000000 weavel-0.4.1/testapp/test.py
+-rw-r--r--   0 jypark     (501) staff       (20)      278 2024-04-05 02:56:14.000000 weavel-0.4.1/testapp/test_identify.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.138949 weavel-0.4.1/venv/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.143127 weavel-0.4.1/venv/bin/
+-rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.4.1/venv/bin/pwiz.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.4.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.143970 weavel-0.4.1/weavel/
+-rw-r--r--   0 jypark     (501) staff       (20)      107 2024-04-05 02:56:10.000000 weavel-0.4.1/weavel/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.4.1/weavel/_api_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1692 2024-04-05 02:11:37.000000 weavel-0.4.1/weavel/_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/_constants.py
+-rw-r--r--   0 jypark     (501) staff       (20)    10005 2024-04-05 02:24:57.000000 weavel-0.4.1/weavel/_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     5824 2024-04-05 02:54:30.000000 weavel-0.4.1/weavel/client.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145012 weavel-0.4.1/weavel/poe/
+-rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.4.1/weavel/poe/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/_poe_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4756 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/_poe_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1278 2024-03-22 06:53:42.000000 weavel-0.4.1/weavel/poe/poe_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     2701 2024-04-05 02:24:52.000000 weavel-0.4.1/weavel/types.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.145337 weavel-0.4.1/weavel/utils/
+-rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.4.1/weavel/utils/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.4.1/weavel/utils/crypto.py
+-rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.4.1/weavel/utils/logger.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-04-05 02:57:23.144531 weavel-0.4.1/weavel.egg-info/
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)     1115 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/SOURCES.txt
+-rw-r--r--   0 jypark     (501) staff       (20)        1 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/dependency_links.txt
+-rw-r--r--   0 jypark     (501) staff       (20)      184 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/requires.txt
+-rw-r--r--   0 jypark     (501) staff       (20)       20 2024-04-05 02:57:23.000000 weavel-0.4.1/weavel.egg-info/top_level.txt
```

### Comparing `weavel-0.4.0/setup.py` & `weavel-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read README.md for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="weavel",
-    version="0.4.0",
+    version="0.4.1",
     packages=find_namespace_packages(),
     entry_points={},
     description="Weavel, natural language analysis Dashboard for LLM Agent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="weavel",
     url="https://github.com/weavel-ai/weavel-python",
```

### Comparing `weavel-0.4.0/weavel/_api_client.py` & `weavel-0.4.1/weavel/_api_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/_buffer_storage.py` & `weavel-0.4.1/weavel/_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/_worker.py` & `weavel-0.4.1/weavel/_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from concurrent.futures import Future, ThreadPoolExecutor
 
 from weavel.types import (
     TraceDataRole,
     OpenTraceBody,
     CaptureTraceDataBody,
     CaptureTrackEventBody,
+    SaveUserIdentityBody
 )
 from weavel._constants import BACKEND_SERVER_URL
 from weavel._buffer_storage import BufferStorage
 from weavel._api_client import APIClient
 from weavel.utils import logger
 
 
@@ -67,14 +68,34 @@
             timestamp=str(timestamp or datetime.now().isoformat()),
             metadata=metadata,
         )
 
         self.buffer_storage.push(request)
 
         return trace_id
+    
+    def identify_user(self, user_id: str, properties: Dict) -> None:
+        """
+        Identifies a user with the given properties.
+
+        Args:
+            user_id (str): The ID of the user.
+            properties (Dict): The properties associated with the user.
+
+        Returns:
+            None
+        """
+        request = SaveUserIdentityBody(
+            user_id=user_id,
+            properties=properties,
+            timestamp=str(datetime.now().isoformat()),
+        )
+        self.buffer_storage.push(request)
+
+        return
 
     def log_track_event(self, user_id: str, name: str, properties: Dict) -> None:
         """
         Logs a track event for a user.
 
         Args:
             user_id (str): The ID of the user.
```

### Comparing `weavel-0.4.0/weavel/client.py` & `weavel-0.4.1/weavel/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 from datetime import datetime
-from typing import Dict, Literal, Optional
+from typing import Dict, Literal, Optional, Any
 
 from dotenv import load_dotenv
 
 from weavel._worker import Worker
 
 load_dotenv()
 
@@ -149,14 +149,24 @@
         Args:
             user_id (str): The identifier of the user.
             event_name (str): The name of the track event.
             properties (Dict): The properties of the track event.
 
         """
         self._worker.log_track_event(user_id, event_name, properties)
+        
+    def identify(self, user_id: str, properties: Dict[str, Any]):
+        """Identify a user with the specified properties.
+        
+        You can save any user information you know about a user for user_id, such as their email, name, or phone number in dict format.
+        Properties will be updated for every call.
+        """
+        
+        self._worker.identify_user(user_id, properties)
+        
 
     def close(self):
         """Close the client connection."""
         self._worker.stop()
 
 
 def create_client(
```

### Comparing `weavel-0.4.0/weavel/poe/_poe_buffer_storage.py` & `weavel-0.4.1/weavel/poe/_poe_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/poe/_poe_worker.py` & `weavel-0.4.1/weavel/poe/_poe_worker.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/poe/poe_client.py` & `weavel-0.4.1/weavel/poe/poe_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/types.py` & `weavel-0.4.1/weavel/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 class BackgroundTaskType(str, Enum):
     open_trace = "open_trace"
     capture_trace_data = "capture_trace_data"
     capture_track_event = "capture_track_event"
     create_semantic_event = "create_semantic_event"
     extract_keywords = "extract_keywords"
+    save_user_identity = "save_user_identity"
 
 
 class OpenTraceBody(WeavelObject):
     """Start Trace body."""
 
     type: Literal["open_trace"] = "open_trace"
     user_id: str
@@ -70,14 +71,20 @@
     trace_id: str
     role: str
     content: str
     unit_name: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     timestamp: Optional[str] = None
 
+class SaveUserIdentityBody(WeavelObject):
+    """Save user identity body."""
+    type: Literal["save_user_identity"] = "save_user_identity"
+    user_id: str
+    properties: Dict[str, Any]
+    timestamp: Optional[str] = None
 
 # class SaveMetadataTraceBody(WeavelObject):
 #     """Save metadata body."""
 #     trace_id: str
 #     metadata: Dict[str, str]
```

### Comparing `weavel-0.4.0/weavel/utils/crypto.py` & `weavel-0.4.1/weavel/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.0/weavel/utils/logger.py` & `weavel-0.4.1/weavel/utils/logger.py`

 * *Files identical despite different names*

