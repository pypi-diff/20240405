# Comparing `tmp/serializable-0.4.0.tar.gz` & `tmp/serializable-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializable-0.4.0.tar", last modified: Tue Feb  6 06:12:51 2024, max compression
+gzip compressed data, was "serializable-0.4.1.tar", last modified: Fri Apr  5 19:58:27 2024, max compression
```

## Comparing `serializable-0.4.0.tar` & `serializable-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-02-06 06:12:51.492527 serializable-0.4.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2022-04-18 20:09:03.000000 serializable-0.4.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2113 2024-02-06 06:12:51.492102 serializable-0.4.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1461 2024-01-31 03:44:27.000000 serializable-0.4.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-02-06 06:12:51.479411 serializable-0.4.0/serializable/
--rw-r--r--   0 iskander   (501) staff       (20)      868 2024-02-06 06:12:15.000000 serializable-0.4.0/serializable/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)    10307 2024-01-30 17:36:43.000000 serializable-0.4.0/serializable/helpers.py
--rw-r--r--   0 iskander   (501) staff       (20)     1099 2024-01-30 17:36:35.000000 serializable-0.4.0/serializable/primitive_types.py
--rw-r--r--   0 iskander   (501) staff       (20)     4785 2024-01-30 17:32:35.000000 serializable-0.4.0/serializable/serializable.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-02-06 06:12:51.491768 serializable-0.4.0/serializable.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2113 2024-02-06 06:12:51.000000 serializable-0.4.0/serializable.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      570 2024-02-06 06:12:51.000000 serializable-0.4.0/serializable.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2024-02-06 06:12:51.000000 serializable-0.4.0/serializable.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)       29 2024-02-06 06:12:51.000000 serializable-0.4.0/serializable.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)       13 2024-02-06 06:12:51.000000 serializable-0.4.0/serializable.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2024-02-06 06:12:51.492664 serializable-0.4.0/setup.cfg
--rw-r--r--   0 iskander   (501) staff       (20)     2035 2024-01-30 17:32:22.000000 serializable-0.4.0/setup.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-02-06 06:12:51.491503 serializable-0.4.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      957 2024-01-30 17:35:28.000000 serializable-0.4.0/tests/test_class.py
--rw-r--r--   0 iskander   (501) staff       (20)      798 2024-01-30 17:35:26.000000 serializable-0.4.0/tests/test_default_to_dict_implementation.py
--rw-r--r--   0 iskander   (501) staff       (20)      980 2024-01-30 17:35:23.000000 serializable-0.4.0/tests/test_function.py
--rw-r--r--   0 iskander   (501) staff       (20)     2830 2024-01-30 17:35:19.000000 serializable-0.4.0/tests/test_keyword_aliases.py
--rw-r--r--   0 iskander   (501) staff       (20)      828 2024-01-30 17:35:16.000000 serializable-0.4.0/tests/test_namedtuple.py
--rw-r--r--   0 iskander   (501) staff       (20)     1079 2024-01-30 17:34:58.000000 serializable-0.4.0/tests/test_nesting.py
--rw-r--r--   0 iskander   (501) staff       (20)     1202 2024-01-30 17:35:07.000000 serializable-0.4.0/tests/test_object.py
--rw-r--r--   0 iskander   (501) staff       (20)      990 2024-01-30 17:35:59.000000 serializable-0.4.0/tests/test_primitive_values.py
--rw-r--r--   0 iskander   (501) staff       (20)      890 2024-01-30 17:35:57.000000 serializable-0.4.0/tests/test_set.py
--rw-r--r--   0 iskander   (501) staff       (20)      890 2024-01-30 17:35:53.000000 serializable-0.4.0/tests/test_tuple.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-04-05 19:58:27.906423 serializable-0.4.1/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2022-04-18 20:09:03.000000 serializable-0.4.1/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2224 2024-04-05 19:58:27.906208 serializable-0.4.1/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1572 2024-02-06 06:16:22.000000 serializable-0.4.1/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-04-05 19:58:27.895886 serializable-0.4.1/serializable/
+-rw-r--r--   0 iskander   (501) staff       (20)      868 2024-04-05 19:58:03.000000 serializable-0.4.1/serializable/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)    10307 2024-01-30 17:36:43.000000 serializable-0.4.1/serializable/helpers.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1099 2024-01-30 17:36:35.000000 serializable-0.4.1/serializable/primitive_types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4785 2024-01-30 17:32:35.000000 serializable-0.4.1/serializable/serializable.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-04-05 19:58:27.905926 serializable-0.4.1/serializable.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2224 2024-04-05 19:58:27.000000 serializable-0.4.1/serializable.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      570 2024-04-05 19:58:27.000000 serializable-0.4.1/serializable.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2024-04-05 19:58:27.000000 serializable-0.4.1/serializable.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       29 2024-04-05 19:58:27.000000 serializable-0.4.1/serializable.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       13 2024-04-05 19:58:27.000000 serializable-0.4.1/serializable.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2024-04-05 19:58:27.906467 serializable-0.4.1/setup.cfg
+-rw-r--r--   0 iskander   (501) staff       (20)     2035 2024-01-30 17:32:22.000000 serializable-0.4.1/setup.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-04-05 19:58:27.905660 serializable-0.4.1/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      957 2024-01-30 17:35:28.000000 serializable-0.4.1/tests/test_class.py
+-rw-r--r--   0 iskander   (501) staff       (20)      798 2024-01-30 17:35:26.000000 serializable-0.4.1/tests/test_default_to_dict_implementation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      980 2024-01-30 17:35:23.000000 serializable-0.4.1/tests/test_function.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2830 2024-01-30 17:35:19.000000 serializable-0.4.1/tests/test_keyword_aliases.py
+-rw-r--r--   0 iskander   (501) staff       (20)      828 2024-01-30 17:35:16.000000 serializable-0.4.1/tests/test_namedtuple.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1079 2024-01-30 17:34:58.000000 serializable-0.4.1/tests/test_nesting.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1202 2024-01-30 17:35:07.000000 serializable-0.4.1/tests/test_object.py
+-rw-r--r--   0 iskander   (501) staff       (20)      990 2024-01-30 17:35:59.000000 serializable-0.4.1/tests/test_primitive_values.py
+-rw-r--r--   0 iskander   (501) staff       (20)      890 2024-01-30 17:35:57.000000 serializable-0.4.1/tests/test_set.py
+-rw-r--r--   0 iskander   (501) staff       (20)      890 2024-01-30 17:35:53.000000 serializable-0.4.1/tests/test_tuple.py
```

### Comparing `serializable-0.4.0/LICENSE` & `serializable-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/PKG-INFO` & `serializable-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializable
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base class with serialization helpers for user-defined Python objects
 Home-page: https://github.com/iskandr/serializable
 Author: Alex Rubinsteyn
 Author-email: alex@openvax.org
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -14,16 +14,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typechecks>=0.0.2
 Requires-Dist: simplejson
 
 [![Tests](https://github.com/openvax/serializable/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/serializable/actions/workflows/tests.yml)
 <a href="https://pypi.python.org/pypi/serializable/">
-    <img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
+<img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
 </a>
+[![PyPI downloads](https://img.shields.io/pypi/dm/serializable.svg)](https://pypistats.org/packages/serializable)
+
 # serializable
 
 Base class with serialization methods for user-defined Python objects
 
 ## Usage
 
 Classes which inherit from `Serializable` are enabled with default implementations of
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: serializable Version: 0.4.0 Summary: Base class
+Metadata-Version: 2.1 Name: serializable Version: 0.4.1 Summary: Base class
 with serialization helpers for user-defined Python objects Home-page: https://
 github.com/iskandr/serializable Author: Alex Rubinsteyn Author-email:
 alex@openvax.org License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 typechecks>=0.0.2 Requires-Dist: simplejson [![Tests](https://github.com/
 openvax/serializable/actions/workflows/tests.yml/badge.svg)](https://
-github.com/openvax/serializable/actions/workflows/tests.yml) _[_P_y_P_I_]#
-serializable Base class with serialization methods for user-defined Python
-objects ## Usage Classes which inherit from `Serializable` are enabled with
-default implementations of `to_json`, `from_json`, `__reduce__` (for pickling),
-and other serialization helpers. A derived class must either: - have a member
-data matching the name of each argument to `__init__` - provide a user-defined
-`to_dict()` method which returns a dictionary whose keys match the arguments to
-`__init__` If you change the keyword arguments to a class which derives from
-`Serializable` but would like to be able to deserialize older JSON
-representations then you can define a class-level dictionary called
-`_KEYWORD_ALIASES` which maps old keywords to new names (or `None` if a keyword
-was removed). ## Limitations - Serializable objects must inherit from
-`Serializable`, be tuples or namedtuples, be serializble primitive types such
-as dict, list, int, float, or str. - The serialized representation of objects
-relies on reserved keywords (such as `"__name__"`, and `"__class__"`), so
-dictionaries are expected to not contain any keys which begin with two
-underscores.
+github.com/openvax/serializable/actions/workflows/tests.yml) _[_P_y_P_I_][![PyPI
+downloads](https://img.shields.io/pypi/dm/serializable.svg)](https://
+pypistats.org/packages/serializable) # serializable Base class with
+serialization methods for user-defined Python objects ## Usage Classes which
+inherit from `Serializable` are enabled with default implementations of
+`to_json`, `from_json`, `__reduce__` (for pickling), and other serialization
+helpers. A derived class must either: - have a member data matching the name of
+each argument to `__init__` - provide a user-defined `to_dict()` method which
+returns a dictionary whose keys match the arguments to `__init__` If you change
+the keyword arguments to a class which derives from `Serializable` but would
+like to be able to deserialize older JSON representations then you can define a
+class-level dictionary called `_KEYWORD_ALIASES` which maps old keywords to new
+names (or `None` if a keyword was removed). ## Limitations - Serializable
+objects must inherit from `Serializable`, be tuples or namedtuples, be
+serializble primitive types such as dict, list, int, float, or str. - The
+serialized representation of objects relies on reserved keywords (such as
+`"__name__"`, and `"__class__"`), so dictionaries are expected to not contain
+any keys which begin with two underscores.
```

### Comparing `serializable-0.4.0/README.md` & `serializable-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [![Tests](https://github.com/openvax/serializable/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/serializable/actions/workflows/tests.yml)
 <a href="https://pypi.python.org/pypi/serializable/">
-    <img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
+<img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
 </a>
+[![PyPI downloads](https://img.shields.io/pypi/dm/serializable.svg)](https://pypistats.org/packages/serializable)
+
 # serializable
 
 Base class with serialization methods for user-defined Python objects
 
 ## Usage
 
 Classes which inherit from `Serializable` are enabled with default implementations of
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
 [![Tests](https://github.com/openvax/serializable/actions/workflows/tests.yml/
 badge.svg)](https://github.com/openvax/serializable/actions/workflows/
-tests.yml) _[_P_y_P_I_]# serializable Base class with serialization methods for user-
-defined Python objects ## Usage Classes which inherit from `Serializable` are
-enabled with default implementations of `to_json`, `from_json`, `__reduce__`
-(for pickling), and other serialization helpers. A derived class must either: -
-have a member data matching the name of each argument to `__init__` - provide a
-user-defined `to_dict()` method which returns a dictionary whose keys match the
-arguments to `__init__` If you change the keyword arguments to a class which
-derives from `Serializable` but would like to be able to deserialize older JSON
+tests.yml) _[_P_y_P_I_][![PyPI downloads](https://img.shields.io/pypi/dm/
+serializable.svg)](https://pypistats.org/packages/serializable) # serializable
+Base class with serialization methods for user-defined Python objects ## Usage
+Classes which inherit from `Serializable` are enabled with default
+implementations of `to_json`, `from_json`, `__reduce__` (for pickling), and
+other serialization helpers. A derived class must either: - have a member data
+matching the name of each argument to `__init__` - provide a user-defined
+`to_dict()` method which returns a dictionary whose keys match the arguments to
+`__init__` If you change the keyword arguments to a class which derives from
+`Serializable` but would like to be able to deserialize older JSON
 representations then you can define a class-level dictionary called
 `_KEYWORD_ALIASES` which maps old keywords to new names (or `None` if a keyword
 was removed). ## Limitations - Serializable objects must inherit from
 `Serializable`, be tuples or namedtuples, be serializble primitive types such
 as dict, list, int, float, or str. - The serialized representation of objects
 relies on reserved keywords (such as `"__name__"`, and `"__class__"`), so
 dictionaries are expected to not contain any keys which begin with two
```

### Comparing `serializable-0.4.0/serializable/__init__.py` & `serializable-0.4.1/serializable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     to_serializable_repr,
     from_serializable_repr,
     to_json,
     from_json,
     to_dict,
 )
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 __all__ = [
     "Serializable",
     "to_serializable_repr",
     "from_serializable_repr",
     "to_json",
     "from_json",
```

### Comparing `serializable-0.4.0/serializable/helpers.py` & `serializable-0.4.1/serializable/helpers.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/serializable/primitive_types.py` & `serializable-0.4.1/serializable/primitive_types.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/serializable/serializable.py` & `serializable-0.4.1/serializable/serializable.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/serializable.egg-info/PKG-INFO` & `serializable-0.4.1/serializable.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializable
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base class with serialization helpers for user-defined Python objects
 Home-page: https://github.com/iskandr/serializable
 Author: Alex Rubinsteyn
 Author-email: alex@openvax.org
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -14,16 +14,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typechecks>=0.0.2
 Requires-Dist: simplejson
 
 [![Tests](https://github.com/openvax/serializable/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/serializable/actions/workflows/tests.yml)
 <a href="https://pypi.python.org/pypi/serializable/">
-    <img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
+<img src="https://img.shields.io/pypi/v/serializable.svg?maxAge=1000" alt="PyPI" />
 </a>
+[![PyPI downloads](https://img.shields.io/pypi/dm/serializable.svg)](https://pypistats.org/packages/serializable)
+
 # serializable
 
 Base class with serialization methods for user-defined Python objects
 
 ## Usage
 
 Classes which inherit from `Serializable` are enabled with default implementations of
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: serializable Version: 0.4.0 Summary: Base class
+Metadata-Version: 2.1 Name: serializable Version: 0.4.1 Summary: Base class
 with serialization helpers for user-defined Python objects Home-page: https://
 github.com/iskandr/serializable Author: Alex Rubinsteyn Author-email:
 alex@openvax.org License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 typechecks>=0.0.2 Requires-Dist: simplejson [![Tests](https://github.com/
 openvax/serializable/actions/workflows/tests.yml/badge.svg)](https://
-github.com/openvax/serializable/actions/workflows/tests.yml) _[_P_y_P_I_]#
-serializable Base class with serialization methods for user-defined Python
-objects ## Usage Classes which inherit from `Serializable` are enabled with
-default implementations of `to_json`, `from_json`, `__reduce__` (for pickling),
-and other serialization helpers. A derived class must either: - have a member
-data matching the name of each argument to `__init__` - provide a user-defined
-`to_dict()` method which returns a dictionary whose keys match the arguments to
-`__init__` If you change the keyword arguments to a class which derives from
-`Serializable` but would like to be able to deserialize older JSON
-representations then you can define a class-level dictionary called
-`_KEYWORD_ALIASES` which maps old keywords to new names (or `None` if a keyword
-was removed). ## Limitations - Serializable objects must inherit from
-`Serializable`, be tuples or namedtuples, be serializble primitive types such
-as dict, list, int, float, or str. - The serialized representation of objects
-relies on reserved keywords (such as `"__name__"`, and `"__class__"`), so
-dictionaries are expected to not contain any keys which begin with two
-underscores.
+github.com/openvax/serializable/actions/workflows/tests.yml) _[_P_y_P_I_][![PyPI
+downloads](https://img.shields.io/pypi/dm/serializable.svg)](https://
+pypistats.org/packages/serializable) # serializable Base class with
+serialization methods for user-defined Python objects ## Usage Classes which
+inherit from `Serializable` are enabled with default implementations of
+`to_json`, `from_json`, `__reduce__` (for pickling), and other serialization
+helpers. A derived class must either: - have a member data matching the name of
+each argument to `__init__` - provide a user-defined `to_dict()` method which
+returns a dictionary whose keys match the arguments to `__init__` If you change
+the keyword arguments to a class which derives from `Serializable` but would
+like to be able to deserialize older JSON representations then you can define a
+class-level dictionary called `_KEYWORD_ALIASES` which maps old keywords to new
+names (or `None` if a keyword was removed). ## Limitations - Serializable
+objects must inherit from `Serializable`, be tuples or namedtuples, be
+serializble primitive types such as dict, list, int, float, or str. - The
+serialized representation of objects relies on reserved keywords (such as
+`"__name__"`, and `"__class__"`), so dictionaries are expected to not contain
+any keys which begin with two underscores.
```

### Comparing `serializable-0.4.0/serializable.egg-info/SOURCES.txt` & `serializable-0.4.1/serializable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/setup.py` & `serializable-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_class.py` & `serializable-0.4.1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_default_to_dict_implementation.py` & `serializable-0.4.1/tests/test_default_to_dict_implementation.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_function.py` & `serializable-0.4.1/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_keyword_aliases.py` & `serializable-0.4.1/tests/test_keyword_aliases.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_namedtuple.py` & `serializable-0.4.1/tests/test_namedtuple.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_nesting.py` & `serializable-0.4.1/tests/test_nesting.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_object.py` & `serializable-0.4.1/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_primitive_values.py` & `serializable-0.4.1/tests/test_primitive_values.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_set.py` & `serializable-0.4.1/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `serializable-0.4.0/tests/test_tuple.py` & `serializable-0.4.1/tests/test_tuple.py`

 * *Files identical despite different names*

