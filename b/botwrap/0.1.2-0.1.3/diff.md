# Comparing `tmp/botwrap-0.1.2.tar.gz` & `tmp/botwrap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botwrap-0.1.2.tar", last modified: Sat Mar 23 03:58:59 2024, max compression
+gzip compressed data, was "botwrap-0.1.3.tar", last modified: Fri Apr  5 19:46:02 2024, max compression
```

## Comparing `botwrap-0.1.2.tar` & `botwrap-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 03:58:59.119533 botwrap-0.1.2/
--rw-rw-rw-   0        0        0     3283 2024-03-23 03:58:59.115450 botwrap-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2024-03-23 01:07:38.000000 botwrap-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 03:58:59.113445 botwrap-0.1.2/botwrap.egg-info/
--rw-rw-rw-   0        0        0     3283 2024-03-23 03:58:58.000000 botwrap-0.1.2/botwrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2024-03-23 03:58:59.000000 botwrap-0.1.2/botwrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 03:58:58.000000 botwrap-0.1.2/botwrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2024-03-23 03:58:59.000000 botwrap-0.1.2/botwrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-23 03:58:59.000000 botwrap-0.1.2/botwrap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-23 03:58:59.089871 botwrap-0.1.2/openaiwrapper/
--rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.2/openaiwrapper/__init__.py
--rw-rw-rw-   0        0        0     4610 2024-03-23 01:53:05.000000 botwrap-0.1.2/openaiwrapper/api_client.py
--rw-rw-rw-   0        0        0     2086 2024-03-23 01:07:05.000000 botwrap-0.1.2/openaiwrapper/assistants.py
--rw-rw-rw-   0        0        0      697 2024-03-23 01:18:57.000000 botwrap-0.1.2/openaiwrapper/config.py
--rw-rw-rw-   0        0        0      453 2024-03-23 01:07:27.000000 botwrap-0.1.2/openaiwrapper/exceptions.py
--rw-rw-rw-   0        0        0     3744 2024-03-23 01:45:37.000000 botwrap-0.1.2/openaiwrapper/files.py
--rw-rw-rw-   0        0        0     2116 2024-03-23 01:07:20.000000 botwrap-0.1.2/openaiwrapper/messages.py
--rw-rw-rw-   0        0        0     3423 2024-03-23 01:39:20.000000 botwrap-0.1.2/openaiwrapper/openai_wrapper.py
--rw-rw-rw-   0        0        0     2607 2024-03-23 01:07:17.000000 botwrap-0.1.2/openaiwrapper/runs.py
--rw-rw-rw-   0        0        0     2282 2024-03-23 01:07:23.000000 botwrap-0.1.2/openaiwrapper/threads.py
--rw-rw-rw-   0        0        0     3569 2024-03-23 01:07:12.000000 botwrap-0.1.2/openaiwrapper/tools.py
--rw-rw-rw-   0        0        0     3233 2024-03-23 01:46:07.000000 botwrap-0.1.2/openaiwrapper/utils.py
--rw-rw-rw-   0        0        0       42 2024-03-23 03:58:59.120532 botwrap-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1447 2024-03-23 03:56:04.000000 botwrap-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 03:58:59.109432 botwrap-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-03-23 01:04:27.000000 botwrap-0.1.2/tests/test_api_client.py
--rw-rw-rw-   0        0        0     3221 2024-03-23 01:00:07.000000 botwrap-0.1.2/tests/test_assistants.py
--rw-rw-rw-   0        0        0     3858 2024-03-23 01:04:30.000000 botwrap-0.1.2/tests/test_files.py
--rw-rw-rw-   0        0        0     2898 2024-03-23 01:06:50.000000 botwrap-0.1.2/tests/test_messages.py
--rw-rw-rw-   0        0        0     2705 2024-03-23 00:57:26.000000 botwrap-0.1.2/tests/test_runs.py
--rw-rw-rw-   0        0        0     2383 2024-03-23 00:57:35.000000 botwrap-0.1.2/tests/test_threads.py
--rw-rw-rw-   0        0        0     3668 2024-03-23 00:57:41.000000 botwrap-0.1.2/tests/test_tools.py
--rw-rw-rw-   0        0        0     3987 2024-03-23 01:06:55.000000 botwrap-0.1.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:46:02.458798 botwrap-0.1.3/
+-rw-rw-rw-   0        0        0     3277 2024-04-05 19:46:02.456820 botwrap-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1513 2024-03-23 23:09:32.000000 botwrap-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 19:46:02.453800 botwrap-0.1.3/botwrap.egg-info/
+-rw-rw-rw-   0        0        0     3277 2024-04-05 19:46:02.000000 botwrap-0.1.3/botwrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2024-04-05 19:46:02.000000 botwrap-0.1.3/botwrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:46:02.000000 botwrap-0.1.3/botwrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2024-04-05 19:46:02.000000 botwrap-0.1.3/botwrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-05 19:46:02.000000 botwrap-0.1.3/botwrap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 19:46:02.426154 botwrap-0.1.3/openaiwrapper/
+-rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.3/openaiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     3860 2024-04-05 19:29:34.000000 botwrap-0.1.3/openaiwrapper/api_client.py
+-rw-rw-rw-   0        0        0     3300 2024-04-04 06:28:29.000000 botwrap-0.1.3/openaiwrapper/assistants.py
+-rw-rw-rw-   0        0        0     1400 2024-04-04 06:36:55.000000 botwrap-0.1.3/openaiwrapper/config.py
+-rw-rw-rw-   0        0        0     1841 2024-04-04 06:35:29.000000 botwrap-0.1.3/openaiwrapper/exceptions.py
+-rw-rw-rw-   0        0        0     4342 2024-04-04 06:26:25.000000 botwrap-0.1.3/openaiwrapper/files.py
+-rw-rw-rw-   0        0        0     3046 2024-04-04 06:15:41.000000 botwrap-0.1.3/openaiwrapper/messages.py
+-rw-rw-rw-   0        0        0    11317 2024-04-04 06:13:47.000000 botwrap-0.1.3/openaiwrapper/openai_wrapper.py
+-rw-rw-rw-   0        0        0     2770 2024-04-04 06:21:44.000000 botwrap-0.1.3/openaiwrapper/runs.py
+-rw-rw-rw-   0        0        0     2866 2024-04-04 06:18:54.000000 botwrap-0.1.3/openaiwrapper/threads.py
+-rw-rw-rw-   0        0        0     3127 2024-04-04 06:39:51.000000 botwrap-0.1.3/openaiwrapper/tools.py
+-rw-rw-rw-   0        0        0     3569 2024-04-04 06:44:47.000000 botwrap-0.1.3/openaiwrapper/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:46:02.458798 botwrap-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2024-04-05 19:44:54.000000 botwrap-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:46:02.450537 botwrap-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 23:19:35.000000 botwrap-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-05 19:32:00.000000 botwrap-0.1.3/tests/test_api_client.py
+-rw-rw-rw-   0        0        0     2746 2024-04-05 19:00:48.000000 botwrap-0.1.3/tests/test_assistants.py
+-rw-rw-rw-   0        0        0     2290 2024-04-05 19:07:26.000000 botwrap-0.1.3/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     2085 2024-04-05 19:03:58.000000 botwrap-0.1.3/tests/test_files.py
+-rw-rw-rw-   0        0        0     2427 2024-04-05 19:05:25.000000 botwrap-0.1.3/tests/test_messages.py
+-rw-rw-rw-   0        0        0     2845 2024-04-05 19:21:07.000000 botwrap-0.1.3/tests/test_openai_wrapper.py
+-rw-rw-rw-   0        0        0     2435 2024-04-05 19:07:10.000000 botwrap-0.1.3/tests/test_runs.py
+-rw-rw-rw-   0        0        0     2858 2024-04-05 19:09:58.000000 botwrap-0.1.3/tests/test_threads.py
+-rw-rw-rw-   0        0        0     2869 2024-04-05 19:16:17.000000 botwrap-0.1.3/tests/test_tools.py
+-rw-rw-rw-   0        0        0     3376 2024-04-05 19:18:51.000000 botwrap-0.1.3/tests/test_utils.py
```

### Comparing `botwrap-0.1.2/PKG-INFO` & `botwrap-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botwrap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A convenient wrapper for the OpenAI API.
 Home-page: https://github.com/BizPrincess/botwrap
 Author: BizPrincess
 Author-email: professionallyjami@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -31,15 +31,15 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3==2.1.0
 
 # botwrap
 
 Project Structure
