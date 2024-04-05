# Comparing `tmp/veilid-0.3.0.tar.gz` & `tmp/veilid-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilid-0.3.0.tar", max compression
+gzip compressed data, was "veilid-0.3.1.tar", max compression
```

## Comparing `veilid-0.3.0.tar` & `veilid-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    15581 2023-07-19 17:22:19.917057 veilid-0.3.0/LICENSE.md
--rw-r--r--   0        0        0      833 2023-09-16 22:58:30.780273 veilid-0.3.0/README.md
--rw-r--r--   0        0        0      541 2024-03-28 02:34:47.979238 veilid-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-16 21:06:23.269310 veilid-0.3.0/veilid/__init__.py
--rw-r--r--   0        0        0    10005 2024-03-28 02:34:47.979238 veilid-0.3.0/veilid/api.py
--rw-r--r--   0        0        0     5217 2024-03-28 02:34:47.979238 veilid-0.3.0/veilid/config.py
--rw-r--r--   0        0        0     3594 2023-11-07 03:14:10.762364 veilid-0.3.0/veilid/error.py
--rw-r--r--   0        0        0    41203 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/json_api.py
--rw-r--r--   0        0        0     3039 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/operations.py
--rw-r--r--   0        0        0   103830 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/schema/RecvMessage.json
--rw-r--r--   0        0        0    38789 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/schema/Request.json
--rw-r--r--   0        0        0    12239 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/state.py
--rw-r--r--   0        0        0    12702 2024-03-28 02:34:47.983238 veilid-0.3.0/veilid/types.py
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 veilid-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    15581 2023-07-19 16:52:47.952728 veilid-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0      833 2024-04-05 01:29:50.201762 veilid-0.3.1/README.md
+-rw-r--r--   0        0        0      541 2024-04-05 01:29:50.201762 veilid-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-17 21:54:35.187940 veilid-0.3.1/veilid/__init__.py
+-rw-r--r--   0        0        0    10005 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/api.py
+-rw-r--r--   0        0        0     5217 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/config.py
+-rw-r--r--   0        0        0     3594 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/error.py
+-rw-r--r--   0        0        0    41203 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/json_api.py
+-rw-r--r--   0        0        0     3039 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/operations.py
+-rw-r--r--   0        0        0   103960 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/schema/RecvMessage.json
+-rw-r--r--   0        0        0    38789 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/schema/Request.json
+-rw-r--r--   0        0        0    12291 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/state.py
+-rw-r--r--   0        0        0    12702 2024-04-05 01:29:50.205762 veilid-0.3.1/veilid/types.py
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 veilid-0.3.1/PKG-INFO
```

### Comparing `veilid-0.3.0/LICENSE.md` & `veilid-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/README.md` & `veilid-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/pyproject.toml` & `veilid-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # --- Bumpversion match - do not reorder
 name = "veilid"
-version = "0.3.0"
+version = "0.3.1"
 # ---
 description = ""
 authors = ["Veilid Team <contact@veilid.com>"]
 readme = "README.md"
 packages = [{ include = "veilid" }]
 
 [tool.poetry.dependencies]
```

### Comparing `veilid-0.3.0/veilid/api.py` & `veilid-0.3.1/veilid/api.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/config.py` & `veilid-0.3.1/veilid/config.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/error.py` & `veilid-0.3.1/veilid/error.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/json_api.py` & `veilid-0.3.1/veilid/json_api.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/operations.py` & `veilid-0.3.1/veilid/operations.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/schema/RecvMessage.json` & `veilid-0.3.1/veilid/schema/RecvMessage.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999565972222222%*

 * *Differences: {"'oneOf'": "{1: {'oneOf': {7: {'required': {delete: [4]}, 'properties': {'value': {replace: "*

 * *            "OrderedDict([('anyOf', [OrderedDict([('$ref', '#/definitions/ValueData')]), "*

 * *            "OrderedDict([('type', 'null')])])])}}}}}}"}*

```diff
@@ -4232,23 +4232,29 @@
                                 "maxItems": 2,
                                 "minItems": 2,
                                 "type": "array"
                             },
                             "type": "array"
                         },
                         "value": {
-                            "$ref": "#/definitions/ValueData"
+                            "anyOf": [
+                                {
+                                    "$ref": "#/definitions/ValueData"
+                                },
+                                {
+                                    "type": "null"
+                                }
+                            ]
                         }
                     },
                     "required": [
                         "count",
                         "key",
                         "kind",
-                        "subkeys",
-                        "value"
+                        "subkeys"
                     ],
                     "type": "object"
                 },
                 {
                     "properties": {
                         "kind": {
                             "enum": [
```

### Comparing `veilid-0.3.0/veilid/schema/Request.json` & `veilid-0.3.1/veilid/schema/Request.json`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/veilid/state.py` & `veilid-0.3.1/veilid/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,30 +354,30 @@
         )
 
 
 class VeilidValueChange:
     key: TypedKey
     subkeys: list[tuple[ValueSubkey, ValueSubkey]]
     count: int
-    value: ValueData
+    value: Optional[ValueData]
 
-    def __init__(self, key: TypedKey, subkeys: list[tuple[ValueSubkey, ValueSubkey]], count: int, value: ValueData):
+    def __init__(self, key: TypedKey, subkeys: list[tuple[ValueSubkey, ValueSubkey]], count: int, value: Optional[ValueData]):
         self.key = key
         self.subkeys = subkeys
         self.count = count
         self.value = value
 
     @classmethod
     def from_json(cls, j: dict) -> Self:
         """JSON object hook"""
         return cls(
             TypedKey(j["key"]),
             [(p[0], p[1]) for p in j["subkeys"]],
             j["count"],
-            ValueData.from_json(j["value"]),
+            None if j["value"] is None else ValueData.from_json(j["value"]),
         )
 
 
 class VeilidUpdateKind(StrEnum):
     LOG = "Log"
     APP_MESSAGE = "AppMessage"
     APP_CALL = "AppCall"
```

### Comparing `veilid-0.3.0/veilid/types.py` & `veilid-0.3.1/veilid/types.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.0/PKG-INFO` & `veilid-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilid
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Veilid Team
 Author-email: contact@veilid.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

