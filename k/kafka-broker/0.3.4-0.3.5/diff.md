# Comparing `tmp/kafka-broker-0.3.4.tar.gz` & `tmp/kafka-broker-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.4.tar", last modified: Fri Apr  5 11:17:38 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.5.tar", last modified: Fri Apr  5 11:52:45 2024, max compression
```

## Comparing `kafka-broker-0.3.4.tar` & `kafka-broker-0.3.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.865652 kafka-broker-0.3.4/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:17:38.863661 kafka-broker-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 11:17:33.000000 kafka-broker-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 11:17:38.866605 kafka-broker-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.814797 kafka-broker-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.836209 kafka-broker-0.3.4/src/kafka_broker/
--rw-rw-rw-   0        0        0     6148 2024-04-05 11:17:26.000000 kafka-broker-0.3.4/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     1997 2024-04-05 08:21:59.000000 kafka-broker-0.3.4/src/kafka_broker/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.852554 kafka-broker-0.3.4/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.4/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1790 2024-04-05 08:36:05.000000 kafka-broker-0.3.4/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3229 2024-04-05 08:17:11.000000 kafka-broker-0.3.4/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.4/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.858657 kafka-broker-0.3.4/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.4/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.4/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.4/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.861605 kafka-broker-0.3.4/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 11:17:38.000000 kafka-broker-0.3.4/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 11:17:38.859607 kafka-broker-0.3.4/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.4/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.240556 kafka-broker-0.3.5/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:52:45.236547 kafka-broker-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 11:52:42.000000 kafka-broker-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:52:45.241558 kafka-broker-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.160654 kafka-broker-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.195900 kafka-broker-0.3.5/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.5/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.5/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.218036 kafka-broker-0.3.5/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.5/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.5/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.5/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.5/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3243 2024-04-05 11:50:46.000000 kafka-broker-0.3.5/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.5/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.228029 kafka-broker-0.3.5/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1382 2024-04-05 11:51:06.000000 kafka-broker-0.3.5/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.5/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.233528 kafka-broker-0.3.5/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.231017 kafka-broker-0.3.5/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.4/LICENSE` & `kafka-broker-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/PKG-INFO` & `kafka-broker-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.4/README.md` & `kafka-broker-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/pyproject.toml` & `kafka-broker-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker/__init__.py` & `kafka-broker-0.3.5/src/kafka_broker/broker_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from typing import Any, Callable
 from pydantic import BaseModel
 from typing_extensions import deprecated
 from confluent_kafka import Consumer
 
 from .enums import EventStatus
-
-from .cache import Cache
-from .classes import ConsumerStorage, EventObject, EventRouter
 from .consumer import init_consumer, initialize, consume
 from .producer import default_callback, produce
+from .classes.consumer_storage import ConsumerStorage
+from .classes.event_object import EventObject
+from .classes.cache import Cache
 from .config import get_config
 
 
 class BrokerManager:
     consumer_storage: ConsumerStorage
     cache: Cache
 
@@ -71,21 +71,18 @@
         if not self.consumer:
             kafka_config = self.config["kafka.default"]
             kafka_config.update(self.config["kafka.consumer"])
             self.consumer = Consumer(kafka_config)
             self.consumer.subscribe([self.config["general"]["current_location"]])
         return consume(self.consumer, self.logger)
 
