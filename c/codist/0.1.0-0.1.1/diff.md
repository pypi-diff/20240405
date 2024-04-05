# Comparing `tmp/codist-0.1.0.tar.gz` & `tmp/codist-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codist-0.1.0.tar", last modified: Thu Apr  4 10:38:10 2024, max compression
+gzip compressed data, was "codist-0.1.1.tar", last modified: Fri Apr  5 00:23:18 2024, max compression
```

## Comparing `codist-0.1.0.tar` & `codist-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963887 codist-0.1.0/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-04 10:38:10.963688 codist-0.1.0/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3446 2024-04-04 10:33:01.000000 codist-0.1.0/README.md
--rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-04 10:38:08.000000 codist-0.1.0/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-04 10:38:10.963929 codist-0.1.0/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.960588 codist-0.1.0/src/
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.961963 codist-0.1.0/src/codist/
--rw-r--r--   0 jfin305  (1356368322) 1403514002       44 2024-04-04 10:36:12.000000 codist-0.1.0/src/codist/__init__.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      547 2024-04-04 03:48:03.000000 codist-0.1.0/src/codist/ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     6319 2024-04-04 10:19:05.000000 codist-0.1.0/src/codist/distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1721 2024-04-04 10:12:00.000000 codist-0.1.0/src/codist/tree.py
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963501 codist-0.1.0/src/codist.egg-info/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      304 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963212 codist-0.1.0/tests/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.0/tests/test_ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2654 2024-04-04 07:20:13.000000 codist-0.1.0/tests/test_distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.0/tests/test_trees.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.117203 codist-0.1.1/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-05 00:23:18.116978 codist-0.1.1/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3446 2024-04-04 10:33:01.000000 codist-0.1.1/README.md
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-05 00:22:33.000000 codist-0.1.1/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-05 00:23:18.117252 codist-0.1.1/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.113749 codist-0.1.1/src/
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.114667 codist-0.1.1/src/codist/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      168 2024-04-05 00:21:58.000000 codist-0.1.1/src/codist/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      618 2024-04-04 23:27:33.000000 codist-0.1.1/src/codist/ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     7963 2024-04-05 00:13:19.000000 codist-0.1.1/src/codist/distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     2012 2024-04-05 00:05:36.000000 codist-0.1.1/src/codist/tree.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.116744 codist-0.1.1/src/codist.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      304 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.116306 codist-0.1.1/tests/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.1/tests/test_ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3541 2024-04-04 22:53:09.000000 codist-0.1.1/tests/test_distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.1/tests/test_trees.py
```

### Comparing `codist-0.1.0/PKG-INFO` & `codist-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codist
-Version: 0.1.0
+Version: 0.1.1
 Summary: AST edit distance
 Project-URL: repository, https://github.com/James-Ansley/codist
 Classifier: Development Status :: 1 - Planning
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.12
```

### Comparing `codist-0.1.0/README.md` & `codist-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `codist-0.1.0/pyproject.toml` & `codist-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codist"
-version = "0.1.0"
+version = "0.1.1"
 description = "AST edit distance"
 
 readme = "README.md"
 requires-python = ">=3.12"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `codist-0.1.0/src/codist/ast.py` & `codist-0.1.1/src/codist/ast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+"""
+Utilities for converting abstract syntax trees to :data:`codist.tree.Tree`
+objects
+"""
+
 import ast
 
-from .distance import Tree
-from .tree import t
+from .tree import t, Tree
 
 __all__ = ("parse_ast_silhouette", "ast_silhouette")
 
 
 def parse_ast_silhouette(code: str) -> Tree[str]:
     """
     Parses the given code and returns a Tree containing only AST node type
```

### Comparing `codist-0.1.0/src/codist/tree.py` & `codist-0.1.1/src/codist/tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+"""
+Tree utilities and type definitions.
+"""
+
 from collections.abc import Hashable
 
-__all__ = ("Tree", "Forest", "t", "postorder", "keyroots", "leftmosts")
+__all__ = ("Tree", "t", "postorder", "keyroots", "leftmosts")
+
+from typing import TypeVar
+
+T = TypeVar("T", bound=Hashable)
+#: A tree type.
+#: A tree is any tuple of the form: ``Tree[T] = tuple[T, tuple[Tree[T], ...]]``
+Tree: type["tuple[T, tuple[Tree[T], ...]]"]
 
 type Tree[T: Hashable] = tuple[T, tuple[Tree[T], ...]]
-type Forest[T: Hashable] = tuple[Tree[T], ...]
 
 
 def t[T](
       value: T,
       *children: Tree[T],
 ) -> Tree[T]:
     """Small convenience function to help construct trees"""
@@ -22,15 +32,15 @@
         current = s1.pop()
         s2.append(current[0])
         s1.extend(current[1])
     return tuple(reversed(s2))
 
 
 def keyroots[T](tree: Tree[T]) -> tuple[int, ...]:
-    """keyroot indices for keyroots in ``tree``"""
+    """Postorder traversal of keyroot indices for keyroots in :math:`T`"""
     s1 = [(True, tree)]
     s2 = []
     while s1:
         is_keyroot, current = s1.pop()
         s2.append(is_keyroot)
         _, children = current
         if children:
@@ -46,14 +56,15 @@
     """
     s1 = [tree]
     s2 = []
     while s1:
         current = s1.pop()
         s2.append(current)
         s1.extend(current[1])
+    # memo depends on node identity in postorder traversal, not node value.
     memo = {}
     indices = []
     for i, node in enumerate(reversed(s2)):
         if node[1]:
             child = node[1][0]
             index = memo[id(child)]
             memo[id(node)] = index
```

### Comparing `codist-0.1.0/src/codist.egg-info/PKG-INFO` & `codist-0.1.1/src/codist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codist
-Version: 0.1.0
+Version: 0.1.1
 Summary: AST edit distance
 Project-URL: repository, https://github.com/James-Ansley/codist
 Classifier: Development Status :: 1 - Planning
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.12
```

### Comparing `codist-0.1.0/tests/test_trees.py` & `codist-0.1.1/tests/test_trees.py`

 * *Files identical despite different names*

