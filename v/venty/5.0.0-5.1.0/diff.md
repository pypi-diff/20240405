# Comparing `tmp/venty-5.0.0.tar.gz` & `tmp/venty-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venty-5.0.0.tar", last modified: Wed Mar 27 06:57:51 2024, max compression
+gzip compressed data, was "venty-5.1.0.tar", last modified: Fri Apr  5 05:11:10 2024, max compression
```

## Comparing `venty-5.0.0.tar` & `venty-5.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:57:51.544027 venty-5.0.0/
--rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-5.0.0/LICENSE
--rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2120 2024-03-27 06:57:51.543027 venty-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2024-03-16 17:46:39.000000 venty-5.0.0/README.md
--rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-5.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 06:57:51.544027 venty-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2021 2024-03-27 06:33:31.000000 venty-5.0.0/setup.py
--rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-5.0.0/test_requirements.txt
--rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-5.0.0/tox.ini
-drwxrwxrwx   0        0        0        0 2024-03-27 06:57:51.532027 venty-5.0.0/venty/
--rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-5.0.0/venty/__init__.py
--rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-5.0.0/venty/_dummy.py
--rw-rw-rw-   0        0        0     1693 2024-03-26 00:45:31.000000 venty-5.0.0/venty/aggregate_root.py
--rw-rw-rw-   0        0        0     1220 2024-03-26 00:47:56.000000 venty-5.0.0/venty/aggregate_store.py
--rw-rw-rw-   0        0        0     2123 2024-03-27 06:14:06.000000 venty-5.0.0/venty/aggregate_store_test.py
--rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-5.0.0/venty/event_channel.py
--rw-rw-rw-   0        0        0      521 2024-03-16 16:58:05.000000 venty-5.0.0/venty/event_channel_test.py
--rw-rw-rw-   0        0        0     5036 2024-03-27 06:20:52.000000 venty-5.0.0/venty/event_logger.py
--rw-rw-rw-   0        0        0     2081 2024-03-27 06:38:20.000000 venty-5.0.0/venty/event_producer.py
--rw-rw-rw-   0        0        0     1366 2024-03-27 06:39:25.000000 venty-5.0.0/venty/event_producer_stack.py
--rw-rw-rw-   0        0        0     1435 2024-03-27 06:37:35.000000 venty-5.0.0/venty/event_producer_stack_test.py
--rw-rw-rw-   0        0        0      848 2024-03-27 06:35:25.000000 venty-5.0.0/venty/event_producer_test.py
--rw-rw-rw-   0        0        0     6996 2024-03-16 15:40:44.000000 venty-5.0.0/venty/event_store.py
--rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-5.0.0/venty/http_event_channel.py
--rw-rw-rw-   0        0        0     1850 2024-03-16 17:18:33.000000 venty-5.0.0/venty/http_event_channel_test.py
--rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-5.0.0/venty/in_memory_event_channel.py
--rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-5.0.0/venty/in_memory_event_channel_test.py
--rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-5.0.0/venty/in_memory_event_store.py
--rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-5.0.0/venty/in_memory_event_store_test.py
--rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-5.0.0/venty/py.typed
--rw-rw-rw-   0        0        0      509 2024-03-16 15:58:02.000000 venty-5.0.0/venty/settings.py
--rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-5.0.0/venty/settings_test.py
--rw-rw-rw-   0        0        0     8535 2024-03-26 00:16:29.000000 venty-5.0.0/venty/sql_event_store.py
--rw-rw-rw-   0        0        0     6821 2024-03-16 22:24:29.000000 venty-5.0.0/venty/sql_event_store_test.py
--rw-rw-rw-   0        0        0      287 2024-03-16 17:21:51.000000 venty-5.0.0/venty/strong_types.py
--rw-rw-rw-   0        0        0     1003 2024-03-15 19:20:28.000000 venty-5.0.0/venty/strong_types_test.py
--rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-5.0.0/venty/timing.py
--rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-5.0.0/venty/timing_test.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:57:51.543027 venty-5.0.0/venty.egg-info/
--rw-rw-rw-   0        0        0     2120 2024-03-27 06:57:51.000000 venty-5.0.0/venty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-03-27 06:57:51.000000 venty-5.0.0/venty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:57:51.000000 venty-5.0.0/venty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-03-27 06:57:51.000000 venty-5.0.0/venty.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-27 06:57:51.000000 venty-5.0.0/venty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 05:11:10.086174 venty-5.1.0/
+-rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-5.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2120 2024-04-05 05:11:10.086174 venty-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2024-03-16 17:46:39.000000 venty-5.1.0/README.md
+-rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-5.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 05:11:10.086174 venty-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2021 2024-04-05 05:05:23.000000 venty-5.1.0/setup.py
+-rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-5.1.0/test_requirements.txt
+-rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-5.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-05 05:11:10.073411 venty-5.1.0/venty/
+-rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-5.1.0/venty/__init__.py
+-rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-5.1.0/venty/_dummy.py
+-rw-rw-rw-   0        0        0     1693 2024-03-26 00:45:31.000000 venty-5.1.0/venty/aggregate_root.py
+-rw-rw-rw-   0        0        0     1220 2024-03-26 00:47:56.000000 venty-5.1.0/venty/aggregate_store.py
+-rw-rw-rw-   0        0        0     2123 2024-03-27 06:14:06.000000 venty-5.1.0/venty/aggregate_store_test.py
+-rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-5.1.0/venty/event_channel.py
+-rw-rw-rw-   0        0        0      521 2024-03-16 16:58:05.000000 venty-5.1.0/venty/event_channel_test.py
+-rw-rw-rw-   0        0        0     5036 2024-03-27 06:20:52.000000 venty-5.1.0/venty/event_logger.py
+-rw-rw-rw-   0        0        0     2986 2024-04-05 04:27:52.000000 venty-5.1.0/venty/event_producer.py
+-rw-rw-rw-   0        0        0     1544 2024-04-05 05:09:43.000000 venty-5.1.0/venty/event_producer_stack.py
+-rw-rw-rw-   0        0        0     1435 2024-03-27 06:37:35.000000 venty-5.1.0/venty/event_producer_stack_test.py
+-rw-rw-rw-   0        0        0     1419 2024-04-05 04:27:59.000000 venty-5.1.0/venty/event_producer_test.py
+-rw-rw-rw-   0        0        0     6996 2024-03-16 15:40:44.000000 venty-5.1.0/venty/event_store.py
+-rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-5.1.0/venty/http_event_channel.py
+-rw-rw-rw-   0        0        0     1850 2024-03-16 17:18:33.000000 venty-5.1.0/venty/http_event_channel_test.py
+-rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-5.1.0/venty/in_memory_event_channel.py
+-rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-5.1.0/venty/in_memory_event_channel_test.py
+-rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-5.1.0/venty/in_memory_event_store.py
+-rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-5.1.0/venty/in_memory_event_store_test.py
+-rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-5.1.0/venty/py.typed
+-rw-rw-rw-   0        0        0      509 2024-03-16 15:58:02.000000 venty-5.1.0/venty/settings.py
+-rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-5.1.0/venty/settings_test.py
+-rw-rw-rw-   0        0        0     8535 2024-03-26 00:16:29.000000 venty-5.1.0/venty/sql_event_store.py
+-rw-rw-rw-   0        0        0     6821 2024-03-16 22:24:29.000000 venty-5.1.0/venty/sql_event_store_test.py
+-rw-rw-rw-   0        0        0      287 2024-03-16 17:21:51.000000 venty-5.1.0/venty/strong_types.py
+-rw-rw-rw-   0        0        0     1003 2024-03-15 19:20:28.000000 venty-5.1.0/venty/strong_types_test.py
+-rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-5.1.0/venty/timing.py
+-rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-5.1.0/venty/timing_test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:11:10.084631 venty-5.1.0/venty.egg-info/
+-rw-rw-rw-   0        0        0     2120 2024-04-05 05:11:09.000000 venty-5.1.0/venty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2024-04-05 05:11:09.000000 venty-5.1.0/venty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 05:11:09.000000 venty-5.1.0/venty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-05 05:11:09.000000 venty-5.1.0/venty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 05:11:09.000000 venty-5.1.0/venty.egg-info/top_level.txt
```

### Comparing `venty-5.0.0/LICENSE` & `venty-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/PKG-INFO` & `venty-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 5.0.0
+Version: 5.1.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Alexander Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-5.0.0/README.md` & `venty-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/setup.py` & `venty-5.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 here = Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setuptools.setup(
         name="venty",
-        version="5.0.0",
+        version="5.1.0",
         author="Alexander Tkachev",
         author_email="sasha64sasha@gmail.com",
         description="Venty",
         long_description_content_type="text/markdown",
         long_description=long_description,
         home_page="https://github.com/sasha-tkachev/venty",
         url="https://github.com/sasha-tkachev/venty",
```

### Comparing `venty-5.0.0/tox.ini` & `venty-5.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/aggregate_root.py` & `venty-5.1.0/venty/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/aggregate_store.py` & `venty-5.1.0/venty/aggregate_store.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/aggregate_store_test.py` & `venty-5.1.0/venty/aggregate_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/event_channel.py` & `venty-5.1.0/venty/event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/event_channel_test.py` & `venty-5.1.0/venty/event_channel_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/event_logger.py` & `venty-5.1.0/venty/event_logger.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/event_producer.py` & `venty-5.1.0/venty/event_producer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from datetime import datetime
+import sys
+from datetime import datetime, timezone
 from typing import Any, Dict, Optional, Callable, TypeVar
-from uuid import uuid4
+from uuid import uuid4, UUID, uuid5
 
 from cloudevents.pydantic import CloudEvent
 from cloudevents.sdk.event.attribute import (
     default_id_selection_algorithm,
     default_time_selection_algorithm,
 )
 
@@ -27,14 +28,32 @@
     ) -> CloudEvent:
         raise NotImplementedError()
 
 
 EventProducerT = TypeVar("EventProducerT", bound=EventProducer)
 
 
