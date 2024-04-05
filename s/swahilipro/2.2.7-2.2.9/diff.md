# Comparing `tmp/swahilipro-2.2.7.tar.gz` & `tmp/swahilipro-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swahilipro-2.2.7.tar", last modified: Thu Nov 30 12:59:05 2023, max compression
+gzip compressed data, was "swahilipro-2.2.9.tar", last modified: Fri Apr  5 11:35:54 2024, max compression
```

## Comparing `swahilipro-2.2.7.tar` & `swahilipro-2.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-30 12:59:05.714796 swahilipro-2.2.7/
--rw-rw-rw-   0        0        0     1896 2023-11-30 12:59:05.714796 swahilipro-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-10-20 10:19:29.000000 swahilipro-2.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-11-30 12:59:05.715798 swahilipro-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-11-30 12:58:38.000000 swahilipro-2.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-30 12:59:05.703827 swahilipro-2.2.7/swahilipro/
--rw-rw-rw-   0        0        0     1264 2023-10-24 10:09:54.000000 swahilipro-2.2.7/swahilipro/shell.py
--rw-rw-rw-   0        0        0      781 2023-10-24 10:05:42.000000 swahilipro-2.2.7/swahilipro/strings_with_arrows.py
--rw-rw-rw-   0        0        0    66153 2023-11-30 09:22:48.000000 swahilipro-2.2.7/swahilipro/swahilipro.py
-drwxrwxrwx   0        0        0        0 2023-11-30 12:59:05.712945 swahilipro-2.2.7/swahilipro.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-11-30 12:59:05.000000 swahilipro-2.2.7/swahilipro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-11-30 12:59:05.000000 swahilipro-2.2.7/swahilipro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-30 12:59:05.000000 swahilipro-2.2.7/swahilipro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-11-30 12:59:05.000000 swahilipro-2.2.7/swahilipro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-11-30 12:59:05.000000 swahilipro-2.2.7/swahilipro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:35:54.724871 swahilipro-2.2.9/
+-rw-rw-rw-   0        0        0     1896 2024-04-05 11:35:54.723341 swahilipro-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-10-20 10:19:29.000000 swahilipro-2.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:35:54.726063 swahilipro-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      582 2024-04-05 11:35:49.000000 swahilipro-2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:35:54.659929 swahilipro-2.2.9/swahilipro/
+-rw-rw-rw-   0        0        0     1264 2023-10-24 10:09:54.000000 swahilipro-2.2.9/swahilipro/shell.py
+-rw-rw-rw-   0        0        0      781 2023-10-24 10:05:42.000000 swahilipro-2.2.9/swahilipro/strings_with_arrows.py
+-rw-rw-rw-   0        0        0    66148 2024-04-05 11:33:16.000000 swahilipro-2.2.9/swahilipro/swahilipro.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:35:54.719381 swahilipro-2.2.9/swahilipro.egg-info/
+-rw-rw-rw-   0        0        0     1896 2024-04-05 11:35:54.000000 swahilipro-2.2.9/swahilipro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-05 11:35:54.000000 swahilipro-2.2.9/swahilipro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:35:54.000000 swahilipro-2.2.9/swahilipro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-05 11:35:54.000000 swahilipro-2.2.9/swahilipro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 11:35:54.000000 swahilipro-2.2.9/swahilipro.egg-info/top_level.txt
```

### Comparing `swahilipro-2.2.7/PKG-INFO` & `swahilipro-2.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: swahilipro
-Version: 2.2.7
-Summary: A compiler package
-Author: Masota & Ngigi
-Author-email: bonniemasota@gmail.com
-Description-Content-Type: text/markdown
-
 # SwahiliPro Programming Language Compiler
 
 SwahiliPro is a Swahili-based programming language and compiler designed to make programming more accessible to Swahili-speaking developers. This README provides an overview of SwahiliPro and instructions for building and using the compiler.
 
 ## Table of Contents
 - [Getting Started](#getting-started)
 - [Features](#features)
```

### Comparing `swahilipro-2.2.7/README.md` & `swahilipro-2.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: swahilipro
+Version: 2.2.9
+Summary: A compiler package
+Author: Masota & Ngigi
+Author-email: bonniemasota@gmail.com
+Description-Content-Type: text/markdown
+
 # SwahiliPro Programming Language Compiler
 
 SwahiliPro is a Swahili-based programming language and compiler designed to make programming more accessible to Swahili-speaking developers. This README provides an overview of SwahiliPro and instructions for building and using the compiler.
 
 ## Table of Contents
 - [Getting Started](#getting-started)
 - [Features](#features)
```

### Comparing `swahilipro-2.2.7/swahilipro/shell.py` & `swahilipro-2.2.9/swahilipro/shell.py`

 * *Files identical despite different names*

### Comparing `swahilipro-2.2.7/swahilipro/strings_with_arrows.py` & `swahilipro-2.2.9/swahilipro/strings_with_arrows.py`

 * *Files identical despite different names*

### Comparing `swahilipro-2.2.7/swahilipro/swahilipro.py` & `swahilipro-2.2.9/swahilipro/swahilipro.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,28 +120,28 @@
 TT_POW		= 'KARISIMU'
 TT_KEYWORD  = 'NENO_MUHIMU'
 TT_IDENTIFIER = 'KITAMBULISHO'
 TT_EQ	= 'SAWA'
 TT_STRING = 'NENO'
 
 KEYWORDS = [
-  'VAR',
-  'NA',
-  'AU',
-  'IKIWA',
-  'AU_IKIWA',
-  'IKIWA_NYINGINE',
-  'KWA',
-  'HADI',
-  'WAKATI',
-  'NJIA',
-  'BASI',
-  'FUNGA',
-  'RUDISHA',
-  'VUNJA',
+  'var',
+  'na',
+  'au',
+  'ikiwa',
+  'au_ikiwa',
+  'ikiwa_nyingine',
+  'kwa',
+  'hadi',
+  'wakati',
+  'njia',
+  'basi',
+  'funga',
+  'rudisha',
+  'vunja',
 ]
 
 class Token:
   def __init__(self, type_, value=None, pos_start=None, pos_end=None):
     self.type = type_
     self.value = value
 
@@ -2155,31 +2155,31 @@
     return RTResult().success_break()
 
 #######################################
 # RUN
 #######################################
 
 global_symbol_table = SymbolTable()
-global_symbol_table.set("UONGO", Number.false)
-global_symbol_table.set("KWELI", Number.true)
-global_symbol_table.set("MATH_PI", Number.math_PI)
-global_symbol_table.set("ANDIKA", BuiltInFunction.print)
-global_symbol_table.set("ANDIKA_MSTARI_MPYA", BuiltInFunction.print_ret)
-global_symbol_table.set("BONYEZA", BuiltInFunction.input)
-global_symbol_table.set("BONYEZA_NAM", BuiltInFunction.input_int)
-global_symbol_table.set("FUTA", BuiltInFunction.clear)
-global_symbol_table.set("CLS", BuiltInFunction.clear)
-global_symbol_table.set("NI_NAMBARI", BuiltInFunction.is_number)
-global_symbol_table.set("NI_NENO", BuiltInFunction.is_string)
-global_symbol_table.set("NI_ORODHA", BuiltInFunction.is_list)
-global_symbol_table.set("NI_NJIA", BuiltInFunction.is_function)
-global_symbol_table.set("UNGANISHA", BuiltInFunction.append)
-global_symbol_table.set("POP", BuiltInFunction.pop)
-global_symbol_table.set("EXTEND", BuiltInFunction.extend)
-global_symbol_table.set("UREFU", BuiltInFunction.len)
+global_symbol_table.set("uongo", Number.false)
+global_symbol_table.set("kweli", Number.true)
+global_symbol_table.set("pi", Number.math_PI)
+global_symbol_table.set("andika", BuiltInFunction.print)
+global_symbol_table.set("andika_mstari_mpya", BuiltInFunction.print_ret)
+global_symbol_table.set("bonyeza", BuiltInFunction.input)
+global_symbol_table.set("bonyeza_num", BuiltInFunction.input_int)
+global_symbol_table.set("futa", BuiltInFunction.clear)
+global_symbol_table.set("cls", BuiltInFunction.clear)
+global_symbol_table.set("ni_nambari", BuiltInFunction.is_number)
+global_symbol_table.set("ni_neno", BuiltInFunction.is_string)
+global_symbol_table.set("ni_orodha", BuiltInFunction.is_list)
+global_symbol_table.set("ni_njia", BuiltInFunction.is_function)
+global_symbol_table.set("unganisha", BuiltInFunction.append)
+global_symbol_table.set("toa", BuiltInFunction.pop)
+global_symbol_table.set("ongeza", BuiltInFunction.extend)
+global_symbol_table.set("urefu", BuiltInFunction.len)
 global_symbol_table.set("swa", BuiltInFunction.run)
 
 def run(fn, text):
   # Generate tokens
   lexer = Lexer(fn, text)
   tokens, error = lexer.make_tokens()
   if error: return None, error
```

### Comparing `swahilipro-2.2.7/swahilipro.egg-info/PKG-INFO` & `swahilipro-2.2.9/swahilipro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swahilipro
-Version: 2.2.7
+Version: 2.2.9
 Summary: A compiler package
 Author: Masota & Ngigi
 Author-email: bonniemasota@gmail.com
 Description-Content-Type: text/markdown
 
 # SwahiliPro Programming Language Compiler
```