-openaiwrapper/
+botwrap/
 â”‚
 â”œâ”€â”€ openaiwrapper/       # Main package directory
 â”‚   â”œâ”€â”€ __init__.py      # Initializes the openaiwrapper package
 â”‚   â”œâ”€â”€ api_client.py    # Base module for API interactions
 â”‚   â”œâ”€â”€ assistants.py    # Assistants module
 â”‚   â”œâ”€â”€ threads.py       # Threads module
 â”‚   â”œâ”€â”€ messages.py      # Messages module
```

### Comparing `botwrap-0.1.2/README.md` & `botwrap-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # botwrap
 
 Project Structure
-openaiwrapper/
+botwrap/
 │
 ├── openaiwrapper/       # Main package directory
 │   ├── __init__.py      # Initializes the openaiwrapper package
 │   ├── api_client.py    # Base module for API interactions
 │   ├── assistants.py    # Assistants module
 │   ├── threads.py       # Threads module
 │   ├── messages.py      # Messages module
```

### Comparing `botwrap-0.1.2/botwrap.egg-info/PKG-INFO` & `botwrap-0.1.3/botwrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botwrap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A convenient wrapper for the OpenAI API.
 Home-page: https://github.com/BizPrincess/botwrap
 Author: BizPrincess
 Author-email: professionallyjami@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -31,15 +31,15 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3==2.1.0
 
 # botwrap
 
 Project Structure
