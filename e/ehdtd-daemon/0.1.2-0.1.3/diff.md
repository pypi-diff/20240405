# Comparing `tmp/ehdtd_daemon-0.1.2.tar.gz` & `tmp/ehdtd_daemon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.2.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.3.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.2.tar` & `ehdtd_daemon-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.2/LICENSE
--rw-r--r--   0        0        0     3227 2024-03-31 05:25:31.149699 ehdtd_daemon-0.1.2/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.2/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0     9632 2024-04-04 01:41:43.749676 ehdtd_daemon-0.1.2/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     7213 2024-03-31 05:29:48.675926 ehdtd_daemon-0.1.2/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      582 2024-04-04 01:26:17.025737 ehdtd_daemon-0.1.2/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-04-04 10:26:43.760193 ehdtd_daemon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.3/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.3/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    11668 2024-04-05 09:26:03.505231 ehdtd_daemon-0.1.3/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0     7213 2024-04-05 09:26:48.307492 ehdtd_daemon-0.1.3/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.3/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      705 2024-04-05 07:52:49.150202 ehdtd_daemon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.3/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.2/LICENSE` & `ehdtd_daemon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.2/README.md` & `ehdtd_daemon-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ### Database Configuration
 
 The database configuration section defines parameters for connecting to the database.
 
 #### Parameters
 
-    db_type: The type of database used by the daemon. Supported options are PostgreSQL and MySQL.
+    db_type: The type of database used by the daemon. Supported options are postgresql, pgsql and mysql.
     db_name: The name of the database.
     db_user: The username used to connect to the database.
     db_pass: The password used to authenticate the database user.
     db_host: The hostname or IP address of the database server.
     db_port: The port number on which the database server is listening.
 
 ### Exchange Configuration
@@ -73,15 +73,15 @@
 
 ### Example Configuration
 
 ```yaml
 
 global:
   log_dir: /var/log/ehdtd-daemon
-  run_dir: /run
+  run_dir: /run/ehdtd-daemon
   debug: false
 
 db_data:
   db_type: postgresql
   db_name: 'DB_NAME'
   db_user: 'DB_USER'
   db_pass: 'DB_PASS'
```

### Comparing `ehdtd_daemon-0.1.2/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.3/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.2/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.3/ehdtd_daemon/aux_common_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -92,15 +92,14 @@
             req = urllib.request.Request(url, None, headers)
 
         if req is not None:
             try:
                 with urllib.request.urlopen(req, None, timeout=timeout) as response:
                     result = response.read()
 
-
             except Exception: # pylint: disable=broad-except
                 result = None
 
         if mode != 'b' and result is not None and isinstance(result, bytes):
             result = result.decode()
 
     except Exception: # pylint: disable=broad-except
@@ -285,45 +284,94 @@
     if config_data is not None and schema.is_valid(config_data)\
         and config_data['global'] is not None\
         and schema_global.is_valid(config_data['global']):
         result = True
 
     return result
 
+def create_dir_without_exception(dir_in):
+    """
+    create_dir_without_exception
+    ============================
+
+    """
+    result = None
+    try:
+        if not os.path.exists(dir_in):
+            os.makedirs(dir_in)
+        result = True
+    except Exception: # pylint: disable=broad-except
+        result = False
+
+    return result
+
 def get_config_data(config_file):
     """
     get_config_data
     ===============
 
     """
     result = None
     default_log_dir = '/var/log/ehdtd-daemon'
     default_run_dir = '/run/ehdtd-daemon'
 
+    home_dir = os.getenv('HOME')
+
+    default_home_log_dir = os.path.join(home_dir, '.ehdtd-daemon/var/log')
+    default_home_run_dir = os.path.join(home_dir, '.ehdtd-daemon/var/run')
+
+
     config_data = None
     default_config_file = '/etc/ehdtd-daemon/ehdtd-daemon-config.yaml'
+
     if config_file is not None and isinstance(config_file, str) and os.path.exists(config_file):
         config_data = read_config_yaml(config_file)
     elif os.path.exists(default_config_file):
         config_data = read_config_yaml(default_config_file)
 
     if __check_config_structure(config_data):
         result = config_data
 
         if result['global']['log_dir'] is None or not isinstance(result['global']['log_dir'], str):
             result['global']['log_dir'] = default_log_dir
 
