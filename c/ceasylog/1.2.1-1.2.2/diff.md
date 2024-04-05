# Comparing `tmp/ceasylog-1.2.1.tar.gz` & `tmp/ceasylog-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceasylog-1.2.1.tar", last modified: Thu Apr  4 12:26:29 2024, max compression
+gzip compressed data, was "ceasylog-1.2.2.tar", last modified: Fri Apr  5 06:41:57 2024, max compression
```

## Comparing `ceasylog-1.2.1.tar` & `ceasylog-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.645442 ceasylog-1.2.1/
--rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.2.1/LICENSE
--rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-04 12:26:29.645079 ceasylog-1.2.1/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)     6079 2024-04-04 12:26:11.000000 ceasylog-1.2.1/README.md
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.642202 ceasylog-1.2.1/ceasylog/
--rw-r--r--   0 adminhuang   (501) staff       (20)     7239 2024-04-04 12:22:40.000000 ceasylog-1.2.1/ceasylog/Logger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)    11433 2024-04-04 12:19:51.000000 ceasylog-1.2.1/ceasylog/LoggerConfiger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.2.1/ceasylog/LoggerLevel.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      633 2024-04-04 11:52:17.000000 ceasylog-1.2.1/ceasylog/LoggerNetworkConfiger.py
--rw-r--r--   0 adminhuang   (501) staff       (20)      213 2024-04-04 11:52:17.000000 ceasylog-1.2.1/ceasylog/__init__.py
-drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-04 12:26:29.644731 ceasylog-1.2.1/ceasylog.egg-info/
--rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/PKG-INFO
--rw-r--r--   0 adminhuang   (501) staff       (20)      310 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/SOURCES.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/dependency_links.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)       18 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/requires.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-04-04 12:26:29.000000 ceasylog-1.2.1/ceasylog.egg-info/top_level.txt
--rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-04-04 12:26:29.645510 ceasylog-1.2.1/setup.cfg
--rw-r--r--   0 adminhuang   (501) staff       (20)      371 2024-04-04 05:48:58.000000 ceasylog-1.2.1/setup.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.668830 ceasylog-1.2.2/
+-rw-r--r--   0 adminhuang   (501) staff       (20)    11339 2024-03-24 13:12:02.000000 ceasylog-1.2.2/LICENSE
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-05 06:41:57.668219 ceasylog-1.2.2/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)     6854 2024-04-05 06:39:16.000000 ceasylog-1.2.2/README.md
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.664754 ceasylog-1.2.2/ceasylog/
+-rw-r--r--   0 adminhuang   (501) staff       (20)     8801 2024-04-05 06:24:07.000000 ceasylog-1.2.2/ceasylog/Logger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)    11433 2024-04-04 12:19:51.000000 ceasylog-1.2.2/ceasylog/LoggerConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      737 2024-03-31 05:32:26.000000 ceasylog-1.2.2/ceasylog/LoggerLevel.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      633 2024-04-04 11:52:17.000000 ceasylog-1.2.2/ceasylog/LoggerNetworkConfiger.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      430 2024-04-05 06:40:02.000000 ceasylog-1.2.2/ceasylog/LoggerStatic.py
+-rw-r--r--   0 adminhuang   (501) staff       (20)      257 2024-04-04 14:16:03.000000 ceasylog-1.2.2/ceasylog/__init__.py
+drwxr-xr-x   0 adminhuang   (501) staff       (20)        0 2024-04-05 06:41:57.667645 ceasylog-1.2.2/ceasylog.egg-info/
+-rw-r--r--   0 adminhuang   (501) staff       (20)      254 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/PKG-INFO
+-rw-r--r--   0 adminhuang   (501) staff       (20)      335 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/SOURCES.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        1 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/dependency_links.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       18 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/requires.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)        9 2024-04-05 06:41:57.000000 ceasylog-1.2.2/ceasylog.egg-info/top_level.txt
+-rw-r--r--   0 adminhuang   (501) staff       (20)       38 2024-04-05 06:41:57.668894 ceasylog-1.2.2/setup.cfg
+-rw-r--r--   0 adminhuang   (501) staff       (20)      371 2024-04-04 14:16:03.000000 ceasylog-1.2.2/setup.py
```

### Comparing `ceasylog-1.2.1/LICENSE` & `ceasylog-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ceasylog-1.2.1/README.md` & `ceasylog-1.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 # CEasyLog
 
 一个简单的日志记录工具
 
-更新时间 2024-04-04 
+更新时间 2024-04-05 
 
 ## 介绍
 
 您可以使用CEasyLog来优雅的记录和打印程序运行过程中的日志信息
 
+### 日志的等级
+
+ceasylog把常用的日志情况分成了五大等级
+
+* DEBUG 调试日志
+* INFO 一般日志
+* WARN 警告日志
+* ERROR 错误日志
+* CRITICAL 严重错误日志
+
 ## 安装
 
 ```bash
 pip install ceasylog
 ```
 
 ## 使用方法
