# Comparing `tmp/arb_logger-2.1.3.tar.gz` & `tmp/arb_logger-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arb_logger-2.1.3.tar", last modified: Sun Apr 16 08:55:05 2023, max compression
+gzip compressed data, was "arb_logger-2.2.1.tar", last modified: Fri Apr  5 18:49:57 2024, max compression
```

## Comparing `arb_logger-2.1.3.tar` & `arb_logger-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.692069 arb_logger-2.1.3/
--rw-r--r--   0 acid3croco   (501) staff       (20)     3997 2023-04-16 08:55:05.691510 arb_logger-2.1.3/PKG-INFO
--rw-r--r--   0 acid3croco   (501) staff       (20)     3748 2023-04-13 14:43:15.000000 arb_logger-2.1.3/README.md
-drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.688125 arb_logger-2.1.3/arb_logger/
--rw-r--r--   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:53:23.000000 arb_logger-2.1.3/arb_logger/__init__.py
--rw-r--r--   0 acid3croco   (501) staff       (20)     2040 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/alert_message.py
--rw-r--r--   0 acid3croco   (501) staff       (20)     2694 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/arb_alerts.py
--rw-r--r--   0 acid3croco   (501) staff       (20)     4853 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/logger.py
-drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.690816 arb_logger-2.1.3/arb_logger.egg-info/
--rw-r--r--   0 acid3croco   (501) staff       (20)     3997 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/PKG-INFO
--rw-r--r--   0 acid3croco   (501) staff       (20)      321 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/SOURCES.txt
--rw-r--r--   0 acid3croco   (501) staff       (20)        1 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/dependency_links.txt
--rw-r--r--   0 acid3croco   (501) staff       (20)       58 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/entry_points.txt
--rw-r--r--   0 acid3croco   (501) staff       (20)       23 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/requires.txt
--rw-r--r--   0 acid3croco   (501) staff       (20)       11 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/top_level.txt
--rw-r--r--   0 acid3croco   (501) staff       (20)       38 2023-04-16 08:55:05.692242 arb_logger-2.1.3/setup.cfg
--rw-r--r--   0 acid3croco   (501) staff       (20)      577 2023-04-16 08:53:35.000000 arb_logger-2.1.3/setup.py
+drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-04-05 18:49:57.412961 arb_logger-2.2.1/
+-rw-r--r--   0 jack       (501) staff       (20)     4063 2024-04-05 18:49:57.412757 arb_logger-2.2.1/PKG-INFO
+-rw-r--r--   0 jack       (501) staff       (20)     3746 2024-03-03 12:58:39.000000 arb_logger-2.2.1/README.md
+drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-04-05 18:49:57.411348 arb_logger-2.2.1/arb_logger/
+-rw-r--r--   0 jack       (501) staff       (20)        0 2023-07-29 09:25:49.000000 arb_logger-2.2.1/arb_logger/__init__.py
+-rw-r--r--   0 jack       (501) staff       (20)     2040 2023-07-29 09:25:49.000000 arb_logger-2.2.1/arb_logger/alert_message.py
+-rw-r--r--   0 jack       (501) staff       (20)     2694 2023-07-29 09:25:49.000000 arb_logger-2.2.1/arb_logger/arb_alerts.py
+-rw-r--r--   0 jack       (501) staff       (20)     6182 2024-04-05 18:47:20.000000 arb_logger-2.2.1/arb_logger/logger.py
+drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-04-05 18:49:57.412547 arb_logger-2.2.1/arb_logger.egg-info/
+-rw-r--r--   0 jack       (501) staff       (20)     4063 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/PKG-INFO
+-rw-r--r--   0 jack       (501) staff       (20)      342 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 jack       (501) staff       (20)        1 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 jack       (501) staff       (20)       58 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/entry_points.txt
+-rw-r--r--   0 jack       (501) staff       (20)       23 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/requires.txt
+-rw-r--r--   0 jack       (501) staff       (20)       11 2024-04-05 18:49:57.000000 arb_logger-2.2.1/arb_logger.egg-info/top_level.txt
+-rw-r--r--   0 jack       (501) staff       (20)       38 2024-04-05 18:49:57.413005 arb_logger-2.2.1/setup.cfg
+-rw-r--r--   0 jack       (501) staff       (20)      577 2024-04-05 18:47:30.000000 arb_logger-2.2.1/setup.py
+drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-04-05 18:49:57.412284 arb_logger-2.2.1/tests/
+-rw-r--r--   0 jack       (501) staff       (20)     5190 2023-07-29 09:25:49.000000 arb_logger-2.2.1/tests/test_logger.py
```

### Comparing `arb_logger-2.1.3/PKG-INFO` & `arb_logger-2.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: arb_logger
-Version: 2.1.3
-Summary: A custom logger with Redis integration
-Home-page: https://github.com/Acid3croco/arb-trops-services
-Author: arb
-Author-email: arb.trops@gmail.com
-Description-Content-Type: text/markdown
-
 # arb_logger
 
 ## Introduction
 
 `arb_logger` is a Python package that provides advanced logging capabilities, including file logging, console logging with colors, and Redis integration. This package aims to simplify and standardize logging for Python applications by offering an easy-to-use interface and configurable options.
 
 ## Features
