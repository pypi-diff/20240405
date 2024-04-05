# Comparing `tmp/Torrelque-0.6.0.tar.gz` & `tmp/Torrelque-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Torrelque-0.6.0.tar", last modified: Sat May 28 13:08:33 2022, max compression
+gzip compressed data, was "Torrelque-0.7.0.tar", last modified: Fri Apr  5 11:27:37 2024, max compression
```

## Comparing `Torrelque-0.6.0.tar` & `Torrelque-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 13:08:33.777058 Torrelque-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     4559 2022-05-28 13:08:33.773058 Torrelque-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3428 2021-11-27 15:46:38.000000 Torrelque-0.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 13:08:33.773058 Torrelque-0.6.0/Torrelque.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4559 2022-05-28 13:08:33.000000 Torrelque-0.6.0/Torrelque.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2022-05-28 13:08:33.000000 Torrelque-0.6.0/Torrelque.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-28 13:08:33.000000 Torrelque-0.6.0/Torrelque.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2022-05-28 13:08:33.000000 Torrelque-0.6.0/Torrelque.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-05-28 13:08:33.000000 Torrelque-0.6.0/Torrelque.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-28 13:08:33.777058 Torrelque-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1630 2022-05-28 13:00:11.000000 Torrelque-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-28 13:08:33.773058 Torrelque-0.6.0/torrelque/
--rw-rw-rw-   0 root         (0) root         (0)    24632 2021-11-27 16:36:06.000000 Torrelque-0.6.0/torrelque/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2021-10-18 20:54:58.000000 Torrelque-0.6.0/torrelque/dequeue.lua
--rw-rw-rw-   0 root         (0) root         (0)     2398 2021-10-18 20:54:58.000000 Torrelque-0.6.0/torrelque/sweep.lua
--rw-rw-rw-   0 root         (0) root         (0)    49110 2021-11-27 19:06:18.000000 Torrelque-0.6.0/torrelque/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:27:37.591527 Torrelque-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     4536 2024-04-05 11:27:37.587527 Torrelque-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-04-05 10:02:06.000000 Torrelque-0.7.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:27:37.587527 Torrelque-0.7.0/Torrelque.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4536 2024-04-05 11:27:37.000000 Torrelque-0.7.0/Torrelque.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-05 11:27:37.000000 Torrelque-0.7.0/Torrelque.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 11:27:37.000000 Torrelque-0.7.0/Torrelque.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-05 11:27:37.000000 Torrelque-0.7.0/Torrelque.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-05 11:27:37.000000 Torrelque-0.7.0/Torrelque.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 11:27:37.591527 Torrelque-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2024-04-05 11:09:49.000000 Torrelque-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 11:27:37.587527 Torrelque-0.7.0/torrelque/
+-rw-rw-rw-   0 root         (0) root         (0)    24774 2024-04-05 11:00:05.000000 Torrelque-0.7.0/torrelque/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2021-10-18 20:54:58.000000 Torrelque-0.7.0/torrelque/dequeue.lua
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2021-10-18 20:54:58.000000 Torrelque-0.7.0/torrelque/sweep.lua
+-rw-rw-rw-   0 root         (0) root         (0)    49386 2024-04-05 11:00:05.000000 Torrelque-0.7.0/torrelque/test.py
```

### Comparing `Torrelque-0.6.0/PKG-INFO` & `Torrelque-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: Torrelque
-Version: 0.6.0
+Version: 0.7.0
 Summary: Asynchronous Redis-backed reliable queue package
 Home-page: https://heptapod.host/saajns/torrelque
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/torrelque
 Project-URL: Documentation, https://torrelque.readthedocs.io/
 Project-URL: Release Notes, https://torrelque.readthedocs.io/en/latest/history.html
 Keywords: python redis asynchronous job-queue work-queue
 Platform: Any
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
-Provides-Extra: test
+Requires-Python: >= 3
+Requires-Dist: redis>=5.0.1
 Provides-Extra: manual
+Requires-Dist: sphinx<8,>=7; extra == "manual"
 
 .. image:: https://img.shields.io/pypi/l/Torrelque.svg
    :target: https://spdx.org/licenses/LGPL-3.0-only.html
    :alt: PyPI - License
 .. image:: https://heptapod.host/saajns/torrelque/badges/branch/default/pipeline.svg
    :target: https://heptapod.host/saajns/torrelque/-/commits/branch/default
    :alt: Pipeline status
@@ -41,48 +44,45 @@
    :target: https://torrelque.readthedocs.io/en/latest/?badge=latest
    :alt: RTFD
 
 *********
 Torrelque
 *********
 Torrelque is a Python package that provides minimal asynchronous reliable
-distributed Redis-backed work queues. It is built:
+distributed Redis-backed (or a protocol-compatible alternative) work queues.
+It is built:
 
 1. Lock-free. It relies on Redis transactions and its single-threaded
    execution model.
 2. Poll-free. Waiting subset of the Python API relies either on blocking Redis
    commands or notifications.
 3. Bulk-friendly. Tasks can be produced and consumed in bulk.
 4. Introspectable. Task stats, task status transition watching API, and
    the data model comprehensible directly in Redis.
 
-.. note::
-
-   Prior to version 0.2 Torrelque was Tornado-specific. Since version 5 Tornado
-   runs on ``asyncio`` event loop by default, hence newer Torrelque is still
-   compatible with (newer) Tornado, even though it's based on ``asyncio`` now.
-
 Install
 =======
 ::
 
    pip install Torrelque
 
