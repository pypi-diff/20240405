# Comparing `tmp/yippy-1.0.0.tar.gz` & `tmp/yippy-1.1.0.tar.gz`

## Comparing `yippy-1.0.0.tar` & `yippy-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 yippy-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 yippy-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 yippy-1.0.0/README.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.0.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 yippy-1.0.0/src/yippy/__init__.py
--rwxr-xr-x   0        0        0    18971 2020-02-02 00:00:00.000000 yippy-1.0.0/src/yippy/coronagraph.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 yippy-1.0.0/src/yippy/logger.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yippy-1.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.0.0/LICENSE
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 yippy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 yippy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 yippy-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 yippy-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 yippy-1.1.0/README.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 yippy-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 yippy-1.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yippy-1.1.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/_version.py
+-rwxr-xr-x   0        0        0    10284 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/coronagraph.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/logger.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/offax_base.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/util.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/offax_psf/__init__.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/offax_psf/one_d.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/offax_psf/quarter_symmetric.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 yippy-1.1.0/src/yippy/offax_psf/two_d.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yippy-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yippy-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 yippy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 yippy-1.1.0/PKG-INFO
```

### Comparing `yippy-1.0.0/.pre-commit-config.yaml` & `yippy-1.1.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,24 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.5.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.0
+    rev: v0.3.4
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
     rev: v3.1.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
         args: []
+  # - repo: https://github.com/RobertCraigie/pyright-python
+  #   rev: v1.1.355
+  #   hooks:
+  #   - id: pyright
```

### Comparing `yippy-1.0.0/CHANGELOG.md` & `yippy-1.1.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [1.1.0](https://github.com/CoreySpohn/yippy/compare/v1.0.0...v1.1.0) (2024-04-05)
+
+
+### Features
+
+* **main:** Add off-axis psfs with automatic unit conversion ([6f5b815](https://github.com/CoreySpohn/yippy/commit/6f5b815093e6fe7898cd625451ad31ab1acee221))
+
 ## 1.0.0 (2024-03-22)
 
 
 ### Features
 
 * Automatic versioning and changelog ([ef1acc1](https://github.com/CoreySpohn/yippy/commit/ef1acc1381058fdb32f6b32bb3d695a2035ad048))
```

### Comparing `yippy-1.0.0/.github/workflows/publish-to-pypi.yml` & `yippy-1.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.0.0/.github/workflows/release-please.yml` & `yippy-1.1.0/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `yippy-1.0.0/src/yippy/logger.py` & `yippy-1.1.0/src/yippy/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+"""Logging module for yippy."""
+
 import logging
 
 
 def setup_logger(shell_level="INFO", file_level="DEBUG", disable_shell_logging=False):
+    """Set up the logger."""
     # Map string level names to logging levels
     level_mapping = {
         "CRITICAL": logging.CRITICAL,
         "ERROR": logging.ERROR,
         "WARNING": logging.WARNING,
         "INFO": logging.INFO,
         "DEBUG": logging.DEBUG,
@@ -18,25 +21,26 @@
 
     logger.setLevel(logging.DEBUG)  # Set the lowest level to capture all logs
 
     # File Handler
     file_handler = logging.FileHandler("debug.log")
     file_handler.setLevel(level_mapping.get(file_level.upper(), logging.DEBUG))
     file_fmt = (
-        "%(levelname)s %(asctime)s [%(filename)s:%(funcName)s:%(lineno)d] %(message)s"
+        "[yippy] %(levelname)s %(asctime)s "
+        "[%(filename)s:%(funcName)s:%(lineno)d] %(message)s"
     )
     file_formatter = logging.Formatter(file_fmt)
     file_handler.setFormatter(file_formatter)
     logger.addHandler(file_handler)
 
     # Shell Handler
     if not disable_shell_logging:
         shell_handler = logging.StreamHandler()
         shell_handler.setLevel(level_mapping.get(shell_level.upper(), logging.INFO))
-        shell_fmt = "%(levelname)s [%(asctime)s] %(message)s"
+        shell_fmt = "yippy %(levelname)s [%(asctime)s] %(message)s"
         shell_formatter = logging.Formatter(shell_fmt)
         shell_handler.setFormatter(shell_formatter)
         logger.addHandler(shell_handler)
 
     logger.propagate = False
     return logger
```

### Comparing `yippy-1.0.0/.gitignore` & `yippy-1.1.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+*_version.py
+.DS_Store
```

### Comparing `yippy-1.0.0/LICENSE` & `yippy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yippy-1.0.0/PKG-INFO` & `yippy-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yippy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A minimal wrapper to create a coronagraph object from a yield input package
 Project-URL: Homepage, https://github.com/CoreySpohn/yippy
 Project-URL: Issues, https://github.com/CoreySpohn/yippy/issues
 Author-email: Corey Spohn <corey.a.spohn@nasa.gov>
 License: MIT License
         
         Copyright (c) 2024 Corey Spohn
@@ -27,16 +27,28 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.9
 Requires-Dist: astropy
 Requires-Dist: lod-unit
-Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tqdm
+Requires-Dist: xarray
+Provides-Extra: docs
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-autoapi; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinx-book-theme; extra == 'docs'
+Provides-Extra: test
+Requires-Dist: hypothesis; extra == 'test'
+Requires-Dist: nox; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # yippy
 A minimal wrapper to create a coronagraph object from a yield input package
```

