# Comparing `tmp/kafka-broker-0.3.2.tar.gz` & `tmp/kafka-broker-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.2.tar", last modified: Fri Apr  5 07:59:50 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.3.tar", last modified: Fri Apr  5 11:12:10 2024, max compression
```

## Comparing `kafka-broker-0.3.2.tar` & `kafka-broker-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.457001 kafka-broker-0.3.2/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 07:59:50.456046 kafka-broker-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 07:55:47.000000 kafka-broker-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 07:59:50.457999 kafka-broker-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.401922 kafka-broker-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.423970 kafka-broker-0.3.2/src/kafka_broker/
--rw-rw-rw-   0        0        0     4742 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     1999 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.442427 kafka-broker-0.3.2/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2635 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1335 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3192 2024-02-27 08:41:59.000000 kafka-broker-0.3.2/src/kafka_broker/consumer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.450563 kafka-broker-0.3.2/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      598 2023-11-21 13:40:04.000000 kafka-broker-0.3.2/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.2/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.2/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.453288 kafka-broker-0.3.2/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 07:59:50.000000 kafka-broker-0.3.2/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 07:59:50.451617 kafka-broker-0.3.2/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.2/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.159889 kafka-broker-0.3.3/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:12:10.156868 kafka-broker-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 11:12:06.000000 kafka-broker-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:12:10.160879 kafka-broker-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.115631 kafka-broker-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.131554 kafka-broker-0.3.3/src/kafka_broker/
+-rw-rw-rw-   0        0        0     6164 2024-04-05 09:02:03.000000 kafka-broker-0.3.3/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     1997 2024-04-05 08:21:59.000000 kafka-broker-0.3.3/src/kafka_broker/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.148127 kafka-broker-0.3.3/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0      249 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.3/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1790 2024-04-05 08:36:05.000000 kafka-broker-0.3.3/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3229 2024-04-05 08:17:11.000000 kafka-broker-0.3.3/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.3/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.151334 kafka-broker-0.3.3/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.3/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1361 2023-11-21 13:42:05.000000 kafka-broker-0.3.3/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.3/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.155868 kafka-broker-0.3.3/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 11:12:09.000000 kafka-broker-0.3.3/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:12:10.154872 kafka-broker-0.3.3/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.3/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.2/LICENSE` & `kafka-broker-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.2/PKG-INFO` & `kafka-broker-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.2/README.md` & `kafka-broker-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.2/pyproject.toml` & `kafka-broker-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/__init__.py` & `kafka-broker-0.3.3/src/kafka_broker/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import logging
 
 from typing import Any, Callable
+from pydantic import BaseModel
+from typing_extensions import deprecated
 from confluent_kafka import Consumer
 
+from src.kafka_broker.enums import EventStatus
+
 from .cache import Cache
 from .classes import ConsumerStorage, EventObject, EventRouter
 from .consumer import init_consumer, initialize, consume
 from .producer import default_callback, produce
 from .config import get_config
 
 
 class BrokerManager:
     consumer_storage: ConsumerStorage
     cache: Cache
 
     def __init__(self) -> None:
         """Produce to and consume from a kafka message queue."""
-        
+
         filename = "broker_config.ini"
 
         self.consumer = None
         self.config = get_config(filename)
 
         log_level = self.config["logging"]["log_level"]
         logging.basicConfig(format="%(levelname)s:\t%(message)s", level=int(log_level))
@@ -59,25 +63,29 @@
         ## EventObject
         When the producer sends a message to the broker, it tries to
         encode it. If provided in the config, the custom encode function
         must return a key and value pair in the form of a tuple.
         """
         produce(self.config, self.cache, self.logger, topic, event_object, callback)
 
-    def consume(self):
+    def consume(self) -> EventObject | None:
         if not self.consumer:
             kafka_config = self.config["kafka.default"]
             kafka_config.update(self.config["kafka.consumer"])
             self.consumer = Consumer(kafka_config)
             self.consumer.subscribe([self.config["general"]["current_location"]])
         return consume(self.consumer, self.logger)
 
+    @deprecated
     def init_consumer_app(self, app):
         """Setup the consumer on a FastAPI instance.
 
+        It says depricated, but it might still work.
+        It will not be updated anymore.
+
         Parameters
         ----------
         app : FastAPI
             The FastAPI app.
 
         Returns
         -------
