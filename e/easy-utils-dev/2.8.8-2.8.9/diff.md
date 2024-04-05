# Comparing `tmp/easy_utils_dev-2.8.8.tar.gz` & `tmp/easy_utils_dev-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.8.8.tar", last modified: Fri Apr  5 14:41:23 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.8.9.tar", last modified: Fri Apr  5 14:49:27 2024, max compression
```

## Comparing `easy_utils_dev-2.8.8.tar` & `easy_utils_dev-2.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.426321 easy_utils_dev-2.8.8/
--rw-rw-rw-   0        0        0      174 2024-04-05 14:41:23.420463 easy_utils_dev-2.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.364811 easy_utils_dev-2.8.8/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.8/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.8/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.8/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.8/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.8/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.8/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7186 2024-04-05 14:41:01.000000 easy_utils_dev-2.8.8/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7829 2024-04-05 13:44:11.000000 easy_utils_dev-2.8.8/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.8/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.8/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.8/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.8/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.8/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.8/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.8/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:23.413640 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 14:41:23.000000 easy_utils_dev-2.8.8/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:41:23.426321 easy_utils_dev-2.8.8/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-05 14:41:16.000000 easy_utils_dev-2.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.861501 easy_utils_dev-2.8.9/
+-rw-rw-rw-   0        0        0      174 2024-04-05 14:49:27.856618 easy_utils_dev-2.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.788974 easy_utils_dev-2.8.9/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.9/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.9/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.9/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.9/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.9/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.9/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7180 2024-04-05 14:49:15.000000 easy_utils_dev-2.8.9/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7829 2024-04-05 13:44:11.000000 easy_utils_dev-2.8.9/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.9/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.9/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.9/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.9/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.9/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.9/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.9/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.850760 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:49:27.861501 easy_utils_dev-2.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-05 14:49:23.000000 easy_utils_dev-2.8.9/setup.py
```

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.8.9/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/Events.py` & `easy_utils_dev-2.8.9/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.8.9/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/debugger.py` & `easy_utils_dev-2.8.9/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.8.9/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.8.9/easy_utils_dev/keycloakapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib3
 from threading import Thread
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 version = '1.0 build 22032024'
 
 class KeyCloack :
-    def __init__(self, address,  user, password,port=8443 ,debug_name='keycloackapi', token_refresh_period=1700, client_id='wp-KeyCloack-service',client_secret='c74b4dfb-4293-46da-a38a-9fd46fce23b0') -> None:
+    def __init__(self, address,  user, password,port=8443 ,debug_name='keycloackapi', token_refresh_period=1700, client_id='wp-lra-service',client_secret='c74b4dfb-4293-46da-a38a-9fd46fce23b0') -> None:
         '''
         address: string
         token_refresh_period number , string
         password : string
         port : int
         debug_name : string
         '''
```

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/lralib.py` & `easy_utils_dev-2.8.9/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.8.9/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.8.9/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.8.9/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.8.9/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/utils.py` & `easy_utils_dev-2.8.9/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.8.9/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.8.9/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.8/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.8.9/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

