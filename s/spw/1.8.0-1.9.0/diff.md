# Comparing `tmp/spw-1.8.0.tar.gz` & `tmp/spw-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spw-1.8.0.tar", max compression
+gzip compressed data, was "spw-1.9.0.tar", max compression
```

## Comparing `spw-1.8.0.tar` & `spw-1.9.0.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0    35059 2020-02-12 10:32:05.496019 spw-1.8.0/LICENSE
--rw-r--r--   0        0        0     2660 2023-11-07 18:43:59.870248 spw-1.8.0/README.md
--rw-r--r--   0        0        0      976 2023-11-07 18:43:51.006626 spw-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-18 16:16:47.774721 spw-1.8.0/spw/__init__.py
--rw-r--r--   0        0        0       44 2022-09-18 16:16:47.774721 spw-1.8.0/spw/__main__.py
--rw-r--r--   0        0        0        0 2022-09-18 16:16:47.778054 spw-1.8.0/spw/config/__init__.py
--rw-r--r--   0        0        0      468 2023-11-07 18:44:18.397516 spw-1.8.0/spw/config/config.py
--rwxr-xr-x   0        0        0    11856 2023-11-07 19:12:22.204153 spw-1.8.0/spw/main.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 spw-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2020-02-12 10:32:05.496019 spw-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2927 2024-01-06 18:30:21.889013 spw-1.9.0/README.md
+-rw-r--r--   0        0        0      722 2024-01-06 18:27:40.907328 spw-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-06 18:30:50.076558 spw-1.9.0/spw/__init__.py
+-rw-r--r--   0        0        0       44 2024-01-06 18:30:50.079892 spw-1.9.0/spw/__main__.py
+-rwxr-xr-x   0        0        0    12367 2024-01-06 18:30:50.076558 spw-1.9.0/spw/main.py
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 spw-1.9.0/PKG-INFO
```

### Comparing `spw-1.8.0/LICENSE` & `spw-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spw-1.8.0/README.md` & `spw-1.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,34 @@
 spw is an application that stores and retrieves passwords in a secure manner. spw is designed to be quick, light on resources/dependencies, and command line/script driven.
 
 Passwords are stored in an encrypted format using PKCS1_OAEP encryption. This means you use a public and private key to encrypt and decrypt items stored within the store. This is a secure method of password storage and there is virtually no chance someone (including yourself) can view decrypted passwords without the private key.
 
 spw is intended to provide a secure mechanism to store (and more importantly retrieve) passwords. spw's command-line interface allows easy integration into openbox's keyboard shortcut functionality (or similar tools). spw provides an easy mechanism for copying a password to the clipboard (e.g. C+A+j will copy the gmail junk account's password to your clipboard).
 
 
+### Latest Changes
+
+- replaced black, flake8, isort with ruff
+- upgraded packages: cryptography
+- add modified [date] to --version & standardize version metadata
+- removed config module as it is not needed/used
+- minimum python version increased to 3.11 for tomllib support
+
+
 ### Requiremnts
 
 - python3
 
 
 ### Install
 
-We recommend using [pipx](https://github.com/pypa/pipx) to install spw: `pipx install spw`. You can also install via pip: `pip install --user spw`.
+We recommend using [pipx](https://github.com/pypa/pipx). To install:
+
+- with pipx: `pipx install spw`
+- with pip: `pip install --user spw`
 
 
 ### Configure
 
 cryptik uses a config file to store your setup. This file contains information where your secure database is stored and the private key to use as well as other configuration items. You can grab the sample config file from  [spw/example/spw.ini.template](https://gitlab.com/drad/spw/-/blob/master/examples/spw.ini.template) and place it at `~/.config/spw/spw.ini`.
 
 Refer to the example `spw.ini.template` file for details on each config item. The default (e.g. `spw.ini.template`) should suffice for most usage; however, you can change where your keys are located, logging level, and more in the file.
```

### Comparing `spw-1.8.0/spw/main.py` & `spw-1.9.0/spw/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
 #  Copyright 2023 drad <sa@adercon.com>
 
 import ast
 import configparser
+import tomllib
 import logging
 import os
 import secrets
 import string
 import subprocess  # nosec
 import sys
 import threading
 from optparse import OptionParser
 
 import lmdb
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 
-from spw.config.config import APP_NAME, APP_VERSION
+_log_level = "INFO"  # [CRITICAL|ERROR|WARNING|INFO|DEBUG] (suggest INFO)
 
 required_config_files = [os.path.expanduser("~/.config/spw/spw.ini")]
 config = configparser.ConfigParser()
 found_configs = config.read(required_config_files)
 missing_configs = set(required_config_files) - set(found_configs)
 if missing_configs:
     print(f"ERROR: Missing Config File: {missing_configs}, cannot continue")
     sys.exit(1)
 
+logging.basicConfig(
+    format="%(message)s",
+    level=logging.getLevelName(_log_level),
+    stream=sys.stdout,
+)
+
 logger_base = logging.getLogger(__name__)
 write_to_console = False
 
 
 def show_version():
     """
     Show application version.
+    NOTICE: we load the pyproject.toml here (rather than a config) so its not loaded on normal app usage as it is not needed then.
     """
 
-    logging.critical(f"{APP_NAME} {APP_VERSION}")
+    with open("pyproject.toml", "rb") as f:
+        _meta = tomllib.load(f)
+
+    _name = _meta["tool"]["poetry"]["name"]
+    _version = _meta["tool"]["poetry"]["version"]
+    _modified = _meta["internal"]["modified"]
+
+    logging.critical(f"{_name} {_version} ({_modified})")
 
 
 def expand_path(path):
     """
     Expand the path to account for user home and environment variables
     """
```

### Comparing `spw-1.8.0/PKG-INFO` & `spw-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 Metadata-Version: 2.1
 Name: spw
-Version: 1.8.0
+Version: 1.9.0
 Summary: store and retrieve passwords securely all while being scriptable!
 Home-page: https://gitlab.com/drad/spw
 License: GPL-3.0-only
 Keywords: cli,encryption,password,openbox,scriptable
 Author: David Rader
 Author-email: sa@adercon.com
 Maintainer: David Rader
 Maintainer-email: sa@adercon.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cryptography (>=41.0.5,<42.0.0)
-Requires-Dist: lmdb (>=1.4.1,<2.0.0)
+Requires-Dist: cryptography (>=41.0,<42.0)
+Requires-Dist: lmdb (>=1.4,<2.0)
 Project-URL: Repository, https://gitlab.com/drad/spw
 Description-Content-Type: text/markdown
 
 ### About
 
 spw is an application that stores and retrieves passwords in a secure manner. spw is designed to be quick, light on resources/dependencies, and command line/script driven.
 
 Passwords are stored in an encrypted format using PKCS1_OAEP encryption. This means you use a public and private key to encrypt and decrypt items stored within the store. This is a secure method of password storage and there is virtually no chance someone (including yourself) can view decrypted passwords without the private key.
 
 spw is intended to provide a secure mechanism to store (and more importantly retrieve) passwords. spw's command-line interface allows easy integration into openbox's keyboard shortcut functionality (or similar tools). spw provides an easy mechanism for copying a password to the clipboard (e.g. C+A+j will copy the gmail junk account's password to your clipboard).
 
 
+### Latest Changes
+
+- replaced black, flake8, isort with ruff
+- upgraded packages: cryptography
+- add modified [date] to --version & standardize version metadata
+- removed config module as it is not needed/used
+- minimum python version increased to 3.11 for tomllib support
+
+
 ### Requiremnts
 
 - python3
 
 
 ### Install
 
-We recommend using [pipx](https://github.com/pypa/pipx) to install spw: `pipx install spw`. You can also install via pip: `pip install --user spw`.
+We recommend using [pipx](https://github.com/pypa/pipx). To install:
+
+- with pipx: `pipx install spw`
+- with pip: `pip install --user spw`
 
 
 ### Configure
 
 cryptik uses a config file to store your setup. This file contains information where your secure database is stored and the private key to use as well as other configuration items. You can grab the sample config file from  [spw/example/spw.ini.template](https://gitlab.com/drad/spw/-/blob/master/examples/spw.ini.template) and place it at `~/.config/spw/spw.ini`.
 
 Refer to the example `spw.ini.template` file for details on each config item. The default (e.g. `spw.ini.template`) should suffice for most usage; however, you can change where your keys are located, logging level, and more in the file.
```

