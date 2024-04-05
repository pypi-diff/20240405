# Comparing `tmp/fast-templates-0.1.9.tar.gz` & `tmp/fast-templates-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-templates-0.1.9.tar", last modified: Thu Apr  4 22:57:16 2024, max compression
+gzip compressed data, was "fast-templates-0.2.0.tar", last modified: Thu Apr  4 23:07:28 2024, max compression
```

## Comparing `fast-templates-0.1.9.tar` & `fast-templates-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.454931 fast-templates-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-04 22:57:12.000000 fast-templates-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 22:57:16.454931 fast-templates-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-04 22:57:12.000000 fast-templates-0.1.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fast_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 22:57:16.000000 fast-templates-0.1.9/fast_templates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/routes/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/app/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/baselayout/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.446931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/mongo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:16.450931 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/templates/extras/db/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-04 22:57:12.000000 fast-templates-0.1.9/fasttemplates/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:57:16.454931 fast-templates-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 22:57:12.000000 fast-templates-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.868827 fast-templates-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-04 23:07:24.000000 fast-templates-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 23:07:28.868827 fast-templates-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 23:07:24.000000 fast-templates-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.868827 fast-templates-0.2.0/fast_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 23:07:28.000000 fast-templates-0.2.0/fast_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.860827 fast-templates-0.2.0/fasttemplates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/baselayout/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/routes/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/app/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/baselayout/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.860827 fast-templates-0.2.0/fasttemplates/templates/extras/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.860827 fast-templates-0.2.0/fasttemplates/templates/extras/cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.860827 fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.860827 fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/app/utils/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/extras/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.864827 fast-templates-0.2.0/fasttemplates/templates/extras/db/mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/db/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/db/mongo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:28.868827 fast-templates-0.2.0/fasttemplates/templates/extras/db/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/db/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/templates/extras/db/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-04 23:07:24.000000 fast-templates-0.2.0/fasttemplates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:07:28.868827 fast-templates-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 23:07:24.000000 fast-templates-0.2.0/setup.py
```

### Comparing `fast-templates-0.1.9/LICENSE` & `fast-templates-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/PKG-INFO` & `fast-templates-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.9
+Version: 0.2.0
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
@@ -15,23 +15,27 @@
 =======================
 
 CLI that contains fastapi templates for different projects
 
 Installation
 ============
 
+This package is designed to be used with (`venv <https://docs.python.org/3/library/venv.html>`_), so make sure you have a virtual environment set up.
+
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install Fast-Templates.
 
 .. code-block:: bash
 
    pip install fast-templates
 
 Usage
 =====
 
+Once installed, and after activating your virtual environment, you can run the following command to see the available templates:
+
 .. code-block:: bash
 
    fastcli
 
 License
 =======
```

### Comparing `fast-templates-0.1.9/fast_templates.egg-info/PKG-INFO` & `fast-templates-0.2.0/fast_templates.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.9
+Version: 0.2.0
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
@@ -15,23 +15,27 @@
 =======================
 
 CLI that contains fastapi templates for different projects
 
 Installation
 ============
 
+This package is designed to be used with (`venv <https://docs.python.org/3/library/venv.html>`_), so make sure you have a virtual environment set up.
+
 Use the package manager `pip <https://pip.pypa.io/en/stable/>`_ to install Fast-Templates.
 
 .. code-block:: bash
 
    pip install fast-templates
 
 Usage
 =====
 
+Once installed, and after activating your virtual environment, you can run the following command to see the available templates:
+
 .. code-block:: bash
 
    fastcli
 
 License
 =======
```

### Comparing `fast-templates-0.1.9/fast_templates.egg-info/SOURCES.txt` & `fast-templates-0.2.0/fast_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/fasttemplates/constants.py` & `fast-templates-0.2.0/fasttemplates/constants.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/fasttemplates/main.py` & `fast-templates-0.2.0/fasttemplates/main.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/fasttemplates/templates/extras/cache/redis/app/utils/cache.py` & `fast-templates-0.2.0/fasttemplates/templates/extras/cache/redis/app/utils/cache.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/fasttemplates/utils.py` & `fast-templates-0.2.0/fasttemplates/utils.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.9/setup.py` & `fast-templates-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='fast-templates',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     package_data={'': ['**/*', '.env', '.gitignore']},
     url='https://github.com/pybalt/FastAPI-TemplateWizard',
     author='pybalt',
     author_email='96897286+pybalt@users.noreply.github.com',
     description='A CLI to generate FastAPI templates',
     long_description=long_description,
```

