# Comparing `tmp/fast-templates-0.1.8.tar.gz` & `tmp/fast-templates-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-templates-0.1.8.tar", last modified: Mon Apr  1 21:49:44 2024, max compression
+gzip compressed data, was "fast-templates-0.1.9.tar", last modified: Thu Apr  4 22:57:16 2024, max compression
```

## Comparing `fast-templates-0.1.8.tar` & `fast-templates-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-01 21:49:40.000000 fast-templates-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 21:49:44.318834 fast-templates-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 21:49:40.000000 fast-templates-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fast_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:49:44.000000 fast-templates-0.1.8/fast_templates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/baselayout/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/db/mongo/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/db/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/db/mongo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/routes/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/app/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/baselayout/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/extras/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/extras/cache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.314834 fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/app/utils/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/extras/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/extras/db/mongo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/db/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/db/mongo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.318834 fast-templates-0.1.8/fasttemplates/templates/extras/db/redis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/db/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/templates/extras/db/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 21:49:40.000000 fast-templates-0.1.8/fasttemplates/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:49:44.318834 fast-templates-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-01 21:49:40.000000 fast-templates-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.454931 fast-templates-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-04 22:57:12.000000 fast-templates-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 22:57:16.454931 fast-templates-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-04 22:57:12.000000 fast-templates-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fast_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:57:16.454931 fast-templates-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 22:57:12.000000 fast-templates-0.1.9/setup.py
```

### Comparing `fast-templates-0.1.8/LICENSE` & `fast-templates-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.8/PKG-INFO` & `fast-templates-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
+Requires-Dist: pyyaml
 
 =======================
 fast-templates
 =======================
 
 CLI that contains fastapi templates for different projects
```

### Comparing `fast-templates-0.1.8/fast_templates.egg-info/PKG-INFO` & `fast-templates-0.1.9/fast_templates.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
+Requires-Dist: pyyaml
 
 =======================
 fast-templates
 =======================
 
 CLI that contains fastapi templates for different projects
```

### Comparing `fast-templates-0.1.8/fast_templates.egg-info/SOURCES.txt` & `fast-templates-0.1.9/fast_templates.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 fasttemplates/utils.py
 fasttemplates/templates/baselayout/Dockerfile
 fasttemplates/templates/baselayout/docker-compose.yml
 fasttemplates/templates/baselayout/requirements.txt
 fasttemplates/templates/baselayout/app/constants.py
 fasttemplates/templates/baselayout/app/main.py
 fasttemplates/templates/baselayout/app/settings.py
-fasttemplates/templates/baselayout/app/db/__init__.py
-fasttemplates/templates/baselayout/app/db/mongo/__init__.py
-fasttemplates/templates/baselayout/app/db/mongo/client.py
 fasttemplates/templates/baselayout/app/routes/__init__.py
 fasttemplates/templates/baselayout/app/routes/example.py
 fasttemplates/templates/baselayout/app/utils/__init__.py
 fasttemplates/templates/baselayout/app/utils/cache.py
 fasttemplates/templates/baselayout/app/utils/logger.py
 fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
 fasttemplates/templates/extras/cache/redis/app/utils/cache.py
```

### Comparing `fast-templates-0.1.8/fasttemplates/main.py` & `fast-templates-0.1.9/fasttemplates/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 
 import typer
 import questionary
+import tempfile
+import shutil
+import stat
+import yaml
 
 from fasttemplates.constants import *
 from fasttemplates.utils import *
 
 app = typer.Typer()
 
 
@@ -22,33 +26,33 @@
     if redis_present:
         add_redis()
         print("Redis database added")
         cache = questionary.confirm("Do you want to use Redis as cache?").ask()
         if cache:
             add_cache_with_redis()
             print("Redis cache added")
+    
+    create_docker_compose()
 
 
 def popular() -> None:
     "Clones the popular template from the github repository"
 
     optionLambdas = {
-        FASTAPI_FS: lambda: os.system(f'git clone {FASTAPI_FULLSTACK} {WORKING_DIR}'),
-        FASTAPI_DJANGO_ORM: lambda: os.system(
-            f'git clone {FASTAPI_WITH_DJANGO_ORM} {WORKING_DIR}')
+        FASTAPI_FS: lambda: clone_and_copy(FASTAPI_FULLSTACK),
+        FASTAPI_DJANGO_ORM: lambda: clone_and_copy(FASTAPI_WITH_DJANGO_ORM),
     }
 
     option = questionary.select("Which popular template do you want to clone?", choices=[
         FASTAPI_FS, FASTAPI_DJANGO_ORM]).ask()
 
     optionLambdas[option]()
 
     print("Popular template added")
 