-openaiwrapper/
+botwrap/
 â”‚
 â”œâ”€â”€ openaiwrapper/       # Main package directory
 â”‚   â”œâ”€â”€ __init__.py      # Initializes the openaiwrapper package
 â”‚   â”œâ”€â”€ api_client.py    # Base module for API interactions
 â”‚   â”œâ”€â”€ assistants.py    # Assistants module
 â”‚   â”œâ”€â”€ threads.py       # Threads module
 â”‚   â”œâ”€â”€ messages.py      # Messages module
```

### Comparing `botwrap-0.1.2/botwrap.egg-info/SOURCES.txt` & `botwrap-0.1.3/botwrap.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,13 +16,15 @@
 openaiwrapper/runs.py
 openaiwrapper/threads.py
 openaiwrapper/tools.py
 openaiwrapper/utils.py
 tests/__init__.py
 tests/test_api_client.py
 tests/test_assistants.py
+tests/test_exceptions.py
 tests/test_files.py
 tests/test_messages.py
+tests/test_openai_wrapper.py
 tests/test_runs.py
 tests/test_threads.py
 tests/test_tools.py
 tests/test_utils.py
```

### Comparing `botwrap-0.1.2/openaiwrapper/api_client.py` & `botwrap-0.1.3/openaiwrapper/api_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,84 @@
 ##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\api_client.py
-        
-import requests
+
+import aiohttp
 import logging
-from requests.exceptions import HTTPError, RequestException
-from time import sleep
+from aiohttp import ClientResponseError, ClientSession
+from asyncio import sleep
+from functools import wraps
+from .exceptions import OpenAIRequestError  # Ensure this is correctly imported from your package structure
 
-# Define constants for readability
-HTTP_SERVER_ERROR_START = 500
-HTTP_SERVER_ERROR_END = 600
+# Define constants for readability and configuration
 DEFAULT_RETRY_ATTEMPTS = 3
 CONTENT_TYPE_JSON = 'application/json'
+API_BASE_URL = "https://api.openai.com/v1"  # This could also be configurable via an environment variable
 
 # Set up logging
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 handler = logging.StreamHandler()
 formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
-class OpenAIRequestError(Exception):
-    """Exception raised for errors in making API requests to OpenAI."""
-    def __init__(self, message: str, status_code: int):
-        super().__init__(message)
-        self.message = message
-        self.status_code = status_code
+def retry(exceptions, tries=DEFAULT_RETRY_ATTEMPTS, delay=1, backoff=2, jitter=0.1):
+    """A decorator for retrying a function with exponential backoff and jitter."""
+    def decorator(func):
+        @wraps(func)
+        async def wrapper(*args, **kwargs):
+            _tries, _delay = tries, delay
+            while _tries > 0:
+                try:
+                    return await func(*args, **kwargs)
+                except exceptions as e:
+                    _tries -= 1
+                    if _tries == 0:
+                        logger.error(f'Final attempt of {func.__name__} failed due to {e}, no more retries left.')
+                        raise
+                    wait = _delay + jitter * _delay * (random.random() - 0.5)  # Adding jitter
+                    logger.warning(f'Retrying {func.__name__} due to {e}, attempt {tries - _tries} of {tries}. Waiting {wait} seconds.')
+                    await sleep(wait)
+                    _delay *= backoff
+        return wrapper
+    return decorator
 
 class OpenAIAPIClient:
-    def __init__(self, api_key: str, retry_attempts: int = DEFAULT_RETRY_ATTEMPTS):
-        """Initializes an OpenAIAPIClient with an API key and configurable number of retry attempts.
-
-        Args:
-            api_key: API key for authenticating with OpenAI's services.
-            retry_attempts: Number of times to retry a request after server errors (5xx).
-        """
+    def __init__(self, api_key: str, base_url=API_BASE_URL):
         self.api_key = api_key
-        self.base_url = "https://api.openai.com/v1"
-        self.retry_attempts = retry_attempts
+        self.base_url = base_url
+        self.session = None  # Lazy instantiation of ClientSession
 
