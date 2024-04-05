# Comparing `tmp/marioutils-1.1.1.tar.gz` & `tmp/marioutils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marioutils-1.1.1.tar", last modified: Tue Apr  2 21:50:12 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `marioutils-1.1.1.tar` & `marioutils-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.827178 marioutils-1.1.1/
--rw-rw-rw-   0        0        0     1088 2024-03-29 19:37:30.000000 marioutils-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      925 2024-04-02 21:50:12.826182 marioutils-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.398955 marioutils-1.1.1/mario_utils/
--rw-rw-rw-   0        0        0      269 2024-03-29 19:37:30.000000 marioutils-1.1.1/mario_utils/README.md
--rw-rw-rw-   0        0        0      166 2024-04-02 00:21:18.000000 marioutils-1.1.1/mario_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.434023 marioutils-1.1.1/mario_utils/databasemanagement/
--rw-rw-rw-   0        0        0       93 2024-04-02 00:18:26.000000 marioutils-1.1.1/mario_utils/databasemanagement/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.503021 marioutils-1.1.1/mario_utils/databasemanagement/src/
--rw-rw-rw-   0        0        0       99 2024-04-01 21:45:12.000000 marioutils-1.1.1/mario_utils/databasemanagement/src/__init__.py
--rw-rw-rw-   0        0        0     1613 2024-04-02 21:41:01.000000 marioutils-1.1.1/mario_utils/databasemanagement/src/exceptions.py
--rw-rw-rw-   0        0        0     6220 2024-04-02 21:43:37.000000 marioutils-1.1.1/mario_utils/databasemanagement/src/manager.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.506020 marioutils-1.1.1/mario_utils/databasemanagement/tests/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.1.1/mario_utils/databasemanagement/tests/__init__.py
--rw-rw-rw-   0        0        0     2479 2024-04-02 21:45:02.000000 marioutils-1.1.1/mario_utils/databasemanagement/tests/test_.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.507021 marioutils-1.1.1/mario_utils/logger/
--rw-rw-rw-   0        0        0       67 2024-04-01 21:49:53.000000 marioutils-1.1.1/mario_utils/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.592020 marioutils-1.1.1/mario_utils/logger/src/
--rw-rw-rw-   0        0        0       70 2024-04-01 21:48:54.000000 marioutils-1.1.1/mario_utils/logger/src/__init__.py
--rw-rw-rw-   0        0        0      982 2024-04-02 00:23:57.000000 marioutils-1.1.1/mario_utils/logger/src/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.596020 marioutils-1.1.1/mario_utils/logger/test/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.1.1/mario_utils/logger/test/__init__.py
--rw-rw-rw-   0        0        0      572 2024-04-02 00:22:14.000000 marioutils-1.1.1/mario_utils/logger/test/test_logger.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:50:12.793046 marioutils-1.1.1/marioutils.egg-info/
--rw-rw-rw-   0        0        0      925 2024-04-02 21:50:12.000000 marioutils-1.1.1/marioutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2024-04-02 21:50:12.000000 marioutils-1.1.1/marioutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:50:12.000000 marioutils-1.1.1/marioutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-02 21:50:12.000000 marioutils-1.1.1/marioutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 21:50:12.000000 marioutils-1.1.1/marioutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 21:50:12.828182 marioutils-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-04-02 21:49:36.000000 marioutils-1.1.1/setup.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 marioutils-1.1.2/.vscode/DatabaseManagement.code-workspace
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 marioutils-1.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 marioutils-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/src/__init__.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/src/exceptions.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/src/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/tests/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/databasemanagement/tests/test_.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/logger/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/logger/src/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/logger/src/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/logger/test/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 marioutils-1.1.2/mario_utils/logger/test/test_logger.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 marioutils-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 marioutils-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 marioutils-1.1.2/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 marioutils-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 marioutils-1.1.2/PKG-INFO
```

### Comparing `marioutils-1.1.1/LICENSE.txt` & `marioutils-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marioutils-1.1.1/PKG-INFO` & `marioutils-1.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1
-Name: marioutils
-Version: 1.1.1
-Summary: Utils library for DB connection and logging
-Home-page: https://github.com/MarioHdzCtu/MarioUtils
-Author: Mario Hernandez
-Author-email: mariohertu@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.12
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pymssql>=2.2.11
-Requires-Dist: sqlalchemy>=2.0.25
-Requires-Dist: mariadb>=1.1.10
-Provides-Extra: dev
-Requires-Dist: pytest>=8.0.0; extra == "dev"
-
-
-# Mario Utils
-
-This project is used as a Python library for managing database connections (Now just supporting SQLServer over pymssql) and Logging for future scripts, avoiding boilerplate code.
-
-
-## Authors
-
-- [@MarioHdzCtu](https://github.com/MarioHdzCtu)
-
+Metadata-Version: 2.3
+Name: marioutils
+Version: 1.1.2
+Summary: Utils library for DB connection and logging
+Project-URL: Homepage, https://github.com/MarioHdzCtu/MarioUtils
+Project-URL: Issues, https://github.com/MarioHdzCtu/MarioUtils/issues
+Author-email: Mario Hernandez <mariohertu@gmail.com>
+License-File: LICENSE.txt
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Requires-Dist: mariadb>=1.1.10
+Requires-Dist: pymssql>=2.2.11
+Requires-Dist: sqlalchemy>=2.0.25
+Provides-Extra: dev
+Requires-Dist: pytest>=8.0.0; extra == 'dev'
+Description-Content-Type: text/markdown
+
+
+# Mario Utils
+
+This project is used as a Python library for managing database connections (Now just supporting SQLServer over pymssql) and Logging for future scripts, avoiding boilerplate code.
+
+
+## Authors
+
+- [@MarioHdzCtu](https://github.com/MarioHdzCtu)
+
```

### Comparing `marioutils-1.1.1/mario_utils/databasemanagement/src/exceptions.py` & `marioutils-1.1.2/mario_utils/databasemanagement/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.1.1/mario_utils/databasemanagement/src/manager.py` & `marioutils-1.1.2/mario_utils/databasemanagement/src/manager.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.1.1/mario_utils/databasemanagement/tests/test_.py` & `marioutils-1.1.2/mario_utils/databasemanagement/tests/test_.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.1.1/mario_utils/logger/src/logger.py` & `marioutils-1.1.2/mario_utils/logger/src/logger.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.1.1/mario_utils/logger/test/test_logger.py` & `marioutils-1.1.2/mario_utils/logger/test/test_logger.py`

 * *Files identical despite different names*

