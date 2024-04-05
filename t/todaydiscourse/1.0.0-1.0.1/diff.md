# Comparing `tmp/todaydiscourse-1.0.0.tar.gz` & `tmp/todaydiscourse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todaydiscourse-1.0.0.tar", last modified: Sat Mar 30 16:27:39 2024, max compression
+gzip compressed data, was "todaydiscourse-1.0.1.tar", last modified: Fri Apr  5 17:18:14 2024, max compression
```

## Comparing `todaydiscourse-1.0.0.tar` & `todaydiscourse-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:39.490618 todaydiscourse-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-30 16:27:39.490618 todaydiscourse-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 16:27:39.490618 todaydiscourse-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:39.490618 todaydiscourse-1.0.0/todaydiscourse/
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/todaydiscourse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/todaydiscourse/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-30 16:27:35.000000 todaydiscourse-1.0.0/todaydiscourse/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:27:39.490618 todaydiscourse-1.0.0/todaydiscourse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-30 16:27:39.000000 todaydiscourse-1.0.0/todaydiscourse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-30 16:27:39.000000 todaydiscourse-1.0.0/todaydiscourse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:27:39.000000 todaydiscourse-1.0.0/todaydiscourse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 16:27:39.000000 todaydiscourse-1.0.0/todaydiscourse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 16:27:39.000000 todaydiscourse-1.0.0/todaydiscourse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:18:14.243967 todaydiscourse-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-05 17:18:14.239967 todaydiscourse-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:18:14.243967 todaydiscourse-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:18:14.239967 todaydiscourse-1.0.1/todaydiscourse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/todaydiscourse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/todaydiscourse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/todaydiscourse/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 17:18:09.000000 todaydiscourse-1.0.1/todaydiscourse/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:18:14.239967 todaydiscourse-1.0.1/todaydiscourse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-05 17:18:14.000000 todaydiscourse-1.0.1/todaydiscourse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 17:18:14.000000 todaydiscourse-1.0.1/todaydiscourse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:18:14.000000 todaydiscourse-1.0.1/todaydiscourse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 17:18:14.000000 todaydiscourse-1.0.1/todaydiscourse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 17:18:14.000000 todaydiscourse-1.0.1/todaydiscourse.egg-info/top_level.txt
```

### Comparing `todaydiscourse-1.0.0/LICENSE` & `todaydiscourse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `todaydiscourse-1.0.0/PKG-INFO` & `todaydiscourse-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todaydiscourse
-Version: 1.0.0
+Version: 1.0.1
 Summary: 今日所想，对物所评，一语，即可概括。
 Author-email: YeyingXingchen <yeyingxingchen@yeah.net>, NoNameGMM <nonamegmm@qq.com>
 License: MIT License
         
         Copyright (c) 2024 TodayDiscourse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,18 +34,27 @@
 License-File: LICENSE
 
 # 今日话语-TodayDiscourse
 ## 简介
 今日所想，一句话语，即可概括。  
 今日话语是一款基于[CPython](https://www.python.org/)的一言API，可以在被调用时从词库中获取每日一句。
 ## 部署
-请前往[官方文档](https://xinghetechnology.github.io/apis/todaydiscourse/)查看。
+### 从Pip部署（推荐）
+在开始部署前，请确保您已安装[Python](https://www.python.org/)。
+随后，在命令行中执行以下命令：
+```bash
+pip install todaydiscourse
+cd example
+```
+随后，执行下面的命令启动服务器：
+```bash
+todaydiscourse
+```
+此时，您已成功启动在8080端口启动服务器。
 
 ## 调用
-默认访问 localhost:8000 获取今日话语
-您也可以访问settings.json自行修改端口号
-更多高阶用法，请前往[官方文档](https://xinghetechnology.github.io/apis/todaydiscourse/)
+默认访问 localhost:8000 获取今日话语  
+您也可以访问settings.json自行修改端口号  
+更多高阶用法，请前往[官方文档](https://xingchenopensource.github.io/apis/todaydiscourse/)
 
 ## 鸣谢
-感谢[VScode](https://code.visualstudio.com/)提供的免费开发环境。  
-感谢[GitHub](https://github.com)提供的免费代码托管服务。  
-感谢[CPython](https://python.org/)的免费编程语言。
+感谢这些本项目的贡献者，您们都是好样的！
```

### Comparing `todaydiscourse-1.0.0/pyproject.toml` & `todaydiscourse-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "todaydiscourse"
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.12"
 authors = [
   {name = "YeyingXingchen", email = "yeyingxingchen@yeah.net"},
   {name = "NoNameGMM", email = "nonamegmm@qq.com"}
 ]
 description = "今日所想，对物所评，一语，即可概括。"
 readme = "README.md"
```

### Comparing `todaydiscourse-1.0.0/todaydiscourse.egg-info/PKG-INFO` & `todaydiscourse-1.0.1/todaydiscourse.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todaydiscourse
-Version: 1.0.0
+Version: 1.0.1
 Summary: 今日所想，对物所评，一语，即可概括。
 Author-email: YeyingXingchen <yeyingxingchen@yeah.net>, NoNameGMM <nonamegmm@qq.com>
 License: MIT License
         
         Copyright (c) 2024 TodayDiscourse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,18 +34,27 @@
 License-File: LICENSE
 
 # 今日话语-TodayDiscourse
 ## 简介
 今日所想，一句话语，即可概括。  
 今日话语是一款基于[CPython](https://www.python.org/)的一言API，可以在被调用时从词库中获取每日一句。
 ## 部署
-请前往[官方文档](https://xinghetechnology.github.io/apis/todaydiscourse/)查看。
+### 从Pip部署（推荐）
+在开始部署前，请确保您已安装[Python](https://www.python.org/)。
+随后，在命令行中执行以下命令：
+```bash
+pip install todaydiscourse
+cd example
+```
+随后，执行下面的命令启动服务器：
+```bash
+todaydiscourse
+```
+此时，您已成功启动在8080端口启动服务器。
 
 ## 调用
-默认访问 localhost:8000 获取今日话语
-您也可以访问settings.json自行修改端口号
-更多高阶用法，请前往[官方文档](https://xinghetechnology.github.io/apis/todaydiscourse/)
+默认访问 localhost:8000 获取今日话语  
+您也可以访问settings.json自行修改端口号  
+更多高阶用法，请前往[官方文档](https://xingchenopensource.github.io/apis/todaydiscourse/)
 
 ## 鸣谢
-感谢[VScode](https://code.visualstudio.com/)提供的免费开发环境。  
-感谢[GitHub](https://github.com)提供的免费代码托管服务。  
-感谢[CPython](https://python.org/)的免费编程语言。
+感谢这些本项目的贡献者，您们都是好样的！
```