-        if not os.path.exists(result['global']['log_dir']):
-            os.makedirs(result['global']['log_dir'])
+        if not (create_dir_without_exception(result['global']['log_dir'])\
+            and os.access(result['global']['log_dir'], os.W_OK)):
+            result['global']['log_dir'] = default_log_dir
+            if not (create_dir_without_exception(result['global']['log_dir'])\
+                and os.access(result['global']['log_dir'], os.W_OK)):
+                result['global']['log_dir'] = default_home_log_dir
+                if not (create_dir_without_exception(result['global']['log_dir'])\
+                    and os.access(result['global']['log_dir'], os.W_OK)):
+                    return None
 
-        if result['global']['run_dir'] is None or not isinstance(result['global']['run_dir'], str):
+        if not (create_dir_without_exception(result['global']['run_dir'])\
+            and os.access(result['global']['run_dir'], os.W_OK)):
             result['global']['run_dir'] = default_run_dir
-
-        if not os.path.exists(result['global']['run_dir']):
-            os.makedirs(result['global']['run_dir'])
+            if not (create_dir_without_exception(result['global']['run_dir'])\
+                and os.access(result['global']['run_dir'], os.W_OK)):
+                result['global']['run_dir'] = default_home_run_dir
+                if not (create_dir_without_exception(result['global']['run_dir'])\
+                    and os.access(result['global']['run_dir'], os.W_OK)):
+                    return None
+
+        if result['db_data']['db_type'] is not None\
+            and isinstance(result['db_data']['db_type'], str)\
+            and result['db_data']['db_type'] == 'pgsql':
+            result['db_data']['db_type'] = 'postgresql'
+
+        if result['db_data']['db_port'] is None\
+            or result['db_data']['db_port'] is False\
+            or (isinstance(result['db_data']['db_port'], str)\
+                and len(result['db_data']['db_port']) == 0):
+
+            if result['db_data']['db_type'] == 'postgresql':
+                result['db_data']['db_port'] = '5432'
+            elif result['db_data']['db_type'] == 'mysql':
+                result['db_data']['db_port'] = '3306'
 
     return result
 
 def is_pid_running(pid):
     """
     is_pid_running
     ==============
```

### Comparing `ehdtd_daemon-0.1.2/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.3/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.2/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.1.3/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 global:
     log_dir: null # Default /var/log/ehdtd-daemon
     run_dir: null # Default /run/ehdtd-daemon
     debug: false
 
 db_data:
-  db_type: '_DBC_DBTYPE_'  # postgresql, mysql
+  db_type: '_DBC_DBTYPE_'  # postgresql, pgsql, mysql
   db_name: '_DBC_DBNAME_'
   db_user: '_DBC_DBUSER_'
   db_pass: '_DBC_DBPASS_'
   db_host: '_DBC_DBSERVER_'
   db_port: '_DBC_DBPORT_'
 
 exchanges:
```

### Comparing `ehdtd_daemon-0.1.2/pyproject.toml` & `ehdtd_daemon-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.2"
+version = "0.1.3"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
```

### Comparing `ehdtd_daemon-0.1.2/PKG-INFO` & `ehdtd_daemon-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -67,15 +67,15 @@
 
 ### Database Configuration
 
 The database configuration section defines parameters for connecting to the database.
 
 #### Parameters
 
-    db_type: The type of database used by the daemon. Supported options are PostgreSQL and MySQL.
+    db_type: The type of database used by the daemon. Supported options are postgresql, pgsql and mysql.
     db_name: The name of the database.
     db_user: The username used to connect to the database.
     db_pass: The password used to authenticate the database user.
     db_host: The hostname or IP address of the database server.
     db_port: The port number on which the database server is listening.
 
 ### Exchange Configuration
@@ -94,15 +94,15 @@
 
 ### Example Configuration
 
 ```yaml
 
 global:
   log_dir: /var/log/ehdtd-daemon
-  run_dir: /run
+  run_dir: /run/ehdtd-daemon
   debug: false
 
 db_data:
   db_type: postgresql
   db_name: 'DB_NAME'
   db_user: 'DB_USER'
   db_pass: 'DB_PASS'
```

