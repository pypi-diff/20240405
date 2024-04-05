# Comparing `tmp/lxml_html_clean-0.1.0.tar.gz` & `tmp/lxml_html_clean-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxml_html_clean-0.1.0.tar", last modified: Mon Feb 26 13:16:04 2024, max compression
+gzip compressed data, was "lxml_html_clean-0.1.1.tar", last modified: Fri Apr  5 06:50:03 2024, max compression
```

## Comparing `lxml_html_clean-0.1.0.tar` & `lxml_html_clean-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-02-26 13:16:04.842037 lxml_html_clean-0.1.0/
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1488 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.0/LICENSE.txt
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1520 2024-02-26 13:16:04.842037 lxml_html_clean-0.1.0/PKG-INFO
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      727 2024-02-26 13:07:31.000000 lxml_html_clean-0.1.0/README.md
-drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-02-26 13:16:04.841036 lxml_html_clean-0.1.0/lxml_html_clean/
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       21 2024-02-26 10:33:55.000000 lxml_html_clean-0.1.0/lxml_html_clean/__init__.py
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)    28166 2024-02-26 12:04:38.000000 lxml_html_clean-0.1.0/lxml_html_clean/clean.py
-drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-02-26 13:16:04.842037 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1520 2024-02-26 13:16:04.000000 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/PKG-INFO
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      322 2024-02-26 13:16:04.000000 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/SOURCES.txt
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)        1 2024-02-26 13:16:04.000000 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/dependency_links.txt
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)        5 2024-02-26 13:16:04.000000 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/requires.txt
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       16 2024-02-26 13:16:04.000000 lxml_html_clean-0.1.0/lxml_html_clean.egg-info/top_level.txt
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       87 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.0/pyproject.toml
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      845 2024-02-26 13:16:04.842037 lxml_html_clean-0.1.0/setup.cfg
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       37 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.0/setup.py
-drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-02-26 13:16:04.842037 lxml_html_clean-0.1.0/tests/
--rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)    11510 2024-02-26 10:35:21.000000 lxml_html_clean-0.1.0/tests/test_clean.py
+drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-04-05 06:50:03.419258 lxml_html_clean-0.1.1/
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1488 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.1/LICENSE.txt
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1520 2024-04-05 06:50:03.419258 lxml_html_clean-0.1.1/PKG-INFO
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      727 2024-02-26 13:07:31.000000 lxml_html_clean-0.1.1/README.md
+drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-04-05 06:50:03.418258 lxml_html_clean-0.1.1/lxml_html_clean/
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       21 2024-02-26 10:33:55.000000 lxml_html_clean-0.1.1/lxml_html_clean/__init__.py
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)    28167 2024-04-05 06:41:20.000000 lxml_html_clean-0.1.1/lxml_html_clean/clean.py
+drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-04-05 06:50:03.419258 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)     1520 2024-04-05 06:50:03.000000 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/PKG-INFO
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      322 2024-04-05 06:50:03.000000 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)        1 2024-04-05 06:50:03.000000 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)        5 2024-04-05 06:50:03.000000 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/requires.txt
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       16 2024-04-05 06:50:03.000000 lxml_html_clean-0.1.1/lxml_html_clean.egg-info/top_level.txt
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       87 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.1/pyproject.toml
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)      845 2024-04-05 06:50:03.420258 lxml_html_clean-0.1.1/setup.cfg
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)       37 2024-02-26 10:36:17.000000 lxml_html_clean-0.1.1/setup.py
+drwxr-xr-x   0 lbalhar   (1000) lbalhar   (1000)        0 2024-04-05 06:50:03.419258 lxml_html_clean-0.1.1/tests/
+-rw-r--r--   0 lbalhar   (1000) lbalhar   (1000)    12354 2024-04-05 06:41:20.000000 lxml_html_clean-0.1.1/tests/test_clean.py
```

### Comparing `lxml_html_clean-0.1.0/LICENSE.txt` & `lxml_html_clean-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lxml_html_clean-0.1.0/PKG-INFO` & `lxml_html_clean-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxml_html_clean
-Version: 0.1.0
+Version: 0.1.1
 Summary: HTML cleaner from lxml project
 Home-page: https://github.com/fedora-python/lxml_html_clean/
 Author: Lumír Balhar
 Author-email: lbalhar@redhat.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://lxml-html-clean.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lxml_html_clean-0.1.0/README.md` & `lxml_html_clean-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lxml_html_clean-0.1.0/lxml_html_clean/clean.py` & `lxml_html_clean-0.1.1/lxml_html_clean/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 _looks_like_tag_content = re.compile(
     r'</?[a-zA-Z]+|\son[a-zA-Z]+\s*=',
     (re.ASCII)).search
 
 # All kinds of schemes besides just javascript: that can cause
 # execution:
 _find_image_dataurls = re.compile(
-    r'data:image/(.+);base64,', re.I).findall
+    r'data:image/(.+?);base64,', re.I).findall
 _possibly_malicious_schemes = re.compile(
     r'(javascript|jscript|livescript|vbscript|data|about|mocha):',
     re.I).findall
 # SVG images can contain script content
 _is_unsafe_image_type = re.compile(r"(xml|svg)", re.I).search
 
 def _has_javascript_scheme(s):
