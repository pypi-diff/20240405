# Comparing `tmp/omdeventhandler-0.4.2.tar.gz` & `tmp/omdeventhandler-0.5.0.tar.gz`

## Comparing `omdeventhandler-0.4.2.tar` & `omdeventhandler-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rwxr-xr-x   0        0        0     6688 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/bin/eventhandler
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/baseclass.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/bash/runner.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/default/decider.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/nsc_web/runner.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/omd_site_self_heal/decider.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/src/eventhandler/ssh/runner.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/tests/test_classes.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/tests/test_package.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 omdeventhandler-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     6905 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/bin/eventhandler
+-rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/baseclass.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/bash/runner.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/default/decider.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/nsc_web/runner.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/omd_site_self_heal/decider.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/src/eventhandler/ssh/runner.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_classes.py
+-rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_notify.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/test_package.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/runner.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/notificationforwarder/eventhandler_report/formatter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/README.md
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 omdeventhandler-0.5.0/PKG-INFO
```

### Comparing `omdeventhandler-0.4.2/bin/eventhandler` & `omdeventhandler-0.5.0/bin/eventhandler`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                       help='Show logs at stdout',
                       default=False)
     parser.add_argument('--debug', action='store_true',
                       dest="debug",
                       help='Increase the log level to DEBUG',
                       default=False)
     parser.add_argument('--version', action='version',
-                      version=f'%(prog)%s 0.0')
+                      version=f'%(prog)%s 0.5.0')
 
     args = parser.parse_args()
     if not any(vars(args).values()):
         parser.print_help()
         parser.exit()
 
     if os.path.exists(os.environ["OMD_ROOT"]+"/var/log/eventhandler.debug"):
@@ -142,9 +142,13 @@
             logger_name = "notificationforwarder_"+args.forwarder+("_"+args.forwardertag if args.forwardertag else "")
             logger = logging.getLogger(logger_name)
             if args.debug:
                 traceback.print_exc(file=sys.stdout)
             logger.critical("there is no class for forwarder {} and formatter {}".format(args.forwarder, args.formatter))
             sys.exit(1)
     
-    runner.handle(args.eventopt)
-
+    success = runner.handle(args.eventopt)
+    if args.forwarder:
+        if success != None:
+            args.eventopt["eventhandler_success"] = success
+            runner.forwarder.forward(args.eventopt)
+    sys.exit(1 if success == False else 0)
```

### Comparing `omdeventhandler-0.4.2/src/eventhandler/baseclass.py` & `omdeventhandler-0.5.0/src/eventhandler/baseclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
             instance.decide_and_prepare(decided_event)
             return decided_event
         except Exception as e:
             logger.critical("when deciding based on this {} with this {} there was an error <{}>".format(str(raw_event), instance.__class__.__name__+"@"+instance.__module_file__, str(e)))
             return None
 
     def handle(self, raw_event):
+        success = False
         try:
             decided_event = self.decide_and_prepare_event(raw_event)
             if decided_event.is_discarded:
                 if not decided_event.is_discarded_silently:
                     if not decided_event.summary:
                         decided_event.summary = str(raw_event)
                     logger.info("discarded: {}".format(decided_event.summary))
@@ -150,17 +151,19 @@
                 decided_event = None
         except Exception as e:
             try:
                 decided_event
             except NameError:
                 logger.critical("raw event {} caused error {}".format(str(raw_event), str(e)))
             decided_event = None
+            success = None
         if decided_event:
             self.overwrite_attributes(decided_event.payload)
             success = self.run_decided(decided_event)
+        return success
 
     def overwrite_attributes(self, payload):
         # paload can overwrite runneropts
         for k in payload:
             if hasattr(self, k):
                 setattr(self, k, payload[k])
```

### Comparing `omdeventhandler-0.4.2/src/eventhandler/default/decider.py` & `omdeventhandler-0.5.0/src/eventhandler/default/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.4.2/src/eventhandler/nsc_web/runner.py` & `omdeventhandler-0.5.0/src/eventhandler/nsc_web/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.4.2/src/eventhandler/omd_site_self_heal/decider.py` & `omdeventhandler-0.5.0/src/eventhandler/omd_site_self_heal/decider.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.4.2/src/eventhandler/ssh/runner.py` & `omdeventhandler-0.5.0/src/eventhandler/ssh/runner.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.4.2/tests/test_classes.py` & `omdeventhandler-0.5.0/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `omdeventhandler-0.4.2/tests/pythonpath/local/lib/python/eventhandler/example/decider.py` & `omdeventhandler-0.5.0/tests/pythonpath/local/lib/python/eventhandler/example/decider.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 class ExampleDecider(EventhandlerDecider):
 
     def decide_and_prepare(self, event):
         if "discard" in event.eventopts:
             event.discard(silently=event.eventopts["discard"])
             event.summary = "halo i bims 1 alarm vong naemon her und i schmeis mi weg"
         else:
-            event.summary = event.eventopts.get("summary", None)
+            event.summary = "summary is "+event.eventopts.get("summary", None)
         event.payload = {
             "content": event.eventopts["content"],
         }
         if "delay" in event.eventopts:
             event.payload["delay"] = event.eventopts["delay"]
```

### Comparing `omdeventhandler-0.4.2/pyproject.toml` & `omdeventhandler-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 packages = ["src/eventhandler"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "./bin/eventhandler" = "eventhandler/bin_folder/eventhandler"
 
 [project]
 name = "omdeventhandler"
-version = "0.4.2"
+version = "0.5.0"
 authors = [
   { name="Gerhard Lausser", email="lausser@yahoo.com" },
 ]
 description = "A framework for event handlers for OMD"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `omdeventhandler-0.4.2/PKG-INFO` & `omdeventhandler-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omdeventhandler
-Version: 0.4.2
+Version: 0.5.0
 Summary: A framework for event handlers for OMD
 Project-URL: Homepage, https://github.com/lausser/noteventificationforhandlerwarder
 Project-URL: Bug Tracker, https://github.com/lausser/noteventificationforhandlerwarder/issues
 Author-email: Gerhard Lausser <lausser@yahoo.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