-    def _make_request(self, method: str, url: str, headers: dict, data: dict = None, files: dict = None, params: dict = None):
-        """Internal function to make the actual request with retry logic.
+    async def __aenter__(self):
+        if not self.session:  # Check if session has already been created
+            self.session = ClientSession()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.close()
+
+    async def close(self):
+        if self.session:
+            await self.session.close()
+            self.session = None
 
-        Args:
-            method: The HTTP method to use ('GET', 'POST', etc.).
-            url: The full URL for the request.
-            headers: Headers to include in the request.
-            data: Data to be sent in the body of the request.
-            files: Files to be sent in the body of the request.
-            params: URL parameters to be sent in the request.
-
-        Returns:
-            A dictionary containing the JSON response.
-
-        Raises:
-            OpenAIRequestError: An error occurred while making the API request.
-        """
-        headers["OpenAI-Beta"] = "assistants=v1"  # Add this line to include the required header
-        for attempt in range(self.retry_attempts):
-            try:
-                if files:
-                    headers.pop("Content-Type", None)  # Let requests handle multipart/form-data
-                response = requests.request(method, url, headers=headers, json=data, files=files, params=params)
-                response.raise_for_status()
-
-                if CONTENT_TYPE_JSON in response.headers.get('Content-Type', ''):
-                    return response.json()
-                else:
-                    raise OpenAIRequestError("Response content type is not JSON.", status_code=response.status_code)
-
-            except HTTPError as e:
-                if HTTP_SERVER_ERROR_START <= e.response.status_code < HTTP_SERVER_ERROR_END and attempt < self.retry_attempts - 1:
-                    sleep(2 ** attempt)  # Exponential backoff
-                else:
-                    logger.error(f"HTTPError: {e.response.status_code}, Message: {e.response.text}")
-                    raise OpenAIRequestError(e.response.text, status_code=e.response.status_code)
-            except RequestException as e:
-                logger.error(f"Request exception: {str(e)}")
-                raise OpenAIRequestError(f"Failed to make a request to OpenAI API: {str(e)}", status_code=0)
-
-
-    def make_api_call(self, endpoint: str, method: str = "GET", data: dict = None, files: dict = None, params: dict = None) -> dict:
-        """Makes an API call to the specified endpoint.
-
-        Args:
-            endpoint: The endpoint of the API to interact with.
-            method: The HTTP method to use ('GET', 'POST', etc.).
-            data: Data to send in the body of the request.
-            files: Files to send in the body of the request.
-            params: URL parameters to send in the request.
-
-        Returns:
-            A dictionary containing the JSON response.
-
-        Raises:
-            OpenAIRequestError: An error occurred while making the API request.
-        """
+    @retry(exceptions=(ClientResponseError,))
+    async def _make_request(self, method: str, url: str, data=None, files=None, params=None):
         headers = {"Authorization": f"Bearer {self.api_key}"}
         if not files:
             headers["Content-Type"] = CONTENT_TYPE_JSON
+        
+        # Ensure self.session is initialized before making a request
+        if not self.session:
+            self.session = ClientSession()
+
+        full_url = f"{self.base_url}/{url}"
+        async with self.session.request(method, full_url, headers=headers, json=data, params=params) as response:
+            if response.status == 429:  # Rate limit handling
+                retry_after = int(response.headers.get("Retry-After", "60"))
+                logger.warning(f"Rate limit exceeded. Retrying after {retry_after} seconds.")
+                await sleep(retry_after)
+                return await self._make_request(method, url, data, files, params)  # Recursive retry after delay
+            response.raise_for_status()  # Raises error for 400 and 500 codes
+            return await response.json()  # Assuming all successful responses are JSON
 
-        url = f"{self.base_url}/{endpoint}"
-
-        return self._make_request(method, url, headers, data, files, params)
+    async def make_api_call(self, endpoint: str, method: str = "GET", data=None, files=None, params=None) -> dict:
+        return await self._make_request(method, endpoint, data=data, files=files, params=params)
```

### Comparing `botwrap-0.1.2/openaiwrapper/files.py` & `botwrap-0.1.3/openaiwrapper/files.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,100 @@
 ##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\files.py
 
 import os
-import requests
+import aiohttp
 import logging
+import asyncio
+import functools
 from .api_client import OpenAIAPIClient, OpenAIRequestError
 
 class FileOperationError(Exception):
     """Custom exception for file operation errors."""
     pass
 
+# Updated retry decorator for async functions
+def retry(func):
+    @functools.wraps(func)
+    async def wrapper(*args, **kwargs):
+        retries = 5
+        base_delay = 0.5  # seconds
+        factor = 2.0
+        for i in range(retries):
+            try:
+                return await func(*args, **kwargs)
+            except (aiohttp.ClientError, OpenAIRequestError) as e:
+                if i < retries - 1:
+                    sleep_time = base_delay * (factor ** i)
+                    logging.warning(f"Retrying in {sleep_time:.2f}s... ({i+1}/{retries})")
+                    await asyncio.sleep(sleep_time)
+                else:
+                    raise e
+    return wrapper
+
 class FileManager:
     def __init__(self, api_client: OpenAIAPIClient):
         self.api_client = api_client
         self.logger = logging.getLogger(__name__)
 