+def deterministic_id_factory(seed: int = 0) -> Callable[[], str]:
+    i = iter(range(sys.maxsize))
+
+    def _next() -> str:
+        return str(uuid5(UUID(int=seed), str(next(i))))
+
+    return _next
+
+
+def deterministic_time_factory() -> Callable[[], datetime]:
+    i = iter(range(sys.maxsize))
+
+    def _next() -> datetime:
+        return datetime.fromtimestamp(next(i), tz=timezone.utc)
+
+    return _next
+
+
 class SimpleEventProducer(EventProducer):
     def __init__(
         self,
         *,
         source: Optional[EventSource] = None,
         default_attributes: Optional[Dict[str, Any]] = None,
         id_selection_algorithm: IdSelection = default_id_selection_algorithm,
@@ -54,7 +73,21 @@
     ) -> CloudEvent:
         actual_attributes = self._default_attributes.copy()
         actual_attributes.update(attributes)
         actual_attributes["source"] = self._source
         actual_attributes["id"] = self._id_selection_algorithm()
         actual_attributes["time"] = self._time_selection_algorithm()
         return CloudEvent.create(actual_attributes, data)
+
+
+def testing_event_producer(
+    *,
+    source: Optional[EventSource] = EventSource("fake-source"),
+    default_attributes: Optional[Dict[str, Any]] = None,
+    seed: int = 0,
+) -> EventProducer:
+    return SimpleEventProducer(
+        source=source,
+        default_attributes=default_attributes,
+        id_selection_algorithm=deterministic_id_factory(seed),
+        time_selection_algorithm=deterministic_time_factory(),
+    )
```

### Comparing `venty-5.0.0/venty/event_producer_stack.py` & `venty-5.1.0/venty/event_producer_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 
 from cloudevents.pydantic import CloudEvent
 
 from venty.event_producer import EventProducer, EventProducerT
 from collections import OrderedDict
 from uuid import uuid4, UUID
 from contextlib import contextmanager
