# Comparing `tmp/kafka-broker-0.3.5.tar.gz` & `tmp/kafka-broker-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-broker-0.3.5.tar", last modified: Fri Apr  5 11:52:45 2024, max compression
+gzip compressed data, was "kafka-broker-0.3.6.tar", last modified: Fri Apr  5 11:57:07 2024, max compression
```

## Comparing `kafka-broker-0.3.5.tar` & `kafka-broker-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.240556 kafka-broker-0.3.5/
--rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:52:45.236547 kafka-broker-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/README.md
--rw-rw-rw-   0        0        0      851 2024-04-05 11:52:42.000000 kafka-broker-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 11:52:45.241558 kafka-broker-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.160654 kafka-broker-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.195900 kafka-broker-0.3.5/src/kafka_broker/
--rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.5/src/kafka_broker/__init__.py
--rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/base_config.ini
--rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.5/src/kafka_broker/broker_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.218036 kafka-broker-0.3.5/src/kafka_broker/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.5/src/kafka_broker/classes/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.5/src/kafka_broker/classes/cache.py
--rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/src/kafka_broker/classes/consumer_storage.py
--rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.5/src/kafka_broker/classes/event_object.py
--rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.5/src/kafka_broker/classes/event_router.py
--rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/src/kafka_broker/config.py
--rw-rw-rw-   0        0        0     3243 2024-04-05 11:50:46.000000 kafka-broker-0.3.5/src/kafka_broker/consumer.py
--rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.5/src/kafka_broker/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.228029 kafka-broker-0.3.5/src/kafka_broker/exceptions/
--rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/__init__.py
--rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/base.py
--rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.5/src/kafka_broker/exceptions/cache.py
--rw-rw-rw-   0        0        0     1382 2024-04-05 11:51:06.000000 kafka-broker-0.3.5/src/kafka_broker/producer.py
--rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.5/src/kafka_broker/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.233528 kafka-broker-0.3.5/src/kafka_broker.egg-info/
--rw-rw-rw-   0        0        0     4264 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 11:52:44.000000 kafka-broker-0.3.5/src/kafka_broker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 11:52:45.231017 kafka-broker-0.3.5/tests/
--rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.5/tests/test_event_object.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.396316 kafka-broker-0.3.6/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 13:02:13.000000 kafka-broker-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:57:07.394306 kafka-broker-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-11-10 08:57:39.000000 kafka-broker-0.3.6/README.md
+-rw-rw-rw-   0        0        0      851 2024-04-05 11:56:18.000000 kafka-broker-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:57:07.397031 kafka-broker-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-02-27 08:41:59.000000 kafka-broker-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.328671 kafka-broker-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.359228 kafka-broker-0.3.6/src/kafka_broker/
+-rw-rw-rw-   0        0        0      385 2024-04-05 11:50:25.000000 kafka-broker-0.3.6/src/kafka_broker/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-11-21 13:40:04.000000 kafka-broker-0.3.6/src/kafka_broker/base_config.ini
+-rw-rw-rw-   0        0        0     6032 2024-04-05 11:51:35.000000 kafka-broker-0.3.6/src/kafka_broker/broker_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.382929 kafka-broker-0.3.6/src/kafka_broker/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 11:48:50.000000 kafka-broker-0.3.6/src/kafka_broker/classes/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-04-05 11:38:52.000000 kafka-broker-0.3.6/src/kafka_broker/classes/cache.py
+-rw-rw-rw-   0        0        0     2190 2023-11-10 08:57:39.000000 kafka-broker-0.3.6/src/kafka_broker/classes/consumer_storage.py
+-rw-rw-rw-   0        0        0     2888 2024-04-05 08:36:09.000000 kafka-broker-0.3.6/src/kafka_broker/classes/event_object.py
+-rw-rw-rw-   0        0        0     1804 2024-04-05 11:48:32.000000 kafka-broker-0.3.6/src/kafka_broker/classes/event_router.py
+-rw-rw-rw-   0        0        0     1167 2023-11-10 08:57:39.000000 kafka-broker-0.3.6/src/kafka_broker/config.py
+-rw-rw-rw-   0        0        0     3237 2024-04-05 11:56:59.000000 kafka-broker-0.3.6/src/kafka_broker/consumer.py
+-rw-rw-rw-   0        0        0      184 2024-04-05 08:27:51.000000 kafka-broker-0.3.6/src/kafka_broker/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.388211 kafka-broker-0.3.6/src/kafka_broker/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-11-21 13:40:04.000000 kafka-broker-0.3.6/src/kafka_broker/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-11-21 13:40:04.000000 kafka-broker-0.3.6/src/kafka_broker/exceptions/base.py
+-rw-rw-rw-   0        0        0      605 2024-04-05 08:22:05.000000 kafka-broker-0.3.6/src/kafka_broker/exceptions/cache.py
+-rw-rw-rw-   0        0        0     1371 2024-04-05 11:56:46.000000 kafka-broker-0.3.6/src/kafka_broker/producer.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:49:08.000000 kafka-broker-0.3.6/src/kafka_broker/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.392483 kafka-broker-0.3.6/src/kafka_broker.egg-info/
+-rw-rw-rw-   0        0        0     4264 2024-04-05 11:57:07.000000 kafka-broker-0.3.6/src/kafka_broker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2024-04-05 11:57:07.000000 kafka-broker-0.3.6/src/kafka_broker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:57:07.000000 kafka-broker-0.3.6/src/kafka_broker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-05 11:57:07.000000 kafka-broker-0.3.6/src/kafka_broker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 11:57:07.000000 kafka-broker-0.3.6/src/kafka_broker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 11:57:07.390351 kafka-broker-0.3.6/tests/
+-rw-rw-rw-   0        0        0      356 2023-11-10 08:57:39.000000 kafka-broker-0.3.6/tests/test_event_object.py
```

### Comparing `kafka-broker-0.3.5/LICENSE` & `kafka-broker-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/PKG-INFO` & `kafka-broker-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.5/README.md` & `kafka-broker-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/pyproject.toml` & `kafka-broker-0.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kafka-broker"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Tijmen Simons", email="tijmen.simons@student.hu.nl" },
   { name="Ivar Stek", email="ivar.stek@student.hu.nl" },
 ]
 description = "A python package implementation for the confluent kafka package. Managing producing and consuming."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `kafka-broker-0.3.5/src/kafka_broker/broker_manager.py` & `kafka-broker-0.3.6/src/kafka_broker/broker_manager.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/classes/cache.py` & `kafka-broker-0.3.6/src/kafka_broker/classes/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/classes/consumer_storage.py` & `kafka-broker-0.3.6/src/kafka_broker/classes/consumer_storage.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/classes/event_object.py` & `kafka-broker-0.3.6/src/kafka_broker/classes/event_object.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/classes/event_router.py` & `kafka-broker-0.3.6/src/kafka_broker/classes/event_router.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/config.py` & `kafka-broker-0.3.6/src/kafka_broker/config.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/consumer.py` & `kafka-broker-0.3.6/src/kafka_broker/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     """Handle a non error event."""
     topic = msg.topic()
     key = msg.key().decode("utf-8")
     value = msg.value().decode("utf-8")
 
     logger.info(
         "Consumed - topic {topic}: key = {key} value = {value}".format(
-            topic=topic, key=key, value=f"{value[:200]}..."
+            topic=topic, key=key, value=f"{value}..."
         )
     )
 
     obj: EventObject = EventObject.decode(value)
     obj.update_audit_log()
     return obj
```

