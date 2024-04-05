# Comparing `tmp/pytest_celery-1.0.0rc2.tar.gz` & `tmp/pytest_celery-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_celery-1.0.0rc2.tar", max compression
+gzip compressed data, was "pytest_celery-1.0.0rc3.tar", max compression
```

## Comparing `pytest_celery-1.0.0rc2.tar` & `pytest_celery-1.0.0rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1791 2024-03-27 12:07:07.304911 pytest_celery-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     4512 2024-03-27 12:07:19.032890 pytest_celery-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     7228 2024-03-27 12:07:19.116889 pytest_celery-1.0.0rc2/src/pytest_celery/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/__init__.py
--rw-r--r--   0        0        0     1923 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/backend.py
--rw-r--r--   0        0        0    10591 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/base.py
--rw-r--r--   0        0        0     1880 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/broker.py
--rw-r--r--   0        0        0     4956 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/container.py
--rw-r--r--   0        0        0     9307 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/setup.py
--rw-r--r--   0        0        0     3737 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/api/worker.py
--rw-r--r--   0        0        0     3728 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/defaults.py
--rw-r--r--   0        0        0        0 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/__init__.py
--rw-r--r--   0        0        0     2287 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/backend.py
--rw-r--r--   0        0        0     2312 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/broker.py
--rw-r--r--   0        0        0     2816 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/setup.py
--rw-r--r--   0        0        0     2033 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/worker.py
--rw-r--r--   0        0        0      207 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/plugin.py
--rw-r--r--   0        0        0      452 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/__init__.py
--rw-r--r--   0        0        0      147 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/__init__.py
--rw-r--r--   0        0        0      298 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/api.py
--rw-r--r--   0        0        0     1861 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/container.py
--rw-r--r--   0        0        0      431 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/defaults.py
--rw-r--r--   0        0        0     2775 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/fixtures.py
--rw-r--r--   0        0        0      145 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/__init__.py
--rw-r--r--   0        0        0      291 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/api.py
--rw-r--r--   0        0        0     2056 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/container.py
--rw-r--r--   0        0        0      404 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/defaults.py
--rw-r--r--   0        0        0     2706 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/fixtures.py
--rw-r--r--   0        0        0      135 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/__init__.py
--rw-r--r--   0        0        0      143 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/__init__.py
--rw-r--r--   0        0        0      780 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/api.py
--rw-r--r--   0        0        0      238 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/defaults.py
--rw-r--r--   0        0        0     3049 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/fixtures.py
--rw-r--r--   0        0        0      142 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/broker/__init__.py
--rw-r--r--   0        0        0      285 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/broker/api.py
--rw-r--r--   0        0        0      233 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/broker/defaults.py
--rw-r--r--   0        0        0     3015 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/broker/fixtures.py
--rw-r--r--   0        0        0     2119 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/container.py
--rw-r--r--   0        0        0      274 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/defaults.py
--rw-r--r--   0        0        0      969 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/Dockerfile
--rw-r--r--   0        0        0      152 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/__init__.py
--rw-r--r--   0        0        0     6510 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/container.py
--rw-r--r--   0        0        0      152 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/content/__init__.py
--rw-r--r--   0        0        0      498 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/content/app.py
--rw-r--r--   0        0        0      677 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/content/utils.py
--rw-r--r--   0        0        0     1113 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/defaults.py
--rw-r--r--   0        0        0     9315 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/fixtures.py
--rw-r--r--   0        0        0     3549 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/tasks.py
--rw-r--r--   0        0        0     9142 2024-03-27 12:07:07.312911 pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/volume.py
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 pytest_celery-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1791 2024-04-05 16:14:25.718155 pytest_celery-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     4531 2024-04-05 16:14:43.834252 pytest_celery-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     7303 2024-04-05 16:14:43.918253 pytest_celery-1.0.0rc3/src/pytest_celery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/__init__.py
+-rw-r--r--   0        0        0     1923 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/backend.py
+-rw-r--r--   0        0        0    10591 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/base.py
+-rw-r--r--   0        0        0     1880 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/broker.py
+-rw-r--r--   0        0        0     5284 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/container.py
+-rw-r--r--   0        0        0     9307 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/setup.py
+-rw-r--r--   0        0        0     3737 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/worker.py
+-rw-r--r--   0        0        0     3728 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/__init__.py
+-rw-r--r--   0        0        0     2287 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/backend.py
+-rw-r--r--   0        0        0     2312 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/broker.py
+-rw-r--r--   0        0        0     2816 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/setup.py
+-rw-r--r--   0        0        0     2033 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/worker.py
+-rw-r--r--   0        0        0      207 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/plugin.py
+-rw-r--r--   0        0        0      452 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/__init__.py
+-rw-r--r--   0        0        0      298 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/api.py
+-rw-r--r--   0        0        0     1861 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/container.py
+-rw-r--r--   0        0        0      431 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/defaults.py
+-rw-r--r--   0        0        0     2775 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/fixtures.py
+-rw-r--r--   0        0        0      145 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/api.py
+-rw-r--r--   0        0        0     2056 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/container.py
+-rw-r--r--   0        0        0      404 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/defaults.py
+-rw-r--r--   0        0        0     2706 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/fixtures.py
+-rw-r--r--   0        0        0      135 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/api.py
+-rw-r--r--   0        0        0      238 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/defaults.py
+-rw-r--r--   0        0        0     3049 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/fixtures.py
+-rw-r--r--   0        0        0      142 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/api.py
+-rw-r--r--   0        0        0      233 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/defaults.py
+-rw-r--r--   0        0        0     3015 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/fixtures.py
+-rw-r--r--   0        0        0     2235 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/container.py
+-rw-r--r--   0        0        0      274 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/defaults.py
+-rw-r--r--   0        0        0     1170 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/Dockerfile
+-rw-r--r--   0        0        0      152 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/__init__.py
+-rw-r--r--   0        0        0     7317 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/container.py
+-rw-r--r--   0        0        0      152 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/app.py
+-rw-r--r--   0        0        0      677 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/utils.py
+-rw-r--r--   0        0        0     1192 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/defaults.py
+-rw-r--r--   0        0        0     9720 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/fixtures.py
+-rw-r--r--   0        0        0     3549 2024-04-05 16:14:25.730155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/tasks.py
+-rw-r--r--   0        0        0     9142 2024-04-05 16:14:25.730155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/volume.py
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 pytest_celery-1.0.0rc3/PKG-INFO
```

### Comparing `pytest_celery-1.0.0rc2/LICENSE` & `pytest_celery-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/pyproject.toml` & `pytest_celery-1.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "Operating System :: OS Independent",
 ]
 
 description = "Pytest plugin for Celery"
 homepage = "https://github.com/celery/pytest-celery"
 license = "BSD"
 name = "pytest-celery"
