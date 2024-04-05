# Comparing `tmp/lanisapi-0.4.0a0.tar.gz` & `tmp/lanisapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanisapi-0.4.0a0.tar", last modified: Mon Nov 20 22:30:02 2023, max compression
+gzip compressed data, was "lanisapi-0.4.1.tar", last modified: Sun Nov 26 00:46:09 2023, max compression
```

## Comparing `lanisapi-0.4.0a0.tar` & `lanisapi-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.979629 lanisapi-0.4.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.979629 lanisapi-0.4.0a0/src/lanisapi/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/src/lanisapi/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/authentication_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/conversations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/schools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/functions/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/src/lanisapi/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/cryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/html_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-11-20 22:29:53.000000 lanisapi-0.4.0a0/src/lanisapi/helpers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 22:30:02.983629 lanisapi-0.4.0a0/src/lanisapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-11-20 22:30:02.000000 lanisapi-0.4.0a0/src/lanisapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-20 22:30:02.000000 lanisapi-0.4.0a0/src/lanisapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 22:30:02.000000 lanisapi-0.4.0a0/src/lanisapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-20 22:30:02.000000 lanisapi-0.4.0a0/src/lanisapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-20 22:30:02.000000 lanisapi-0.4.0a0/src/lanisapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-26 00:45:57.000000 lanisapi-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-11-26 00:46:09.130667 lanisapi-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2023-11-26 00:45:57.000000 lanisapi-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-11-26 00:45:57.000000 lanisapi-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 00:46:09.130667 lanisapi-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.126667 lanisapi-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.126667 lanisapi-0.4.1/src/lanisapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/authentication_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/conversations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/schools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/functions/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/cryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/html_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-11-26 00:45:57.000000 lanisapi-0.4.1/src/lanisapi/helpers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:46:09.130667 lanisapi-0.4.1/src/lanisapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-26 00:46:09.000000 lanisapi-0.4.1/src/lanisapi.egg-info/top_level.txt
```

### Comparing `lanisapi-0.4.0a0/LICENSE` & `lanisapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/PKG-INFO` & `lanisapi-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanisapi
-Version: 0.4.0a0
+Version: 0.4.1
 Summary: A unofficial python api for Lanis.
 Author: kurwjan
 Project-URL: Homepage, https://github.com/kurwjan/LanisAPI
 Project-URL: Bug Tracker, https://github.com/kurwjan/LanisAPI/issues
 Project-URL: Documentation, https://lanisapi.readthedocs.io/
 Keywords: Lanis,SPH,Schulportal Hessen,Hessen,API
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: German
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: selectolax
 Requires-Dist: pycryptodomex
