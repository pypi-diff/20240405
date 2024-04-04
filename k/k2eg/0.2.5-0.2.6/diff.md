# Comparing `tmp/k2eg-0.2.5.tar.gz` & `tmp/k2eg-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k2eg-0.2.5.tar", last modified: Thu Apr  4 03:41:34 2024, max compression
+gzip compressed data, was "k2eg-0.2.6.tar", last modified: Thu Apr  4 23:40:31 2024, max compression
```

## Comparing `k2eg-0.2.5.tar` & `k2eg-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 03:41:34.120003 k2eg-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 03:41:16.000000 k2eg-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.116003 k2eg-0.2.5/k2eg/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/k2eg/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/put.py
--rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/dml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/k2eg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 03:41:20.000000 k2eg-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:41:34.120003 k2eg-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 03:41:16.000000 k2eg-0.2.5/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-04 03:41:16.000000 k2eg-0.2.5/tests/test_dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 23:40:31.723717 k2eg-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 23:40:07.000000 k2eg-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.719717 k2eg-0.2.6/k2eg/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/k2eg/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/cli/put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-04-04 23:40:07.000000 k2eg-0.2.6/k2eg/dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/k2eg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 23:40:31.000000 k2eg-0.2.6/k2eg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 23:40:16.000000 k2eg-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:40:31.723717 k2eg-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:40:31.723717 k2eg-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 23:40:07.000000 k2eg-0.2.6/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-04 23:40:07.000000 k2eg-0.2.6/tests/test_dml.py
```

### Comparing `k2eg-0.2.5/PKG-INFO` & `k2eg-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.5
+Version: 0.2.6
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.5/README.md` & `k2eg-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/broker.py` & `k2eg-0.2.6/k2eg/broker.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/cli/__main__.py` & `k2eg-0.2.6/k2eg/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/cli/get.py` & `k2eg-0.2.6/k2eg/cli/get.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/cli/monitor.py` & `k2eg-0.2.6/k2eg/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/cli/put.py` & `k2eg-0.2.6/k2eg/cli/put.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.5/k2eg/dml.py` & `k2eg-0.2.6/k2eg/dml.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                         continue
                     with self.reply_wait_condition:
                         was_a_reply = msg_id in self.reply_message
                         if was_a_reply is True:
                             # print(f"message received from topic: {message.topic()} offset: {message.offset()}")
                             logging.debug(f"received reply on topic {message.topic()}")
                             self.reply_message[msg_id] = decoded_message
-                            self.reply_wait_condition.notifyAll()
+                            self.reply_wait_condition.notify_all()
                         elif msg_id in self.__monitor_pv_handler:
                                 executor.submit(
                                     self.process_event,
                                     message.topic(),
                                     msg_id,
                                     decoded_message[msg_id]
                                 )
@@ -174,29 +174,28 @@
         pass
 
     def __normalize_pv_name(self, pv_name):
         return pv_name.replace(":", "_")
 
     def __wait_for_reply(self, new_reply_id, timeout) -> (int, any):
         #with self.reply_wait_condition:
-        got_it = self.reply_wait_condition.wait(timeout)
-        if(got_it is False):
-            # the timeout is expired, so delete the answer slot
-            # and rise exception
-            del(self.reply_message[new_reply_id])
+        got_it = self.reply_wait_condition.wait_for(
+            lambda: new_reply_id in self.reply_message and self.reply_message[new_reply_id] is not None,
+            timeout
+        )
+        if not got_it:
+            # The timeout has expired and no message was received
             return -2, None
-        if self.reply_message[new_reply_id] is None:
-            return -1
-        reply_msg = self.reply_message[new_reply_id]
-        del(self.reply_message[new_reply_id])
-        error = reply_msg['error']
+        reply_msg = self.reply_message.pop(new_reply_id, None)
+        if reply_msg is None:
+            # This should not occur due to the lambda check, but added as a safety net
+            return -1, None
+        error = reply_msg.get('error', 0)
         if error != 0:
-            str_msg = None
-            if 'message' in reply_msg:
-                str_msg = reply_msg['message']   
+            str_msg = reply_msg.get('message', None)
             raise OperationError(error, str_msg)
         return 0, reply_msg
 
     def wait_for_backends(self):
         logging.debug("Waiting for join kafka reply topic")
         self.__broker.wait_for_reply_available()
 
@@ -220,15 +219,15 @@
                 new_reply_id
             )
             while(not fetched):
                 op_res, result =  self.__wait_for_reply(new_reply_id, timeout)
                 if op_res == -2:
                     # raise timeout exception
                     raise OperationTimeout(
-                            f"Timeout during start monitor operation for {pv_name}"
+                            f"Timeout during get operation for {pv_name}"
                             )
                 elif op_res == -1:
                     continue
                 else:
                     fetched = True
         if result is not None and pv_name in result:
             return result[pv_name]
