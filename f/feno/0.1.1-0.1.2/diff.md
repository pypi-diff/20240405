# Comparing `tmp/feno-0.1.1.tar.gz` & `tmp/feno-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.1.tar", last modified: Thu Apr  4 23:45:13 2024, max compression
+gzip compressed data, was "feno-0.1.2.tar", last modified: Fri Apr  5 00:33:00 2024, max compression
```

## Comparing `feno-0.1.1.tar` & `feno-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.342985 feno-0.1.1/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.1/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.1/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)      899 2024-04-04 23:45:13.342985 feno-0.1.1/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.1.1/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      558 2024-04-04 23:38:13.000000 feno-0.1.1/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.1/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-04 23:45:13.342985 feno-0.1.1/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.1/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.329652 feno-0.1.1/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.339652 feno-0.1.1/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-04 23:26:18.000000 feno-0.1.1/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1994 2024-04-04 23:24:21.000000 feno-0.1.1/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5184 2024-04-04 23:40:16.000000 feno-0.1.1/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.1/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.1/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.1/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.1/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8485 2024-04-04 23:00:46.000000 feno-0.1.1/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.1/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3435 2024-04-04 23:36:07.000000 feno-0.1.1/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.1/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.1/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.1/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.1/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-04 23:45:13.342985 feno-0.1.1/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)      899 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-04 23:45:13.000000 feno-0.1.1/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.316221 feno-0.1.2/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.2/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.2/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2322 2024-04-05 00:33:00.316221 feno-0.1.2/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1469 2024-04-05 00:25:42.000000 feno-0.1.2/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      558 2024-04-04 23:38:13.000000 feno-0.1.2/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.2/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-05 00:33:00.316221 feno-0.1.2/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.2/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.302888 feno-0.1.2/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.309554 feno-0.1.2/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-05 00:32:44.000000 feno-0.1.2/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2003 2024-04-04 23:51:34.000000 feno-0.1.2/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5188 2024-04-04 23:50:56.000000 feno-0.1.2/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.2/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.2/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.2/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.2/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8485 2024-04-04 23:00:46.000000 feno-0.1.2/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.2/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.2/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.2/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.2/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.2/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.2/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-05 00:33:00.312888 feno-0.1.2/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2322 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-05 00:33:00.000000 feno-0.1.2/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.1/LICENSE` & `feno-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/changelog.md` & `feno-0.1.2/changelog.md`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/setup.py` & `feno-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/__main__.py` & `feno-0.1.2/src/feno/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         exit(1)
 
     for target in args.targets:
         hook = os.path.basename(os.path.abspath(target))
 
         actions = Actions(target, args.remote, args.tko)
         Log.resume(hook, end=": [ ")
-        Log.verbose(hook)
+        Log.verbose(hook, end=" ")
 
         if not actions.validate():
             continue
 
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
```

### Comparing `feno-0.1.1/src/feno/actions.py` & `feno-0.1.2/src/feno/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         shutil.rmtree(self.cache)
         os.makedirs(self.cache)
         return self
     
     def need_rebuild(self):
         if Check.need_rebuild(self.source_dir, self.target):
             Log.resume("Changes ", end="")
-            Log.verbose(f"changes in {self.source_dir}")
+            Log.verbose(f"    Changes in {self.source_dir}")
             return True
             
         Log.verbose("")
         return False
     
     def remote_md(self):
         cfg = RemoteCfg()
```

### Comparing `feno-0.1.1/src/feno/cases.py` & `feno-0.1.2/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/check.py` & `feno-0.1.2/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/css_style.py` & `feno-0.1.2/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/filter.py` & `feno-0.1.2/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/html.py` & `feno-0.1.2/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/indexer.py` & `feno-0.1.2/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/jsontools.py` & `feno-0.1.2/src/feno/jsontools.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
                     for file in cfg["required"]:
                         self.add_required(norm_join(source, file))
             return True
         return False
     
     def load_drafts(self, cache_draft: str):
         found = False
+        if not os.path.isdir(cache_draft):
+            return False
         for lang in os.listdir(cache_draft):
             lang_path = norm_join(cache_draft, lang)
             if os.path.isdir(lang_path):
                 for file in os.listdir(lang_path):
                     file_path = norm_join(lang_path, file)
                     self.add_draft(lang, file_path)
                     found = True
```

### Comparing `feno-0.1.1/src/feno/mdpp.py` & `feno-0.1.2/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/remote_md.py` & `feno-0.1.2/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno/tree.py` & `feno-0.1.2/src/feno/tree.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.1/src/feno.egg-info/SOURCES.txt` & `feno-0.1.2/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

