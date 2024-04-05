# Comparing `tmp/wkl-nmi-0.0.8.tar.gz` & `tmp/wkl-nmi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkl-nmi-0.0.8.tar", last modified: Wed Feb  7 17:21:25 2024, max compression
+gzip compressed data, was "wkl-nmi-0.0.9.tar", last modified: Fri Mar  1 20:32:51 2024, max compression
```

## Comparing `wkl-nmi-0.0.8.tar` & `wkl-nmi-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 17:21:25.604689 wkl-nmi-0.0.8/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkl-nmi-0.0.8/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)    10997 2024-02-07 17:21:25.604388 wkl-nmi-0.0.8/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)    10563 2024-02-07 17:21:03.000000 wkl-nmi-0.0.8/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      492 2024-02-07 17:21:19.000000 wkl-nmi-0.0.8/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-02-07 17:21:25.604731 wkl-nmi-0.0.8/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 17:21:25.601231 wkl-nmi-0.0.8/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 17:21:25.602488 wkl-nmi-0.0.8/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 16:28:08.000000 wkl-nmi-0.0.8/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     4241 2024-02-07 16:39:14.000000 wkl-nmi-0.0.8/src/test/test_billing.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1932 2024-02-07 16:39:03.000000 wkl-nmi-0.0.8/src/test/test_config.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      956 2024-02-07 16:38:55.000000 wkl-nmi-0.0.8/src/test/test_customerVault.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1401 2024-02-07 16:58:53.000000 wkl-nmi-0.0.8/src/test/test_pay.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2645 2024-02-07 16:38:37.000000 wkl-nmi-0.0.8/src/test/test_plans.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2392 2024-02-07 16:38:15.000000 wkl-nmi-0.0.8/src/test/test_subscriptions.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 17:21:25.604166 wkl-nmi-0.0.8/src/wkl_nmi.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)    10997 2024-02-07 17:21:25.000000 wkl-nmi-0.0.8/src/wkl_nmi.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      524 2024-02-07 17:21:25.000000 wkl-nmi-0.0.8/src/wkl_nmi.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-02-07 17:21:25.000000 wkl-nmi-0.0.8/src/wkl_nmi.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       11 2024-02-07 17:21:25.000000 wkl-nmi-0.0.8/src/wkl_nmi.egg-info/top_level.txt
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 17:21:25.603963 wkl-nmi-0.0.8/src/wknmi/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2023-11-28 19:55:41.000000 wkl-nmi-0.0.8/src/wknmi/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1127 2024-02-07 16:41:11.000000 wkl-nmi-0.0.8/src/wknmi/auth.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1986 2023-12-01 17:32:15.000000 wkl-nmi-0.0.8/src/wknmi/billing.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1334 2023-12-01 22:38:18.000000 wkl-nmi-0.0.8/src/wknmi/config.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1654 2024-02-07 17:18:14.000000 wkl-nmi-0.0.8/src/wknmi/customer_vault.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1869 2024-02-07 16:59:41.000000 wkl-nmi-0.0.8/src/wknmi/payment.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     2601 2023-12-01 17:45:19.000000 wkl-nmi-0.0.8/src/wknmi/plans.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3275 2023-12-06 18:20:20.000000 wkl-nmi-0.0.8/src/wknmi/subscriptions.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-03-01 20:32:51.045283 wkl-nmi-0.0.9/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkl-nmi-0.0.9/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)    10997 2024-03-01 20:32:51.044977 wkl-nmi-0.0.9/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)    10563 2024-02-07 17:21:03.000000 wkl-nmi-0.0.9/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      492 2024-03-01 20:32:15.000000 wkl-nmi-0.0.9/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-03-01 20:32:51.045325 wkl-nmi-0.0.9/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-03-01 20:32:51.038546 wkl-nmi-0.0.9/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-03-01 20:32:51.041269 wkl-nmi-0.0.9/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-02-07 16:28:08.000000 wkl-nmi-0.0.9/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     4241 2024-02-23 05:29:09.000000 wkl-nmi-0.0.9/src/test/test_billing.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1932 2024-02-07 16:39:03.000000 wkl-nmi-0.0.9/src/test/test_config.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1005 2024-02-23 05:33:06.000000 wkl-nmi-0.0.9/src/test/test_customerVault.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1401 2024-02-07 16:58:53.000000 wkl-nmi-0.0.9/src/test/test_pay.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2645 2024-02-07 16:38:37.000000 wkl-nmi-0.0.9/src/test/test_plans.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2392 2024-02-07 16:38:15.000000 wkl-nmi-0.0.9/src/test/test_subscriptions.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-03-01 20:32:51.044719 wkl-nmi-0.0.9/src/wkl_nmi.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)    10997 2024-03-01 20:32:51.000000 wkl-nmi-0.0.9/src/wkl_nmi.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      524 2024-03-01 20:32:51.000000 wkl-nmi-0.0.9/src/wkl_nmi.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-03-01 20:32:51.000000 wkl-nmi-0.0.9/src/wkl_nmi.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       11 2024-03-01 20:32:51.000000 wkl-nmi-0.0.9/src/wkl_nmi.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-03-01 20:32:51.044286 wkl-nmi-0.0.9/src/wknmi/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2023-11-28 19:55:41.000000 wkl-nmi-0.0.9/src/wknmi/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1159 2024-02-23 05:33:27.000000 wkl-nmi-0.0.9/src/wknmi/auth.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2096 2024-03-01 20:32:17.000000 wkl-nmi-0.0.9/src/wknmi/billing.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1334 2023-12-01 22:38:18.000000 wkl-nmi-0.0.9/src/wknmi/config.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1654 2024-02-07 17:18:14.000000 wkl-nmi-0.0.9/src/wknmi/customer_vault.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1869 2024-02-07 16:59:41.000000 wkl-nmi-0.0.9/src/wknmi/payment.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     2601 2023-12-01 17:45:19.000000 wkl-nmi-0.0.9/src/wknmi/plans.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3275 2023-12-06 18:20:20.000000 wkl-nmi-0.0.9/src/wknmi/subscriptions.py
```

### Comparing `wkl-nmi-0.0.8/LICENSE` & `wkl-nmi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/PKG-INFO` & `wkl-nmi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkl-nmi
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Nmi library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkl-nmi-0.0.8/README.md` & `wkl-nmi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/test/test_billing.py` & `wkl-nmi-0.0.9/src/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/test/test_config.py` & `wkl-nmi-0.0.9/src/test/test_config.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/test/test_customerVault.py` & `wkl-nmi-0.0.9/src/test/test_customerVault.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,7 +22,11 @@
                     "phone": "",
                     "email": "",
                 },
             }
         )
         self.assertEqual(result["status_code"], 200)
         self.assertEqual(result["response"]["nm_response"]["response_code"], "100")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `wkl-nmi-0.0.8/src/test/test_pay.py` & `wkl-nmi-0.0.9/src/test/test_pay.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/test/test_plans.py` & `wkl-nmi-0.0.9/src/test/test_plans.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/test/test_subscriptions.py` & `wkl-nmi-0.0.9/src/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wkl_nmi.egg-info/PKG-INFO` & `wkl-nmi-0.0.9/src/wkl_nmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkl-nmi
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Nmi library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkl-nmi-0.0.8/src/wkl_nmi.egg-info/SOURCES.txt` & `wkl-nmi-0.0.9/src/wkl_nmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wknmi/auth.py` & `wkl-nmi-0.0.9/src/wknmi/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import google.auth.transport.requests
 import google.oauth2.id_token
 
 
 def get_id_token(audience):
 
+    print("audience", audience)
     if audience == "http://127.0.0.1:8000":
         return ""
 
     """
     make_authorized_get_request makes a GET request to the specified HTTP endpoint
     by authenticating with the ID token obtained from the google-auth client library
     using the specified audience value.
```

