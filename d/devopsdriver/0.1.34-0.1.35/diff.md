# Comparing `tmp/devopsdriver-0.1.34.tar.gz` & `tmp/devopsdriver-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.34.tar", last modified: Tue Apr  2 00:28:54 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.35.tar", last modified: Thu Apr  4 20:13:42 2024, max compression
```

## Comparing `devopsdriver-0.1.34.tar` & `devopsdriver-0.1.35.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.710596 devopsdriver-0.1.34/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.34/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)     4927 2024-04-02 00:28:54.710327 devopsdriver-0.1.34/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     2429 2024-04-02 00:28:23.000000 devopsdriver-0.1.34/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.708654 devopsdriver-0.1.34/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)       87 2024-04-02 00:28:09.000000 devopsdriver-0.1.34/devopsdriver/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)    12690 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/devopsdriver/settings.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.710075 devopsdriver-0.1.34/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)     4927 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      284 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       30 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1226 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-02 00:28:54.710653 devopsdriver-0.1.34/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.709614 devopsdriver-0.1.34/tests/
--rw-r--r--   0 marcp      (501) staff       (20)    12527 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/tests/test_settings.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.446279 devopsdriver-0.1.35/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.35/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)     5000 2024-04-04 20:13:42.446066 devopsdriver-0.1.35/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     2431 2024-04-04 20:12:27.000000 devopsdriver-0.1.35/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.440270 devopsdriver-0.1.35/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      113 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.444310 devopsdriver-0.1.35/devopsdriver/azure/
+-rw-r--r--   0 marcp      (501) staff       (20)      381 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/devopsdriver/azure/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1867 2024-04-03 21:36:46.000000 devopsdriver-0.1.35/devopsdriver/azure/clients.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.444847 devopsdriver-0.1.35/devopsdriver/azure/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)      107 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/devopsdriver/azure/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2954 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/devopsdriver/azure/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     7777 2024-04-03 16:25:55.000000 devopsdriver-0.1.35/devopsdriver/azure/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1445 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/devopsdriver/azure/workitem/workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12865 2024-04-03 21:29:38.000000 devopsdriver-0.1.35/devopsdriver/settings.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.445806 devopsdriver-0.1.35/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)     5000 2024-04-04 20:13:42.000000 devopsdriver-0.1.35/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)      626 2024-04-04 20:13:42.000000 devopsdriver-0.1.35/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-04 20:13:42.000000 devopsdriver-0.1.35/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       71 2024-04-04 20:13:42.000000 devopsdriver-0.1.35/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-04 20:13:42.000000 devopsdriver-0.1.35/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1318 2024-04-03 01:14:37.000000 devopsdriver-0.1.35/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-04 20:13:42.446337 devopsdriver-0.1.35/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-04 20:13:42.445598 devopsdriver-0.1.35/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     5343 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4202 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/tests/test_azure_workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1742 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2389 2024-04-04 20:11:44.000000 devopsdriver-0.1.35/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)    11540 2024-04-03 22:02:08.000000 devopsdriver-0.1.35/tests/test_settings.py
```

### Comparing `devopsdriver-0.1.34/LICENSE` & `devopsdriver-0.1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.34/PKG-INFO` & `devopsdriver-0.1.35/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.34
+Version: 0.1.35
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -44,29 +44,33 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.0.0
+Requires-Dist: setuptools==69.0.2
+Requires-Dist: azure-devops==7.1.0b4
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.35&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.35/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
+[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
+[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
 [![status sheild](https://img.shields.io/static/v1?label=test+coverage&message=99%&color=active&style=plastic)](https://github.com/marcpage/devops-driver/blob/main/Makefile#L4)
 [![issues sheild](https://img.shields.io/github/issues-raw/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/pulls)
-[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
-[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![follow sheild](https://img.shields.io/github/followers/marcpage?label=Follow&style=social)](https://github.com/marcpage?tab=followers)
 [![watch sheild](https://img.shields.io/github/watchers/marcpage/devops-driver?label=Watch&style=social)](https://github.com/marcpage/devops-driver/watchers)
 
 # devops-driver
 
 Devops-driver is a set of tools to help streamline developer's experience. It is a collection of tools to help gain insights into various processes.
+
```

### Comparing `devopsdriver-0.1.34/README.md` & `devopsdriver-0.1.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.35&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.35/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
+[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
+[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
 [![status sheild](https://img.shields.io/static/v1?label=test+coverage&message=99%&color=active&style=plastic)](https://github.com/marcpage/devops-driver/blob/main/Makefile#L4)
 [![issues sheild](https://img.shields.io/github/issues-raw/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/pulls)
-[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
-[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![follow sheild](https://img.shields.io/github/followers/marcpage?label=Follow&style=social)](https://github.com/marcpage?tab=followers)
 [![watch sheild](https://img.shields.io/github/watchers/marcpage/devops-driver?label=Watch&style=social)](https://github.com/marcpage/devops-driver/watchers)
 
 # devops-driver
 
 Devops-driver is a set of tools to help streamline developer's experience. It is a collection of tools to help gain insights into various processes.
+
```

### Comparing `devopsdriver-0.1.34/devopsdriver/settings.py` & `devopsdriver-0.1.35/devopsdriver/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,17 @@
             key (str): The dotted key
 
         Returns:
             bool: True if the key exists
         """
         return self.__lookup(key, check=True)
 
+    def __contains__(self, key: str) -> bool:
+        return self.has(key)
+
     def __getitem__(self, key: str) -> any:
         if not self.has(key):
             raise KeyError(key)
 
         return self.get(key)
 
     @staticmethod
@@ -358,23 +361,27 @@
 
 def main() -> None:
     """Get settings values"""
     settings = Settings(__file__, dirname(dirname(__file__))).key("secrets")
 
     args = list(ARGV[1:])
 
-    if "--set_secrets" in args:
-        args.remove("--set_secrets")
+    if "--secrets" in args:
+        args.remove("--secrets")
 
         for secret, key in settings.secrets.items():
+            PRINT(f"secret: {secret}  key: {key}")
+
             if not settings.has(secret):
                 value = GET_PASS(f"{secret} ({key}): ")
 
                 if value:
                     SET_PASSWORD(*Settings.split_key(key), value)
+            else:
+                PRINT("\tValue set")
 
     for arg in args:
         PRINT(settings.get(arg))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `devopsdriver-0.1.34/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.35/devopsdriver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.34
+Version: 0.1.35
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -44,29 +44,33 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.0.0
+Requires-Dist: setuptools==69.0.2
+Requires-Dist: azure-devops==7.1.0b4
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.35&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.35/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
+[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
+[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
 [![status sheild](https://img.shields.io/static/v1?label=test+coverage&message=99%&color=active&style=plastic)](https://github.com/marcpage/devops-driver/blob/main/Makefile#L4)
 [![issues sheild](https://img.shields.io/github/issues-raw/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/pulls)
-[![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
-[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![follow sheild](https://img.shields.io/github/followers/marcpage?label=Follow&style=social)](https://github.com/marcpage?tab=followers)
 [![watch sheild](https://img.shields.io/github/watchers/marcpage/devops-driver?label=Watch&style=social)](https://github.com/marcpage/devops-driver/watchers)
 
 # devops-driver
 
 Devops-driver is a set of tools to help streamline developer's experience. It is a collection of tools to help gain insights into various processes.
+
```

### Comparing `devopsdriver-0.1.34/pyproject.toml` & `devopsdriver-0.1.35/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 requires-python = ">= 3.10"
 dependencies = [
   "PyYAML==6.0.1",
   "keyring==25.0.0",
+  "setuptools==69.0.2",  # neded for azure-devops to use 7.1 API
+  "azure-devops==7.1.0b4",
 ]
 keywords = ["azure", "devops", "jira", "confluence", "email", "pipelines", "tools"]
 classifiers=[
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `devopsdriver-0.1.34/tests/test_settings.py` & `devopsdriver-0.1.35/tests/test_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,21 @@
 #!/usr/bin/env python3
 
 """ Tests Settings class """
 
 from tempfile import TemporaryDirectory
-from os.path import join, splitext, dirname
-from os import makedirs
-from json import dump
+from os.path import join
 from string import ascii_lowercase
 from itertools import product
 
-from yaml import safe_dump
+from helpers import setup_settings, ensure, write
 
 import devopsdriver.settings as settings
 
 
-def __setup_settings(os: str = "Linux", shared: str = "test", **pref_dirs) -> None:
-    settings.ENVIRON = {}
-    settings.ARGV = []
-    settings.SYSTEM = lambda: os
-    settings.SHARED = shared
-    settings.PRINT = lambda s: s
-    settings.GET_PASSWORD = lambda s, n: f"{s}:{n}"
-    settings.GET_PASS = lambda p: p
-    settings.SET_PASSWORD = lambda s, n, p: f"{s} {n} {p}"
-    # settings.MAKEDIRS = lambda p: p
-    # settings.Settings.FORMATS = None
-    settings.Settings.PREF_DIR = pref_dirs
-
-
-def ensure(directory: str) -> str:
-    """Ensures that a directory exists before using
-
-    Args:
-        directory (str): The directory to create
-
-    Returns:
-        str: The directory that now exists
-    """
-    makedirs(directory, exist_ok=True)
-    return directory
-
-
-def __write(path: str, **options) -> None:
-    ensure(dirname(path))
-
-    with open(path, "w", encoding="utf-8") as settings_file:
-        if splitext(path)[1] == ".json":
-            dump(options, settings_file)
-        else:
-            safe_dump(options, settings_file)
-
-
 def __setup_files(directory: str, dir1: str, dir2: str) -> None:
     """
     Priorities:
         <dir>/main.yml a
         <dir>/main.yaml b
         <dir>/main.json c
         <dir1>/main.yml d
@@ -82,40 +43,40 @@
     lin_dir = ensure(settings.Settings.PREF_DIR["Linux"])
     mac_dir = ensure(settings.Settings.PREF_DIR["Darwin"])
     win_dir = ensure(settings.Settings.PREF_DIR["Windows"])
     letters = list(ascii_lowercase)
 
     for name in ("test", "main"):
         for letter, os_dir in (("l", lin_dir), ("w", win_dir), ("m", mac_dir)):
-            __write(
+            write(
                 join(os_dir, "test.json"),
                 **{l: f"{name[0]}{letter}{l}" for l in letters},
                 dp={l: f"{name[0]}{letter}{l}" for l in letters},
             )
 
         letters.pop()
 
     for directory, name, ext in product(
         (dir2, dir1, directory), ("test", "main"), (".json", ".yaml", ".yml")
     ):
-        __write(
+        write(
             join(directory, name + ext),
             **{l: f"{directory[-1]}{ext[2]}{name[0]}{letter}{l}" for l in letters},
             dp={l: f"{directory[-1]}{ext[2]}{name[0]}{letter}{l}" for l in letters},
         )
         letters.pop()
 
 
 def test_basic():
     """test the basic functionality"""
     with TemporaryDirectory() as working_dir:
         base_dir = join(working_dir, "base")
 
         for os in ("Linux", "Darwin", "Windows", "Unknown"):
-            __setup_settings(
+            setup_settings(
                 os=os,
                 shared="test",
                 Linux=join(base_dir, "Linux"),
                 Darwin=join(base_dir, "macOS"),
                 Windows=join(base_dir, "Windows"),
             )
             dir1 = join(base_dir, "dir1")
@@ -202,30 +163,30 @@
                 pass
 
 
 def test_cli_env_in_yaml():
     """test setting cli and env lookups in the yaml itself"""
     with TemporaryDirectory() as working_dir:
         base_dir = join(working_dir, "base")
-        __setup_settings(
+        setup_settings(
             os="Linux",
             shared="test",
             Linux=join(base_dir, "Linux"),
             Darwin=join(base_dir, "macOS"),
             Windows=join(base_dir, "Windows"),
         )
-        __write(
+        write(
             join(base_dir, "main.yml"),
             env={"aa": "alpha", "yy": "yota"},
             cli={"bb": "--beta"},
             yy="main yy",
             aa="main aa",
             bb="main bb",
         )
-        __write(
+        write(
             join(base_dir, "test.yml"),
             env={"zz": "zeta"},
             cli={"dd": "--delta"},
             zz="test zz",
             dd="test dd",
         )
         settings.ENVIRON = {
@@ -255,22 +216,22 @@
         assert opts["zz"] == "environ zz", opts["zz"]
 
 
 def test_environ_values():
     """test environment variable substitution"""
     with TemporaryDirectory() as working_dir:
         base_dir = join(working_dir, "base")
-        __setup_settings(
+        setup_settings(
             os="Linux",
             shared="test",
             Linux=join(base_dir, "Linux"),
             Darwin=join(base_dir, "macOS"),
             Windows=join(base_dir, "Windows"),
         )
-        __write(
+        write(
             join(base_dir, "main.yml"),
             output="${home}/reports",
             settings="${appDir}/settings.json",
             value="testing ${noenv} for noenv",
         )
         settings.ENVIRON = {
             "HOME": "sweet home",
@@ -285,55 +246,59 @@
         assert opts["settings"] == "app data dir/settings.json", opts["settings"]
         assert opts["value"] == "testing ${noenv} for noenv", opts["value"]
 
 
 def test_main():
     """test the main entry point"""
     with TemporaryDirectory() as working_dir:
-        __setup_settings(shared="test", Linux=join(working_dir, "Linux"))
+        setup_settings(shared="test", Linux=join(working_dir, "Linux"))
         settings.ARGV = ["ignore", "test"]
-        __write(join(working_dir, "Linux", "test.yml"), test=3)
+        write(join(working_dir, "Linux", "test.yml"), test=3)
         settings.main()
 
 
 def test_secret():
     """test os secret storage"""
     with TemporaryDirectory() as working_dir:
         base_dir = join(working_dir, "base")
         passwords = {"system": {"john": "setec astronomy"}}
-        __setup_settings(
+        setup_settings(
             os="Linux",
             shared="test",
             Linux=join(base_dir, "Linux"),
             Darwin=join(base_dir, "macOS"),
             Windows=join(base_dir, "Windows"),
         )
         settings.GET_PASSWORD = lambda s, e: passwords.get(s, {}).get(e, None)
-        __write(join(base_dir, "main.yml"), password="main")
+        write(join(base_dir, "main.yml"), password="main")
         opts = settings.Settings(join(base_dir, "main.py")).key(
             "password", "system/john"
         )
         assert opts["password"] == "setec astronomy", opts["password"]
 
 
 def test_main_set_secret():
     """test the main entry point when settings keychain secrets"""
 
     def set_password(s, n, p):
-        assert s == "azure" and n == "token" and p == "setec astronomy", f"{s} {n} {p}"
+        assert (
+            s in ("azure", "jira") and n == "token" and p == "setec astronomy"
+        ), f"{s} {n} {p}"
 
     with TemporaryDirectory() as working_dir:
-        __setup_settings(shared="test", Linux=join(working_dir, "Linux"))
-        settings.ARGV = ["ignore", "--set_secrets"]
-        settings.GET_PASSWORD = lambda s, n: None
+        setup_settings(shared="test", Linux=join(working_dir, "Linux"))
+        settings.ARGV = ["ignore", "--secrets"]
+        settings.GET_PASSWORD = lambda s, n: (
+            "password" if f"{s}/{n}" == "azure/token" else None
+        )
         settings.GET_PASS = lambda p: "setec astronomy"
         settings.SET_PASSWORD = set_password
-        __write(
+        write(
             join(working_dir, "Linux", "test.yml"),
-            secrets={"azure.token": "azure/token"},
+            secrets={"azure.token": "azure/token", "jira.token": "jira/token"},
         )
         settings.main()
 
 
 if __name__ == "__main__":
     test_main_set_secret()
     test_secret()
```

