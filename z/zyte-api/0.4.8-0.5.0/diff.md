# Comparing `tmp/zyte-api-0.4.8.tar.gz` & `tmp/zyte-api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-api-0.4.8.tar", last modified: Thu Nov  2 13:40:47 2023, max compression
+gzip compressed data, was "zyte-api-0.5.0.tar", last modified: Fri Apr  5 12:41:02 2024, max compression
```

## Comparing `zyte-api-0.4.8.tar` & `zyte-api-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 13:40:47.405737 zyte-api-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-11-02 13:40:30.000000 zyte-api-0.4.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-11-02 13:40:30.000000 zyte-api-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-02 13:40:30.000000 zyte-api-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2023-11-02 13:40:47.405737 zyte-api-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-11-02 13:40:30.000000 zyte-api-0.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 13:40:47.405737 zyte-api-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1527 2023-11-02 13:40:30.000000 zyte-api-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 13:40:47.401737 zyte-api-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-11-02 13:40:30.000000 zyte-api-0.4.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-11-02 13:40:30.000000 zyte-api-0.4.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 13:40:47.401737 zyte-api-0.4.8/zyte_api/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 13:40:47.405737 zyte-api-0.4.8/zyte_api/aio/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/aio/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/aio/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-11-02 13:40:30.000000 zyte-api-0.4.8/zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 13:40:47.405737 zyte-api-0.4.8/zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-02 13:40:47.000000 zyte-api-0.4.8/zyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-05 12:40:37.000000 zyte-api-0.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-05 12:40:37.000000 zyte-api-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 12:40:37.000000 zyte-api-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-05 12:41:02.167657 zyte-api-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-05 12:40:37.000000 zyte-api-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 12:40:37.000000 zyte-api-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 12:41:02.167657 zyte-api-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-05 12:40:37.000000 zyte-api-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.163657 zyte-api-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-05 12:40:37.000000 zyte-api-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/aio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-05 12:40:37.000000 zyte-api-0.5.0/zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:41:02.167657 zyte-api-0.5.0/zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 12:41:02.000000 zyte-api-0.5.0/zyte_api.egg-info/top_level.txt
```

### Comparing `zyte-api-0.4.8/CHANGES.rst` & `zyte-api-0.5.0/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 Changes
 =======
 
+0.5.0 (2024-04-05)
+------------------
+
+* Removed Python 3.7 support.
+
+* Added :class:`~zyte_api.ZyteAPI` and :class:`~zyte_api.AsyncZyteAPI` to
+  provide both sync and async Python interfaces with a cleaner API.
+
+* Deprecated ``zyte_api.aio``:
+
+  * Replace ``zyte_api.aio.client.AsyncClient`` with the new
+    :class:`~zyte_api.AsyncZyteAPI` class.
+
+  * Replace ``zyte_api.aio.client.create_session`` with the new
+    :meth:`AsyncZyteAPI.session <zyte_api.AsyncZyteAPI.session>` method.
+
+  * Import ``zyte_api.aio.errors.RequestError``,
+    ``zyte_api.aio.retry.RetryFactory`` and
+    ``zyte_api.aio.retry.zyte_api_retrying`` directly from ``zyte_api`` now.
+
+* When using the command-line interface, you can now use ``--store-errors`` to
+  have error responses be stored alongside successful responses.
+
+* Improved the documentation.
+
 0.4.8 (2023-11-02)
 ------------------
 
 * Include the Zyte API request ID value in a new ``.request_id`` attribute
   in ``zyte_api.aio.errors.RequestError``.
 
 0.4.7 (2023-09-26)
```

### Comparing `zyte-api-0.4.8/LICENSE` & `zyte-api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-api-0.4.8/setup.py` & `zyte-api-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 #!/usr/bin/env python
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 
 def get_version():
     about = {}
     here = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(here, 'zyte_api/__version__.py')) as f:
+    with open(os.path.join(here, "zyte_api/__version__.py")) as f:
         exec(f.read(), about)
