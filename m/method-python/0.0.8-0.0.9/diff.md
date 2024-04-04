# Comparing `tmp/method-python-0.0.8.tar.gz` & `tmp/method-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/method-python/method-python/dist/tmpwonyujmb/method-python-0.0.8.tar", last modified: Fri Oct 22 01:18:32 2021, max compression
+gzip compressed data, was "/home/runner/work/method-python/method-python/dist/tmp3y_zbs_9/method-python-0.0.9.tar", last modified: Fri Oct 22 21:35:00 2021, max compression
```

## Comparing `method-python-0.0.8.tar` & `method-python-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 01:18:32.000000 method-python-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-10-22 01:18:21.000000 method-python-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-22 01:18:32.000000 method-python-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-10-22 01:18:21.000000 method-python-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 01:18:32.000000 method-python-0.0.8/method/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-10-22 01:18:21.000000 method-python-0.0.8/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-10-22 01:18:21.000000 method-python-0.0.8/method/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-10-22 01:18:21.000000 method-python-0.0.8/method/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-10-22 01:18:21.000000 method-python-0.0.8/method/method.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 01:18:32.000000 method-python-0.0.8/method/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Account.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Bin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Element.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Merchant.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Payment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Report.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/RoutingNumber.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/Webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2021-10-22 01:18:21.000000 method-python-0.0.8/method/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-22 01:18:32.000000 method-python-0.0.8/method_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 01:18:32.000000 method-python-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-22 01:18:21.000000 method-python-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 21:35:00.000000 method-python-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-10-22 21:34:50.000000 method-python-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-22 21:35:00.000000 method-python-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-10-22 21:34:50.000000 method-python-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 21:35:00.000000 method-python-0.0.9/method/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-10-22 21:34:50.000000 method-python-0.0.9/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-10-22 21:34:50.000000 method-python-0.0.9/method/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-10-22 21:34:50.000000 method-python-0.0.9/method/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2021-10-22 21:34:50.000000 method-python-0.0.9/method/method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2434 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 21:35:00.000000 method-python-0.0.9/method/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Account.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Bin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Element.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2830 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/HealthCheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Merchant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Payment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Report.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/RoutingNumber.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Verification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/Webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2021-10-22 21:34:50.000000 method-python-0.0.9/method/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-22 21:35:00.000000 method-python-0.0.9/method_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 21:35:00.000000 method-python-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-22 21:34:50.000000 method-python-0.0.9/setup.py
```

### Comparing `method-python-0.0.8/LICENSE` & `method-python-0.0.9/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2021 Method Financial
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -13,7 +15,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `method-python-0.0.8/method/configuration.py` & `method-python-0.0.9/method/configuration.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/errors.py` & `method-python-0.0.9/method/errors.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resource.py` & `method-python-0.0.9/method/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,34 @@
         self.config = config
         self.client = Client(config.url, headers={
             'Authorization': 'Bearer {token}'.format(token=config.api_key),
             'Content-Type': 'application/json'
         })
 
     @MethodError.catch
+    def _get_raw(self) -> Any:
+        return self.client.GET().json()
+
+    @MethodError.catch
     def _get(self) -> Any:
         return self.client.GET().json().get('data')
 
     @MethodError.catch
     def _get_with_id(self, _id: str) -> Any:
         return self.client.GET(_id).json().get('data')
 
     @MethodError.catch
     def _get_with_params(self, params: Dict) -> Any:
         return self.client.GET(params=params).json().get('data')
 
     @MethodError.catch
+    def _get_with_sub_path(self, path: str) -> Any:
+        return self.client(path).GET().json().get('data')
+
+    @MethodError.catch
     def _list(self, params: Optional[Dict] = None) -> List[Any]:
         return self.client.GET(params=params).json().get('data')
 
     @MethodError.catch
     def _create(self, data: Dict, request_opts: Optional[RequestOpts] = None) -> Any:
         opts = {'headers': {}}
         if request_opts and request_opts.get('idempotency_key'):
```

### Comparing `method-python-0.0.8/method/resources/Account.py` & `method-python-0.0.9/method/resources/Account.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Bin.py` & `method-python-0.0.9/method/resources/Bin.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Element.py` & `method-python-0.0.9/method/resources/Element.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Entity.py` & `method-python-0.0.9/method/resources/Entity.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Merchant.py` & `method-python-0.0.9/method/resources/Merchant.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Payment.py` & `method-python-0.0.9/method/resources/Payment.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Report.py` & `method-python-0.0.9/method/resources/Report.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/RoutingNumber.py` & `method-python-0.0.9/method/resources/RoutingNumber.py`

 * *Files identical despite different names*

### Comparing `method-python-0.0.8/method/resources/Verification.py` & `method-python-0.0.9/method/resources/Verification.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,19 +53,26 @@
 
 class VerificationCreateOpts(TypedDict):
     type: VerificationTypesLiterals
     plaid: Optional[VerificationPlaidCreate]
     mx: Optional[VerificationMXCreate]
 
 
+class VerificationTestAmountsResponse(TypedDict):
+    amounts: List[int]
+
+
 class VerificationResource(Resource):
     def __init__(self, config: Configuration):
         super(VerificationResource, self).__init__(config.add_path('verification'))
 
     def get(self) -> Verification:
         return super(VerificationResource, self)._get()
 
     def update(self, opts: VerificationUpdateOpts) -> Verification:
         return super(VerificationResource, self)._update(opts)
 
     def create(self, opts: VerificationCreateOpts) -> Verification:
         return super(VerificationResource, self)._create(opts)
+
+    def get_test_amounts(self) -> VerificationTestAmountsResponse:
+        return super(VerificationResource, self)._get_with_sub_path('/amounts')
```

### Comparing `method-python-0.0.8/method/resources/Webhook.py` & `method-python-0.0.9/method/resources/Webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from method.resource import Resource, RequestOpts
 from method.configuration import Configuration
 
 
 WebhookTypesLiterals = Literal[
     'payment.create',
-    'payment.update'
+    'payment.update',
+    'account_verification.sent'
 ]
 
 
 class Webhook(TypedDict):
     id: str
     type: WebhookTypesLiterals
     url: str
```

### Comparing `method-python-0.0.8/method/resources/__init__.py` & `method-python-0.0.9/method/resources/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 from method.resources.Entity import Entity, EntityResource
 from method.resources.Merchant import Merchant, MerchantResource
 from method.resources.Payment import Payment, PaymentResource
 from method.resources.Report import Report, ReportResource
 from method.resources.RoutingNumber import RoutingNumber, RoutingNumberResource
 from method.resources.Verification import Verification, VerificationResource
 from method.resources.Webhook import Webhook, WebhookResource
+from method.resources.HealthCheck import HealthCheckResource
```

### Comparing `method-python-0.0.8/method_python.egg-info/SOURCES.txt` & `method-python-0.0.9/method_python.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 method/errors.py
 method/method.py
 method/resource.py
 method/resources/Account.py
 method/resources/Bin.py
 method/resources/Element.py
 method/resources/Entity.py
+method/resources/HealthCheck.py
 method/resources/Merchant.py
 method/resources/Payment.py
 method/resources/Report.py
 method/resources/RoutingNumber.py
 method/resources/Verification.py
 method/resources/Webhook.py
 method/resources/__init__.py
```

