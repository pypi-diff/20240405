# Comparing `tmp/robotframework-confluentkafkalibrary-2.0.2.post3.tar.gz` & `tmp/robotframework-confluentkafkalibrary-2.0.2.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post3.tar", last modified: Sun Jan 21 20:12:31 2024, max compression
+gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post4.tar", last modified: Thu Apr  4 22:05:32 2024, max compression
```

## Comparing `robotframework-confluentkafkalibrary-2.0.2.post3.tar` & `robotframework-confluentkafkalibrary-2.0.2.post4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:12:31.317817 robotframework-confluentkafkalibrary-2.0.2.post3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-21 20:12:31.317817 robotframework-confluentkafkalibrary-2.0.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 20:12:31.317817 robotframework-confluentkafkalibrary-2.0.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:12:31.313817 robotframework-confluentkafkalibrary-2.0.2.post3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:12:31.313817 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15921 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-21 20:12:19.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:12:31.317817 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-21 20:12:31.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-21 20:12:31.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 20:12:31.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-21 20:12:31.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-21 20:12:31.000000 robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.013607 robotframework-confluentkafkalibrary-2.0.2.post4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/LICENSE` & `robotframework-confluentkafkalibrary-2.0.2.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post3
+Version: 2.0.2.post4
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/README.md` & `robotframework-confluentkafkalibrary-2.0.2.post4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/setup.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/__init__.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/admin_client.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/admin_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/consumer.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,16 @@
         """
         if group_id is None:
             group_id = str(uuid.uuid4())
         if topics is None:
             raise ValueError("Topics can not be empty!")
 
         consumer_thread = GetMessagesThread(server, port, topics, group_id=group_id, only_value=only_value, **kwargs)
+        group_id = consumer_thread.group_id
+        self.consumers[group_id] = consumer_thread.consumer.consumers[group_id]
         return consumer_thread
 
     def get_messages_from_thread(self, running_thread, decode_format=None):
         """Returns all records gathered from specific thread
         - ``running_thread`` (Thread object) - thread which was executed with
             `Start Consumer Threaded` keyword
         - ``decode_format`` (str) - If you need to decode data to specific format
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/producer.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/producer.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/ConfluentKafkaLibrary/serialization.py` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/serialization.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post3
+Version: 2.0.2.post4
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post3/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

