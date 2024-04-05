# Comparing `tmp/antfyutils-0.0.5.tar.gz` & `tmp/antfyutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antfyutils-0.0.5.tar", last modified: Wed Apr  3 01:55:02 2024, max compression
+gzip compressed data, was "antfyutils-0.0.6.tar", last modified: Fri Apr  5 13:38:17 2024, max compression
```

## Comparing `antfyutils-0.0.5.tar` & `antfyutils-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:55:02.965452 antfyutils-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      177 2024-04-03 01:55:02.961452 antfyutils-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:55:02.961452 antfyutils-0.0.5/antfyutils/
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-31 14:22:59.000000 antfyutils-0.0.5/antfyutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 14:22:59.000000 antfyutils-0.0.5/antfyutils/data_obj.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-03-31 10:25:33.000000 antfyutils-0.0.5/antfyutils/format.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 10:25:33.000000 antfyutils-0.0.5/antfyutils/obj.py
--rw-r--r--   0 root         (0) root         (0)     3695 2024-04-03 01:54:30.000000 antfyutils-0.0.5/antfyutils/push_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:55:02.961452 antfyutils-0.0.5/antfyutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      177 2024-04-03 01:55:02.000000 antfyutils-0.0.5/antfyutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2024-04-03 01:55:02.000000 antfyutils-0.0.5/antfyutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 01:55:02.000000 antfyutils-0.0.5/antfyutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-03 01:55:02.000000 antfyutils-0.0.5/antfyutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 01:55:02.000000 antfyutils-0.0.5/antfyutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-04-03 01:54:30.000000 antfyutils-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 01:55:02.965452 antfyutils-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:38:17.108388 antfyutils-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-05 13:38:17.108388 antfyutils-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:38:17.104388 antfyutils-0.0.6/antfyutils/
+-rw-r--r--   0 root         (0) root         (0)      115 2024-03-31 14:22:59.000000 antfyutils-0.0.6/antfyutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 14:22:59.000000 antfyutils-0.0.6/antfyutils/data_obj.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-03-31 10:25:33.000000 antfyutils-0.0.6/antfyutils/format.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 10:25:33.000000 antfyutils-0.0.6/antfyutils/obj.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-04-05 13:35:47.000000 antfyutils-0.0.6/antfyutils/push_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 13:38:17.108388 antfyutils-0.0.6/antfyutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-05 13:38:17.000000 antfyutils-0.0.6/antfyutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2024-04-05 13:38:17.000000 antfyutils-0.0.6/antfyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 13:38:17.000000 antfyutils-0.0.6/antfyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-05 13:38:17.000000 antfyutils-0.0.6/antfyutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-05 13:38:17.000000 antfyutils-0.0.6/antfyutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-05 13:37:22.000000 antfyutils-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 13:38:17.108388 antfyutils-0.0.6/setup.cfg
```

### Comparing `antfyutils-0.0.5/antfyutils/data_obj.py` & `antfyutils-0.0.6/antfyutils/data_obj.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.5/antfyutils/format.py` & `antfyutils-0.0.6/antfyutils/format.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.5/antfyutils/obj.py` & `antfyutils-0.0.6/antfyutils/obj.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.5/antfyutils/push_utils.py` & `antfyutils-0.0.6/antfyutils/push_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     # lock: threading.RLock
     def __init__(self, cfg: CfgDcNtfy, queue_size=30, cn=False, info=True) -> None:
         self.cfg = cfg
         self.pool = asyncio.Queue(maxsize=queue_size)
         self.thread = None
         self.cn = cn
         self.info = info
+        self.eventloop = asyncio.new_event_loop()
         pass
     async def __run_loop(self):
         asyncio.set_event_loop(self.eventloop)
         s = set()
         while True:
             msg = await self.pool.get()
             if not msg:
@@ -39,15 +40,14 @@
                 if self.pool.empty():
                     break
                 msg = self.pool.get_nowait()
             await asyncio.gather(*s)
             await asyncio.sleep(0.1)
         pass
     def __run_thread(self):
-        self.eventloop = asyncio.new_event_loop()
         self.eventloop.run_until_complete(self.__run_loop())
         pass
     def startServer(self):
         self.thread = Thread(name="Push Thread", target=self.__run_thread)
         self.thread.start()
         pass
     def stopServer(self):
```