### Comparing `kafka-broker-0.3.5/src/kafka_broker/exceptions/cache.py` & `kafka-broker-0.3.6/src/kafka_broker/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `kafka-broker-0.3.5/src/kafka_broker/producer.py` & `kafka-broker-0.3.6/src/kafka_broker/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         cache.update(event_object)
     except KeyNotFoundException:
         cache.add(event_object)
 
     logger.info(
         "Produced - topic {topic}: key = {key} value = {value}".format(
             topic=topic,
-            key=f"{str(event_object.correlation_id)[:16]}...",
-            value=f"{event_json[:100]}...",
+            key=f"{str(event_object.correlation_id)}...",
+            value=f"{event_json}...",
         )
     )
```

### Comparing `kafka-broker-0.3.5/src/kafka_broker.egg-info/PKG-INFO` & `kafka-broker-0.3.6/src/kafka_broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-broker
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python package implementation for the confluent kafka package. Managing producing and consuming.
 Author-email: Tijmen Simons <tijmen.simons@student.hu.nl>, Ivar Stek <ivar.stek@student.hu.nl>
 Project-URL: Homepage, https://github.com/TijmenSimons/kafka-broker
 Project-URL: Bug Tracker, https://github.com/TijmenSimons/kafka-broker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kafka-broker-0.3.5/src/kafka_broker.egg-info/SOURCES.txt` & `kafka-broker-0.3.6/src/kafka_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

