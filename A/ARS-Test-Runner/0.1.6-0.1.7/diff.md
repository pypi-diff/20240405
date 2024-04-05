# Comparing `tmp/ARS_Test_Runner-0.1.6.tar.gz` & `tmp/ARS_Test_Runner-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARS_Test_Runner-0.1.6.tar", last modified: Mon Apr  1 18:04:23 2024, max compression
+gzip compressed data, was "ARS_Test_Runner-0.1.7.tar", last modified: Tue Apr  2 14:39:17 2024, max compression
```

## Comparing `ARS_Test_Runner-0.1.6.tar` & `ARS_Test_Runner-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 18:04:23.860829 ARS_Test_Runner-0.1.6/
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 18:04:23.855949 ARS_Test_Runner-0.1.6/ARS_Test_Runner/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/__init__.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/cli.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    23052 2024-04-01 17:52:41.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/semantic_test.py
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 18:04:23.859494 ARS_Test_Runner-0.1.6/ARS_Test_Runner/templates/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/templates/affects_creative.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/templates/treats.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner/templates/treats_creative.json
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 18:04:23.860205 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/SOURCES.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/dependency_links.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/entry_points.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/requires.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-01 18:04:23.000000 ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/top_level.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.6/LICENSE.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-01 18:04:23.860644 ARS_Test_Runner-0.1.6/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.6/README.md
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-01 18:04:23.861349 ARS_Test_Runner-0.1.6/setup.cfg
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-01 18:03:19.000000 ARS_Test_Runner-0.1.6/setup.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.380583 ARS_Test_Runner-0.1.7/
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.374280 ARS_Test_Runner-0.1.7/ARS_Test_Runner/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/__init__.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/cli.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22705 2024-04-02 14:39:05.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/semantic_test.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.379033 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/affects_creative.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/treats.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/treats_creative.json
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.379877 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-02 14:39:17.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/SOURCES.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/dependency_links.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/entry_points.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/requires.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/top_level.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.7/LICENSE.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-02 14:39:17.380354 ARS_Test_Runner-0.1.7/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.7/README.md
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-02 14:39:17.381156 ARS_Test_Runner-0.1.7/setup.cfg
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-02 14:39:05.000000 ARS_Test_Runner-0.1.7/setup.py
```

### Comparing `ARS_Test_Runner-0.1.6/ARS_Test_Runner/cli.py` & `ARS_Test_Runner-0.1.7/ARS_Test_Runner/cli.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.6/ARS_Test_Runner/semantic_test.py` & `ARS_Test_Runner-0.1.7/ARS_Test_Runner/semantic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,22 +123,22 @@
         report_card={}
         report_card['pk']={}
         report_card['results']=message
     else:
         children, parent_pk = await get_children(message, ARS_URL, output_curie)
         if children[0][0] == 'ars-default-agent' and 'error' in children[0][1].keys():
             report_card={}
-            report_card['pk']={}
+            report_card['pks']={}
             report_card['results']=[]
             for child in children:
                 if child[0] == 'ars-default-agent':
-                    report_card['pk']['parent_pk'] = child[2]
+                    report_card['pks']['parent_pk'] = child[2]
                     report_card['results'].append(child[1])
                 else:
-                    report_card['pk'][child[0]] = child[2]
+                    report_card['pks'][child[0].split('-')[1]] = child[2]
                     report_card['results'].append(child[1])
         else:
             report_card = await ARS_semantic_analysis(children, parent_pk, output_curie, expected_output)
 
     return report_card
 
 async def ARS_semantic_analysis(children: List[List], pk: str, output_curie: List[str], expected_output: str):
@@ -316,15 +316,15 @@
     start_time=time.time()
     parent_pk = response["pk"]
     #print(f'starting to check for parent pk: {parent_pk}')
     logging.debug("parent_pk for query {}  is {} ".format(query, str(parent_pk)))
     url = ARS_URL + "messages/" + parent_pk + "?trace=y"
     if timeout is None:
         timeout = 60
-    while (time.time()-start_time)/60<10:
+    while (time.time()-start_time)/60<15:
         #for 8 min, constantly check the parent status
         async with httpx.AsyncClient(verify=False) as client:
                 r = await client.get(url,timeout=timeout)
         try:
             data = r.json()
         except json.decoder.JSONDecodeError:
             logging.error("Non-JSON content received:")
@@ -472,23 +472,14 @@
     runner_setting = getattr(args, "runner_setting")
     expected_output = getattr(args, "expected_output")
     biolink_object_aspect_qualifier = getattr(args, "biolink_object_aspect_qualifier")
     biolink_object_direction_qualifier = getattr(args, "biolink_object_direction_qualifier")
     input_category = getattr(args,"input_category")
     input_curie = getattr(args, "input_curie")
     output_curie = getattr(args, "output_curie")
-    env = 'ci'
-    predicate = 'treats'
-    runner_setting = ['inferred']
-    expected_output = ['TopAnswer']
-    biolink_object_aspect_qualifier = '' #'activity_or_abundance'
-    biolink_object_direction_qualifier = '' #'increased'
-    input_category =  'biolink:Disease' #'Gene'
-    input_curie = 'MONDO:0009265'
-    output_curie = ['PUBCHEM.COMPOUND:23652731']
 
     current_time = datetime.datetime.now()
     formatted_start_time = current_time.strftime('%H:%M:%S')
     print(f"started performing ARS_Test pass/fail Analysis at {formatted_start_time}")
     print(asyncio.run(run_semantic_test(env,predicate, runner_setting, expected_output, biolink_object_aspect_qualifier, biolink_object_direction_qualifier, input_category, input_curie, output_curie)))
     endtime = datetime.datetime.now()
     formatted_end_time = endtime.strftime('%H:%M:%S')
```

### Comparing `ARS_Test_Runner-0.1.6/ARS_Test_Runner/templates/affects_creative.json` & `ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/affects_creative.json`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.6/ARS_Test_Runner.egg-info/PKG-INFO` & `ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS-Test-Runner
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.6/LICENSE.txt` & `ARS_Test_Runner-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.6/PKG-INFO` & `ARS_Test_Runner-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS_Test_Runner
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.6/README.md` & `ARS_Test_Runner-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.6/setup.py` & `ARS_Test_Runner-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from semantic_release import setup_hook
     setup_hook(sys.argv)
 except ImportError:
     pass
 
-__version__='0.1.6'
+__version__='0.1.7'
 setup(
     name="ARS_Test_Runner",
     version= __version__,
     description="Python package for ARS pass/fail test",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Shervin Abdollahi, Mark Williams",
```

