# Comparing `tmp/btc_embedded-23.3.9.tar.gz` & `tmp/btc_embedded-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-23.3.9.tar", last modified: Fri Mar  8 16:20:50 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.0.tar", last modified: Fri Apr  5 08:59:29 2024, max compression
```

## Comparing `btc_embedded-23.3.9.tar` & `btc_embedded-24.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-03-08 16:20:50.592550 btc_embedded-23.3.9/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-03-08 16:20:50.592622 btc_embedded-23.3.9/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-03-08 16:20:50.591680 btc_embedded-23.3.9/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    20436 2024-03-08 16:20:21.000000 btc_embedded-23.3.9/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-23.3.9/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-23.3.9/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-03-08 16:20:50.592250 btc_embedded-23.3.9/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-03-08 16:20:50.000000 btc_embedded-23.3.9/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-03-08 16:20:50.000000 btc_embedded-23.3.9/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-03-08 16:20:50.000000 btc_embedded-23.3.9/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-03-08 16:20:50.000000 btc_embedded-23.3.9/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-03-08 16:20:50.000000 btc_embedded-23.3.9/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-03-08 16:20:50.592818 btc_embedded-23.3.9/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-03-08 16:20:46.000000 btc_embedded-23.3.9/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.552547 btc_embedded-24.1.0/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 08:59:29.552612 btc_embedded-24.1.0/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.551936 btc_embedded-24.1.0/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    21227 2024-04-05 08:58:56.000000 btc_embedded-24.1.0/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.0/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.0/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 08:59:29.552448 btc_embedded-24.1.0/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-05 08:59:29.000000 btc_embedded-24.1.0/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-05 08:59:29.552798 btc_embedded-24.1.0/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-05 08:58:56.000000 btc_embedded-24.1.0/setup.py
```

### Comparing `btc_embedded-23.3.9/LICENSE.txt` & `btc_embedded-24.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/PKG-INFO` & `btc_embedded-24.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 23.3.9
+Version: 24.1.0
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-23.3.9/README.md` & `btc_embedded-24.1.0/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded/api.py` & `btc_embedded-24.1.0/btc_embedded/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         On Mac and Linux operating systems, the tool start is not handled by the wrapper.
         Instead, it tries to connect to a running instance at the specified port.
         You can call something like
            'docker run -p 1337:8080 -v "/my/workdir:/my/workdir" btces/ep'
         to run the BTC EmbeddedPlatform docker image.
         """
-        self._PORT_ = str(port)
+        self._PORT_ = "8080" if platform.system() == 'Linux' else str(port)
         self._HOST_ = host
         self.definitively_closed = False
         self.actively_started = False
         # use default config, if no config was specified
         if not config: config = get_global_config()
         # apply timeout from config if specified
         if 'startupTimeout' in config: timeout = config['startupTimeout']
@@ -44,23 +44,26 @@
         if not (version and install_location) and 'installationRoot' in config and 'epVersion' in config:
             version = config['epVersion']
             install_location = f"{config['installationRoot']}/ep{config['epVersion']}"
         if not self._is_rest_service_available():
             if platform.system() == 'Windows': self._start_app_windows(version, install_location, port, license_location, lic, config)
             elif platform.system() == 'Linux': self._start_app_linux()
         else:
-            print(f'Connected to BTC EmbeddedPlatform REST API at {host}:{port}')
+            print(f'Connected to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
             self._apply_preferences(config)
             return
         start_time = time.time()
-        print(f'Connecting to BTC EmbeddedPlatform REST API at {host}:{port}')
+        print(f'Connecting to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
         while not self._is_rest_service_available():
             if (time.time() - start_time) > timeout:
                 print(f"\n\nCould not connect to EP within the specified timeout of {timeout} seconds. \n\n")
                 raise Exception("Application didn't respond within the defined timeout.")
+            elif (self.ep_process.poll() is None):
+                print(f"\n\nApplication failed to start. Please check the log file for further information:\n{self.log_file_path}\n\n")
+                raise Exception("Application failed to start.")
             time.sleep(2)
             print('.', end='')
         print('\nBTC EmbeddedPlatform has started.')
         self._apply_preferences(config)
 
     # - - - - - - - - - - - - - - - - - - - - 
     #   PUBLIC FUNCTIONS
@@ -124,14 +127,15 @@
         path = f"/message-markers/{self.message_marker_date}/messages"
         if search_string: path += '?search-string=' + search_string
         if severity: path += ('&' if search_string else '?') + f"severity={severity}"
         messages = self.get(path)
         messages.sort(key=lambda msg: datetime.strptime(msg['date'], DATE_FORMAT))
         for msg in messages:
             print(f"[{msg['severity']}] {msg['message']}" + (f" (Hint: {msg['hint']})" if 'hint' in msg and msg['hint'] else ""))
+        print("\n")
 
     # - - - - - - - - - - - - - - - - - - - - 
     #   DEPRICATED PUBLIC FUNCTIONS
     # - - - - - - - - - - - - - - - - - - - - 
 
     # Performs a get request on the given url extension
     def get_req(self, urlappendix, message=None):
@@ -209,14 +213,15 @@
     # This method is used to poll a request until the progress is done.
     def _check_long_running(self, response):
         if not response.ok:
             response_content = response.content.decode('utf-8')
             # if more of these whitelisted errors show up: optimize approach
             if not 'The compiler is already defined' in response_content:
                 print(f"\n\nError: {response_content}\n\n")
+                self.print_messages()
                 raise Exception(f"Received unsuccessful response from EP.")
         if response.status_code == 202:
             jsonResponse = response.json()
             for key, value in jsonResponse.items():
                 if key == 'jobID':
                     while response.status_code == 202:
                         time.sleep(2)
@@ -288,16 +293,16 @@
             if message: print(message)
         url_combined = urlappendix
         if urlappendix[:9] == 'profiles/':
             # set/reset message marker
             self.message_marker_date = self.post('message-markers')['date']
             # ensure profile is available and path is url-safe
             index_qmark = urlappendix.find('?')
-            path = urlappendix[9:index_qmark] if index_qmark else urlappendix[9:]
-            suffix = urlappendix[index_qmark:] if index_qmark else ""
+            path = urlappendix[9:index_qmark] if index_qmark > 0 else urlappendix[9:]
+            suffix = urlappendix[index_qmark:] if index_qmark > 0 else ""
             path = unquote(path) # unquote incase caller already quoted the path
             if not os.path.isfile(path):
                 print(f"\nThe profile '{path}' cannot be found. Please ensure that the file is available.\n")
                 exit(1)
             path = quote(path, safe="")
             url_combined = 'profiles/' + path + suffix
         
@@ -316,45 +321,52 @@
                 continue
         return False
 
     # start commands depending on OS
 
     def _start_app_linux(self):
         # container use case -> start EP and Matlab
-        ep_ini_path = os.path.join(os.environ['EP_INSTALL_PATH'], 'ep.ini')
-        with open(ep_ini_path, 'r') as file:
-            content = file.read()
-        version = re.search(r'/ep/(\d+\.\d+[a-zA-Z]*\d+)/', content).group(1)
-
+        try:
+            ep_ini_path = os.path.join(os.environ['EP_INSTALL_PATH'], 'ep.ini')
+            with open(ep_ini_path, 'r') as file:
+                content = file.read()
+            version = re.search(r'/ep/(\d+\.\d+[a-zA-Z]*\d+)/', content).group(1)
+        except:
+            version = '24.1p0'
+        headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
+        matlab_ip = os.environ['MATLAB_IP'] if 'MATLAB_IP' in os.environ else '127.0.0.1'
         print(f'Waiting for BTC EmbeddedPlatform {version} to be available:')
 
-        headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
-        args = os.environ['EP_INSTALL_PATH'] + '/ep'
-        args += ' -clearPersistedState -application ' + headless_application_id
-        args += ' -nosplash -console -consoleLog'
-        args += ' -vmargs'
-        args += '   -Dep.linux.config=' + os.environ['EP_REGISTRY']
-        args += '   -Dlogback.configurationFile=' + os.environ['EP_LOG_CONFIG']
-        args += '   -Dep.configuration.logpath=' + os.environ['LOG_DIR']
-        args += '   -Dep.runtime.workdir=' + os.environ['WORK_DIR']
-        args += '   -Dbtc.root.temp.dir=' + os.environ['TMP_DIR']
-        args += '   -Dep.licensing.location=' + os.environ['LICENSE_LOCATION']
-        args += '   -Dep.licensing.package=' + os.environ['LICENSE_PACKAGE']
-        args += '   -Drest.port=' + os.environ['REST_PORT']
-        args += '   -Dep.runtime.batch=ep'
-        args += '   -Dep.runtime.api.port=1109'
-        args += '   -Dep.matlab.ip.range=127.0.0.1'
+        args = [ os.environ['EP_INSTALL_PATH'] + '/ep',
+            '-clearPersistedState', '-nosplash', '-console', '-consoleLog',
+            '-application', headless_application_id,            
+            '-vmargs',
+            '-Dep.linux.config=' + os.environ['EP_REGISTRY'],
+            '-Dlogback.configurationFile=' + os.environ['EP_LOG_CONFIG'],
+            '-Dep.configuration.logpath=' + os.environ['LOG_DIR'],
+            '-Dep.runtime.workdir=' + os.environ['WORK_DIR'],
+            '-Dbtc.root.temp.dir=' + os.environ['TMP_DIR'],
+            '-Dep.licensing.location=' + os.environ['LICENSE_LOCATION'],
+            '-Dep.licensing.package=' + os.environ['LICENSE_PACKAGES'],
+            '-Drest.port=' + os.environ['REST_PORT'],
+            '-Dosgi.configuration.area.default=/tmp/ep/configuration',
+            '-Dosgi.instance.area.default=/tmp/ep/workspace',
+            '-Dep.runtime.batch=ep',
+            '-Dep.runtime.api.port=1109',
+            '-Dep.matlab.ip.range=' + matlab_ip ]
         
         # start ep process
-        subprocess.Popen(args, stdout=open(os.devnull, 'wb'), stderr=open(os.devnull, 'wb'))
+        self.ep_process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        self.log_file_path = os.environ['LOG_DIR'] + '/current.log'
         self.actively_started = True
         
         # if container has matlab -> assume that this shall be started as well
         if shutil.which('matlab'): subprocess.Popen('matlab')
 
+
     def _start_app_windows(self, version, install_location, port, license_location, lic, config):
         headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
         # check if we have what we need
         if not (version and install_location): raise Exception("Cannot start BTC EmbeddedPlatform. Arguments version and install_location or install_root directory must be specified or configured in a config file (installationRoot)")
         # all good -> prepare start command for BTC EmbeddedPlatform
         appdata_location = os.environ['APPDATA'].replace('\\', '/') + f"/BTC/ep/{version}/"
         ml_port = 29300 + (port % 100)
@@ -381,15 +393,16 @@
             ' -Dosgi.configuration.area.default="' + appdata_location + self._PORT_ + '/configuration"' + \
             ' -Dosgi.instance.area.default="' + appdata_location + self._PORT_ + '/workspace"' + \
             ' -Dep.configuration.logpath=AppData/Roaming/BTC/ep/' + version + '/' + self._PORT_ + '/logs' + \
             ' -Dep.runtime.workdir=BTC/ep/' + version + '/' + self._PORT_ + \
             ' -Dep.licensing.package=' + lic + \
             ' -Dep.rest.port=' + self._PORT_
         if license_location or config and 'licenseLocation' in config:
-            args += f" -Dep.licensing.location={(license_location or config['licenseLocation'])}"
-        subprocess.Popen(args, stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
+                f" -Dep.licensing.location={(license_location or config['licenseLocation'])}"
+        self.ep_process = subprocess.Popen(args, stdout=open(os.devnull, 'wb'), stderr=subprocess.STDOUT)
+        self.log_file_path = appdata_location + self._PORT_ + '/logs/current.log'
         self.actively_started = True
 
 
 # if called directly, starts EP based on the global config
 if __name__ == '__main__':
     EPRestApi()
```

### Comparing `btc_embedded-23.3.9/btc_embedded/btc_config.yml` & `btc_embedded-24.1.0/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.0/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded/config.py` & `btc_embedded-24.1.0/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded/reporting.py` & `btc_embedded-24.1.0/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded/util.py` & `btc_embedded-24.1.0/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-23.3.9/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.0/btc_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 23.3.9
+Version: 24.1.0
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-23.3.9/setup.py` & `btc_embedded-24.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='23.3.9',
+    version='24.1.0',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

