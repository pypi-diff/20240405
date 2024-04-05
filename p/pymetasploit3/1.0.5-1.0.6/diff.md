# Comparing `tmp/pymetasploit3-1.0.5.tar.gz` & `tmp/pymetasploit3-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasploit3-1.0.5.tar", last modified: Thu Dec 28 19:21:33 2023, max compression
+gzip compressed data, was "pymetasploit3-1.0.6.tar", last modified: Fri Apr  5 20:27:39 2024, max compression
```

## Comparing `pymetasploit3-1.0.5.tar` & `pymetasploit3-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/pymetasploit3/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2309 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/msfconsole.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    72114 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/msfrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/pymetasploit3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1675 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/scripts/pymsfconsole.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1118 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/scripts/pymsfrpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1632 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/pymetasploit3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/pymetasploit3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2023-12-28 19:21:33.000000 pymetasploit3-1.0.5/pymetasploit3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-28 19:21:33.000000 pymetasploit3-1.0.5/pymetasploit3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 19:21:33.000000 pymetasploit3-1.0.5/pymetasploit3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 19:21:33.000000 pymetasploit3-1.0.5/pymetasploit3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-28 19:21:33.000000 pymetasploit3-1.0.5/pymetasploit3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 19:21:33.924310 pymetasploit3-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-28 19:21:32.000000 pymetasploit3-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:27:39.653360 pymetasploit3-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-04-05 20:27:39.653360 pymetasploit3-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:27:39.649360 pymetasploit3-1.0.6/pymetasploit3/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2309 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/msfconsole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73509 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/msfrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:27:39.653360 pymetasploit3-1.0.6/pymetasploit3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1675 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/scripts/pymsfconsole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1118 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/scripts/pymsfrpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3120 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/pymetasploit3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:27:39.653360 pymetasploit3-1.0.6/pymetasploit3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-04-05 20:27:39.000000 pymetasploit3-1.0.6/pymetasploit3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 20:27:39.000000 pymetasploit3-1.0.6/pymetasploit3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:27:39.000000 pymetasploit3-1.0.6/pymetasploit3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 20:27:39.000000 pymetasploit3-1.0.6/pymetasploit3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 20:27:39.000000 pymetasploit3-1.0.6/pymetasploit3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:27:39.653360 pymetasploit3-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-05 20:27:38.000000 pymetasploit3-1.0.6/setup.py
```

### Comparing `pymetasploit3-1.0.5/LICENSE` & `pymetasploit3-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasploit3-1.0.5/PKG-INFO` & `pymetasploit3-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasploit3
-Version: 1.0.5
+Version: 1.0.6
 Summary: A full-fledged msfrpc library for Metasploit framework.
 Home-page: https://github.com/DanMcInerney/pymetasploit3
 Author: Dan McInerney
 Author-email: danhmcinerney@gmail.com
 License: GPL
 Download-URL: https://github.com/DanMcInerney/pymetasploit3/zipball/master
 Platform: UNKNOWN
```

### Comparing `pymetasploit3-1.0.5/README.md` & `pymetasploit3-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pymetasploit3-1.0.5/pymetasploit3/msfconsole.py` & `pymetasploit3-1.0.6/pymetasploit3/msfconsole.py`

 * *Files identical despite different names*

### Comparing `pymetasploit3-1.0.5/pymetasploit3/msfrpc.py` & `pymetasploit3-1.0.6/pymetasploit3/msfrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,24 +125,27 @@
     ModuleEvasion = 'module.evasion'
     ModuleAuxiliary = 'module.auxiliary'
     ModulePayloads = 'module.payloads'
     ModuleEncoders = 'module.encoders'
     ModuleNops = 'module.nops'
     ModulePlatforms = 'module.platforms'
     ModulePost = 'module.post'
+    ModuleInfoHTML = 'module.info_html'
     ModuleInfo = 'module.info'
     ModuleCompatiblePayloads = 'module.compatible_payloads'
+    ModuleCompatibleEvasionPayloads = 'module.compatible_evasion_payloads'
     ModuleCompatibleSessions = 'module.compatible_sessions'
     ModuleTargetCompatiblePayloads = 'module.target_compatible_payloads'
+    ModuleTargetCompatibleEvasionPayloads = 'module.target_compatible_evasion_payloads'
     ModuleOptions = 'module.options'
     ModuleExecute = 'module.execute'
     ModuleEncodeFormats = 'module.encode_formats'
     ModuleEncode = 'module.encode'
     ModuleSearch = 'module.search'
-    ModuleCompatibleSessions = 'module.compatible_sessions'
+    ModuleRunningStats = 'module.running_stats'
     ModuleCheck = 'module.check'
     ModuleResults = 'module.results'
     PluginLoad = 'plugin.load'
     PluginUnload = 'plugin.unload'
     PluginLoaded = 'plugin.loaded'
     SessionList = 'session.list'
     SessionStop = 'session.stop'
@@ -190,15 +193,16 @@
 
     def __init__(self, password, **kwargs):
         self.uri = kwargs.get('uri', '/api/')
         self.port = kwargs.get('port', 55553)
         self.host = kwargs.get('server', '127.0.0.1')
         self.ssl = kwargs.get('ssl', False)
         self.token = kwargs.get('token')