-
 @app.command()
 def main() -> None:
     popular_or_simplified_functions = {
         'Popular': popular,
         'Custom': custom
     }
     popular_or_simplified = questionary.select("Popular templates or custom templates?", choices=[
@@ -66,26 +70,34 @@
     os.makedirs(MONGO_DIR, exist_ok=True)
     copy_files(DB_TREE, MONGO_DIR, ignore_dirs=[REDIS_DIR_NAME])
 
     # Add dnspython & pymongo to requirements.txt
     with open(os.path.join(WORKING_DIR, "requirements.txt"), "a") as f:
         f.write("\ndnspython\npymongo\n")
 
-    # Modify docker-compose.yml
-    with open(os.path.join(WORKING_DIR, "docker-compose.yml"), "a") as f:
-        f.write(DOCKER_COMPOSE_YML)
+    docker_compose_dict['services'].update(mongo_service)
+    docker_compose_dict['volumes'].update(mongo_volume)
 
     add_mongo_uri_to_settings()
 
 
+def create_docker_compose() -> None:
+    with open(os.path.join(WORKING_DIR, "docker-compose.yml"), "w") as f:
+        yaml.dump(docker_compose_dict, f, default_flow_style=False, sort_keys=False)
+
 def add_redis() -> None:
     REDIS_DIR = os.path.join(WORKING_DIR, DB_DIR)
     os.makedirs(REDIS_DIR, exist_ok=True)
     copy_files(DB_TREE, REDIS_DIR, ignore_dirs=[MONGO_DIR_NAME])
 
+    docker_compose_dict['services'].update(redis_service)
+    docker_compose_dict['volumes'].update(redis_volume)
+
+    add_redis_uri_to_settings()
+
 
 def add_cache_with_redis() -> None:
     os.makedirs(WORKING_DIR, exist_ok=True)
     copy_files(REDIS_CACHE_TREE, WORKING_DIR)
 
 
 if __name__ == "__main__":
```

### Comparing `fast-templates-0.1.8/fasttemplates/templates/extras/cache/redis/app/utils/cache.py` & `fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/cache.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.8/fasttemplates/utils.py` & `fast-templates-0.1.9/fasttemplates/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,24 +17,44 @@
 
         if os.path.isdir(src_item):
             os.makedirs(dst_item, exist_ok=True)
             copy_files(src_item, dst_item, ignore_dirs)
         else:
             shutil.copy2(src_item, dst_item)
 
-
-def add_mongo_uri_to_settings():
-    # Add MONGO_URI to Settings class
+def cout_settings_properties() -> int:
     settings_path = os.path.join(WORKING_DIR, "app\\settings.py")
     with open(settings_path, "r") as f:
         lines = f.readlines()
-
-    # Find the line with the class definition
+    
     class_def_index = next(i for i, line in enumerate(
-        lines) if 'class Settings(BaseSettings):' in line)
+        lines) if SETTINGS_CLASS_DEFINITION in line)
+    
+    return len([line for line in lines if line.strip() and not line.strip().startswith('#')])+1
 
-    # Insert the new line after the class definition
-    lines.insert(class_def_index + 3, '    MONGO_URI:  str = None\n')
+def add_property_to_settings(_K: str, _T: type, _V: str) -> None:
+    settings_path = os.path.join(WORKING_DIR, SETTINGS_DIR)
+    with open(settings_path, "r") as f:
+        lines = f.readlines()
+    
+    NUMBER_OF_PROPERTIES = cout_settings_properties()
+    lines.insert(NUMBER_OF_PROPERTIES, f'    {_K}: {_T.__name__} = {_V}\n')
 
-    # Write the modified lines back to the file
     with open(settings_path, "w") as f:
         f.writelines(lines)
+
+def add_mongo_uri_to_settings():
+    add_property_to_settings('MONGO_URI', str, "'mongodb://localhost:27017'")
+
+def add_redis_uri_to_settings():
+    add_property_to_settings('REDIS_URI', str, "'redis://localhost:6379/0'")
+
+def on_rm_error(func, path, exc_info) -> None:
+    "Error handler for `shutil.rmtree`"
+    os.chmod(path, stat.S_IWRITE)
+    os.unlink(path)
+
+def clone_and_copy(repo_url: str) -> None:
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        os.system(f'git clone {repo_url} {tmpdirname}')
+        shutil.rmtree(os.path.join(tmpdirname, '.git'), onerror=on_rm_error)
+        copy_files(tmpdirname, WORKING_DIR)
```

### Comparing `fast-templates-0.1.8/setup.py` & `fast-templates-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='fast-templates',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     package_data={'': ['**/*', '.env', '.gitignore']},
     url='https://github.com/pybalt/FastAPI-TemplateWizard',
     author='pybalt',
     author_email='96897286+pybalt@users.noreply.github.com',
     description='A CLI to generate FastAPI templates',
     long_description=long_description,
     install_requires=[
         'typer',
-        'questionary'
+        'questionary',
+        'pyyaml'
     ],
     entry_points='''
         [console_scripts]
         fastcli=fasttemplates.main:app
     '''
 )
```

