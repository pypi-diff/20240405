# Comparing `tmp/acid-xblock-0.3.0.tar.gz` & `tmp/acid-xblock-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acid-xblock-0.3.0.tar", last modified: Wed Mar 20 15:16:54 2024, max compression
+gzip compressed data, was "acid-xblock-0.3.1.tar", last modified: Fri Apr  5 14:38:47 2024, max compression
```

## Comparing `acid-xblock-0.3.0.tar` & `acid-xblock-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.917491 acid-xblock-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-20 15:16:54.917491 acid-xblock-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/acid/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/acid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/acid/public/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/public/test_data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.909491 acid-xblock-0.3.0/acid/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/acid/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/css/acid.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/acid/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/html/acid.html.mako
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/html/acid_parent.html.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/html/aside.html.mako
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/html/scope_storage_test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/acid/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/js/acid.js
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/js/acid_parent.js
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/js/acid_update_status.js
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/acid/static/js/jquery.ajaxq-0.0.1.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.917491 acid-xblock-0.3.0/acid_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-20 15:16:54.000000 acid-xblock-0.3.0/acid_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:16:54.913491 acid-xblock-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 15:16:54.917491 acid-xblock-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-20 15:16:47.000000 acid-xblock-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.517804 acid-xblock-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-05 14:38:47.517804 acid-xblock-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/acid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/public/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/public/test_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/css/acid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/html/acid.html.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/html/acid_parent.html.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/html/aside.html.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/html/scope_storage_test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.513804 acid-xblock-0.3.1/acid/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/js/acid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/js/acid_parent.js
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/js/acid_update_status.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/acid/static/js/jquery.ajaxq-0.0.1.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.517804 acid-xblock-0.3.1/acid_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 14:38:47.000000 acid-xblock-0.3.1/acid_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:38:47.517804 acid-xblock-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:38:47.517804 acid-xblock-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-05 14:38:44.000000 acid-xblock-0.3.1/setup.py
```

### Comparing `acid-xblock-0.3.0/LICENSE.TXT` & `acid-xblock-0.3.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/PKG-INFO` & `acid-xblock-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: acid-xblock
-Version: 0.3.0
+Version: 0.3.1
 Summary: Acid XBlock Test
 Home-page: https://github.com/openedx/acid-block
 Author: edX
 Author-email: oscm@edx.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 License-File: AUTHORS
 Requires-Dist: Mako
 Requires-Dist: XBlock
 Requires-Dist: lazy
```

### Comparing `acid-xblock-0.3.0/acid/acid.py` & `acid-xblock-0.3.1/acid/acid.py`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/css/acid.css` & `acid-xblock-0.3.1/acid/static/css/acid.css`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/html/acid.html.mako` & `acid-xblock-0.3.1/acid/static/html/acid.html.mako`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/html/acid_parent.html.mako` & `acid-xblock-0.3.1/acid/static/html/acid_parent.html.mako`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/html/aside.html.mako` & `acid-xblock-0.3.1/acid/static/html/aside.html.mako`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/html/scope_storage_test.html` & `acid-xblock-0.3.1/acid/static/html/scope_storage_test.html`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/js/acid.js` & `acid-xblock-0.3.1/acid/static/js/acid.js`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/js/acid_parent.js` & `acid-xblock-0.3.1/acid/static/js/acid_parent.js`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/js/acid_update_status.js` & `acid-xblock-0.3.1/acid/static/js/acid_update_status.js`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid/static/js/jquery.ajaxq-0.0.1.js` & `acid-xblock-0.3.1/acid/static/js/jquery.ajaxq-0.0.1.js`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/acid_xblock.egg-info/PKG-INFO` & `acid-xblock-0.3.1/acid_xblock.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: acid-xblock
-Version: 0.3.0
+Version: 0.3.1
 Summary: Acid XBlock Test
 Home-page: https://github.com/openedx/acid-block
 Author: edX
 Author-email: oscm@edx.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 License-File: AUTHORS
 Requires-Dist: Mako
 Requires-Dist: XBlock
 Requires-Dist: lazy
```

### Comparing `acid-xblock-0.3.0/acid_xblock.egg-info/SOURCES.txt` & `acid-xblock-0.3.1/acid_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acid-xblock-0.3.0/setup.py` & `acid-xblock-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,9 +127,10 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
     ]
 )
```