-    def upload_file(self, file_path: str):
-        """Uploads a file to the OpenAI API.
-
-        Args:
-            file_path: Path to the file to be uploaded.
-
-        Returns:
-            The API response for the file upload.
-
-        Raises:
-            FileOperationError: If the file cannot be uploaded.
-        """
+    @retry
+    async def upload_file(self, file_path: str):
+        """Uploads a file to the OpenAI API asynchronously with retry logic."""
         self.validate_file_for_upload(file_path)
         url = f"{self.api_client.base_url}/files"
         headers = {"Authorization": f"Bearer {self.api_client.api_key}"}
-        files = {"file": open(file_path, "rb")}
-        try:
-            response = requests.post(url, headers=headers, files=files)
-            response.raise_for_status()
-            return response.json()
-        except requests.exceptions.HTTPError as e:
-            self.logger.error(f"HTTPError during file upload: {e}")
-            raise FileOperationError(f"HTTPError during file upload: {e}")
-        except Exception as e:
-            self.logger.error(f"Unexpected error during file upload: {e}")
-            raise FileOperationError(f"Unexpected error during file upload: {e}")
-
-    def delete_file(self, file_id: str):
-        """Deletes a specific file by ID.
-
-        Args:
-            file_id: ID of the file to delete.
 
-        Returns:
-            The API response for the file deletion.
-        """
+        with open(file_path, "rb") as file_stream:
+            files = {"file": (os.path.basename(file_path), file_stream)}
+            try:
+                async with aiohttp.ClientSession() as session:
+                    async with session.post(url, headers=headers, data=files) as response:
+                        response.raise_for_status()
+                        return await response.json()
+            except aiohttp.ClientResponseError as e:
+                self.logger.error(f"HTTPError during file upload: {e}")
+                raise FileOperationError(f"HTTPError during file upload: {e.message}")
+            except Exception as e:
+                self.logger.error(f"Unexpected error during file upload: {e}")
+                raise FileOperationError(f"Unexpected error during file upload: {e}")
+
+    @retry
+    async def delete_file(self, file_id: str):
+        """Deletes a specific file by ID asynchronously with retry logic."""
         try:
-            return self.api_client.make_api_call(f"files/{file_id}", method="DELETE")
+            return await self.api_client.make_api_call(f"files/{file_id}", method="DELETE")
         except OpenAIRequestError as e:
             raise FileOperationError(f"Failed to delete file {file_id}: {e}")
 
-    def get_file_content(self, file_id: str):
-        """Fetches and returns the content of a specified file.
-
-        Args:
-            file_id: ID of the file whose content is to be fetched.
-
-        Returns:
-            The content of the file.
-        """
+    @retry
+    async def get_file_content(self, file_id: str):
+        """Fetches and returns the content of a specified file asynchronously with retry logic."""
         try:
-            response = self.api_client.make_api_call(f"files/{file_id}/content", method="GET", stream=True)
-            return response.content
+            response = await self.api_client.make_api_call(f"files/{file_id}/content", method="GET", stream=True)
+            return await response.read()
         except OpenAIRequestError as e:
             raise FileOperationError(f"Failed to fetch content for file {file_id}: {e}")
 
-    def list_files(self, **kwargs):
-        """Lists files with optional filtering and sorting.
-
-        Args:
-            **kwargs: Optional arguments that `list_files` function accepts.
-
-        Returns:
-            The API response for listing files.
-        """
+    @retry
+    async def list_files(self, **kwargs):
+        """Lists files with optional filtering and sorting asynchronously with retry logic."""
         params = {key: value for key, value in kwargs.items() if value is not None}
         try:
-            return self.api_client.make_api_call("files", method="GET", params=params)
+            response = await self.api_client.make_api_call("files", method="GET", params=params)
+            return await response.json()
         except OpenAIRequestError as e:
             raise FileOperationError(f"Failed to list files: {e}")
 
     def validate_file_for_upload(self, file_path: str):
         """Validates the file against OpenAI's upload constraints before uploading.
 
         Args:
             file_path: Path to the file to be validated.
 
         Raises:
             ValueError: If the file does not meet the criteria for upload.
         """
+        # This method remains synchronous as it doesn't perform I/O operations
         max_file_size = 52428800  # 50 MB for example
         file_size = os.path.getsize(file_path)
         if file_size > max_file_size:
             raise ValueError("File exceeds the maximum allowed size.")
-        # Additional validations can be added here.
+        # Additional validations can be added here.
```

### Comparing `botwrap-0.1.2/openaiwrapper/runs.py` & `botwrap-0.1.3/openaiwrapper/runs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,55 @@
 ##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\runs.py
 
 import logging
