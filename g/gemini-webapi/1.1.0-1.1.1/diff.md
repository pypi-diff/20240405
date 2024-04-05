# Comparing `tmp/gemini-webapi-1.1.0.tar.gz` & `tmp/gemini-webapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-webapi-1.1.0.tar", last modified: Sat Mar 23 20:23:49 2024, max compression
+gzip compressed data, was "gemini-webapi-1.1.1.tar", last modified: Fri Apr  5 03:32:45 2024, max compression
```

## Comparing `gemini-webapi-1.1.0.tar` & `gemini-webapi-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.957217 gemini-webapi-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.957217 gemini-webapi-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.957217 gemini-webapi-1.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    54384 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.957217 gemini-webapi-1.1.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 20:23:49.965217 gemini-webapi-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.957217 gemini-webapi-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    54384 2024-03-23 20:23:49.000000 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-23 20:23:49.000000 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 20:23:49.000000 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-23 20:23:49.000000 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-23 20:23:49.000000 gemini-webapi-1.1.0/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:23:49.961217 gemini-webapi-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-23 20:23:44.000000 gemini-webapi-1.1.0/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.438973 gemini-webapi-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_save_image.py
```

### Comparing `gemini-webapi-1.1.0/.github/workflows/pypi-publish.yml` & `gemini-webapi-1.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/.gitignore` & `gemini-webapi-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/LICENSE` & `gemini-webapi-1.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -629,16 +629,16 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Affero General Public License for more details.
```

### Comparing `gemini-webapi-1.1.0/PKG-INFO` & `gemini-webapi-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.1.0
-Summary: A reverse-engineered async wrapper for Google Gemini web client
+Version: 1.1.1
+Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -634,16 +634,16 @@
         state the exclusion of warranty; and each file should have at least
         the "copyright" line and a pointer to where the full notice is found.
         
             <one line to give the program's name and a brief idea of what it does.>
             Copyright (C) <year>  <name of author>
         
             This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
             This program is distributed in the hope that it will be useful,
             but WITHOUT ANY WARRANTY; without even the implied warranty of
             MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
             GNU Affero General Public License for more details.
         
@@ -666,15 +666,14 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Repository, https://github.com/HanaokaYuzu/Gemini-API
 Project-URL: Issues, https://github.com/HanaokaYuzu/Gemini-API/issues
 Keywords: API,async,Gemini,Bard,Google,Generative AI,LLM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.25.2
