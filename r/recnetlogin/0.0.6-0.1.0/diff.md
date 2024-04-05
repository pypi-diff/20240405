# Comparing `tmp/recnetlogin-0.0.6.tar.gz` & `tmp/recnetlogin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recnetlogin-0.0.6.tar", last modified: Sun Mar  5 10:03:45 2023, max compression
+gzip compressed data, was "recnetlogin-0.1.0.tar", last modified: Fri Apr  5 16:24:54 2024, max compression
```

## Comparing `recnetlogin-0.0.6.tar` & `recnetlogin-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 10:03:45.773087 recnetlogin-0.0.6/
--rw-rw-rw-   0        0        0     1064 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1929 2023-03-05 10:03:45.773087 recnetlogin-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1299 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/README.md
--rw-rw-rw-   0        0        0      752 2023-03-05 10:03:26.000000 recnetlogin-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-05 10:03:45.721316 recnetlogin-0.0.6/recnetlogin/
--rw-rw-rw-   0        0        0       80 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/__init__.py
--rw-rw-rw-   0        0        0     1366 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/api_info.py
--rw-rw-rw-   0        0        0     2834 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/async_client.py
--rw-rw-rw-   0        0        0      598 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/base_client.py
--rw-rw-rw-   0        0        0     1417 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/exceptions.py
--rw-rw-rw-   0        0        0     1845 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/helpers.py
--rw-rw-rw-   0        0        0     2537 2022-10-31 11:52:06.000000 recnetlogin-0.0.6/recnetlogin/sync_client.py
-drwxrwxrwx   0        0        0        0 2023-03-05 10:03:45.772085 recnetlogin-0.0.6/recnetlogin.egg-info/
--rw-rw-rw-   0        0        0     1929 2023-03-05 10:03:45.000000 recnetlogin-0.0.6/recnetlogin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-03-05 10:03:45.000000 recnetlogin-0.0.6/recnetlogin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 10:03:45.000000 recnetlogin-0.0.6/recnetlogin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-03-05 10:03:45.000000 recnetlogin-0.0.6/recnetlogin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-05 10:03:45.000000 recnetlogin-0.0.6/recnetlogin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-05 10:03:45.773087 recnetlogin-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 16:24:54.153878 recnetlogin-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-29 17:35:01.000000 recnetlogin-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3485 2024-04-05 16:24:54.152371 recnetlogin-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2024-04-05 16:23:03.000000 recnetlogin-0.1.0/README.md
+-rw-rw-rw-   0        0        0      721 2024-04-05 16:18:00.000000 recnetlogin-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:24:54.153878 recnetlogin-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 16:24:54.119342 recnetlogin-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 16:24:54.130388 recnetlogin-0.1.0/src/recnetlogin/
+-rw-rw-rw-   0        0        0       33 2023-06-29 17:38:02.000000 recnetlogin-0.1.0/src/recnetlogin/__init__.py
+-rw-rw-rw-   0        0        0     4647 2024-04-05 16:02:32.000000 recnetlogin-0.1.0/src/recnetlogin/client.py
+-rw-rw-rw-   0        0        0      886 2023-06-29 17:37:04.000000 recnetlogin-0.1.0/src/recnetlogin/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:24:54.151374 recnetlogin-0.1.0/src/recnetlogin.egg-info/
+-rw-rw-rw-   0        0        0     3485 2024-04-05 16:24:54.000000 recnetlogin-0.1.0/src/recnetlogin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-05 16:24:54.000000 recnetlogin-0.1.0/src/recnetlogin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:24:54.000000 recnetlogin-0.1.0/src/recnetlogin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-05 16:24:54.000000 recnetlogin-0.1.0/src/recnetlogin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 16:24:54.000000 recnetlogin-0.1.0/src/recnetlogin.egg-info/top_level.txt
```

### Comparing `recnetlogin-0.0.6/LICENSE.txt` & `recnetlogin-0.1.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Jegarde
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Jesse Nieminen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