@@ -265,15 +264,15 @@
                 new_reply_id
             )
             while(not fetched):
                 op_res, result =  self.__wait_for_reply(new_reply_id, timeout)
                 if op_res == -2:
                     # raise timeout exception
                     raise OperationTimeout(
-                            f"Timeout during start monitor operation for {pv_name}"
+                            f"Timeout during start get operation for {pv_name}"
                             )
                 elif op_res == -1:
                     continue
                 else:
                     return result
```

### Comparing `k2eg-0.2.5/k2eg.egg-info/PKG-INFO` & `k2eg-0.2.6/k2eg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.5
+Version: 0.2.6
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.5/pyproject.toml` & `k2eg-0.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "k2eg"
-version = "0.2.5"
+version = "0.2.6"
 description = "A k2eg library"
 readme = "README.md"
 authors = [{name = "Claudio Bisegni", email = "bisegni@slac.stanford.edu"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `k2eg-0.2.5/tests/test_dml.py` & `k2eg-0.2.6/tests/test_dml.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from concurrent.futures import ThreadPoolExecutor
 import logging
 import k2eg
 from k2eg.dml import _filter_pv_uri
 import time
 import pytest
 from unittest import TestCase
 
@@ -138,14 +139,37 @@
     k.put("pva://variable:a", 2)
     k.put("pva://variable:b", 2)
     #give some time to ioc to update
     time.sleep(1)
     res_get = k.get("pva://variable:sum")
     assert res_get['value'] == 4, "value should not be 0"
 
+def test_multi_threading_put():
+    put_dic={
+        "pva://variable:a": 0,
+        "pva://variable:b": 0
+    }
+    with ThreadPoolExecutor(10) as executor:
+        for key, value in put_dic.items():
+            executor.submit(put, key, value)
+    time.sleep(5)
+    res_get = k.get("pva://variable:sum")
+    assert res_get['value'] == 0, "value should not be 0"
+    put_dic={
+        "pva://variable:a": 2,
+        "pva://variable:b": 2
+    }
+    with ThreadPoolExecutor(10) as executor:
+        for key, value in put_dic.items():
+            executor.submit(put, key, value)
+    #give some time to ioc to update
+    time.sleep(5)
+    res_get = k.get("pva://variable:sum")
+    assert res_get['value'] == 4, "value should not be 0"
+
 # def test_multiple_put():
 #     def monitor_handler(pv_name, new_value):
 #        pass
         
 #     monitor_pv = [
 #                     'ca://SOLN:IN20:121:BACT',
 #                     'ca://QUAD:IN20:121:BACT',
@@ -160,27 +184,33 @@
 #                     'ca://QUAD:IN20:441:BACT',
 #                     'ca://QUAD:IN20:511:BACT',
 #                     'ca://QUAD:IN20:525:BACT',
 #                     'ca://FBCK:BCI0:1:CHRG_S',
 #                     'ca://CAMR:IN20:186:XRMS',
 #                     'ca://CAMR:IN20:186:YRMS'
 #                     ]
-#     k.monitor_many(monitor_pv, monitor_handler)
+#     #k.monitor_many(monitor_pv, monitor_handler)
 #     monitor_put = {
-#         'LUME:MLFLOW:SIGMA_X': '-99830.6330126242',
-#         'LUME:MLFLOW:SIGMA_Y': '225322.341204345',
-#         'LUME:MLFLOW:SIGMA_Z': '10352.2788770893'
+#         'pva://LUME:MLFLOW:SIGMA_X': '-99830.6330126242',
+#         'pva://LUME:MLFLOW:SIGMA_Y': '225322.341204345',
+#         'pva://LUME:MLFLOW:SIGMA_Z': '10352.2788770893'
 #     }
-#     for key, value in monitor_put.items():  # Add .items() method to iterate over key-value pairs
-#         print(f"Output: {key}, Value: {value}")  # Update print statement to use f-strings
-#         try:
-#             msg = k.put("pva://" + key, value, 1000000)
-#             print(f"Message: {msg}")
-#         except Exception as e:
-#             print(f"An error occurred: {e}")
+#     time_start = time.time()
+#     with ThreadPoolExecutor(10) as executor:
+#         for key, value in monitor_put.items():
+#             executor.submit(put, key, value)
+#     time_end = time.time()
+#     print(f"Time taken to put: {time_end - time_start} - {(time_end - time_start)/len(monitor_put) })")
+
+def put(key, value):
+    try:
+        k.put(key, value, 10)
+        print(f"Put {key} with value {value}")
+    except Exception as e:
+        print(f"An error occured: {e}")
 
 def test_put_timeout():
     with pytest.raises(k2eg.OperationTimeout, 
                     match=r"Timeout.*"):
                     k.put("pva://bad:pv:name", 0, timeout=0.5)
```

