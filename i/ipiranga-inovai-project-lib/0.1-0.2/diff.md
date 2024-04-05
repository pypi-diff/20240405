# Comparing `tmp/ipiranga-inovai-project-lib-0.1.tar.gz` & `tmp/ipiranga-inovai-project-lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.1.tar", last modified: Fri Apr  5 20:03:40 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-0.2.tar", last modified: Fri Apr  5 20:28:57 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.1.tar` & `ipiranga-inovai-project-lib-0.2.tar`

### file list

```diff
@@ -1,22 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.298582 ipiranga-inovai-project-lib-0.1/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.1/LICENSE
--rw-rw-rw-   0        0        0      516 2024-04-05 20:03:40.296714 ipiranga-inovai-project-lib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.294073 ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-04-05 20:03:40.000000 ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2024-04-05 20:03:40.000000 ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:03:40.000000 ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-05 20:03:40.000000 ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 20:03:40.298582 ipiranga-inovai-project-lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-04-05 20:02:50.000000 ipiranga-inovai-project-lib-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.275641 ipiranga-inovai-project-lib-0.1/src/
--rw-rw-rw-   0        0        0        0 2024-04-05 19:41:31.000000 ipiranga-inovai-project-lib-0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.277974 ipiranga-inovai-project-lib-0.1/src/domain/
--rw-rw-rw-   0        0        0        0 2024-04-05 19:16:19.000000 ipiranga-inovai-project-lib-0.1/src/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.281516 ipiranga-inovai-project-lib-0.1/src/domain/entity/
--rw-rw-rw-   0        0        0        0 2024-02-06 13:06:58.000000 ipiranga-inovai-project-lib-0.1/src/domain/entity/__init__.py
--rw-rw-rw-   0        0        0    12475 2024-02-28 20:27:08.000000 ipiranga-inovai-project-lib-0.1/src/domain/entity/entities.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:03:40.289950 ipiranga-inovai-project-lib-0.1/src/domain/enum/
--rw-rw-rw-   0        0        0        0 2024-02-06 13:06:58.000000 ipiranga-inovai-project-lib-0.1/src/domain/enum/__init__.py
--rw-rw-rw-   0        0        0      111 2024-04-05 19:41:36.000000 ipiranga-inovai-project-lib-0.1/src/domain/enum/document_movement_type.py
--rw-rw-rw-   0        0        0      189 2024-04-05 19:41:36.000000 ipiranga-inovai-project-lib-0.1/src/domain/enum/document_status.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:28:57.373690 ipiranga-inovai-project-lib-0.2/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.2/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-04-05 20:28:57.366790 ipiranga-inovai-project-lib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 20:28:57.366790 ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-04-05 20:28:57.000000 ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-05 20:28:57.000000 ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:28:57.000000 ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:28:57.000000 ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 20:28:57.373690 ipiranga-inovai-project-lib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-04-05 20:28:34.000000 ipiranga-inovai-project-lib-0.2/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.1/PKG-INFO` & `ipiranga-inovai-project-lib-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.1
+Version: 0.2
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.1/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-0.2/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.1
+Version: 0.2
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.1/setup.py` & `ipiranga-inovai-project-lib-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

