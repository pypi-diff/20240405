# Comparing `tmp/kafka-broker-0.3.3.tar.gz` & `tmp/kafka-broker-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.3.tar", last modified: Fri Apr  5 11:12:10 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.4.tar", last modified: Fri Apr  5 11:17:38 2024, max compression
```

## Comparing `kafka-broker-0.3.3.tar` & `kafka-broker-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.159889 kafka-broker-0.3.3/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:12:10.156868 kafka-broker-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 11:12:06.000000 kafka-broker-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 11:12:10.160879 kafka-broker-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.115631 kafka-broker-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.131554 kafka-broker-0.3.3/src/kafka_broker/
--rw-rw-rw-   0        0        0     6164 2024-04-05 09:02:03.000000 kafka-broker-0.3.3/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     1997 2024-04-05 08:21:59.000000 kafka-broker-0.3.3/src/kafka_broker/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.148127 kafka-broker-0.3.3/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.3/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1790 2024-04-05 08:36:05.000000 kafka-broker-0.3.3/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3229 2024-04-05 08:17:11.000000 kafka-broker-0.3.3/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.3/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.151334 kafka-broker-0.3.3/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.3/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.3/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.155868 kafka-broker-0.3.3/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.154872 kafka-broker-0.3.3/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.865652 kafka-broker-0.3.4/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:17:38.863661 kafka-broker-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 11:17:33.000000 kafka-broker-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:17:38.866605 kafka-broker-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.814797 kafka-broker-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.836209 kafka-broker-0.3.4/src/kafka_broker/
+-rw-rw-rw-   0        0        0     6148 2024-04-05 11:17:26.000000 kafka-broker-0.3.4/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     1997 2024-04-05 08:21:59.000000 kafka-broker-0.3.4/src/kafka_broker/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.852554 kafka-broker-0.3.4/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.4/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1790 2024-04-05 08:36:05.000000 kafka-broker-0.3.4/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3229 2024-04-05 08:17:11.000000 kafka-broker-0.3.4/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.4/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.858657 kafka-broker-0.3.4/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.4/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.4/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.861605 kafka-broker-0.3.4/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.859607 kafka-broker-0.3.4/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.3/LICENSE` & `kafka-broker-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/PKG-INFO` & `kafka-broker-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.3/README.md` & `kafka-broker-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/pyproject.toml` & `kafka-broker-0.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.3/src/kafka_broker/__init__.py` & `kafka-broker-0.3.4/src/kafka_broker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from typing import Any, Callable
 from pydantic import BaseModel
 from typing_extensions import deprecated
 from confluent_kafka import Consumer
 
-from src.kafka_broker.enums import EventStatus
+from .enums import EventStatus
 
 from .cache import Cache
 from .classes import ConsumerStorage, EventObject, EventRouter
 from .consumer import init_consumer, initialize, consume
 from .producer import default_callback, produce
 from .config import get_config
```

### Comparing `kafka-broker-0.3.3/src/kafka_broker/cache.py` & `kafka-broker-0.3.4/src/kafka_broker/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.4/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.4/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.4/src/kafka_broker/classes/event_router.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/config.py` & `kafka-broker-0.3.4/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/consumer.py` & `kafka-broker-0.3.4/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.4/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker/producer.py` & `kafka-broker-0.3.4/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.3/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.4/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.3/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.4/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

