# Comparing `tmp/jsm_user_services-1.3.6.tar.gz` & `tmp/jsm_user_services-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.3.6.tar", max compression
+gzip compressed data, was "jsm_user_services-1.3.7.tar", max compression
```

## Comparing `jsm_user_services-1.3.6.tar` & `jsm_user_services-1.3.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/LICENSE
--rw-r--r--   0        0        0    10306 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/README.md
--rw-r--r--   0        0        0       54 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     2475 2023-09-11 17:09:25.194296 jsm_user_services-1.3.6/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    14221 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/flask/__init__.py
--rw-r--r--   0        0        0     3462 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/flask/middleware.py
--rw-r--r--   0        0        0     3167 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4247 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     4657 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     1840 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1007 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      419 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     2185 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1573 2023-09-11 17:09:25.198297 jsm_user_services-1.3.6/pyproject.toml
--rw-r--r--   0        0        0    11392 1970-01-01 00:00:00.000000 jsm_user_services-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/LICENSE
+-rw-r--r--   0        0        0    10306 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/README.md
+-rw-r--r--   0        0        0       54 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2475 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14221 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/flask/__init__.py
+-rw-r--r--   0        0        0     3462 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/flask/middleware.py
+-rw-r--r--   0        0        0     3292 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4247 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     4657 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     1840 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1007 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      415 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1574 2024-04-05 19:24:06.819015 jsm_user_services-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0    11293 1970-01-01 00:00:00.000000 jsm_user_services-1.3.7/PKG-INFO
```

### Comparing `jsm_user_services-1.3.6/LICENSE` & `jsm_user_services-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/README.md` & `jsm_user_services-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.3.7/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.3.7/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.3.7/jsm_user_services/drf_tools/permissions.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/exception.py` & `jsm_user_services-1.3.7/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.3.7/jsm_user_services/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/middleware.py` & `jsm_user_services-1.3.7/jsm_user_services/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 from jsm_user_services.services.user import get_session_id_from_bearer_token
 from jsm_user_services.support.auth_jwt import get_bearer_authorization_token
 from jsm_user_services.support.http_utils import convert_header_to_meta_key
 from jsm_user_services.support.local_threading_utils import add_to_local_threading
 from jsm_user_services.support.local_threading_utils import remove_from_local_threading
 from jsm_user_services.support.string_utils import get_first_value_from_comma_separated_string
 
-try:
-    from django.utils.deprecation import MiddlewareMixin
-except ImportError:
-    MiddlewareMixin = object
-
 logger = logging.getLogger(__name__)
 
 header_with_client_ip_address = convert_header_to_meta_key(os.getenv("PRIMARY_IP_ADDRESS_HEADER", "true-client-ip"))
 header_with_list_of_addresses = convert_header_to_meta_key(
     os.getenv("GUNICORN_IP_ADDRESS_HEADER", "x-original-forwarded-for")
 )
 
 
-class JsmJwtService(MiddlewareMixin):
+class JsmJwtService:
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        self.process_request(request)
+        response = self.get_response(request)
+        return self.process_response(request, response)
+
     def process_request(self, request):
         add_to_local_threading("authorization_token", self._get_jwt_token_from_request(request))
         add_to_local_threading("user_ip", self._get_user_ip_from_request(request))
         add_to_local_threading("user_session_id", self._get_user_session_id_from_request(request))
 
     def process_response(self, request, response):
         remove_from_local_threading("authorization_token")
```

### Comparing `jsm_user_services-1.3.6/jsm_user_services/services/everest.py` & `jsm_user_services-1.3.7/jsm_user_services/services/everest.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/services/google.py` & `jsm_user_services-1.3.7/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/services/user.py` & `jsm_user_services-1.3.7/jsm_user_services/services/user.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/settings.py` & `jsm_user_services-1.3.7/jsm_user_services/settings.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.3.7/jsm_user_services/support/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.3.7/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.3.7/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/support/request_id.py` & `jsm_user_services-1.3.7/jsm_user_services/support/request_id.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.3.7/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.6/pyproject.toml` & `jsm_user_services-1.3.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.3.6"
+version = "1.3.7"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
@@ -16,15 +16,15 @@
     "Framework :: Django",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 PyJWT = "^2.4.0"
 requests = "*"
 
 [tool.poetry.extras]
 flask = ["flask", "flask-log-request-id"]
 drf = ["djangorestframework", "request-id-django-log"]
```

### Comparing `jsm_user_services-1.3.6/PKG-INFO` & `jsm_user_services-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.3.6
+Version: 1.3.7
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: drf
 Provides-Extra: flask
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: requests
```

