# Comparing `tmp/inmanta-dev-dependencies-2.98.0.tar.gz` & `tmp/inmanta-dev-dependencies-2.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-dev-dependencies-2.98.0.tar", last modified: Fri Dec 22 12:59:03 2023, max compression
+gzip compressed data, was "inmanta-dev-dependencies-2.99.0.tar", last modified: Fri Dec 22 17:59:34 2023, max compression
```

## Comparing `inmanta-dev-dependencies-2.98.0.tar` & `inmanta-dev-dependencies-2.99.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-22 12:59:03.086157 inmanta-dev-dependencies-2.98.0/
--rw-r--r--   0 jenkins    (988) jenkins    (986)     1834 2023-12-22 12:59:03.086157 inmanta-dev-dependencies-2.98.0/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      647 2023-12-22 12:58:45.000000 inmanta-dev-dependencies-2.98.0/README.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1744 2023-12-22 12:58:55.000000 inmanta-dev-dependencies-2.98.0/pyproject.toml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       38 2023-12-22 12:59:03.086157 inmanta-dev-dependencies-2.98.0/setup.cfg
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-22 12:59:03.083157 inmanta-dev-dependencies-2.98.0/src/
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-22 12:59:03.083157 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       23 2023-12-22 12:58:55.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies/__init__.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-22 12:59:03.084157 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/
--rw-r--r--   0 jenkins    (988) jenkins    (986)     1834 2023-12-22 12:59:03.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      324 2023-12-22 12:59:03.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2023-12-22 12:59:03.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      659 2023-12-22 12:59:03.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       25 2023-12-22 12:59:03.000000 inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2023-12-22 17:59:34.248935 inmanta-dev-dependencies-2.99.0/
+-rw-r--r--   0 jenkins    (987) jenkins    (985)     1834 2023-12-22 17:59:34.248935 inmanta-dev-dependencies-2.99.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      647 2023-12-22 17:59:15.000000 inmanta-dev-dependencies-2.99.0/README.md
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     1744 2023-12-22 17:59:26.000000 inmanta-dev-dependencies-2.99.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       38 2023-12-22 17:59:34.248935 inmanta-dev-dependencies-2.99.0/setup.cfg
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2023-12-22 17:59:34.245935 inmanta-dev-dependencies-2.99.0/src/
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2023-12-22 17:59:34.245935 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies/
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       23 2023-12-22 17:59:26.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies/__init__.py
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2023-12-22 17:59:34.246935 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/
+-rw-r--r--   0 jenkins    (987) jenkins    (985)     1834 2023-12-22 17:59:34.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      324 2023-12-22 17:59:34.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)        1 2023-12-22 17:59:34.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      659 2023-12-22 17:59:34.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       25 2023-12-22 17:59:34.000000 inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/top_level.txt
```

### Comparing `inmanta-dev-dependencies-2.98.0/PKG-INFO` & `inmanta-dev-dependencies-2.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-dev-dependencies
-Version: 2.98.0
+Version: 2.99.0
 Summary: Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions.
 Author-email: Inmanta <code@inmanta.com>
 Requires-Python: >=3.9
 Requires-Dist: black==23.12.0
 Requires-Dist: flake8==6.1.0
 Requires-Dist: flake8-copyright==0.2.4
 Requires-Dist: flake8-black==0.3.6
@@ -27,15 +27,15 @@
 Requires-Dist: inmanta-core[pytest-inmanta-extensions]; extra == "extension"
 Requires-Dist: asyncpg<1.0.0,>=0.21.0; extra == "extension"
 Requires-Dist: pytest-env==1.1.3; extra == "extension"
 Requires-Dist: pytest-postgresql==5.0.0; extra == "extension"
 Requires-Dist: psycopg==3.1.16; extra == "extension"
 Requires-Dist: tornado<7.0,>=6.1; extra == "extension"
 Provides-Extra: async
