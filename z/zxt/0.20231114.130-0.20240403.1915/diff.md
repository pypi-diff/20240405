# Comparing `tmp/zxt-0.20231114.130.tar.gz` & `tmp/zxt-0.20240403.1915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zxt-0.20231114.130.tar", last modified: Fri Nov  3 17:36:03 2023, max compression
+gzip compressed data, was "zxt-0.20240403.1915.tar", last modified: Fri Apr  5 06:37:29 2024, max compression
```

## Comparing `zxt-0.20231114.130.tar` & `zxt-0.20240403.1915.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-11-03 17:36:03.051518 zxt-0.20231114.130/
--rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20231114.130/LICENSE
--rw-rw-rw-   0        0        0    42926 2023-11-03 17:36:03.050149 zxt-0.20231114.130/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-04-28 08:58:03.000000 zxt-0.20231114.130/README.md
--rw-rw-rw-   0        0        0      815 2023-11-03 17:32:57.000000 zxt-0.20231114.130/pyproject.toml
--rw-rw-rw-   0        0        0      555 2023-11-03 17:36:03.053705 zxt-0.20231114.130/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20231114.130/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-03 17:36:03.022562 zxt-0.20231114.130/zxt/
--rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20231114.130/zxt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-03 17:36:03.039272 zxt-0.20231114.130/zxt/log/
--rw-rw-rw-   0        0        0     5538 2023-08-11 01:48:48.000000 zxt-0.20231114.130/zxt/log/logging_helper.py
-drwxrwxrwx   0        0        0        0 2023-11-03 17:36:03.047459 zxt-0.20231114.130/zxt/log/ztrfh/
--rw-rw-rw-   0        0        0    24853 2023-08-11 02:22:05.000000 zxt-0.20231114.130/zxt/log/ztrfh/ztrfh3.py
--rw-rw-rw-   0        0        0    21211 2023-08-11 02:22:21.000000 zxt-0.20231114.130/zxt/log/ztrfh/ztrfh3_origin.py
--rw-rw-rw-   0        0        0     4361 2023-11-03 17:19:48.000000 zxt-0.20231114.130/zxt/log_helper.py
--rw-rw-rw-   0        0        0     5234 2023-11-03 17:30:28.000000 zxt-0.20231114.130/zxt/process_pool_executor_zx.py
--rw-rw-rw-   0        0        0     6720 2023-11-03 16:48:10.000000 zxt-0.20231114.130/zxt/pth.py
--rw-rw-rw-   0        0        0    12104 2023-08-11 01:34:54.000000 zxt-0.20231114.130/zxt/redis_helper.py
--rw-rw-rw-   0        0        0    10412 2023-09-03 12:06:06.000000 zxt-0.20231114.130/zxt/sql_helper.py
--rw-rw-rw-   0        0        0     1393 2023-11-03 17:27:32.000000 zxt-0.20231114.130/zxt/utility.py
-drwxrwxrwx   0        0        0        0 2023-11-03 17:36:03.035555 zxt-0.20231114.130/zxt.egg-info/
--rw-rw-rw-   0        0        0    42926 2023-11-03 17:36:02.000000 zxt-0.20231114.130/zxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-11-03 17:36:02.000000 zxt-0.20231114.130/zxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-03 17:36:02.000000 zxt-0.20231114.130/zxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-11-03 17:36:02.000000 zxt-0.20231114.130/zxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-11-03 17:36:02.000000 zxt-0.20231114.130/zxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 06:37:29.584968 zxt-0.20240403.1915/
+-rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20240403.1915/LICENSE
+-rw-rw-rw-   0        0        0    43004 2024-04-05 06:37:29.584968 zxt-0.20240403.1915/PKG-INFO
+-rw-rw-rw-   0        0        0     1236 2024-04-05 06:33:57.000000 zxt-0.20240403.1915/README.md
+-rw-rw-rw-   0        0        0      824 2024-04-03 11:21:38.000000 zxt-0.20240403.1915/pyproject.toml
+-rw-rw-rw-   0        0        0      563 2024-04-05 06:37:29.588422 zxt-0.20240403.1915/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20240403.1915/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:37:29.548982 zxt-0.20240403.1915/zxt/
+-rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20240403.1915/zxt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:37:29.567034 zxt-0.20240403.1915/zxt/log/
+-rw-rw-rw-   0        0        0     5538 2023-08-11 01:48:48.000000 zxt-0.20240403.1915/zxt/log/logging_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:37:29.576966 zxt-0.20240403.1915/zxt/log/ztrfh/
+-rw-rw-rw-   0        0        0    24853 2024-04-03 11:17:24.000000 zxt-0.20240403.1915/zxt/log/ztrfh/ztrfh3.py
+-rw-rw-rw-   0        0        0    21211 2024-04-03 11:16:56.000000 zxt-0.20240403.1915/zxt/log/ztrfh/ztrfh3_origin.py
+-rw-rw-rw-   0        0        0     4361 2023-11-04 09:06:55.000000 zxt-0.20240403.1915/zxt/log_helper.py
+-rw-rw-rw-   0        0        0     1689 2024-04-03 11:13:01.000000 zxt-0.20240403.1915/zxt/process_pool_executor_example.py
+-rw-rw-rw-   0        0        0     8628 2024-04-03 10:08:55.000000 zxt-0.20240403.1915/zxt/process_pool_executor_sim.py
+-rw-rw-rw-   0        0        0     6445 2024-04-03 11:13:57.000000 zxt-0.20240403.1915/zxt/process_pool_executor_zx.py
+-rw-rw-rw-   0        0        0     6720 2023-11-03 16:48:10.000000 zxt-0.20240403.1915/zxt/pth.py
+-rw-rw-rw-   0        0        0    12096 2024-04-03 11:13:45.000000 zxt-0.20240403.1915/zxt/redis_helper.py
+-rw-rw-rw-   0        0        0    10412 2023-09-03 12:06:06.000000 zxt-0.20240403.1915/zxt/sql_helper.py
+-rw-rw-rw-   0        0        0     2513 2024-04-03 11:13:10.000000 zxt-0.20240403.1915/zxt/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:37:29.581973 zxt-0.20240403.1915/zxt.egg-info/
+-rw-rw-rw-   0        0        0    43004 2024-04-05 06:37:29.000000 zxt-0.20240403.1915/zxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-04-05 06:37:29.000000 zxt-0.20240403.1915/zxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 06:37:29.000000 zxt-0.20240403.1915/zxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-05 06:37:29.000000 zxt-0.20240403.1915/zxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-05 06:37:29.000000 zxt-0.20240403.1915/zxt.egg-info/top_level.txt
```

### Comparing `zxt-0.20231114.130/LICENSE` & `zxt-0.20240403.1915/LICENSE`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/PKG-INFO` & `zxt-0.20240403.1915/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20231114.130
+Version: 0.20240403.1915
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -684,49 +684,51 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: peewee
 Requires-Dist: pymysql
 Requires-Dist: redis
+Requires-Dist: numba
 
 # zxtools
 
 #### 介绍
-zx的一个工具集，以Python为主，
+zx的一个工具集，以Python为主，  
+https://pypi.org/project/zxt/
 
 #### 安装教程
 
 1.  python -m pip install .
 2.  python -m pip install zxt
 3.  python -m pip install --upgrade zxt
 
 #### 上传教程
 
-1.  创建 .pypirc 文件
+1.  创建 .pypirc 文件  
     type NUL > %UserProfile%\.pypirc
 
-2.  pypirc 规范
+2.  pypirc 规范  
     https://packaging.python.org/specifications/pypirc/
 
-3.  升级工具
-    python -m pip install --upgrade build
+3.  升级工具  
+    python -m pip install --upgrade build  
     python -m pip install --upgrade twine
 
-4.  Generating distribution archives (生成档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
-    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)
+4.  Generating distribution archives (生成档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
+    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)  
     python -m build
 
-5.  Uploading the distribution archives (上传档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
+5.  Uploading the distribution archives (上传档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
     python -m twine upload --repository zxt dist/*
 
 #### 调试教程
 
-1.  卸载 zxt 包
+1.  卸载 zxt 包  
     python -m pip uninstall zxt
 
-2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:
+2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:  
     python ./pth.py --dflt_opt=C
 
 3.  源码已关联到 python 环境, 可以写代码调用 zxt 包进行调试了
```