### Comparing `wkl-nmi-0.0.8/src/wknmi/billing.py` & `wkl-nmi-0.0.9/src/wknmi/billing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 from wknmi.auth import get_id_token
-import requests 
+import requests
 
-class Billing():
+
+class Billing:
     def __init__(self, url, org):
         self.url = url
         self.org = org
 
     def add(self, body):
-        """add billing id """
+        """add billing id"""
         _token_id = get_id_token(self.url)
-        headers = {'Authorization': 'Bearer ' + _token_id}
-        response = requests.post(f'{self.url}/billing/add', headers=headers, json=body)
+        headers = {"Authorization": "Bearer " + _token_id}
+        response = requests.post(f"{self.url}/billing/add", headers=headers, json=body)
         return {"response": response.json(), "status_code": response.status_code}
-    
+
     def update_billing_info(self, body):
-        """update billing id """
+        """update billing id"""
         _token_id = get_id_token(self.url)
-        headers = {'Authorization': 'Bearer ' + _token_id}
-        response = requests.put(f'{self.url}/billing/update-billing-info', headers=headers, json=body)
+        headers = {"Authorization": "Bearer " + _token_id}
+        response = requests.put(
+            f"{self.url}/billing/update-billing-info", headers=headers, json=body
+        )
         return {"response": response.json(), "status_code": response.status_code}
