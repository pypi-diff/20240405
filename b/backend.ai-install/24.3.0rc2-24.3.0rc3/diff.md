# Comparing `tmp/backend.ai-install-24.3.0rc2.tar.gz` & `tmp/backend.ai-install-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-install-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:11 2024, max compression
+gzip compressed data, was "backend.ai-install-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:37 2024, max compression
```

## Comparing `backend.ai-install-24.3.0rc2.tar` & `backend.ai-install-24.3.0rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.527451 backend.ai-install-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-31 14:09:11.523451 backend.ai-install-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.519451 backend.ai-install-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.519451 backend.ai-install-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.523451 backend.ai-install-24.3.0rc2/ai/backend/install/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/app.tcss
--rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.523451 backend.ai-install-24.3.0rc2/ai/backend/install/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/agent.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/manager.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/storage-proxy.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configs/webserver.conf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    46366 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.523451 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-keypairs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-resource-presets.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-session-templates.json
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-set-user-main-access-keys.json
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-users.json
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/http.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/tomltool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/ai/backend/install/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.523451 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:11.527451 backend.ai-install-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-31 14:09:11.000000 backend.ai-install-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.554045 backend.ai-install-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-05 02:25:37.554045 backend.ai-install-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.546044 backend.ai-install-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.546044 backend.ai-install-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.550044 backend.ai-install-24.3.0rc3/ai/backend/install/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/app.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.550044 backend.ai-install-24.3.0rc3/ai/backend/install/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/agent.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/manager.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/storage-proxy.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configs/webserver.conf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46366 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.554045 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-keypairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-resource-presets.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-session-templates.json
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-set-user-main-access-keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-users.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/tomltool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/ai/backend/install/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.554045 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:37.554045 backend.ai-install-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 02:25:37.000000 backend.ai-install-24.3.0rc3/setup.py
```

### Comparing `backend.ai-install-24.3.0rc2/PKG-INFO` & `backend.ai-install-24.3.0rc3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-install
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Installer
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: asyncpg>=0.27.0
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: pydantic~=2.4.2
+Requires-Dist: python-dateutil>=2.8
+Requires-Dist: rich~=13.6
+Requires-Dist: textual~=0.52.1
+Requires-Dist: tomlkit~=0.11.1
+Requires-Dist: types-aiofiles
+Requires-Dist: types-python-dateutil
 
 Backend.AI Installer
 ====================
 
 Package Structure
 -----------------
 
@@ -38,15 +52,15 @@
 ```shell
 ./py -m pip install textual-dev
 ```
 
 Open two terminal sessions.
 In the first one, run:
 ```shell
-dist/export/python/virtualenvs/python-default/3.11.6/bin/textual console
+dist/export/python/virtualenvs/python-default/3.12.2/bin/textual console
 ```
 
 > **Warning**
 > You should use the `textual` executable created *inside the venv's `bin` directory*.
 > `./py -m textual` only shows the demo instead of executing the devtool command.
 
 In the second one, run:
```

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/app.tcss` & `backend.ai-install-24.3.0rc3/ai/backend/install/app.tcss`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/cli.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/common.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/common.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/agent.toml` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/agent.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/alembic.ini` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/docker-compose.yml` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/manager.toml` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/manager.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/storage-proxy.toml` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/storage-proxy.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/configs/webserver.conf` & `backend.ai-install-24.3.0rc3/ai/backend/install/configs/webserver.conf`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/context.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/dev.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/dev.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/docker.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-keypairs.json` & `backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-keypairs.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-resource-presets.json` & `backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-resource-presets.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-session-templates.json` & `backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-session-templates.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-set-user-main-access-keys.json` & `backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-set-user-main-access-keys.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/fixtures/example-users.json` & `backend.ai-install-24.3.0rc3/ai/backend/install/fixtures/example-users.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/http.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/http.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/tomltool.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/tomltool.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/types.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/ai/backend/install/widgets.py` & `backend.ai-install-24.3.0rc3/ai/backend/install/widgets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/PKG-INFO` & `backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-install
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Installer
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
+Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiotools~=1.7.0
+Requires-Dist: asyncpg>=0.27.0
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: pydantic~=2.4.2
+Requires-Dist: python-dateutil>=2.8
+Requires-Dist: rich~=13.6
+Requires-Dist: textual~=0.52.1
+Requires-Dist: tomlkit~=0.11.1
+Requires-Dist: types-aiofiles
+Requires-Dist: types-python-dateutil
 
 Backend.AI Installer
 ====================
 
 Package Structure
 -----------------
 
@@ -38,15 +52,15 @@
 ```shell
 ./py -m pip install textual-dev
 ```
 
 Open two terminal sessions.
 In the first one, run:
 ```shell
-dist/export/python/virtualenvs/python-default/3.11.6/bin/textual console
+dist/export/python/virtualenvs/python-default/3.12.2/bin/textual console
 ```
 
 > **Warning**
 > You should use the `textual` executable created *inside the venv's `bin` directory*.
 > `./py -m textual` only shows the demo instead of executing the devtool command.
 
 In the second one, run:
```

### Comparing `backend.ai-install-24.3.0rc2/backend.ai_install.egg-info/SOURCES.txt` & `backend.ai-install-24.3.0rc3/backend.ai_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/backend_shim.py` & `backend.ai-install-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.0rc2/setup.py` & `backend.ai-install-24.3.0rc3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,31 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Installer',
     'entry_points': {
         'backendai_cli_v10': [
             'install = ai.backend.install.cli:main',
         ],
     },
     'install_requires': (
         'aiofiles~=0.8.0',
         'aiohttp~=3.9.1',
         'aiotools~=1.7.0',
         'asyncpg>=0.27.0',
-        """backend.ai-common==24.03.0rc2
+        """backend.ai-common==24.03.0rc3
 """,
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
         'click~=8.1.7',
         'pydantic~=2.4.2',
         'python-dateutil>=2.8',
         'rich~=13.6',
         'textual~=0.52.1',
         'tomlkit~=0.11.1',
@@ -61,15 +61,15 @@
 ```shell
 ./py -m pip install textual-dev
 ```
 
 Open two terminal sessions.
 In the first one, run:
 ```shell
-dist/export/python/virtualenvs/python-default/3.11.6/bin/textual console
+dist/export/python/virtualenvs/python-default/3.12.2/bin/textual console
 ```
 
 > **Warning**
 > You should use the `textual` executable created *inside the venv's `bin` directory*.
 > `./py -m textual` only shows the demo instead of executing the devtool command.
 
 In the second one, run:
@@ -108,13 +108,13 @@
         'ai.backend.install.configs',
         'ai.backend.install.fixtures',
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
-    'python_requires': '>=3.11,<3.12',
+    'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc2
+    'version': """24.03.0rc3
 """,
     'zip_safe': False,
 })
```

