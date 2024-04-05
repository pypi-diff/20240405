# Comparing `tmp/utility_api-0.2.2.tar.gz` & `tmp/utility_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utility_api-0.2.2.tar", max compression
+gzip compressed data, was "utility_api-0.2.3.tar", max compression
```

## Comparing `utility_api-0.2.2.tar` & `utility_api-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       14 2024-02-21 02:42:59.889067 utility_api-0.2.2/README.md
--rw-r--r--   0        0        0     1016 2024-02-21 02:42:59.889067 utility_api-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       64 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/__init__.py
--rw-r--r--   0        0        0     1952 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/endpoints/authorization.py
--rw-r--r--   0        0        0     4485 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/endpoints/bill.py
--rw-r--r--   0        0        0      624 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/endpoints/form.py
--rw-r--r--   0        0        0     2420 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/endpoints/interval.py
--rw-r--r--   0        0        0     3094 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/endpoints/meter.py
--rw-r--r--   0        0        0     1103 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/base_enum.py
--rw-r--r--   0        0        0     1569 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/bill_types.py
--rw-r--r--   0        0        0      564 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/general_types.py
--rw-r--r--   0        0        0      496 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/interval_types.py
--rw-r--r--   0        0        0      673 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/meter_types.py
--rw-r--r--   0        0        0      985 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/models/object_types/test_scenario.py
--rw-r--r--   0        0        0    15878 2024-02-21 02:42:59.889067 utility_api-0.2.2/utility_api/service.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 utility_api-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-04-05 01:03:41.011480 utility_api-0.2.3/README.md
+-rw-r--r--   0        0        0     1016 2024-04-05 01:03:41.011480 utility_api-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-05 01:03:41.011480 utility_api-0.2.3/utility_api/__init__.py
+-rw-r--r--   0        0        0     1952 2024-04-05 01:03:41.011480 utility_api-0.2.3/utility_api/models/endpoints/authorization.py
+-rw-r--r--   0        0        0     4485 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/endpoints/bill.py
+-rw-r--r--   0        0        0      624 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/endpoints/form.py
+-rw-r--r--   0        0        0     2420 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/endpoints/interval.py
+-rw-r--r--   0        0        0     3141 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/endpoints/meter.py
+-rw-r--r--   0        0        0     1103 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/base_enum.py
+-rw-r--r--   0        0        0     1569 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/bill_types.py
+-rw-r--r--   0        0        0      564 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/general_types.py
+-rw-r--r--   0        0        0      496 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/interval_types.py
+-rw-r--r--   0        0        0      673 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/meter_types.py
+-rw-r--r--   0        0        0      985 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/models/object_types/test_scenario.py
+-rw-r--r--   0        0        0    15878 2024-04-05 01:03:41.015480 utility_api-0.2.3/utility_api/service.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 utility_api-0.2.3/PKG-INFO
```

### Comparing `utility_api-0.2.2/pyproject.toml` & `utility_api-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utility-api"
-version = "0.2.2"
+version = "0.2.3"
 description = "An interface for interacting with Utility API"
 authors = ["Gabrielle Anne Sblendorio <glsblendorio@gmail.com>"]
 readme = "README.md"
 packages = [{include = "utility_api"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13"
@@ -20,15 +20,15 @@
 flake8 = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tbump.version]
-current = "0.2.2"
+current = "0.2.3"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `utility_api-0.2.2/utility_api/models/endpoints/authorization.py` & `utility_api-0.2.3/utility_api/models/endpoints/authorization.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/endpoints/bill.py` & `utility_api-0.2.3/utility_api/models/endpoints/bill.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/endpoints/form.py` & `utility_api-0.2.3/utility_api/models/endpoints/form.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/endpoints/interval.py` & `utility_api-0.2.3/utility_api/models/endpoints/interval.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/endpoints/meter.py` & `utility_api-0.2.3/utility_api/models/endpoints/meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class OngoingMonitoring:
     """Ongoing monitoring settings for a meter."""
 
+    fixed_refresh_day: Optional[str]
     frequency: FrequencyType
     prepay: Optional[PrepayType] = None
     next_prepay: Optional[datetime] = field(
         metadata=config(field_name="next_prepay", decoder=datetime.fromisoformat),
         default=None,
     )
     next_refresh: Optional[datetime] = field(
@@ -38,15 +39,15 @@
 @dataclass_json(undefined=Undefined.RAISE)
 @dataclass
 class Base:
     """Basic information about the meter."""
 
     billing_account: str
     billing_address: Optional[str]
-    billing_contact: str
+    billing_contact: Optional[str]
     meter_numbers: List[str]
     service_address: str
     service_class: ServiceType
     service_identifier: str
     service_tariff: str
```

### Comparing `utility_api-0.2.2/utility_api/models/object_types/base_enum.py` & `utility_api-0.2.3/utility_api/models/object_types/base_enum.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/object_types/bill_types.py` & `utility_api-0.2.3/utility_api/models/object_types/bill_types.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/object_types/general_types.py` & `utility_api-0.2.3/utility_api/models/object_types/general_types.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/object_types/meter_types.py` & `utility_api-0.2.3/utility_api/models/object_types/meter_types.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/models/object_types/test_scenario.py` & `utility_api-0.2.3/utility_api/models/object_types/test_scenario.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/utility_api/service.py` & `utility_api-0.2.3/utility_api/service.py`

 * *Files identical despite different names*

### Comparing `utility_api-0.2.2/PKG-INFO` & `utility_api-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utility-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: An interface for interacting with Utility API
 Author: Gabrielle Anne Sblendorio
 Author-email: glsblendorio@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

