# Comparing `tmp/dnb-urn-service-0.1.5.tar.gz` & `tmp/dnb-urn-service-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnb-urn-service-0.1.5.tar", last modified: Fri Feb 17 13:20:28 2023, max compression
+gzip compressed data, was "dnb-urn-service-0.1.6.tar", last modified: Thu Apr  4 11:31:47 2024, max compression
```

## Comparing `dnb-urn-service-0.1.5.tar` & `dnb-urn-service-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:20:28.716379 dnb-urn-service-0.1.5/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      296 2022-07-29 13:30:54.000000 dnb-urn-service-0.1.5/AUTHORS.rst
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1080 2022-05-04 14:57:50.000000 dnb-urn-service-0.1.5/LICENSE
--rw-r--r--   0 gressho   (1000) gressho   (1000)      868 2023-02-17 13:20:28.716379 dnb-urn-service-0.1.5/PKG-INFO
--rw-r--r--   0 gressho   (1000) gressho   (1000)      440 2023-02-17 09:35:46.000000 dnb-urn-service-0.1.5/README.rst
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:20:28.644379 dnb-urn-service-0.1.5/dnb_urn_service/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      439 2023-02-17 13:19:58.000000 dnb-urn-service-0.1.5/dnb_urn_service/__init__.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     2076 2022-10-25 13:55:58.000000 dnb-urn-service-0.1.5/dnb_urn_service/errors.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     3676 2022-10-27 09:02:10.000000 dnb-urn-service-0.1.5/dnb_urn_service/request.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     6708 2023-02-01 14:33:42.000000 dnb-urn-service-0.1.5/dnb_urn_service/rest_client.py
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:20:28.716379 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      868 2023-02-17 13:20:28.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/PKG-INFO
--rw-r--r--   0 gressho   (1000) gressho   (1000)      393 2023-02-17 13:20:28.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/SOURCES.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)        1 2023-02-17 13:20:28.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/dependency_links.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)        1 2022-11-02 09:33:32.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/not-zip-safe
--rw-r--r--   0 gressho   (1000) gressho   (1000)      137 2023-02-17 13:20:28.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/requires.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)       16 2023-02-17 13:20:28.000000 dnb-urn-service-0.1.5/dnb_urn_service.egg-info/top_level.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1560 2023-02-17 13:20:28.717379 dnb-urn-service-0.1.5/setup.cfg
--rw-r--r--   0 gressho   (1000) gressho   (1000)      363 2023-02-16 11:22:08.000000 dnb-urn-service-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:31:47.940824 dnb-urn-service-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-04 11:31:47.940824 dnb-urn-service-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:31:47.937824 dnb-urn-service-0.1.6/dnb_urn_service/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/dnb_urn_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/dnb_urn_service/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-04-04 11:20:05.000000 dnb-urn-service-0.1.6/dnb_urn_service/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-04 11:20:05.000000 dnb-urn-service-0.1.6/dnb_urn_service/rest_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:31:47.939824 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 11:31:47.000000 dnb-urn-service-0.1.6/dnb_urn_service.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-04 11:31:47.941824 dnb-urn-service-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-03 12:55:39.000000 dnb-urn-service-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:31:47.938824 dnb-urn-service-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-04-04 11:20:05.000000 dnb-urn-service-0.1.6/tests/test_dnb_urn_service.py
```

### Comparing `dnb-urn-service-0.1.5/LICENSE` & `dnb-urn-service-0.1.6/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 MIT License
 
-Copyright (C) 2022 University of Münster.
+Copyright (C) 2024 University of Münster.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dnb-urn-service-0.1.5/dnb_urn_service/errors.py` & `dnb-urn-service-0.1.6/dnb_urn_service/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of Invenio.
-#
-# Copyright (C) 2022 University Münster.
+# Copyright (C) 2022-2024 University Münster.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the Revised BSD License; see LICENSE file for
 # more details.
 
 """Errors for the DNB URN service API."""
```

### Comparing `dnb-urn-service-0.1.5/dnb_urn_service/request.py` & `dnb-urn-service-0.1.6/dnb_urn_service/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of Invenio.
-#
-# Copyright (C) 2022 University Münster.
+# Copyright (C) 2022-2024 University Münster.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the Revised BSD License; see LICENSE file for
 # more details.
 
 """Module for making requests to the DNB URN service API."""
 