+Requires-Dist: py-machineid
 
 [[README DE](https://github.com/kurwjan/LanisAPI/blob/master/README-DE.md)]  [[README EN](https://github.com/kurwjan/LanisAPI/blob/master/README.md)]
 
 # LanisAPI
 
 > ## ⚠ Notice
 > **Because the Schulportal Hessen changes quickly and is very fragmented, some functions at specific schools or after a while may no longer work.**
@@ -36,14 +37,19 @@
 + Fetch calendar events.
 + Fetch conversations.
 + Fetch all schools that have Lanis.
 + Fetch all web applets with their links.
 
 **Overview of future Features, Problems and other things [here](https://github.com/users/kurwjan/projects/2).**
 
+## App for the Schulportal Hessen
+If you want to have an app for Lanis, check out [SPH-vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) by [@alessioC42](https://github.com/alessioC42). _It's still in an early phase!_
+
+**It would be also really nice if you contribute to this project**, like bug reporting, if you know Dart and Flutter it would be nice to see your help or you could learn Dart, it's not hard.
+
 ## How do I install it?
 
 ```sh
 pip install lanisapi
 ```
 
 Required is Python 3.11. *(older versions are probably not working, I didn't tested it.)*
@@ -81,15 +87,15 @@
 
 The Javascript project [SPHclient](https://github.com/alessioC42/SPHclient) from [@alessioC42](https://github.com/alessioC42) helped me to understand the *Schulportal Hessen*.
 
 The Android-App [sph-planner](https://github.com/koenidv/sph-planner) from [@koenidv](https://github.com/koenidv) helped me to understand the Level 2 encryption.
 
 Other projects that didn't helped me but are cool:
 
-+ **Good TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)**
-+ Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)
++ **Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)**
++ TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)
 + Javascript app [SchulportalApp](https://github.com/DerOwnerHD/SchulportalApp) from [DerOwnerHD](https://github.com/DerOwnerHD)
 + Flutter Android app [lkwslr-sphplaner](https://github.com/flutter-preview/lkwslr-sphplaner) from [flutter-preview](https://github.com/flutter-preview)
 
 ## Notice
 
 This project isn't officially related to the Schulportal Hessen. It's only a unofficial library, supported by the community.
```

### Comparing `lanisapi-0.4.0a0/README.md` & `lanisapi-0.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 + Fetch calendar events.
 + Fetch conversations.
 + Fetch all schools that have Lanis.
 + Fetch all web applets with their links.
 
 **Overview of future Features, Problems and other things [here](https://github.com/users/kurwjan/projects/2).**
 
+## App for the Schulportal Hessen
+If you want to have an app for Lanis, check out [SPH-vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) by [@alessioC42](https://github.com/alessioC42). _It's still in an early phase!_
+
+**It would be also really nice if you contribute to this project**, like bug reporting, if you know Dart and Flutter it would be nice to see your help or you could learn Dart, it's not hard.
+
 ## How do I install it?
 
 ```sh
 pip install lanisapi
 ```
 
 Required is Python 3.11. *(older versions are probably not working, I didn't tested it.)*
@@ -61,15 +66,15 @@
 
 The Javascript project [SPHclient](https://github.com/alessioC42/SPHclient) from [@alessioC42](https://github.com/alessioC42) helped me to understand the *Schulportal Hessen*.
 
 The Android-App [sph-planner](https://github.com/koenidv/sph-planner) from [@koenidv](https://github.com/koenidv) helped me to understand the Level 2 encryption.
 
 Other projects that didn't helped me but are cool:
 
-+ **Good TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)**
-+ Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)
++ **Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)**
++ TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)
 + Javascript app [SchulportalApp](https://github.com/DerOwnerHD/SchulportalApp) from [DerOwnerHD](https://github.com/DerOwnerHD)
 + Flutter Android app [lkwslr-sphplaner](https://github.com/flutter-preview/lkwslr-sphplaner) from [flutter-preview](https://github.com/flutter-preview)
 
 ## Notice
 
 This project isn't officially related to the Schulportal Hessen. It's only a unofficial library, supported by the community.
```

### Comparing `lanisapi-0.4.0a0/pyproject.toml` & `lanisapi-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lanisapi"
-version = "0.4.0a"
+version = "0.4.1"
 authors = [
     { name = "kurwjan" }
 ]
 description = "A unofficial python api for Lanis."
 keywords = [
     "Lanis",
     "SPH",
@@ -24,14 +24,15 @@
     "Operating System :: OS Independent",
     "Natural Language :: German"
 ]
 dependencies = [
     "httpx",
     "selectolax",
     "pycryptodomex",
+    "py-machineid"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kurwjan/LanisAPI"
 "Bug Tracker" = "https://github.com/kurwjan/LanisAPI/issues"
 "Documentation" = "https://lanisapi.readthedocs.io/"
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/__init__.py` & `lanisapi-0.4.1/src/lanisapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A lib to interact with the Schulportal Hessen. Use LanisClient to interact."""
 
 from .client import LanisClient
 from .functions.apps import App, Folder
-from .functions.authentication_types import LanisAccount, LanisCookie, School
+from .functions.authentication_types import LanisAccount, LanisCookie, School, SessionType
 from .functions.calendar import Calendar
 from .functions.conversations import Conversation
 from .functions.substitution import SubstitutionPlan
 from .functions.tasks import Task
 
 __all__ = [
     "LanisClient",
@@ -15,8 +15,9 @@
     "Calendar",
     "Conversation",
     "App",
     "Folder",
     "LanisAccount",
     "LanisCookie",
     "School",
+    "SessionType"
 ]
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/client.py` & `lanisapi-0.4.1/src/lanisapi/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 """This script includes the LanisClient to interact with Lanis."""
 
 import json
 import os
-from base64 import b64decode, b64encode
 from datetime import datetime, timedelta
+from enum import Enum
 from pathlib import Path
 from time import time
 
 import httpx
-from Cryptodome.Cipher import AES
-from Cryptodome.Protocol.KDF import scrypt
-from Cryptodome.Random import get_random_bytes
 
-from .constants import LOGGER, URL
+from .constants import JSON, LOGGER, URL
 from .exceptions import (
+    ForceNewAuthenticationError,
     NoSchoolFoundError,
     WrongCredentialsError,
 )
 from .functions.apps import (
     App,
     Folder,
     _get_app_availability,
     _get_apps,
     _get_available_apps,
     _get_folders,
 )
-from .functions.authentication_types import LanisAccount, LanisCookie
+from .functions.authentication_types import LanisAccount, LanisCookie, SessionType
 from .functions.calendar import Calendar, _get_calendar, _get_calendar_month
 from .functions.conversations import Conversation, _get_conversations
 from .functions.schools import _get_schools
 from .functions.substitution import SubstitutionPlan, _get_substitutions
 from .functions.tasks import Task, _get_tasks
 from .helpers.authentication import (
     get_authentication_sid,
     get_authentication_url,
     get_session,
+    get_session_and_autologin,
+    get_session_by_autologin,
 )
 from .helpers.cryptor import Cryptor
 from .helpers.html_logger import HTMLLogger
 from .helpers.request import Request
 from .helpers.wrappers import check_availability, handle_exceptions, requires_auth
 
 
 class LanisClient:
     """The interface between python and Schulportal Hessen.
 
     Use ``authenticate()`` to use this interface.
 
     Parameters
     ----------
-    authentication : LanisAccount | LanisCookie
+    authentication : LanisAccount or LanisCookie or None
         1. A Lanis account with its username and password, and a school id or school name and city in ``School``.
         2. Cookies with authentication data (school id and session id) in ``LanisCookie`` for instantly interacting with Lanis. You can obtain this during a session with ``authentication_cookies``.
-    save : bool, default True
-        If False the school list, html data logs and future things won't be saved to a file.
+        3. If None it will use the session.json, like for the 30-days session or last session (100min), when no session.json exists, it will return ``ForceNewAuthenticationError``.
     ad_header : httpx.Headers, default {"user-agent": ....}
         Send custom headers to Lanis. Primarily used to send a
         custom ``user-agent``.
     """
 
+    class AuthenticationMethod(Enum):
+        """Used to indicate with which method that this lib provides was used."""
+
+        LanisCookie = 1
+        LanisAccount = 2
+        SessionsFile = 3
+
     def __init__(  # noqa: D107
         self,
-        authentication: LanisAccount | LanisCookie,
-        save: bool = True,
+        authentication: LanisAccount | LanisCookie | None,
         ad_header: httpx.Headers = None,
     ) -> None:
         self.authentication = authentication
-
-        self.save = save
-
         self.ad_header = (
             ad_header
             if ad_header is not None
             else httpx.Headers(
                 {
-                    "user-agent": "LanisClient by kurwjan and contributors (https://github.com/kurwjan/LanisAPI/)"
+                    "user-agent": "LanisAPI by kurwjan and contributors (https://github.com/kurwjan/LanisAPI/)"
                 }
             )
         )
-
         self.authenticated = False
-
-        self.authentication_method = None
+        self.authentication_method: self.AuthenticationMethod = None
+        self.session_type: SessionType = None
+        self.autologin: list[str] | None = None
+        self.cryptor = Cryptor()
 
         Request.set_headers(self.ad_header)
 
-        self.cryptor = Cryptor()
-
-        LOGGER.info("USING VERSION 0.4.0 ALPHA")
+        LOGGER.info("USING VERSION 0.4.1 (0.4.0)")
 
         LOGGER.warning("LANISAPI IS STILL IN A EARLY STAGE SO EXPECT BUGS.")
 
         LOGGER.warning(
-            "IMPORTANT: Schulportal Hessen can change things quickly "
+            "IMPORTANT: Schulportal Hessen can change some things "
             "and is fragmented (some schools work, some not), "
             "so expect something to not be working"
         )
 
-        HTMLLogger.setup(self.save)
+        HTMLLogger.init()
 
     def __del__(self) -> None:
         """If the script closes close the parser."""
         Request.close()
 
     @property
     def authentication_cookies(self) -> LanisCookie:
@@ -111,58 +112,60 @@
 
     def close(self) -> None:
         """Close the client and saves to session.json; you need to do this."""
         Request.close()
 
         self.authenticated = False
 
-        # If we already authenticated using the file just update it quickly
-        if self.authentication_method == "SessionsFile":
-            with open("session.json", "r+") as file:
-                session_file: dict[str, any] = json.loads(file.read())
-                session_file["timestamp"] = time()
-                session_file.update(session_file)
-
-                file.seek(0)
-                file.write(json.dumps(session_file))
-
+        if (
+            self.session_type == SessionType.LONG
+            and self.authentication_method == self.AuthenticationMethod.SessionsFile
+        ):
             LOGGER.info("Closed current session.")
 
             return
 
-        # Encrypt the session data using AES-GCM and scrypt for the key
-        salt = get_random_bytes(12)
-        key = b64encode(scrypt(self.authentication.password, salt, 16, 2**14, 8, 1))
-        cipher = AES.new(key, AES.MODE_GCM, nonce=salt)
+        session_data_normal = {
+            "session_id": self.authentication_cookies.session_id,
+            "timestamp": time(),
+        }
 
-        session_id = cipher.encrypt_and_digest(
-            self.authentication_cookies.session_id.encode()
+        session_data_long = (
+            {"autologin": self.autologin[0], "timestamp": self.autologin[1]}
+            if self.session_type == SessionType.LONG
+            else None
         )
 
-        # session_id: Append salt to beginning (16 chars) then mac (32 chars) and then the ciphertext.
         session_data = {
-            "school_id": self.authentication_cookies.school_id,
-            "session_id": f"{b64encode(salt).decode()}{b64encode(session_id[1]).decode()}{b64encode(session_id[0]).decode()}",
-            "timestamp": time(),
+            "SCHOOLID": self.authentication_cookies.school_id,
+            "NORMAL": session_data_normal,
+            "LONG": session_data_long,
         }
 
         # If file exist update it.
         if Path("session.json").exists():
             with open("session.json", "r+") as file:
                 raw_session_file = file.read()
                 # If empty
                 if not raw_session_file:
                     file.write(json.dumps(session_data))
                     LOGGER.info("Closed current session.")
                     return
 
-                session_file: dict[str, any] = json.loads(raw_session_file)
+                session_file: JSON = json.loads(raw_session_file)
+                session_data["LONG"] = (
+                    session_file["LONG"]
+                    if session_data["LONG"] is None
+                    else session_data["LONG"]
+                )
+                session_data["NORMAL"]["timestamp"] = time()
                 session_file.update(session_data)
 
                 file.seek(0)
+                file.truncate(0)
                 file.write(json.dumps(session_file))
         else:
             with open("session.json", "w") as file:
                 file.write(json.dumps(session_data))
 
         LOGGER.info("Closed current session.")
 
@@ -171,157 +174,223 @@
         """Return all schools with their id, name and city.
 
         Returns
         -------
         list[dict[str, str]]
             JSON
         """
-        return _get_schools(self.save)
+        return _get_schools()
+
+    @handle_exceptions
+    def _create_new_session(self) -> None:
+        # Check if a id or school and place is provided.
+        if isinstance(self.authentication.school, str):
+            school_id = self.authentication.school
+        else:
+            schools = self.get_schools()
+
+            # Try to get wanted school with a one liner generator.
+            try:
+                school_id = next(
+                    school
+                    for school in schools
+                    if school["Name"] == self.authentication.school.name
+                    and school["Ort"] == self.authentication.school.city
+                )["Id"]
+            except StopIteration as err:
+                msg = "School doesn't exist, check for right spelling."
+                raise NoSchoolFoundError(msg) from err
+
+        # Get new session (value: SPH-Session) and autologin token by posting to login page.
+        if self.session_type == SessionType.LONG:
+            response_cookies, autologin = get_session_and_autologin(
+                school_id, self.authentication.username, self.authentication.password
+            )
+            self.autologin = autologin
+            response_location = "."
+        else:
+            response_cookies, response_location = get_session(
+                school_id, self.authentication.username, self.authentication.password
+            )
+
+        if not response_location:
+            # It also could be other problems, Lanis can be very finicky.
+            msg = "Could not log in, possibly wrong credentials."
+            raise WrongCredentialsError(msg)
+
+        # Get authentication url to get sid.
+        auth_url = get_authentication_url(response_cookies)
+
+        # Get sid.
+        Request.set_cookies(
+            get_authentication_sid(auth_url, response_cookies, school_id)
+        )
+
+        self.authentication_method = self.AuthenticationMethod.LanisAccount
+
+    @handle_exceptions
+    def _get_from_sessions_file(self) -> None:
+        with open("session.json", "r") as file:
+            raw_session_file = file.read()
+
+            # If session file is empty return forced authenticate
+            if raw_session_file:
+                try:
+                    session_file: JSON = json.loads(raw_session_file)
+                except json.JSONDecodeError as err:
+                    LOGGER.warning("Authenticate: session.json file is corrupted.")
+
+                    if not self.authentication:
+                        msg = "Can't login, no credentials and corrupted session.json."
+                        raise WrongCredentialsError(msg) from err
+
+                    os.remove("session.json")
+                    self.authenticate(force=True, session_type=self.session_type)
+                    raise ForceNewAuthenticationError from err
+            else:
+                LOGGER.info("Authenticate: session.json file is empty.")
+
+                if not self.authentication:
+                    msg = "Can't login, no credentials and empty session.json."
+                    raise WrongCredentialsError(msg)
+
+                self.authenticate(force=True, session_type=self.session_type)
+                raise ForceNewAuthenticationError
+
+            try:
+                if session_file["NORMAL"] and datetime.fromtimestamp(
+                    session_file["NORMAL"]["timestamp"]
+                ) > datetime.now() + timedelta(minutes=-100):
+                    session_id = session_file["NORMAL"]["session_id"]
+                else:
+                    LOGGER.info(
+                        "Authenticate: Check for long session, because normal session is empty or outdated."
+                    )
+                    # Check if autologin timestamp is older then now.
+                    if (
+                        session_file["LONG"]
+                        and datetime.fromtimestamp(session_file["LONG"]["timestamp"])
+                        > datetime.now()
+                    ):
+                        LOGGER.info(
+                            "Authenticate: Get now session id by autologin token."
+                        )
+
+                        self.autologin = session_file["LONG"]["autologin"]
+
+                        response_cookies = get_session_by_autologin(
+                            session_file["SCHOOLID"], self.autologin
+                        )
+
+                        auth_url = get_authentication_url(response_cookies)
+
+                        session_id = get_authentication_sid(
+                            auth_url,
+                            response_cookies,
+                            schoolid=session_file["SCHOOLID"],
+                        )["sid"]
+
+                        self.session_type = SessionType.LONG
+                    else:
+                        LOGGER.info("Authenticate: Long session is outdated or empty.")
+                        os.remove("session.json")
+                        self.authenticate(force=True, session_type=self.session_type)
+                        raise ForceNewAuthenticationError
+            except (ValueError, KeyError) as err:
+                LOGGER.info("Authenticate: session.json file is corrupted.")
+
+                if not self.authentication:
+                    msg = "Can't login, no credentials and corrupted session.json."
+                    raise WrongCredentialsError(msg) from err
+
+                self.authenticate(force=True, session_type=self.session_type)
+                raise ForceNewAuthenticationError from err
+
+            Request.set_cookies(
+                {
+                    "i": session_file["SCHOOLID"],
+                    "sid": session_id,
+                }
+            )
+
+            LOGGER.info("Authenticate: Using found session.json file.")
+            self.authentication_method = self.AuthenticationMethod.SessionsFile
 
     @handle_exceptions
-    def authenticate(self, force: bool = False) -> None:
+    def authenticate(
+        self, session_type: SessionType = SessionType.NORMAL, force: bool = False
+    ) -> None:
         """Log into the school portal and sets the session id in the auth_cookies.
 
         Parameters
         ----------
         force : bool, optional
             If True it always makes a new session with Lanis, by default False
+        session_type : SessionType, optional by default SessionType.NORMAL
+            Which session to create.
+            There are two session types: NORMAL and LONG. The long session is 30-days long (``angemeldet bleiben`` option) and needs no password or name to be put in afterwards.
+            It does not force a new session!
 
         Note
         ----
         Supports only the new system (login.schulportal.hessen.de).
         More at https://support.schulportal.hessen.de/knowledgebase.php?article=1087.
         """
         if self.authenticated:
             LOGGER.warning("Authenticate: Already authenticated.")
             return
 
-        school_id: int
+        self.session_type = session_type
 
+        if self.authentication is None and not Path("session.json").exists():
+            msg = "Can't login, no credentials and no session.json."
+            raise WrongCredentialsError(msg)
+
+        # First check if we can restore session from a file.
         if not force:
+            # LanisCookie login (highest priority)
             if isinstance(self.authentication, LanisCookie):
                 Request.set_cookies(
                     {
                         "i": self.authentication.school_id,
                         "sid": self.authentication.session_id,
                     }
                 )
                 LOGGER.info(
                     "Authenticate: Using cookies to authenticate, skip authentication."
                 )
-                self.authentication_method = "LanisCookie"
+                self.authentication_method = self.AuthenticationMethod.LanisCookie
+            # Login with session.json
             elif Path("session.json").exists():
-                with open("session.json", "r") as file:
-                    raw_session_file = file.read()
-
-                # If session file is empty return forced authenticate
-                if raw_session_file:
-                    try:
-                        session_file: dict[str, any] = json.loads(raw_session_file)
-                    except json.JSONDecodeError:
-                        LOGGER.warning("Authenticate: session.json file is corrupted.")
-                        os.remove("session.json")
-                        self.authenticate(True)
-                        return
-                else:
-                    LOGGER.info("Authenticate: session.json file is empty.")
-                    self.authenticate(True)
-                    return
-
-                # If session data is not older then 100 minutes.
-                if session_file and datetime.fromtimestamp(
-                    session_file["timestamp"]
-                ) > datetime.now() + timedelta(minutes=-100):
-                    # Preparing the decrypt of the session id.
-                    salt = b64decode(session_file["session_id"][:16])
-                    mac = b64decode(session_file["session_id"][16:40])
-                    key = b64encode(
-                        scrypt(
-                            self.authentication.password, salt, 16, 2**14, 8, 1
-                        )
-                    )
-                    cipher = AES.new(key, AES.MODE_GCM, nonce=salt)
-
-                    # Decrypt and verify if the mac is right.
-                    try:
-                        session_id = cipher.decrypt_and_verify(
-                            b64decode(session_file["session_id"][40:].encode()), mac
-                        ).decode()
-                    except ValueError:
-                        LOGGER.info("Authenticate: session.json file is corrupted.")
-                        self.authenticate(True)
-                        return
-
-                    Request.set_cookies(
-                        {
-                            "i": session_file["school_id"],
-                            "sid": session_id,
-                        }
-                    )
-                else:
-                    LOGGER.info("Authenticate: Session.json file is outdated.")
-                    os.remove("session.json")
-                    self.authenticate(True)
+                try:
+                    self._get_from_sessions_file()
+                except ForceNewAuthenticationError:
+                    LOGGER.info("Authenticate: Forced new authentication, return.")
                     return
 
-                LOGGER.info("Authenticate: Using found session.json file.")
-                self.authentication_method = "SessionsFile"
-
+        # Create new session if force is True or the other methods are False.
         if force or not (
             Path("session.json").exists()
             or isinstance(self.authentication, LanisCookie)
         ):
-            # Check if a id or school and place is provided.
-            if isinstance(self.authentication.school, str):
-                school_id = self.authentication.school
-            else:
-                schools = self.get_schools()
-
-                # Try to get wanted school with a one liner generator.
-                try:
-                    school_id = next(
-                        school
-                        for school in schools
-                        if school["Name"] == self.authentication.school.name
-                        and school["Ort"] == self.authentication.school.city
-                    )["Id"]
-                except StopIteration as err:
-                    msg = "School doesn't exist, check for right spelling."
-                    raise NoSchoolFoundError(msg) from err
-
-            # Get new session (value: SPH-Session) by posting to login page.
-            response_session = get_session(
-                school_id, self.authentication.username, self.authentication.password
-            )
-            response_cookies = response_session["cookies"]
-
-            if not response_session["location"]:
-                # It also could be other problems, Lanis can be very finicky.
-                msg = "Could not log in, possibly wrong credentials."
-                raise WrongCredentialsError(msg)
-
-            # Get authentication url to get sid.
-            auth_url = get_authentication_url(response_cookies)
-
-            # Get sid.
-            Request.set_cookies(
-                get_authentication_sid(auth_url, response_cookies, schoolid=school_id)
-            )
-
-            self.authentication_method = "LanisAccount"
+            self._create_new_session()
 
         # Tell Lanis how to encrypt
         if not self.cryptor.authenticate():
             LOGGER.error("Authenticate: Couldn't handshake with Lanis.")
             return
 
         self.authenticated = True
 
         available_apps = _get_available_apps()
 
+        LOGGER.info(f"Session type: {self.session_type.name}")
+
+        LOGGER.info(f"Authentication method: {self.authentication_method.name}")
+
         LOGGER.info(
             "Available apps:\n"
             f"  Calendar: {'Kalender' in available_apps}\n"
             + f"  Tasks: {'Mein Unterricht' in available_apps}\n"
             + f"  Conversations: {'Nachrichten - Beta-Version' in available_apps}\n"
             + f"  Substitution plan: {'Vertretungsplan' in available_apps}"
         )
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/constants.py` & `lanisapi-0.4.1/src/lanisapi/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """This script has various global constants."""
 
 import logging
 from dataclasses import dataclass
+from typing import TypeAlias
 from urllib.parse import urljoin
 
 LOGGER = logging.getLogger("LanisClient")
 
 logging.basicConfig(level=logging.INFO, format="%(levelname)s - %(name)s   %(message)s")
 
+JSON: TypeAlias = dict[str, any]
 
 @dataclass
 class URL:
     """Contain various constant URLs."""
 
     base = "https://start.schulportal.hessen.de/"
     index = urljoin(base, "index.php")
     conversations = urljoin(base, "nachrichten.php")
     tasks = urljoin(base, "meinunterricht.php")
     calendar = urljoin(base, "kalender.php")
     substitution_plan = urljoin(base, "vertretungsplan.php")
     schools = urljoin("https://startcache.schulportal.hessen.de/", "exporteur.php")
     encryption = urljoin(base, "ajax.php")
+    login = "https://login.schulportal.hessen.de/"
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/exceptions.py` & `lanisapi-0.4.1/src/lanisapi/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,8 +22,12 @@
 
 
 class WrongCredentialsError(Exception):
     """Returned if you passed a wrong password or username."""
 
 
 class NoSchoolFoundError(Exception):
-    """Returned if no school was found using the ``School`` params."""
+    """Returned if no school was found using the ``School`` params."""
+
+
+class ForceNewAuthenticationError(Exception):
+    """Thrown if we need to make a completely new session. Usually it is not thrown outside of the lib."""
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/apps.py` & `lanisapi-0.4.1/src/lanisapi/functions/apps.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/authentication_types.py` & `lanisapi-0.4.1/src/lanisapi/functions/authentication_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This script includes handy dataclasses for authenticating with Lanis."""
 
 from dataclasses import dataclass
+from enum import Enum
 
 
 @dataclass
 class School:
     """Alternative to school id for authentication.
 
     Parameters
@@ -52,7 +53,19 @@
     Note
     ----
     Use ``LanisClient.authentication_cookies`` from a previous session to get ``LanisCookie`` for the next session.
     """
 
     school_id: str
     session_id: str
+
+
+class SessionType(Enum):
+    """Used in ``authenticate()`` to indicate which session type you want.
+
+    * NORMAL, used to get a normal session which lasts 100min.
+    * LONG, used to get a 30-days (``angemeldet bleiben`` option).
+
+    """
+
+    NORMAL = 1
+    LONG = 2
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/calendar.py` & `lanisapi-0.4.1/src/lanisapi/functions/calendar.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/conversations.py` & `lanisapi-0.4.1/src/lanisapi/functions/conversations.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/schools.py` & `lanisapi-0.4.1/src/lanisapi/functions/schools.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 
 from ..constants import LOGGER, URL
 from ..helpers.request import Request
 
 
-def _get_schools(save: bool) -> list[dict[str, str]]:
+def _get_schools() -> list[dict[str, str]]:
     """Return all schools with their id, name and city.
 
     Returns
     -------
     list[dict[str, str]]
         JSON
     """
@@ -31,14 +31,10 @@
     schools = []
 
     # We don't want the categories only the schools.
     for group in response:
         for school in group["Schulen"]:
             schools.append(school)
 
-    if save is True:
-        with open("schools.json", "w") as file:
-            json.dump(schools, file)
-
     LOGGER.info("Get schools: Successfully got schools.")
 
     return schools
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/substitution.py` & `lanisapi-0.4.1/src/lanisapi/functions/substitution.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/functions/tasks.py` & `lanisapi-0.4.1/src/lanisapi/functions/tasks.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/helpers/cryptor.py` & `lanisapi-0.4.1/src/lanisapi/helpers/cryptor.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/helpers/html_logger.py` & `lanisapi-0.4.1/src/lanisapi/helpers/html_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,18 @@
 """This script includes the HTMLLogger for handy html bug reports."""
 import os
 from time import time
 
-from ..constants import LOGGER
-
 
 class HTMLLogger:
     """Provide various logging functions to send html code for bug reports."""
 
-    save: bool
-
     @classmethod
-    def setup(cls, save_to_file: bool) -> None:
-        """Create a initial html_logs.txt file and checks if saving is allowed.
-
-        Parameters
-        ----------
-        save_to_file : bool
-            _description_
-        """
-        cls.save = save_to_file
-
-        if not cls.save:
-            LOGGER.info(
-                "HTMLLogger: Saving to file was set to False, logs will be very messy!"
-            )
-            return
-
+    def init(cls) -> None:
+        """Create a initial html_logs.txt file and checks if saving is allowed."""
         if not os.path.exists("html_logs.txt"):
             with open("html_logs.txt", "w", encoding="utf-8") as file:
                 file.writelines(
                     [
                         "## Info ################################################################################################\n",
                         "# This file has various html data WHICH MAY CONTAIN SENSITIVE DATA but it's very useful for debugging! #\n",
                         "# This file will be uploaded by you to the GitHub errors page if any warning or error occurred!         #\n"
@@ -70,13 +52,9 @@
 *~~Element-HTML~~~~~~~~~~~~*
 
 {html}
 #--End--------------------------#
 
 """
 
-        if not cls.save:
-            LOGGER.info(f"HTMLLogger: {log}")
-            return
-
         with open("html_logs.txt", "a", encoding="utf-8") as file:
             file.write(log)
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi/helpers/request.py` & `lanisapi-0.4.1/src/lanisapi/helpers/request.py`

 * *Files identical despite different names*

### Comparing `lanisapi-0.4.0a0/src/lanisapi/helpers/wrappers.py` & `lanisapi-0.4.1/src/lanisapi/helpers/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import httpx
 
 from ..constants import LOGGER
 from ..exceptions import (
     AppNotAvailableError,
     CriticalElementWasNotFoundError,
+    ForceNewAuthenticationError,
     LoginPageRedirectError,
     NoSchoolFoundError,
     NotAuthenticatedError,
     PageNotFoundError,
     WrongCredentialsError,
 )
 from ..functions.apps import _get_app_availability
@@ -34,14 +35,15 @@
             )
         except (
             PageNotFoundError,
             CriticalElementWasNotFoundError,
             LoginPageRedirectError,
             NoSchoolFoundError,
             WrongCredentialsError,
+            ForceNewAuthenticationError,
         ) as err:
             raise err
 
     return handle_exceptions_wrapper
 
 
 def requires_auth(function: FunctionType) -> FunctionType:
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi.egg-info/PKG-INFO` & `lanisapi-0.4.1/src/lanisapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanisapi
-Version: 0.4.0a0
+Version: 0.4.1
 Summary: A unofficial python api for Lanis.
 Author: kurwjan
 Project-URL: Homepage, https://github.com/kurwjan/LanisAPI
 Project-URL: Bug Tracker, https://github.com/kurwjan/LanisAPI/issues
 Project-URL: Documentation, https://lanisapi.readthedocs.io/
 Keywords: Lanis,SPH,Schulportal Hessen,Hessen,API
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: German
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: selectolax
 Requires-Dist: pycryptodomex
+Requires-Dist: py-machineid
 
 [[README DE](https://github.com/kurwjan/LanisAPI/blob/master/README-DE.md)]  [[README EN](https://github.com/kurwjan/LanisAPI/blob/master/README.md)]
 
 # LanisAPI
 
 > ## ⚠ Notice
 > **Because the Schulportal Hessen changes quickly and is very fragmented, some functions at specific schools or after a while may no longer work.**
@@ -36,14 +37,19 @@
 + Fetch calendar events.
 + Fetch conversations.
 + Fetch all schools that have Lanis.
 + Fetch all web applets with their links.
 
 **Overview of future Features, Problems and other things [here](https://github.com/users/kurwjan/projects/2).**
 
+## App for the Schulportal Hessen
+If you want to have an app for Lanis, check out [SPH-vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) by [@alessioC42](https://github.com/alessioC42). _It's still in an early phase!_
+
+**It would be also really nice if you contribute to this project**, like bug reporting, if you know Dart and Flutter it would be nice to see your help or you could learn Dart, it's not hard.
+
 ## How do I install it?
 
 ```sh
 pip install lanisapi
 ```
 
 Required is Python 3.11. *(older versions are probably not working, I didn't tested it.)*
@@ -81,15 +87,15 @@
 
 The Javascript project [SPHclient](https://github.com/alessioC42/SPHclient) from [@alessioC42](https://github.com/alessioC42) helped me to understand the *Schulportal Hessen*.
 
 The Android-App [sph-planner](https://github.com/koenidv/sph-planner) from [@koenidv](https://github.com/koenidv) helped me to understand the Level 2 encryption.
 
 Other projects that didn't helped me but are cool:
 
-+ **Good TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)**
-+ Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)
++ **Flutter Android app [SPH-Vertretungsplan](https://github.com/alessioC42/SPH-vertretungsplan) also from [@alessioC42](https://github.com/alessioC42)**
++ TypeScript library [Maria](https://github.com/elderguardian/maria) from [Elderguardian](https://github.com/elderguardian/)
 + Javascript app [SchulportalApp](https://github.com/DerOwnerHD/SchulportalApp) from [DerOwnerHD](https://github.com/DerOwnerHD)
 + Flutter Android app [lkwslr-sphplaner](https://github.com/flutter-preview/lkwslr-sphplaner) from [flutter-preview](https://github.com/flutter-preview)
 
 ## Notice
 
 This project isn't officially related to the Schulportal Hessen. It's only a unofficial library, supported by the community.
```

### Comparing `lanisapi-0.4.0a0/src/lanisapi.egg-info/SOURCES.txt` & `lanisapi-0.4.1/src/lanisapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

