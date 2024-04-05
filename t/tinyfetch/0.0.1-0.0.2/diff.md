# Comparing `tmp/tinyfetch-0.0.1.tar.gz` & `tmp/tinyfetch-0.0.2.tar.gz`

## Comparing `tinyfetch-0.0.1.tar` & `tinyfetch-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/src/tinyfetch/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/README.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyfetch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/core.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/README.md
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/PKG-INFO
```

### Comparing `tinyfetch-0.0.1/.gitignore` & `tinyfetch-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.1/LICENSE.txt` & `tinyfetch-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.1/pyproject.toml` & `tinyfetch-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 dependencies = []
 
 [project.urls]
 Source = "https://github.com/beucismis/tinyfetch"
 Issues = "https://github.com/beucismis/tinyfetch/issues"
 Documentation = "https://github.com/beucismis/tinyfetch#readme"
 
+[project.scripts]
+tinyfetch = "tinyfetch.cli:main"
+
 [tool.hatch.version]
 path = "src/tinyfetch/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["pytest"]
 
 [tool.hatch.envs.default.scripts]
```

### Comparing `tinyfetch-0.0.1/PKG-INFO` & `tinyfetch-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyfetch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python and system information command-line fetch tool
 Project-URL: Source, https://github.com/beucismis/tinyfetch
 Project-URL: Issues, https://github.com/beucismis/tinyfetch/issues
 Project-URL: Documentation, https://github.com/beucismis/tinyfetch#readme
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -20,14 +20,28 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # tinyfetch
 
 Python and system information command-line fetch tool.
 
+Like this!
+```
+beucismis@thinkpad
+------------------
+Python Version: 3.11.2
+PIP Version: 24.0
+PIP Packages: 8
+Implementation: CPython
+Compiler: GCC 12.2.0
+
+Kernel: Linux-6.1.0-18-amd64
+OS: Devuan GNU/Linux 5 (daedalus) x86_64
+```
+
 ## Installation
 
 ```console
 pip install tinyfetch
 ```
 
 ## License
```