@@ -27,24 +25,30 @@
     :param password: HTTP Basic Authentication Password
     :param default_params: A key/value-mapping which will be converted into a
         query string on all requests.
     :param timeout: Connect and read timeout in seconds. Specify a tuple
         (connect, read) to specify each timeout individually.
     """
 
-    def __init__(self, base_url=None, username=None, password=None,
-                 default_params=None, timeout=None):
+    def __init__(
+        self,
+        base_url=None,
+        username=None,
+        password=None,
+        default_params=None,
+        timeout=None,
+    ):
         """Initialize request object."""
         self.base_url = base_url
         self.username = username
-        self.password = password.encode('utf8')
+        self.password = password.encode("utf-8")
         self.default_params = default_params or {}
         self.timeout = timeout
 
-    def request(self, url, method='GET', body=None, params=None, headers=None):
+    def request(self, url, method="GET", body=None, params=None, headers=None):
         """Make a request.
 
         If the request was successful (i.e no exceptions), you can find the
         HTTP response code in self.code and the response body in self.value.
         :param url: Request URL (relative to base_url if set)
         :param method: Request method (GET, POST, DELETE) supported
         :param body: Request body
@@ -60,53 +64,55 @@
         if self.default_params:
             params.update(self.default_params)
 
         if self.base_url:
             url = self.base_url + url
 
         if body and isinstance(body, str):
-            body = body.encode('utf-8')
+            body = body.encode("utf-8")
 
         request_func = getattr(requests, method.lower())
         kwargs = dict(
             auth=HTTPBasicAuth(self.username, self.password),
             params=params,
             headers=headers,
         )
 
-        if method == 'POST':
-            kwargs['data'] = body
-        if method == 'PUT':
-            kwargs['data'] = body
-        if method == 'PATCH':
-            kwargs['data'] = body
+        if method == "POST":
+            kwargs["data"] = body
+        if method == "PUT":
+            kwargs["data"] = body
+        if method == "PATCH":
+            kwargs["data"] = body
         if self.timeout is not None:
-            kwargs['timeout'] = self.timeout
+            kwargs["timeout"] = self.timeout
 
         try:
             return request_func(url, **kwargs)
         except RequestException as e:
             raise HttpError(e)
         except ssl.SSLError as e:
             raise HttpError(e)
 
     def get(self, url, params=None, headers=None):
         """Make a GET request."""
         return self.request(url, params=params, headers=headers)
 
     def post(self, url, body=None, params=None, headers=None):
         """Make a POST request."""
-        return self.request(url, method="POST", body=body, params=params,
-                            headers=headers)
+        return self.request(
+            url, method="POST", body=body, params=params, headers=headers
+        )
 
     def delete(self, url):
         """Make a DELETE request."""
         return self.request(url, method="DELETE")
 
     def head(self, url):
         """Make a HEAD request."""
         return self.request(url, method="HEAD")
 
     def patch(self, url, body=None, params=None, headers=None):
         """Make a POST request."""
-        return self.request(url, method="PATCH", body=body, params=params,
-                            headers=headers)
+        return self.request(
+            url, method="PATCH", body=body, params=params, headers=headers
+        )
```

### Comparing `dnb-urn-service-0.1.5/dnb_urn_service/rest_client.py` & `dnb-urn-service-0.1.6/dnb_urn_service/rest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of Invenio.
-#
-# Copyright (C) 2022 University Münster.
+# Copyright (C) 2022-2024 University Münster.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the Revised BSD License; see LICENSE file for
 # more details.
 
 """Python API client wrapper for the DNB URN service API.
 
@@ -18,24 +16,25 @@
 
 import requests
 from idutils import normalize_urn
 
 from .errors import DNBURNServiceError, DNBURNServiceUserNotAuthorizedError
 from .request import DNBUrnServiceRequest
 
-HTTP_OK = requests.codes['ok']
-HTTP_CREATED = requests.codes['created']
-HTTP_NO_CONTENT = requests.codes['no_content']
+HTTP_OK = requests.codes["ok"]
+HTTP_CREATED = requests.codes["created"]
+HTTP_NO_CONTENT = requests.codes["no_content"]
 
 
 class DNBUrnServiceRESTClient(object):
     """DNB URN service API client wrapper."""
 
-    def __init__(self, username, password, prefix, test_mode=False, url=None,
-                 timeout=None):
+    def __init__(
+        self, username, password, prefix, test_mode=False, url=None, timeout=None
+    ):
         """Initialize the API client wrapper.
 
         :param username: DNB username.
         :param password: DNB password.
         :param prefix: URN prefix (or DNB_URN_PREFIX).
         :param test_mode: use test URL when True
         :param url: DNB URN service API base URL.
@@ -47,22 +46,22 @@
         self.prefix = str(prefix)
 
         if test_mode:
             self.api_url = "https://api.nbn-resolving.org/sandbox/v2/"
         else:
             self.api_url = url or "https://api.nbn-resolving.org/v2/"
 
-        if not self.api_url.endswith('/'):
-            self.api_url += '/'
+        if not self.api_url.endswith("/"):
+            self.api_url += "/"
 
         self.timeout = timeout
 
     def __repr__(self):
         """Create string representation of object."""
