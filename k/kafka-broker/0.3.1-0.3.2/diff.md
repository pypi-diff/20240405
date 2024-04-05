# Comparing `tmp/kafka-broker-0.3.1.tar.gz` & `tmp/kafka-broker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.1.tar", last modified: Wed Jan 17 19:08:47 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.2.tar", last modified: Fri Apr  5 07:59:50 2024, max compression
```

## Comparing `kafka-broker-0.3.1.tar` & `kafka-broker-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.367523 kafka-broker-0.3.1/
--rw-rw-rw-   0        0        0     1090 2023-11-08 08:14:34.000000 kafka-broker-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-01-17 19:08:47.367006 kafka-broker-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-09 00:14:54.000000 kafka-broker-0.3.1/README.md
--rw-rw-rw-   0        0        0      851 2024-01-17 19:07:58.000000 kafka-broker-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-17 19:08:47.367523 kafka-broker-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      365 2023-12-06 11:16:46.000000 kafka-broker-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.345896 kafka-broker-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.355213 kafka-broker-0.3.1/src/kafka_broker/
--rw-rw-rw-   0        0        0     4742 2023-11-21 09:47:37.000000 kafka-broker-0.3.1/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 09:47:34.000000 kafka-broker-0.3.1/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     1999 2024-01-17 19:08:31.000000 kafka-broker-0.3.1/src/kafka_broker/cache.py
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.362309 kafka-broker-0.3.1/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0      249 2023-11-08 08:39:27.000000 kafka-broker-0.3.1/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-11-09 09:30:42.000000 kafka-broker-0.3.1/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2635 2024-01-10 13:22:41.000000 kafka-broker-0.3.1/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1335 2023-12-06 11:15:54.000000 kafka-broker-0.3.1/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-09 14:58:28.000000 kafka-broker-0.3.1/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3192 2024-01-17 09:20:39.000000 kafka-broker-0.3.1/src/kafka_broker/consumer.py
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.364908 kafka-broker-0.3.1/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:32:52.000000 kafka-broker-0.3.1/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 09:32:52.000000 kafka-broker-0.3.1/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      598 2023-11-21 09:32:52.000000 kafka-broker-0.3.1/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1361 2023-11-22 09:24:36.000000 kafka-broker-0.3.1/src/kafka_broker/producer.py
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.359180 kafka-broker-0.3.1/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-01-17 19:08:47.000000 kafka-broker-0.3.1/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-01-17 19:08:47.000000 kafka-broker-0.3.1/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 19:08:47.000000 kafka-broker-0.3.1/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-01-17 19:08:47.000000 kafka-broker-0.3.1/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-17 19:08:47.000000 kafka-broker-0.3.1/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-17 19:08:47.365958 kafka-broker-0.3.1/tests/
--rw-rw-rw-   0        0        0      356 2023-11-09 00:14:54.000000 kafka-broker-0.3.1/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.457001 kafka-broker-0.3.2/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 07:59:50.456046 kafka-broker-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 07:55:47.000000 kafka-broker-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 07:59:50.457999 kafka-broker-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.401922 kafka-broker-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.423970 kafka-broker-0.3.2/src/kafka_broker/
+-rw-rw-rw-   0        0        0     4742 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     1999 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.442427 kafka-broker-0.3.2/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2635 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1335 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3192 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/consumer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.450563 kafka-broker-0.3.2/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      598 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.2/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.2/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.453288 kafka-broker-0.3.2/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.451617 kafka-broker-0.3.2/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.1/LICENSE` & `kafka-broker-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/PKG-INFO` & `kafka-broker-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.1/README.md` & `kafka-broker-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/pyproject.toml` & `kafka-broker-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.1/src/kafka_broker/__init__.py` & `kafka-broker-0.3.2/src/kafka_broker/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/cache.py` & `kafka-broker-0.3.2/src/kafka_broker/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.2/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.2/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.2/src/kafka_broker/classes/event_router.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/config.py` & `kafka-broker-0.3.2/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/consumer.py` & `kafka-broker-0.3.2/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.2/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker/producer.py` & `kafka-broker-0.3.2/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.1/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.2/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.1/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.2/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/kafka_broker/__init__.py
 src/kafka_broker/base_config.ini
 src/kafka_broker/cache.py
 src/kafka_broker/config.py
 src/kafka_broker/consumer.py
 src/kafka_broker/producer.py
+src/kafka_broker/py.typed
 src/kafka_broker.egg-info/PKG-INFO
 src/kafka_broker.egg-info/SOURCES.txt
 src/kafka_broker.egg-info/dependency_links.txt
 src/kafka_broker.egg-info/requires.txt
 src/kafka_broker.egg-info/top_level.txt
 src/kafka_broker/classes/__init__.py
 src/kafka_broker/classes/consumer_storage.py
```

