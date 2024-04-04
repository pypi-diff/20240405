# Comparing `tmp/minigram_py-0.1.2.tar.gz` & `tmp/minigram_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minigram_py-0.1.2.tar", last modified: Wed Apr  3 21:08:36 2024, max compression
+gzip compressed data, was "minigram_py-0.1.3.tar", last modified: Thu Apr  4 22:36:23 2024, max compression
```

## Comparing `minigram_py-0.1.2.tar` & `minigram_py-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.2/LICENSE
--rw-r--r--   0        0        0     2922 2024-04-03 21:06:24.236374 minigram_py-0.1.2/README.md
--rw-r--r--   0        0        0      542 2024-04-03 21:08:36.048473 minigram_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.2/src/minigram/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.2/src/minigram/aiohttp.py
--rw-r--r--   0        0        0      698 2024-04-03 21:07:03.769425 minigram_py-0.1.2/src/minigram/ass.py
--rw-r--r--   0        0        0     5105 2024-04-03 21:05:43.162608 minigram_py-0.1.2/src/minigram/main.py
--rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.2/src/minigram/py.typed
--rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.2/src/minigram/request.py
--rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.2/src/minigram/starlette.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 minigram_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2922 2024-04-03 21:06:24.236374 minigram_py-0.1.3/README.md
+-rw-r--r--   0        0        0      542 2024-04-04 22:36:23.608093 minigram_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.3/src/minigram/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.3/src/minigram/aiohttp.py
+-rw-r--r--   0        0        0      698 2024-04-03 21:07:03.769425 minigram_py-0.1.3/src/minigram/ass.py
+-rw-r--r--   0        0        0     5070 2024-04-04 22:35:29.636944 minigram_py-0.1.3/src/minigram/main.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.3/src/minigram/py.typed
+-rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.3/src/minigram/request.py
+-rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.3/src/minigram/starlette.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 minigram_py-0.1.3/PKG-INFO
```

### Comparing `minigram_py-0.1.2/LICENSE` & `minigram_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.2/README.md` & `minigram_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.2/pyproject.toml` & `minigram_py-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "minigram-py"
-version = "0.1.2"
+version = "0.1.3"
 description = "minimalistic telegram bot framework that can be used in AWS Lambda or anywhere"
 authors = [
     { name = "Grigory Bakunov", email = "bobuk@rubedo.cloud" },
 ]
 dependencies = []
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `minigram_py-0.1.2/src/minigram/ass.py` & `minigram_py-0.1.3/src/minigram/ass.py`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.2/src/minigram/main.py` & `minigram_py-0.1.3/src/minigram/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         if CURRENT is None:
             raise ValueError("No current MiniGram")
         return CURRENT
 
     @ass
     async def req(self, method: str, **kwargs) -> dict:
         url = f"https://api.telegram.org/bot{self.key}/{method}"
-        print("log2", url, kwargs)
         code, response = await req(url, kwargs)
         return response
 
     @ass
     async def start_polling(self):
         while True:
             updates = await self.get_updates()
```

### Comparing `minigram_py-0.1.2/src/minigram/request.py` & `minigram_py-0.1.3/src/minigram/request.py`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.2/PKG-INFO` & `minigram_py-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minigram-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: minimalistic telegram bot framework that can be used in AWS Lambda or anywhere
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: MIT
 Requires-Python: >=3.12
 Provides-Extra: starlette
 Provides-Extra: aiohttp
 Requires-Dist: starlette>=0.37.2; extra == "starlette"
```

