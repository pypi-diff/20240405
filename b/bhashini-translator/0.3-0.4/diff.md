# Comparing `tmp/bhashini_translator-0.3.tar.gz` & `tmp/bhashini_translator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhashini_translator-0.3.tar", last modified: Thu Mar 21 11:57:28 2024, max compression
+gzip compressed data, was "bhashini_translator-0.4.tar", last modified: Fri Apr  5 13:44:45 2024, max compression
```

## Comparing `bhashini_translator-0.3.tar` & `bhashini_translator-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-03-21 11:57:28.178408 bhashini_translator-0.3/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     1066 2024-01-14 12:40:09.000000 bhashini_translator-0.3/LICENSE
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      421 2024-03-21 11:57:28.178408 bhashini_translator-0.3/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     2314 2024-01-19 12:17:11.000000 bhashini_translator-0.3/README.md
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2024-03-21 11:57:28.178408 bhashini_translator-0.3/setup.cfg
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      595 2024-03-21 11:57:25.000000 bhashini_translator-0.3/setup.py
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-03-21 11:57:28.178408 bhashini_translator-0.3/src/
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-03-21 11:57:28.178408 bhashini_translator-0.3/src/bhashini_translator/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       42 2024-01-14 12:40:09.000000 bhashini_translator-0.3/src/bhashini_translator/__init__.py
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     4201 2024-03-20 14:24:07.000000 bhashini_translator-0.3/src/bhashini_translator/bhashini_translator.py
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       89 2024-01-14 12:40:09.000000 bhashini_translator-0.3/src/bhashini_translator/config.py
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     2108 2024-03-21 11:23:41.000000 bhashini_translator-0.3/src/bhashini_translator/payloads.py
--rw-rw-r--   0 kanak     (1000) kanak     (1000)     1955 2024-01-19 05:53:12.000000 bhashini_translator-0.3/src/bhashini_translator/pipeline_config.py
-drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-03-21 11:57:28.178408 bhashini_translator-0.3/src/bhashini_translator.egg-info/
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      421 2024-03-21 11:57:28.000000 bhashini_translator-0.3/src/bhashini_translator.egg-info/PKG-INFO
--rw-rw-r--   0 kanak     (1000) kanak     (1000)      456 2024-03-21 11:57:28.000000 bhashini_translator-0.3/src/bhashini_translator.egg-info/SOURCES.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2024-03-21 11:57:28.000000 bhashini_translator-0.3/src/bhashini_translator.egg-info/dependency_links.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)        9 2024-03-21 11:57:28.000000 bhashini_translator-0.3/src/bhashini_translator.egg-info/requires.txt
--rw-rw-r--   0 kanak     (1000) kanak     (1000)       20 2024-03-21 11:57:28.000000 bhashini_translator-0.3/src/bhashini_translator.egg-info/top_level.txt
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-04-05 13:44:45.222867 bhashini_translator-0.4/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     1066 2024-01-14 12:40:09.000000 bhashini_translator-0.4/LICENSE
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      421 2024-04-05 13:44:45.222867 bhashini_translator-0.4/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     2314 2024-01-19 12:17:11.000000 bhashini_translator-0.4/README.md
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       38 2024-04-05 13:44:45.222867 bhashini_translator-0.4/setup.cfg
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      595 2024-04-05 13:44:28.000000 bhashini_translator-0.4/setup.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-04-05 13:44:45.222867 bhashini_translator-0.4/src/
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-04-05 13:44:45.222867 bhashini_translator-0.4/src/bhashini_translator/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      150 2024-03-30 11:41:35.000000 bhashini_translator-0.4/src/bhashini_translator/__init__.py
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     4715 2024-04-05 01:10:46.000000 bhashini_translator-0.4/src/bhashini_translator/bhashini_translator.py
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       89 2024-01-14 12:40:09.000000 bhashini_translator-0.4/src/bhashini_translator/config.py
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     2657 2024-03-30 11:34:46.000000 bhashini_translator-0.4/src/bhashini_translator/payloads.py
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)     1955 2024-01-19 05:53:12.000000 bhashini_translator-0.4/src/bhashini_translator/pipeline_config.py
+drwxrwxr-x   0 kanak     (1000) kanak     (1000)        0 2024-04-05 13:44:45.222867 bhashini_translator-0.4/src/bhashini_translator.egg-info/
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      421 2024-04-05 13:44:45.000000 bhashini_translator-0.4/src/bhashini_translator.egg-info/PKG-INFO
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)      456 2024-04-05 13:44:45.000000 bhashini_translator-0.4/src/bhashini_translator.egg-info/SOURCES.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)        1 2024-04-05 13:44:45.000000 bhashini_translator-0.4/src/bhashini_translator.egg-info/dependency_links.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)        9 2024-04-05 13:44:45.000000 bhashini_translator-0.4/src/bhashini_translator.egg-info/requires.txt
+-rw-rw-r--   0 kanak     (1000) kanak     (1000)       20 2024-04-05 13:44:45.000000 bhashini_translator-0.4/src/bhashini_translator.egg-info/top_level.txt
```

### Comparing `bhashini_translator-0.3/LICENSE` & `bhashini_translator-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bhashini_translator-0.3/README.md` & `bhashini_translator-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bhashini_translator-0.3/setup.py` & `bhashini_translator-0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bhashini_translator",
-    version="0.3",
+    version="0.4",
     packages=["bhashini_translator"],
     install_requires=["requests"],
     author="Rajesh Pethe",
     author_email="rajesh.pethe@gmail.com",
     description="Python client interface to leverage Bhashini(ULCA) APIs.",
     readme="README.md",
     long_description="Python client interface to leverage Bhashini(ULCA) APIs.",
