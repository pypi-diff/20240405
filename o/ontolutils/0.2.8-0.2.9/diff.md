# Comparing `tmp/ontolutils-0.2.8.tar.gz` & `tmp/ontolutils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontolutils-0.2.8.tar", last modified: Thu Mar 21 13:58:02 2024, max compression
+gzip compressed data, was "ontolutils-0.2.9.tar", last modified: Fri Mar 22 08:50:35 2024, max compression
```

## Comparing `ontolutils-0.2.8.tar` & `ontolutils-0.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.265902 ontolutils-0.2.8/
--rw-rw-rw-   0        0        0     1092 2024-03-04 06:55:20.000000 ontolutils-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     3420 2024-03-21 13:58:02.264902 ontolutils-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2024-03-18 16:52:24.000000 ontolutils-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.112280 ontolutils-0.2.8/ontolutils/
--rw-rw-rw-   0        0        0     1017 2024-03-16 13:17:02.000000 ontolutils-0.2.8/ontolutils/__init__.py
--rw-rw-rw-   0        0        0      316 2024-03-16 13:17:02.000000 ontolutils-0.2.8/ontolutils/_version.py
--rw-rw-rw-   0        0        0      317 2024-03-16 13:16:43.000000 ontolutils-0.2.8/ontolutils/cache.py
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.147348 ontolutils-0.2.8/ontolutils/classes/
--rw-rw-rw-   0        0        0      222 2024-03-16 13:17:02.000000 ontolutils-0.2.8/ontolutils/classes/__init__.py
--rw-rw-rw-   0        0        0     2514 2024-03-17 15:34:44.000000 ontolutils-0.2.8/ontolutils/classes/decorator.py
--rw-rw-rw-   0        0        0     9921 2024-03-16 15:23:29.000000 ontolutils-0.2.8/ontolutils/classes/query_util.py
--rw-rw-rw-   0        0        0    11753 2024-03-20 22:24:31.000000 ontolutils-0.2.8/ontolutils/classes/thing.py
--rw-rw-rw-   0        0        0      463 2024-03-16 13:17:02.000000 ontolutils-0.2.8/ontolutils/classes/typing.py
--rw-rw-rw-   0        0        0     4554 2024-03-16 15:06:37.000000 ontolutils-0.2.8/ontolutils/classes/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.233386 ontolutils-0.2.8/ontolutils/namespacelib/
--rw-rw-rw-   0        0        0    12061 2024-03-21 12:54:10.000000 ontolutils-0.2.8/ontolutils/namespacelib/__dev.py
--rw-rw-rw-   0        0        0      315 2024-03-21 13:56:35.000000 ontolutils-0.2.8/ontolutils/namespacelib/__init__.py
--rw-rw-rw-   0        0        0     3420 2024-03-16 13:17:02.000000 ontolutils-0.2.8/ontolutils/namespacelib/_iana_utils.py
--rw-rw-rw-   0        0        0     1485 2024-03-02 12:35:43.000000 ontolutils-0.2.8/ontolutils/namespacelib/codemeta.py
--rw-rw-rw-   0        0        0    12857 2024-03-02 12:33:42.000000 ontolutils-0.2.8/ontolutils/namespacelib/m4i.py
--rw-rw-rw-   0        0        0     2907 2024-03-02 12:33:47.000000 ontolutils-0.2.8/ontolutils/namespacelib/obo.py
--rw-rw-rw-   0        0        0    13156 2024-03-21 13:56:33.000000 ontolutils-0.2.8/ontolutils/namespacelib/pivmeta.py
--rw-rw-rw-   0        0        0  1979534 2024-03-20 19:47:35.000000 ontolutils-0.2.8/ontolutils/namespacelib/qudt_kind.py
--rw-rw-rw-   0        0        0  2428299 2024-03-02 12:35:12.000000 ontolutils-0.2.8/ontolutils/namespacelib/qudt_unit.py
--rw-rw-rw-   0        0        0  1085598 2024-03-20 19:45:41.000000 ontolutils-0.2.8/ontolutils/namespacelib/schema.py
--rw-rw-rw-   0        0        0     1394 2024-03-02 12:35:55.000000 ontolutils-0.2.8/ontolutils/namespacelib/ssno.py
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.261915 ontolutils-0.2.8/ontolutils.egg-info/
--rw-rw-rw-   0        0        0     3420 2024-03-21 13:58:02.000000 ontolutils-0.2.8/ontolutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-03-21 13:58:02.000000 ontolutils-0.2.8/ontolutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 13:58:02.000000 ontolutils-0.2.8/ontolutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-03-21 13:58:02.000000 ontolutils-0.2.8/ontolutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 13:58:02.000000 ontolutils-0.2.8/ontolutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2024-03-01 12:34:13.000000 ontolutils-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0     1023 2024-03-21 13:58:02.266903 ontolutils-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-03-05 08:21:25.000000 ontolutils-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 13:58:02.258903 ontolutils-0.2.8/tests/
--rw-rw-rw-   0        0        0    11066 2024-03-20 22:35:11.000000 ontolutils-0.2.8/tests/test_classes.py
--rw-rw-rw-   0        0        0     1194 2024-03-16 13:17:02.000000 ontolutils-0.2.8/tests/test_decorator.py
--rw-rw-rw-   0        0        0     4719 2024-03-20 19:48:41.000000 ontolutils-0.2.8/tests/test_namespaces.py
--rw-rw-rw-   0        0        0     7346 2024-03-19 14:43:53.000000 ontolutils-0.2.8/tests/test_query.py
--rw-rw-rw-   0        0        0      961 2024-03-16 13:16:43.000000 ontolutils-0.2.8/tests/test_readme.py
--rw-rw-rw-   0        0        0      558 2024-03-16 13:16:43.000000 ontolutils-0.2.8/tests/test_typing.py
--rw-rw-rw-   0        0        0     1925 2024-03-16 15:07:19.000000 ontolutils-0.2.8/tests/test_utils.py
--rw-rw-rw-   0        0        0      999 2024-03-04 10:26:17.000000 ontolutils-0.2.8/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:35.102445 ontolutils-0.2.9/
+-rw-rw-rw-   0        0        0     1092 2024-03-04 06:55:20.000000 ontolutils-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     3420 2024-03-22 08:50:35.101464 ontolutils-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2024-03-18 16:52:24.000000 ontolutils-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:34.945537 ontolutils-0.2.9/ontolutils/
+-rw-rw-rw-   0        0        0     1125 2024-03-22 08:10:45.000000 ontolutils-0.2.9/ontolutils/__init__.py
+-rw-rw-rw-   0        0        0      316 2024-03-16 13:17:02.000000 ontolutils-0.2.9/ontolutils/_version.py
+-rw-rw-rw-   0        0        0      317 2024-03-16 13:16:43.000000 ontolutils-0.2.9/ontolutils/cache.py
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:34.972537 ontolutils-0.2.9/ontolutils/classes/
+-rw-rw-rw-   0        0        0      284 2024-03-22 08:10:02.000000 ontolutils-0.2.9/ontolutils/classes/__init__.py
+-rw-rw-rw-   0        0        0     2516 2024-03-22 08:08:49.000000 ontolutils-0.2.9/ontolutils/classes/decorator.py
+-rw-rw-rw-   0        0        0     9921 2024-03-16 15:23:29.000000 ontolutils-0.2.9/ontolutils/classes/query_util.py
+-rw-rw-rw-   0        0        0    17946 2024-03-22 08:46:27.000000 ontolutils-0.2.9/ontolutils/classes/thing.py
+-rw-rw-rw-   0        0        0      463 2024-03-16 13:17:02.000000 ontolutils-0.2.9/ontolutils/classes/typing.py
+-rw-rw-rw-   0        0        0     4554 2024-03-16 15:06:37.000000 ontolutils-0.2.9/ontolutils/classes/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:35.013636 ontolutils-0.2.9/ontolutils/namespacelib/
+-rw-rw-rw-   0        0        0    12061 2024-03-21 12:54:10.000000 ontolutils-0.2.9/ontolutils/namespacelib/__dev.py
+-rw-rw-rw-   0        0        0      315 2024-03-21 13:56:35.000000 ontolutils-0.2.9/ontolutils/namespacelib/__init__.py
+-rw-rw-rw-   0        0        0     3420 2024-03-16 13:17:02.000000 ontolutils-0.2.9/ontolutils/namespacelib/_iana_utils.py
+-rw-rw-rw-   0        0        0     1485 2024-03-02 12:35:43.000000 ontolutils-0.2.9/ontolutils/namespacelib/codemeta.py
+-rw-rw-rw-   0        0        0    12857 2024-03-02 12:33:42.000000 ontolutils-0.2.9/ontolutils/namespacelib/m4i.py
+-rw-rw-rw-   0        0        0     2907 2024-03-02 12:33:47.000000 ontolutils-0.2.9/ontolutils/namespacelib/obo.py
+-rw-rw-rw-   0        0        0    13156 2024-03-21 13:56:33.000000 ontolutils-0.2.9/ontolutils/namespacelib/pivmeta.py
+-rw-rw-rw-   0        0        0  1979534 2024-03-20 19:47:35.000000 ontolutils-0.2.9/ontolutils/namespacelib/qudt_kind.py
+-rw-rw-rw-   0        0        0  2428299 2024-03-02 12:35:12.000000 ontolutils-0.2.9/ontolutils/namespacelib/qudt_unit.py
+-rw-rw-rw-   0        0        0  1085598 2024-03-20 19:45:41.000000 ontolutils-0.2.9/ontolutils/namespacelib/schema.py
+-rw-rw-rw-   0        0        0     1394 2024-03-02 12:35:55.000000 ontolutils-0.2.9/ontolutils/namespacelib/ssno.py
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:35.098433 ontolutils-0.2.9/ontolutils.egg-info/
+-rw-rw-rw-   0        0        0     3420 2024-03-22 08:50:34.000000 ontolutils-0.2.9/ontolutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-03-22 08:50:34.000000 ontolutils-0.2.9/ontolutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-22 08:50:34.000000 ontolutils-0.2.9/ontolutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-03-22 08:50:34.000000 ontolutils-0.2.9/ontolutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-22 08:50:34.000000 ontolutils-0.2.9/ontolutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2024-03-01 12:34:13.000000 ontolutils-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1023 2024-03-22 08:50:35.103444 ontolutils-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-03-05 08:21:25.000000 ontolutils-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-22 08:50:35.096335 ontolutils-0.2.9/tests/
+-rw-rw-rw-   0        0        0    12731 2024-03-22 08:14:32.000000 ontolutils-0.2.9/tests/test_classes.py
+-rw-rw-rw-   0        0        0     1194 2024-03-16 13:17:02.000000 ontolutils-0.2.9/tests/test_decorator.py
+-rw-rw-rw-   0        0        0     4719 2024-03-20 19:48:41.000000 ontolutils-0.2.9/tests/test_namespaces.py
+-rw-rw-rw-   0        0        0     7346 2024-03-19 14:43:53.000000 ontolutils-0.2.9/tests/test_query.py
+-rw-rw-rw-   0        0        0     1313 2024-03-22 08:42:34.000000 ontolutils-0.2.9/tests/test_readme.py
+-rw-rw-rw-   0        0        0      558 2024-03-16 13:16:43.000000 ontolutils-0.2.9/tests/test_typing.py
+-rw-rw-rw-   0        0        0     1925 2024-03-16 15:07:19.000000 ontolutils-0.2.9/tests/test_utils.py
+-rw-rw-rw-   0        0        0      999 2024-03-04 10:26:17.000000 ontolutils-0.2.9/tests/test_version.py
```

### Comparing `ontolutils-0.2.8/LICENSE` & `ontolutils-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/PKG-INFO` & `ontolutils-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolutils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utility library for the work with ontologies.
 Home-page: https://github.com/matthiasprobst/ontology-utils
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ontolutils-0.2.8/README.md` & `ontolutils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/__init__.py` & `ontolutils-0.2.9/ontolutils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Ontolutils package."""
 import logging
 
 from ._version import __version__
-from .classes import Thing
+from .classes import Thing, get_urirefs, get_namespaces
 from .classes import namespaces, urirefs
 from .classes import query, dquery
 from .classes.utils import merge_jsonld
 from .namespacelib import *
 
 DEFAULT_LOGGING_LEVEL = logging.WARNING
 _formatter = logging.Formatter(
@@ -31,8 +31,11 @@
 __all__ = ['Thing',
            '__version__',
            'namespaces',
            'urirefs',
            'query',
            'set_logging_level',
            'merge_jsonld',
+           'dquery',
+           'get_urirefs',
+           'get_namespaces',
            ]
```

### Comparing `ontolutils-0.2.8/ontolutils/classes/decorator.py` & `ontolutils-0.2.9/ontolutils/classes/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,7 +91,8 @@
                 NamespaceManager[cls][k] = str(ns)
             if k not in fields:
                 raise KeyError(f"Field '{k}' not found in {cls.__name__}")
             URIRefManager[cls][k] = str(v)
         return cls
 
     return _decorator
+
```

### Comparing `ontolutils-0.2.8/ontolutils/classes/query_util.py` & `ontolutils-0.2.9/ontolutils/classes/query_util.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/classes/utils.py` & `ontolutils-0.2.9/ontolutils/classes/utils.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/__dev.py` & `ontolutils-0.2.9/ontolutils/namespacelib/__dev.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/_iana_utils.py` & `ontolutils-0.2.9/ontolutils/namespacelib/_iana_utils.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/codemeta.py` & `ontolutils-0.2.9/ontolutils/namespacelib/codemeta.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/m4i.py` & `ontolutils-0.2.9/ontolutils/namespacelib/m4i.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/obo.py` & `ontolutils-0.2.9/ontolutils/namespacelib/obo.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/pivmeta.py` & `ontolutils-0.2.9/ontolutils/namespacelib/pivmeta.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/qudt_kind.py` & `ontolutils-0.2.9/ontolutils/namespacelib/qudt_kind.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/qudt_unit.py` & `ontolutils-0.2.9/ontolutils/namespacelib/qudt_unit.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/schema.py` & `ontolutils-0.2.9/ontolutils/namespacelib/schema.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils/namespacelib/ssno.py` & `ontolutils-0.2.9/ontolutils/namespacelib/ssno.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/ontolutils.egg-info/PKG-INFO` & `ontolutils-0.2.9/ontolutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolutils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utility library for the work with ontologies.
 Home-page: https://github.com/matthiasprobst/ontology-utils
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ontolutils-0.2.8/ontolutils.egg-info/SOURCES.txt` & `ontolutils-0.2.9/ontolutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/setup.cfg` & `ontolutils-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6e74 6f6c 7574 696c 730d 0a76   = ontolutils..v
-00000020: 6572 7369 6f6e 203d 2030 2e32 2e38 0d0a  ersion = 0.2.8..
+00000020: 6572 7369 6f6e 203d 2030 2e32 2e39 0d0a  ersion = 0.2.9..
 00000030: 6175 7468 6f72 203d 204d 6174 7468 6961  author = Matthia
 00000040: 7320 5072 6f62 7374 0d0a 6175 7468 6f72  s Probst..author
 00000050: 5f65 6d61 696c 203d 206d 6174 7468 6961  _email = matthia
 00000060: 732e 7072 6f62 7374 406b 6974 2e65 6475  s.probst@kit.edu
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5574 696c 6974 7920 6c69 6272 6172 7920  Utility library 
 00000090: 666f 7220 7468 6520 776f 726b 2077 6974  for the work wit
```

### Comparing `ontolutils-0.2.8/tests/test_classes.py` & `ontolutils-0.2.9/tests/test_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 import json
 import logging
 import pydantic
 import unittest
 from pydantic import EmailStr
 
-from ontolutils import Thing, urirefs, namespaces
+from ontolutils import Thing, urirefs, namespaces, get_urirefs, get_namespaces
 from ontolutils import set_logging_level
 from ontolutils.classes import decorator
 
 LOG_LEVEL = logging.DEBUG
 
 
 class TestNamespaces(unittest.TestCase):
 
     def setUp(self):
+        self.maxDiff = None
         logger = logging.getLogger('ontolutils')
         self.INITIAL_LOG_LEVEL = logger.level
 
         set_logging_level(LOG_LEVEL)
 
         assert logger.level == LOG_LEVEL
 
     def tearDown(self):
         set_logging_level(self.INITIAL_LOG_LEVEL)
         assert logging.getLogger('ontolutils').level == self.INITIAL_LOG_LEVEL
 
+    def test_thing_custom_prop(self):
+        """It is helpful to have the properties equal to the urirefs keys,
+        however, this should not be required!"""
+
+        @namespaces(foaf='http://xmlns.com/foaf/0.1/',
+                    prov='http://www.w3.org/ns/prov#')
+        @urirefs(Person='prov:Person',
+                 first_name='foaf:firstName',
+                 lastName='foaf:lastName')
+        class Person(Thing):
+            first_name: str = None
+            lastName: str
+
+        p = Person(first_name='John', lastName='Doe')
+        print(p.model_dump_jsonld(resolve_keys=False))
+
     def test_sort_classes(self):
         thing1 = Thing(label='Thing 1')
         thing2 = Thing(label='Thing 2')
         self.assertFalse(thing1 < thing2)
         with self.assertRaises(TypeError):
             thing1 < 4
         thing1 = Thing(label='Thing 1', id='http://example.com/thing1')
@@ -251,35 +268,55 @@
                              jsonld)
 
     def test_update_namespace_and_uri(self):
         class CustomPerson(Thing):
             pass
 
         mt = CustomPerson()
-        print(mt.get_context())
-        print(mt.namespaces)
-        print(mt.urirefs)
+        # custom person has no
+        self.assertDictEqual(mt.urirefs, get_urirefs(Thing))
+        self.assertDictEqual(mt.urirefs, {'Thing': 'owl:Thing', 'label': 'rdfs:label'})
+        self.assertDictEqual(mt.namespaces, get_namespaces(Thing))
+        self.assertDictEqual(mt.namespaces, {'owl': 'http://www.w3.org/2002/07/owl#',
+                                             'rdfs': 'http://www.w3.org/2000/01/rdf-schema#'})
 
         mt = CustomPerson(first_name='John', last_name='Doe')
         with self.assertRaises(AttributeError):
             mt.namespaces = 'http://xmlns.com/foaf/0.1/'
         with self.assertRaises(AttributeError):
             mt.urirefs = 'foaf:lastName'
+
         mt.namespaces['foaf'] = 'http://xmlns.com/foaf/0.1/'
         mt.urirefs['first_name'] = 'foaf:firstName'
         mt.urirefs['last_name'] = 'foaf:lastName'
         # print(mt.model_dump_json(indent=2, exclude_none=True))
         ref_jsonld = {
             "@context": {
                 "owl": "http://www.w3.org/2002/07/owl#",
                 "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
                 "foaf": "http://xmlns.com/foaf/0.1/"
             },
             "@type": "CustomPerson",
             "foaf:firstName": "John",
-            "foaf:lastName": "Doe",
-            # "@id": "local:30d80c1d-d470-4602-87d5-75390ee295fd"
+            "foaf:lastName": "Doe"
+        }
+        jsonld_dict = json.loads(mt.model_dump_jsonld(resolve_keys=True))
+        jsonld_dict.pop('@id')
+        self.assertDictEqual(jsonld_dict,
+                             ref_jsonld)
+
+        ref_jsonld = {
+            "@context": {
+                "owl": "http://www.w3.org/2002/07/owl#",
+                "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+                "foaf": "http://xmlns.com/foaf/0.1/",
+                "first_name": "http://xmlns.com/foaf/0.1/firstName",
+                "last_name": "http://xmlns.com/foaf/0.1/lastName"
+            },
+            "@type": "CustomPerson",
+            "first_name": "John",
+            "last_name": "Doe"
         }
-        jsonld_dict = json.loads(mt.model_dump_jsonld())
+        jsonld_dict = json.loads(mt.model_dump_jsonld(resolve_keys=False))
         jsonld_dict.pop('@id')
         self.assertDictEqual(jsonld_dict,
                              ref_jsonld)
```

### Comparing `ontolutils-0.2.8/tests/test_decorator.py` & `ontolutils-0.2.9/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/tests/test_namespaces.py` & `ontolutils-0.2.9/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/tests/test_query.py` & `ontolutils-0.2.9/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/tests/test_readme.py` & `ontolutils-0.2.9/tests/test_readme.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Testing code used in the README.md file"""
 import pathlib