@@ -725,28 +724,29 @@
 - [Installation](#installation)
 - [Authentication](#authentication)
 - [Usage](#usage)
   - [Initialization](#initialization)
   - [Generate contents from text](#generate-contents-from-text)
   - [Generate contents from image](#generate-contents-from-image)
   - [Conversations across multiple turns](#conversations-across-multiple-turns)
+  - [Continue previous conversations](#continue-previous-conversations)
   - [Retrieve images in response](#retrieve-images-in-response)
   - [Generate images with ImageFx](#generate-images-with-imagefx)
   - [Save images to local files](#save-images-to-local-files)
   - [Generate contents with Gemini extensions](#generate-contents-with-gemini-extensions)
   - [Check and switch to other reply candidates](#check-and-switch-to-other-reply-candidates)
   - [Control log level](#control-log-level)
 - [References](#references)
 - [Stargazers](#stargazers)
 
 ## Installation
 
 > [!NOTE]
 >
-> This package requires Python 3.10 or later.
+> This package requires Python 3.10 or higher.
 
 Install/update the package with pip.
 
 ```bash
 pip install -U gemini_webapi
 ```
 
@@ -843,14 +843,35 @@
 asyncio.run(main())
 ```
 
 > [!TIP]
 >
 > Same as `GeminiClient.generate_content`, `ChatSession.send_message` also accepts `image` as an optional argument.
 
+### Continue previous conversations
+
+To manually retrieve previous conversations, you can pass previous `ChatSession`'s metadata to `GeminiClient.start_chat` when creating a new `ChatSession`. Alternatively, you can persist previous metadata to a file or db if you need to access them after the current Python process has exited.
+
+```python
+async def main():
+    # Start a new chat session
+    chat = client.start_chat()
+    response = await chat.send_message("Fine weather today")
+
+    # Save chat's metadata
+    previous_session = chat.metadata
+
+    # Load the previous conversation
+    previous_chat = client.start_chat(metadata=previous_session)
+    response = await previous_chat.send_message("What was my previous message?")
+    print(response)
+
+asyncio.run(main())
+```
+
 ### Retrieve images in response
 
 Images in the API's output are stored as a list of `Image` objects. You can access the image title, URL, and description by calling `image.title`, `image.url` and `image.alt` respectively.
 
 ```python
 async def main():
     response = await client.generate_content("Send me some pictures of cats")
```

### Comparing `gemini-webapi-1.1.0/README.md` & `gemini-webapi-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,28 +42,29 @@
 - [Installation](#installation)
 - [Authentication](#authentication)
 - [Usage](#usage)
   - [Initialization](#initialization)
   - [Generate contents from text](#generate-contents-from-text)
   - [Generate contents from image](#generate-contents-from-image)
   - [Conversations across multiple turns](#conversations-across-multiple-turns)
+  - [Continue previous conversations](#continue-previous-conversations)
   - [Retrieve images in response](#retrieve-images-in-response)
   - [Generate images with ImageFx](#generate-images-with-imagefx)
   - [Save images to local files](#save-images-to-local-files)
   - [Generate contents with Gemini extensions](#generate-contents-with-gemini-extensions)
   - [Check and switch to other reply candidates](#check-and-switch-to-other-reply-candidates)
   - [Control log level](#control-log-level)
 - [References](#references)
 - [Stargazers](#stargazers)
 
 ## Installation
 
 > [!NOTE]
 >
-> This package requires Python 3.10 or later.
+> This package requires Python 3.10 or higher.
 
 Install/update the package with pip.
 
 ```bash
 pip install -U gemini_webapi
 ```
 
@@ -160,14 +161,35 @@
 asyncio.run(main())
 ```
 
 > [!TIP]
 >
 > Same as `GeminiClient.generate_content`, `ChatSession.send_message` also accepts `image` as an optional argument.
 
+### Continue previous conversations
+
+To manually retrieve previous conversations, you can pass previous `ChatSession`'s metadata to `GeminiClient.start_chat` when creating a new `ChatSession`. Alternatively, you can persist previous metadata to a file or db if you need to access them after the current Python process has exited.
+
+```python
+async def main():
+    # Start a new chat session
+    chat = client.start_chat()
+    response = await chat.send_message("Fine weather today")
+
+    # Save chat's metadata
+    previous_session = chat.metadata
+
+    # Load the previous conversation
+    previous_chat = client.start_chat(metadata=previous_session)
+    response = await previous_chat.send_message("What was my previous message?")
+    print(response)
+
+asyncio.run(main())
+```
+
 ### Retrieve images in response
 
 Images in the API's output are stored as a list of `Image` objects. You can access the image title, URL, and description by calling `image.title`, `image.url` and `image.alt` respectively.
 
 ```python
 async def main():
     response = await client.generate_content("Send me some pictures of cats")
```

#### html2text {}

```diff
@@ -14,23 +14,24 @@
 python_quickstart)'s official API. - **Asynchronous** - Utilizes `asyncio` to
 run generating tasks and return outputs efficiently. ## Table of Contents -
 [Features](#features) - [Table of Contents](#table-of-contents) -
 [Installation](#installation) - [Authentication](#authentication) - [Usage]
 (#usage) - [Initialization](#initialization) - [Generate contents from text]
 (#generate-contents-from-text) - [Generate contents from image](#generate-
 contents-from-image) - [Conversations across multiple turns](#conversations-
-across-multiple-turns) - [Retrieve images in response](#retrieve-images-in-
-response) - [Generate images with ImageFx](#generate-images-with-imagefx) -
-[Save images to local files](#save-images-to-local-files) - [Generate contents
-with Gemini extensions](#generate-contents-with-gemini-extensions) - [Check and
-switch to other reply candidates](#check-and-switch-to-other-reply-candidates)
-- [Control log level](#control-log-level) - [References](#references) -
-[Stargazers](#stargazers) ## Installation > [!NOTE] > > This package requires
-Python 3.10 or later. Install/update the package with pip. ```bash pip install
--U gemini_webapi ``` Optionally, package offers a way to automatically import
+across-multiple-turns) - [Continue previous conversations](#continue-previous-
+conversations) - [Retrieve images in response](#retrieve-images-in-response) -
+[Generate images with ImageFx](#generate-images-with-imagefx) - [Save images to
+local files](#save-images-to-local-files) - [Generate contents with Gemini
+extensions](#generate-contents-with-gemini-extensions) - [Check and switch to
+other reply candidates](#check-and-switch-to-other-reply-candidates) - [Control
+log level](#control-log-level) - [References](#references) - [Stargazers]
+(#stargazers) ## Installation > [!NOTE] > > This package requires Python 3.10
+or higher. Install/update the package with pip. ```bash pip install -
+U gemini_webapi ``` Optionally, package offers a way to automatically import
 cookies from your local browser. To enable this feature, install `browser-
 cookie3` as well. Supported platforms and browsers can be found [here](https://
 github.com/borisbabic/browser_cookie3?tab=readme-ov-file#contribute). ```bash
 pip install -U browser-cookie3 ``` ## Authentication > [!TIP] > > If `browser-
 cookie3` is installed, you can skip this step and go directly to [usage]
 (#usage) section. Just make sure you have logged in to
 gemini.google.com> in your browser. - Go to
@@ -74,18 +75,28 @@
 object and send messages through it. The conversation history will be
 automatically handled and get updated after each turn. ```python async def main
 (): chat = client.start_chat() response1 = await chat.send_message("Briefly
 introduce Europe") response2 = await chat.send_message("What's the population
 there?") print(response1.text, response2.text, sep="\n\n-----------------------
 -----------\n\n") asyncio.run(main()) ``` > [!TIP] > > Same as
 `GeminiClient.generate_content`, `ChatSession.send_message` also accepts
-`image` as an optional argument. ### Retrieve images in response Images in the
-API's output are stored as a list of `Image` objects. You can access the image
-title, URL, and description by calling `image.title`, `image.url` and
-`image.alt` respectively. ```python async def main(): response = await
+`image` as an optional argument. ### Continue previous conversations To
+manually retrieve previous conversations, you can pass previous `ChatSession`'s
+metadata to `GeminiClient.start_chat` when creating a new `ChatSession`.
+Alternatively, you can persist previous metadata to a file or db if you need to
+access them after the current Python process has exited. ```python async def
+main(): # Start a new chat session chat = client.start_chat() response = await
+chat.send_message("Fine weather today") # Save chat's metadata previous_session
+= chat.metadata # Load the previous conversation previous_chat =
+client.start_chat(metadata=previous_session) response = await
+previous_chat.send_message("What was my previous message?") print(response)
+asyncio.run(main()) ``` ### Retrieve images in response Images in the API's
+output are stored as a list of `Image` objects. You can access the image title,
+URL, and description by calling `image.title`, `image.url` and `image.alt`
+respectively. ```python async def main(): response = await
 client.generate_content("Send me some pictures of cats") for image in
 response.images: print(image, "\n\n----------------------------------\n")
 asyncio.run(main()) ``` ### Generate images with ImageFx In February 2022,
 Google introduced a new AI image generator called ImageFx and integrated it
 into Gemini. You can ask Gemini to generate images with ImageFx simply by
 natural language. > [!IMPORTANT] > > Google has some limitations on the image
 generation feature in Gemini, so its availability could be different per
```

### Comparing `gemini-webapi-1.1.0/assets/banner.png` & `gemini-webapi-1.1.1/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/assets/logo.svg` & `gemini-webapi-1.1.1/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/client.py` & `gemini-webapi-1.1.1/src/gemini_webapi/client.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/constants.py` & `gemini-webapi-1.1.1/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/exceptions.py` & `gemini-webapi-1.1.1/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/types/candidate.py` & `gemini-webapi-1.1.1/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/types/image.py` & `gemini-webapi-1.1.1/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/types/modeloutput.py` & `gemini-webapi-1.1.1/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/utils/get_access_token.py` & `gemini-webapi-1.1.1/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini-webapi-1.1.1/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/utils/logger.py` & `gemini-webapi-1.1.1/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini-webapi-1.1.1/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi/utils/upload_file.py` & `gemini-webapi-1.1.1/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi.egg-info/PKG-INFO` & `gemini-webapi-1.1.1/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.1.0
-Summary: A reverse-engineered async wrapper for Google Gemini web client
+Version: 1.1.1
+Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -634,16 +634,16 @@
         state the exclusion of warranty; and each file should have at least
         the "copyright" line and a pointer to where the full notice is found.
         
             <one line to give the program's name and a brief idea of what it does.>
             Copyright (C) <year>  <name of author>
         
             This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
             This program is distributed in the hope that it will be useful,
             but WITHOUT ANY WARRANTY; without even the implied warranty of
             MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
             GNU Affero General Public License for more details.
         
@@ -666,15 +666,14 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Repository, https://github.com/HanaokaYuzu/Gemini-API
 Project-URL: Issues, https://github.com/HanaokaYuzu/Gemini-API/issues
 Keywords: API,async,Gemini,Bard,Google,Generative AI,LLM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.25.2
@@ -725,28 +724,29 @@
 - [Installation](#installation)
 - [Authentication](#authentication)
 - [Usage](#usage)
   - [Initialization](#initialization)
   - [Generate contents from text](#generate-contents-from-text)
   - [Generate contents from image](#generate-contents-from-image)
   - [Conversations across multiple turns](#conversations-across-multiple-turns)
+  - [Continue previous conversations](#continue-previous-conversations)
   - [Retrieve images in response](#retrieve-images-in-response)
   - [Generate images with ImageFx](#generate-images-with-imagefx)
   - [Save images to local files](#save-images-to-local-files)
   - [Generate contents with Gemini extensions](#generate-contents-with-gemini-extensions)
   - [Check and switch to other reply candidates](#check-and-switch-to-other-reply-candidates)
   - [Control log level](#control-log-level)
 - [References](#references)
 - [Stargazers](#stargazers)
 
 ## Installation
 
 > [!NOTE]
 >
-> This package requires Python 3.10 or later.
+> This package requires Python 3.10 or higher.
 
 Install/update the package with pip.
 
 ```bash
 pip install -U gemini_webapi
 ```
 
@@ -843,14 +843,35 @@
 asyncio.run(main())
 ```
 
 > [!TIP]
 >
 > Same as `GeminiClient.generate_content`, `ChatSession.send_message` also accepts `image` as an optional argument.
 
+### Continue previous conversations
+
+To manually retrieve previous conversations, you can pass previous `ChatSession`'s metadata to `GeminiClient.start_chat` when creating a new `ChatSession`. Alternatively, you can persist previous metadata to a file or db if you need to access them after the current Python process has exited.
+
+```python
+async def main():
+    # Start a new chat session
+    chat = client.start_chat()
+    response = await chat.send_message("Fine weather today")
+
+    # Save chat's metadata
+    previous_session = chat.metadata
+
+    # Load the previous conversation
+    previous_chat = client.start_chat(metadata=previous_session)
+    response = await previous_chat.send_message("What was my previous message?")
+    print(response)
+
+asyncio.run(main())
+```
+
 ### Retrieve images in response
 
 Images in the API's output are stored as a list of `Image` objects. You can access the image title, URL, and description by calling `image.title`, `image.url` and `image.alt` respectively.
 
 ```python
 async def main():
     response = await client.generate_content("Send me some pictures of cats")
```

### Comparing `gemini-webapi-1.1.0/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini-webapi-1.1.1/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/tests/test_client_features.py` & `gemini-webapi-1.1.1/tests/test_client_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,25 @@
         self.assertTrue(response1.text)
         logger.debug(response1.text)
         response2 = await chat.send_message("What's the population there?")
         self.assertTrue(response2.text)
         logger.debug(response2.text)
 
     @logger.catch(reraise=True)
+    async def test_retrieve_previous_conversation(self):
+        chat = self.geminiclient.start_chat()
+        await chat.send_message("Fine weather today")
+        self.assertTrue(len(chat.metadata) == 3)
+        previous_session = chat.metadata
+        logger.debug(previous_session)
+        previous_chat = self.geminiclient.start_chat(metadata=previous_session)
+        response = await previous_chat.send_message("What was my previous message?")
+        logger.debug(response)
+
+    @logger.catch(reraise=True)
     async def test_chatsession_with_image(self):
         chat = self.geminiclient.start_chat()
         response1 = await chat.send_message(
             "Describe the image", image="assets/banner.png"
         )
         self.assertTrue(response1.text)
         logger.debug(response1.text)
```

### Comparing `gemini-webapi-1.1.0/tests/test_rotate_cookies.py` & `gemini-webapi-1.1.1/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.0/tests/test_save_image.py` & `gemini-webapi-1.1.1/tests/test_save_image.py`

 * *Files identical despite different names*

