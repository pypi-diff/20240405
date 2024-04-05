# Comparing `tmp/smawe_tools-0.3.5.tar.gz` & `tmp/smawe_tools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smawe_tools-0.3.5.tar", last modified: Tue Nov 21 11:37:19 2023, max compression
+gzip compressed data, was "smawe_tools-0.3.6.tar", last modified: Fri Apr  5 13:58:53 2024, max compression
```

## Comparing `smawe_tools-0.3.5.tar` & `smawe_tools-0.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.702358 smawe_tools-0.3.5/
--rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     6671 2023-11-21 11:37:19.701355 smawe_tools-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     6094 2023-11-21 11:30:20.000000 smawe_tools-0.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-11-21 11:37:19.702358 smawe_tools-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-11-21 11:30:20.000000 smawe_tools-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.676618 smawe_tools-0.3.5/smawe_tools/
--rw-rw-rw-   0        0        0      194 2023-11-21 11:27:09.000000 smawe_tools-0.3.5/smawe_tools/__init__.py
--rw-rw-rw-   0        0        0       76 2023-11-21 11:30:20.000000 smawe_tools-0.3.5/smawe_tools/__version__.py
--rw-rw-rw-   0        0        0      394 2023-06-18 06:13:54.000000 smawe_tools-0.3.5/smawe_tools/algorithm.py
--rw-rw-rw-   0        0        0     6799 2023-11-06 11:48:04.000000 smawe_tools-0.3.5/smawe_tools/config.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.687616 smawe_tools-0.3.5/smawe_tools/exception/
--rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.5/smawe_tools/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.690335 smawe_tools-0.3.5/smawe_tools/net/
--rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.5/smawe_tools/net/__init__.py
--rw-rw-rw-   0        0        0     2887 2023-11-21 11:30:20.000000 smawe_tools-0.3.5/smawe_tools/net/network_tool.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.693336 smawe_tools-0.3.5/smawe_tools/retrying/
--rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.5/smawe_tools/retrying/__init__.py
--rw-rw-rw-   0        0        0     2657 2023-11-21 11:30:20.000000 smawe_tools-0.3.5/smawe_tools/retrying/retry.py
--rw-rw-rw-   0        0        0      705 2023-11-08 06:55:39.000000 smawe_tools-0.3.5/smawe_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.694336 smawe_tools-0.3.5/smawe_tools/struct/
--rw-rw-rw-   0        0        0      944 2023-11-02 06:42:01.000000 smawe_tools-0.3.5/smawe_tools/struct/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-11-08 00:09:53.000000 smawe_tools-0.3.5/smawe_tools/tool.py
--rw-rw-rw-   0        0        0     1748 2023-11-10 03:37:29.000000 smawe_tools-0.3.5/smawe_tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.700354 smawe_tools-0.3.5/smawe_tools.egg-info/
--rw-rw-rw-   0        0        0     6671 2023-11-21 11:37:19.000000 smawe_tools-0.3.5/smawe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-11-21 11:37:19.000000 smawe_tools-0.3.5/smawe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 11:37:19.000000 smawe_tools-0.3.5/smawe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-11-21 11:37:19.000000 smawe_tools-0.3.5/smawe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-11-21 11:37:19.000000 smawe_tools-0.3.5/smawe_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-21 11:37:19.697337 smawe_tools-0.3.5/tests/
--rw-rw-rw-   0        0        0      725 2023-06-25 09:21:46.000000 smawe_tools-0.3.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.009571 smawe_tools-0.3.6/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     6784 2024-04-05 13:58:53.007571 smawe_tools-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6207 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:58:53.009571 smawe_tools-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-11-21 11:30:20.000000 smawe_tools-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.956571 smawe_tools-0.3.6/smawe_tools/
+-rw-rw-rw-   0        0        0      194 2023-11-21 11:27:09.000000 smawe_tools-0.3.6/smawe_tools/__init__.py
+-rw-rw-rw-   0        0        0       76 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/smawe_tools/__version__.py
+-rw-rw-rw-   0        0        0      394 2023-06-18 06:13:54.000000 smawe_tools-0.3.6/smawe_tools/algorithm.py
+-rw-rw-rw-   0        0        0     6799 2023-11-06 11:48:04.000000 smawe_tools-0.3.6/smawe_tools/config.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.976571 smawe_tools-0.3.6/smawe_tools/exception/
+-rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.6/smawe_tools/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.980571 smawe_tools-0.3.6/smawe_tools/net/
+-rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.6/smawe_tools/net/__init__.py
+-rw-rw-rw-   0        0        0     2887 2023-11-21 11:30:20.000000 smawe_tools-0.3.6/smawe_tools/net/network_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.988572 smawe_tools-0.3.6/smawe_tools/retrying/
+-rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.6/smawe_tools/retrying/__init__.py
+-rw-rw-rw-   0        0        0     3357 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/smawe_tools/retrying/retry.py
+-rw-rw-rw-   0        0        0      705 2023-11-08 06:55:39.000000 smawe_tools-0.3.6/smawe_tools/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.996571 smawe_tools-0.3.6/smawe_tools/struct/
+-rw-rw-rw-   0        0        0      944 2023-11-02 06:42:01.000000 smawe_tools-0.3.6/smawe_tools/struct/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-11-08 00:09:53.000000 smawe_tools-0.3.6/smawe_tools/tool.py
+-rw-rw-rw-   0        0        0     1748 2023-11-10 03:37:29.000000 smawe_tools-0.3.6/smawe_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.006571 smawe_tools-0.3.6/smawe_tools.egg-info/
+-rw-rw-rw-   0        0        0     6784 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.003571 smawe_tools-0.3.6/tests/
+-rw-rw-rw-   0        0        0      725 2023-06-25 09:21:46.000000 smawe_tools-0.3.6/tests/test.py
```

### Comparing `smawe_tools-0.3.5/LICENSE` & `smawe_tools-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/PKG-INFO` & `smawe_tools-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe_tools
-Version: 0.3.5
+Version: 0.3.6
 Summary: small tool
 Home-page: https://github.com/Smawexi/SmaweTools
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,18 +12,28 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: requests
 
-### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
+<<<<<<< HEAD
+### 一个python工具库
 
 ---
 
+### **安装**
+
+```text
+pip install smawe-tools
+```
+---
+
+=======
+>>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章  
@@ -49,21 +59,22 @@
 
 
 - get_pubnet_ip():  
     获取本机的公网ip(也就是上网时所使用的ip)  
     return: str
 
 
-- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_exception=None):  
+- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_on_exception=None):  
+    0.3.6中添加了实例方法, 类方法, 静态方法的支持  
     发生异常进行重试，默认进行1次重试且每次重试前睡眠0-1s的随机时间，超过最大重试次数后还发生异常，则抛出MaxRetryError异常 
     重试期间如果正常返回结果或没发生异常，则不进行重试。
     stop_max_attempt_number: 停止时的最大重试次数，超出次数后还发生异常，则抛出MaxRetryError异常  
     wait_random_min：随机等待的最小时间(单位毫秒)  
     wait_random_max: 随机等待的最大时间(单位毫秒)  
-    retry_exception: 要重试的异常类型，默认为Exception
+    retry_on_exception: 要重试的异常类型，默认为Exception
   
 - modify_encoding():   
     此函数要从smawe_tools.settings模块进行导入, 如: 
     ~~~ python
     from smawe_tools.settings import modify_encoding 
     # 直接调用即可
     modify_encoding()  
@@ -154,15 +165,15 @@
 import logging
 from smawe_tools.utils import ErrorLogger
 
 error_logger = ErrorLogger(
     from_addr="xxxx@qq.com",
     to_addrs=["xyzxxxx@qq.com", "abcdefg@qq.com"],
     subject="python test",
-    password="xxxxxxxxx",
+    password="xxxxxxxxx", #这里是QQ授权码
     handler_level=logging.INFO,
     logger_level=logging.INFO
 )
 
 # 这里已经将日志记录发送到QQ邮箱了
 error_logger.info("test message")
 # 然后你的QQ邮箱会收到这样类似的消息
```

### Comparing `smawe_tools-0.3.5/README.md` & `smawe_tools-0.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
-### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
+<<<<<<< HEAD
+### 一个python工具库
 
 ---
 
+### **安装**
+
+```text
+pip install smawe-tools
+```
+---
+
+=======
+>>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章  
@@ -31,21 +41,22 @@
 
 
 - get_pubnet_ip():  
     获取本机的公网ip(也就是上网时所使用的ip)  
     return: str
 
 
-- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_exception=None):  
+- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_on_exception=None):  
+    0.3.6中添加了实例方法, 类方法, 静态方法的支持  
     发生异常进行重试，默认进行1次重试且每次重试前睡眠0-1s的随机时间，超过最大重试次数后还发生异常，则抛出MaxRetryError异常 
     重试期间如果正常返回结果或没发生异常，则不进行重试。
     stop_max_attempt_number: 停止时的最大重试次数，超出次数后还发生异常，则抛出MaxRetryError异常  
     wait_random_min：随机等待的最小时间(单位毫秒)  
     wait_random_max: 随机等待的最大时间(单位毫秒)  
-    retry_exception: 要重试的异常类型，默认为Exception
+    retry_on_exception: 要重试的异常类型，默认为Exception
   
 - modify_encoding():   
     此函数要从smawe_tools.settings模块进行导入, 如: 
     ~~~ python
     from smawe_tools.settings import modify_encoding 
     # 直接调用即可
     modify_encoding()  
@@ -136,15 +147,15 @@
 import logging
 from smawe_tools.utils import ErrorLogger
 
 error_logger = ErrorLogger(
     from_addr="xxxx@qq.com",
     to_addrs=["xyzxxxx@qq.com", "abcdefg@qq.com"],
     subject="python test",
-    password="xxxxxxxxx",
+    password="xxxxxxxxx", #这里是QQ授权码
     handler_level=logging.INFO,
     logger_level=logging.INFO
 )
 
 # 这里已经将日志记录发送到QQ邮箱了
 error_logger.info("test message")
 # 然后你的QQ邮箱会收到这样类似的消息
```

### Comparing `smawe_tools-0.3.5/setup.py` & `smawe_tools-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/config.py` & `smawe_tools-0.3.6/smawe_tools/config.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/net/network_tool.py` & `smawe_tools-0.3.6/smawe_tools/net/network_tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/retrying/retry.py` & `smawe_tools-0.3.6/smawe_tools/retrying/retry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,83 @@
 import functools
 import time
 import random
 import logging
 import importlib
+import warnings
 _exception = importlib.import_module(".exception", package="smawe_tools")
 
 
 class Retrying(object):
 
     def __init__(
             self,
             func,
             stop_max_attempt_number=None,
             wait_random_min=None,
             wait_random_max=None,
-            retry_exception=None,
+            retry_on_exception=None,
     ):
-        if not callable(func):
+        if not callable(func) and not isinstance(func, (classmethod, staticmethod)):
             raise ValueError("func param error")
         functools.update_wrapper(self, func)
         self._func = func
 
-        self._retry_exception = retry_exception if retry_exception is not None else Exception
+        self._retry_on_exception = retry_on_exception if retry_on_exception is not None else Exception
 
         self._stop_max_attempt_number = stop_max_attempt_number if stop_max_attempt_number else 1
 
         self._wait_random_min = wait_random_min / 1000 if isinstance(wait_random_min, int) else 0
         self._wait_random_max = wait_random_max / 1000 if isinstance(wait_random_max, int) else 1
         if self._wait_random_max <= self._wait_random_min:
             raise ValueError("wait_random_min is greater than or equal to wait_random_max")
 
+    def __get__(self, instance, owner=None):
+        if isinstance(self._func, (staticmethod, classmethod)):
+            self._func = self._func.__get__(instance, owner)
+            return self
+
+        self._func = functools.partial(self._func, instance)
+        return self
+
     def __call__(self, *args, **kwargs):
         current_retry_num = 0
-
         while True:
             if current_retry_num > self._stop_max_attempt_number:
                 raise _exception.MaxRetryError("Exceeded maximum retry count error")
             try:
                 if current_retry_num:
                     logging.info("\033[1;34mThis is currently the {} retry\033[0m".format(current_retry_num))
                     time.sleep(random.uniform(self._wait_random_min, self._wait_random_max))
                 return self._func(*args, **kwargs)