```

### Comparing `lxml_html_clean-0.1.0/lxml_html_clean.egg-info/PKG-INFO` & `lxml_html_clean-0.1.1/lxml_html_clean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxml_html_clean
-Version: 0.1.0
+Version: 0.1.1
 Summary: HTML cleaner from lxml project
 Home-page: https://github.com/fedora-python/lxml_html_clean/
 Author: Lumír Balhar
 Author-email: lbalhar@redhat.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://lxml-html-clean.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lxml_html_clean-0.1.0/setup.cfg` & `lxml_html_clean-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lxml_html_clean
-version = 0.1.0
+version = 0.1.1
 description = HTML cleaner from lxml project
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/fedora-python/lxml_html_clean/
 project_urls = 
 	Documentation = https://lxml-html-clean.readthedocs.io/
 author = Lumír Balhar
```

### Comparing `lxml_html_clean-0.1.0/tests/test_clean.py` & `lxml_html_clean-0.1.1/tests/test_clean.py`

 * *Files 9% similar despite different names*

```diff
@@ -251,14 +251,39 @@
 
             cleaned = lxml.html.tostring(clean_html(s))
             self.assertEqual(
                 html.encode("UTF-8"),
                 cleaned,
                 "%s  ->  %s" % (url, cleaned))
 
+    def test_image_data_links_in_inline_style(self):
+        safe_attrs = set(lxml.html.defs.safe_attrs)
+        safe_attrs.add('style')
+
+        cleaner = Cleaner(
+            safe_attrs_only=True,
+            safe_attrs=safe_attrs)
+
+        data = b'123'
+        data_b64 = base64.b64encode(data).decode('ASCII')
+        url = "url(data:image/jpeg;base64,%s)" % data_b64
+        styles = [
+            "background: %s" % url,
+            "background: %s; background-image: %s" % (url, url),
+        ]
+        for style in styles:
+            html = '<div style="%s"></div>' % style
+            s = lxml.html.fragment_fromstring(html)
+
+            cleaned = lxml.html.tostring(cleaner.clean_html(s))
+            self.assertEqual(
+                html.encode("UTF-8"),
+                cleaned,
+                "%s  ->  %s" % (style, cleaned))
+
     def test_formaction_attribute_in_button_input(self):
         # The formaction attribute overrides the form's action and should be
         # treated as a malicious link attribute
         html = ('<form id="test"><input type="submit" formaction="javascript:alert(1)"></form>'
         '<button form="test" formaction="javascript:alert(1)">X</button>')
         expected = ('<div><form id="test"><input type="submit" formaction=""></form>'
         '<button form="test" formaction="">X</button></div>')
```

