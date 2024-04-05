# Comparing `tmp/plink_pipelines-0.1.7a0.tar.gz` & `tmp/plink_pipelines-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plink_pipelines-0.1.7a0.tar", max compression
+gzip compressed data, was "plink_pipelines-0.2.0.tar", max compression
```

## Comparing `plink_pipelines-0.1.7a0.tar` & `plink_pipelines-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2021-06-10 12:58:24.000000 plink_pipelines-0.1.7a0/LICENSE
--rw-r--r--   0        0        0        0 2021-06-10 12:58:24.000000 plink_pipelines-0.1.7a0/plink_pipelines/__init__.py
--rw-r--r--   0        0        0    15580 2023-04-13 15:22:21.776348 plink_pipelines-0.1.7a0/plink_pipelines/make_dataset.py
--rw-r--r--   0        0        0      417 2023-04-13 15:18:20.326181 plink_pipelines-0.1.7a0/plink_pipelines/validation_functions.py
--rw-r--r--   0        0        0      845 2023-07-21 13:16:16.940552 plink_pipelines-0.1.7a0/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plink_pipelines-0.1.7a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-05 18:21:28.527252 plink_pipelines-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-05 18:21:28.527252 plink_pipelines-0.2.0/plink_pipelines/__init__.py
+-rw-r--r--   0        0        0    15672 2024-04-05 18:21:28.527252 plink_pipelines-0.2.0/plink_pipelines/make_dataset.py
+-rw-r--r--   0        0        0      417 2024-04-05 18:21:28.527252 plink_pipelines-0.2.0/plink_pipelines/validation_functions.py
+-rw-r--r--   0        0        0      848 2024-04-05 18:21:28.527252 plink_pipelines-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 plink_pipelines-0.2.0/PKG-INFO
```

### Comparing `plink_pipelines-0.1.7a0/LICENSE` & `plink_pipelines-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plink_pipelines-0.1.7a0/plink_pipelines/make_dataset.py` & `plink_pipelines-0.2.0/plink_pipelines/make_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import subprocess
 import warnings
+import logging
 from pathlib import Path
 from shutil import copyfile, rmtree, which
 from typing import Generator, Tuple, Literal, Optional, Sequence
 
 import deeplake
 import luigi
 import numpy as np
@@ -15,14 +16,17 @@
 from luigi.task import flatten
 from luigi.util import requires, inherits
 
 from plink_pipelines.validation_functions import validate_cl_args
 
 logger = get_logger(name=__name__)
 
+luigi_logger = logging.getLogger("luigi")
+luigi_logger.setLevel(logging.INFO)
+
 
 class RenameOnFailureMixin(object):
     def on_failure(self, exception):
         targets = luigi.task.flatten(self.output())
         for target in targets:
             if target.exists() and isinstance(target, luigi.LocalTarget):
                 target_path = Path(target.path)
@@ -490,15 +494,15 @@
         action="store_true",
         help="Whether to only use autosomes. " "Only applicable if do_qc is set.",
     )
 
     parser.add_argument(
         "--extract_snp_file",
         type=str,
-        default=None,
+        default="",
         help=".bim file to use if generating only the "
         "intersection between the data and the "
         "specified .bim file.",
     )
 
     return parser
```

### Comparing `plink_pipelines-0.1.7a0/pyproject.toml` & `plink_pipelines-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "plink_pipelines"
-version = "0.1.7-alpha"
+version = "0.2.0"
 description = ""
 authors = ["Arnor Sigurdsson <arnor-sigurdsson@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^2.0.3"
-py = "^1.10.0"
-luigi = "^3.0.3"
+python = ">=3.10,<4.0"
+pandas = "^2.2.1"
+py = "^1.11.0"
+luigi = "^3.5.0"
 aislib = "^0.1.6-alpha.0"
-bed-reader = "^0.2.24"
-deeplake = "^3.0.13"
+bed-reader = "^1.0.2"
+deeplake = "^3.8.27"
 # Freeze numpy due to some 1.24 compatibility issues
-numpy = "1.23.5"
+numpy = "^1.26.4"
 
 [tool.poetry.scripts]
 plink_pipelines = "plink_pipelines.make_dataset:main"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^6.2.5"
-tox = "^3.23.1"
-flake8 = "^4.0.1"
+pytest = "^8.1.1"
+tox = "^4.14.2"
+flake8 = "^7.0.0"
 jupyter = "^1.0.0"
-ipykernel = "^6.5.0"
-Sphinx = "^4.0.2"
-coverage = "^6.1.1"
-snakeviz = "^2.1.0"
-pytest-cov = "^3.0.0"
+ipykernel = "^6.29.4"
+Sphinx = "^7.2.6"
+coverage = "^7.4.4"
+snakeviz = "^2.2.0"
+pytest-cov = "^5.0.0"
 pynvim = "^0.4.3"
-visidata = "^2.4"
-pre-commit = "^2.13.0"
-black = "^23.3.0"
+visidata = "^3.0.2"
+pre-commit = "^3.7.0"
+black = "^24.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plink_pipelines-0.1.7a0/PKG-INFO` & `plink_pipelines-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: plink-pipelines
-Version: 0.1.7a0
+Name: plink_pipelines
+Version: 0.2.0
 Summary: 
 Author: Arnor Sigurdsson
 Author-email: arnor-sigurdsson@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aislib (>=0.1.6-alpha.0,<0.2.0)
-Requires-Dist: bed-reader (>=0.2.24,<0.3.0)
-Requires-Dist: deeplake (>=3.0.13,<4.0.0)
-Requires-Dist: luigi (>=3.0.3,<4.0.0)
-Requires-Dist: numpy (==1.23.5)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: py (>=1.10.0,<2.0.0)
+Requires-Dist: bed-reader (>=1.0.2,<2.0.0)
+Requires-Dist: deeplake (>=3.8.27,<4.0.0)
+Requires-Dist: luigi (>=3.5.0,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: py (>=1.11.0,<2.0.0)
```