-        
+
     def delete(self, org, user_id, billing_id):
-        """delete billing id """
+        """delete billing id"""
         _token_id = get_id_token(self.url)
-        headers = {'Authorization': 'Bearer ' + _token_id}
-        response = requests.delete(f'{self.url}/billing/delete?org={org}&user_id={user_id}&billing_id={billing_id}', headers=headers)
+        headers = {"Authorization": "Bearer " + _token_id}
+        response = requests.delete(
+            f"{self.url}/billing/delete?org={org}&user_id={user_id}&billing_id={billing_id}",
+            headers=headers,
+        )
         return {"response": response.json(), "status_code": response.status_code}
-    
+
     def set_priority(self, body):
         """change billing id priority"""
         _token_id = get_id_token(self.url)
-        headers = {'Authorization': 'Bearer ' + _token_id}
-        response = requests.put(f'{self.url}/billing/change-priority', headers=headers, json=body)
+        headers = {"Authorization": "Bearer " + _token_id}
+        response = requests.put(
+            f"{self.url}/billing/change-priority", headers=headers, json=body
+        )
         return {"response": response.json(), "status_code": response.status_code}
-    
 
-    def info(self, org, user_id):
+    def info(self, org, transaction_id):
         """get billing info"""
         _token_id = get_id_token(self.url)
-        headers = {'Authorization': 'Bearer ' + _token_id}
-        response = requests.get(f'{self.url}/billing/billing-of-user?org={org}&user_id={user_id}', headers=headers)
-        return {"response": response.json(), "status_code": response.status_code}
+        headers = {"Authorization": "Bearer " + _token_id}
+        response = requests.get(
+            f"{self.url}/billing/billing-of-user?org={org}&transaction_id={transaction_id}",
+            headers=headers,
+        )
+        return {"response": response.json(), "status_code": response.status_code}
```

### Comparing `wkl-nmi-0.0.8/src/wknmi/config.py` & `wkl-nmi-0.0.9/src/wknmi/config.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wknmi/customer_vault.py` & `wkl-nmi-0.0.9/src/wknmi/customer_vault.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wknmi/payment.py` & `wkl-nmi-0.0.9/src/wknmi/payment.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wknmi/plans.py` & `wkl-nmi-0.0.9/src/wknmi/plans.py`

 * *Files identical despite different names*

### Comparing `wkl-nmi-0.0.8/src/wknmi/subscriptions.py` & `wkl-nmi-0.0.9/src/wknmi/subscriptions.py`

 * *Files identical despite different names*

