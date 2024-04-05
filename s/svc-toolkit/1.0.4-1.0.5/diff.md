# Comparing `tmp/svc_toolkit-1.0.4.tar.gz` & `tmp/svc_toolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svc_toolkit-1.0.4.tar", max compression
+gzip compressed data, was "svc_toolkit-1.0.5.tar", max compression
```

## Comparing `svc_toolkit-1.0.4.tar` & `svc_toolkit-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      851 2024-04-04 11:13:01.632975 svc_toolkit-1.0.4/README.md
--rw-r--r--   0        0        0     1459 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/conversion/__init__.py
--rw-r--r--   0        0        0      787 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/conversion/converter.py
--rw-r--r--   0        0        0     2443 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/conversion/converter_trainer.py
--rw-r--r--   0        0        0     1056 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/conversion/mixer.py
--rw-r--r--   0        0        0    12669 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/img/icon.png
--rw-r--r--   0        0        0    31498 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/img/loading.gif
--rw-r--r--   0        0        0     2377 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/main.py
--rw-r--r--   0        0        0      214 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/models/manifest.yml
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/__init__.py
--rw-r--r--   0        0        0      293 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/common.py
--rw-r--r--   0        0        0      828 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/conversion.py
--rw-r--r--   0        0        0      613 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/mixing.py
--rw-r--r--   0        0        0     2595 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/separation.py
--rw-r--r--   0        0        0      675 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/presenter/training.py
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/__init__.py
--rw-r--r--   0        0        0      987 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/audio.py
--rw-r--r--   0        0        0      196 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/constants.py
--rw-r--r--   0        0        0     7065 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/data.py
--rw-r--r--   0        0        0     2168 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/evaluator.py
--rw-r--r--   0        0        0     1985 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/logger.py
--rw-r--r--   0        0        0     7133 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/models.py
--rw-r--r--   0        0        0     3580 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/preprocess.py
--rw-r--r--   0        0        0     4697 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/separator.py
--rw-r--r--   0        0        0      752 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation/utility.py
--rw-r--r--   0        0        0     1290 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation_evaluation.py
--rw-r--r--   0        0        0      978 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation_preprocess.py
--rw-r--r--   0        0        0     3922 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/separation_train.py
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/utility/__init__.py
--rw-r--r--   0        0        0      239 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/utility/functions.py
--rw-r--r--   0        0        0        0 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/__init__.py
--rw-r--r--   0        0        0     7941 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/common.py
--rw-r--r--   0        0        0     7972 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/conversion.py
--rw-r--r--   0        0        0      760 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/loading_overlay.py
--rw-r--r--   0        0        0      993 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/loading_window.py
--rw-r--r--   0        0        0      578 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/main_window.py
--rw-r--r--   0        0        0     3325 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/mixing.py
--rw-r--r--   0        0        0     4679 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/separation.py
--rw-r--r--   0        0        0     5279 2024-04-04 11:13:01.636976 svc_toolkit-1.0.4/src/svc_toolkit/widget/training.py
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 svc_toolkit-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      897 2024-04-05 01:40:24.743965 svc_toolkit-1.0.5/README.md
+-rw-r--r--   0        0        0     1634 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter.py
+-rw-r--r--   0        0        0     2443 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter_trainer.py
+-rw-r--r--   0        0        0     1056 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/mixer.py
+-rw-r--r--   0        0        0    12669 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/img/icon.png
+-rw-r--r--   0        0        0    31498 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/img/loading.gif
+-rw-r--r--   0        0        0     2377 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/main.py
+-rw-r--r--   0        0        0      197 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/models/manifest.yml
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/common.py
+-rw-r--r--   0        0        0      828 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/conversion.py
+-rw-r--r--   0        0        0      613 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/mixing.py
+-rw-r--r--   0        0        0     2595 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/separation.py
+-rw-r--r--   0        0        0      675 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/training.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/audio.py
+-rw-r--r--   0        0        0      196 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/constants.py
+-rw-r--r--   0        0        0     7065 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/data.py
+-rw-r--r--   0        0        0     2168 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/evaluator.py
+-rw-r--r--   0        0        0     1985 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/logger.py
+-rw-r--r--   0        0        0     7133 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/models.py
+-rw-r--r--   0        0        0     3580 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/preprocess.py
+-rw-r--r--   0        0        0     4697 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/separator.py
+-rw-r--r--   0        0        0      752 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/utility.py
+-rw-r--r--   0        0        0     1290 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_evaluation.py
+-rw-r--r--   0        0        0      978 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_preprocess.py
+-rw-r--r--   0        0        0     3922 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_train.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/utility/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/utility/functions.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/common.py
+-rw-r--r--   0        0        0     7972 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/conversion.py
+-rw-r--r--   0        0        0      760 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_overlay.py
+-rw-r--r--   0        0        0      993 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_window.py
+-rw-r--r--   0        0        0      578 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/main_window.py
+-rw-r--r--   0        0        0     3325 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/mixing.py
+-rw-r--r--   0        0        0     4679 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/separation.py
+-rw-r--r--   0        0        0     5279 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/training.py
+-rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 svc_toolkit-1.0.5/PKG-INFO
```

### Comparing `svc_toolkit-1.0.4/README.md` & `svc_toolkit-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Singing Voice Conversion with GUI
+# Singing Voice Conversion Toolkit
 
 ![Tests](https://github.com/jljl1337/svc-toolkit/actions/workflows/tests.yml/badge.svg)
 ![Deployment](https://github.com/jljl1337/svc-toolkit/actions/workflows/deployments.yml/badge.svg)
 [![Codecov](https://codecov.io/gh/jljl1337/svc-toolkit/graph/badge.svg?token=QBM6OLIG00)](https://codecov.io/gh/jljl1337/svc-toolkit)
 
-A self-contained singing voice conversion using so-vits-svc, with vocal separation
-and easy to use GUI.
+A self-contained singing voice conversion using the so-vits-svc architecture, 
+with Deep U-Net model for vocal separation feature and easy to use GUI.
 
 ## Getting Started
 
 ### Installation
 
 1. Install [pipx](https://github.com/pypa/pipx)
```

### Comparing `svc_toolkit-1.0.4/pyproject.toml` & `svc_toolkit-1.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "svc-toolkit"
-version = "1.0.4"
-description = "A self-contained singing voice conversion toolkit."
+version = "1.0.5"
+description = "A self-contained singing voice conversion using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI."
 authors = ["jljl1337 <lckjack123@gmail.com>"]
 license = ""
 readme = "README.md"
-#repository = ""
-#documentation = ""
+repository = "https://github.com/jljl1337/svc-toolkit"
+documentation = "https://jljl1337.github.io/svc-toolkit/"
 classifiers = [
     "Operating System :: OS Independent",
 ]
 packages = [
    { include = "svc_toolkit", from = "src" },
 ]
```

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/conversion/converter.py` & `svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/conversion/converter_trainer.py` & `svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter_trainer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/conversion/mixer.py` & `svc_toolkit-1.0.5/src/svc_toolkit/conversion/mixer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/img/icon.png` & `svc_toolkit-1.0.5/src/svc_toolkit/img/icon.png`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/img/loading.gif` & `svc_toolkit-1.0.5/src/svc_toolkit/img/loading.gif`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/main.py` & `svc_toolkit-1.0.5/src/svc_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/presenter/conversion.py` & `svc_toolkit-1.0.5/src/svc_toolkit/presenter/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/presenter/mixing.py` & `svc_toolkit-1.0.5/src/svc_toolkit/presenter/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/presenter/separation.py` & `svc_toolkit-1.0.5/src/svc_toolkit/presenter/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/presenter/training.py` & `svc_toolkit-1.0.5/src/svc_toolkit/presenter/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/audio.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/audio.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/data.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/data.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/evaluator.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/evaluator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/logger.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/logger.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/models.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/models.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/preprocess.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/separator.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/separator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation/utility.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation/utility.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation_evaluation.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation_evaluation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation_preprocess.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation_preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/separation_train.py` & `svc_toolkit-1.0.5/src/svc_toolkit/separation_train.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/common.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/common.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/conversion.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/loading_overlay.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_overlay.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/loading_window.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/main_window.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/main_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/mixing.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/separation.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/src/svc_toolkit/widget/training.py` & `svc_toolkit-1.0.5/src/svc_toolkit/widget/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.4/PKG-INFO` & `svc_toolkit-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: svc-toolkit
-Version: 1.0.4
-Summary: A self-contained singing voice conversion toolkit.
+Version: 1.0.5
+Summary: A self-contained singing voice conversion using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI.
+Home-page: https://github.com/jljl1337/svc-toolkit
 Author: jljl1337
 Author-email: lckjack123@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,24 +22,26 @@
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: scikit-learn (==1.4.0)
 Requires-Dist: scipy (==1.12.0)
 Requires-Dist: so-vits-svc-fork (==4.1.40)
 Requires-Dist: torch (==2.1.1)
 Requires-Dist: torchaudio (==2.1.1)
 Requires-Dist: torchmetrics (==1.2.0)
+Project-URL: Documentation, https://jljl1337.github.io/svc-toolkit/
+Project-URL: Repository, https://github.com/jljl1337/svc-toolkit
 Description-Content-Type: text/markdown
 
-# Singing Voice Conversion with GUI
+# Singing Voice Conversion Toolkit
 
 ![Tests](https://github.com/jljl1337/svc-toolkit/actions/workflows/tests.yml/badge.svg)
 ![Deployment](https://github.com/jljl1337/svc-toolkit/actions/workflows/deployments.yml/badge.svg)
 [![Codecov](https://codecov.io/gh/jljl1337/svc-toolkit/graph/badge.svg?token=QBM6OLIG00)](https://codecov.io/gh/jljl1337/svc-toolkit)
 
-A self-contained singing voice conversion using so-vits-svc, with vocal separation
-and easy to use GUI.
+A self-contained singing voice conversion using the so-vits-svc architecture, 
+with Deep U-Net model for vocal separation feature and easy to use GUI.
 
 ## Getting Started
 
 ### Installation
 
 1. Install [pipx](https://github.com/pypa/pipx)
```