+Supported Redis server implementations: Redis, KeyDB.
+
 Quickstart
 ==========
 Producer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
    queue = torrelque.Torrelque(redis, queue='email')
    queue.schedule_sweep()
 
    task_data = {'addr': 'joe@doe.com', 'subj': 'hello', 'body': '...'}
-   task_id = await queue.enqueue(task)
+   task_id = await queue.enqueue(task_data)
    logger.info('Email task enqueued %s', task_id)
 
 Consumer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
@@ -94,27 +94,24 @@
            await some_email_client.send(**task_data)
        except SomeEmailError:
            logger.exception('Sending error, retrying in 30 seconds')
            await queue.requeue(task_id, delay=30)
        else:
            await queue.release(task_id)
 
-
 Example list
 ============
 - `Producer-consumer <e1_>`_. Infinite producing and consuming loops.
 - `Batch processing <e2_>`_. Finite number of tasks, consumers stop with a
   poison pill, bulk enqueue. This example can be used as a synthetic benchmark.
   Because there's no IO-bound workload, it'll be CPU-bound which isn't normal
   mode of operation for an asynchronous application. But it can be used to
   compare between CPython, PyPy and concurrency parameters.
 - `Web application background task <e3_>`_. This tornado application allows
   to start a task and push server-sent events (SSE) to UI about its status. UI
-  starts a task and waits for it to complete. When a task fails it's requeued
+  starts a task and waits for it to complete. When a task fails it's re-queued
   with exponential back-off.
 
 
 .. _e1: https://heptapod.host/saajns/torrelque/blob/branch/default/example/producer_consumer.py
 .. _e2: https://heptapod.host/saajns/torrelque/blob/branch/default/example/batch_processing.py
 .. _e3: https://heptapod.host/saajns/torrelque/blob/branch/default/example/wait_until_complete.py
-
-
```

### Comparing `Torrelque-0.6.0/README.rst` & `Torrelque-0.7.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,48 +14,45 @@
    :target: https://torrelque.readthedocs.io/en/latest/?badge=latest
    :alt: RTFD
 
 *********
 Torrelque
 *********
 Torrelque is a Python package that provides minimal asynchronous reliable
-distributed Redis-backed work queues. It is built:
+distributed Redis-backed (or a protocol-compatible alternative) work queues.
+It is built:
 
 1. Lock-free. It relies on Redis transactions and its single-threaded
    execution model.
 2. Poll-free. Waiting subset of the Python API relies either on blocking Redis
    commands or notifications.
 3. Bulk-friendly. Tasks can be produced and consumed in bulk.
 4. Introspectable. Task stats, task status transition watching API, and
    the data model comprehensible directly in Redis.
 
-.. note::
-
-   Prior to version 0.2 Torrelque was Tornado-specific. Since version 5 Tornado
-   runs on ``asyncio`` event loop by default, hence newer Torrelque is still
-   compatible with (newer) Tornado, even though it's based on ``asyncio`` now.
-
 Install
 =======
 ::
 
    pip install Torrelque
 
+Supported Redis server implementations: Redis, KeyDB.
+
 Quickstart
 ==========
 Producer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
    queue = torrelque.Torrelque(redis, queue='email')
    queue.schedule_sweep()
 
    task_data = {'addr': 'joe@doe.com', 'subj': 'hello', 'body': '...'}
-   task_id = await queue.enqueue(task)
+   task_id = await queue.enqueue(task_data)
    logger.info('Email task enqueued %s', task_id)
 
 Consumer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
@@ -67,25 +64,24 @@
            await some_email_client.send(**task_data)
        except SomeEmailError:
            logger.exception('Sending error, retrying in 30 seconds')
            await queue.requeue(task_id, delay=30)
        else:
            await queue.release(task_id)
 
-
 Example list
 ============
 - `Producer-consumer <e1_>`_. Infinite producing and consuming loops.
 - `Batch processing <e2_>`_. Finite number of tasks, consumers stop with a
   poison pill, bulk enqueue. This example can be used as a synthetic benchmark.
   Because there's no IO-bound workload, it'll be CPU-bound which isn't normal
   mode of operation for an asynchronous application. But it can be used to
   compare between CPython, PyPy and concurrency parameters.
 - `Web application background task <e3_>`_. This tornado application allows
   to start a task and push server-sent events (SSE) to UI about its status. UI
-  starts a task and waits for it to complete. When a task fails it's requeued
+  starts a task and waits for it to complete. When a task fails it's re-queued
   with exponential back-off.
 
 
 .. _e1: https://heptapod.host/saajns/torrelque/blob/branch/default/example/producer_consumer.py
 .. _e2: https://heptapod.host/saajns/torrelque/blob/branch/default/example/batch_processing.py
 .. _e3: https://heptapod.host/saajns/torrelque/blob/branch/default/example/wait_until_complete.py
```

### Comparing `Torrelque-0.6.0/Torrelque.egg-info/PKG-INFO` & `Torrelque-0.7.0/Torrelque.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: Torrelque
-Version: 0.6.0
+Version: 0.7.0
 Summary: Asynchronous Redis-backed reliable queue package
 Home-page: https://heptapod.host/saajns/torrelque
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/torrelque
 Project-URL: Documentation, https://torrelque.readthedocs.io/
 Project-URL: Release Notes, https://torrelque.readthedocs.io/en/latest/history.html
 Keywords: python redis asynchronous job-queue work-queue
 Platform: Any
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
-Provides-Extra: test
+Requires-Python: >= 3
+Requires-Dist: redis>=5.0.1
 Provides-Extra: manual
