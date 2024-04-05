# Comparing `tmp/ftb-snbt-lib-0.1.3.tar.gz` & `tmp/ftb-snbt-lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb-snbt-lib-0.1.3.tar", last modified: Wed Apr  3 05:12:15 2024, max compression
+gzip compressed data, was "ftb-snbt-lib-0.2.1.tar", last modified: Fri Apr  5 14:19:18 2024, max compression
```

## Comparing `ftb-snbt-lib-0.1.3.tar` & `ftb-snbt-lib-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 05:12:15.000000 ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:12:15.922379 ftb-snbt-lib-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 05:12:11.000000 ftb-snbt-lib-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:18.377540 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 14:19:18.000000 ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:19:18.381541 ftb-snbt-lib-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 14:19:11.000000 ftb-snbt-lib-0.2.1/setup.py
```

### Comparing `ftb-snbt-lib-0.1.3/LICENSE` & `ftb-snbt-lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/PKG-INFO` & `ftb-snbt-lib-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.1.3
+Version: 0.2.1
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 
 # ftb-snbt-lib
+
+![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
+
 A python library to parse, edit, and save FTB snbt tag.
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
@@ -107,12 +110,13 @@
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
 * [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
```

### Comparing `ftb-snbt-lib-0.1.3/README.md` & `ftb-snbt-lib-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # ftb-snbt-lib
+
+![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
+
 A python library to parse, edit, and save FTB snbt tag.
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
@@ -90,12 +93,13 @@
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
 * [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
```

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/parse.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     """key_value_pair : NAME COLON value
                       | STRING COLON value"""
     p[0] = (p[1], p[3])
 
 def p_value(p):
     """value : compound
                 | list
+                | array
                 | BOOL
                 | BYTE
                 | SHORT
                 | DOUBLE
                 | LONG
                 | INTEGER
                 | STRING"""
@@ -48,14 +49,22 @@
     """list : LBRACKET values RBRACKET
                 | LBRACKET RBRACKET"""
     if len(p) == 3:
         p[0] = List()
     else:
         p[0] = List(p[2])
 
+def p_array(p):
+    """array : LBRACKET NAME SEMICOLON values RBRACKET
+                | LBRACKET NAME SEMICOLON RBRACKET"""
+    if len(p) == 4:
+        p[0] = Array(p[2], [])
+    else:
+        p[0] = Array(p[2], p[4])
+
 def p_values(p):
     """values : values value
               | values COMMA value
               | value"""
     if len(p) == 2:
         p[0] = [p[1]]
     elif len(p) == 4:
```

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/cpp.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ctokens.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/lex.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/yacc.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/ply/ygen.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/tag.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Short", "Integer", "Long", "Double", "Bool", "String", "List", "Compound"]
+__all__ = ["Base", "Numeric", "NumericInteger", "Byte", "Short", "Integer", "Long", "Double", "Bool", "String", "List", "Array", "Compound"]
 
 class InvalidTypeError(ValueError):
     def __init__(self, item, cls):
         self.item = item
         self.cls = cls
         super().__init__(f"{self.item!r} is not a valid type for the items of {cls.__name__}.\nThis error is likely caused by a type mismatch in a list.")
 
@@ -148,11 +148,79 @@
         if not isinstance(item, cls.subtype):
             try:
                 return cls.subtype(item)
             except Exception as e:
                 raise CastError(item, cls.subtype) from e
             
         return item
+
+class Array(Base, list):
+    __slots__ = ()
+    write_func = "array"
+    subtype = None
+    array_prefix = None
+
+    def __new__(cls, subtype, iterable=()):
+        if cls.subtype is None:
+            cls = cls[subtype]
+        return super().__new__(cls, subtype, iterable)
+    
+    def __init__(self, subtype, iterable=()):
+        super().__init__(map(self.cast_item, iterable))
+
+    def __class_getitem__(cls, subtype):
+        if subtype == "B":
+            return ByteArray
+        if subtype == "I":
+            return IntArray
+        if subtype == "L":
+            return LongArray
+        raise TypeError(f"Array type must be specified with 'B', 'I', or 'L'")
+    
+    def __setitem__(self, index, value):
+        if isinstance(index, int):
+            super().__setitem__(index, self.cast_item(value))
+        elif isinstance(index, slice):
+            super().__setitem__(index, map(self.cast_item, value))
+        else:
+            raise TypeError(f"Array indices must be integers or slices, not {index.__class__.__name__}")
+    
+    def append(self, value):
+        super().append(self.cast_item(value))
+    
+    def extend(self, iterable):
+        super().extend(map(self.cast_item, iterable))
+    
+    def insert(self, index, value):
+        super().insert(index, self.cast_item(value))
+
+    @classmethod
+    def cast_item(cls, item):
+        if cls.subtype is None:
+            raise InvalidTypeError(item, cls)
+        
+        if not isinstance(item, cls.subtype):
+            try:
+                return cls.subtype(item)
+            except Exception as e:
+                raise CastError(item, cls.subtype) from e
+            
+        return item
+
+class ByteArray(Array):
+    __slots__ = ()
+    subtype = Byte
+    array_prefix = "B"
+
+class IntArray(Array):
+    __slots__ = ()
+    subtype = Integer
+    array_prefix = "I"
+
+class LongArray(Array):
+    __slots__ = ()
+    subtype = Long
+    array_prefix = "L"
     
 class Compound(Base, dict):
     __slots__ = ()
     write_func = "compound"
```

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/token.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/token.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "SHORT",
     "DOUBLE",
     "LONG",
     "INTEGER",
     "STRING",
     "NAME",
     "COLON",
+    "SEMICOLON",
     "COMMA",
 )
 
 t_ignore = ' \t\r'
 
 def t_newline(t):
     r'\n'
@@ -83,14 +84,18 @@
     r'[a-zA-Z0-9._+-]+'
     return t
 
 def t_COLON(t):
     r'\:'
     return t
 
+def t_SEMICOLON(t):
+    r'\;'
+    return t
+
 def t_COMMA(t):
     r'\,'
     return t
 
 def t_error(t):
     print(f"Illegal character {t.value[0]!r}")
     t.lexer.skip(1)
```

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib/write.py` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib/write.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,20 +93,20 @@
             prev = self.prev_indent
             self.prev_indent = self.indent
             self.indent += self.indentation
             yield
             self.indent = self.prev_indent
             self.prev_indent = prev
             
-    def should_expand(self, tag: List | Compound) -> bool:
+    def should_expand(self, tag: List | Array | Compound) -> bool:
         return (
             self.indentation is not None
             and (
                 not self.prev_indent
-                or isinstance(tag, (List, Compound))
+                or isinstance(tag, (List, Array, Compound))
             )
         )
 
     def expand(self, fmt: str) -> tuple[str, str]:
         return (
             f"\n{self.indent}",
             fmt.replace("{}", f"\n{self.indent}{{}}\n{self.prev_indent}"),
@@ -133,14 +133,28 @@
 
         if len(tag) == 0:
             return fmt.format(" ")
         if len(tag) == 1:
             return fmt.format(self.write(tag[0]))
         
         with self.depth():
+            if self.should_expand(tag):
+                separator, fmt = self.expand(fmt)
+
+            return fmt.format(separator.join(map(self.write, tag)))
+        
+    def write_array(self, tag: Array) -> str:
+        separator, fmt = "\n", f"[{tag.array_prefix};{{}}]"
+
+        if len(tag) == 0:
+            return fmt.format(" ")
+        if len(tag) == 1:
+            return fmt.format(self.write(tag[0]))
+        
+        with self.depth():
             if self.should_expand(tag):
                 separator, fmt = self.expand(fmt)
 
             return fmt.format(separator.join(map(self.write, tag)))
     
     def write_compound(self, tag: Compound) -> str:
         separator, fmt = "\n", "{{{}}}"
```

### Comparing `ftb-snbt-lib-0.1.3/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb-snbt-lib-0.2.1/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.1.3
+Version: 0.2.1
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 
 # ftb-snbt-lib
+
+![GitHub Release](https://img.shields.io/github/v/release/peunsu/ftb-snbt-lib?style=for-the-badge)
+
 A python library to parse, edit, and save FTB snbt tag.
 
 The FTB snbt tag is a variant of the "vanilla" snbt tag. It has no commas at end of lines, different suffixes for numeric values, and no support for array data type.
 
 This is the example of the FTB snbt tag:
 ```python
 {
@@ -107,12 +110,13 @@
 | Short | A signed 16-bit integer.<br>Range: ``-32,768`` ~ ``32,767`` | ``<number>s`` | ``132s``, ``-243s`` |
 | Integer | A signed 32-bit integer.<br>Range: ``-2,147,483,647`` ~ ``2,147,483,647`` | ``<number>`` | ``12345`` |
 | Long | A signed 64-bit integer.<br>Range: ``9,223,372,036,854,775,808`` ~ ``9,223,372,036,854,775,807`` | ``<number>L`` | ``12345L`` |
 | Double | A 64-bit, double-precision floating-point number.<br>Range: ``-1.7E+308`` ~ ``+1.7E+308.`` | ``<number>d`` | ``12.345d`` |
 | Bool | A boolean data type.<br>``0`` for ``false``, ``1`` for ``true``. | ``false``, ``true`` | ``true`` |
 | String | A sequence of characters. | A string enclosed in **double quotes ``""``**.<br>Nested double quotes can be included within a string using a **escaping character ``\"``**. | `"Hello, World!"`,<br>`"Say \"Hello, World!\""` |
 | List | An ordered list of tags.<br>The tags must be of **the same type**, determined by the first tag in the list. | Unnamed tags enclosed in square brackets and delimited by **newline** characters (``\n``). | <pre>[<br>    3.2d<br>    1.4d<br>    ...<br>]</pre> |
+| Array | An ordered list of 8-bit(ByteArray), 32-bit(IntArray), 64-bit(LongArray) integers. | ``<array_prefix>;`` followed by an ordered list of tags enclosed in square brackets and delimited by **newline** characters (``\n``).<br>Valid array prefixes are ``B``(Byte), ``I``(Integer), and ``L``(Long). | <pre>[B;<br>    12b<br>    -35b<br>    ...<br>]</pre> |
 | Compound | An ordered list of attribute-value pairs.<br>Each tag can be of **any type**. | Named tags enclosed in curly braces and delimited by commas or **newline** characters (``\n``).<br>The key (tag name) can be unquoted if it contains only ``0-9``, ``A-Z``, ``a-z``, ``_``, ``-``, ``.``, and ``+``. Otherwise the key should be quoted, using the format of ``String`` type. | <pre>[<br>    tag1: "string"<br>    tag2: 12b<br>    \"quoted:tag\": 3.5d<br>    ...<br>]</pre> |
 
 ## References
 * [PLY - Python Lex-Yacc](https://github.com/dabeaz/ply) by [David Beazley](https://www.dabeaz.com)
 * [nbtlib](https://github.com/vberlier/nbtlib) by [vberlier](https://github.com/vberlier)
```

### Comparing `ftb-snbt-lib-0.1.3/pyproject.toml` & `ftb-snbt-lib-0.2.1/pyproject.toml`

 * *Files identical despite different names*

