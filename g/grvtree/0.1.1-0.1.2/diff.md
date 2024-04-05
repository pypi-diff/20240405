# Comparing `tmp/grvtree-0.1.1.tar.gz` & `tmp/grvtree-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grvtree-0.1.1.tar", max compression
+gzip compressed data, was "grvtree-0.1.2.tar", max compression
```

## Comparing `grvtree-0.1.1.tar` & `grvtree-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-04 07:01:38.167759 grvtree-0.1.1/README.md
--rw-r--r--   0        0        0    14631 2024-04-05 00:36:31.663764 grvtree-0.1.1/grvtree/__init__.py
--rw-r--r--   0        0        0      592 2024-04-05 00:37:04.416998 grvtree-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 grvtree-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 07:01:38.167759 grvtree-0.1.2/README.md
+-rw-r--r--   0        0        0    14716 2024-04-05 12:39:27.150665 grvtree-0.1.2/grvtree/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-05 12:39:39.478448 grvtree-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 grvtree-0.1.2/PKG-INFO
```

### Comparing `grvtree-0.1.1/grvtree/__init__.py` & `grvtree-0.1.2/grvtree/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     The last cells are not counted, either.
     """
 
     matched_lex_cat: int
     matched_form: int
 
     def lengths(
-        self, cut_end: bool = False, relative: bool = True
+        self, cut_end: bool = True, relative: bool = True
     ):  # -> tuple[Any, Any]:# -> tuple[Any, Any]:
         return (
             self.length_this - (1 if cut_end else 0) - (1 if relative else 0),
             self.length_other - (1 if cut_end else 0) - (1 if relative else 0),
         )
 
     def precision_height_diff(self, relative: bool = True) -> float:
@@ -60,24 +60,24 @@
         else:
             return (
                 self.matched_height_diff
                 + (1 if not relative and self.first_height_diff_match else 0)
             ) / max(len_this, len_other)
 
     def precision_phrase_cat(self) -> float:
-        if (max_len := max(self.lengths())) <= 1:
+        if (max_len := max(self.lengths(cut_end=True, relative=False))) <= 1:
             return 1
         else:
             return self.matched_phrase_cat / (max_len - 1)
 
     def precision_lex_cat(self) -> float:
-        return self.matched_lex_cat / max(self.lengths())
+        return self.matched_lex_cat / max(self.lengths(cut_end=False, relative=False))
 
     def precision_form(self) -> float:
-        return self.matched_form / max(self.lengths())
+        return self.matched_form / max(self.lengths(cut_end=False, relative=False))
 
     def to_dict(self, relative: bool = True) -> dict[str, int | float]:
         return {
             **dataclasses.asdict(self),
             "precision_height_diff": self.precision_height_diff(relative=relative),
             "precision_phrase_cat": self.precision_phrase_cat(),
             "precision_lex_cat": self.precision_lex_cat(),
```

### Comparing `grvtree-0.1.1/pyproject.toml` & `grvtree-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grvtree"
-version = "0.1.1"
+version = "0.1.2"
 description = "An implementation of Gómez-Rodríguez and Vilares' tree linearization"
 homepage = "https://pypi.org/project/grvtree/"
 repository = "https://github.com/aslemen/GRV-tree"
 authors = ["Nori Hayashi <net@hayashi-lin.net>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `grvtree-0.1.1/PKG-INFO` & `grvtree-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grvtree
-Version: 0.1.1
+Version: 0.1.2
 Summary: An implementation of Gómez-Rodríguez and Vilares' tree linearization
 Home-page: https://pypi.org/project/grvtree/
 License: Apache-2.0
 Author: Nori Hayashi
 Author-email: net@hayashi-lin.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

