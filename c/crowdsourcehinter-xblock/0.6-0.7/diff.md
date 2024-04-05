# Comparing `tmp/crowdsourcehinter-xblock-0.6.tar.gz` & `tmp/crowdsourcehinter-xblock-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crowdsourcehinter-xblock-0.6.tar", last modified: Fri Jun  5 10:49:43 2020, max compression
+gzip compressed data, was "crowdsourcehinter-xblock-0.7.tar", last modified: Fri Apr  5 14:31:10 2024, max compression
```

## Comparing `crowdsourcehinter-xblock-0.6.tar` & `crowdsourcehinter-xblock-0.7.tar`

### file list

```diff
@@ -1,19 +1,36 @@
-drwxr-xr-x   0 jenkins   (1008) jenkins   (1010)        0 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/
-drwxr-xr-x   0 jenkins   (1008) jenkins   (1010)        0 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter/
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)    20198 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter/crowdsourcehinter.py
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       49 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter/__init__.py
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)    59256 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_correct.png
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)    44231 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_hint.png
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)   154511 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_setup.png
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       38 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/setup.cfg
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)     3091 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/PKG-INFO
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)     2492 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/setup.py
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       92 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/MANIFEST.in
-drwxr-xr-x   0 jenkins   (1008) jenkins   (1010)        0 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       18 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       25 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)       69 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)     3091 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)        1 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)      474 2020-06-05 10:49:43.000000 crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1008) jenkins   (1010)     2151 2020-06-05 10:49:42.000000 crowdsourcehinter-xblock-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.767079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/crowdsourcehinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.767079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/public/3rdParty/
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/public/3rdParty/mustache.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/css/crowdsourcehinter.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/html/crowdsourcehinter.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/html/crowdsourcehinterstudio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.767079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/js/src/crowdsourcehinter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter/static/js/src/crowdsourcehinter_studio.js
+-rw-r--r--   0 runner    (1001) docker     (127)    59256 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_correct.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44231 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_hint.png
+-rw-r--r--   0 runner    (1001) docker     (127)   154511 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_setup.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 14:31:10.000000 crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:31:10.771079 crowdsourcehinter-xblock-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-05 14:31:07.000000 crowdsourcehinter-xblock-0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crowdsourcehinter-xblock-0.6/crowdsourcehinter/crowdsourcehinter.py` & `crowdsourcehinter-xblock-0.7/crowdsourcehinter/crowdsourcehinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from __future__ import absolute_import
+import copy
+import json
 import logging
-import operator
-import pkg_resources
 import random
-import json
-import copy
 
-import six.moves.urllib.request, six.moves.urllib.parse, six.moves.urllib.error
-import six.moves.html_parser
+import pkg_resources
 
-from xblock.core import XBlock
-from xblock.fields import Scope, Dict, List, Boolean, String
+import six.moves.html_parser
+import six.moves.urllib.error
+import six.moves.urllib.parse
+import six.moves.urllib.request
 from web_fragments.fragment import Fragment
+from xblock.core import XBlock
+from xblock.fields import Dict, List, Scope, String
 
 log = logging.getLogger(__name__)
 html_parser = six.moves.html_parser.HTMLParser()
 
+
 class CrowdsourceHinter(XBlock):
     """
     This is the Crowdsource Hinter XBlock. This Xblock provides
     students with hints that specifically address their
     mistake. The hints are crowdsourced from the students.
     """
```

### Comparing `crowdsourcehinter-xblock-0.6/crowdsourcehinter_correct.png` & `crowdsourcehinter-xblock-0.7/crowdsourcehinter_correct.png`

 * *Files identical despite different names*

### Comparing `crowdsourcehinter-xblock-0.6/crowdsourcehinter_hint.png` & `crowdsourcehinter-xblock-0.7/crowdsourcehinter_hint.png`

 * *Files identical despite different names*

### Comparing `crowdsourcehinter-xblock-0.6/crowdsourcehinter_setup.png` & `crowdsourcehinter-xblock-0.7/crowdsourcehinter_setup.png`

 * *Files identical despite different names*

### Comparing `crowdsourcehinter-xblock-0.6/PKG-INFO` & `crowdsourcehinter-xblock-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: crowdsourcehinter-xblock
-Version: 0.6
+Version: 0.7
 Summary: crowdsourcehinter XBlock
