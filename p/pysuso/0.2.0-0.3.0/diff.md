# Comparing `tmp/pysuso-0.2.0.tar.gz` & `tmp/pysuso-0.3.0.tar.gz`

## Comparing `pysuso-0.2.0.tar` & `pysuso-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 pysuso-0.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pysuso-0.2.0/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pysuso-0.2.0/README.md
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 pysuso-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pysuso-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 pysuso-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pysuso-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pysuso-0.3.0/README.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 pysuso-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pysuso-0.3.0/PKG-INFO
```

### Comparing `pysuso-0.2.0/.gitignore` & `pysuso-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pysuso-0.2.0/LICENSE` & `pysuso-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysuso-0.2.0/README.md` & `pysuso-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ```py
 solver.solve()
 ```
 
 Full example including imports:
 
-```py
+```py linenums="1"
 from pysuso.boards import Board
 from pysuso.solvers import BasicSolver
 
 board = Board.from_list(
     [
         0, 5, 0, 7, 0, 3, 0, 6, 0,
         0, 0, 7, 0, 0, 0, 8, 0, 0,
```

### Comparing `pysuso-0.2.0/pyproject.toml` & `pysuso-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysuso-0.2.0/PKG-INFO` & `pysuso-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pysuso
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sudoku sovler written in Python
 Project-URL: Home, https://mcneall.github.io/PySuSo/
 Project-URL: Repository, https://github.com/McNeall/PySuSo
 Project-URL: Documentation, https://mcneall.github.io/PySuSo/
 Project-URL: pypi, https://pypi.org/project/pysuso
 Author-email: Robert Schmidt <allthingscoding21th@gmail.com>
 License: MIT
@@ -69,15 +69,15 @@
 
 ```py
 solver.solve()
 ```
 
 Full example including imports:
 
-```py
+```py linenums="1"
 from pysuso.boards import Board
 from pysuso.solvers import BasicSolver
 
 board = Board.from_list(
     [
         0, 5, 0, 7, 0, 3, 0, 6, 0,
         0, 0, 7, 0, 0, 0, 8, 0, 0,
```

