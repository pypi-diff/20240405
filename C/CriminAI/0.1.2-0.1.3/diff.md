# Comparing `tmp/CriminAI-0.1.2.tar.gz` & `tmp/CriminAI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CriminAI-0.1.2.tar", last modified: Tue Apr  2 15:27:57 2024, max compression
+gzip compressed data, was "CriminAI-0.1.3.tar", last modified: Fri Apr  5 14:33:55 2024, max compression
```

## Comparing `CriminAI-0.1.2.tar` & `CriminAI-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:27:57.700872 CriminAI-0.1.2/
-drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:27:57.700631 CriminAI-0.1.2/CriminAI.egg-info/
--rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:27:57.000000 CriminAI-0.1.2/CriminAI.egg-info/PKG-INFO
--rw-r--r--   0 matis      (501) staff       (20)      136 2024-04-02 15:27:57.000000 CriminAI-0.1.2/CriminAI.egg-info/SOURCES.txt
--rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:27:57.000000 CriminAI-0.1.2/CriminAI.egg-info/dependency_links.txt
--rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:27:57.000000 CriminAI-0.1.2/CriminAI.egg-info/top_level.txt
--rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:27:57.700785 CriminAI-0.1.2/PKG-INFO
--rw-r--r--   0 matis      (501) staff       (20)       38 2024-04-02 15:27:57.700915 CriminAI-0.1.2/setup.cfg
--rw-r--r--   0 matis      (501) staff       (20)      546 2024-04-02 15:27:39.000000 CriminAI-0.1.2/setup.py
+drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-05 14:33:55.329218 CriminAI-0.1.3/
+drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-05 14:33:55.329042 CriminAI-0.1.3/CriminAI.egg-info/
+-rw-r--r--   0 matis      (501) staff       (20)      702 2024-04-05 14:33:55.000000 CriminAI-0.1.3/CriminAI.egg-info/PKG-INFO
+-rw-r--r--   0 matis      (501) staff       (20)      199 2024-04-05 14:33:55.000000 CriminAI-0.1.3/CriminAI.egg-info/SOURCES.txt
+-rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-05 14:33:55.000000 CriminAI-0.1.3/CriminAI.egg-info/dependency_links.txt
+-rw-r--r--   0 matis      (501) staff       (20)       42 2024-04-05 14:33:55.000000 CriminAI-0.1.3/CriminAI.egg-info/requires.txt
+-rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-05 14:33:55.000000 CriminAI-0.1.3/CriminAI.egg-info/top_level.txt
+-rw-r--r--   0 matis      (501) staff       (20)     1107 2024-04-05 14:21:11.000000 CriminAI-0.1.3/LICENSE.txt
+-rw-r--r--   0 matis      (501) staff       (20)      702 2024-04-05 14:33:55.329265 CriminAI-0.1.3/PKG-INFO
+-rw-r--r--   0 matis      (501) staff       (20)     2028 2024-04-05 14:18:54.000000 CriminAI-0.1.3/README.md
+-rw-r--r--   0 matis      (501) staff       (20)       79 2024-04-05 14:33:55.329423 CriminAI-0.1.3/setup.cfg
+-rw-r--r--   0 matis      (501) staff       (20)      841 2024-04-05 14:33:34.000000 CriminAI-0.1.3/setup.py
```

### Comparing `CriminAI-0.1.2/CriminAI.egg-info/PKG-INFO` & `CriminAI-0.1.3/CriminAI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: CriminAI
-Version: 0.1.2
+Version: 0.1.3
 Summary: CriminAI est un logiciel de génération de portraits robots par IA
-Home-page: UNKNOWN
+Home-page: https://github.com/matzouari/ProjetDevLogiciel/
 Author: ZOUARI Matis, PEREZ Lisa, SUTTER Clemence, ZHONG Zhihan
 Author-email: matis.zouari@insa-lyon.fr, lisa.perez@insa-lyon.fr, clemence.sutter@insa-lyon.fr, zhihan.zhong@insa-lyon.fr
 License: UNKNOWN
+Download-URL: https://github.com/matzouari/ProjetDevLogiciel/archive/refs/tags/1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `CriminAI-0.1.2/PKG-INFO` & `CriminAI-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: CriminAI
-Version: 0.1.2
+Version: 0.1.3
 Summary: CriminAI est un logiciel de génération de portraits robots par IA
-Home-page: UNKNOWN
+Home-page: https://github.com/matzouari/ProjetDevLogiciel/
 Author: ZOUARI Matis, PEREZ Lisa, SUTTER Clemence, ZHONG Zhihan
 Author-email: matis.zouari@insa-lyon.fr, lisa.perez@insa-lyon.fr, clemence.sutter@insa-lyon.fr, zhihan.zhong@insa-lyon.fr
 License: UNKNOWN
+Download-URL: https://github.com/matzouari/ProjetDevLogiciel/archive/refs/tags/1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
+License-File: LICENSE.txt
 
 UNKNOWN
```

