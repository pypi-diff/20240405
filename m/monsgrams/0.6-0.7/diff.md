# Comparing `tmp/monsgrams-0.6.tar.gz` & `tmp/monsgrams-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.6.tar", last modified: Thu Apr  4 19:17:38 2024, max compression
+gzip compressed data, was "monsgrams-0.7.tar", last modified: Thu Apr  4 20:00:29 2024, max compression
```

## Comparing `monsgrams-0.6.tar` & `monsgrams-0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.956426 monsgrams-0.6/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      615 2024-04-04 19:17:38.952426 monsgrams-0.6/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      434 2024-04-04 19:14:44.000000 monsgrams-0.6/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.940426 monsgrams-0.6/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.6/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      412 2024-04-04 18:43:28.000000 monsgrams-0.6/monsgrams/api.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1337 2024-04-04 19:15:40.000000 monsgrams-0.6/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.948426 monsgrams-0.6/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      615 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      207 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 19:17:38.956426 monsgrams-0.6/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      333 2024-04-04 19:17:04.000000 monsgrams-0.6/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.996426 monsgrams-0.7/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-04 20:00:28.996426 monsgrams-0.7/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.7/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.984426 monsgrams-0.7/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       82 2024-04-04 19:58:17.000000 monsgrams-0.7/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      778 2024-04-04 19:50:47.000000 monsgrams-0.7/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      210 2024-04-04 19:58:09.000000 monsgrams-0.7/monsgrams/context.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1463 2024-04-04 19:58:55.000000 monsgrams-0.7/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 20:00:28.992426 monsgrams-0.7/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      759 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      228 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 20:00:28.000000 monsgrams-0.7/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 20:00:29.000426 monsgrams-0.7/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      387 2024-04-04 19:28:18.000000 monsgrams-0.7/setup.py
```

### Comparing `monsgrams-0.6/monsgrams/main.py` & `monsgrams-0.7/monsgrams/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import asyncio
 import aiohttp
 from api import TelegramAPI
+from context import BotContext
 
 class Bot:
     def __init__(self, token):
         self.api = TelegramAPI(token)
         self.commands = {}
 
     async def get_updates(self, offset=None):
-        url = self.api.base_url + "getUpdates"
-        params = {"offset": offset} if offset else {}
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, params=params) as response:
-                return await response.json()
+        return await self.api.get_updates(offset)
 
     def command(self, name):
         def decorator(func):
             self.commands[name] = func
             return func
         return decorator
 
@@ -25,15 +22,20 @@
         while True:
             updates = await self.get_updates(offset)
             for update in updates.get("result", []):
                 offset = update["update_id"] + 1
                 message = update.get("message", {})
                 text = message.get("text", "")
                 chat_id = message.get("chat", {}).get("id")
+                from_user_id = message.get("from", {}).get("id")
+                chat_type = message.get("chat", {}).get("type")
                 if text.startswith("/"):
                     command_name = text.split()[0][1:]
                     command = self.commands.get(command_name)
                     if command:
-                        await command(self, chat_id)
+                        context = BotContext(self, chat_id, from_user_id, chat_type)
+                        await command(context)
                     else:
                         print("not found cmd")
 
+    async def send_message(self, chat_id, text):
+        return await self.api.send_message(chat_id, text)
```

