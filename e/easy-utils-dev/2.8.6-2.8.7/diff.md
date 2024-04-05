# Comparing `tmp/easy_utils_dev-2.8.6.tar.gz` & `tmp/easy_utils_dev-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.8.6.tar", last modified: Thu Apr  4 15:43:33 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.8.7.tar", last modified: Fri Apr  5 13:43:14 2024, max compression
```

## Comparing `easy_utils_dev-2.8.6.tar` & `easy_utils_dev-2.8.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:43:33.248020 easy_utils_dev-2.8.6/
--rw-rw-rw-   0        0        0      174 2024-04-04 15:43:33.243137 easy_utils_dev-2.8.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 15:43:33.202124 easy_utils_dev-2.8.6/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.6/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.6/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      339 2024-04-04 13:44:23.000000 easy_utils_dev-2.8.6/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.6/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.6/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.6/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7730 2024-04-04 15:43:25.000000 easy_utils_dev-2.8.6/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.6/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.6/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.6/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.6/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.6/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.6/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 11:55:23.000000 easy_utils_dev-2.8.6/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:43:33.238255 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-04 15:43:33.000000 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2024-04-04 15:43:33.000000 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:43:33.000000 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 15:43:33.000000 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 15:43:33.000000 easy_utils_dev-2.8.6/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 15:43:33.248020 easy_utils_dev-2.8.6/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-04 15:43:29.000000 easy_utils_dev-2.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.218496 easy_utils_dev-2.8.7/
+-rw-rw-rw-   0        0        0      174 2024-04-05 13:43:14.213613 easy_utils_dev-2.8.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.151573 easy_utils_dev-2.8.7/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.7/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.7/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.7/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.7/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.7/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.7/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     6147 2024-04-05 13:42:50.000000 easy_utils_dev-2.8.7/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7828 2024-04-04 18:36:57.000000 easy_utils_dev-2.8.7/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.7/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.7/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.7/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.7/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.7/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.7/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.7/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.208733 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:43:14.219473 easy_utils_dev-2.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-05 13:43:07.000000 easy_utils_dev-2.8.7/setup.py
```

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.8.7/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/Events.py` & `easy_utils_dev-2.8.7/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.8.7/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/debugger.py` & `easy_utils_dev-2.8.7/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.8.7/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/lralib.py` & `easy_utils_dev-2.8.7/easy_utils_dev/lralib.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib3
 from threading import Thread
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 version = '1.0 build 22032024'
 
 class LraLib :
-    def __init__(self, address,  user, password,port=8443 ,debug_name='lralib', token_refresh_period=1700) -> None:
+    def __init__(self, address,  user, password,port=8443 ,debug_name='lralib', token_refresh_period=1700 , client_id='wp-lra-service',client_secret='c74b4dfb-4293-46da-a38a-9fd46fce23b0' ) -> None:
         '''
         address: string
         token_refresh_period number , string
         password : string
         port : int
         debug_name : string
         '''
@@ -20,15 +20,16 @@
         self.address = address
         self.port = port
         self.baseUrl = f'https://{self.address}:{self.port}'
         self.username = user
         self.password = password
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
-        self.client_id='wp-lra-service'
+        self.client_id=client_id
+        self.client_secret = client_secret
         self.baseUrl = self.updateBaseUrl(address , port )
 
     def set_debug_level(self , level ) :
         self.logger.set_level(level)    
 
     def updateBaseUrl( self, address, port ) :
             self.baseUrl = f"https://{address}:{port}"
@@ -57,16 +58,16 @@
         url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
         self.logger.info(f"Authentication Params: username={self.username} password=********")
         self.logger.info(f"Authentication Params: username={self.username} password={self.password} url={url}")
         payload = {
             'grant_type': 'password',
             'username': self.username ,
             'password': self.password,
-            'client_id': 'wp-lra-service',
-            'client_secret': 'c74b4dfb-4293-46da-a38a-9fd46fce23b0'
+            'client_id': self.client_id,
+            'client_secret': self.client_secret
         }
         headers = {'Content-type': 'application/x-www-form-urlencoded' }
         self.logger.debug(f'Authentication Payload: {payload}')
         response = requests.post(url , data=payload , headers=headers , verify=False)
         self.logger.info(f'Authentication response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code != 200 :
```

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.8.7/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.8.7/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.8.7/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.8.7/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/utils.py` & `easy_utils_dev-2.8.7/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.8.7/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.8.7/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.6/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.8.7/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 easy_utils_dev/EasySsh.py
 easy_utils_dev/Events.py
 easy_utils_dev/__init__.py
 easy_utils_dev/custom_env.py
 easy_utils_dev/debugger.py
 easy_utils_dev/encryptor.py
+easy_utils_dev/keycloakapi.py
 easy_utils_dev/lralib.py
 easy_utils_dev/ne1830PSS.py
 easy_utils_dev/optics_utils.py
 easy_utils_dev/simple_sqlite.py
 easy_utils_dev/uiserver.py
 easy_utils_dev/utils.py
 easy_utils_dev/wsnoclib.py
```

