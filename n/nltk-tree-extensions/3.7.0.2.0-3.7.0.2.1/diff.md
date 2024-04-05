# Comparing `tmp/nltk_tree_extensions-3.7.0.2.0.tar.gz` & `tmp/nltk_tree_extensions-3.7.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nltk_tree_extensions-3.7.0.2.0.tar", max compression
+gzip compressed data, was "nltk_tree_extensions-3.7.0.2.1.tar", max compression
```

## Comparing `nltk_tree_extensions-3.7.0.2.0.tar` & `nltk_tree_extensions-3.7.0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-03 13:57:42.619919 nltk_tree_extensions-3.7.0.2.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-04-03 11:47:27.532488 nltk_tree_extensions-3.7.0.2.0/README.md
--rw-r--r--   0        0        0        8 2024-04-03 11:37:21.380969 nltk_tree_extensions-3.7.0.2.0/nltk-stubs/py.typed
--rw-r--r--   0        0        0     7280 2024-04-04 06:14:42.744785 nltk_tree_extensions-3.7.0.2.0/nltk-stubs/tree/tree.pyi
--rw-r--r--   0        0        0        0 2024-04-03 11:02:00.842675 nltk_tree_extensions-3.7.0.2.0/nltk_tree_ext/__init__.py
--rw-r--r--   0        0        0    17069 2024-04-04 14:13:49.952516 nltk_tree_extensions-3.7.0.2.0/nltk_tree_ext/funcs.py
--rw-r--r--   0        0        0      730 2024-04-03 13:56:54.176499 nltk_tree_extensions-3.7.0.2.0/nltk_tree_ext/patch.py
--rw-r--r--   0        0        0      650 2024-04-04 14:36:59.809908 nltk_tree_extensions-3.7.0.2.0/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 nltk_tree_extensions-3.7.0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 13:57:42.619919 nltk_tree_extensions-3.7.0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-03 11:47:27.532488 nltk_tree_extensions-3.7.0.2.1/README.md
+-rw-r--r--   0        0        0        8 2024-04-03 11:37:21.380969 nltk_tree_extensions-3.7.0.2.1/nltk-stubs/py.typed
+-rw-r--r--   0        0        0     7431 2024-04-05 00:40:47.710162 nltk_tree_extensions-3.7.0.2.1/nltk-stubs/tree/tree.pyi
+-rw-r--r--   0        0        0        0 2024-04-03 11:02:00.842675 nltk_tree_extensions-3.7.0.2.1/nltk_tree_ext/__init__.py
+-rw-r--r--   0        0        0    17069 2024-04-04 14:13:49.952516 nltk_tree_extensions-3.7.0.2.1/nltk_tree_ext/funcs.py
+-rw-r--r--   0        0        0      889 2024-04-05 00:39:57.708952 nltk_tree_extensions-3.7.0.2.1/nltk_tree_ext/patch.py
+-rw-r--r--   0        0        0      650 2024-04-05 00:41:14.192789 nltk_tree_extensions-3.7.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 nltk_tree_extensions-3.7.0.2.1/PKG-INFO
```

### Comparing `nltk_tree_extensions-3.7.0.2.0/LICENSE.txt` & `nltk_tree_extensions-3.7.0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nltk_tree_extensions-3.7.0.2.0/nltk-stubs/tree/tree.pyi` & `nltk_tree_extensions-3.7.0.2.1/nltk-stubs/tree/tree.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -220,11 +220,15 @@
         self: Tree[NODE, LEAF]
     ) -> Iterator[
         Literal[funcs.TokenType.OPEN]
         | Literal[funcs.TokenType.CLOSE]
         | tuple[Literal[funcs.TokenType.NODE], NODE]
         | tuple[Literal[funcs.TokenType.LEAF], LEAF]
     ]: ...
-    def encode_skeleton(self: Tree[NODE, LEAF]) -> str: ...
+    def encode_skeleton(self) -> str: ...
     def encode_skeleton_nodes_leaves(
-        self: Tree[NODE, LEAF], indices: dict[NODE | LEAF, str] | None = None
+        self, indices: dict[NODE | LEAF, str] | None = None
     ) -> tuple[str, dict[NODE | LEAF, str]]: ...
+    def levenshtein_ratio_skeleton(self, other: Tree[NODE, LEAF]) -> float: ...
+    def levenshtein_ratio_skeleton_nodes_leaves(
+        self, other: Tree[NODE, LEAF]
+    ) -> float: ...
```

### Comparing `nltk_tree_extensions-3.7.0.2.0/nltk_tree_ext/funcs.py` & `nltk_tree_extensions-3.7.0.2.1/nltk_tree_ext/funcs.py`

 * *Files identical despite different names*

### Comparing `nltk_tree_extensions-3.7.0.2.0/nltk_tree_ext/patch.py` & `nltk_tree_extensions-3.7.0.2.1/nltk_tree_ext/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,7 +9,9 @@
 Tree.iter_leaves_with_branches = funcs.iter_leaves_with_branches
 Tree.overwrite_leaves = funcs.overwrite_leaves
 Tree.merge_nonterminal_unary_nodes = funcs.merge_nonterminal_unary_nodes
 Tree.unfold_nonterminal_unary_nodes = funcs.unfold_nonterminal_unary_nodes
 Tree.to_tokens = funcs.to_tokens
 Tree.encode_skeleton = funcs.encode_skeleton
 Tree.encode_skeleton_nodes_leaves = funcs.encode_skeleton_nodes_leaves
+Tree.levenshtein_ratio_skeleton = funcs.levenshtein_ratio_skeleton
+Tree.levenshtein_ratio_skeleton_nodes_leaves = funcs.levenshtein_ratio_skeleton_nodes_leaves
```

### Comparing `nltk_tree_extensions-3.7.0.2.0/pyproject.toml` & `nltk_tree_extensions-3.7.0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nltk-tree-extensions"
-version = "3.7.0.2.0"
+version = "3.7.0.2.1"
 description = "An extension module for nltk.tree"
 authors = ["Nori Hayashi <net@hayashi-lin.net>"]
 homepage = "https://pypi.com/project/nltk-tree-extensions"
 repository = "https://github.com/aslemen/nltk-tree-extensions"
 readme = "README.md"
 packages = [
     { include = "nltk_tree_ext" },
```

### Comparing `nltk_tree_extensions-3.7.0.2.0/PKG-INFO` & `nltk_tree_extensions-3.7.0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nltk-tree-extensions
-Version: 3.7.0.2.0
+Version: 3.7.0.2.1
 Summary: An extension module for nltk.tree
 Home-page: https://pypi.com/project/nltk-tree-extensions
 License: Apache-2.0
 Author: Nori Hayashi
 Author-email: net@hayashi-lin.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