-        return '<DNBUrnServiceRESTClient: {0}>'.format(self.username)
+        return "<DNBUrnServiceRESTClient: {0}>".format(self.username)
 
     def _create_request(self):
         """Create a new Request object."""
         return DNBUrnServiceRequest(
             base_url=self.api_url,
             username=self.username,
             password=self.password,
@@ -73,15 +72,15 @@
         """Get the URL where the resource pointed by the URN is located.
 
         :param urn: URN name of the resource.
         """
         request = self._create_request()
         resp = request.get("urns/urn/" + urn + "/my-urls")
         if resp.status_code == HTTP_OK:
-            return resp.json()['items'][0]['url']
+            return resp.json()["items"][0]["url"]
         else:
             raise DNBURNServiceError.factory(resp.status_code, resp.text)
 
     def head_urn(self, urn):
         """Check if a URN is registered.
 
         :param urn: URN name of the resource.
@@ -91,66 +90,61 @@
         if resp.status_code == HTTP_OK:
             return normalize_urn(urn)
         else:
             raise DNBURNServiceError.factory(resp.status_code, resp.text)
 
     def check_urn(self, urn):
         """Check urn structure.
+
         Check that the urn has a form
         urn:nbn: with the prefix defined
         """
-        split = urn.split('-')
-        prefix = split[0] + '-'
+        split = urn.split("-")
+        prefix = split[0] + "-"
         if not urn.startswith(self.prefix):
             # Provided a URN with the wrong prefix
-            raise ValueError('Wrong URN {0} prefix provided, it should be '
-                             '{1} as defined in the rest client'
-                             .format(prefix, self.prefix))
+            raise ValueError(
+                "Wrong URN {0} prefix provided, it should be "
+                "{1} as defined in the rest client".format(prefix, self.prefix)
+            )
         return normalize_urn(urn)
 
     def post_urn(self, data):
         """Post a new JSON payload to DNB."""
         headers = {
-            'content-type': 'application/json',
-            'accept': 'application/json',
+            "content-type": "application/json",
+            "accept": "application/json",
         }
         body = data
         request = self._create_request()
-        resp = request.post(
-            "urns",
-            body=json.dumps(body),
-            headers=headers)
+        resp = request.post("urns", body=json.dumps(body), headers=headers)
         if resp.status_code == HTTP_CREATED:
-            return normalize_urn(resp.json()['urn'])
+            return normalize_urn(resp.json()["urn"])
         else:
             raise DNBURNServiceError.factory(resp.status_code, resp.text)
 
     def patch_urn(self, urn, data):
         """Patch a new JSON payload to DNB."""
         headers = {"content-type": "application/json"}
         body = data
         request = self._create_request()
-        resp = request.patch(
-            "urns/urn/" + urn,
-            body=json.dumps(body),
-            headers=headers)
+        resp = request.patch("urns/urn/" + urn, body=json.dumps(body), headers=headers)
         if resp.status_code == HTTP_NO_CONTENT:
             return ""
         else:
             raise DNBURNServiceError.factory(resp.status_code, resp.text)
 
     def patch_urls(self, urn, data):
         """Patch a new JSON payload to patch the URL's at DNB."""
         headers = {"content-type": "application/json"}
         body = data
         request = self._create_request()
         resp = request.patch(
-            "urns/urn/" + urn + "/my-urls",
-            body=json.dumps(body),
-            headers=headers)
+            "urns/urn/" + urn + "/my-urls", body=json.dumps(body), headers=headers
+        )
         if resp.status_code == HTTP_NO_CONTENT:
             return ""
         else:
             raise DNBURNServiceError.factory(resp.status_code, resp.text)
 
     def delete_urn(self, urn):
         """Delete a URN completely.
@@ -165,42 +159,27 @@
 
         This URN will be public and can be deleted.
         If urn is not provided, there will be an error.
         :param url: URL where the urn will resolve.
         :param urn: URN (e.g. urn:nbn:de:hbz:6-1234)
         :return:
         """
-        data = {
-            "urn": urn,
-            "urls": [
-                {
-                    "url": url,
-                    "priority": 10
-                }
-            ]
-        }
+        data = {"urn": urn, "urls": [{"url": url, "priority": 10}]}
         return self.post_urn(data)
 
     def modify_urn(self, url, urn):
         """Modify the url of an existing urn.
 
         This URN will be public and can't be deleted.
         If urn is not provided, there will be an error.
         :param url: URL where the urn will resolve.
         :param urn: URN (e.g. urn:nbn:de:hbz:6-1234)
         :return:
         """
-        data = {
-            [
-                {
-                    "url": url,
-                    "priority": 10
-                }
-            ]
-        }
+        data = {[{"url": url, "priority": 10}]}
         return self.patch_urls(urn, data)
 
     def check_if_registered(self, urn):
         """Check if a URN is registered."""
         return self.head_urn(urn)
 
     def create_successor(self, urn, successor):
```

