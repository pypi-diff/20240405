# Comparing `tmp/btc_embedded-24.1.0.tar.gz` & `tmp/btc_embedded-24.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-24.1.0.tar", last modified: Fri Apr  5 08:59:29 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.1.tar", last modified: Fri Apr  5 09:04:07 2024, max compression
```

## Comparing `btc_embedded-24.1.0.tar` & `btc_embedded-24.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.552547 btc_embedded-24.1.0/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 08:59:29.552612 btc_embedded-24.1.0/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.551936 btc_embedded-24.1.0/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    21227 2024-04-05 08:58:56.000000 btc_embedded-24.1.0/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.0/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.552448 btc_embedded-24.1.0/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-05 08:59:29.552798 btc_embedded-24.1.0/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-05 08:58:56.000000 btc_embedded-24.1.0/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:04:07.684568 btc_embedded-24.1.1/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 09:04:07.684633 btc_embedded-24.1.1/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:04:07.683747 btc_embedded-24.1.1/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    20790 2024-04-05 09:03:23.000000 btc_embedded-24.1.1/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.1/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.1/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:04:07.684441 btc_embedded-24.1.1/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 09:04:07.000000 btc_embedded-24.1.1/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-05 09:04:07.000000 btc_embedded-24.1.1/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-05 09:04:07.000000 btc_embedded-24.1.1/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-05 09:04:07.000000 btc_embedded-24.1.1/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-05 09:04:07.000000 btc_embedded-24.1.1/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-05 09:04:07.684812 btc_embedded-24.1.1/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-05 09:04:05.000000 btc_embedded-24.1.1/setup.py
```

### Comparing `btc_embedded-24.1.0/LICENSE.txt` & `btc_embedded-24.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/PKG-INFO` & `btc_embedded-24.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 24.1.0
+Version: 24.1.1
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.0/README.md` & `btc_embedded-24.1.1/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded/api.py` & `btc_embedded-24.1.1/btc_embedded/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,14 @@
             return
         start_time = time.time()
         print(f'Connecting to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
         while not self._is_rest_service_available():
             if (time.time() - start_time) > timeout:
                 print(f"\n\nCould not connect to EP within the specified timeout of {timeout} seconds. \n\n")
                 raise Exception("Application didn't respond within the defined timeout.")
-            elif (self.ep_process.poll() is None):
-                print(f"\n\nApplication failed to start. Please check the log file for further information:\n{self.log_file_path}\n\n")
-                raise Exception("Application failed to start.")
             time.sleep(2)
             print('.', end='')
         print('\nBTC EmbeddedPlatform has started.')
         self._apply_preferences(config)
 
     # - - - - - - - - - - - - - - - - - - - - 
     #   PUBLIC FUNCTIONS
@@ -327,15 +324,15 @@
         # container use case -> start EP and Matlab
         try:
             ep_ini_path = os.path.join(os.environ['EP_INSTALL_PATH'], 'ep.ini')
             with open(ep_ini_path, 'r') as file:
                 content = file.read()
             version = re.search(r'/ep/(\d+\.\d+[a-zA-Z]*\d+)/', content).group(1)
         except:
-            version = '24.1p0'
+            version = '23.3p0'
         headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
         matlab_ip = os.environ['MATLAB_IP'] if 'MATLAB_IP' in os.environ else '127.0.0.1'
         print(f'Waiting for BTC EmbeddedPlatform {version} to be available:')
 
         args = [ os.environ['EP_INSTALL_PATH'] + '/ep',
             '-clearPersistedState', '-nosplash', '-console', '-consoleLog',
             '-application', headless_application_id,            
@@ -351,16 +348,15 @@
             '-Dosgi.configuration.area.default=/tmp/ep/configuration',
             '-Dosgi.instance.area.default=/tmp/ep/workspace',
             '-Dep.runtime.batch=ep',
             '-Dep.runtime.api.port=1109',
             '-Dep.matlab.ip.range=' + matlab_ip ]
         
         # start ep process
-        self.ep_process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        self.log_file_path = os.environ['LOG_DIR'] + '/current.log'
+        subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         self.actively_started = True
         
         # if container has matlab -> assume that this shall be started as well
         if shutil.which('matlab'): subprocess.Popen('matlab')
 
 
     def _start_app_windows(self, version, install_location, port, license_location, lic, config):
@@ -394,15 +390,14 @@
             ' -Dosgi.instance.area.default="' + appdata_location + self._PORT_ + '/workspace"' + \
             ' -Dep.configuration.logpath=AppData/Roaming/BTC/ep/' + version + '/' + self._PORT_ + '/logs' + \
             ' -Dep.runtime.workdir=BTC/ep/' + version + '/' + self._PORT_ + \
             ' -Dep.licensing.package=' + lic + \
             ' -Dep.rest.port=' + self._PORT_
         if license_location or config and 'licenseLocation' in config:
                 f" -Dep.licensing.location={(license_location or config['licenseLocation'])}"
-        self.ep_process = subprocess.Popen(args, stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
-        self.log_file_path = appdata_location + self._PORT_ + '/logs/current.log'
+        subprocess.Popen(args, stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
         self.actively_started = True
 
 
 # if called directly, starts EP based on the global config
 if __name__ == '__main__':
     EPRestApi()
```

### Comparing `btc_embedded-24.1.0/btc_embedded/btc_config.yml` & `btc_embedded-24.1.1/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.1/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded/config.py` & `btc_embedded-24.1.1/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded/reporting.py` & `btc_embedded-24.1.1/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded/util.py` & `btc_embedded-24.1.1/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.0/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.1/btc_embedded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 24.1.0
+Version: 24.1.1
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.0/setup.py` & `btc_embedded-24.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='24.1.0',
+    version='24.1.1',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

