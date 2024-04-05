# Comparing `tmp/pysen-plugins-2023.5.22.tar.gz` & `tmp/pysen-plugins-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysen-plugins-2023.5.22.tar", last modified: Mon May 22 03:36:17 2023, max compression
+gzip compressed data, was "pysen-plugins-2024.4.5.tar", last modified: Fri Apr  5 08:11:36 2024, max compression
```

## Comparing `pysen-plugins-2023.5.22.tar` & `pysen-plugins-2024.4.5.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/
--rw-r--r--   0 root         (0) root         (0)     1081 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2207 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/README.md
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.132679 pysen-plugins-2023.5.22/pysen_plugins/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-22 03:35:48.000000 pysen-plugins-2023.5.22/pysen_plugins/_version.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/clang_format.py
--rw-r--r--   0 root         (0) root         (0)     3495 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/cmake_format.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/golint.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/goreturns.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/jq.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/mypy_init_check.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/mypy_simple.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/prettier.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins/pylint/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/command.py
--rw-r--r--   0 root         (0) root         (0)      607 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/component.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/pylint/plugin.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruamel_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins/ruff/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4732 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/ruff/preset.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/shellcheck.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/shfmt.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/pysen_plugins/tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/pysen_plugins.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2207 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-22 03:36:17.000000 pysen-plugins-2023.5.22/pysen_plugins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 03:36:17.136013 pysen-plugins-2023.5.22/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-22 03:31:54.000000 pysen-plugins-2023.5.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.598263 pysen-plugins-2024.4.5/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-05 08:11:36.598263 pysen-plugins-2024.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      350 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.594929 pysen-plugins-2024.4.5/pysen_plugins/
+-rw-r--r--   0 root         (0) root         (0)      617 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-05 08:11:20.000000 pysen-plugins-2024.4.5/pysen_plugins/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/clang_format.py
+-rw-r--r--   0 root         (0) root         (0)     3495 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/cmake_format.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.594929 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/black.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/flake8.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/isort.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/mypy.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/customizable_builtins/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/golint.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/goreturns.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/jq.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/mypy_init_check.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/mypy_simple.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/prettier.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.594929 pysen-plugins-2024.4.5/pysen_plugins/pylint/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/pylint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/pylint/command.py
+-rw-r--r--   0 root         (0) root         (0)      607 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/pylint/component.py
+-rw-r--r--   0 root         (0) root         (0)      660 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/pylint/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/ruamel_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.598263 pysen-plugins-2024.4.5/pysen_plugins/ruff/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/ruff/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/ruff/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/ruff/preset.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/shellcheck.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/shfmt.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/pysen_plugins/tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:11:36.594929 pysen-plugins-2024.4.5/pysen_plugins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-05 08:11:36.000000 pysen-plugins-2024.4.5/pysen_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-05 08:11:36.000000 pysen-plugins-2024.4.5/pysen_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 08:11:36.000000 pysen-plugins-2024.4.5/pysen_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-05 08:11:36.000000 pysen-plugins-2024.4.5/pysen_plugins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-05 08:11:36.000000 pysen-plugins-2024.4.5/pysen_plugins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 08:11:36.598263 pysen-plugins-2024.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-05 08:01:58.000000 pysen-plugins-2024.4.5/setup.py
```

### Comparing `pysen-plugins-2023.5.22/LICENSE` & `pysen-plugins-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/PKG-INFO` & `pysen-plugins-2024.4.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pysen-plugins
-Version: 2023.5.22
+Version: 2024.4.5
 Summary: Collection of pysen plugins