-        self.encoding = kwargs.get('encoding', 'utf-8')
+        self.encodings = kwargs.get('encodings', ['utf-8'])
+        self.decode_error_handling: str = kwargs.get('decode_error_handling', 'strict')
         self.headers = {"Content-type": "binary/message-pack"}
         if self.token is None:
             self.login(kwargs.get('username', 'msf'), password)
 
     def call(self, method, opts=None, is_raw=False):
         if not isinstance(opts, list):
             opts = []
@@ -220,15 +224,15 @@
         r = self.post_request(url, payload)
 
         opts[:] = []  # Clear opts list
 
         if is_raw:
             return r.content
 
-        return convert(decode(r.content), self.encoding)  # convert all keys/vals to utf8
+        return convert(decode(r.content), self.encodings, self.decode_error_handling)  # convert all keys/vals to utf8
 
     @retry(tries=3, delay=1, backoff=2)
     def post_request(self, url, payload):
         return requests.post(url, data=payload, headers=self.headers, verify=False)
 
     def login(self, user, password):
         auth = self.call(MsfRpcMethod.AuthLogin, [user, password])
@@ -1514,14 +1518,22 @@
         """
         A list of compatible payloads.
         """
         #        return self.rpc.call(MsfRpcMethod.ModuleCompatiblePayloads, self.modulename)['payloads']
         return self.targetpayloads(self.target)
 
     @property
+    def evasion_payloads(self):
+        """
+        A list of compatible evasion payloads.
+        """
+        return self.rpc.call(MsfRpcMethod.ModuleCompatibleEvasionPayloads, self.modulename)
+        
+
+    @property
     def target(self):
         return self._target
 
     @target.setter
     def target(self, target):
         if target not in self.targets:
             raise ValueError('Target must be one of %s' % repr(list(self.targets.keys())))
@@ -1532,14 +1544,23 @@
         Returns a list of compatible payloads for a given target ID.
 
         Optional Keyword Arguments:
         - t : the target ID (default: 0, e.g. 'Automatic')
         """
         return self.rpc.call(MsfRpcMethod.ModuleTargetCompatiblePayloads, [self.modulename, t])['payloads']
 
+    def targetevasionpayloads(self, t=0):
+        """
+        Returns a list of compatible evasion payloads for a given target ID.
+
+        Optional Keyword Arguments:
+        - t : the target ID (default: 0, e.g. 'Automatic')
+        """
+        return self.rpc.call(MsfRpcMethod.ModuleTargetCompatibleEvasionPayloads, [self.modulename, t])['payloads']
+
 
 class PostModule(MsfModule):
 
     def __init__(self, rpc, post):
         """
         Initializes the use of a post exploitation module.
 
@@ -1674,14 +1695,32 @@
         - mtype : Module type
         - mname : Module name
 
         Optional Keyword Arguments:
         - **kwargs : the module's run options
         """
         return self.rpc.call(MsfRpcMethod.ModuleCheck, [mtype, mname, kwargs])
+    
+    def running_stats(self):
+        """
+        Returns the currently running module stats in each state.
+        """
+        
+        return self.rpc.call(MsfRpcMethod.ModuleRunningStats, [])
+    
+    def info_html(self, mtype, mname):
+        """
+        Returns detailed information about a module in HTML.
+        
+        Mandatory Arguments:
+        - mtype : Module type
+        - mname : Module name
+        """
+        
+        return self.rpc.call(MsfRpcMethod.ModuleInfoHTML, [mtype, mname])
 
     def results(self, uuid):
         return self.rpc.call(MsfRpcMethod.ModuleResults, [uuid])
 
 
     @property
     def exploits(self):
```

### Comparing `pymetasploit3-1.0.5/pymetasploit3/scripts/pymsfconsole.py` & `pymetasploit3-1.0.6/pymetasploit3/scripts/pymsfconsole.py`

 * *Files identical despite different names*

### Comparing `pymetasploit3-1.0.5/pymetasploit3/scripts/pymsfrpc.py` & `pymetasploit3-1.0.6/pymetasploit3/scripts/pymsfrpc.py`

 * *Files identical despite different names*

### Comparing `pymetasploit3-1.0.5/pymetasploit3.egg-info/PKG-INFO` & `pymetasploit3-1.0.6/pymetasploit3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasploit3
-Version: 1.0.5
+Version: 1.0.6
 Summary: A full-fledged msfrpc library for Metasploit framework.
 Home-page: https://github.com/DanMcInerney/pymetasploit3
 Author: Dan McInerney
 Author-email: danhmcinerney@gmail.com
 License: GPL
 Download-URL: https://github.com/DanMcInerney/pymetasploit3/zipball/master
 Platform: UNKNOWN
```

### Comparing `pymetasploit3-1.0.5/setup.py` & `pymetasploit3-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     return open(path.join(path.dirname(__file__), fname)).read()
 
 
 setup(
     name='pymetasploit3',
     author='Dan McInerney',
-    version='1.0.5',
+    version='1.0.6',
     author_email='danhmcinerney@gmail.com',
     description='A full-fledged msfrpc library for Metasploit framework.',
     license='GPL',
     packages=find_packages(exclude='tests'),
     scripts=[
         'pymetasploit3/scripts/pymsfconsole.py',
         'pymetasploit3/scripts/pymsfrpc.py'
```

