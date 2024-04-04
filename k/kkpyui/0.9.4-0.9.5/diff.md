# Comparing `tmp/kkpyui-0.9.4.tar.gz` & `tmp/kkpyui-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyui-0.9.4.tar", max compression
+gzip compressed data, was "kkpyui-0.9.5.tar", max compression
```

## Comparing `kkpyui-0.9.4.tar` & `kkpyui-0.9.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-11-13 02:06:12.416530 kkpyui-0.9.4/LICENSE
--rw-r--r--   0        0        0      944 2023-11-13 02:06:12.416760 kkpyui-0.9.4/README.md
--rw-r--r--   0        0        0      396 2023-11-22 06:22:35.668451 kkpyui-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    35255 2023-11-22 06:22:06.855615 kkpyui-0.9.4/src/kkpyui.py
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 kkpyui-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-11-13 02:06:12.416530 kkpyui-0.9.5/LICENSE
+-rw-r--r--   0        0        0      944 2023-11-13 02:06:12.416760 kkpyui-0.9.5/README.md
+-rw-r--r--   0        0        0      396 2023-11-23 00:43:46.305780 kkpyui-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    35525 2023-11-23 00:43:12.744507 kkpyui-0.9.5/src/kkpyui.py
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 kkpyui-0.9.5/PKG-INFO
```

### Comparing `kkpyui-0.9.4/LICENSE` & `kkpyui-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyui-0.9.4/README.md` & `kkpyui-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `kkpyui-0.9.4/src/kkpyui.py` & `kkpyui-0.9.5/src/kkpyui.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,19 +408,22 @@
     def on_quit(self):
         self.controller.quit(None)
 
 
 class FormController:
     """
     - observe all entries and update model
+    - both form and realtime apps can use this class,
+    - realtime apps can set arg-tracers while form apps can use submit() to update model
     """
 
-    def __init__(self, fm=None, model=None):
-        self.form = fm
+    def __init__(self, form=None, model=None):
+        self.form = form
         self.model = model
+        self.set_progress = lambda title, progress, description: Globals.progressQueue.put((title, progress, description))
 
     def update(self):
         self.model = {pg.get_title(): {entry.text: entry.get_data() for entry in pg.winfo_children()} for pg in self.form.pages.values()}
 
     def load(self, preset):
         """
         - model includes input and config
```

### Comparing `kkpyui-0.9.4/PKG-INFO` & `kkpyui-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkpyui
-Version: 0.9.4
+Version: 0.9.5
 Summary: Tkinter-based GUI widget library for building small tool applications
 Author: Beinan Li
 Author-email: li.beinan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: kkpyutil
```

