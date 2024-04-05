# Comparing `tmp/mailck-0.2.0.tar.gz` & `tmp/mailck-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailck-0.2.0.tar", max compression
+gzip compressed data, was "mailck-0.3.0.tar", max compression
```

## Comparing `mailck-0.2.0.tar` & `mailck-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.2.0/LICENSE
--rw-r--r--   0        0        0     4284 2024-01-06 17:04:03.311076 mailck-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-12-20 14:09:26.334235 mailck-0.2.0/mailck/__init__.py
--rw-r--r--   0        0        0     7539 2024-01-06 17:03:22.089800 mailck-0.2.0/mailck/main.py
--rw-r--r--   0        0        0      644 2024-01-06 16:57:31.405607 mailck-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 mailck-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4222 2024-04-05 09:47:28.352692 mailck-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-12-20 14:09:26.334235 mailck-0.3.0/mailck/__init__.py
+-rw-r--r--   0        0        0     7301 2024-04-05 09:48:12.227381 mailck-0.3.0/mailck/main.py
+-rw-r--r--   0        0        0      644 2024-04-05 09:41:21.844730 mailck-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 mailck-0.3.0/PKG-INFO
```

### Comparing `mailck-0.2.0/LICENSE` & `mailck-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailck-0.2.0/README.md` & `mailck-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 - light: small size and resource usage
 - low dependencies: low or no external dependencies
 - terminal-focused: terminal usage focused (input and output) - primarily focused on usage through conky
 
 
 ## Latest Changes
 
-- replaced black, flake8, isort with ruff
-- add modified [date] to --version & standardize version metadata
+- changed --version to use importlib.metadata
 
 
 ### Notices
 
 - it does not make much sense to run this more frequently than every 10s as connecting takes ~1-2s
```

### Comparing `mailck-0.2.0/mailck/main.py` & `mailck-0.3.0/mailck/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import json
 import logging
 import sys
 from datetime import datetime
 from enum import Enum
 from optparse import OptionParser
 from os import getenv
-import tomllib
 
 
 logger_base = logging.getLogger("default")
 logger_base.setLevel(logging.getLevelName(getenv("LOG_LEVEL", "INFO")))
 logger_base.addHandler(logging.StreamHandler(sys.stdout))
 logger = logging.LoggerAdapter(logging.getLogger("default"))
 
@@ -88,25 +87,23 @@
 
         return json.dumps(self.__dict__, indent=4)
 
 
 def show_version():
     """
     Show version.
-    NOTICE: we load the pyproject.toml here (rather than a config) so its not loaded on normal app usage as it is not needed then.
     """
 
-    with open("pyproject.toml", "rb") as f:
-        _meta = tomllib.load(f)
+    import importlib.metadata
 
-    _name = _meta["tool"]["poetry"]["name"]
-    _version = _meta["tool"]["poetry"]["version"]
-    _modified = _meta["internal"]["modified"]
+    _meta = importlib.metadata.metadata("mailck")
+    _name = _meta["Name"]
+    _version = _meta["Version"]
 
-    logger.critical(f"{_name} {_version} ({_modified})")
+    logger.critical(f"{_name} {_version}")
 
 
 def check_mail(r: MCRequest = None):
     """
     Check mail.
     """
```

### Comparing `mailck-0.2.0/pyproject.toml` & `mailck-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [internal]
 created = 2023-12-20
 modified = 2024-01-06
 
 [tool.poetry]
 name = "mailck"
-version = "0.2.0"
+version = "0.3.0"
 description = "a simple mail check utility, currently supporting IMAP"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/mailck"
 repository = "https://gitlab.com/drad/mailck"
```

### Comparing `mailck-0.2.0/PKG-INFO` & `mailck-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailck
-Version: 0.2.0
+Version: 0.3.0
 Summary: a simple mail check utility, currently supporting IMAP
 Home-page: https://gitlab.com/drad/mailck
 License: GPL-3.0-only
 Keywords: mail,imap,check,conky,cron,terminal,email
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
@@ -24,16 +24,15 @@
 - light: small size and resource usage
 - low dependencies: low or no external dependencies
 - terminal-focused: terminal usage focused (input and output) - primarily focused on usage through conky
 
 
 ## Latest Changes
 
-- replaced black, flake8, isort with ruff
-- add modified [date] to --version & standardize version metadata
+- changed --version to use importlib.metadata
 
 
 ### Notices
 
 - it does not make much sense to run this more frequently than every 10s as connecting takes ~1-2s
```

