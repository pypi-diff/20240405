# Comparing `tmp/openai_requests_utils-0.0.7.tar.gz` & `tmp/openai_requests_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_requests_utils-0.0.7.tar", last modified: Thu Mar 14 21:12:38 2024, max compression
+gzip compressed data, was "openai_requests_utils-0.0.8.tar", last modified: Fri Apr  5 17:16:20 2024, max compression
```

## Comparing `openai_requests_utils-0.0.7.tar` & `openai_requests_utils-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 21:12:38.045200 openai_requests_utils-0.0.7/
--rw-rw-rw-   0        0        0     1086 2024-02-01 19:48:18.000000 openai_requests_utils-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      974 2024-03-14 21:12:38.044201 openai_requests_utils-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-02-01 20:47:35.000000 openai_requests_utils-0.0.7/README.md
--rw-rw-rw-   0        0        0      499 2024-03-14 21:11:58.000000 openai_requests_utils-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 21:12:38.045200 openai_requests_utils-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 21:12:38.027199 openai_requests_utils-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 21:12:38.036199 openai_requests_utils-0.0.7/src/openai_requests_utils/
--rw-rw-rw-   0        0        0      139 2024-02-01 22:09:07.000000 openai_requests_utils-0.0.7/src/openai_requests_utils/__init__.py
--rw-rw-rw-   0        0        0    13074 2024-03-14 21:11:08.000000 openai_requests_utils-0.0.7/src/openai_requests_utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:12:38.044201 openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/
--rw-rw-rw-   0        0        0      974 2024-03-14 21:12:38.000000 openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-03-14 21:12:38.000000 openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 21:12:38.000000 openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-14 21:12:38.000000 openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 17:16:20.540618 openai_requests_utils-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2024-02-01 19:48:18.000000 openai_requests_utils-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      974 2024-04-05 17:16:20.539618 openai_requests_utils-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-02-01 20:47:35.000000 openai_requests_utils-0.0.8/README.md
+-rw-rw-rw-   0        0        0      499 2024-04-05 17:16:09.000000 openai_requests_utils-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:16:20.540618 openai_requests_utils-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 17:16:20.527618 openai_requests_utils-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 17:16:20.530618 openai_requests_utils-0.0.8/src/openai_requests_utils/
+-rw-rw-rw-   0        0        0      139 2024-02-01 22:09:07.000000 openai_requests_utils-0.0.8/src/openai_requests_utils/__init__.py
+-rw-rw-rw-   0        0        0    13202 2024-04-05 17:14:43.000000 openai_requests_utils-0.0.8/src/openai_requests_utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:16:20.539618 openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/
+-rw-rw-rw-   0        0        0      974 2024-04-05 17:16:20.000000 openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-05 17:16:20.000000 openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:16:20.000000 openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-05 17:16:20.000000 openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/top_level.txt
```

### Comparing `openai_requests_utils-0.0.7/LICENSE` & `openai_requests_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_requests_utils-0.0.7/PKG-INFO` & `openai_requests_utils-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_requests_utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Useful utils to use with openai models
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openai_requests_utils-0.0.7/README.md` & `openai_requests_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `openai_requests_utils-0.0.7/src/openai_requests_utils/utils.py` & `openai_requests_utils-0.0.8/src/openai_requests_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
         params["presence_penalty"] = presence_penalty
 
     formatted_params = json.dumps(params, ensure_ascii=False)
     encoded_params = formatted_params.encode('utf-8')
 
     response = requests.post('https://api.openai.com/v1/chat/completions', headers=headers, data=encoded_params, timeout=timeout, stream=True)
 
+    if response.status_code != 200:
+        raise Exception(f"Error in OAI call: {response.status_code} - {response.text}")
+
     # Dictionary to hold the log data
     oai_call_log = {
         "id": "",
         "object": "",
         "created": "",
         "model": model,
         "temperature": temperature,
```

### Comparing `openai_requests_utils-0.0.7/src/openai_requests_utils.egg-info/PKG-INFO` & `openai_requests_utils-0.0.8/src/openai_requests_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_requests_utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Useful utils to use with openai models
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