@@ -116,27 +124,77 @@
         to not have persisting data which takes up memory.
 
         ### EventObject
         In the config you can define a custome decode function.
         When the consumer receives a message from the broker it tries
         to decode the message before sending it to the ConsumerStorage.
         """
-        app, consumer_storage = init_consumer(self.config, self.logger, self.consumer_storage, app)
+        app, consumer_storage = init_consumer(
+            self.config, self.logger, self.consumer_storage, app
+        )
         self.consumer_storage = consumer_storage
         return app
 
     def init_consumer(self):
-        consuming, consumer_storage = initialize(self.config, self.logger, self.consumer_storage)
+        consuming, consumer_storage = initialize(
+            self.config, self.logger, self.consumer_storage
+        )
         self.consumer_storage = consumer_storage
         return consuming
 
+    def _format_data(data):
+        if isinstance(data, BaseModel):
+            data = data.model_dump()
+
+        elif (
+            isinstance(data, list) and len(data) > 0 and isinstance(data[0], BaseModel)
+        ):
+            data = [d.model_dump() for d in data]
+
+        return data
+
+    def reply(
+        self,
+        event_object: EventObject,
+        status_code: int,
+        msg: str,
+        data: Any = None,
+    ):
+        data = self._format_data(data)
+
+        event_object.data = {
+            "status_code": status_code,
+            "message": msg,
+            "payload": data,
+        }
+
+        event_object.status = EventStatus.COMPLETED
+        event_object.event = "respond"
+
+        self.cache.update(event_object)
+
+    def send(
+        self,
+        event_object: EventObject,
+        module: str,
+        event: str,
+        data: Any = None,
+        **kwargs,
+    ):
+        data = self._format_data(data)
+
+        event_object.event = event
+        event_object.data = {"payload": data, **kwargs}
+
+        self.produce(module, event_object)
+
 
 broker_manager = BrokerManager()
 
 __all__ = [
     "broker_manager",
     "BrokerManager",
     "ConsumerStorage",
     "EventObject",
     "EventRouter",
-    "Cache"
+    "Cache",
 ]
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/cache.py` & `kafka-broker-0.3.3/src/kafka_broker/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from logging import Logger
 from uuid import UUID
 
-from .exceptions.cache import CouldNotEditMemcache, KeyNotFoundException
+from .exceptions.cache import (
+    ConnectionException,
+    CouldNotEditMemcache,
+    KeyNotFoundException,
+)
 from .classes import EventObject
 from pymemcache.client.base import Client
 
 
 class Cache:
     def __init__(self, config, logger: Logger) -> None:
         self.client = self.innitialize_connection(config)
@@ -18,20 +22,18 @@
                 config["memcached"]["cache_location"],
                 config["memcached"]["cache_port"],
             )
         )
         if client is not None:
             return client
         else:
-            raise ConnectionError
+            raise ConnectionException
 
     def add(self, event_object: EventObject):
-        res = self.client.add(
-            str(event_object.correlation_id), event_object.encode()
-        )
+        res = self.client.add(str(event_object.correlation_id), event_object.encode())
         if res is False:
             raise CouldNotEditMemcache
         self.logger.info(f"Added {str(event_object.correlation_id)} to cache.")
 
     def get(self, correlation_id: UUID):
         byte_string = self.get_raw(correlation_id)
         return EventObject.decode(byte_string.decode("utf-8"))
@@ -46,14 +48,12 @@
         res = self.client.delete(str(correlation_id))
         if res is False:
             raise CouldNotEditMemcache
         self.logger.info(f"Deleted {str(correlation_id)} to cache.")
         return res
 
     def update(self, event_object: EventObject):
-        res = self.client.set(
-            str(event_object.correlation_id), event_object.encode()
-        )
+        res = self.client.set(str(event_object.correlation_id), event_object.encode())
         if res is False:
             raise CouldNotEditMemcache
         self.logger.info(f"Updated {str(event_object.correlation_id)} in cache.")
         return res
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.3/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.2/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.3/src/kafka_broker/classes/event_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import uuid
 from pydantic import BaseModel
 
 
 class EventObject:
     def __init__(
         self,
+        *,
         correlation_id: int = None,
         event: str = None,
         data: dict[any] = None,
         status: str = None,
         audit_log: list[dict[str, int, int]] = None,
     ) -> None:
         """Initialize the EventObject:
@@ -45,14 +46,21 @@
             status = "pending"
         self.status = status
 
         if not audit_log:
             audit_log = []
         self.audit_log = audit_log
 