-Author: Toru Ogawa, Ryo Miyajima, Yuki Igarashi
-Author-email: ogawa@preferred.jp, ryo@preferred.jp, igarashi@preferred.jp
+Author: Toru Ogawa, Ryo Miyajima, Linsho Kaku
+Author-email: ogawa@preferred.jp, ryo@preferred.jp, linsho@preferred.jp
 License: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,14 +56,19 @@
   - [jq](https://stedolan.github.io/jq) (lint, format)
   - [prettier](https://prettier.io) (lint, format)
 - Python
   - mypy_init_check (lint)
   - mypy_simple (lint)
   - [pylint](http://pylint.pycqa.org) (lint)
   - [ruff](https://github.com/charliermarsh/ruff) (lint, format)
+  - customizable_builtins (lint, format)
+    - black
+    - isort
+    - flake8
+    - mypy
 - Shell script
   - [shellcheck](https://github.com/koalaman/shellcheck) (lint)
   - [shfmt](https://github.com/mvdan/sh) (lint, format)
 - TypeScript
   - [prettier](https://prettier.io) (lint, format)
 - XML
   - [tidy](http://www.html-tidy.org) (lint, format)
```

### Comparing `pysen-plugins-2023.5.22/README.md` & `pysen-plugins-2024.4.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,19 @@
   - [jq](https://stedolan.github.io/jq) (lint, format)
   - [prettier](https://prettier.io) (lint, format)
 - Python
   - mypy_init_check (lint)
   - mypy_simple (lint)
   - [pylint](http://pylint.pycqa.org) (lint)
   - [ruff](https://github.com/charliermarsh/ruff) (lint, format)
+  - customizable_builtins (lint, format)
+    - black
+    - isort
+    - flake8
+    - mypy
 - Shell script
   - [shellcheck](https://github.com/koalaman/shellcheck) (lint)
   - [shfmt](https://github.com/mvdan/sh) (lint, format)
 - TypeScript
   - [prettier](https://prettier.io) (lint, format)
 - XML
   - [tidy](http://www.html-tidy.org) (lint, format)
```

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/__init__.py` & `pysen-plugins-2024.4.5/pysen_plugins/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .clang_format import clang_format  # NOQA
 from .cmake_format import cmake_format  # NOQA
+from .customizable_builtins import customizable_builtins  # NOQA
 from .golint import golint  # NOQA
 from .goreturns import goreturns  # NOQA
 from .jq import jq  # NOQA
 from .mypy_init_check import mypy_init_check  # NOQA
 from .mypy_simple import mypy_simple  # NOQA
 from .prettier import prettier  # NOQA
 from .pylint import pylint  # NOQA
```

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/clang_format.py` & `pysen-plugins-2024.4.5/pysen_plugins/clang_format.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/cmake_format.py` & `pysen-plugins-2024.4.5/pysen_plugins/cmake_format.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/golint.py` & `pysen-plugins-2024.4.5/pysen_plugins/golint.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/goreturns.py` & `pysen-plugins-2024.4.5/pysen_plugins/goreturns.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/jq.py` & `pysen-plugins-2024.4.5/pysen_plugins/jq.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/mypy_init_check.py` & `pysen-plugins-2024.4.5/pysen_plugins/mypy_init_check.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/mypy_simple.py` & `pysen-plugins-2024.4.5/pysen_plugins/mypy_simple.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/prettier.py` & `pysen-plugins-2024.4.5/pysen_plugins/prettier.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/pylint/command.py` & `pysen-plugins-2024.4.5/pysen_plugins/pylint/command.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/pylint/component.py` & `pysen-plugins-2024.4.5/pysen_plugins/pylint/component.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/pylint/plugin.py` & `pysen-plugins-2024.4.5/pysen_plugins/pylint/plugin.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/ruamel_yaml.py` & `pysen-plugins-2024.4.5/pysen_plugins/ruamel_yaml.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/ruff/plugin.py` & `pysen-plugins-2024.4.5/pysen_plugins/ruff/plugin.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/ruff/preset.py` & `pysen-plugins-2024.4.5/pysen_plugins/ruff/preset.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/shellcheck.py` & `pysen-plugins-2024.4.5/pysen_plugins/shellcheck.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/shfmt.py` & `pysen-plugins-2024.4.5/pysen_plugins/shfmt.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins/tidy.py` & `pysen-plugins-2024.4.5/pysen_plugins/tidy.py`

 * *Files identical despite different names*

### Comparing `pysen-plugins-2023.5.22/pysen_plugins.egg-info/PKG-INFO` & `pysen-plugins-2024.4.5/pysen_plugins.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pysen-plugins
-Version: 2023.5.22
+Version: 2024.4.5
 Summary: Collection of pysen plugins
-Author: Toru Ogawa, Ryo Miyajima, Yuki Igarashi
-Author-email: ogawa@preferred.jp, ryo@preferred.jp, igarashi@preferred.jp
+Author: Toru Ogawa, Ryo Miyajima, Linsho Kaku
+Author-email: ogawa@preferred.jp, ryo@preferred.jp, linsho@preferred.jp
 License: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,14 +56,19 @@
   - [jq](https://stedolan.github.io/jq) (lint, format)
   - [prettier](https://prettier.io) (lint, format)
 - Python
   - mypy_init_check (lint)
   - mypy_simple (lint)
   - [pylint](http://pylint.pycqa.org) (lint)
   - [ruff](https://github.com/charliermarsh/ruff) (lint, format)
+  - customizable_builtins (lint, format)
+    - black
+    - isort
+    - flake8
+    - mypy
 - Shell script
   - [shellcheck](https://github.com/koalaman/shellcheck) (lint)
   - [shfmt](https://github.com/mvdan/sh) (lint, format)
 - TypeScript
   - [prettier](https://prettier.io) (lint, format)
 - XML
   - [tidy](http://www.html-tidy.org) (lint, format)
```

### Comparing `pysen-plugins-2023.5.22/setup.py` & `pysen-plugins-2024.4.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 setup(
     name="pysen-plugins",
     version=__version__,  # type: ignore[name-defined]  # NOQA: F821
     packages=find_packages(),
     description="Collection of pysen plugins",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="Toru Ogawa, Ryo Miyajima, Yuki Igarashi",
-    author_email="ogawa@preferred.jp, ryo@preferred.jp, igarashi@preferred.jp",
+    author="Toru Ogawa, Ryo Miyajima, Linsho Kaku",
+    author_email="ogawa@preferred.jp, ryo@preferred.jp, linsho@preferred.jp",
     license="MIT License",
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Operating System :: MacOS",
         "Operating System :: Unix",
     ],
-    install_requires=["pysen>=0.10.0,<0.11.0"],
+    install_requires=["pysen>=0.11.0,<0.12.0"],
     package_data={"pysen_plugins": ["py.typed"]},
 )
```

