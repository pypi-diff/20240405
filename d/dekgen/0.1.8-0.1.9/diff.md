# Comparing `tmp/dekgen-0.1.8.tar.gz` & `tmp/dekgen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekgen-0.1.8.tar", last modified: Sun Mar  3 15:27:35 2024, max compression
+gzip compressed data, was "dekgen-0.1.9.tar", last modified: Sat Mar 16 14:36:55 2024, max compression
```

## Comparing `dekgen-0.1.8.tar` & `dekgen-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/__init__.py
--rw-r--r--   0        0        0       42 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/click/__entry__.py
--rw-r--r--   0        0        0      521 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/click/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/python/__init__.py
--rw-r--r--   0        0        0     3370 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/python/generator.py
--rw-r--r--   0        0        0     5574 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/python/imports.py
--rw-r--r--   0        0        0     1205 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/python/template/__init__.py
--rw-r--r--   0        0        0      180 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/code/python/template/env.py
--rw-r--r--   0        0        0     5090 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/resloader/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/tmpl/__init__.py
--rw-r--r--   0        0        0      749 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/tmpl/env.py
--rw-r--r--   0        0        0     3905 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/tmpl/generator.py
--rw-r--r--   0        0        0     1042 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/tmpl/render.py
--rw-r--r--   0        0        0     4272 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/tmpl/template.py
--rw-r--r--   0        0        0        0 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/utils/__init__.py
--rw-r--r--   0        0        0      268 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/utils/yaml/__init__.py
--rw-r--r--   0        0        0       20 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/utils/yaml/tags/__init__.py
--rw-r--r--   0        0        0     5806 2024-03-03 15:27:33.393513 dekgen-0.1.8/dekgen/utils/yaml/tags/tmpl.py
--rw-r--r--   0        0        0      482 2024-03-03 15:27:35.149514 dekgen-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      606 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0       25 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/render/templates/.dockerignore
--rw-r--r--   0        0        0       52 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/render/templates/main.txt
--rw-r--r--   0        0        0       32 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/render/values.test.yaml
--rw-r--r--   0        0        0       36 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/render/values.yaml
--rw-r--r--   0        0        0      315 2024-03-03 15:27:33.393513 dekgen-0.1.8/tests/res/test.yaml
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dekgen-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/__init__.py
+-rw-r--r--   0        0        0       42 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/click/__entry__.py
+-rw-r--r--   0        0        0      725 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/click/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/python/__init__.py
+-rw-r--r--   0        0        0     3370 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/python/generator.py
+-rw-r--r--   0        0        0     5574 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/python/imports.py
+-rw-r--r--   0        0        0     1205 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/python/template/__init__.py
+-rw-r--r--   0        0        0      180 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/code/python/template/env.py
+-rw-r--r--   0        0        0     5090 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/resloader/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/tmpl/__init__.py
+-rw-r--r--   0        0        0      749 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/tmpl/env.py
+-rw-r--r--   0        0        0     3905 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/tmpl/generator.py
+-rw-r--r--   0        0        0     1062 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/tmpl/render.py
+-rw-r--r--   0        0        0     4272 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/tmpl/template.py
+-rw-r--r--   0        0        0        0 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/utils/__init__.py
+-rw-r--r--   0        0        0      268 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/utils/yaml/__init__.py
+-rw-r--r--   0        0        0       20 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/utils/yaml/tags/__init__.py
+-rw-r--r--   0        0        0     5806 2024-03-16 14:36:54.317262 dekgen-0.1.9/dekgen/utils/yaml/tags/tmpl.py
+-rw-r--r--   0        0        0      482 2024-03-16 14:36:55.581254 dekgen-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      606 2024-03-16 14:36:54.317262 dekgen-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0       25 2024-03-16 14:36:54.317262 dekgen-0.1.9/tests/render/templates/.dockerignore
+-rw-r--r--   0        0        0       52 2024-03-16 14:36:54.317262 dekgen-0.1.9/tests/render/templates/main.txt
+-rw-r--r--   0        0        0       32 2024-03-16 14:36:54.317262 dekgen-0.1.9/tests/render/values.test.yaml
+-rw-r--r--   0        0        0       36 2024-03-16 14:36:54.321262 dekgen-0.1.9/tests/render/values.yaml
+-rw-r--r--   0        0        0      315 2024-03-16 14:36:54.321262 dekgen-0.1.9/tests/res/test.yaml
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 dekgen-0.1.9/PKG-INFO
```

### Comparing `dekgen-0.1.8/dekgen/code/python/generator.py` & `dekgen-0.1.9/dekgen/code/python/generator.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/code/python/imports.py` & `dekgen-0.1.9/dekgen/code/python/imports.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/code/python/template/__init__.py` & `dekgen-0.1.9/dekgen/code/python/template/__init__.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/resloader/__init__.py` & `dekgen-0.1.9/dekgen/resloader/__init__.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/tmpl/env.py` & `dekgen-0.1.9/dekgen/tmpl/env.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/tmpl/generator.py` & `dekgen-0.1.9/dekgen/tmpl/generator.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/tmpl/render.py` & `dekgen-0.1.9/dekgen/tmpl/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class RenderTemplate(TemplateWide):
     file_ignore_tpl = [f"../{x}" for x in TemplateWide.file_ignore_tpl]
     file_ignore_override = [f"../{x}" for x in TemplateWide.file_ignore_override]
     file_ignore = [f"../{x}" for x in TemplateWide.file_ignore]
 
 
-def render_dir(dest, src, files=None, updated=None):
+def render_dir(dest, src, files=None, updated=None, **kwargs):
     data = {}
     path_values = os.path.join(src, 'values.yaml')
     if os.path.isfile(path_values):
         data = dict(Values=yaml.load(path_values))
     if files:
         for f in files:
             strict = True
@@ -23,8 +23,8 @@
                 f = f[1:]
                 strict = False
             if not strict and not os.path.isfile(f):
                 continue
             dict_merge(data, dict(Values=yaml.load(f)))
     if updated:
         object_path_update(data, updated)
-    RenderTemplate(data).render_dir(dest, os.path.join(src, 'templates'))
+    RenderTemplate(data, **kwargs).render_dir(dest, os.path.join(src, 'templates'))
```

### Comparing `dekgen-0.1.8/dekgen/tmpl/template.py` & `dekgen-0.1.9/dekgen/tmpl/template.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/dekgen/utils/yaml/tags/tmpl.py` & `dekgen-0.1.9/dekgen/utils/yaml/tags/tmpl.py`

 * *Files identical despite different names*

### Comparing `dekgen-0.1.8/tests/__init__.py` & `dekgen-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