-Home-page: https://github.com/edx/crowdsourcehinter
+Home-page: https://github.com/openedx/crowdsourcehinter
 Author: edX
-License: UNKNOWN
-Description: This is the repository for the Crowdsource Hinter XBlock. The Crowdsource Hinter serves to provide students with hints when they incorrectly answer a problem within a course. The hinter is compatible with numerical input and text input type problems.
-        
-        This XBlock is still a prototype. 
-        
-        An example of a student recieving a hint 
-        ![CrowdSourceHinter Hint Screenshot](crowdsourcehinter_hint.png)
-        
-        
-        An example of after a student corrects their answer
-        ![CrowdSourceHinter Screenshot](crowdsourcehinter_correct.png)
-        
-        To bring the crowd sourced hinter into a demo course:
-        
-        Follow https://github.com/edx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
-        
-        In studio view, edit the hinter so that the "Problem Element" is set to the "data-usage-id" of the problem block (findable by inspecting element of the problem block). If no problem element is set manually, the hinter will default to respond to the first problem block on the page.
-        
-        ![CrowdSourceHinter Installation Screenshot](crowdsourcehinter_setup.png)
-        
-        The two key features of the crowdsource hinter are the abilities to show students hints and to have the students themselves create hints to be shown to future students. 
-        
-        When a student incorrectly answers a problem, the hinter will look through its database to search for a hint that has been stored for that exact incorrect answer input (i.e. when the database is large enough, two different incorrect answers would not receive the same hint). If hints exist for a student's incorrect answer, this hint is shown to the student. The student then may have the opportunity to input their answer again, which may prompt another hint to be displayed.
-        
-        After a student re-submits an answer correctly, they can rate hints for their usefulness or contribute a new hint to be used by other students. Rating hints works by upvoting, downvoting, or reporting hints. The new hint that is contributed by a student is specific to the incorrect answer that they make (currently the first incorrect answer will be prompted for contributing new hints).
-        
 Keywords: crowdsourcehinter xblock
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: XBlock
+Requires-Dist: six
+Requires-Dist: web-fragments
+
+This is the repository for the Crowdsource Hinter XBlock. The Crowdsource Hinter serves to provide students with hints when they incorrectly answer a problem within a course. The hinter is compatible with numerical input and text input type problems.
+
+This XBlock is still a prototype. 
+
+An example of a student recieving a hint 
+![CrowdSourceHinter Hint Screenshot](crowdsourcehinter_hint.png)
+
+
+An example of after a student corrects their answer
+![CrowdSourceHinter Screenshot](crowdsourcehinter_correct.png)
+
+To bring the crowd sourced hinter into a demo course:
+
+Follow https://github.com/openedx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
+
+In studio view, edit the hinter so that the "Problem Element" is set to the "data-usage-id" of the problem block (findable by inspecting element of the problem block). If no problem element is set manually, the hinter will default to respond to the first problem block on the page.
+
+![CrowdSourceHinter Installation Screenshot](crowdsourcehinter_setup.png)
+
+The two key features of the crowdsource hinter are the abilities to show students hints and to have the students themselves create hints to be shown to future students. 
+
+When a student incorrectly answers a problem, the hinter will look through its database to search for a hint that has been stored for that exact incorrect answer input (i.e. when the database is large enough, two different incorrect answers would not receive the same hint). If hints exist for a student's incorrect answer, this hint is shown to the student. The student then may have the opportunity to input their answer again, which may prompt another hint to be displayed.
+
+After a student re-submits an answer correctly, they can rate hints for their usefulness or contribute a new hint to be used by other students. Rating hints works by upvoting, downvoting, or reporting hints. The new hint that is contributed by a student is specific to the incorrect answer that they make (currently the first incorrect answer will be prompted for contributing new hints).
```

### Comparing `crowdsourcehinter-xblock-0.6/crowdsourcehinter_xblock.egg-info/PKG-INFO` & `crowdsourcehinter-xblock-0.7/crowdsourcehinter_xblock.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: crowdsourcehinter-xblock
-Version: 0.6
+Version: 0.7
 Summary: crowdsourcehinter XBlock
-Home-page: https://github.com/edx/crowdsourcehinter
+Home-page: https://github.com/openedx/crowdsourcehinter
 Author: edX
