# Comparing `tmp/monsgrams-0.9.tar.gz` & `tmp/monsgrams-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.9.tar", last modified: Fri Apr  5 03:31:11 2024, max compression
+gzip compressed data, was "monsgrams-1.1.tar", last modified: Fri Apr  5 04:54:30 2024, max compression
```

## Comparing `monsgrams-0.9.tar` & `monsgrams-1.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.462729 monsgrams-0.9/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      789 2024-04-05 03:31:11.462729 monsgrams-0.9/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      523 2024-04-04 20:00:03.000000 monsgrams-0.9/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.450729 monsgrams-0.9/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       52 2024-04-04 23:18:54.000000 monsgrams-0.9/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      167 2024-04-05 03:30:56.000000 monsgrams-0.9/monsgrams/api.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     2175 2024-04-05 03:11:01.000000 monsgrams-0.9/monsgrams/bot.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      395 2024-04-04 22:54:44.000000 monsgrams-0.9/monsgrams/context.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 03:31:11.458729 monsgrams-0.9/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      789 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      259 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       15 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/requires.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 03:31:11.000000 monsgrams-0.9/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 03:31:11.466729 monsgrams-0.9/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      443 2024-04-05 03:29:33.000000 monsgrams-0.9/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.786729 monsgrams-1.1/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)     1118 2024-04-05 04:54:30.786729 monsgrams-1.1/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      852 2024-04-05 04:52:16.000000 monsgrams-1.1/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.770729 monsgrams-1.1/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       20 2024-04-05 04:49:36.000000 monsgrams-1.1/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     4013 2024-04-05 04:49:25.000000 monsgrams-1.1/monsgrams/bot.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-05 04:54:30.782729 monsgrams-1.1/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)     1118 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      221 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       15 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/requires.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-05 04:54:30.000000 monsgrams-1.1/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-05 04:54:30.786729 monsgrams-1.1/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      443 2024-04-05 04:54:22.000000 monsgrams-1.1/setup.py
```

### Comparing `monsgrams-0.9/README.md` & `monsgrams-1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 **This library provides interesting opportunities for creating telegram bots.
 convenient syntax, decorators.**
 
 # EXAMPLE USE!
 ```python
-bot = Bot("7181251700:AAF26R-70RNWYXprybRMqtthnTRjJU7LeNM")
+import asyncio
+from monsgrams import Bot
+bot = Bot("")
 
 @bot.command("start")
 async def start_command(context):
-    await context.bot.send_message(context.chat_id, f"Hello! I am bot. How are you? User ID: {context.from_user_id}, Chat Type: {context.chat_type}")
+    chat_info = await bot.get_chat(context.chat_id)
+    chat_id = chat_info['result']['id']
+    username = chat_info['result']['username']
+    await bot.send_message(chat_id, f"Hello, {username}!")
+
+@bot.command("avatar")
+async def avatar_command(context):
+    photos_info = await bot.get_user_profile_photos(context.user_id)
+    print(photos_info)
+    file_id = photos_info['result']['photos'][-1][-1]['file_id']
+    print(file_id)
+    await bot.send_photo(context.chat_id, file_id)
 
 async def main():
     await bot.polling_loop()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