### Comparing `zxt-0.20231114.130/README.md` & `zxt-0.20240403.1915/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # zxtools
 
 #### 介绍
-zx的一个工具集，以Python为主，
+zx的一个工具集，以Python为主，  
+https://pypi.org/project/zxt/
 
 #### 安装教程
 
 1.  python -m pip install .
 2.  python -m pip install zxt
 3.  python -m pip install --upgrade zxt
 
 #### 上传教程
 
-1.  创建 .pypirc 文件
+1.  创建 .pypirc 文件  
     type NUL > %UserProfile%\.pypirc
 
-2.  pypirc 规范
+2.  pypirc 规范  
     https://packaging.python.org/specifications/pypirc/
 
-3.  升级工具
-    python -m pip install --upgrade build
+3.  升级工具  
+    python -m pip install --upgrade build  
     python -m pip install --upgrade twine
 
-4.  Generating distribution archives (生成档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
-    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)
+4.  Generating distribution archives (生成档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
+    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)  
     python -m build
 
-5.  Uploading the distribution archives (上传档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
+5.  Uploading the distribution archives (上传档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
     python -m twine upload --repository zxt dist/*
 
 #### 调试教程
 
-1.  卸载 zxt 包
+1.  卸载 zxt 包  
     python -m pip uninstall zxt
 
-2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:
+2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:  
     python ./pth.py --dflt_opt=C
 
 3.  源码已关联到 python 环境, 可以写代码调用 zxt 包进行调试了
```

### Comparing `zxt-0.20231114.130/pyproject.toml` & `zxt-0.20240403.1915/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#creating-pyproject-toml
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "zxt"
-version = "0.20231114.0130"
+version = "0.20240403.1915"
 description = "A handy toolkit"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["tool", "toolkit"]
 # https://pypi.org/pypi?:action=list_classifiers
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: Chinese (Simplified)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
-dependencies = ["peewee", "pymysql", "redis"]
+dependencies = ["peewee", "pymysql", "redis", "numba"]
```

### Comparing `zxt-0.20231114.130/setup.cfg` & `zxt-0.20240403.1915/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 7874 0d0a 7665 7273 696f 6e20   = zxt..version 
-00000020: 3d20 302e 3230 3233 3038 3131 2e31 3833  = 0.20230811.183
-00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
+00000020: 3d20 302e 3230 3234 3034 3033 2e31 3931  = 0.20240403.191
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
 00000040: 2061 2068 616e 6479 2074 6f6f 6c6b 6974   a handy toolkit
 00000050: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000060: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
 00000070: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
 00000080: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
 00000090: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
 000000a0: 6f77 6e0d 0a6c 6963 656e 7365 203d 2047  own..license = G
@@ -25,11 +25,12 @@
 00000180: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 00000190: 6e64 6570 656e 6465 6e74 0d0a 0950 726f  ndependent...Pro
 000001a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000001b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
 000001d0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
 000001e0: 3d20 0d0a 0970 6565 7765 650d 0a09 7079  = ...peewee...py
-000001f0: 6d79 7371 6c0d 0a09 7265 6469 730d 0a0d  mysql...redis...
-00000200: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000210: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000220: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000001f0: 6d79 7371 6c0d 0a09 7265 6469 730d 0a09  mysql...redis...
+00000200: 6e75 6d62 610d 0a0d 0a5b 6567 675f 696e  numba....[egg_in
+00000210: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000220: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000230: 0a0d 0a                                  ...
```

### Comparing `zxt-0.20231114.130/zxt/log/logging_helper.py` & `zxt-0.20240403.1915/zxt/log/logging_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt/log/ztrfh/ztrfh3.py` & `zxt-0.20240403.1915/zxt/log/ztrfh/ztrfh3.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt/log/ztrfh/ztrfh3_origin.py` & `zxt-0.20240403.1915/zxt/log/ztrfh/ztrfh3_origin.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt/log_helper.py` & `zxt-0.20240403.1915/zxt/log_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt/process_pool_executor_zx.py` & `zxt-0.20240403.1915/zxt/process_pool_executor_zx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,50 @@
+# !/usr/bin/env python3
+# coding=utf8
+""""""
 import datetime
 import functools
 import logging
 import multiprocessing
 import multiprocessing.pool
 import time
 from _collections_abc import dict_keys, dict_values, Iterable
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from itertools import product
 from multiprocessing import get_context
 from tqdm import tqdm
 from typing import Dict, List, Set, Tuple, Optional, Union, Callable, Type
 
 
+# 为什么python中的Pool不可嵌套调用？
+# https://www.zhihu.com/question/300315099
+# Python multiprocessing: is it possible to have a pool inside of a pool?
+# https://stackoverflow.com/questions/17223301/python-multiprocessing-is-it-possible-to-have-a-pool-inside-of-a-pool/17229030
+# Python进程池不是守护进程？
+# https://cloud.tencent.com/developer/ask/sof/186084
+
+
 class ProcessPoolExecutorZx(object):
     """"""
+    '''
+    可能如下报错:
+    Process ForkPoolWorker-54:
+    Traceback (most recent call last):
+    File "/usr/lib/python3.10/multiprocessing/pool.py", line 131, in worker
+        put((job, i, result))
+    File "/usr/lib/python3.10/multiprocessing/queues.py", line 377, in put
+        self._writer.send_bytes(obj)
+    File "/usr/lib/python3.10/multiprocessing/connection.py", line 200, in send_bytes
+        self._send_bytes(m[offset:offset + size])
+    File "/usr/lib/python3.10/multiprocessing/connection.py", line 411, in _send_bytes
+        self._send(header + buf)
+    File "/usr/lib/python3.10/multiprocessing/connection.py", line 368, in _send
+        n = write(self._handle, buf)
+    BrokenPipeError: [Errno 32] Broken pipe
+    '''
 
     @classmethod
     def as_completed(cls, fs, timeout=None):
         """"""
         fs = set(fs)
 
         while fs:
@@ -40,15 +67,15 @@
 
         def __init__(self, apply_result: multiprocessing.pool.ApplyResult) -> None:
             """"""
             self._apply_result: multiprocessing.pool.ApplyResult = apply_result
 
         def result(self):
             """"""
-            self._apply_result.get()
+            return self._apply_result.get()
 
     class _Item(object):
         """"""
 
         def __init__(self, fn, args, kwargs, rslt, exc):
             """"""
             self.fn = fn
```

### Comparing `zxt-0.20231114.130/zxt/pth.py` & `zxt-0.20240403.1915/zxt/pth.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt/redis_helper.py` & `zxt-0.20240403.1915/zxt/redis_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def GET(cls, redis_object: redis.Redis, name) -> Optional[str]:
         """
         def get(self, name: KeyT) -> ResponseT:
         For more information see https://redis.io/commands/get
         代码文件: Python/Python310/site-packages/redis/commands/core.py
         key 存在, 返回 str
         key 不存在, 返回 None
-        key 的 value 不是 string, 抛异常 redis.exceptions.ResponseError        
+        key 的 value 不是 string, 抛异常 redis.exceptions.ResponseError
         """
         dst = redis_object.get(name)
         dst = dst.decode(encoding='utf8') if isinstance(dst, bytes) else dst
         return dst
 
     @classmethod
     def SET(cls, redis_object: redis.Redis, name, value, ex=None):
```

### Comparing `zxt-0.20231114.130/zxt/sql_helper.py` & `zxt-0.20240403.1915/zxt/sql_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20231114.130/zxt.egg-info/PKG-INFO` & `zxt-0.20240403.1915/zxt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20231114.130
+Version: 0.20240403.1915
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -684,49 +684,51 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: peewee
 Requires-Dist: pymysql
 Requires-Dist: redis
+Requires-Dist: numba
 
 # zxtools
 
 #### 介绍
-zx的一个工具集，以Python为主，
+zx的一个工具集，以Python为主，  
+https://pypi.org/project/zxt/
 
 #### 安装教程
 
 1.  python -m pip install .
 2.  python -m pip install zxt
 3.  python -m pip install --upgrade zxt
 
 #### 上传教程
 
-1.  创建 .pypirc 文件
+1.  创建 .pypirc 文件  
     type NUL > %UserProfile%\.pypirc
 
-2.  pypirc 规范
+2.  pypirc 规范  
     https://packaging.python.org/specifications/pypirc/
 
-3.  升级工具
-    python -m pip install --upgrade build
+3.  升级工具  
+    python -m pip install --upgrade build  
     python -m pip install --upgrade twine
 
-4.  Generating distribution archives (生成档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
-    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)
+4.  Generating distribution archives (生成档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
+    切换到 pyproject.toml 的同级目录, 一般先删除 dist 目录(RMDIR /S .\dist\ /Q)  
     python -m build
 
-5.  Uploading the distribution archives (上传档案)
-    https://packaging.python.org/en/latest/tutorials/packaging-projects/
+5.  Uploading the distribution archives (上传档案)  
+    https://packaging.python.org/en/latest/tutorials/packaging-projects/  
     python -m twine upload --repository zxt dist/*
 
 #### 调试教程
 
-1.  卸载 zxt 包
+1.  卸载 zxt 包  
     python -m pip uninstall zxt
 
-2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:
+2.  从 zxt 的源码中找到 pth.py 所在目录, 在该目录下执行如下命令:  
     python ./pth.py --dflt_opt=C
 
 3.  源码已关联到 python 环境, 可以写代码调用 zxt 包进行调试了
```