@@ -99,14 +109,48 @@
 logger.critical("这是一条严重错误日志")
 ```
 
 ## 更多功能
 
 **注：所有的相关demo都在项目/demo文件夹中**
 
+### 打印异常
+
+您可以用try-except配合ceasylog处理异常
+
+```python
+"""
+打印异常
+"""
+from ceasylog import *
+
+# 创建日志配置器
+loggerCfg = LoggerConfiger()
+
+logger = Logger(loggerCfg)
+
+
+def hahaha():
+    # 手动触发个异常
+    return 1 / 0
+
+
+if __name__ == '__main__':
+    try:
+        # 捕捉异常
+        hahaha()
+    except Exception as e:
+        # 打印异常
+        logger.exception(e, LoggerLevel.ERROR)
+        
+        # 这里的LoggerLevel.ERROR指的是打印出来的异常为什么日志等级
+        # 也可以不传 缺省ERROR
+
+```
+
 ### 配置继承
 
 不同的日志记录器之间的配置可以进行继承
 
 ```python
 """
 配置继承的使用
@@ -188,15 +232,15 @@
 logger.error("错误信息")
 logger.critical("严重错误信息")
 
 ```
 
 其中配置文件路径可以为绝对路径 或者是相对于主脚本运行目录的相对路径
 
-#### 推送至网络服务器
+### 推送信息至网络服务器
 
 ceasylog支持把日志信息推送到您自建的日志服务器上
 
 ```python
 """
 向网络服务器发送日志信息
```

### Comparing `ceasylog-1.2.1/ceasylog/Logger.py` & `ceasylog-1.2.2/ceasylog/Logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import platform
 import random
 import string
 import threading
 import time
+import traceback
 import uuid
 from datetime import datetime
 
 import requests
 from colorama import Fore, Style
 from colorama import init as coloramaInit
 
@@ -181,14 +182,46 @@
     def critical(self, msg: str):
         uid = getUID()
         nowTimePrint, nowTimeRecord, timeStamp = getTime(self.config.printTimeFormat, self.config.recordTimeFormat)
         logPrint(msg, LoggerLevel.CRITICAL, self.config, uid, self.logStyle, nowTimePrint)
         logRecord(msg, LoggerLevel.CRITICAL, self.config, uid, nowTimeRecord)
         logNetworkSender(msg, LoggerLevel.CRITICAL, self.config, uid, timeStamp)
 
+    def exception(self, e: BaseException, level: LoggerLevel = LoggerLevel.ERROR):
+        if not isinstance(e, BaseException):
+            return
+        exceptionBaseInfo = traceback.format_exc(limit=None, chain=True)
+        exceptionBaseInfoList = exceptionBaseInfo.split("\n")
+        exceptionInfo = ""
+        for i in range(len(exceptionBaseInfoList)):
+            i -= 1
+            if i == 0:
+                exceptionInfo = exceptionBaseInfoList[i]
+                continue
+            exceptionInfo = exceptionInfo + "\n" + " " * (len(getTime(self.config.printTimeFormat, self.config.recordTimeFormat)[0]) + 1 + len(getUID()) + 1 + MAX_BLANK + 8) + exceptionBaseInfoList[i]
+        exceptionLoggerCfg = LoggerConfiger()
+        exceptionLoggerCfg.extendBy(self.config)
+        exceptionLoggerCfg.setName(self.config.name)
+        exceptionLoggerCfg.setMaxPrintLevel(level)
+        exceptionLoggerCfg.setMinPrintLevel(level)
+        exceptionLoggerCfg.setMaxRecordLevel(level)
+        exceptionLoggerCfg.setMinRecordLevel(level)
+        exceptionLogger = Logger(exceptionLoggerCfg)
+        if level == LoggerLevel.DEBUG:
+            exceptionLogger.debug(exceptionInfo)
+        elif level == LoggerLevel.INFO:
+            exceptionLogger.info(exceptionInfo)
+        elif level == LoggerLevel.WARN:
+            exceptionLogger.warn(exceptionInfo)
+        elif level == LoggerLevel.ERROR:
+            exceptionLogger.error(exceptionInfo)
+        elif level == LoggerLevel.CRITICAL:
+            exceptionLogger.critical(exceptionInfo)
+
+
     # def d(self, msg):
     #     self.debug(msg)
     #
     # def i(self, msg):
     #     self.info(msg)
     #
     # def w(self, msg):
```

### Comparing `ceasylog-1.2.1/ceasylog/LoggerConfiger.py` & `ceasylog-1.2.2/ceasylog/LoggerConfiger.py`

 * *Files identical despite different names*

### Comparing `ceasylog-1.2.1/ceasylog/LoggerLevel.py` & `ceasylog-1.2.2/ceasylog/LoggerLevel.py`

 * *Files identical despite different names*

### Comparing `ceasylog-1.2.1/ceasylog/LoggerNetworkConfiger.py` & `ceasylog-1.2.2/ceasylog/LoggerNetworkConfiger.py`

 * *Files identical despite different names*