-
+import asyncio  # Use asyncio for async sleep instead of time.sleep
 
 class RunManager:
     def __init__(self, api_client):
-        """Initializes the RunManager with an API client.
-
-        Args:
-            api_client: An instance of APIClient that handles making API calls.
-        """
+        """Initializes the RunManager with an async API client."""
         self.api_client = api_client
         self.logger = logging.getLogger(__name__)
 
-    def create(self, thread_id, assistant_id, **kwargs):
-        """Creates a Run for a Thread with the specified Assistant.
-
-        Args:
-            thread_id: The ID of the thread to create a run for.
-            assistant_id: The ID of the assistant to use for the run.
-            **kwargs: Additional parameters for the run creation.
-
-        Returns:
-            A dictionary containing the response data from the API call.
-        """
+    async def create(self, thread_id, assistant_id, **kwargs):
+        """Creates a Run for a Thread with the specified Assistant asynchronously."""
         data = {"assistant_id": assistant_id, **kwargs}
         try:
-            return self.api_client.make_api_call(f"threads/{thread_id}/runs", method="POST", data=data)
+            response = await self.api_client.make_api_call(f"threads/{thread_id}/runs", method="POST", data=data)
+            return response  # Assuming handle_api_response is handled within the api_client
         except Exception as e:
             self.logger.error(f"Failed to create run for thread {thread_id} with assistant {assistant_id}: {e}")
             raise
 
-    def retrieve(self, thread_id, run_id):
-        """Retrieves details of a specific Run.
-
-        Args:
-            thread_id: The ID of the thread the run belongs to.
-            run_id: The ID of the run to retrieve.
-
-        Returns:
-            A dictionary containing the response data from the API call.
-        """
+    async def retrieve(self, thread_id, run_id):
+        """Asynchronously retrieves details of a specific Run."""
         try:
-            return self.api_client.make_api_call(f"threads/{thread_id}/runs/{run_id}", method="GET")
+            return await self.api_client.make_api_call(f"threads/{thread_id}/runs/{run_id}", method="GET")
         except Exception as e:
             self.logger.error(f"Failed to retrieve run {run_id} from thread {thread_id}: {e}")
             raise
 
-    def list(self, thread_id, **kwargs):
-        """Lists all runs for a specific thread, supporting pagination.
+    async def wait_for_run_completion(self, thread_id, run_id, timeout=300):
+        """Asynchronously waits for a run to complete and returns its status."""
+        start_time = asyncio.get_event_loop().time()
+        while True:
+            run_status = await self.retrieve(thread_id, run_id)
+            if run_status.get('status') == 'completed':
+                self.logger.info("Run completed successfully.")
+                return run_status
+            elif run_status.get('status') == 'failed':
+                self.logger.error("Run failed.")
+                return run_status
+            elif asyncio.get_event_loop().time() - start_time > timeout:
+                self.logger.error("Run timed out.")
+                return None
+            await asyncio.sleep(10)  # Asynchronously wait before the next poll
 
-        Args:
-            thread_id: The ID of the thread to list runs for.
-            **kwargs: Parameters for filtering or pagination.
-
-        Returns:
-            A tuple containing a list of runs and the next page token, if any.
-        """
+    async def list(self, thread_id, **kwargs):
+        """Asynchronously lists all runs for a specific thread, supporting pagination."""
         try:
-            response = self.api_client.make_api_call(f"threads/{thread_id}/runs", method="GET", params=kwargs)
-
+            response = await self.api_client.make_api_call(f"threads/{thread_id}/runs", method="GET", params=kwargs)
             runs = response.get('data')
             next_page_token = response.get('pagination', {}).get('next_page_token')
-
             return runs, next_page_token
         except Exception as e:
             self.logger.error(f"Failed to list runs for thread {thread_id}: {e}")
-            raise
+            raise
```

### Comparing `botwrap-0.1.2/openaiwrapper/utils.py` & `botwrap-0.1.3/openaiwrapper/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 ##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\utils.py
 
 import logging
-from typing import Any, Dict, List
-from requests.models import Response
+import asyncio
+import aiohttp
+import json
 from datetime import datetime
+from typing import Any, Dict, List
 from .exceptions import OpenAIRequestError
 
-# Set up logging
+# Set up structured logging
 logger = logging.getLogger(__name__)
 