-
 from pydantic import EmailStr
 
 from ontolutils import Thing, namespaces, urirefs
 
 
 @namespaces(prov="http://www.w3.org/ns/prov#",
             foaf="http://xmlns.com/foaf/0.1/")
@@ -34,7 +33,21 @@
 #     found_agents = Agent.from_jsonld(data=f.read())
 
 found_agents = Agent.from_jsonld(source="agent.json")
 found_agent = found_agents[0]
 print(found_agent.mbox)
 
 pathlib.Path("agent.json").unlink(missing_ok=True)
+
+
+@namespaces(prov='http://www.w3.org/ns/prov#',
+
+            foaf='http://xmlns.com/foaf/0.1/')
+@urirefs(Person='prov:Person', first_name='foaf:firstName')
+class Person(Thing):
+    first_name: str = None
+    last_name: str = None
+
+p = Person(first_name='John', last_name='Doe', age=30)
+print(p.model_dump_jsonld())
+
+# Person(first_name=1)
```

### Comparing `ontolutils-0.2.8/tests/test_typing.py` & `ontolutils-0.2.9/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/tests/test_utils.py` & `ontolutils-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ontolutils-0.2.8/tests/test_version.py` & `ontolutils-0.2.9/tests/test_version.py`

 * *Files identical despite different names*