-Requires-Dist: pytest-asyncio==0.21.1; extra == "async"
+Requires-Dist: pytest-asyncio==0.23.1; extra == "async"
 Requires-Dist: pytest-timeout==2.2.0; extra == "async"
 Provides-Extra: pytest
 Requires-Dist: pytest-env==1.1.3; extra == "pytest"
 Requires-Dist: pytest-cover==3.0.0; extra == "pytest"
 Requires-Dist: pytest-randomly==3.15.0; extra == "pytest"
 Requires-Dist: pytest-xdist==3.5.0; extra == "pytest"
 Requires-Dist: pytest-sugar==0.9.7; extra == "pytest"
```

### Comparing `inmanta-dev-dependencies-2.98.0/README.md` & `inmanta-dev-dependencies-2.99.0/README.md`

 * *Files identical despite different names*

### Comparing `inmanta-dev-dependencies-2.98.0/pyproject.toml` & `inmanta-dev-dependencies-2.99.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inmanta-dev-dependencies"
-version = "2.98.0"
+version = "2.99.0"
 requires-python = ">=3.9"
 description = "Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions."
 authors = [
     {name = "Inmanta", email = "code@inmanta.com"},
 ]
 
 dependencies = [
@@ -46,15 +46,15 @@
     "asyncpg>=0.21.0,<1.0.0",
     "pytest-env==1.1.3",
     "pytest-postgresql==5.0.0",
     "psycopg==3.1.16",
     "tornado>=6.1,<7.0"
 ]
 async = [
-    "pytest-asyncio==0.21.1",
+    "pytest-asyncio==0.23.1",
     "pytest-timeout==2.2.0"
 ]
 pytest = [
     "pytest-env==1.1.3",
     "pytest-cover==3.0.0",
     "pytest-randomly==3.15.0",
     "pytest-xdist==3.5.0",
```

### Comparing `inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/PKG-INFO` & `inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-dev-dependencies
-Version: 2.98.0
+Version: 2.99.0
 Summary: Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions.
 Author-email: Inmanta <code@inmanta.com>
 Requires-Python: >=3.9
 Requires-Dist: black==23.12.0
 Requires-Dist: flake8==6.1.0
 Requires-Dist: flake8-copyright==0.2.4
 Requires-Dist: flake8-black==0.3.6
@@ -27,15 +27,15 @@
 Requires-Dist: inmanta-core[pytest-inmanta-extensions]; extra == "extension"
 Requires-Dist: asyncpg<1.0.0,>=0.21.0; extra == "extension"
 Requires-Dist: pytest-env==1.1.3; extra == "extension"
 Requires-Dist: pytest-postgresql==5.0.0; extra == "extension"
 Requires-Dist: psycopg==3.1.16; extra == "extension"
 Requires-Dist: tornado<7.0,>=6.1; extra == "extension"
 Provides-Extra: async
-Requires-Dist: pytest-asyncio==0.21.1; extra == "async"
+Requires-Dist: pytest-asyncio==0.23.1; extra == "async"
 Requires-Dist: pytest-timeout==2.2.0; extra == "async"
 Provides-Extra: pytest
 Requires-Dist: pytest-env==1.1.3; extra == "pytest"
 Requires-Dist: pytest-cover==3.0.0; extra == "pytest"
 Requires-Dist: pytest-randomly==3.15.0; extra == "pytest"
 Requires-Dist: pytest-xdist==3.5.0; extra == "pytest"
 Requires-Dist: pytest-sugar==0.9.7; extra == "pytest"
```

### Comparing `inmanta-dev-dependencies-2.98.0/src/inmanta_dev_dependencies.egg-info/requires.txt` & `inmanta-dev-dependencies-2.99.0/src/inmanta_dev_dependencies.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 lxml==4.9.4
 mypy==1.8.0
 pep8-naming==0.13.3
 pytest==7.4.3
 pyupgrade==3.15.0
 
 [async]
-pytest-asyncio==0.21.1
+pytest-asyncio==0.23.1
 pytest-timeout==2.2.0
 
 [core]
 asyncpg<1.0.0,>=0.21.0
 pytest-env==1.1.3
 pytest-postgresql==5.0.0
 psycopg==3.1.16
```

