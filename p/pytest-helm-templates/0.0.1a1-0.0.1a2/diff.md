# Comparing `tmp/pytest-helm-templates-0.0.1a1.tar.gz` & `tmp/pytest-helm-templates-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-helm-templates-0.0.1a1.tar", last modified: Thu Apr  4 14:05:37 2024, max compression
+gzip compressed data, was "pytest-helm-templates-0.0.1a2.tar", last modified: Thu Apr  4 16:23:24 2024, max compression
```

## Comparing `pytest-helm-templates-0.0.1a1.tar` & `pytest-helm-templates-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/template_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates/helm_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:37.380186 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:05:37.000000 pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 14:05:37.388186 pytest-helm-templates-0.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 14:04:52.000000 pytest-helm-templates-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/helm_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/setup.py
```

### Comparing `pytest-helm-templates-0.0.1a1/LICENSE` & `pytest-helm-templates-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/PKG-INFO` & `pytest-helm-templates-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
```

### Comparing `pytest-helm-templates-0.0.1a1/README.md` & `pytest-helm-templates-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/pyproject.toml` & `pytest-helm-templates-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/pytest_helm_templates/commands/template_command.py` & `pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/template_command.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/pytest_helm_templates/helm_runner.py` & `pytest-helm-templates-0.0.1a2/pytest_helm_templates/helm_runner.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/PKG-INFO` & `pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
```

### Comparing `pytest-helm-templates-0.0.1a1/pytest_helm_templates.egg-info/requires.txt` & `pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a1/setup.py` & `pytest-helm-templates-0.0.1a2/setup.py`

 * *Files identical despite different names*