@@ -31,15 +22,15 @@
 ```bash
 pip install arb_logger
 ```
 
 To install the `arb_logger` package from source, simply clone the repository and install it using `pip`:
 
 ```bash
-git clone https://github.com/yourusername/arb_logger.git
+git clone https://github.com/acid3croco/arb_logger.git
 cd arb_logger
 pip install .
 ```
 
 ## Usage
 
 ### Basic Usage
```

### Comparing `arb_logger-2.1.3/README.md` & `arb_logger-2.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: arb_logger
+Version: 2.2.1
+Summary: A custom logger with Redis integration
+Home-page: https://github.com/Acid3croco/arb-trops-services
+Author: arb
+Author-email: arb.trops@gmail.com
+Description-Content-Type: text/markdown
+Requires-Dist: coloredlogs
+Requires-Dist: redis
+Requires-Dist: pync
+
 # arb_logger
 
 ## Introduction
 
 `arb_logger` is a Python package that provides advanced logging capabilities, including file logging, console logging with colors, and Redis integration. This package aims to simplify and standardize logging for Python applications by offering an easy-to-use interface and configurable options.
 
 ## Features
@@ -22,15 +34,15 @@
 ```bash
 pip install arb_logger
 ```
 
 To install the `arb_logger` package from source, simply clone the repository and install it using `pip`:
 
 ```bash
-git clone https://github.com/yourusername/arb_logger.git
+git clone https://github.com/acid3croco/arb_logger.git
 cd arb_logger
 pip install .
 ```
 
 ## Usage
 
 ### Basic Usage
```

### Comparing `arb_logger-2.1.3/arb_logger/alert_message.py` & `arb_logger-2.2.1/arb_logger/alert_message.py`

 * *Files identical despite different names*

### Comparing `arb_logger-2.1.3/arb_logger/arb_alerts.py` & `arb_logger-2.2.1/arb_logger/arb_alerts.py`

 * *Files identical despite different names*

### Comparing `arb_logger-2.1.3/arb_logger.egg-info/PKG-INFO` & `arb_logger-2.2.1/arb_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: arb-logger
-Version: 2.1.3
+Version: 2.2.1
 Summary: A custom logger with Redis integration
 Home-page: https://github.com/Acid3croco/arb-trops-services
 Author: arb
 Author-email: arb.trops@gmail.com
 Description-Content-Type: text/markdown
+Requires-Dist: coloredlogs
+Requires-Dist: redis
+Requires-Dist: pync
 
 # arb_logger
 
 ## Introduction
 
 `arb_logger` is a Python package that provides advanced logging capabilities, including file logging, console logging with colors, and Redis integration. This package aims to simplify and standardize logging for Python applications by offering an easy-to-use interface and configurable options.
 
@@ -31,15 +34,15 @@
 ```bash
 pip install arb_logger
 ```
 
 To install the `arb_logger` package from source, simply clone the repository and install it using `pip`:
 
 ```bash
-git clone https://github.com/yourusername/arb_logger.git
+git clone https://github.com/acid3croco/arb_logger.git
 cd arb_logger
 pip install .
 ```
 
 ## Usage
 
 ### Basic Usage
```

### Comparing `arb_logger-2.1.3/setup.py` & `arb_logger-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     name='arb_logger',
     author='arb',
     author_email='arb.trops@gmail.com',
     description="A custom logger with Redis integration",
     url="https://github.com/Acid3croco/arb-trops-services",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    version='2.1.3',
+    version='2.2.1',
     packages=find_packages(),
     install_requires=['coloredlogs', 'redis', 'pync'],
     entry_points={
         'console_scripts': [
             'arb_alerts = arb_logger.arb_alerts:main',
         ]
     },
```

