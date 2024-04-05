# Comparing `tmp/cmi_docx-0.1.2.tar.gz` & `tmp/cmi_docx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmi_docx-0.1.2.tar", max compression
+gzip compressed data, was "cmi_docx-0.1.3.tar", max compression
```

## Comparing `cmi_docx-0.1.2.tar` & `cmi_docx-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26526 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/LICENSE
--rw-r--r--   0        0        0     2762 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/README.md
--rw-r--r--   0        0        0     1557 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      295 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/__init__.py
--rw-r--r--   0        0        0     4921 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/document.py
--rw-r--r--   0        0        0     4925 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/paragraph.py
--rw-r--r--   0        0        0     4253 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/run.py
--rw-r--r--   0        0        0     2684 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/table.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-04 20:43:29.851616 cmi_docx-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2762 2024-04-04 20:43:29.851616 cmi_docx-0.1.3/README.md
+-rw-r--r--   0        0        0     1557 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      295 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/src/cmi_docx/__init__.py
+-rw-r--r--   0        0        0     4921 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/src/cmi_docx/document.py
+-rw-r--r--   0        0        0     4925 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/src/cmi_docx/paragraph.py
+-rw-r--r--   0        0        0     4747 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/src/cmi_docx/run.py
+-rw-r--r--   0        0        0     2684 2024-04-04 20:43:29.855616 cmi_docx-0.1.3/src/cmi_docx/table.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.3/PKG-INFO
```

### Comparing `cmi_docx-0.1.2/LICENSE` & `cmi_docx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.2/README.md` & `cmi_docx-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.2/pyproject.toml` & `cmi_docx-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmi_docx"
-version = "0.1.2"
+version = "0.1.3"
 description = ".docx utilities"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cmi_docx", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cmi_docx-0.1.2/src/cmi_docx/document.py` & `cmi_docx-0.1.3/src/cmi_docx/document.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.2/src/cmi_docx/paragraph.py` & `cmi_docx-0.1.3/src/cmi_docx/paragraph.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.2/src/cmi_docx/run.py` & `cmi_docx-0.1.3/src/cmi_docx/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 """Module for extending python-docx Run objects."""
 
-import dataclasses
-
 from docx import shared
 from docx.text import paragraph as docx_paragraph
 
 
-@dataclasses.dataclass
 class FindRun:
     """Data class for maintaing find results in runs.
 
     Attributes:
         paragraph: The paragraph containing the text.
         run_indices: The run indices of the text needle's start and end.
         character_indices: The character indices of the text in the runs.
             The first index is the start of the text in the first run containing
             the text. The second index is the end of the text in the last run.
     """
 
-    paragraph: docx_paragraph.Paragraph
-    run_indices: tuple[int, int]
-    character_indices: tuple[int, int]
+    def __init__(
+        self,
+        paragraph: docx_paragraph.Paragraph,
+        run_indices: tuple[int, int],
+        character_indices: tuple[int, int],
+    ) -> None:
+        """Initializes a FindRun object.
+
+        Args:
+            paragraph: The paragraph containing the text.
+            run_indices: The run indices of the text needle's start and end.
+            character_indices: The character indices of the text in the runs.
+        """
+        self.paragraph = paragraph
+        self.run_indices = run_indices
+        self.character_indices = character_indices
 
     @property
     def runs(self) -> list[docx_paragraph.Run]:
         """Returns the runs containing the text."""
         return self.paragraph.runs[self.run_indices[0] : self.run_indices[1] + 1]
 
     def replace(self, replace: str) -> None:
         """Replaces the text in the runs with the replacement text.
 
         Args:
             replace: The text to replace.
         """
         start = self.character_indices[0]
         end = self.character_indices[1]
-        if len(self.runs) > 1:
-            self.runs[0].text = (
-                self.runs[0].text[:start] + replace + self.runs[-1].text[end:]
-            )
-        else:
+
+        if len(self.runs) == 1:
             self.runs[0].text = (
                 self.runs[0].text[:start] + replace + self.runs[0].text[end:]
             )
-        self.run_indices = (self.run_indices[0], self.run_indices[0])
+        else:
+            self.runs[0].text = self.runs[0].text[:start] + replace
+            for run in self.runs[1:-1]:
+                run.clear()
+            self.runs[-1].text = self.runs[-1].text[end:]
         self.character_indices = (start, start + len(replace))
+        self.run_indices = (self.run_indices[0], self.run_indices[0])
 
     def __lt__(self, other: "FindRun") -> bool:
         """Sorts FindRun in order of appearance in the paragraph.
 
         Makes FindRun objects sortable.
 
         Args:
```

### Comparing `cmi_docx-0.1.2/src/cmi_docx/table.py` & `cmi_docx-0.1.3/src/cmi_docx/table.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.2/PKG-INFO` & `cmi_docx-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmi_docx
-Version: 0.1.2
+Version: 0.1.3
 Summary: .docx utilities
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