-            except self._retry_exception:
+            except self._retry_on_exception:
                 current_retry_num += 1
 
 
 def retry(
     stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None,
-    retry_exception=None
+    retry_on_exception=None, **kwargs
 ):
     """
-    异常重试装饰器
+    异常重试装饰器, 0.3.6中添加了实例方法, 类方法, 静态方法的支持
     :param stop_max_attempt_number: 最大重试次数(默认为1次)
     :param wait_random_min: 重试间隔的随机等待最小时间(默认为0s), 单位毫秒
     :param wait_random_max: 重试间隔的随机等待最大时间(默认为1s), 单位毫秒
-    :param retry_exception: 要重试的异常类型(默认为Exception)
+    :param retry_on_exception: 要重试的异常类型(默认为Exception)
     :return:
     """
-    kwargs = _merger_setting(
+    if retry_on_exception is None:
+        retry_on_exception = kwargs.get('retry_exception')
+        warnings.warn("retry_exception param was deprecated, please use retry_on_exception param",  category=DeprecationWarning, stacklevel=2)
+
+    _kwargs = _merger_setting(
         stop_max_attempt_number=stop_max_attempt_number, wait_random_min=wait_random_min,
-        wait_random_max=wait_random_max, retry_exception=retry_exception
+        wait_random_max=wait_random_max, retry_on_exception=retry_on_exception
     )
-    return functools.partial(Retrying, **kwargs)
+    return functools.partial(Retrying, **_kwargs)
 
 
 def _merger_setting(**kwargs):
     new_dict = {}
     new_dict.update(kwargs)
     return new_dict
```

### Comparing `smawe_tools-0.3.5/smawe_tools/settings.py` & `smawe_tools-0.3.6/smawe_tools/settings.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/struct/__init__.py` & `smawe_tools-0.3.6/smawe_tools/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/tool.py` & `smawe_tools-0.3.6/smawe_tools/tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools/utils.py` & `smawe_tools-0.3.6/smawe_tools/utils.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/smawe_tools.egg-info/PKG-INFO` & `smawe_tools-0.3.6/smawe_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smawe-tools
-Version: 0.3.5
+Name: smawe_tools
+Version: 0.3.6
 Summary: small tool
 Home-page: https://github.com/Smawexi/SmaweTools
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,18 +12,28 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: requests
 
-### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
+<<<<<<< HEAD
+### 一个python工具库
 
 ---
 
+### **安装**
+
+```text
+pip install smawe-tools
+```
+---
+
+=======
+>>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章  
@@ -49,21 +59,22 @@
 
 
 - get_pubnet_ip():  
     获取本机的公网ip(也就是上网时所使用的ip)  
     return: str
 
 
-- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_exception=None):  
+- retry(stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None, retry_on_exception=None):  
+    0.3.6中添加了实例方法, 类方法, 静态方法的支持  
     发生异常进行重试，默认进行1次重试且每次重试前睡眠0-1s的随机时间，超过最大重试次数后还发生异常，则抛出MaxRetryError异常 
     重试期间如果正常返回结果或没发生异常，则不进行重试。
     stop_max_attempt_number: 停止时的最大重试次数，超出次数后还发生异常，则抛出MaxRetryError异常  
     wait_random_min：随机等待的最小时间(单位毫秒)  
     wait_random_max: 随机等待的最大时间(单位毫秒)  
-    retry_exception: 要重试的异常类型，默认为Exception
+    retry_on_exception: 要重试的异常类型，默认为Exception
   
 - modify_encoding():   
     此函数要从smawe_tools.settings模块进行导入, 如: 
     ~~~ python
     from smawe_tools.settings import modify_encoding 
     # 直接调用即可
     modify_encoding()  
@@ -154,15 +165,15 @@
 import logging
 from smawe_tools.utils import ErrorLogger
 
 error_logger = ErrorLogger(
     from_addr="xxxx@qq.com",
     to_addrs=["xyzxxxx@qq.com", "abcdefg@qq.com"],
     subject="python test",
-    password="xxxxxxxxx",
+    password="xxxxxxxxx", #这里是QQ授权码
     handler_level=logging.INFO,
     logger_level=logging.INFO
 )
 
 # 这里已经将日志记录发送到QQ邮箱了
 error_logger.info("test message")
 # 然后你的QQ邮箱会收到这样类似的消息
```

### Comparing `smawe_tools-0.3.5/smawe_tools.egg-info/SOURCES.txt` & `smawe_tools-0.3.6/smawe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.5/tests/test.py` & `smawe_tools-0.3.6/tests/test.py`

 * *Files identical despite different names*

