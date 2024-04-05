# Comparing `tmp/liulianmao-1.0.0.tar.gz` & `tmp/liulianmao-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-1.0.0.tar", max compression
+gzip compressed data, was "liulianmao-1.1.0.tar", max compression
```

## Comparing `liulianmao-1.0.0.tar` & `liulianmao-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.0.0/LICENSE
--rw-r--r--   0        0        0      781 2024-04-01 15:26:59.075866 liulianmao-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3008 2024-04-01 15:24:25.334858 liulianmao-1.0.0/README.md
--rw-r--r--   0        0        0      408 2024-04-01 15:14:12.426716 liulianmao-1.0.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0     4821 2024-04-01 12:25:19.703374 liulianmao-1.0.0/src/liulianmao/client_core.py
--rw-r--r--   0        0        0      294 2024-03-20 13:24:32.987009 liulianmao-1.0.0/src/liulianmao/client_langchain.py
--rw-r--r--   0        0        0     1751 2024-04-01 11:46:03.341528 liulianmao-1.0.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.0.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 11:46:03.346082 liulianmao-1.0.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0      542 2024-03-20 13:24:32.988008 liulianmao-1.0.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1359 2024-04-01 11:46:03.350081 liulianmao-1.0.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 liulianmao-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.1.0/LICENSE
+-rw-r--r--   0        0        0      781 2024-04-05 06:13:28.357557 liulianmao-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3346 2024-04-04 10:15:27.974883 liulianmao-1.1.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.1.0/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-05 06:11:53.754203 liulianmao-1.1.0/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.1.0/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0     5032 2024-04-03 13:07:44.762569 liulianmao-1.1.0/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      583 2024-04-03 13:08:46.866069 liulianmao-1.1.0/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      117 2024-04-01 16:47:06.824622 liulianmao-1.1.0/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0     1751 2024-04-02 06:21:17.164107 liulianmao-1.1.0/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.1.0/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.1.0/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0      542 2024-03-20 13:24:32.988008 liulianmao-1.1.0/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1359 2024-04-01 11:46:03.350081 liulianmao-1.1.0/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.1.0/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.1.0/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 liulianmao-1.1.0/PKG-INFO
```

### Comparing `liulianmao-1.0.0/LICENSE` & `liulianmao-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-1.0.0/pyproject.toml` & `liulianmao-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "1.0.0"
+version = "1.1.0"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-1.0.0/README.md` & `liulianmao-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,8 +56,16 @@
 
 ~~( 虽然是MIT协议，您可以自由使用，但如果您是在GitHub上搜到的这个项目，建议使用前先与我咨询，因为可能真的不好用。若能帮到您，就算交个朋友啦！**φ(゜▽゜*)♪** )~~
 
 ## 关于命名
 
 Q: 如果是硬凑LLM首字母缩写，为什么不用“溜溜梅”？
 
-A：我怕来告我。
+A: 我怕来告我。
+
+Q: 如果我觉得鼠宝宝是在重新发明轮子，其实有很多这种简易客户端了，怎么办？
+
+A: 好问题，我也觉得。
+
+Q: 有没有类似榴莲猫的项目？
+
+A: 如果您有小米智能音响，可以试试[yihong0618/xiaogpt](https://github.com/yihong0618/xiaogpt)，给小爱同学装上最强大脑。
```

### Comparing `liulianmao-1.0.0/src/liulianmao/client_core.py` & `liulianmao-1.1.0/src/liulianmao/client/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import json
 import os
+import sys
 
 import requests
 
-from .module.authentication import API_KEY, API_URL
-from .module.log import logger
-from .module.model import select_model
-from .module.storage import PROJECT_FOLDER, get_user_folder, init
+current_dir = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(current_dir, ".."))
+
+from module.authentication import API_KEY, API_URL
+from module.log import logger
+from module.model import select_model
+from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 
 def load_conf():
     config_file_path = os.path.join(
         get_user_folder(), PROJECT_FOLDER, "assets", "config.json"
     )
     with open(config_file_path, "r") as file:
@@ -162,10 +166,13 @@
 def talk():
     with open("terminal/question.txt", "r", encoding="utf-8") as file:
         msg = file.read()
     tts(msg)
 
 
 def main():
-    init()
-    chat()
-    # talk()
+    logger.critical("THIS PROGRAM NOT INTENT TO RUN SUBMODULE".upper())
+    exit(0)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `liulianmao-1.0.0/src/liulianmao/module/authentication.py` & `liulianmao-1.1.0/src/liulianmao/module/authentication.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.0.0/src/liulianmao/module/log.py` & `liulianmao-1.1.0/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.0.0/src/liulianmao/module/model.py` & `liulianmao-1.1.0/src/liulianmao/module/model.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.0.0/src/liulianmao/module/storage.py` & `liulianmao-1.1.0/src/liulianmao/module/storage.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.0.0/PKG-INFO` & `liulianmao-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liulianmao
-Version: 1.0.0
+Version: 1.1.0
 Summary: A LLM client for use from the command line or IDE.
 Home-page: https://github.com/LaoshuBaby/liulianmao
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -82,8 +82,16 @@
 
 ~~( 虽然是MIT协议，您可以自由使用，但如果您是在GitHub上搜到的这个项目，建议使用前先与我咨询，因为可能真的不好用。若能帮到您，就算交个朋友啦！**φ(゜▽゜*)♪** )~~
 
 ## 关于命名
 
 Q: 如果是硬凑LLM首字母缩写，为什么不用“溜溜梅”？
 
-A：我怕来告我。
+A: 我怕来告我。
+
+Q: 如果我觉得鼠宝宝是在重新发明轮子，其实有很多这种简易客户端了，怎么办？
+
+A: 好问题，我也觉得。
+
+Q: 有没有类似榴莲猫的项目？
+
+A: 如果您有小米智能音响，可以试试[yihong0618/xiaogpt](https://github.com/yihong0618/xiaogpt)，给小爱同学装上最强大脑。
```