+import sys
 
+if sys.version_info < (3, 9):
+    from typing import OrderedDict as OrderedDictType
 
-EventProducers = OrderedDict[UUID, Optional[EventProducer]]
+    EventProducers = OrderedDictType[UUID, Optional[EventProducer]]
+else:
+    EventProducers = OrderedDict[UUID, Optional[EventProducer]]
 
 
 def _last(event_producers: EventProducers) -> EventProducer:
     # it is O(1)
     # https://stackoverflow.com/questions/9917178/last-element-in-ordereddict
     _, last_value = next(reversed(event_producers.items()))
     return last_value
```

### Comparing `venty-5.0.0/venty/event_producer_stack_test.py` & `venty-5.1.0/venty/event_producer_stack_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/event_producer_test.py` & `venty-5.1.0/venty/event_producer_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 from cloudevents.conversion import to_dict
 
 
-from venty.event_producer import SimpleEventProducer
+from venty.event_producer import SimpleEventProducer, testing_event_producer
 from venty.strong_types import EventSource
 
 
 def test_event_producer_sanity():
     producer = SimpleEventProducer(
         source=EventSource("my-source"),
         id_selection_algorithm=lambda: "1",
@@ -22,7 +22,25 @@
         "id": "1",
         "source": "my-source",
         "specversion": "1.0",
         "subject": "hello",
         "time": "2024-01-01T00:00:00",
         "type": "my-type",
     }
+
+
+def test_fake_event_producer():
+    producer = testing_event_producer(
+        default_attributes={"subject": "hello"},
+    )
+    result = producer.produce_event({"type": "my-type"}, None)
+    assert to_dict(result) == {
+        "data": None,
+        "datacontenttype": None,
+        "dataschema": None,
+        "id": "b6c54489-38a0-5f50-a60a-fd8d76219cae",
+        "source": "fake-source",
+        "specversion": "1.0",
+        "subject": "hello",
+        "time": "1970-01-01T00:00:00+00:00",
+        "type": "my-type",
+    }
```

### Comparing `venty-5.0.0/venty/event_store.py` & `venty-5.1.0/venty/event_store.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/http_event_channel.py` & `venty-5.1.0/venty/http_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/http_event_channel_test.py` & `venty-5.1.0/venty/http_event_channel_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/in_memory_event_channel.py` & `venty-5.1.0/venty/in_memory_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/in_memory_event_store.py` & `venty-5.1.0/venty/in_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/in_memory_event_store_test.py` & `venty-5.1.0/venty/in_memory_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/settings_test.py` & `venty-5.1.0/venty/settings_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/sql_event_store.py` & `venty-5.1.0/venty/sql_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/sql_event_store_test.py` & `venty-5.1.0/venty/sql_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/strong_types_test.py` & `venty-5.1.0/venty/strong_types_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/timing.py` & `venty-5.1.0/venty/timing.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty/timing_test.py` & `venty-5.1.0/venty/timing_test.py`

 * *Files identical despite different names*

### Comparing `venty-5.0.0/venty.egg-info/PKG-INFO` & `venty-5.1.0/venty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 5.0.0
+Version: 5.1.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Alexander Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-5.0.0/venty.egg-info/SOURCES.txt` & `venty-5.1.0/venty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