-    @deprecated
+    @deprecated("It says depricated, but it might still work. It will not be updated anymore.")
     def init_consumer_app(self, app):
         """Setup the consumer on a FastAPI instance.
 
-        It says depricated, but it might still work.
-        It will not be updated anymore.
-
         Parameters
         ----------
         app : FastAPI
             The FastAPI app.
 
         Returns
         -------
@@ -184,17 +181,8 @@
 
         event_object.event = event
         event_object.data = {"payload": data, **kwargs}
 
         self.produce(module, event_object)
 
 
-broker_manager = BrokerManager()
-
-__all__ = [
-    "broker_manager",
-    "BrokerManager",
-    "ConsumerStorage",
-    "EventObject",
-    "EventRouter",
-    "Cache",
-]
+broker_manager = BrokerManager()
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker/cache.py` & `kafka-broker-0.3.5/src/kafka_broker/classes/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from logging import Logger
 from uuid import UUID
 
-from .exceptions.cache import (
+from ..exceptions.cache import (
     ConnectionException,
     CouldNotEditMemcache,
     KeyNotFoundException,
 )
-from .classes import EventObject
+from .event_object import EventObject
 from pymemcache.client.base import Client
 
 
 class Cache:
     def __init__(self, config, logger: Logger) -> None:
         self.client = self.innitialize_connection(config)
         self.config = config
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.5/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.5/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.5/src/kafka_broker/classes/event_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Self
 
 from ..enums import EventStatus
+from ..broker_manager import broker_manager
 from .event_object import EventObject
-from .. import broker_manager
 
 
 class EventRouter:
     """A simple router.
     Bind events to expose them to the router.
     Bind routers to expand the router.
     """
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker/config.py` & `kafka-broker-0.3.5/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/src/kafka_broker/consumer.py` & `kafka-broker-0.3.5/src/kafka_broker/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from confluent_kafka import Consumer
 from multiprocessing import Pipe, Process
 
 # from multiprocessing.connection import PipeConnection
 
-from .classes import ConsumerStorage, EventObject
+from .classes.consumer_storage import ConsumerStorage
+from .classes.event_object import EventObject
 
 
 def init_consumer(
     config: dict, logger: logging.Logger, consumer_storage: ConsumerStorage, app
 ):
     """Initialize the consumer for FastAPI."""
     global consumer_storage_
@@ -77,15 +78,15 @@
     except KeyboardInterrupt:
         pass
 
     finally:
         consumer.close()
 
 
-def consume(consumer: Consumer, logger: logging.Logger) -> EventObject | None:
+def consume(consumer: Consumer, logger: logging.Logger):
     """Consumer loop."""
     try:
         while True:
             msg = consumer.poll(1.0)
 
             logger.debug("[*] Waiting...")
 
@@ -98,15 +99,15 @@
             else:
                 return handle(logger, msg)
 
     except KeyboardInterrupt:
         consumer.close()
 
 
-def handle(logger: logging.Logger, msg) -> EventObject:
+def handle(logger: logging.Logger, msg):
     """Handle a non error event."""
     topic = msg.topic()
     key = msg.key().decode("utf-8")
     value = msg.value().decode("utf-8")
 
     logger.info(
         "Consumed - topic {topic}: key = {key} value = {value}".format(
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.5/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.4/src/kafka_broker/producer.py` & `kafka-broker-0.3.5/src/kafka_broker/producer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Callable
 from confluent_kafka import Producer
 from .exceptions.cache import KeyNotFoundException
 
-from .classes import EventObject
-from .cache import Cache
+from .classes.cache import Cache
+from .classes.event_object import EventObject
 
 
 def default_callback(err, msg):
     if err:
         logging.error("Message failed delivery: {}".format(err))
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.5/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.4/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.5/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/kafka_broker/__init__.py
 src/kafka_broker/base_config.ini
-src/kafka_broker/cache.py
+src/kafka_broker/broker_manager.py
 src/kafka_broker/config.py
 src/kafka_broker/consumer.py
 src/kafka_broker/enums.py
 src/kafka_broker/producer.py
 src/kafka_broker/py.typed
 src/kafka_broker.egg-info/PKG-INFO
 src/kafka_broker.egg-info/SOURCES.txt
 src/kafka_broker.egg-info/dependency_links.txt
 src/kafka_broker.egg-info/requires.txt
 src/kafka_broker.egg-info/top_level.txt
 src/kafka_broker/classes/__init__.py
+src/kafka_broker/classes/cache.py
 src/kafka_broker/classes/consumer_storage.py
 src/kafka_broker/classes/event_object.py
 src/kafka_broker/classes/event_router.py
 src/kafka_broker/exceptions/__init__.py
 src/kafka_broker/exceptions/base.py
 src/kafka_broker/exceptions/cache.py
 tests/test_event_object.py
```

