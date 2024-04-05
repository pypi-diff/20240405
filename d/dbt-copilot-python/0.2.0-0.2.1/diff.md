# Comparing `tmp/dbt_copilot_python-0.2.0.tar.gz` & `tmp/dbt_copilot_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_python-0.2.0.tar", max compression
+gzip compressed data, was "dbt_copilot_python-0.2.1.tar", max compression
```

## Comparing `dbt_copilot_python-0.2.0.tar` & `dbt_copilot_python-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1090 2023-06-29 15:16:12.111872 dbt_copilot_python-0.2.0/LICENSE
--rw-r--r--   0        0        0     4055 2024-01-29 12:54:43.535129 dbt_copilot_python-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-09-21 15:13:21.158088 dbt_copilot_python-0.2.0/dbt_copilot_python/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 12:54:43.535186 dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/__init__.py
--rw-r--r--   0        0        0      179 2024-01-29 12:54:43.535615 dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/const.py
--rw-r--r--   0        0        0     1463 2024-01-29 12:54:43.535875 dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/healthcheck.py
--rw-r--r--   0        0        0      755 2024-01-29 12:54:43.536105 dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/heartbeat.py
--rw-r--r--   0        0        0     1225 2023-09-21 15:13:21.158382 dbt_copilot_python-0.2.0/dbt_copilot_python/database.py
--rw-r--r--   0        0        0      657 2024-01-24 14:02:54.879693 dbt_copilot_python-0.2.0/dbt_copilot_python/network.py
--rw-r--r--   0        0        0      150 2023-09-22 07:37:42.199035 dbt_copilot_python-0.2.0/dbt_copilot_python/utility.py
--rw-r--r--   0        0        0      862 2024-01-29 12:54:43.537020 dbt_copilot_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4994 1970-01-01 00:00:00.000000 dbt_copilot_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-29 15:16:12.111872 dbt_copilot_python-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4055 2024-01-29 12:54:43.535129 dbt_copilot_python-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-09-21 15:13:21.158088 dbt_copilot_python-0.2.1/dbt_copilot_python/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 12:54:43.535186 dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/__init__.py
+-rw-r--r--   0        0        0      179 2024-01-29 12:54:43.535615 dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/const.py
+-rw-r--r--   0        0        0     1463 2024-01-29 12:54:43.535875 dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/healthcheck.py
+-rw-r--r--   0        0        0      755 2024-01-29 12:54:43.536105 dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/heartbeat.py
+-rw-r--r--   0        0        0     1225 2023-09-21 15:13:21.158382 dbt_copilot_python-0.2.1/dbt_copilot_python/database.py
+-rw-r--r--   0        0        0      692 2024-04-05 06:36:30.198659 dbt_copilot_python-0.2.1/dbt_copilot_python/network.py
+-rw-r--r--   0        0        0      150 2024-04-04 16:59:10.535836 dbt_copilot_python-0.2.1/dbt_copilot_python/utility.py
+-rw-r--r--   0        0        0      862 2024-04-05 06:36:30.199077 dbt_copilot_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4994 1970-01-01 00:00:00.000000 dbt_copilot_python-0.2.1/PKG-INFO
```

### Comparing `dbt_copilot_python-0.2.0/LICENSE` & `dbt_copilot_python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.2.0/README.md` & `dbt_copilot_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/healthcheck.py` & `dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/healthcheck.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.2.0/dbt_copilot_python/celery_health_check/heartbeat.py` & `dbt_copilot_python-0.2.1/dbt_copilot_python/celery_health_check/heartbeat.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.2.0/dbt_copilot_python/database.py` & `dbt_copilot_python-0.2.1/dbt_copilot_python/database.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.2.0/pyproject.toml` & `dbt_copilot_python-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-copilot-python"
-version = "0.2.0"
+version = "0.2.1"
 description = "Helper functions to run Django and Flask applications in AWS Copilot/ECS."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 readme = "README.md"
 packages = [{ include = "dbt_copilot_python" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dbt_copilot_python-0.2.0/PKG-INFO` & `dbt_copilot_python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Helper functions to run Django and Flask applications in AWS Copilot/ECS.
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