+Requires-Dist: sphinx<8,>=7; extra == "manual"
 
 .. image:: https://img.shields.io/pypi/l/Torrelque.svg
    :target: https://spdx.org/licenses/LGPL-3.0-only.html
    :alt: PyPI - License
 .. image:: https://heptapod.host/saajns/torrelque/badges/branch/default/pipeline.svg
    :target: https://heptapod.host/saajns/torrelque/-/commits/branch/default
    :alt: Pipeline status
@@ -41,48 +44,45 @@
    :target: https://torrelque.readthedocs.io/en/latest/?badge=latest
    :alt: RTFD
 
 *********
 Torrelque
 *********
 Torrelque is a Python package that provides minimal asynchronous reliable
-distributed Redis-backed work queues. It is built:
+distributed Redis-backed (or a protocol-compatible alternative) work queues.
+It is built:
 
 1. Lock-free. It relies on Redis transactions and its single-threaded
    execution model.
 2. Poll-free. Waiting subset of the Python API relies either on blocking Redis
    commands or notifications.
 3. Bulk-friendly. Tasks can be produced and consumed in bulk.
 4. Introspectable. Task stats, task status transition watching API, and
    the data model comprehensible directly in Redis.
 
-.. note::
-
-   Prior to version 0.2 Torrelque was Tornado-specific. Since version 5 Tornado
-   runs on ``asyncio`` event loop by default, hence newer Torrelque is still
-   compatible with (newer) Tornado, even though it's based on ``asyncio`` now.
-
 Install
 =======
 ::
 
    pip install Torrelque
 
+Supported Redis server implementations: Redis, KeyDB.
+
 Quickstart
 ==========
 Producer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
    queue = torrelque.Torrelque(redis, queue='email')
    queue.schedule_sweep()
 
    task_data = {'addr': 'joe@doe.com', 'subj': 'hello', 'body': '...'}
-   task_id = await queue.enqueue(task)
+   task_id = await queue.enqueue(task_data)
    logger.info('Email task enqueued %s', task_id)
 
 Consumer:
 
 .. sourcecode:: python
 
    redis = yaaredis.StrictRedis()
@@ -94,27 +94,24 @@
            await some_email_client.send(**task_data)
        except SomeEmailError:
            logger.exception('Sending error, retrying in 30 seconds')
            await queue.requeue(task_id, delay=30)
        else:
            await queue.release(task_id)
 
-
 Example list
 ============
 - `Producer-consumer <e1_>`_. Infinite producing and consuming loops.
 - `Batch processing <e2_>`_. Finite number of tasks, consumers stop with a
   poison pill, bulk enqueue. This example can be used as a synthetic benchmark.
   Because there's no IO-bound workload, it'll be CPU-bound which isn't normal
   mode of operation for an asynchronous application. But it can be used to
   compare between CPython, PyPy and concurrency parameters.
 - `Web application background task <e3_>`_. This tornado application allows
   to start a task and push server-sent events (SSE) to UI about its status. UI
-  starts a task and waits for it to complete. When a task fails it's requeued
+  starts a task and waits for it to complete. When a task fails it's re-queued
   with exponential back-off.
 
 
 .. _e1: https://heptapod.host/saajns/torrelque/blob/branch/default/example/producer_consumer.py
 .. _e2: https://heptapod.host/saajns/torrelque/blob/branch/default/example/batch_processing.py
 .. _e3: https://heptapod.host/saajns/torrelque/blob/branch/default/example/wait_until_complete.py
-
-
```

### Comparing `Torrelque-0.6.0/setup.py` & `Torrelque-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from setuptools import setup
 
 
 setup(
     name             = 'Torrelque',
-    version          = '0.6.0',
+    version          = '0.7.0',
     author           = 'saaj',
     author_email     = 'mail@saaj.me',
     packages         = ['torrelque'],
     package_data     = {'torrelque' : ['*.lua']},
     license          = 'LGPL-3.0-only',
     description      = 'Asynchronous Redis-backed reliable queue package',
     long_description = open('README.rst', 'rb').read().decode('utf-8'),
     platforms        = ['Any'],
+    python_requires  = '>= 3',
     keywords         = 'python redis asynchronous job-queue work-queue',
     url              = 'https://heptapod.host/saajns/torrelque',
     project_urls     = {
         'Source Code'   : 'https://heptapod.host/saajns/torrelque',
         'Documentation' : 'https://torrelque.readthedocs.io/',
         'Release Notes' : 'https://torrelque.readthedocs.io/en/latest/history.html',
     },
     classifiers = [
         'Topic :: Software Development :: Libraries',
         'Framework :: AsyncIO',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Intended Audience :: Developers',
     ],
-    install_requires = ['yaaredis >= 3.0.0, < 4'],
+    install_requires = ['redis >= 5.0.1'],
     extras_require   = {
-        'test'   : ['asynctest < 0.14'],
-        'manual' : ['sphinx >= 4, < 5'],
+        'manual' : ['sphinx >= 7, < 8'],
     },
 )
```

### Comparing `Torrelque-0.6.0/torrelque/__init__.py` & `Torrelque-0.7.0/torrelque/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,44 @@
 '''Asynchronous Redis-backed reliable queue package.'''
 
 
 import asyncio