-version = "v1.0.0rc2"
+version = "v1.0.0rc3"
 
 [tool.poetry_bumpversion.file."src/pytest_celery/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
 
 [tool.poetry_bumpversion.file."README.rst"]
 search = ':Version: {current_version}'
@@ -77,14 +77,15 @@
 python-memcached = { version = "*", optional = true }
 python = ">=3.8,<4.0"
 retry = ">=0.9.2"
 pytest-docker-tools = ">=3.1.3"
 docker = "^7.0.0"
 psutil = ">=5.9.7"
 setuptools = ">=69.1.0"
+debugpy = "^1.8.1"
 
 [tool.poetry.extras]
 all = ["redis", "python-memcached"]
 redis = ["redis"]
 memcached = ["python-memcached"]
 
 [tool.poetry.group.dev]
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/__init__.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Official pytest plugin for Celery."""
 
 # flake8: noqa
 
 
-__version__ = "v1.0.0rc2"
+__version__ = "v1.0.0rc3"
 __author__ = "Tomer Nosrati"
 __contact__ = "tomer.nosrati@gmail.com"
 __homepage__ = "https://pytest-celery.readthedocs.io/"
 __docformat__ = "restructuredtext"
 
 
 import re
@@ -99,14 +99,15 @@
     from pytest_celery.vendors.worker.fixtures import default_worker_cls
     from pytest_celery.vendors.worker.fixtures import default_worker_command
     from pytest_celery.vendors.worker.fixtures import default_worker_container
     from pytest_celery.vendors.worker.fixtures import default_worker_container_cls
     from pytest_celery.vendors.worker.fixtures import default_worker_container_session_cls
     from pytest_celery.vendors.worker.fixtures import default_worker_env
     from pytest_celery.vendors.worker.fixtures import default_worker_initial_content
+    from pytest_celery.vendors.worker.fixtures import default_worker_ports
     from pytest_celery.vendors.worker.fixtures import default_worker_signals
     from pytest_celery.vendors.worker.fixtures import default_worker_tasks
     from pytest_celery.vendors.worker.fixtures import default_worker_utils_module
     from pytest_celery.vendors.worker.fixtures import default_worker_volume
     from pytest_celery.vendors.worker.tasks import *
     from pytest_celery.vendors.worker.volume import WorkerInitialContent
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/backend.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/backend.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/base.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/base.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/broker.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/broker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/container.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,31 @@
 
         Returns:
             dict: Configuration values required for Celery.
         """
         raise NotImplementedError("CeleryTestContainer.celeryconfig")
 
     @classmethod
-    def command(cls, *args: str) -> list[str]:
+    def command(
+        cls,
+        *args: str,
+        debugpy: bool = False,
+        wait_for_client: bool = True,
+        **kwargs: dict,
+    ) -> list[str]:
         """Override the CMD instruction in the Dockerfile.
 
         This method should be overridden in derived classes to provide the
         specific command and its arguments required to start the container.
 
         Args:
             *args (str): Additional command-line arguments.
+            debugpy (bool): Enable debugpy. Defaults to False.
+            wait_for_client (bool): Wait for a debugger to be attached. Defaults to True.
+            **kwargs (dict): Additional keyword arguments.
 
         Raises:
             NotImplementedError: Rely on the Dockerfile if not set otherwise by default.
 
         Returns:
             list[str]: A list containing the command to run in the container as
                 the first element, followed by the command-line arguments.
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/setup.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/api/worker.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/api/worker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/defaults.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/defaults.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/backend.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/backend.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/broker.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/broker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/setup.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/fixtures/worker.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/worker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/container.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/memcached/fixtures.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/container.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/rabbitmq/fixtures.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/api.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/api.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/backend/fixtures.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/broker/fixtures.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/redis/container.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,21 @@
             "host_url": self.host_url,
             "hostname": self.hostname,
             "port": self.port,
             "vhost": self.vhost,
         }
 
     @classmethod
-    def command(cls, *args: str) -> list[str]:
+    def command(
+        cls,
+        *args: str,
+        debugpy: bool = False,
+        wait_for_client: bool = True,
+        **kwargs: dict,
+    ) -> list[str]:
         return ["redis-server", *args]
 
     @property
     def url(self) -> str:
         return f"{self.prefix()}{self.hostname}/{self.vhost}"
 
     @property
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/container.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from celery import Celery
 
 from pytest_celery.api.container import CeleryTestContainer
 from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_ENV
 from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_LOG_LEVEL
 from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_NAME
+from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_PORTS
 from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_QUEUE
 from pytest_celery.vendors.worker.defaults import DEFAULT_WORKER_VERSION
 from pytest_celery.vendors.worker.volume import WorkerInitialContent
 
 
 class CeleryWorkerContainer(CeleryTestContainer):
     """This is the base class for all Celery worker containers. It is
@@ -29,28 +30,56 @@
 
     Responsibility Scope:
         Prepare the worker container with the required filesystem, configurations and
         dependencies of your project.
     """
 
     @classmethod
-    def command(cls, *args: str) -> list[str]:
+    def command(
+        cls,
+        *args: str,
+        debugpy: bool = False,
+        wait_for_client: bool = True,
+        **kwargs: dict,
+    ) -> list[str]:
         args = args or tuple()
-        return [
-            "celery",
-            "-A",
-            "app",
-            "worker",
-            f"--loglevel={cls.log_level()}",
-            "-n",
-            f"{cls.worker_name()}@%h",
-            "-Q",
-            f"{cls.worker_queue()}",
-            *args,
-        ]
+        cmd = list()
+
+        if debugpy:
+            cmd.extend(
+                [
+                    "python",
+                    "-m",
+                    "debugpy",
+                    "--listen",
+                    "0.0.0.0:5678",
+                ]
+            )
+
+            if wait_for_client:
+                cmd.append("--wait-for-client")
+
+            cmd.append("-m")
+
+        cmd.extend(
+            [
+                "celery",
+                "-A",
+                "app",
+                "worker",
+                f"--loglevel={cls.log_level()}",
+                "-n",
+                f"{cls.worker_name()}@%h",
+                "-Q",
+                f"{cls.worker_queue()}",
+                *args,
+            ]
+        )
+
+        return cmd
 
     def _wait_port(self, port: str) -> int:
         # Not needed for worker container
         raise NotImplementedError
 
     @property
     def ready_prompt(self) -> str:
@@ -193,7 +222,12 @@
         if worker_signals:
             content.add_modules("signals", worker_signals)
         if worker_app:
             content.set_app_name(worker_app.main)
             content.set_config_from_object(worker_app)
 
         return content.generate()
+
+    @classmethod
+    def ports(cls) -> dict | None:
+        """Ports to expose from the worker container."""
+        return DEFAULT_WORKER_PORTS
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/content/utils.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/defaults.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,23 @@
 WORKER_ENV = {
     "CELERY_BROKER_URL": "memory://",
     "CELERY_RESULT_BACKEND": "cache+memory://",
     "PYTHONUNBUFFERED": "1",
     "PYTHONDONTWRITEBYTECODE": "1",
     "PYTHONPATH": "/app",
 }
+WORKER_DEBUGPY_PORTS = {
+    "5678/tcp": "5678",
+}
 WORKER_VOLUME = {
     "bind": "/app",
     "mode": "rw",
 }
 DEFAULT_WORKER_APP_NAME = WORKER_CELERY_APP_NAME
 DEFAULT_WORKER_VERSION = WORKER_CELERY_VERSION
 DEFAULT_WORKER_LOG_LEVEL = WORKER_LOG_LEVEL
 DEFAULT_WORKER_NAME = WORKER_NAME
 DEFAULT_WORKER_ENV = WORKER_ENV
+DEFAULT_WORKER_PORTS = None
 DEFAULT_WORKER_QUEUE = WORKER_QUEUE
 DEFAULT_WORKER_CONTAINER_TIMEOUT = 60
 DEFAULT_WORKER_VOLUME = WORKER_VOLUME
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/fixtures.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         type[CeleryWorkerContainer]: API for managing the vendor's container.
     """
     return CeleryWorkerContainer
 
 
 default_worker_container = container(
     image="{celery_base_worker_image.id}",
+    ports=fxtr("default_worker_ports"),
     environment=fxtr("default_worker_env"),
     network="{default_pytest_celery_network.name}",
     volumes={"{default_worker_volume.name}": DEFAULT_WORKER_VOLUME},
     wrapper_class=CeleryWorkerContainer,
     timeout=DEFAULT_WORKER_CONTAINER_TIMEOUT,
     command=fxtr("default_worker_command"),
 )
@@ -234,14 +235,27 @@
         worker_tasks=default_worker_tasks,
         worker_signals=default_worker_signals,
         worker_app=default_worker_app,
     )
 
 
 @pytest.fixture