-def log_api_call(method: str, url: str, data: Dict[str, Any] = None, status_code: int = None, duration: float = None) -> None:
-    """Logs details of an API call including the request method, URL, optional data, status code, and duration."""
-    logger.info(f"API Request - Method: {method}, URL: {url}, Status Code: {status_code}, Duration: {duration} seconds, Data: {data if data else 'No Data'}")
-
-def handle_http_error(response: Response) -> None:
-    """Handles HTTP errors by raising an OpenAIRequestError with detailed message."""
-    try:
-        json_response = response.json()
-        error_message = json_response.get('error', {}).get('message', 'No error message provided.')
-    except ValueError:  # JSON decoding failed
-        error_message = "Failed to decode JSON response."
-    raise OpenAIRequestError(message=error_message, status_code=response.status_code)
-
-def handle_api_error(response: Dict[str, Any]) -> None:
-    """Logs and raises API errors in a consistent format."""
-    error_message = response.get('error', {}).get('message', 'Unknown error.')
-    error_type = response.get('error', {}).get('type', 'APIError')
-    logger.error(f"{error_type}: {error_message}")
-    raise Exception(f"{error_type}: {error_message}")
+async def handle_http_error(response: aiohttp.ClientResponse) -> None:
+    """Asynchronously handles HTTP errors by raising an OpenAIRequestError with detailed message."""
+    if response.status >= 400:
+        try:
+            json_response = await response.json()
+            error_message = json_response.get('error', {}).get('message', 'No error message provided.')
+            error_type = json_response.get('error', {}).get('type', 'APIError')
+            request_id = response.headers.get('X-Request-ID', 'N/A')
+        except Exception:
+            error_message = await response.text()
+            error_type = 'UnknownError'
+            request_id = 'N/A'
+        
+        raise OpenAIRequestError(message=error_message, status_code=response.status, error_type=error_type, request_id=request_id)
+
+def log_api_call(method: str, url: str, status_code: int = None, duration: float = None, data: Dict[str, Any] = None) -> None:
+    """Logs details of an API call including method, URL, status, duration, and data in a structured format."""
+    log_data = {
+        "event": "APIRequest",
+        "method": method,
+        "url": url,
+        "status_code": status_code,
+        "duration": f"{duration:.2f}s",
+        "data": data or {}
+    }
+    logger.info(json.dumps(log_data))
 
-def validate_response_content_type(response: Response, expected_content_type: str) -> None:
-    """Validates the Content-Type of the response."""
+def validate_response_content_type(response: aiohttp.ClientResponse, expected_content_type: str) -> None:
+    """Validates the Content-Type of the response asynchronously."""
     content_type = response.headers.get('Content-Type', '')
     if expected_content_type not in content_type:
         raise ValueError(f"Unexpected Content-Type: {content_type}, expected {expected_content_type}.")
 
 def format_data_for_request(data: Dict[str, Any]) -> Dict[str, Any]:
     """Formats data to be sent in an API request."""
-    formatted_data = {k: v for k, v in data.items() if v is not None}
-    return formatted_data
+    return {k: v for k, v in data.items() if v is not None}
 
 def validate_list_of_dicts(items: List[Dict[str, Any]], required_keys: List[str]) -> bool:
     """Validates that each dictionary in a list contains all required keys."""
     return all(all(key in item for key in required_keys) for item in items)
 
 def datetime_to_iso(dt: datetime) -> str:
     """Converts a datetime object to an ISO formatted string."""
     return dt.isoformat()
 
 def sanitize_input(input_string: str) -> str:
     """Sanitizes input strings to remove potentially harmful characters or patterns."""
     # Implement specific sanitization rules as needed
     return input_string.strip()
 
-def fetch_all_pages(fetch_page_function, **params) -> List[Dict[str, Any]]:
-    """Utility function to fetch all pages of a paginated API response."""
+async def fetch_all_pages(fetch_page_function, **params) -> List[Dict[str, Any]]:
+    """Utility function to fetch all pages of a paginated API response asynchronously."""
     all_items = []
     page_token = None
-    
+
     while True:
-        response, next_page_token = fetch_page_function(page_token=page_token, **params)
+        try:
+            response, next_page_token = await fetch_page_function(page_token=page_token, **params)
+        except OpenAIRequestError as e:
+            logger.warning(f"Encountered an error: {e}. Retrying...")
+            await asyncio.sleep(1)  # Simple backoff, adjust as needed
+            continue  # Retry the current page fetch
+
         all_items.extend(response)
         if not next_page_token:
             break
         page_token = next_page_token
-    
-    return all_items
+
+    return all_items
```

### Comparing `botwrap-0.1.2/setup.py` & `botwrap-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='botwrap',
-    version='0.1.2',
+    version='0.1.3',
     author='BizPrincess',
     author_email='professionallyjami@gmail.com',
     description='A convenient wrapper for the OpenAI API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BizPrincess/botwrap',
     packages=find_packages(),
```

### Comparing `botwrap-0.1.2/tests/test_runs.py` & `botwrap-0.1.3/openaiwrapper/threads.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-##Path of module being tested C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\runs.py
-##Path of test C:\Users\jamig\OneDrive\Desktop\botwrap\tests\test_runs.py
+##Path C:\Users\jamig\OneDrive\Desktop\botwrap\openaiwrapper\threads.py
 
 import logging
