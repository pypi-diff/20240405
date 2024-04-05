# Comparing `tmp/facespace-0.1.1.tar.gz` & `tmp/facespace-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facespace-0.1.1.tar", last modified: Sat Jan 13 08:10:38 2024, max compression
+gzip compressed data, was "facespace-0.1.2.tar", last modified: Fri Apr  5 10:30:25 2024, max compression
```

## Comparing `facespace-0.1.1.tar` & `facespace-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-13 08:10:38.971519 facespace-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-11-04 13:59:28.000000 facespace-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    10581 2024-01-13 08:10:38.971519 facespace-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9794 2023-11-04 14:38:53.000000 facespace-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-13 08:10:38.953004 facespace-0.1.1/facespace/
--rw-rw-rw-   0        0        0       78 2023-11-04 13:26:02.000000 facespace-0.1.1/facespace/__init__.py
--rw-rw-rw-   0        0        0    29695 2024-01-13 08:09:08.000000 facespace-0.1.1/facespace/facespace_client.py
-drwxrwxrwx   0        0        0        0 2024-01-13 08:10:38.969515 facespace-0.1.1/facespace.egg-info/
--rw-rw-rw-   0        0        0    10581 2024-01-13 08:10:38.000000 facespace-0.1.1/facespace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-01-13 08:10:38.000000 facespace-0.1.1/facespace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-13 08:10:38.000000 facespace-0.1.1/facespace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-01-13 08:10:38.000000 facespace-0.1.1/facespace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-13 08:10:38.000000 facespace-0.1.1/facespace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-13 08:10:38.971519 facespace-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-01-13 08:07:45.000000 facespace-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:30:25.683624 facespace-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-11-04 13:59:28.000000 facespace-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    10581 2024-04-05 10:30:25.682115 facespace-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9794 2023-11-04 14:38:53.000000 facespace-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 10:30:25.655978 facespace-0.1.2/facespace/
+-rw-rw-rw-   0        0        0       78 2023-11-04 13:26:02.000000 facespace-0.1.2/facespace/__init__.py
+-rw-rw-rw-   0        0        0    29733 2024-04-05 10:29:34.000000 facespace-0.1.2/facespace/facespace_client.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:30:25.681115 facespace-0.1.2/facespace.egg-info/
+-rw-rw-rw-   0        0        0    10581 2024-04-05 10:30:25.000000 facespace-0.1.2/facespace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-05 10:30:25.000000 facespace-0.1.2/facespace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 10:30:25.000000 facespace-0.1.2/facespace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-05 10:30:25.000000 facespace-0.1.2/facespace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 10:30:25.000000 facespace-0.1.2/facespace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 10:30:25.683624 facespace-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-05 10:30:02.000000 facespace-0.1.2/setup.py
```

### Comparing `facespace-0.1.1/LICENSE.txt` & `facespace-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facespace-0.1.1/PKG-INFO` & `facespace-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facespace
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for FaceSpace API services
 Home-page: https://vision.automa.one
 Author: Automa
 Author-email: facespace@automa.one
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `facespace-0.1.1/README.md` & `facespace-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `facespace-0.1.1/facespace/facespace_client.py` & `facespace-0.1.2/facespace/facespace_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os, requests, time, traceback, logging, inspect, signal
 from datetime import datetime
 from dateutil import parser
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 
 
-API_BASE_URL = "https://visioncore.automa.one"
+API_BASE_URL = "https://visionapi.automa.one/facespace"
 
 
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 )
 
 
@@ -71,15 +71,15 @@
             "ForLoopError: The get_realtime_logs method must be used within a 'for' loop as shown below:\n"
             f"{example_usage}"
         )
 
 
 class LogsAPI:
     """The main class to use for communicating with FaceSpace APIs"""
-    def __init__(self, api_key=None, log_to_file=False, log_level=logging.INFO, file_log_level=logging.DEBUG, additional_headers=None, webhook_url=None, post_realtime=True, post_logs=False):
+    def __init__(self, api_key=None, log_to_file=False, log_level=logging.INFO, file_log_level=logging.DEBUG, additional_headers=None, webhook_url=None, post_realtime=True, post_logs=False, gaze_detection=False):
         """
         Summary:
             Initializes the logging API client with configurable parameters.
 
         Description:
             This constructor sets up the logging environment, including API key configuration, session retries, signal handling, and log handlers for both console and file output based on user preferences.
 
@@ -106,15 +106,15 @@
         self.post_realtime = post_realtime  # Set the flag for real-time log posting
         self.post_logs = post_logs  # Set the flag for log posting
         self.running = False  # Initialize the running state of the logger
         self._within_context_manager = False  # Internal flag for context manager state
         signal.signal(signal.SIGINT, self.signal_handler)  # Set up signal handling for graceful shutdown
         self.request_count = 0  # Initialize the request count
         self.last_active_time = None  # Initialize the last active time
-        
+        self.gaze_detection = gaze_detection
         # Additional headers for HTTP requests
         self.additional_headers = additional_headers or {}
         
         # Webhook URL for posting logs
         self.webhook_url = webhook_url
         
         # Update the headers with additional headers
@@ -399,25 +399,20 @@
         params = {}  # Initialize the parameters dictionary
         if start_time:
             params['start_time'] = self._parse_date(start_time)  # Parse and add start time to parameters
         if end_time:
             params['end_time'] = self._parse_date(end_time)  # Parse and add end time to parameters
         if camera_id:
             params['camera_id'] = camera_id  # Add camera ID to parameters if provided
-        return self._response("/api/logs", params=params)  # Make the API call and return the response
-
-
+        return self._response("/logs", params=params)  # Make the API call and return the response
 
     ##########################################################
-    #      REALTIME API SECTION BELOW, DO NOT TAMPER         #
+    #     REALTIME API SECTION BELOW, DO NOT TAMPER 💀      #
     ##########################################################
     
-    
-    
-    
     def fetch_logs(self):
         """
         Summary:
             Fetches the latest logs from the recognition API endpoint.
 
         Description:
             This method retrieves logs from the recognition API. If the logs contain a stop signal indicating no active cameras,
@@ -427,15 +422,15 @@
         Returns:
             - A dictionary containing the fetched log data.
 
         Exceptions:
             - Raises StopLogsSignal if a stop signal is detected in the log indicating no active cameras.
             - Raises HTTPRequestError if the response from the server is not successful (non-200 status code).
         """
-        response = self.session.get(API_BASE_URL + "/api/recognition", headers=self.headers)  # Perform a GET request to fetch logs
+        response = self.session.get(API_BASE_URL + "/recognition", headers=self.headers)  # Perform a GET request to fetch logs
         if response.status_code == 200:
             log = response.json()  # Parse the log from the response
             # Check for a stop signal in the log
             if isinstance(log, dict) and 'stop' in log and log['stop'].startswith('No cameras active'):
                 raise StopLogsSignal("Stop signal received: " + log['stop'])  # Raise a StopLogsSignal exception
             self.logs.append(log)  # Append the log to the internal list
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `facespace-0.1.1/facespace.egg-info/PKG-INFO` & `facespace-0.1.2/facespace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facespace
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for FaceSpace API services
 Home-page: https://vision.automa.one
 Author: Automa
 Author-email: facespace@automa.one
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `facespace-0.1.1/setup.py` & `facespace-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facespace',
-    version='0.1.1',
+    version='0.1.2',
     author='Automa',
     author_email='facespace@automa.one',
     description='A client for FaceSpace API services',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://vision.automa.one',
     packages=find_packages(),
```

