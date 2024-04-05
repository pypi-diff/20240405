# Comparing `tmp/pytest-helm-templates-0.0.1a2.tar.gz` & `tmp/pytest-helm-templates-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-helm-templates-0.0.1a2.tar", last modified: Thu Apr  4 16:23:24 2024, max compression
+gzip compressed data, was "pytest-helm-templates-0.0.1a3.tar", last modified: Thu Apr  4 22:11:12 2024, max compression
```

## Comparing `pytest-helm-templates-0.0.1a2.tar` & `pytest-helm-templates-0.0.1a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/template_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/helm_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:23:24.418665 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:23:24.000000 pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 16:23:24.422665 pytest-helm-templates-0.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-04 16:22:38.000000 pytest-helm-templates-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:11:12.274634 pytest-helm-templates-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-04 22:11:12.274634 pytest-helm-templates-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:11:12.266634 pytest-helm-templates-0.0.1a3/pytest_helm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:11:12.266634 pytest-helm-templates-0.0.1a3/pytest_helm_templates/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates/commands/template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates/helm_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:11:12.266634 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-04 22:11:12.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 22:11:12.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:11:12.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-04 22:11:12.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 22:11:12.000000 pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:11:12.274634 pytest-helm-templates-0.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-04 22:10:29.000000 pytest-helm-templates-0.0.1a3/setup.py
```

### Comparing `pytest-helm-templates-0.0.1a2/LICENSE` & `pytest-helm-templates-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a2/PKG-INFO` & `pytest-helm-templates-0.0.1a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
@@ -15,61 +15,63 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYaml~=6.0.1
+Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: all
-Requires-Dist: PyYaml~=6.0.1; extra == "all"
-Requires-Dist: black~=23.12.1; extra == "all"
-Requires-Dist: build==1.0.3; extra == "all"
-Requires-Dist: coverage==7.4.4; extra == "all"
-Requires-Dist: coverage-badge==1.1.0; extra == "all"
-Requires-Dist: dlint==0.14.1; extra == "all"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "all"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "all"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "all"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
+Requires-Dist: pyyaml~=6.0.1; extra == "all"
+Requires-Dist: black~=24.2.0; extra == "all"
+Requires-Dist: build~=1.0.3; extra == "all"
+Requires-Dist: coverage~=7.4.4; extra == "all"
+Requires-Dist: coverage-badge~=1.1.0; extra == "all"
+Requires-Dist: dlint~=0.14.1; extra == "all"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "all"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "all"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "all"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "all"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "all"
+Requires-Dist: flake8~=7.0.0; extra == "all"
+Requires-Dist: isort~=5.13.2; extra == "all"
 Requires-Dist: mypy~=1.8.0; extra == "all"
-Requires-Dist: pep8-naming==0.13.3; extra == "all"
-Requires-Dist: pre-commit==3.6.0; extra == "all"
+Requires-Dist: pep8-naming~=0.13.3; extra == "all"
+Requires-Dist: pre-commit~=3.6.0; extra == "all"
 Requires-Dist: pytest-mock~=3.12.0; extra == "all"
-Requires-Dist: pytest-watch~=4.2.0; extra == "all"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "all"
 Requires-Dist: pytest~=7.4.0; extra == "all"
 Requires-Dist: safety==2.3.4; extra == "all"
-Requires-Dist: twine==4.0.2; extra == "all"
-Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "all"
+Requires-Dist: twine~=4.0.2; extra == "all"
+Requires-Dist: types-PyYAML~=6.0.12.20240311; extra == "all"
 Requires-Dist: wheel>=0.42.0; extra == "all"
 Provides-Extra: deps
-Requires-Dist: PyYaml~=6.0.1; extra == "deps"
+Requires-Dist: pyyaml~=6.0.1; extra == "deps"
 Provides-Extra: dev
-Requires-Dist: black~=23.12.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: coverage==7.4.4; extra == "dev"
-Requires-Dist: coverage-badge==1.1.0; extra == "dev"
-Requires-Dist: dlint==0.14.1; extra == "dev"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "dev"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "dev"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "dev"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: build~=1.0.3; extra == "dev"
+Requires-Dist: coverage~=7.4.4; extra == "dev"
+Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
+Requires-Dist: dlint~=0.14.1; extra == "dev"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "dev"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "dev"
+Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
-Requires-Dist: pep8-naming==0.13.3; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
+Requires-Dist: pep8-naming~=0.13.3; extra == "dev"
+Requires-Dist: pre-commit~=3.6.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.12.0; extra == "dev"
-Requires-Dist: pytest-watch~=4.2.0; extra == "dev"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "dev"
 Requires-Dist: pytest~=7.4.0; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
-Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "dev"
+Requires-Dist: twine~=4.0.2; extra == "dev"
+Requires-Dist: types-PyYAML~=6.0.12.20240311; extra == "dev"
 Requires-Dist: wheel>=0.42.0; extra == "dev"
 
 [![code coverage](./.meta/coverage/badge.svg)](./.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/pytest-helm-templates.svg)](https://github.com/tdg5/pytest-helm-templates/blob/main/LICENSE)
 
 # pytest-helm-templates
```

### Comparing `pytest-helm-templates-0.0.1a2/README.md` & `pytest-helm-templates-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a2/pytest_helm_templates/commands/template_command.py` & `pytest-helm-templates-0.0.1a3/pytest_helm_templates/commands/template_command.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a2/pytest_helm_templates/helm_runner.py` & `pytest-helm-templates-0.0.1a3/pytest_helm_templates/helm_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,16 @@
                 skip_tests=True,
                 values=values,
                 version=version,
             )
             notes_output = manifests[0]["NOTES.txt"]
             if not isinstance(notes_output, str):
                 raise ValueError(
-                    (
-                        "Unexpected notes template output. Expected string, got"
-                        " {type(notes_output)}: {notes_output}"
-                    )
+                    "Unexpected notes template output. Expected string, got"
+                    " {type(notes_output)}: {notes_output}"
                 )
             return notes_output
 
     def template(
         self,
         chart: str,
         name: str,
@@ -154,14 +152,12 @@
             env=self.env,
         )
 
         return_code = completed_process.returncode
         if return_code > 0:
             stderr = completed_process.stderr.decode("utf-8")
             raise RuntimeError(
-                (
-                    f"helm command failed with return code {return_code}:"
-                    f"exec {helm_arguments}\n{stderr}"
-                )
+                f"helm command failed with return code {return_code}:"
+                f"exec {helm_arguments}\n{stderr}"
             )
 
         return completed_process.stdout.decode("utf-8")
```

### Comparing `pytest-helm-templates-0.0.1a2/pytest_helm_templates.egg-info/PKG-INFO` & `pytest-helm-templates-0.0.1a3/pytest_helm_templates.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Pytest fixtures for unit testing the output of helm templates
 Home-page: https://github.com/tdg5/pytest-helm-templates
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT
 Keywords: [TODO]
 Classifier: Framework :: Pytest
@@ -15,61 +15,63 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYaml~=6.0.1
+Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: all
-Requires-Dist: PyYaml~=6.0.1; extra == "all"
-Requires-Dist: black~=23.12.1; extra == "all"
-Requires-Dist: build==1.0.3; extra == "all"
-Requires-Dist: coverage==7.4.4; extra == "all"
-Requires-Dist: coverage-badge==1.1.0; extra == "all"
-Requires-Dist: dlint==0.14.1; extra == "all"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "all"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "all"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "all"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
+Requires-Dist: pyyaml~=6.0.1; extra == "all"
+Requires-Dist: black~=24.2.0; extra == "all"
+Requires-Dist: build~=1.0.3; extra == "all"
+Requires-Dist: coverage~=7.4.4; extra == "all"
+Requires-Dist: coverage-badge~=1.1.0; extra == "all"
+Requires-Dist: dlint~=0.14.1; extra == "all"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "all"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "all"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "all"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "all"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "all"
+Requires-Dist: flake8~=7.0.0; extra == "all"
+Requires-Dist: isort~=5.13.2; extra == "all"
 Requires-Dist: mypy~=1.8.0; extra == "all"
-Requires-Dist: pep8-naming==0.13.3; extra == "all"
-Requires-Dist: pre-commit==3.6.0; extra == "all"
+Requires-Dist: pep8-naming~=0.13.3; extra == "all"
+Requires-Dist: pre-commit~=3.6.0; extra == "all"
 Requires-Dist: pytest-mock~=3.12.0; extra == "all"