+import asyncio  # Necessary for async operations
 
-
-class RunManager:
+class ThreadManager:
     def __init__(self, api_client):
-        """Initializes the RunManager with an API client.
-
-        Args:
-            api_client: An instance of APIClient that handles making API calls.
-        """
+        """Initializes the ThreadManager with an API client."""
         self.api_client = api_client
         self.logger = logging.getLogger(__name__)
 
-    def create(self, thread_id, assistant_id, **kwargs):
-        """Creates a Run for a Thread with the specified Assistant.
+    def _validate_thread_id(self, thread_id):
+        """Validates that a thread ID is provided and not empty."""
+        if not thread_id:
+            raise ValueError("Thread ID must be provided and cannot be empty.")
+
+    async def create(self, **kwargs):
+        """Creates a new thread asynchronously."""
+        self.logger.info("Creating new thread")
+        # Ensure api_client.make_api_call is awaited and thus async
+        return await self.api_client.make_api_call("threads", method="POST", data=kwargs)
+
+    async def retrieve(self, thread_id):
+        """Retrieves a specific thread by ID asynchronously."""
+        self._validate_thread_id(thread_id)
+        self.logger.info(f"Retrieving thread with ID: {thread_id}")
+        return await self.api_client.make_api_call(f"threads/{thread_id}", method="GET")
+
+    async def update(self, thread_id, **kwargs):
+        """Updates a specific thread asynchronously."""
+        self._validate_thread_id(thread_id)
+        self.logger.info(f"Updating thread with ID: {thread_id}")
+        return await self.api_client.make_api_call(f"threads/{thread_id}", method="PATCH", data=kwargs)
+
+    async def delete(self, thread_id):
+        """Deletes a specific thread by ID asynchronously."""
+        self._validate_thread_id(thread_id)
+        self.logger.info(f"Deleting thread with ID: {thread_id}")
+        return await self.api_client.make_api_call(f"threads/{thread_id}", method="DELETE")
+
+    async def list(self, **kwargs):
+        """Lists all threads asynchronously, with optional filtering parameters."""
+        self.logger.info("Listing all threads")
+        return await self.api_client.make_api_call("threads", method="GET", params=kwargs)
+
+    async def list_all_threads(self):
+        """Utility method to fetch and return all threads, handling pagination automatically."""
+        all_threads = []
+        page_token = None
+        is_first_page = True
+        
+        # Continue fetching pages until there are no more pages
+        while is_first_page or page_token:
+            params = {'after': page_token} if page_token else {}
+            page = await self.list(**params)
+            threads_data = page.get('data', [])
+            all_threads.extend(threads_data)
+            
+            # Update variables for next iteration
+            page_token = page.get('pagination', {}).get('next_page_token')
+            is_first_page = False
+            
+        return all_threads
 
-        Args:
-            thread_id: The ID of the thread to create a run for.
-            assistant_id: The ID of the assistant to use for the run.
-            **kwargs: Additional parameters for the run creation.
-
-        Returns:
-            A dictionary containing the response data from the API call.
-        """
-        data = {"assistant_id": assistant_id, **kwargs}
-        try:
-            return self.api_client.make_api_call(f"threads/{thread_id}/runs", method="POST", data=data)
-        except Exception as e:
-            self.logger.error(f"Failed to create run for thread {thread_id} with assistant {assistant_id}: {e}")
-            raise
-
-    def retrieve(self, thread_id, run_id):
-        """Retrieves details of a specific Run.
-
-        Args:
-            thread_id: The ID of the thread the run belongs to.
-            run_id: The ID of the run to retrieve.
-
-        Returns:
-            A dictionary containing the response data from the API call.
-        """
-        try:
-            return self.api_client.make_api_call(f"threads/{thread_id}/runs/{run_id}", method="GET")
-        except Exception as e:
-            self.logger.error(f"Failed to retrieve run {run_id} from thread {thread_id}: {e}")
-            raise
-
-    def list(self, thread_id, **kwargs):
-        """Lists all runs for a specific thread, supporting pagination.
-
-        Args:
-            thread_id: The ID of the thread to list runs for.
-            **kwargs: Parameters for filtering or pagination.
-
-        Returns:
-            A tuple containing a list of runs and the next page token, if any.
-        """
-        try:
-            response = self.api_client.make_api_call(f"threads/{thread_id}/runs", method="GET", params=kwargs)
-
-            runs = response.get('data')
-            next_page_token = response.get('pagination', {}).get('next_page_token')
-
-            return runs, next_page_token
-        except Exception as e:
-            self.logger.error(f"Failed to list runs for thread {thread_id}: {e}")
-            raise
```