-import contextlib
 import enum
-import hashlib
 import json
 import logging
 import time
 import uuid
-from importlib.resources import read_text
-from typing import Any, Callable, List, NamedTuple, Optional, Sequence, Tuple, Union
+from typing import Any, AsyncIterable, Callable, Dict, List, NamedTuple, Optional, Tuple, Union
 
-import yaaredis
-from yaaredis.pipeline import StrictPipeline
+import redis.asyncio
+from redis.asyncio.client import Pipeline
+
+
+# read_text is deprecated since Python 3.9
+try:
+    from importlib.resources import files
+except ImportError:  # nocov
+    from importlib.resources import read_text
+else:
+    def read_text(package, resource) -> str:
+        with (files(package) / resource).open('r') as f:
+            return f.read()
+
+# aclosing is available since Python 3.10
+try:
+    from contextlib import aclosing
+except ImportError:  # nocov
+    from contextlib import asynccontextmanager
+
+    @asynccontextmanager
+    async def aclosing(thing):
+        try:
+            yield thing
+        finally:
+            await thing.aclose()
 
 
 __all__ = (
     'Torrelque',
     'TorrelqueQueueStats',
     'TorrelqueTaskStatus',
     'TorrelqueTaskState',
@@ -199,72 +220,65 @@
 
     _serialiser: TorrelqueTaskSerialiser
     '''
     Task data serialiser that converts task object into and from string
     representation.
     '''
 
-    _redis: yaaredis.StrictRedis
+    _client: redis.asyncio.Redis
     '''Redis client.'''
 
     _sweep_task: asyncio.Task
     '''Periodic sweep ``asyncio`` task.'''
 
     _keyspace_notification_enabled = False
     '''
     Flag indicates that Redis keyspace notification were found
     correctly configured, and further tests should be omitted.
     '''
 
-    _scripts: dict
+    _scripts: Dict[str, 'redis.commands.core.AsyncScript']
     '''Dictionary with Lua scripts read on initialisation.'''
 
     def __init__(
         self,
-        redis: yaaredis.StrictRedis,
+        client: redis.asyncio.Redis,
         *,
         queue: str = 'trq',
         serialiser=TorrelqueTaskSerialiser(lambda obj: json.dumps(obj).encode(), json.loads),
     ):
-        if not isinstance(redis, yaaredis.StrictRedis):
-            raise TorrelqueError('yaaredis.StrictRedis instance expected')
+        if not isinstance(client, redis.asyncio.Redis):
+            raise TorrelqueError('redis.asyncio.Redis instance expected')
 
-        self._redis = redis
+        self._client = client
         self._serialiser = serialiser
-        self._scripts = {n: read_text(__package__, f'{n}.lua') for n in ('dequeue', 'sweep')}
+        self._scripts = {
+            n: client.register_script(read_text(__package__, f'{n}.lua'))
+            for n in ('dequeue', 'sweep')
+        }
 
         self.keys = {k: f'{queue}:{v}' for k, v in self.keys.items()}
 
     def _get_state_key(self, task_id):
         return '{}:{}'.format(self.keys['task'], task_id)
 
-    async def _call_script(self, name: str, keys: Sequence, args: Sequence):
-        script = self._scripts[name]
-        digest = hashlib.sha1(script.encode()).hexdigest()
-        try:
-            result = await self._redis.evalsha(digest, len(keys), *(*keys, *args))
-        except yaaredis.NoScriptError:
-            result = await self._redis.eval(script, len(keys), *(*keys, *args))
-
-        return result
-
     async def _enqueue(
         self,
-        pipeline: StrictPipeline,
+        pipeline: Pipeline,
         task,
         task_timeout: Optional[float] = None,
         delay: Optional[float] = None,
     ) -> str:
         task_timeout = task_timeout or self.task_timeout
         task_id = uuid.uuid1().hex
         task_data = self._serialiser.dumps(task)
         task_state_key = self._get_state_key(task_id)
 
         if delay:
-            await pipeline.zadd(self.keys['delayed'], time.time() + delay, task_id)
+            await pipeline.zadd(self.keys['delayed'], {task_id: time.time() + delay})
             await pipeline.hset(task_state_key, 'status', TorrelqueTaskStatus.DELAYED.value)
         else:
             await pipeline.lpush(self.keys['pending'], task_id)
             await pipeline.hset(task_state_key, 'status', TorrelqueTaskStatus.PENDING.value)
 
         await pipeline.hset(self.keys['tasks'], task_id, task_data)
         await pipeline.hset(task_state_key, 'enqueue_time', time.time())
@@ -274,15 +288,15 @@
 
     async def enqueue(
         self,
         task,
         *,
         task_timeout: Optional[float] = None,
         delay: Optional[float] = None,
-        pipeline: Optional[StrictPipeline] = None
+        pipeline: Optional[Pipeline] = None
     ) -> str:
         '''
         Put a task on the queue optionally providing its timeout and delay.
 
         :argument task:
             Arbitrary serialisable task payload.
         :argument task_timeout:
@@ -298,45 +312,45 @@
         :return:
             Task identifier.
         '''
 
         if pipeline is not None:
             task_id = await self._enqueue(pipeline, task, task_timeout, delay)
         else:
-            async with await self._redis.pipeline(transaction=True) as pipeline:
+            async with await self._client.pipeline(transaction=True) as pipeline:
                 task_id = await self._enqueue(pipeline, task, task_timeout, delay)
                 await pipeline.execute()
 
         return task_id
 
     async def _dequeue(self, timeout: int, max_tasks: int) -> List[TaskPair]:
         pending_key = self.keys['pending']
         dequeueing_key = self.keys['dequeueing']
 
         # Try to move max_tasks task ids to dequeueing without blocking
         task_ids: List[bytes] = []
         if max_tasks > 1:
-            async with await self._redis.pipeline(transaction=True) as pipeline:
+            async with await self._client.pipeline(transaction=True) as pipeline:
                 for _ in range(max_tasks):
                     await pipeline.rpoplpush(pending_key, dequeueing_key)
                 task_ids.extend(task_id for task_id in await pipeline.execute() if task_id)
 
         # If the above hasn't succeeded guarantee at least one task
         if not task_ids:
-            task_id = await self._redis.brpoplpush(
+            task_id = await self._client.brpoplpush(
                 pending_key, dequeueing_key, timeout=timeout or 0
             )
             if not task_id:
                 raise TorrelqueTimeoutError
             else:
                 task_ids.append(task_id)
 
         keys = [self.keys[k] for k in ('dequeueing', 'working', 'tasks', 'task')]
         args = [time.time(), TorrelqueTaskStatus.WORKING.value] + task_ids
-        pairs = await self._call_script('dequeue', keys, args)
+        pairs = await self._scripts['dequeue'](keys, args)
 
         result = []
         for task_id, task_data in pairs:
             task_id = task_id.decode()
             task_data = self._serialiser.loads(task_data)
             if not task_data:
                 logger.warning('Task:%s not found in dequeueing list', task_id)
@@ -380,15 +394,15 @@
         assert max_tasks > 0
 
         task_pairs = await self._dequeue(timeout, max_tasks)
         return task_pairs if max_tasks > 1 else task_pairs[0]
 
     async def _requeue(
         self,
-        pipeline: StrictPipeline,
+        pipeline: Pipeline,
         task_id: str,
         delay: Optional[float] = None,
         task_timeout: Optional[float] = None
     ) -> list:
         expected = []
         await pipeline.zrem(self.keys['working'], task_id)
         expected.append(1)
@@ -397,15 +411,15 @@
         if not delay:
             await pipeline.lpush(self.keys['pending'], task_id)
             await pipeline.hset(task_state_key, 'last_requeue_time', time.time())
             await pipeline.hincrby(task_state_key, 'requeue_count', 1)
             await pipeline.hset(task_state_key, 'status', TorrelqueTaskStatus.PENDING.value)
             expected.extend([..., ..., ..., 0])
         else:
-            await pipeline.zadd(self.keys['delayed'], time.time() + delay, task_id)
+            await pipeline.zadd(self.keys['delayed'], {task_id: time.time() + delay})
             await pipeline.hset(task_state_key, 'status', TorrelqueTaskStatus.DELAYED.value)
             expected.extend([1, 0])
 
         if task_timeout:
             await pipeline.hset(task_state_key, 'timeout', task_timeout)
             expected.append(0)
 
@@ -413,15 +427,15 @@
 
     async def requeue(
         self,
         task_id: str,
         delay: Optional[float] = None,
         *,
         task_timeout: Optional[float] = None,
-        pipeline: Optional[StrictPipeline] = None,
+        pipeline: Optional[Pipeline] = None,
     ):
         '''
         Return failed task into the queue with optional delay.
 
         :argument task_id:
             Task identifier.
         :argument delay:
@@ -434,24 +448,24 @@
         :argument pipeline:
             External Redis pipeline that allows for bulk requeue.
         '''
 
         if pipeline is not None:
             await self._requeue(pipeline, task_id, delay, task_timeout)
         else:
-            async with await self._redis.pipeline(transaction=True) as pipeline:
+            async with await self._client.pipeline(transaction=True) as pipeline:
                 expected = await self._requeue(pipeline, task_id, delay, task_timeout)
                 actual = await pipeline.execute()
 
             if not all(expc == actl or expc is ... for expc, actl in zip(expected, actual)):
                 logger.warning('Inconsistent requeue of task:%s: %s', task_id, actual)
 
     async def _release(
         self,
-        pipeline: StrictPipeline,
+        pipeline: Pipeline,
         task_id: str,
         result=None,
         result_ttl: Optional[int] = None,
         status: TorrelqueTaskStatus = TorrelqueTaskStatus.COMPLETED,
     ) -> list:
         if status is not None and not status.isfinal():
             raise TorrelqueError(f'Invalid status for released task: {status}')
@@ -480,15 +494,15 @@
     async def release(
         self,
         task_id: str,
         *,
         result=None,
         result_ttl: Optional[int] = None,
         status: TorrelqueTaskStatus = TorrelqueTaskStatus.COMPLETED,
-        pipeline: Optional[StrictPipeline] = None,
+        pipeline: Optional[Pipeline] = None,
     ):
         '''
         Remove finished task from the queue.
 
         Unless ``result`` is specified, all task information is removed
         from the queue immediately.
 
@@ -513,42 +527,41 @@
         :raises TorrelqueError:
             If the status is not final.
         '''
 
         if pipeline is not None:
             await self._release(pipeline, task_id, result, result_ttl, status)
         else:
-            async with await self._redis.pipeline(transaction=True) as pipeline:
+            async with await self._client.pipeline(transaction=True) as pipeline:
                 expected = await self._release(pipeline, task_id, result, result_ttl, status)
                 actual = await pipeline.execute()
 
             if expected != actual:
                 logger.warning('Inconsistent release of task:%s: %s', task_id, actual)
 
     async def _check_keyspace_notification_config(self):
         if not self._keyspace_notification_enabled:
-            config = await self._redis.config_get('notify-keyspace-events')
+            config = await self._client.config_get('notify-keyspace-events')
             notify_config = set(config['notify-keyspace-events'])
             # See https://redis.io/topics/notifications#configuration
             if {'K', 'A'} - notify_config and {'K', 'g', 'h'} - notify_config:
                 raise TorrelqueError('Redis notify-keyspace-events must include KA or Kgh')
             self._keyspace_notification_enabled = True
 
-    async def _get_keyspace_notification_message(self, pubsub, timeout: float):
+    async def _get_keyspace_notification_message(self, pubsub, timeout: float) -> Optional[dict]:
         try:
-            message = await asyncio.wait_for(pubsub.listen(), timeout)
-            # This is the effect of ignore_subscribe_messages
-            if message is None:
-                message = await self._get_keyspace_notification_message(pubsub, timeout)
+            message = await asyncio.wait_for(pubsub.get_message(), timeout)
         except asyncio.TimeoutError as ex:
             raise TorrelqueTimeoutError from ex
         else:
             return message
 
-    async def watch(self, task_id: str, *, timeout: Optional[float] = None):
+    async def watch(
+        self, task_id: str, *, timeout: Optional[float] = None
+    ) -> AsyncIterable[TorrelqueTaskState]:
         '''
         Watch task status change until it's released from the queue.
 
         .. note::
 
            This method relies on ``notify-keyspace-events`` introduced
            in Redis 2.8. The configuration must have generic and hash
@@ -579,24 +592,24 @@
         task_state = await self.get_task_state(task_id)
         yield task_state
 
         status = task_state.status
         if status.isfinal():
             return
 
-        with contextlib.closing(self._redis.pubsub(ignore_subscribe_messages=True)) as pubsub:
-            dbn = self._redis.connection_pool.connection_kwargs['db']
+        async with aclosing(self._client.pubsub(ignore_subscribe_messages=True)) as pubsub:
+            dbn = self._client.connection_pool.connection_kwargs.get('db', 0)
             await pubsub.subscribe('__keyspace@{}__:{}'.format(dbn, self._get_state_key(task_id)))
 
             iter_timeout = timeout
             while True:
                 message = await self._get_keyspace_notification_message(pubsub, iter_timeout)
-                if message['data'] == b'del':
+                if message and message['data'] == b'del':
                     return  # Released without result
-                elif message['data'] == b'hset':
+                elif message and message['data'] == b'hset':
                     try:
                         task_state = await self.get_task_state(task_id)
                     except TorrelqueLookupError:
                         return  # Race condition with release
 
                     if task_state.status != status:
                         status = task_state.status
@@ -609,32 +622,34 @@
 
     async def sweep(self) -> Tuple[int, int, int]:
         '''
         Execute the task sweep.
 
         :return:
             3-tuple:
+
             - stale tasks from "working" set returned into "pending" list
             - due delayed tasks from "delayed" set returned into "pending" list
             - stale dequeueing task ids returned into "pending" list
         '''
 
         keys = [
             self.keys[k]
             for k in ('pending', 'dequeueing', 'undequeued', 'working', 'delayed', 'task')
         ]
         args = [time.time(), TorrelqueTaskStatus.PENDING.value]
-        return tuple(await self._call_script('sweep', keys, args))
+        result = await self._scripts['sweep'](keys, args)
+        return tuple(result)
 
     async def _sweep_runner(self, interval: float):
         while True:
             start = time.monotonic()
             try:
                 result = await self.sweep()
-            except yaaredis.RedisError:
+            except redis.RedisError:
                 logger.exception('Sweep has failed with Redis error, continuing')
             except asyncio.CancelledError:
                 break
             except Exception:
                 logger.exception('Sweep has failed with unexpected error, stopping')
                 break
             else:
@@ -658,15 +673,15 @@
 
         assert self._sweep_task
         self._sweep_task.cancel()
 
     async def get_queue_stats(self) -> TorrelqueQueueStats:
         '''Get queue counters.'''
 
-        async with await self._redis.pipeline(transaction=True) as pipe:
+        async with await self._client.pipeline(transaction=True) as pipe:
             await pipe.hlen(self.keys['tasks'])
             await pipe.llen(self.keys['pending'])
             await pipe.zcard(self.keys['working'])
             await pipe.zcard(self.keys['delayed'])
             result = await pipe.execute()
 
         return TorrelqueQueueStats(*result)
@@ -677,15 +692,15 @@
 
         :argument task_id:
             Task identifier.
         :raises TorrelqueLookupError:
             If the task state key is not found.
         '''
 
-        result = await self._redis.hgetall(self._get_state_key(task_id))
+        result = await self._client.hgetall(self._get_state_key(task_id))
         if not result:
             raise TorrelqueLookupError
 
         return TorrelqueTaskState(
             status             = TorrelqueTaskStatus(int(result[b'status'])),
             timeout            = float(result[b'timeout']),
             enqueue_time       = float(result[b'enqueue_time']),
```

### Comparing `Torrelque-0.6.0/torrelque/dequeue.lua` & `Torrelque-0.7.0/torrelque/dequeue.lua`

 * *Files identical despite different names*

### Comparing `Torrelque-0.6.0/torrelque/sweep.lua` & `Torrelque-0.7.0/torrelque/sweep.lua`

 * *Files identical despite different names*

### Comparing `Torrelque-0.6.0/torrelque/test.py` & `Torrelque-0.7.0/torrelque/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import asyncio
 import logging
 import os
 import pickle
 import time
 import warnings
-from unittest import mock
+from unittest import IsolatedAsyncioTestCase, mock
 
-import asynctest
-import yaaredis
+import redis.asyncio as redis
 
 from . import (
     Torrelque,
     TorrelqueError,
     TorrelqueLookupError,
     TorrelqueTaskStatus,
     TorrelqueTimeoutError,
@@ -19,34 +18,36 @@
 
 
 def setUpModule():
     logging.basicConfig(level=logging.WARNING)
     warnings.simplefilter('error')
 
 
-class TestTorrelque(asynctest.TestCase):
+class TestTorrelque(IsolatedAsyncioTestCase):
+
+    maxDiff = None
 
     redis = None
     testee = None
 
-    async def setUp(self):
+    async def asyncSetUp(self):
         dsn = os.getenv('TEST_REDIS_DSN', 'redis://localhost/1')
-        self.redis = yaaredis.StrictRedis.from_url(dsn)
+        self.redis = redis.Redis.from_url(dsn)
         self.testee = Torrelque(self.redis)
 
         await self.redis.flushdb()
         await self.redis.config_set('notify-keyspace-events', 'KA')
 
-    def tearDown(self):
-        self.redis.connection_pool.disconnect()
+    async def asyncTearDown(self):
+        await self.redis.connection_pool.disconnect()
 
     def test_instantiation_error(self):
         with self.assertRaises(TorrelqueError) as ctx:
             Torrelque(object())
-        self.assertEqual('yaaredis.StrictRedis instance expected', str(ctx.exception))
+        self.assertEqual('redis.asyncio.Redis instance expected', str(ctx.exception))
 
     async def _get_queue_state(self):
         pending = await self.redis.lrange(self.testee.keys['pending'], 0, -1)
         working = await self.redis.zrange(self.testee.keys['working'], 0, -1, withscores=True)
         delayed = await self.redis.zrange(self.testee.keys['delayed'], 0, -1, withscores=True)
         tasks = await self.redis.hgetall(self.testee.keys['tasks'])
         return pending, working, delayed, tasks
@@ -237,15 +238,15 @@
                 task_id, _ = await queue.dequeue()
                 actual.add(task_id)
                 await queue.release(task_id)
 
         async def run_consumers():
             await asyncio.gather(*[create_consumer() for _ in range(8)])
 
-        consumer_task = self.loop.create_task(run_consumers())
+        consumer_task = asyncio.get_running_loop().create_task(run_consumers())
 
         async for _ in self.testee.watch(task_id2):
             pass
 
         self.assertEqual({task_id1, task_id2}, actual)
 
         consumer_task.cancel()
@@ -343,22 +344,23 @@
         with self.assertRaises(TorrelqueTimeoutError):
             await self.testee.dequeue(max_tasks=4, timeout=1)
 
     async def test_dequeue_not_found_in_dequeueing(self):
         task_id = await self.testee.enqueue({'foo': 'bar'}, task_timeout=5)
         self.testee.schedule_sweep(0.1)
 
-        orig_call_script = self.testee._call_script
+        script = self.testee._scripts['dequeue']
+        orig_call = script.__class__.__call__
 
-        async def call_script(name, *args):
-            if name == 'dequeue':
+        async def call_script(self, *args, **kwargs):
+            if self is script:
                 await asyncio.sleep(0.2)
-            return await orig_call_script(name, *args)
+            return await orig_call(self, *args, **kwargs)
 
-        with mock.patch.object(self.testee, '_call_script', call_script):
+        with mock.patch.object(script.__class__, '__call__', call_script):
             with self.assertRaises(TorrelqueLookupError) as exctx:
                 with self.assertLogs(level='WARNING') as logctx:
                     await self.testee.dequeue()
 
         self.assertEqual(
             [f'WARNING:torrelque:Task:{task_id} not found in dequeueing list'], logctx.output
         )
@@ -726,15 +728,15 @@
 
         states = []
 
         async def watch():
             async for state in self.testee.watch(task_id):
                 states.append(state._asdict())
 
-        watch_task = self.loop.create_task(watch())
+        watch_task = asyncio.get_running_loop().create_task(watch())
         # Watch is typically on the producer's side, but here and below
         # it needs more "space" on the loop to timely receive messages
         await asyncio.sleep(0)
         await self.testee.dequeue()
         await asyncio.sleep(0.05)
         await self.testee.requeue(task_id, task_timeout=30)
         await asyncio.sleep(0.05)
@@ -824,15 +826,15 @@
 
         states = []
 
         async def watch():
             async for state in self.testee.watch(task_id):
                 states.append(state._asdict())
 
-        watch_task = self.loop.create_task(watch())
+        watch_task = asyncio.get_running_loop().create_task(watch())
         # Watch is typically on the producer's side, but here and below
         # it needs more "space" on the loop to timely receive messages
         await asyncio.sleep(0)
         await self.testee.dequeue()
         await asyncio.sleep(0.05)
         await self.testee.release(
             task_id, result={'some_status': 'ERROR'}, status=TorrelqueTaskStatus.REJECTED
@@ -879,18 +881,18 @@
         now = time.time()
 
         task_id = await self.testee.enqueue({'Subterfuge': '!'})
 
         states = []
 
         async def watch():
-            async for state in self.testee.watch(task_id, timeout=0.1):
+            async for state in self.testee.watch(task_id, timeout=0.15):
                 states.append(state._asdict())
 
-        watch_task = self.loop.create_task(watch())
+        watch_task = asyncio.get_running_loop().create_task(watch())
         # Watch is typically on the producer's side, but here and below
         # it needs more "space" on the loop to timely receive messages
         await asyncio.sleep(0)
         await self.testee.dequeue()
         await asyncio.sleep(0.05)
         await self.testee.requeue(task_id, task_timeout=30)
         await asyncio.sleep(0.05)
@@ -899,15 +901,15 @@
 
         with self.assertRaises(TorrelqueTimeoutError):
             await watch_task
 
         for state in states:
             self.assertAlmostEqual(now, state.pop('enqueue_time'), delta=0.1)
             if state['last_dequeue_time']:
-                self.assertAlmostEqual(now, state.pop('last_dequeue_time'), delta=0.1)
+                self.assertAlmostEqual(now, state.pop('last_dequeue_time'), delta=0.15)
             if state['last_requeue_time']:
                 self.assertAlmostEqual(now, state.pop('last_requeue_time'), delta=0.1)
 
         expected = [{
             'dequeue_count': 0,
             'last_dequeue_time': None,
             'last_requeue_time': None,
@@ -927,16 +929,23 @@
         }, {
             'dequeue_count': 1,
             'release_time': None,
             'requeue_count': 1,
             'result': None,
             'status': TorrelqueTaskStatus.PENDING,
             'timeout': 30.0
+        }, {
+            'dequeue_count': 2,
+            'requeue_count': 1,
+            'release_time': None,
+            'result': None,
+            'status': TorrelqueTaskStatus.WORKING,
+            'timeout': 30.0
         }]
-        self.assertEqual(states, expected)
+        self.assertEqual(expected, states)
 
     async def test_watch_nonexistent(self):
         with self.assertRaises(TorrelqueLookupError):
             async for _ in self.testee.watch('the road'):
                 pass
 
     async def test_watch_released(self):
@@ -979,21 +988,21 @@
         self.assertEqual(message, str(ctx.exception))
 
     async def test_watch_invalid_keyspace_notification_checked_once(self):
         task_id = await self.testee.enqueue({'foo': 'bar'})
         await self.testee.dequeue()
         await self.testee.release(task_id, result=1)
 
-        with mock.patch.object(self.testee, '_redis', wraps=self.testee._redis) as spy:
+        with mock.patch.object(self.redis, 'config_get', wraps=self.redis.config_get) as spy:
             async for _ in self.testee.watch(task_id):
                 pass
             async for _ in self.testee.watch(task_id):
                 pass
 
-            spy.config_get.assert_called_once()
+            spy.assert_called_once()
 
     async def test_sweep(self):
         actual = await self.testee.sweep()
         self.assertEqual((0, 0, 0), actual)
 
         now = time.time()
 
@@ -1164,15 +1173,15 @@
         self.assertEqual(task_ids, list(map(bytes.decode, pending)))
 
         for i in range(8):
             await self.redis.rpoplpush(self.testee.keys['pending'], self.testee.keys['dequeueing'])
 
         self.testee.schedule_sweep(0.1)
 
-        with self.assertLogs(level='DEBUG') as ctx:
+        with self.assertLogs(logger='torrelque', level='DEBUG') as ctx:
             await asyncio.sleep(0.25)
 
         # Make sure undequeued task ids are returned on the second call
         self.assertEqual(
             [
                 'DEBUG:torrelque:Sweep has requeued: stale=0, delayed=0, undequeued=0',
                 'DEBUG:torrelque:Sweep has requeued: stale=0, delayed=0, undequeued=8',
@@ -1216,31 +1225,28 @@
         await self.testee.release(task_id)
 
         self.assertEqual(([], [], [], {}), await self._get_queue_state())
 
     async def test_call_script(self):
         await self.redis.script_flush()
 
-        with mock.patch.object(self.testee, '_redis', wraps=self.testee._redis) as spy:
+        with mock.patch.object(self.redis, 'evalsha', wraps=self.redis.evalsha) as spy:
             await self.testee.sweep()
 
-            self.assertEqual(2, len(spy.mock_calls))
-            spy.evalsha.assert_called_once()
-            spy.eval.assert_called_once()
+            self.assertEqual(2, spy.call_count)
 
-        with mock.patch.object(self.testee, '_redis', wraps=self.testee._redis) as spy:
+        with mock.patch.object(self.redis, 'evalsha', wraps=self.redis.evalsha) as spy:
             await self.testee.sweep()
 
             self.assertEqual(1, len(spy.mock_calls))
-            spy.evalsha.assert_called_once()
 
     async def test_sweep_runner(self):
         sweep_mock = asyncio.Future()
         sweep_mock.set_result((2, 2, 1))
-        error_list = [yaaredis.DataError(), sweep_mock]
+        error_list = [redis.DataError(), sweep_mock]
 
         def one_error():
             obj = error_list.pop(0)
             if isinstance(obj, Exception):
                 raise obj
             else:
                 return obj
```