+    def as_reply(self, message: str = "Internal Server Error", status_code: int = 500) -> None:
+        self.data = {
+            "message": message,
+            "status_code": status_code,
+            "payload": self.data
+        }
+
     def encode(self):
         result = {
             "correlation_id": self.correlation_id,
             "status": self.status,
             "event": self.event,
             "data": self.data,
             "audit_log": self.audit_log,
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.3/src/kafka_broker/classes/event_router.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 from typing import Self
+
+from ..enums import EventStatus
 from .event_object import EventObject
+from .. import broker_manager
 
 
 class EventRouter:
     """A simple router.
     Bind events to expose them to the router.
     Bind routers to expand the router.
     """
@@ -24,18 +27,28 @@
         return inner
     
     def include_binder(self, binder: Self):
         self.check_bind(binder.name)
         self.binds[binder.name] = binder
 
     def execute_event(self, event_object: EventObject, events: list[str] = None):
-        if not events:
-            events = event_object.event.split(".")
-
-        for key, func in self.binds.items():
-            if key == events[0]:
-                if isinstance(func, EventRouter):
-                    return func.execute_event(event_object, events[1:])
-                
-                return func(event_object=event_object)
-        else:
-            logging.warning(f"Event '{event_object.event}' not found in '{self.name}'")
+        try:
+            if not events:
+                events = event_object.event.split(".")
+
+            for key, func in self.binds.items():
+                if key == events[0]:
+                    if isinstance(func, EventRouter):
+                        return func.execute_event(event_object, events[1:])
+                    
+                    return func(event_object=event_object)
+            else:
+                logging.warning(f"Event '{event_object.event}' not found in '{self.name}'")
+
+        except Exception as exc:
+            self.exception_handler(exc, event_object)
+
+    def exception_handler(self, exc: Exception, event_object: EventObject):
+        logging.exception(exc)
+        event_object.as_reply()
+        event_object.status = EventStatus.ERROR
+        broker_manager.cache.update(event_object)
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/config.py` & `kafka-broker-0.3.3/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.2/src/kafka_broker/consumer.py` & `kafka-broker-0.3.3/src/kafka_broker/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     except KeyboardInterrupt:
         pass
 
     finally:
         consumer.close()
 
 
-def consume(consumer: Consumer, logger: logging.Logger):
+def consume(consumer: Consumer, logger: logging.Logger) -> EventObject | None:
     """Consumer loop."""
     try:
         while True:
             msg = consumer.poll(1.0)
 
             logger.debug("[*] Waiting...")
 
@@ -98,15 +98,15 @@
             else:
                 return handle(logger, msg)
 
     except KeyboardInterrupt:
         consumer.close()
 
 
-def handle(logger: logging.Logger, msg):
+def handle(logger: logging.Logger, msg) -> EventObject:
     """Handle a non error event."""
     topic = msg.topic()
     key = msg.key().decode("utf-8")
     value = msg.value().decode("utf-8")
 
     logger.info(
         "Consumed - topic {topic}: key = {key} value = {value}".format(
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.3/src/kafka_broker/exceptions/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-
 from http import HTTPStatus
 from .base import CustomException
 
 
-class ConnectionError(CustomException):
-    status_code = 500 
+class ConnectionException(CustomException):
+    status_code = 500
     error_code = "COULD_NOT_INNITIALIZE_CONNECTION"
     message = "The connection could not be established"
 
+
 class KeyNotFoundException(CustomException):
     status_code = HTTPStatus.NOT_FOUND
     error_code = "KEY_NOT_FOUND"
     message = "key not found in memcached"
 
+
 class CouldNotEditMemcache(CustomException):
     status_code = 400
     error_code = "COULD_NOT_EDIT_MEMCACHED"
-    message = "could not add, update or delete the entity in memcached"
+    message = "could not add, update or delete the entity in memcached"
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker/producer.py` & `kafka-broker-0.3.3/src/kafka_broker/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.2/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.3/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.2/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.3/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 src/kafka_broker/__init__.py
 src/kafka_broker/base_config.ini
 src/kafka_broker/cache.py
 src/kafka_broker/config.py
 src/kafka_broker/consumer.py
+src/kafka_broker/enums.py
 src/kafka_broker/producer.py
 src/kafka_broker/py.typed
 src/kafka_broker.egg-info/PKG-INFO
 src/kafka_broker.egg-info/SOURCES.txt
 src/kafka_broker.egg-info/dependency_links.txt
 src/kafka_broker.egg-info/requires.txt
 src/kafka_broker.egg-info/top_level.txt
```

