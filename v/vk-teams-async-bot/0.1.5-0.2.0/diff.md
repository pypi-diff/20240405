# Comparing `tmp/vk_teams_async_bot-0.1.5.tar.gz` & `tmp/vk_teams_async_bot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_teams_async_bot-0.1.5.tar", max compression
+gzip compressed data, was "vk_teams_async_bot-0.2.0.tar", max compression
```

## Comparing `vk_teams_async_bot-0.1.5.tar` & `vk_teams_async_bot-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.1.5/LICENSE
--rw-r--r--   0        0        0     1241 2024-03-25 15:24:40.640733 vk_teams_async_bot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.1.5/vk_teams_async_bot/__init__.py
--rw-r--r--   0        0        0    19962 2024-03-25 14:31:13.864811 vk_teams_async_bot-0.1.5/vk_teams_async_bot/bot.py
--rw-r--r--   0        0        0     4612 2024-03-25 14:06:32.604894 vk_teams_async_bot-0.1.5/vk_teams_async_bot/client_session.py
--rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.1.5/vk_teams_async_bot/constants.py
--rw-r--r--   0        0        0      700 2023-12-27 07:24:44.106567 vk_teams_async_bot-0.1.5/vk_teams_async_bot/dispatcher.py
--rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.1.5/vk_teams_async_bot/errors.py
--rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.1.5/vk_teams_async_bot/events.py
--rw-r--r--   0        0        0     4376 2023-12-28 07:46:16.381833 vk_teams_async_bot-0.1.5/vk_teams_async_bot/filter.py
--rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.1.5/vk_teams_async_bot/handler.py
--rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.1.5/vk_teams_async_bot/helpers.py
--rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.1.5/vk_teams_async_bot/middleware.py
--rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.1.5/vk_teams_async_bot/schemas.py
--rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.1.5/vk_teams_async_bot/state.py
--rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.1.5/vk_teams_async_bot/timer.py
--rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1241 2024-04-05 10:48:05.457116 vk_teams_async_bot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.2.0/vk_teams_async_bot/__init__.py
+-rw-r--r--   0        0        0    20547 2024-04-05 10:39:04.137243 vk_teams_async_bot-0.2.0/vk_teams_async_bot/bot.py
+-rw-r--r--   0        0        0     4612 2024-04-03 15:58:15.609070 vk_teams_async_bot-0.2.0/vk_teams_async_bot/client_session.py
+-rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.2.0/vk_teams_async_bot/constants.py
+-rw-r--r--   0        0        0      700 2023-12-27 07:24:44.106567 vk_teams_async_bot-0.2.0/vk_teams_async_bot/dispatcher.py
+-rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.2.0/vk_teams_async_bot/errors.py
+-rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.2.0/vk_teams_async_bot/events.py
+-rw-r--r--   0        0        0     4763 2024-04-05 10:44:28.021696 vk_teams_async_bot-0.2.0/vk_teams_async_bot/filter.py
+-rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.2.0/vk_teams_async_bot/handler.py
+-rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.2.0/vk_teams_async_bot/helpers.py
+-rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.2.0/vk_teams_async_bot/middleware.py
+-rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.2.0/vk_teams_async_bot/schemas.py
+-rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.2.0/vk_teams_async_bot/state.py
+-rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.2.0/vk_teams_async_bot/timer.py
+-rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.2.0/PKG-INFO
```

### Comparing `vk_teams_async_bot-0.1.5/LICENSE` & `vk_teams_async_bot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/pyproject.toml` & `vk_teams_async_bot-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vk-teams-async-bot"
-version = "0.1.5"
+version = "0.2.0"
 description = ""
 authors = ["Александр Смирнов <alexsmi4444@gmail.com>"]
 readme = "README.md"
 packages = [{include = "vk_teams_async_bot"}]
 license = "MIT"
 repository = "https://github.com/Quakeer444/vk_teams_async_bot"
```

### Comparing `vk_teams_async_bot-0.1.5/README.md` & `vk_teams_async_bot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/bot.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 from io import BytesIO
 from typing import TypeAlias
 
+import aiohttp
 from aiohttp import FormData
 
 from .client_session import VKTeamsSession
 from .constants import ParseMode
 from .dispatcher import Dispatcher
 from .events import Event, EventType
 from .helpers import Format, InlineKeyboardMarkup, async_read_file, format_to_json
@@ -350,14 +351,28 @@
             if inline_keyboard_markup is not None
             else None,
             format=_format if isinstance(_format, str) else format_to_json(_format),
             parse_mode=parse_mode,
             _count_request_retries=count_request_retries,
         )
 
+    @staticmethod
+    async def download_file(file_url: str) -> bytes:
+        """
+        Method for downloading a file
+
+        :param file_url: The URL of the file to download.
+        :return: - bytes: The content of the file as bytes
+                 - None: If the response status code is not 200.
+        """
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(10)) as session:
+            async with session.get(file_url) as response:
+                if response.status == 200:
+                    return await response.read()
+
     async def delete_msg(
         self, chat_id: str, msg_id: list[str], count_request_retries: int = 2
     ):
         """
         Delete a message
 
         :param chat_id: Unique nickname or chat id.
```

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/client_session.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/client_session.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/constants.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/constants.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/dispatcher.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/events.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/events.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/filter.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 
 class AndFilter(CompositeFilter):
     def filter(self, event):
         return self.filter_1(event) and self.filter_2(event)
 
 
+class OrFilter(CompositeFilter):
+    def filter(self, event):
+        return self.filter_1(event) or self.filter_2(event)
+
+
 class MessageFilter(FilterBase):
     def filter(self, event: Event):
         return bool(event.type == EventType.NEW_MESSAGE)
 
 
 class FileFilter(MessageFilter):
     def filter(self, event):
@@ -122,15 +127,23 @@
     def __init__(self, pattern):
         super(RegexpFilter, self).__init__()
 
         self.pattern = re.compile(pattern)
 
     def filter(self, event):
         return super(RegexpFilter, self).filter(event) and self.pattern.search(
-            event.data["text"].strip()
+            event.data.get("text", "").strip()
+        )
+
+
+class ForwardFilter(MessageFilter):
+    def filter(self, event):
+        return (
+            'parts' in event.data and
+            any(p['type'] == Parts.FORWARD.value for p in event.data['parts'])
         )
 
 
 class TagFilter(MessageFilter):
     def __init__(self, tags: list):
         super(MessageFilter, self).__init__()
         self.tags = tags
@@ -146,7 +159,8 @@
     callback_data_regexp = CallbackDataRegexpFilter
     file = FileFilter()
     command = CommandFilter
     state = StateUserFilter
     state_regex = StateUserRegexFilter
     reply = ReplyFilter()
     tag = TagFilter
+    forward = ForwardFilter()
```

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/handler.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/handler.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/helpers.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/helpers.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/state.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/state.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/vk_teams_async_bot/timer.py` & `vk_teams_async_bot-0.2.0/vk_teams_async_bot/timer.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.1.5/PKG-INFO` & `vk_teams_async_bot-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vk-teams-async-bot
-Version: 0.1.5
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/Quakeer444/vk_teams_async_bot
 License: MIT
 Author: Александр Смирнов
 Author-email: alexsmi4444@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

