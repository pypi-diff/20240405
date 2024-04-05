# Comparing `tmp/shuttleai-3.8.1.tar.gz` & `tmp/shuttleai-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.1.tar", last modified: Wed Apr  3 08:55:23 2024, max compression
+gzip compressed data, was "shuttleai-3.8.2.tar", last modified: Fri Apr  5 17:14:45 2024, max compression
```

## Comparing `shuttleai-3.8.1.tar` & `shuttleai-3.8.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.131689 shuttleai-3.8.1/
--rw-rw-rw-   0        0        0     4084 2024-04-03 08:55:23.130688 shuttleai-3.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 08:55:23.132693 shuttleai-3.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-04-03 08:26:16.000000 shuttleai-3.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.088688 shuttleai-3.8.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.093687 shuttleai-3.8.1/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-03 08:54:18.000000 shuttleai-3.8.1/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.1/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.124689 shuttleai-3.8.1/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-02 07:23:05.000000 shuttleai-3.8.1/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17321 2024-04-03 08:54:24.000000 shuttleai-3.8.1/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0     3331 2024-04-03 08:54:30.000000 shuttleai-3.8.1/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.1/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.127687 shuttleai-3.8.1/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.1/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.1/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:55:23.128692 shuttleai-3.8.1/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4084 2024-04-03 08:55:22.000000 shuttleai-3.8.1/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-03 08:55:23.000000 shuttleai-3.8.1/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:55:22.000000 shuttleai-3.8.1/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-03 08:55:22.000000 shuttleai-3.8.1/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-04-03 08:55:22.000000 shuttleai-3.8.1/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 08:55:22.000000 shuttleai-3.8.1/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.654879 shuttleai-3.8.2/
+-rw-rw-rw-   0        0        0     4184 2024-04-05 17:14:45.653880 shuttleai-3.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:14:45.654879 shuttleai-3.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1783 2024-04-05 17:11:32.000000 shuttleai-3.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.613884 shuttleai-3.8.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.618879 shuttleai-3.8.2/src/shuttleai/
+-rw-rw-rw-   0        0        0      576 2024-04-05 17:13:49.000000 shuttleai-3.8.2/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.2/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.646881 shuttleai-3.8.2/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.2/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17420 2024-04-05 17:14:00.000000 shuttleai-3.8.2/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0     3331 2024-04-05 17:14:05.000000 shuttleai-3.8.2/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0    10161 2024-04-05 17:14:08.000000 shuttleai-3.8.2/src/shuttleai/client/_syncr.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.2/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.649879 shuttleai-3.8.2/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.2/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.2/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:14:45.651879 shuttleai-3.8.2/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4184 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 17:14:45.000000 shuttleai-3.8.2/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.1/PKG-INFO` & `shuttleai-3.8.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.1
+Version: 3.8.2
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: orjson
+Requires-Dist: pydantic
 Provides-Extra: cli
-Requires-Dist: asyncclick; extra == "cli"
-Requires-Dist: pystyle; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
+Requires-Dist: aiohttp; extra == "cli"
+Requires-Dist: orjson; extra == "cli"
+Requires-Dist: pydantic; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
```

### Comparing `shuttleai-3.8.1/README.md` & `shuttleai-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.1/setup.py` & `shuttleai-3.8.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 from src.shuttleai import __version__ as version
 
+def read_requirements(file_path, extras=()):
+    requirements = []
+    with open(file_path, 'r') as file:
+        for line in file:
+            line = line.strip()
+            if line and not line.startswith('#'):
+                extras_require = [extra.strip() for extra in line.split(';')[1:]]
+                if not extras_require or any(extra in extras for extra in extras_require):
+                    requirements.append(line.split(';')[0])
+    return requirements
+
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='shuttleai', 
     version=version,
     author='shuttle',
@@ -18,17 +29,17 @@
     package_dir={"": "src"},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    install_requires=['httpx', 'aiohttp', 'orjson'],
+    install_requires=read_requirements('requirements.txt'),
     extras_require={
-        'cli': ['asyncclick', 'pystyle']
+        'cli': read_requirements('requirements.txt', extras=('cli',))
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
         'console_scripts': [
             'shuttleai = shuttleai.cli:main [cli]'
         ],
```

### Comparing `shuttleai-3.8.1/src/shuttleai/__init__.py` & `shuttleai-3.8.2/src/shuttleai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.1"
+__version__ = "3.8.2"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.1/src/shuttleai/cli.py` & `shuttleai-3.8.2/src/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.1/src/shuttleai/client/_async.py` & `shuttleai-3.8.2/src/shuttleai/client/_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @Author: ShuttleAI
-@Version: 3.8.1
-@Date: 4-3-2024
+@Version: 3.8.2
+@Date: 4-5-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
     Union,
@@ -53,20 +53,20 @@
     """
     _session: Optional[aiohttp.ClientSession] = None
 
     def __init__(
             self,
             api_key: Optional[str] = None,
             base_url: Optional[str] = None,
-            timeout: Union[float, aiohttp.ClientTimeout, None] = 60.0,
+            timeout: Union[float, aiohttp.ClientTimeout, int, None] = 60.0,
             session: Optional[aiohttp.ClientSession] = None,
             silent: bool = True
     ):
         """
-        Initialize the ShuttleAsyncClient client.
+        Initialize the ShuttleAsyncClient.
 
         Args:
             api_key (Optional[str], optional): The API key. Defaults to SHUTTLEAI_API_KEY environment variable.
             base_url (Optional[str], optional): The base URL for the API. Defaults to https://api.shuttleai.app/v1.
             timeout (Union[float, aiohttp.ClientTimeout, None], optional): The timeout for the aiohttp.ClientSession. Defaults to 60.0.
             session (Optional[aiohttp.ClientSession], optional): An existing aiohttp.ClientSession. Defaults to None.
             silent (bool, optional): Whether to silent debugging messages. Defaults to True.
@@ -180,15 +180,18 @@
                         except:
                             pass
             return streamer()
         else:
             async with self._session.request(
                 method, url, json=data, headers=headers, params=args, data=files
             ) as response:
-                return await response.json()
+                try:
+                    return await response.json()
+                except:
+                    return await response.text()
             
     async def get_models(
         self,
         free: bool = False,
         premium: bool = False,
         endpoint: str = "all"
     ) -> Models:
```

### Comparing `shuttleai-3.8.1/src/shuttleai/client/_sync.py` & `shuttleai-3.8.2/src/shuttleai/client/_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @Author: ShuttleAI
-@Version: 3.8.1
-@Date: 4-3-2024
+@Version: 3.8.2
+@Date: 4-5-2024
 """
 from typing import Any, Dict, List, Union, TYPE_CHECKING
 
 import httpx
 from ..log import log
 from ..schemas import Chat, Image, Audio, Embedding, Models
```

### Comparing `shuttleai-3.8.1/src/shuttleai/log.py` & `shuttleai-3.8.2/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.1/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8.2/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.1/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.2/src/shuttleai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.1
+Version: 3.8.2
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: orjson
+Requires-Dist: pydantic
 Provides-Extra: cli
-Requires-Dist: asyncclick; extra == "cli"
-Requires-Dist: pystyle; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
+Requires-Dist: aiohttp; extra == "cli"
+Requires-Dist: orjson; extra == "cli"
+Requires-Dist: pydantic; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
```