-License: UNKNOWN
-Description: This is the repository for the Crowdsource Hinter XBlock. The Crowdsource Hinter serves to provide students with hints when they incorrectly answer a problem within a course. The hinter is compatible with numerical input and text input type problems.
-        
-        This XBlock is still a prototype. 
-        
-        An example of a student recieving a hint 
-        ![CrowdSourceHinter Hint Screenshot](crowdsourcehinter_hint.png)
-        
-        
-        An example of after a student corrects their answer
-        ![CrowdSourceHinter Screenshot](crowdsourcehinter_correct.png)
-        
-        To bring the crowd sourced hinter into a demo course:
-        
-        Follow https://github.com/edx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
-        
-        In studio view, edit the hinter so that the "Problem Element" is set to the "data-usage-id" of the problem block (findable by inspecting element of the problem block). If no problem element is set manually, the hinter will default to respond to the first problem block on the page.
-        
-        ![CrowdSourceHinter Installation Screenshot](crowdsourcehinter_setup.png)
-        
-        The two key features of the crowdsource hinter are the abilities to show students hints and to have the students themselves create hints to be shown to future students. 
-        
-        When a student incorrectly answers a problem, the hinter will look through its database to search for a hint that has been stored for that exact incorrect answer input (i.e. when the database is large enough, two different incorrect answers would not receive the same hint). If hints exist for a student's incorrect answer, this hint is shown to the student. The student then may have the opportunity to input their answer again, which may prompt another hint to be displayed.
-        
-        After a student re-submits an answer correctly, they can rate hints for their usefulness or contribute a new hint to be used by other students. Rating hints works by upvoting, downvoting, or reporting hints. The new hint that is contributed by a student is specific to the incorrect answer that they make (currently the first incorrect answer will be prompted for contributing new hints).
-        
 Keywords: crowdsourcehinter xblock
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: XBlock
+Requires-Dist: six
+Requires-Dist: web-fragments
+
+This is the repository for the Crowdsource Hinter XBlock. The Crowdsource Hinter serves to provide students with hints when they incorrectly answer a problem within a course. The hinter is compatible with numerical input and text input type problems.
+
+This XBlock is still a prototype. 
+
+An example of a student recieving a hint 
+![CrowdSourceHinter Hint Screenshot](crowdsourcehinter_hint.png)
+
+
+An example of after a student corrects their answer
+![CrowdSourceHinter Screenshot](crowdsourcehinter_correct.png)
+
+To bring the crowd sourced hinter into a demo course:
+
+Follow https://github.com/openedx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
+
+In studio view, edit the hinter so that the "Problem Element" is set to the "data-usage-id" of the problem block (findable by inspecting element of the problem block). If no problem element is set manually, the hinter will default to respond to the first problem block on the page.
+
+![CrowdSourceHinter Installation Screenshot](crowdsourcehinter_setup.png)
+
+The two key features of the crowdsource hinter are the abilities to show students hints and to have the students themselves create hints to be shown to future students. 
+
+When a student incorrectly answers a problem, the hinter will look through its database to search for a hint that has been stored for that exact incorrect answer input (i.e. when the database is large enough, two different incorrect answers would not receive the same hint). If hints exist for a student's incorrect answer, this hint is shown to the student. The student then may have the opportunity to input their answer again, which may prompt another hint to be displayed.
+
+After a student re-submits an answer correctly, they can rate hints for their usefulness or contribute a new hint to be used by other students. Rating hints works by upvoting, downvoting, or reporting hints. The new hint that is contributed by a student is specific to the incorrect answer that they make (currently the first incorrect answer will be prompted for contributing new hints).
```

### Comparing `crowdsourcehinter-xblock-0.6/README.md` & `crowdsourcehinter-xblock-0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 An example of after a student corrects their answer
 ![CrowdSourceHinter Screenshot](crowdsourcehinter_correct.png)
 
 To bring the crowd sourced hinter into a demo course:
 
-Follow https://github.com/edx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
+Follow https://github.com/openedx/edx-platform/wiki/Installing-a-new-XBlock for basic xblock installation. The name of the module to set in the advanced settings tab is "crowdsourcehinter".
 
 In studio view, edit the hinter so that the "Problem Element" is set to the "data-usage-id" of the problem block (findable by inspecting element of the problem block). If no problem element is set manually, the hinter will default to respond to the first problem block on the page.
 
 ![CrowdSourceHinter Installation Screenshot](crowdsourcehinter_setup.png)
 
 The two key features of the crowdsource hinter are the abilities to show students hints and to have the students themselves create hints to be shown to future students.
```

