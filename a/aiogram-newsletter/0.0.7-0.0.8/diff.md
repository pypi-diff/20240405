# Comparing `tmp/aiogram-newsletter-0.0.7.tar.gz` & `tmp/aiogram-newsletter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-newsletter-0.0.7.tar", last modified: Wed Mar  6 00:59:02 2024, max compression
+gzip compressed data, was "aiogram-newsletter-0.0.8.tar", last modified: Fri Apr  5 21:56:36 2024, max compression
```

## Comparing `aiogram-newsletter-0.0.7.tar` & `aiogram-newsletter-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-03-06 00:59:02.218048 aiogram-newsletter-0.0.7/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1066 2024-03-03 00:51:30.000000 aiogram-newsletter-0.0.7/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-03-06 00:59:02.218048 aiogram-newsletter-0.0.7/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1985 2024-03-03 00:51:38.000000 aiogram-newsletter-0.0.7/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-03-06 00:59:02.214048 aiogram-newsletter-0.0.7/aiogram_newsletter/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-02 00:31:45.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    10748 2024-03-06 00:55:32.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/handlers.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8190 2024-03-06 00:55:32.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/manager.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1504 2024-03-03 00:51:38.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/middleware.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-03-06 00:59:02.218048 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-02-22 07:28:44.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      409 2024-03-01 00:32:48.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/exceptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7165 2024-03-02 01:06:08.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/keyboards.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2868 2024-03-06 00:55:32.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/misc.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      367 2024-03-01 21:20:40.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/states.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9124 2024-03-04 11:26:24.000000 aiogram-newsletter-0.0.7/aiogram_newsletter/utils/texts.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-03-06 00:59:02.218048 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-03-06 00:59:02.000000 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      576 2024-03-06 00:59:02.000000 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-03-06 00:59:02.000000 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       29 2024-03-06 00:59:02.000000 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-03-06 00:59:02.000000 aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-03-06 00:59:02.218048 aiogram-newsletter-0.0.7/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      898 2024-03-06 00:56:58.000000 aiogram-newsletter-0.0.7/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1066 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1985 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.875754 aiogram-newsletter-0.0.8/aiogram_newsletter/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    10748 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/handlers.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8129 2024-04-05 21:55:03.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/manager.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1504 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/middleware.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      409 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7165 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/keyboards.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2868 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/misc.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      367 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/states.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9124 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/texts.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      576 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       29 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      898 2024-04-05 21:56:11.000000 aiogram-newsletter-0.0.8/setup.py
```

### Comparing `aiogram-newsletter-0.0.7/LICENSE` & `aiogram-newsletter-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/PKG-INFO` & `aiogram-newsletter-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aiogram-newsletter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Newsletter handler for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-newsletter/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiogram>=3
-Requires-Dist: apscheduler>=3.10
+Requires-Dist: apscheduler==3.10
 
 # 📦 aiogram Newsletter Handler
 
 [![PyPI](https://img.shields.io/pypi/v/aiogram-newsletter.svg?color=FFE873&labelColor=3776AB)](https://pypi.python.org/pypi/aiogram-newsletter)
 ![Python Versions](https://img.shields.io/badge/Python-3.8%20--%203.12-black?color=FFE873&labelColor=3776AB)
 [![License](https://img.shields.io/github/license/nessshon/aiogram-newsletter)](https://github.com/nessshon/aiogram-newsletter/blob/main/LICENSE)
```

### Comparing `aiogram-newsletter-0.0.7/README.md` & `aiogram-newsletter-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/handlers.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/handlers.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/manager.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from aiogram.exceptions import TelegramBadRequest
 from aiogram.fsm.context import FSMContext
 from aiogram.types import (
     InlineKeyboardMarkup,
     Message,
     User,
 )
-from pytz import timezone
 
 from .utils.exceptions import (
     MESSAGE_DELETE_ERRORS,
     MESSAGE_EDIT_ERRORS,
 )
 from .utils.keyboards import InlineKeyboard
 from .utils.misc import DataStorage
@@ -153,15 +152,15 @@
         await self.state.set_state(ANState.confirmation_now)
         return message
 
     async def open_send_datetime_window(self, text: str = None) -> Message:
         if not text:
             text = self.text_message.get("send_datetime")
         reply_markyp = self.inline_keyboard.back()
-        datetime_now = datetime.now(timezone(self.apscheduler.timezone))
+        datetime_now = datetime.now()
         text = text.format(datetime_string=datetime_now.strftime("%Y-%m-%d %H:%M"))
 
         message = await self.send_message(text, reply_markup=reply_markyp)
         await self.state.set_state(ANState.send_datetime)
         return message
 
     async def open_confirmation_later_window(self) -> Message:
```

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/middleware.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/utils/keyboards.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/utils/misc.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter/utils/texts.py` & `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/texts.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/PKG-INFO` & `aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aiogram-newsletter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Newsletter handler for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-newsletter/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiogram>=3
-Requires-Dist: apscheduler>=3.10
+Requires-Dist: apscheduler==3.10
 
 # 📦 aiogram Newsletter Handler
 
 [![PyPI](https://img.shields.io/pypi/v/aiogram-newsletter.svg?color=FFE873&labelColor=3776AB)](https://pypi.python.org/pypi/aiogram-newsletter)
 ![Python Versions](https://img.shields.io/badge/Python-3.8%20--%203.12-black?color=FFE873&labelColor=3776AB)
 [![License](https://img.shields.io/github/license/nessshon/aiogram-newsletter)](https://github.com/nessshon/aiogram-newsletter/blob/main/LICENSE)
```

### Comparing `aiogram-newsletter-0.0.7/aiogram_newsletter.egg-info/SOURCES.txt` & `aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.7/setup.py` & `aiogram-newsletter-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiogram-newsletter",
-    version="0.0.7",
+    version="0.0.8",
     author="nessshon",
     description="Newsletter handler for aiogram bots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["example"]),
     install_requires=[
         "aiogram>=3",
-        "apscheduler>=3.10",
+        "apscheduler==3.10",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

