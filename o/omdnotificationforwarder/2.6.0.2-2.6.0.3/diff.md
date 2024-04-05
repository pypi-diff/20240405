# Comparing `tmp/omdnotificationforwarder-2.6.0.2.tar.gz` & `tmp/omdnotificationforwarder-2.6.0.3.tar.gz`

## Comparing `omdnotificationforwarder-2.6.0.2.tar` & `omdnotificationforwarder-2.6.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rwxr-xr-x   0        0        0     3610 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/bin/notificationforwarder
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/baseclass.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/email/formatter.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/email/forwarder.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/example/formatter.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/example/forwarder.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/rabbitmq/formatter.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/rabbitmq/forwarder.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/syslog/formatter.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/syslog/forwarder.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/telegram/forwarder.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/src/notificationforwarder/webhook/forwarder.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_alertmanager.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_classes.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_discard.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_formatter.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_package.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_paths.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/test_webhook.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/lib/python/notificationforwarder/split1/forwarder.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/lib/python/notificationforwarder/split2/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/lib/python/notificationforwarder/split2/forwarder.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/lib/python/notificationforwarder/split3/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/lib/python/notificationforwarder/split3/forwarder.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/bayern/formatter.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split1/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split2/forwarder.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split3/formatter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split3/forwarder.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split4/formatter.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/split4/forwarder.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/.gitignore
--rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/README.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/pyproject.toml
--rw-r--r--   0        0        0    14517 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     3617 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/bin/notificationforwarder
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/baseclass.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/formatter.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/forwarder.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/formatter.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/forwarder.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/formatter.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/forwarder.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/formatter.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/forwarder.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/telegram/forwarder.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/src/notificationforwarder/webhook/forwarder.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_alertmanager.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_classes.py
+-rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_discard.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_formatter.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_package.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_paths.py
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/test_webhook.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split1/forwarder.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split2/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split2/forwarder.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split3/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/lib/python/notificationforwarder/split3/forwarder.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/bayern/formatter.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split1/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split2/forwarder.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split3/formatter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split3/forwarder.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split4/formatter.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/split4/forwarder.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/.gitignore
+-rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/README.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/pyproject.toml
+-rw-r--r--   0        0        0    14517 2020-02-02 00:00:00.000000 omdnotificationforwarder-2.6.0.3/PKG-INFO
```

### Comparing `omdnotificationforwarder-2.6.0.2/bin/notificationforwarder` & `omdnotificationforwarder-2.6.0.3/bin/notificationforwarder`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                       help='Show logs at stdout',
                       default=False)
     parser.add_argument('--debug', action='store_true',
                       dest="debug",
                       help='Increase the log level to DEBUG',
                       default=False)
     parser.add_argument('--version', action='version',
-                      version=f'%(prog)s ')
+                      version=f'%(prog)s 2.6.0.3')
 
     args = parser.parse_args()
     if not hasattr(args, 'formatter'):
         args.formatter = args.forwarder
 
     try:
         forwarder = baseclass.new(args.forwarder, args.forwardertag, args.formatter, args.verbose, args.debug, args.forwarderopt)
```

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/baseclass.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/baseclass.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/email/formatter.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/email/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/email/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/example/formatter.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/example/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/example/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/rabbitmq/formatter.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/rabbitmq/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/rabbitmq/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/syslog/formatter.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/syslog/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/syslog/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/telegram/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/telegram/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/src/notificationforwarder/webhook/forwarder.py` & `omdnotificationforwarder-2.6.0.3/src/notificationforwarder/webhook/forwarder.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_alertmanager.py` & `omdnotificationforwarder-2.6.0.3/tests/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_classes.py` & `omdnotificationforwarder-2.6.0.3/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_discard.py` & `omdnotificationforwarder-2.6.0.3/tests/test_discard.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_formatter.py` & `omdnotificationforwarder-2.6.0.3/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_paths.py` & `omdnotificationforwarder-2.6.0.3/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/test_webhook.py` & `omdnotificationforwarder-2.6.0.3/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py` & `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/alertmanager_servicenow/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py` & `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/discard/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py` & `omdnotificationforwarder-2.6.0.3/tests/pythonpath/local/lib/python/notificationforwarder/vong/formatter.py`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/README.md` & `omdnotificationforwarder-2.6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `omdnotificationforwarder-2.6.0.2/pyproject.toml` & `omdnotificationforwarder-2.6.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 packages = ["src/notificationforwarder"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "./bin/notificationforwarder" = "notificationforwarder/bin_folder/notificationforwarder"
 
 [project]
 name = "omdnotificationforwarder"
-version = "2.6.0.2"
+version = "2.6.0.3"
 authors = [
   { name="Gerhard Lausser", email="lausser@yahoo.com" },
 ]
 description = "A framework for notification scripts for OMD"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `omdnotificationforwarder-2.6.0.2/PKG-INFO` & `omdnotificationforwarder-2.6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omdnotificationforwarder
-Version: 2.6.0.2
+Version: 2.6.0.3
 Summary: A framework for notification scripts for OMD
 Project-URL: Homepage, https://github.com/lausser/noteventificationforhandlerwarder
 Project-URL: Bug Tracker, https://github.com/lausser/noteventificationforhandlerwarder/issues
 Author-email: Gerhard Lausser <lausser@yahoo.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

