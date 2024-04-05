# Comparing `tmp/easy_utils_dev-2.8.7.tar.gz` & `tmp/easy_utils_dev-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.8.7.tar", last modified: Fri Apr  5 13:43:14 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.8.8.tar", last modified: Fri Apr  5 14:41:23 2024, max compression
```

## Comparing `easy_utils_dev-2.8.7.tar` & `easy_utils_dev-2.8.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.218496 easy_utils_dev-2.8.7/
--rw-rw-rw-   0        0        0      174 2024-04-05 13:43:14.213613 easy_utils_dev-2.8.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.151573 easy_utils_dev-2.8.7/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.7/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.7/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.7/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.7/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.7/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.7/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     6147 2024-04-05 13:42:50.000000 easy_utils_dev-2.8.7/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7828 2024-04-04 18:36:57.000000 easy_utils_dev-2.8.7/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.7/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.7/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.7/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.7/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.7/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.7/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.7/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:43:14.208733 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 13:43:13.000000 easy_utils_dev-2.8.7/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 13:43:14.219473 easy_utils_dev-2.8.7/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-05 13:43:07.000000 easy_utils_dev-2.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.426321 easy_utils_dev-2.8.8/
+-rw-rw-rw-   0        0        0      174 2024-04-05 14:41:23.420463 easy_utils_dev-2.8.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.364811 easy_utils_dev-2.8.8/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.8/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.8/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.8/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.8/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.8/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.8/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7186 2024-04-05 14:41:01.000000 easy_utils_dev-2.8.8/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7829 2024-04-05 13:44:11.000000 easy_utils_dev-2.8.8/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.8/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.8/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.8/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.8/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.8/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.8/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.8/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.413640 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:41:23.426321 easy_utils_dev-2.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-05 14:41:16.000000 easy_utils_dev-2.8.8/setup.py
```

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.8.8/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/Events.py` & `easy_utils_dev-2.8.8/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.8.8/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/debugger.py` & `easy_utils_dev-2.8.8/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.8.8/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.8.8/easy_utils_dev/keycloakapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.logger.info(f'Auto Token refresh completed.')
 
 
     def authentication(self,autoRefresh=True) :
         self.logger.info('Starting to authenticate with KeyCloack platform ..')
         url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
         self.logger.info(f"Authentication Params: username={self.username} password=********")
-        self.logger.info(f"Authentication Params: username={self.username} password={self.password} url={url}")
+        self.logger.debug(f"Authentication Params: username={self.username} password={self.password} url={url}")
         payload = {
             'grant_type': 'client_credentials',
             'username': self.username ,
             'password': self.password,
             'client_id': self.client_id ,
             'client_secret': self.client_secret
         }
@@ -116,29 +116,46 @@
         self.logger.debug(f'Logout out payload {payload}')
         response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
         self.logger.debug(f'raw response in logout {response.text}')
         self.logger.info(f'Logout status code={response.status_code}')
 
     def getUsers(self) :
         self.logger.info(f"Get users from KeyCloack ...")
-        url= f"{self.baseUrl}/KeyCloack-rest/users"
+        url= f"{self.baseUrl}/wavesuite/common/auth/admin/realms/wavesuite/users/"
         headers = self.getHeaders()
         self.logger.debug(f'Get users headers = {headers}')
         response = requests.get(url , headers=headers , verify=False)
         self.logger.info(f'Get Usr response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code == 200 :
             self.logger.debug(f'response is 200 , return the json as dict and filter on data ...')
-            self.users = response.json().get('items')
+            self.users = response.json()
             return self.users
         else :
             self.logger.error(f'Error getting users  {response.text}')
             self.logger.debug(f'response is not 200 , return empty array')
             self.users = []
             return []
 
-
+    def updateUser(self , user ) :
+        userId=user.get('id')
+        username=user.get('username')
+        self.logger.info(f"Update user in KeyCloack for userId={userId} username={username}")
+        url= f"{self.baseUrl}/wavesuite/common/auth/admin/realms/wavesuite/users/{userId}"
+        headers = self.getHeaders()
+        self.logger.debug(f'update user headers = {headers}')
+        response = requests.put(url , headers=headers, body=json.dumps(user) , verify=False)
+        self.logger.info(f'update Usr response code={response.status_code}')
+        self.logger.debug(f'raw response in user update {response.text}')
+        if response.status_code == 204 :
+            self.logger.debug(f'response is 204 , return the json as dict and filter on data ...')
+            return True
+        else :
+            self.logger.error(f'Error getting users  {response.text}')
+            self.logger.debug(f'response is not 204. return False error={response.text}')
+            return False
+        
 if __name__ == '__main__':
     pass
```

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/lralib.py` & `easy_utils_dev-2.8.8/easy_utils_dev/lralib.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.logger.info(f'Auto Token refresh completed.')
 
 
     def authentication(self,autoRefresh=True) :
         self.logger.info('Starting to authenticate with LRA platform ..')
         url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
         self.logger.info(f"Authentication Params: username={self.username} password=********")
-        self.logger.info(f"Authentication Params: username={self.username} password={self.password} url={url}")
+        self.logger.debug(f"Authentication Params: username={self.username} password={self.password} url={url}")
         payload = {
             'grant_type': 'password',
             'username': self.username ,
             'password': self.password,
             'client_id': self.client_id,
             'client_secret': self.client_secret
         }
```

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.8.8/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.8.8/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.8.8/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.8.8/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/utils.py` & `easy_utils_dev-2.8.8/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.8.8/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.8.8/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.7/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.8.8/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