```

### Comparing `bhashini_translator-0.3/src/bhashini_translator/bhashini_translator.py` & `bhashini_translator-0.4/src/bhashini_translator/bhashini_translator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests, os
 import json
-from .config import ulcaEndPoint
-from .payloads import Payloads
+from bhashini_translator.config import ulcaEndPoint
+from bhashini_translator.payloads import Payloads
 
 
 class Bhashini(Payloads):
     ulcaUserId: str
     ulcaApiKey: str
     sourceLanguage: str
     targetLanguage: str
@@ -79,26 +79,40 @@
 
         pipelineResponse = self.compute_response(requestPayload)
         return (
             pipelineResponse.get("pipelineResponse")[0].get("output")[0].get("source")
         )
 
     def nmt_tts(self, text: str) -> str:
+        # TODO: Fix use of 'gender' in pipeline
         requestPayload = self.nmt_tts_payload(text)
 
         if not self.pipeLineData:
             raise ValueError("Pipe Line data is not available")
 
         pipelineResponse = self.compute_response(requestPayload)
         return (
             pipelineResponse.get("pipelineResponse")[1]
             .get("audio")[0]
             .get("audioContent")
         )
 
+    def asr_nmt_tts(self, base64String: str) -> str:
+        requestPayload = self.asr_nmt_tts_payload(base64String)
+
+        if not self.pipeLineData:
+            raise ValueError("Pipe Line data is not available")
+
+        pipelineResponse = self.compute_response(requestPayload)
+        return (
+            pipelineResponse.get("pipelineResponse")[2]
+            .get("audio")[0]
+            .get("audioContent")
+        )
+
     def compute_response(self, requestPayload: json) -> json:
         if not self.pipeLineData:
             raise ValueError("Intitialize pipe line data first!")
 
         callbackUrl = self.pipeLineData.get("pipelineInferenceAPIEndPoint").get(
             "callbackUrl"
         )
```

### Comparing `bhashini_translator-0.3/src/bhashini_translator/payloads.py` & `bhashini_translator-0.4/src/bhashini_translator/payloads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from .pipeline_config import PipelineConfig
+from bhashini_translator.pipeline_config import PipelineConfig
 
 
 class Payloads(PipelineConfig):
     def nmt_payload(self, text: str) -> json:
         return json.dumps(
             {
                 "pipelineTasks": [
@@ -61,7 +61,22 @@
                 ],
                 "pipelineRequestConfig": {
                     "pipelineId": self.pipeLineId,
                 },
                 "inputData": {"input": [{"source": text}]},
             }
         )
+
+    def asr_nmt_tts_payload(self, base64String: str) -> json:
+        return json.dumps(
+            {
+                "pipelineTasks": [
+                    self.getPipeLineConfig("asr"),
+                    self.getPipeLineConfig("translation"),
+                    self.getPipeLineConfig("tts"),
+                ],
+                "pipelineRequestConfig": {
+                    "pipelineId": self.pipeLineId,
+                },
+                "inputData": {"audio": [{"audioContent": base64String}]},
+            }
+        )
```

### Comparing `bhashini_translator-0.3/src/bhashini_translator/pipeline_config.py` & `bhashini_translator-0.4/src/bhashini_translator/pipeline_config.py`

 * *Files identical despite different names*

