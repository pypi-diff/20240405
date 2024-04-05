# Comparing `tmp/laoshi-0.0.0.tar.gz` & `tmp/laoshi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laoshi-0.0.0.tar", max compression
+gzip compressed data, was "laoshi-0.1.0.tar", max compression
```

## Comparing `laoshi-0.0.0.tar` & `laoshi-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16726 2024-04-05 10:00:52.113290 laoshi-0.0.0/LICENSE
--rw-r--r--   0        0        0       48 2024-04-05 10:00:52.113290 laoshi-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/__init__.py
--rw-r--r--   0        0        0     1173 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/converter.py
--rw-r--r--   0        0        0     4903 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/deckmanager.py
--rw-r--r--   0        0        0     3967 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/flashcardgenerator.py
--rw-r--r--   0        0        0     2176 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/main.py
--rw-r--r--   0        0        0      888 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/speaker.py
--rw-r--r--   0        0        0      467 2024-04-05 10:00:52.113290 laoshi-0.0.0/laoshi/translator.py
--rw-r--r--   0        0        0      648 2024-04-05 10:00:52.113290 laoshi-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 laoshi-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-04-05 09:50:07.294064 laoshi-0.1.0/LICENSE
+-rw-r--r--   0        0        0       48 2024-04-05 09:50:07.294064 laoshi-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/__init__.py
+-rw-r--r--   0        0        0     1173 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/converter.py
+-rw-r--r--   0        0        0     4903 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/deckmanager.py
+-rw-r--r--   0        0        0     3967 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/flashcardgenerator.py
+-rw-r--r--   0        0        0     2176 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/main.py
+-rw-r--r--   0        0        0      888 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/speaker.py
+-rw-r--r--   0        0        0      467 2024-04-05 09:50:07.294064 laoshi-0.1.0/laoshi/translator.py
+-rw-r--r--   0        0        0      540 2024-04-05 09:50:07.294064 laoshi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 laoshi-0.1.0/PKG-INFO
```

### Comparing `laoshi-0.0.0/LICENSE` & `laoshi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/laoshi/converter.py` & `laoshi-0.1.0/laoshi/converter.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/laoshi/deckmanager.py` & `laoshi-0.1.0/laoshi/deckmanager.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/laoshi/flashcardgenerator.py` & `laoshi-0.1.0/laoshi/flashcardgenerator.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/laoshi/main.py` & `laoshi-0.1.0/laoshi/main.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/laoshi/speaker.py` & `laoshi-0.1.0/laoshi/speaker.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.0/PKG-INFO` & `laoshi-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laoshi
-Version: 0.0.0
+Version: 0.1.0
 Summary: 
 Author: Ruben Serradas
 Author-email: rubenserradas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