-    return about['__version__']
+    return about["__version__"]
 
 
 setup(
-    name='zyte-api',
+    name="zyte-api",
     version=get_version(),
-    description='Python interface to Zyte API',
-    long_description=open('README.rst').read() + "\n\n" + open('CHANGES.rst').read(),
-    long_description_content_type='text/x-rst',
-    author='Zyte Group Ltd',
-    author_email='opensource@zyte.com',
-    url='https://github.com/zytedata/python-zyte-api',
-    packages=find_packages(exclude=['tests', 'examples']),
-    entry_points = {
-        'console_scripts': ['zyte-api=zyte_api.__main__:_main'],
+    description="Python interface to Zyte API",
+    long_description=open("README.rst").read(),
+    long_description_content_type="text/x-rst",
+    author="Zyte Group Ltd",
+    author_email="opensource@zyte.com",
+    url="https://github.com/zytedata/python-zyte-api",
+    packages=find_packages(exclude=["tests", "examples"]),
+    entry_points={
+        "console_scripts": ["zyte-api=zyte_api.__main__:_main"],
     },
     install_requires=[
-        'aiohttp >= 3.8.0',
-        'attrs',
-        'brotli',
-        'runstats',
-        'tenacity',
-        'tqdm',
-        'w3lib >= 2.1.1',
+        "aiohttp >= 3.8.0",
+        "attrs",
+        "brotli",
+        "runstats",
+        "tenacity",
+        "tqdm",
+        "w3lib >= 2.1.1",
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `zyte-api-0.4.8/zyte_api/__main__.py` & `zyte-api-0.5.0/zyte_api/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,229 @@
 """ Basic command-line interface for Zyte API. """
 
 import argparse
-import json
-import sys
 import asyncio
+import json
 import logging
 import random
+import sys
+from warnings import warn
 
 import tqdm
 from tenacity import retry_if_exception
 
-from zyte_api.aio.client import (
-    create_session,
-    AsyncClient,
-)
-from zyte_api.constants import ENV_VARIABLE, API_URL
+from zyte_api._async import AsyncZyteAPI
+from zyte_api._retry import RetryFactory, _is_throttling_error
+from zyte_api._utils import create_session
+from zyte_api.constants import API_URL
 from zyte_api.utils import _guess_intype
-from zyte_api.aio.retry import RetryFactory, _is_throttling_error
 
 
 class DontRetryErrorsFactory(RetryFactory):
     retry_condition = retry_if_exception(_is_throttling_error)
 
 
-logger = logging.getLogger('zyte_api')
+logger = logging.getLogger("zyte_api")
 
 _UNSET = object()
 
 
-async def run(queries, out, *, n_conn, stop_on_errors, api_url,
-              api_key=None, retry_errors=True):
+async def run(
+    queries,
+    out,
+    *,
+    n_conn,
+    stop_on_errors=_UNSET,
+    api_url,
+    api_key=None,
+    retry_errors=True,
+    store_errors=None,
+):
+    if stop_on_errors is not _UNSET:
+        warn(
+            "The stop_on_errors parameter is deprecated.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+    else:
+        stop_on_errors = False
+
+    def write_output(content):
+        json.dump(content, out, ensure_ascii=False)
+        out.write("\n")
+        out.flush()
+        pbar.update()
+
     retrying = None if retry_errors else DontRetryErrorsFactory().build()
-    client = AsyncClient(n_conn=n_conn, api_key=api_key, api_url=api_url,
-                         retrying=retrying)
+    client = AsyncZyteAPI(
+        n_conn=n_conn, api_key=api_key, api_url=api_url, retrying=retrying
+    )
     async with create_session(connection_pool_size=n_conn) as session:
-        result_iter = client.request_parallel_as_completed(
+        result_iter = client.iter(
             queries=queries,
             session=session,
         )
-        pbar = tqdm.tqdm(smoothing=0, leave=True, total=len(queries), miniters=1,
-                         unit="url")
+        pbar = tqdm.tqdm(
+            smoothing=0, leave=True, total=len(queries), miniters=1, unit="url"
+        )
         pbar.set_postfix_str(str(client.agg_stats))
         try:
             for fut in result_iter:
                 try:
                     result = await fut
-                    json.dump(result, out, ensure_ascii=False)
-                    out.write("\n")
-                    out.flush()
-                    pbar.update()
                 except Exception as e:
+                    if store_errors:
+                        write_output(e.parsed.response_body.decode())
+
                     if stop_on_errors:
                         raise
+
                     logger.error(str(e))
+                else:
+                    write_output(result)
                 finally:
                     pbar.set_postfix_str(str(client.agg_stats))
         finally:
             pbar.close()
     logger.info(client.agg_stats.summary())
     logger.info(f"\nAPI error types:\n{client.agg_stats.api_error_types.most_common()}")
     logger.info(f"\nStatus codes:\n{client.agg_stats.status_codes.most_common()}")
     logger.info(f"\nException types:\n{client.agg_stats.exception_types.most_common()}")
 
 
 def read_input(input_fp, intype):
     assert intype in {"txt", "jl", _UNSET}
     lines = input_fp.readlines()
+    if not lines:
+        return []
     if intype is _UNSET:
         intype = _guess_intype(input_fp.name, lines)
     if intype == "txt":
         urls = [u.strip() for u in lines if u.strip()]
         records = [{"url": url, "browserHtml": True} for url in urls]
     else:
-        records = [
-            json.loads(line.strip())
-            for line in lines if line.strip()
-        ]
+        records = [json.loads(line.strip()) for line in lines if line.strip()]
     # Automatically replicating the url in echoData to being able to
     # to match URLs with content in the responses
     for record in records:
         record.setdefault("echoData", record.get("url"))
     return records
 
 
-def _main(program_name='zyte-api'):
-    """ Process urls from input file through Zyte API """
+def _get_argument_parser(program_name="zyte-api"):
     p = argparse.ArgumentParser(
         prog=program_name,
-        description="""
-        Process input URLs from a file using Zyte API.
-        """,
-    )
-    p.add_argument("input",
-                   type=argparse.FileType("r", encoding='utf8'),
-                   help="Input file with urls, url per line by default. The "
-                        "Format can be changed using `--intype` argument.")
-    p.add_argument("--intype", default=_UNSET, choices=["txt", "jl"],
-                   help="Type of the input file. "
-                        "Allowed values are 'txt' (1 URL per line) and 'jl' "
-                        "(JSON Lines file, each object describing the "
-                        "parameters of a request). "
-                        "If not specified, the input type is guessed based on "
-                        "the input file name extension (.jl, .jsonl, .txt) or "
-                        "content, and assumed to be txt if guessing fails.")
-    p.add_argument("--limit", type=int,
-                   help="Max number of URLs to take from the input")
-    p.add_argument("--output", "-o",
-                   default=sys.stdout,
-                   type=argparse.FileType("w", encoding='utf8'),
-                   help=".jsonlines file to store extracted data. "
-                        "By default, results are printed to stdout.")
-    p.add_argument("--n-conn", type=int, default=20,
-                   help="number of connections to the API server "
-                        "(default: %(default)s)")
-    p.add_argument("--api-key",
-                   help="Zyte API key. "
-                        "You can also set %s environment variable instead "
-                        "of using this option." % ENV_VARIABLE)
-    p.add_argument("--api-url",
-                   help="Zyte API endpoint (default: %(default)s)",
-                   default=API_URL)
-    p.add_argument("--loglevel", "-L", default="INFO",
-                   choices=["DEBUG", "INFO", "WARNING", "ERROR"],
-                   help="log level (default: %(default)s)")
-    p.add_argument("--shuffle", help="Shuffle input URLs", action="store_true")
-    p.add_argument("--dont-retry-errors",
-                   help="Don't retry request and network errors",
-                   action="store_true")
-    args = p.parse_args()
-    logging.basicConfig(
-        stream=sys.stderr,
-        level=getattr(logging, args.loglevel)
+        description="Send Zyte API requests.",
+    )
+    p.add_argument(
+        "INPUT",
+        type=argparse.FileType("r", encoding="utf8"),
+        help=(
+            "Path to an input file (see 'Command-line client > Input file' in "
+            "the docs for details)."
+        ),
+    )
+    p.add_argument(
+        "--intype",
+        default=_UNSET,
+        choices=["txt", "jl"],
+        help=(
+            "Type of the input file, either 'txt' (plain text) or 'jl' (JSON "
+            "Lines).\n"
+            "\n"
+            "If not specified, the input type is guessed based on the input "
+            "file extension ('.jl', '.jsonl', or '.txt'), or in its content, "
+            "with 'txt' as fallback."
+        ),
     )
+    p.add_argument("--limit", type=int, help="Maximum number of requests to send.")
+    p.add_argument(
+        "--output",
+        "-o",
+        default=sys.stdout,
+        type=argparse.FileType("w", encoding="utf8"),
+        help=(
+            "Path for the output file. Results are written into the output "
+            "file in JSON Lines format.\n"
+            "\n"
+            "If not specified, results are printed to the standard output."
+        ),
+    )
+    p.add_argument(
+        "--n-conn",
+        type=int,
+        default=20,
+        help=("Number of concurrent connections to use (default: %(default)s)."),
+    )
+    p.add_argument(
+        "--api-key",
+        help="Zyte API key.",
+    )
+    p.add_argument(
+        "--api-url", help="Zyte API endpoint (default: %(default)s).", default=API_URL
+    )
+    p.add_argument(
+        "--loglevel",
+        "-L",
+        default="INFO",
+        choices=["DEBUG", "INFO", "WARNING", "ERROR"],
+        help="Log level (default: %(default)s).",
+    )
+    p.add_argument(
+        "--shuffle",
+        help="Shuffle request order.",
+        action="store_true",
+    )
+    p.add_argument(
+        "--dont-retry-errors",
+        help="Do not retry unsuccessful responses and network errors, only rate-limiting responses.",
+        action="store_true",
+    )
+    p.add_argument(
+        "--store-errors",
+        help=(
+            "Store error responses in the output file.\n"
+            "\n"
+            "If omitted, only successful responses are stored."
+        ),
+        action="store_true",
+    )
+    return p
+
+
+def _main(program_name="zyte-api"):
+    """Process urls from input file through Zyte API"""
+    p = _get_argument_parser(program_name=program_name)
+    args = p.parse_args()
+    logging.basicConfig(stream=sys.stderr, level=getattr(logging, args.loglevel))
+
+    queries = read_input(args.INPUT, args.intype)
+    if not queries:
+        print("No input queries found. Is the input file empty?", file=sys.stderr)
+        sys.exit(-1)
 
-    queries = read_input(args.input, args.intype)
     if args.shuffle:
         random.shuffle(queries)
     if args.limit:
-        queries = queries[:args.limit]
+        queries = queries[: args.limit]
 
-    logger.info(f"Loaded {len(queries)} urls from {args.input.name}; shuffled: {args.shuffle}")
+    logger.info(
+        f"Loaded {len(queries)} urls from {args.INPUT.name}; shuffled: {args.shuffle}"
+    )
     logger.info(f"Running Zyte API (connections: {args.n_conn})")
 
     loop = asyncio.get_event_loop()
-    coro = run(queries,
-               out=args.output,
-               n_conn=args.n_conn,
-               stop_on_errors=False,
-               api_url=args.api_url,
-               api_key=args.api_key,
-               retry_errors=not args.dont_retry_errors)
+    coro = run(
+        queries,
+        out=args.output,
+        n_conn=args.n_conn,
+        api_url=args.api_url,
+        api_key=args.api_key,
+        retry_errors=not args.dont_retry_errors,
+        store_errors=args.store_errors,
+    )
     loop.run_until_complete(coro)
     loop.close()
 
 
-if __name__ == '__main__':
-    _main(program_name='python -m zyte_api')
+if __name__ == "__main__":
+    _main(program_name="python -m zyte_api")
```

### Comparing `zyte-api-0.4.8/zyte_api/aio/client.py` & `zyte-api-0.5.0/zyte_api/_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,132 @@
-"""
-Asyncio client for Zyte API
-"""
-
 import asyncio
 import time
+from asyncio import Future
 from functools import partial
-from typing import Optional, Iterator, List
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional
 
 import aiohttp
-from aiohttp import TCPConnector
 from tenacity import AsyncRetrying
 
-from .errors import RequestError
-from .retry import zyte_api_retrying
-from ..apikey import get_apikey
-from ..constants import API_URL, API_TIMEOUT
-from ..stats import AggStats, ResponseStats
-from ..utils import USER_AGENT, _process_query
-
-
-# 120 seconds is probably too long, but we are concerned about the case with
-# many concurrent requests and some processing logic running in the same reactor,
-# thus, saturating the CPU. This will make timeouts more likely.
-AIO_API_TIMEOUT = aiohttp.ClientTimeout(total=API_TIMEOUT + 120)
-
-
-def create_session(connection_pool_size=100, **kwargs) -> aiohttp.ClientSession:
-    """ Create a session with parameters suited for Zyte API """
-    kwargs.setdefault('timeout', AIO_API_TIMEOUT)
-    if "connector" not in kwargs:
-        kwargs["connector"] = TCPConnector(limit=connection_pool_size,
-                                           force_close=True)
-    return aiohttp.ClientSession(**kwargs)
+from ._errors import RequestError
+from ._retry import zyte_api_retrying
+from ._utils import _AIO_API_TIMEOUT, create_session
+from .apikey import get_apikey
+from .constants import API_URL
+from .stats import AggStats, ResponseStats
+from .utils import USER_AGENT, _process_query
+
+if TYPE_CHECKING:
+    _ResponseFuture = Future[Dict[str, Any]]
+else:
+    _ResponseFuture = Future  # Python 3.8 support
 
 
 def _post_func(session):
-    """ Return a function to send a POST request """
+    """Return a function to send a POST request"""
     if session is None:
-        return partial(aiohttp.request,
-                       method='POST',
-                       timeout=AIO_API_TIMEOUT)
+        return partial(aiohttp.request, method="POST", timeout=_AIO_API_TIMEOUT)
     else:
         return session.post
 
 
-class AsyncClient:
-    def __init__(self, *,
-                 api_key=None,
-                 api_url=API_URL,
-                 n_conn=15,
-                 retrying: Optional[AsyncRetrying] = None,
-                 user_agent: Optional[str] = None,
-                 ):
+class _AsyncSession:
+    def __init__(self, client, **session_kwargs):
+        self._client = client
+        self._session = create_session(client.n_conn, **session_kwargs)
+        self._context = None
+
+    async def __aenter__(self):
+        self._context = await self._session.__aenter__()
+        return self
+
+    async def __aexit__(self, *exc_info):
+        result = await self._context.__aexit__(*exc_info)
+        self._context = None
+        return result
+
+    def _check_context(self):
+        if self._context is None:
+            raise RuntimeError(
+                "Attempt to use session method on a session either not opened "
+                "or already closed."
+            )
+
+    async def get(
+        self,
+        query: dict,
+        *,
+        endpoint: str = "extract",
+        handle_retries=True,
+        retrying: Optional[AsyncRetrying] = None,
+    ):
+        self._check_context()
+        return await self._client.get(
+            query=query,
+            endpoint=endpoint,
+            handle_retries=handle_retries,
+            retrying=retrying,
+            session=self._context,
+        )
+
+    def iter(
+        self,
+        queries: List[dict],
+        *,
+        endpoint: str = "extract",
+        handle_retries=True,
+        retrying: Optional[AsyncRetrying] = None,
+    ) -> Iterator[Future]:
+        self._check_context()
+        return self._client.iter(
+            queries=queries,
+            endpoint=endpoint,
+            session=self._context,
+            handle_retries=handle_retries,
+            retrying=retrying,
+        )
+
+
+class AsyncZyteAPI:
+    """:ref:`Asynchronous Zyte API client <asyncio_api>`.
+
+    Parameters work the same as for :class:`ZyteAPI`.
+    """
+
+    def __init__(
+        self,
+        *,
+        api_key=None,
+        api_url=API_URL,
+        n_conn=15,
+        retrying: Optional[AsyncRetrying] = None,
+        user_agent: Optional[str] = None,
+    ):
         self.api_key = get_apikey(api_key)
         self.api_url = api_url
         self.n_conn = n_conn
         self.agg_stats = AggStats()
         self.retrying = retrying or zyte_api_retrying
         self.user_agent = user_agent or USER_AGENT
+        self._semaphore = asyncio.Semaphore(n_conn)
 
-    async def request_raw(self, query: dict, *,
-                          endpoint: str = 'extract',
-                          session=None,
-                          handle_retries=True,
-                          retrying: Optional[AsyncRetrying] = None,
-                          ):
+    async def get(
+        self,
+        query: dict,
+        *,
+        endpoint: str = "extract",
+        session=None,
+        handle_retries=True,
+        retrying: Optional[AsyncRetrying] = None,
+    ) -> _ResponseFuture:
+        """Asynchronous equivalent to :meth:`ZyteAPI.get`."""
         retrying = retrying or self.retrying
         post = _post_func(session)
         auth = aiohttp.BasicAuth(self.api_key)
-        headers = {
-            'User-Agent': self.user_agent,
-            'Accept-Encoding': 'br'
-        }
+        headers = {"User-Agent": self.user_agent, "Accept-Encoding": "br"}
 
         response_stats = []
         start_global = time.perf_counter()
 
         async def request():
             stats = ResponseStats.create(start_global)
             self.agg_stats.n_attempts += 1
@@ -84,34 +135,35 @@
                 url=self.api_url + endpoint,
                 json=_process_query(query),
                 auth=auth,
                 headers=headers,
             )
 
             try:
-                async with post(**post_kwargs) as resp:
-                    stats.record_connected(resp.status, self.agg_stats)
-                    if resp.status >= 400:
-                        content = await resp.read()
-                        resp.release()
-                        stats.record_read()
-                        stats.record_request_error(content, self.agg_stats)
-
-                        raise RequestError(
-                            request_info=resp.request_info,
-                            history=resp.history,
-                            status=resp.status,
-                            message=resp.reason,
-                            headers=resp.headers,
-                            response_content=content,
-                        )
-
-                    response = await resp.json()
-                    stats.record_read(self.agg_stats)
-                    return response
+                async with self._semaphore:
+                    async with post(**post_kwargs) as resp:
+                        stats.record_connected(resp.status, self.agg_stats)
+                        if resp.status >= 400:
+                            content = await resp.read()
+                            resp.release()
+                            stats.record_read()
+                            stats.record_request_error(content, self.agg_stats)
+
+                            raise RequestError(
+                                request_info=resp.request_info,
+                                history=resp.history,
+                                status=resp.status,
+                                message=resp.reason,
+                                headers=resp.headers,
+                                response_content=content,
+                            )
+
+                        response = await resp.json()
+                        stats.record_read(self.agg_stats)
+                        return response
             except Exception as e:
                 if not isinstance(e, RequestError):
                     self.agg_stats.n_errors += 1
                     stats.record_exception(e, agg_stats=self.agg_stats)
                 raise
             finally:
                 response_stats.append(stats)
@@ -125,31 +177,35 @@
             self.agg_stats.n_success += 1
         except Exception:
             self.agg_stats.n_fatal_errors += 1
             raise
 
         return result
 
-    def request_parallel_as_completed(self,
-                                      queries: List[dict],
-                                      *,
-                                      endpoint: str = 'extract',
-                                      session: Optional[aiohttp.ClientSession] = None,
-                                      ) -> Iterator[asyncio.Future]:
-        """ Send multiple requests to Zyte API in parallel.
-        Return an `asyncio.as_completed` iterator.
-
-        ``queries`` is a list of requests to process (dicts).
-
-        ``session`` is an optional aiohttp.ClientSession object.
-        Set the session TCPConnector limit to a value greater than
-        the number of connections.
+    def iter(
+        self,
+        queries: List[dict],
+        *,
+        endpoint: str = "extract",
+        session: Optional[aiohttp.ClientSession] = None,
+        handle_retries=True,
+        retrying: Optional[AsyncRetrying] = None,
+    ) -> Iterator[_ResponseFuture]:
+        """Asynchronous equivalent to :meth:`ZyteAPI.iter`.
+
+        .. note:: Yielded futures, when awaited, do raise their exceptions,
+                  instead of only returning them.
         """
-        sem = asyncio.Semaphore(self.n_conn)
 
-        async def _request(query):
-            async with sem:
-                return await self.request_raw(query,
-                    endpoint=endpoint,
-                    session=session)
+        def _request(query):
+            return self.get(
+                query,
+                endpoint=endpoint,
+                session=session,
+                handle_retries=handle_retries,
+                retrying=retrying,
+            )
 
         return asyncio.as_completed([_request(query) for query in queries])
+
+    def session(self, **kwargs):
+        return _AsyncSession(client=self, **kwargs)
```

### Comparing `zyte-api-0.4.8/zyte_api/aio/errors.py` & `zyte-api-0.5.0/zyte_api/_errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# -*- coding: utf-8 -*-
 import logging
+from typing import Optional
 
 from aiohttp import ClientResponseError
 
 from zyte_api.errors import ParsedError
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("zyte_api")
 
 
 class RequestError(ClientResponseError):
-    """ Exception which is raised when Request-level error is returned.
-    In contrast with ClientResponseError, it allows to inspect response
-    content.
-    """
+    """Exception raised upon receiving a :ref:`rate-limiting
+    <zyte-api-rate-limit>` or :ref:`unsuccessful
+    <zyte-api-unsuccessful-responses>` response from Zyte API."""
+
     def __init__(self, *args, **kwargs):
-        self.response_content = kwargs.pop("response_content")
-        self.request_id = kwargs.pop("request_id", None)
-        if self.request_id is None:
-            self.request_id = kwargs.get("headers", {}).get("request-id")
+        #: Response body.
+        self.response_content: Optional[bytes] = kwargs.pop("response_content")
+        #: Request ID.
+        self.request_id: Optional[str] = kwargs.get("headers", {}).get("request-id")
         super().__init__(*args, **kwargs)
 
     @property
     def parsed(self):
+        """Response as a :class:`ParsedError` object."""
         return ParsedError.from_body(self.response_content)
 
     def __str__(self):
-        return f"RequestError: {self.status}, message={self.message}, " \
-               f"headers={self.headers}, body={self.response_content}, " \
-               f"request_id={self.request_id}"
+        return (
+            f"RequestError: {self.status}, message={self.message}, "
+            f"headers={self.headers}, body={self.response_content}, "
+            f"request_id={self.request_id}"
+        )
```

### Comparing `zyte-api-0.4.8/zyte_api/aio/retry.py` & `zyte-api-0.5.0/zyte_api/_retry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-# -*- coding: utf-8 -*-
-"""
-Zyte API retrying logic.
-
-TODO: Implement retry logic for temparary errors (520) using the proposed retry-after header.
-"""
 import asyncio
 import logging
 
 from aiohttp import client_exceptions
 from tenacity import (
+    AsyncRetrying,
+    RetryCallState,
+    after_log,
+    before_log,
+    before_sleep_log,
+    retry_base,
+    retry_if_exception,
+    stop_after_attempt,
+    stop_after_delay,
     wait_chain,
     wait_fixed,
-    wait_random_exponential,
     wait_random,
-    stop_after_attempt,
-    stop_after_delay,
-    retry_if_exception,
-    RetryCallState,
-    before_sleep_log,
-    after_log, AsyncRetrying, before_log, retry_base,
+    wait_random_exponential,
 )
 from tenacity.stop import stop_never
 
-from .errors import RequestError
-
+from ._errors import RequestError
 
 logger = logging.getLogger(__name__)
 
 
 _NETWORK_ERRORS = (
     asyncio.TimeoutError,  # could happen while reading the response body
     client_exceptions.ClientResponseError,
@@ -55,70 +51,119 @@
 
 
 def _is_temporary_download_error(exc: BaseException) -> bool:
     return isinstance(exc, RequestError) and exc.status == 520
 
 
 class RetryFactory:
+    """Factory class that builds the :class:`tenacity.AsyncRetrying` object
+    that defines the :ref:`default retry policy <default-retry-policy>`.
+
+    To create a custom retry policy, you can subclass this factory class,
+    modify it as needed, and then call :meth:`build` on your subclass to get
+    the corresponding :class:`tenacity.AsyncRetrying` object.
+
+    For example, to increase the maximum number of attempts for :ref:`temporary
+    download errors <zyte-api-temporary-download-errors>` from 4 (i.e. 3
+    retries) to 10 (i.e. 9 retries):
+
+    .. code-block:: python
+
+        from tenacity import stop_after_attempt
+        from zyte_api import RetryFactory
+
+
+        class CustomRetryFactory(RetryFactory):
+            temporary_download_error_stop = stop_after_attempt(10)
+
+
+        CUSTOM_RETRY_POLICY = CustomRetryFactory().build()
+
+    To retry :ref:`permanent download errors
+    <zyte-api-permanent-download-errors>`, treating them the same as
+    :ref:`temporary download errors <zyte-api-temporary-download-errors>`:
+
+    .. code-block:: python
+
+        from tenacity import RetryCallState, retry_if_exception, stop_after_attempt
+        from zyte_api import RequestError, RetryFactory
+
+
+        def is_permanent_download_error(exc: BaseException) -> bool:
+            return isinstance(exc, RequestError) and exc.status == 521
+
+
+        class CustomRetryFactory(RetryFactory):
+
+            retry_condition = RetryFactory.retry_condition | retry_if_exception(
+                is_permanent_download_error
+            )
+
+            def wait(self, retry_state: RetryCallState) -> float:
+                if is_permanent_download_error(retry_state.outcome.exception()):
+                    return self.temporary_download_error_wait(retry_state=retry_state)
+                return super().wait(retry_state)
+
+            def stop(self, retry_state: RetryCallState) -> bool:
+                if is_permanent_download_error(retry_state.outcome.exception()):
+                    return self.temporary_download_error_stop(retry_state)
+                return super().stop(retry_state)
+
+
+        CUSTOM_RETRY_POLICY = CustomRetryFactory().build()
     """
-    Build custom retry configuration
-    """
+
     retry_condition: retry_base = (
         retry_if_exception(_is_throttling_error)
         | retry_if_exception(_is_network_error)
         | retry_if_exception(_is_temporary_download_error)
     )
     # throttling
     throttling_wait = wait_chain(
         # always wait 20-40s first
         wait_fixed(20) + wait_random(0, 20),
-
         # wait 20-40s again
         wait_fixed(20) + wait_random(0, 20),
-
         # wait from 30 to 630s, with full jitter and exponentially
         # increasing max wait time
-        wait_fixed(30) + wait_random_exponential(multiplier=1, max=600)
+        wait_fixed(30) + wait_random_exponential(multiplier=1, max=600),
     )
 
     # connection errors, other client and server failures
     network_error_wait = (
         # wait from 3s to ~1m
-        wait_random(3, 7) + wait_random_exponential(multiplier=1, max=55)
+        wait_random(3, 7)
+        + wait_random_exponential(multiplier=1, max=55)
     )
     temporary_download_error_wait = network_error_wait
     throttling_stop = stop_never
     network_error_stop = stop_after_delay(15 * 60)
     temporary_download_error_stop = stop_after_attempt(4)
 
     def wait(self, retry_state: RetryCallState) -> float:
         assert retry_state.outcome, "Unexpected empty outcome"
         exc = retry_state.outcome.exception()
         assert exc, "Unexpected empty exception"
         if _is_throttling_error(exc):
             return self.throttling_wait(retry_state=retry_state)
-        elif _is_network_error(exc):
+        if _is_network_error(exc):
             return self.network_error_wait(retry_state=retry_state)
-        elif _is_temporary_download_error(exc):
-            return self.temporary_download_error_wait(retry_state=retry_state)
-        else:
-            raise RuntimeError("Invalid retry state exception: %s" % exc)
+        assert _is_temporary_download_error(exc)  # See retry_condition
+        return self.temporary_download_error_wait(retry_state=retry_state)
 
     def stop(self, retry_state: RetryCallState) -> bool:
         assert retry_state.outcome, "Unexpected empty outcome"
         exc = retry_state.outcome.exception()
         assert exc, "Unexpected empty exception"
         if _is_throttling_error(exc):
             return self.throttling_stop(retry_state)
-        elif _is_network_error(exc):
+        if _is_network_error(exc):
             return self.network_error_stop(retry_state)
-        elif _is_temporary_download_error(exc):
-            return self.temporary_download_error_stop(retry_state)
-        else:
-            raise RuntimeError("Invalid retry state exception: %s" % exc)
+        assert _is_temporary_download_error(exc)  # See retry_condition
+        return self.temporary_download_error_stop(retry_state)
 
     def reraise(self) -> bool:
         return True
 
     def build(self) -> AsyncRetrying:
         return AsyncRetrying(
             wait=self.wait,
```

### Comparing `zyte-api-0.4.8/zyte_api/stats.py` & `zyte-api-0.5.0/zyte_api/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # -*- coding: utf-8 -*-
-from typing import Optional
-from collections import Counter
 import functools
 import time
+from collections import Counter
+from typing import Optional
 
 import attr
 from runstats import Statistics
 
 from zyte_api.errors import ParsedError
 
 
 def zero_on_division_error(meth):
     @functools.wraps(meth)
     def wrapper(*args, **kwargs):
         try:
             return meth(*args, **kwargs)
         except ZeroDivisionError:
             return 0
+
     return wrapper
 
 
 class AggStats:
     def __init__(self):
         self.time_connect_stats = Statistics()
         self.time_total_stats = Statistics()
 
         self.n_success = 0  # number of successful results returned to the user
-        self.n_fatal_errors = 0  # number of errors returned to the user, after all retries
+        self.n_fatal_errors = (
+            0  # number of errors returned to the user, after all retries
+        )
 
-        self.n_attempts = 0  # total amount of requests made to Zyte API, including retries
+        self.n_attempts = (
+            0  # total amount of requests made to Zyte API, including retries
+        )
         self.n_429 = 0  # number of 429 (throttling) responses
         self.n_errors = 0  # number of errors, including errors which were retried
 
         self.status_codes = Counter()
         self.exception_types = Counter()
         self.api_error_types = Counter()
 
@@ -42,33 +47,37 @@
             self.time_total_stats.mean(),
             self.throttle_ratio(),
             self.n_errors - self.n_fatal_errors,
             self.n_fatal_errors,
             self.error_ratio(),
             self.n_success,
             self.n_processed,
-            self.success_ratio()
+            self.success_ratio(),
         )
 
     def summary(self):
         return (
-            "\n" +
-            "Summary\n" +
-            "-------\n" +
-            "Mean connection time:     {:0.2f}\n".format(self.time_connect_stats.mean()) +
-            "Mean response time:       {:0.2f}\n".format(self.time_total_stats.mean()) +
-            "Throttle ratio:           {:0.1%}\n".format(self.throttle_ratio()) +
-            "Attempts:                 {}\n".format(self.n_attempts) +
-            "Errors:                   {:0.1%}, fatal: {}, non fatal: {}\n".format(
+            "\n"
+            + "Summary\n"
+            + "-------\n"
+            + "Mean connection time:     {:0.2f}\n".format(
+                self.time_connect_stats.mean()
+            )
+            + "Mean response time:       {:0.2f}\n".format(self.time_total_stats.mean())
+            + "Throttle ratio:           {:0.1%}\n".format(self.throttle_ratio())
+            + "Attempts:                 {}\n".format(self.n_attempts)
+            + "Errors:                   {:0.1%}, fatal: {}, non fatal: {}\n".format(
                 self.error_ratio(),
                 self.n_fatal_errors,
-                self.n_errors - self.n_fatal_errors) +
-            "Successful URLs:          {} of {}\n".format(
-                self.n_success, self.n_processed) +
-            "Success ratio:            {:0.1%}\n".format(self.success_ratio())
+                self.n_errors - self.n_fatal_errors,
+            )
+            + "Successful URLs:          {} of {}\n".format(
+                self.n_success, self.n_processed
+            )
+            + "Success ratio:            {:0.1%}\n".format(self.success_ratio())
         )
 
     @zero_on_division_error
     def throttle_ratio(self):
         return self.n_429 / self.n_attempts
 
     @zero_on_division_error
@@ -77,15 +86,15 @@
 
     @zero_on_division_error
     def success_ratio(self):
         return self.n_success / self.n_processed
 
     @property
     def n_processed(self):
-        """ Total number of processed URLs """
+        """Total number of processed URLs"""
         return self.n_success + self.n_fatal_errors
 
 
 @attr.s
 class ResponseStats:
     _start = attr.ib(repr=False)  # type: float
```

### Comparing `zyte-api-0.4.8/zyte_api/utils.py` & `zyte-api-0.5.0/zyte_api/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from os.path import splitext
 
 from w3lib.url import safe_url_string
 
 from .__version__ import __version__
 
-USER_AGENT = f'python-zyte-api/{__version__}'
+USER_AGENT = f"python-zyte-api/{__version__}"
 
 
 def _guess_intype(file_name, lines):
     _, dot_extension = splitext(file_name)
     extension = dot_extension[1:]
     if extension in {"jl", "jsonl"}:
         return "jl"
     if extension == "txt":
         return "txt"
 
-    if re.search(r'^\s*\{', lines[0]):
+    if re.search(r"^\s*\{", lines[0]):
         return "jl"
 
     return "txt"
 
 
 def _process_query(query):
     """Given a query to be sent to Zyte API, return a functionally-equivalent
```

### Comparing `zyte-api-0.4.8/zyte_api.egg-info/SOURCES.txt` & `zyte-api-0.5.0/zyte_api.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
+setup.cfg
 setup.py
-tests/test_client.py
+tests/__init__.py
+tests/conftest.py
+tests/mockserver.py
+tests/test_async.py
+tests/test_main.py
+tests/test_retry.py
+tests/test_sync.py
 tests/test_utils.py
 zyte_api/__init__.py
 zyte_api/__main__.py
 zyte_api/__version__.py
+zyte_api/_async.py
+zyte_api/_errors.py
+zyte_api/_retry.py
+zyte_api/_sync.py
+zyte_api/_utils.py
 zyte_api/apikey.py
 zyte_api/constants.py
 zyte_api/errors.py
 zyte_api/stats.py
 zyte_api/utils.py
 zyte_api.egg-info/PKG-INFO
 zyte_api.egg-info/SOURCES.txt
```

