# Comparing `tmp/avassa-client-2024.1.1.tar.gz` & `tmp/avassa-client-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avassa-client-2024.1.1.tar", last modified: Thu Jan 18 11:09:54 2024, max compression
+gzip compressed data, was "avassa-client-2024.4.0.tar", last modified: Fri Apr  5 12:39:54 2024, max compression
```

## Comparing `avassa-client-2024.1.1.tar` & `avassa-client-2024.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2024-01-18 11:09:54.017088 avassa-client-2024.1.1/
--rw-r--r--   0 denis     (1000) denis     (1000)    11343 2023-12-20 11:34:34.000000 avassa-client-2024.1.1/LICENSE
--rw-r--r--   0 denis     (1000) denis     (1000)    14236 2024-01-18 11:09:54.017088 avassa-client-2024.1.1/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)      758 2024-01-17 09:52:33.000000 avassa-client-2024.1.1/README.md
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2024-01-18 11:09:54.017088 avassa-client-2024.1.1/avassa_client/
--rw-r--r--   0 denis     (1000) denis     (1000)    10407 2024-01-15 12:52:28.000000 avassa-client-2024.1.1/avassa_client/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)    17628 2024-01-17 09:54:46.000000 avassa-client-2024.1.1/avassa_client/volga.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2024-01-18 11:09:54.017088 avassa-client-2024.1.1/avassa_client.egg-info/
--rw-r--r--   0 denis     (1000) denis     (1000)    14236 2024-01-18 11:09:54.000000 avassa-client-2024.1.1/avassa_client.egg-info/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)      265 2024-01-18 11:09:54.000000 avassa-client-2024.1.1/avassa_client.egg-info/SOURCES.txt
--rw-r--r--   0 denis     (1000) denis     (1000)        1 2024-01-18 11:09:54.000000 avassa-client-2024.1.1/avassa_client.egg-info/dependency_links.txt
--rw-r--r--   0 denis     (1000) denis     (1000)       15 2024-01-18 11:09:54.000000 avassa-client-2024.1.1/avassa_client.egg-info/requires.txt
--rw-r--r--   0 denis     (1000) denis     (1000)       14 2024-01-18 11:09:54.000000 avassa-client-2024.1.1/avassa_client.egg-info/top_level.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      654 2024-01-18 11:09:10.000000 avassa-client-2024.1.1/pyproject.toml
--rw-r--r--   0 denis     (1000) denis     (1000)       38 2024-01-18 11:09:54.017088 avassa-client-2024.1.1/setup.cfg
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.110092 avassa-client-2024.4.0/
+-rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa-client-2024.4.0/LICENSE
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-05 12:39:54.109761 avassa-client-2024.4.0/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      758 2024-01-15 13:20:32.000000 avassa-client-2024.4.0/README.md
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.108776 avassa-client-2024.4.0/avassa_client/
+-rw-r--r--   0 frja       (501) staff       (20)    10414 2024-04-05 12:14:05.000000 avassa-client-2024.4.0/avassa_client/__init__.py
+-rw-r--r--   0 frja       (501) staff       (20)    17620 2024-01-15 13:06:43.000000 avassa-client-2024.4.0/avassa_client/volga.py
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.109559 avassa-client-2024.4.0/avassa_client.egg-info/
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      265 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 frja       (501) staff       (20)        1 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 frja       (501) staff       (20)       15 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/requires.txt
+-rw-r--r--   0 frja       (501) staff       (20)       14 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/top_level.txt
+-rw-r--r--   0 frja       (501) staff       (20)      654 2024-04-05 12:15:21.000000 avassa-client-2024.4.0/pyproject.toml
+-rw-r--r--   0 frja       (501) staff       (20)       38 2024-04-05 12:39:54.110146 avassa-client-2024.4.0/setup.cfg
```

### Comparing `avassa-client-2024.1.1/LICENSE` & `avassa-client-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avassa-client-2024.1.1/PKG-INFO` & `avassa-client-2024.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.1.1
+Version: 2024.4.0
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa-client-2024.1.1/README.md` & `avassa-client-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `avassa-client-2024.1.1/avassa_client/__init__.py` & `avassa-client-2024.4.0/avassa_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         return (response.getcode(),
                 response.msg,
                 response.getheaders(),
                 response.read().decode('utf-8'))
 
 
 def approle_login(host: str,
-                  role_id: str,
+                  role_id: str | None,
                   secret_id: str,
                   user_agent: Optional[str] = None,
                   server_hostname: Optional[str] = None):
     try:
         payload = {'secret-id': secret_id}
         if role_id is not None:
             payload['role-id'] = role_id
```

### Comparing `avassa-client-2024.1.1/avassa_client/volga.py` & `avassa-client-2024.4.0/avassa_client/volga.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         self.log.debug("more payload: %s", cmd)
         await self._ws.send(json.dumps(cmd).encode('utf-8'))
 
     async def recv(self, auto_more=10):
         msg_raw = await self._ws.recv()
         msg = json.loads(msg_raw.decode('utf-8'))
         self.log.debug("recv %s", msg_raw)
-        if auto_more and (msg.get('remain') == 0):
+        if auto_more and (msg['remain'] == 0):
             await self.more(auto_more)
         seqno = msg.get('seqno')
         if seqno is not None:
             self.last_seqno = seqno
         return msg
 
     async def ack(self, seqno=None):
@@ -443,15 +443,15 @@
         self.log.debug("more payload: %s", cmd)
         await self._ws.send(json.dumps(cmd).encode('utf-8'))
 
     async def recv(self, auto_more=10):
         msg_raw = await self._ws.recv()
         msg = json.loads(msg_raw.decode('utf-8'))
         self.log.debug("recv %s", msg_raw)
-        if auto_more and (msg.get('remain') == 0):
+        if auto_more and (msg['remain'] == 0):
             await self.more(auto_more)
         seqno = msg.get('seqno')
         if seqno is not None:
             self.last_seqno = seqno
         return msg
 
     async def ack(self, seqno=None):
```

### Comparing `avassa-client-2024.1.1/avassa_client.egg-info/PKG-INFO` & `avassa-client-2024.4.0/avassa_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.1.1
+Version: 2024.4.0
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa-client-2024.1.1/pyproject.toml` & `avassa-client-2024.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avassa-client"
-version = "2024.1.1"
+version = "2024.4.0"
 description = "Library for integrating with the Avassa APIs"
 readme = "README.md"
 authors = [{ name = "Avassa", email = "info@avassa.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