+def default_worker_ports(default_worker_container_cls: type[CeleryWorkerContainer]) -> dict | None:
+    """Port bindings for this vendor.
+
+    Args:
+        default_worker_container_cls (type[CeleryWorkerContainer]): See also: :ref:`vendor-class`.
+
+    Returns:
+        dict: Port bindings.
+    """
+    return default_worker_container_cls.ports()
+
+
+@pytest.fixture
 def default_worker_app_module(default_worker_container_cls: type[CeleryWorkerContainer]) -> ModuleType:
     """App module for this worker.
 
     Args:
         default_worker_container_cls (type[CeleryWorkerContainer]): See also: :ref:`vendor-class`.
 
     Returns:
```

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/tasks.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/tasks.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/src/pytest_celery/vendors/worker/volume.py` & `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/volume.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc2/PKG-INFO` & `pytest_celery-1.0.0rc3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-celery
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Pytest plugin for Celery
 Home-page: https://github.com/celery/pytest-celery
 License: BSD
 Author: Tomer Nosrati
 Author-email: tomer.nosrati@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: all
 Provides-Extra: memcached
 Provides-Extra: redis
 Requires-Dist: celery
+Requires-Dist: debugpy (>=1.8.1,<2.0.0)
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: psutil (>=5.9.7)
 Requires-Dist: pytest-docker-tools (>=3.1.3)
 Requires-Dist: python-memcached ; extra == "all" or extra == "memcached"
 Requires-Dist: redis ; extra == "all" or extra == "redis"
 Requires-Dist: retry (>=0.9.2)
 Requires-Dist: setuptools (>=69.1.0)
```

