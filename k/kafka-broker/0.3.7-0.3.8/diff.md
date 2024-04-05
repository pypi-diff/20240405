# Comparing `tmp/kafka-broker-0.3.7.tar.gz` & `tmp/kafka-broker-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.7.tar", last modified: Fri Apr  5 12:04:11 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.8.tar", last modified: Fri Apr  5 12:08:14 2024, max compression
```

## Comparing `kafka-broker-0.3.7.tar` & `kafka-broker-0.3.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.332223 kafka-broker-0.3.7/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 12:04:11.330022 kafka-broker-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.7/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 12:01:16.000000 kafka-broker-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 12:04:11.332730 kafka-broker-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.240775 kafka-broker-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.281266 kafka-broker-0.3.7/src/kafka_broker/
--rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.7/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.7/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.7/src/kafka_broker/broker_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.310840 kafka-broker-0.3.7/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.7/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.7/src/kafka_broker/classes/cache.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.7/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.7/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.7/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.7/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3238 2024-04-05 12:00:49.000000 kafka-broker-0.3.7/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.7/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.315832 kafka-broker-0.3.7/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.7/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.7/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.7/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1693 2024-04-05 12:04:05.000000 kafka-broker-0.3.7/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.7/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.323553 kafka-broker-0.3.7/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 12:04:11.000000 kafka-broker-0.3.7/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2024-04-05 12:04:11.000000 kafka-broker-0.3.7/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:04:11.000000 kafka-broker-0.3.7/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 12:04:11.000000 kafka-broker-0.3.7/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 12:04:11.000000 kafka-broker-0.3.7/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 12:04:11.317023 kafka-broker-0.3.7/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.7/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.069801 kafka-broker-0.3.8/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 12:08:14.066788 kafka-broker-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.8/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 12:04:13.000000 kafka-broker-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 12:08:14.070802 kafka-broker-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:13.991022 kafka-broker-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.026682 kafka-broker-0.3.8/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.8/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.8/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.8/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.055790 kafka-broker-0.3.8/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.8/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.8/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.8/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.8/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.8/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.8/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3238 2024-04-05 12:00:49.000000 kafka-broker-0.3.8/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.8/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.061301 kafka-broker-0.3.8/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.8/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.8/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.8/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1824 2024-04-05 12:08:10.000000 kafka-broker-0.3.8/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.8/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.065276 kafka-broker-0.3.8/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 12:08:13.000000 kafka-broker-0.3.8/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2024-04-05 12:08:13.000000 kafka-broker-0.3.8/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:08:13.000000 kafka-broker-0.3.8/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 12:08:13.000000 kafka-broker-0.3.8/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 12:08:13.000000 kafka-broker-0.3.8/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 12:08:14.064271 kafka-broker-0.3.8/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.8/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.7/LICENSE` & `kafka-broker-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/PKG-INFO` & `kafka-broker-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.7/README.md` & `kafka-broker-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/pyproject.toml` & `kafka-broker-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.7"
+version = "0.3.8"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.7/src/kafka_broker/broker_manager.py` & `kafka-broker-0.3.8/src/kafka_broker/broker_manager.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/classes/cache.py` & `kafka-broker-0.3.8/src/kafka_broker/classes/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.8/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.8/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.8/src/kafka_broker/classes/event_router.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/config.py` & `kafka-broker-0.3.8/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/consumer.py` & `kafka-broker-0.3.8/src/kafka_broker/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.8/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.7/src/kafka_broker/producer.py` & `kafka-broker-0.3.8/src/kafka_broker/producer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 from typing import Callable
 from confluent_kafka import Producer
 from .exceptions.cache import KeyNotFoundException
 
 from .classes.cache import Cache
 from .classes.event_object import EventObject
@@ -19,23 +20,23 @@
     topic: str,
     event_object: EventObject,
     callback: Callable = default_callback,
 ):
     """Produce an event to the kafka message queue."""
     logging.debug("just_some_spacing :D")
     logging.debug("just_some_spacing :D")
-    logging.critical(f"start_instruction: {event_object.data.get('start_instruction')}")
+    logging.critical(f"start_instruction: {event_object.data.get('start_instruction')}, json: {json.dumps(event_object.data.get('start_instruction'))}, type: {type(event_object.data.get('start_instruction'))}")
 
     kafka_config = config["kafka.default"]
     kafka_config.update(config["kafka.producer"])
 
     producer = Producer(kafka_config)
     event_object.add_audit_log(config["general"]["current_location"])
     event_json = event_object.encode()
-    
+
     logging.debug("just_some_spacing :D")
     logging.debug("just_some_spacing :D")
     logging.critical(f"event_json: {event_json}")
 
     producer.produce(
         topic,
         key=str(event_object.correlation_id),
```

### Comparing `kafka-broker-0.3.7/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.8/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.7/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.8/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