-Requires-Dist: pytest-watch~=4.2.0; extra == "all"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "all"
 Requires-Dist: pytest~=7.4.0; extra == "all"
 Requires-Dist: safety==2.3.4; extra == "all"
-Requires-Dist: twine==4.0.2; extra == "all"
-Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "all"
+Requires-Dist: twine~=4.0.2; extra == "all"
+Requires-Dist: types-PyYAML~=6.0.12.20240311; extra == "all"
 Requires-Dist: wheel>=0.42.0; extra == "all"
 Provides-Extra: deps
-Requires-Dist: PyYaml~=6.0.1; extra == "deps"
+Requires-Dist: pyyaml~=6.0.1; extra == "deps"
 Provides-Extra: dev
-Requires-Dist: black~=23.12.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: coverage==7.4.4; extra == "dev"
-Requires-Dist: coverage-badge==1.1.0; extra == "dev"
-Requires-Dist: dlint==0.14.1; extra == "dev"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "dev"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "dev"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "dev"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: build~=1.0.3; extra == "dev"
+Requires-Dist: coverage~=7.4.4; extra == "dev"
+Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
+Requires-Dist: dlint~=0.14.1; extra == "dev"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "dev"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "dev"
+Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
-Requires-Dist: pep8-naming==0.13.3; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
+Requires-Dist: pep8-naming~=0.13.3; extra == "dev"
+Requires-Dist: pre-commit~=3.6.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.12.0; extra == "dev"
-Requires-Dist: pytest-watch~=4.2.0; extra == "dev"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "dev"
 Requires-Dist: pytest~=7.4.0; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
-Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "dev"
+Requires-Dist: twine~=4.0.2; extra == "dev"
+Requires-Dist: types-PyYAML~=6.0.12.20240311; extra == "dev"
 Requires-Dist: wheel>=0.42.0; extra == "dev"
 
 [![code coverage](./.meta/coverage/badge.svg)](./.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/pytest-helm-templates.svg)](https://github.com/tdg5/pytest-helm-templates/blob/main/LICENSE)
 
 # pytest-helm-templates
```

### Comparing `pytest-helm-templates-0.0.1a2/setup.py` & `pytest-helm-templates-0.0.1a3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 
 VERSION_PATH = path.join(path.abspath(path.dirname(__file__)), "VERSION")
 
 with open(VERSION_PATH, encoding="utf-8", mode="r") as f:
     VERSION = f.read().strip()
 
 _dependencies = [
-    "PyYaml~=6.0.1",
+    "pyyaml~=6.0.1",
 ]
 
 _dev_dependencies = [
-    "black~=23.12.1",
-    "build==1.0.3",
-    "coverage==7.4.4",
-    "coverage-badge==1.1.0",
-    "dlint==0.14.1",
-    "flake8-comprehensions==3.14.0",
-    "flake8-eradicate==1.5.0",
-    "flake8-spellcheck==0.28.0",
-    "flake8-typing-imports==1.15.0",
-    "flake8==7.0.0",
-    "isort==5.13.2",
+    "black~=24.2.0",
+    "build~=1.0.3",
+    "coverage~=7.4.4",
+    "coverage-badge~=1.1.0",
+    "dlint~=0.14.1",
+    "flake8-comprehensions~=3.14.0",
+    "flake8-eradicate~=1.5.0",
+    "flake8-pyproject~=1.2.3",
+    "flake8-spellcheck~=0.28.0",
+    "flake8-typing-imports~=1.15.0",
+    "flake8~=7.0.0",
+    "isort~=5.13.2",
     "mypy~=1.8.0",
-    "pep8-naming==0.13.3",
-    "pre-commit==3.6.0",
+    "pep8-naming~=0.13.3",
+    "pre-commit~=3.6.0",
     "pytest-mock~=3.12.0",
-    "pytest-watch~=4.2.0",
+    "pytest-watcher~=0.4.2",
     "pytest~=7.4.0",
     "safety==2.3.4",
-    "twine==4.0.2",
-    "types-PyYAML==6.0.12.20240311",
+    "twine~=4.0.2",
+    "types-PyYAML~=6.0.12.20240311",
     "wheel>=0.42.0",
 ]
 
 
 def _setup_packages() -> List:
     default_packages = [
         "pytest_helm_templates",
```

