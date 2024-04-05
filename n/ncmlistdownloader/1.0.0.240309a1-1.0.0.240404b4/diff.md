# Comparing `tmp/ncmlistdownloader-1.0.0.240309a1.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240404b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240309a1.tar", last modified: Sat Mar  9 08:15:04 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240404b4.tar", last modified: Fri Apr  5 14:33:52 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240309a1.tar` & `ncmlistdownloader-1.0.0.240404b4.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 08:15:04.973722 ncmlistdownloader-1.0.0.240309a1/
--rw-rw-rw-   0        0        0    35181 2024-02-12 02:33:29.000000 ncmlistdownloader-1.0.0.240309a1/LICENSE
--rw-rw-rw-   0        0        0       18 2024-02-15 05:12:55.000000 ncmlistdownloader-1.0.0.240309a1/MANIFEST.in
--rw-rw-rw-   0        0        0     1452 2024-03-09 08:15:04.968718 ncmlistdownloader-1.0.0.240309a1/PKG-INFO
--rw-rw-rw-   0        0        0     2589 2024-03-09 08:14:35.000000 ncmlistdownloader-1.0.0.240309a1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 08:15:04.913717 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0    16412 2024-03-09 08:14:35.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/__init__.py
--rw-rw-rw-   0        0        0      923 2024-03-09 08:14:35.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/cmd_script.py
--rw-rw-rw-   0        0        0     2085 2024-02-24 05:07:31.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/encode_sec_key.py
--rw-rw-rw-   0        0        0     1982 2024-03-03 02:12:14.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/global_args.py
-drwxrwxrwx   0        0        0        0 2024-03-09 08:15:04.962717 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1452 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-09 08:15:04.000000 ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 08:15:04.974717 ncmlistdownloader-1.0.0.240309a1/setup.cfg
--rw-rw-rw-   0        0        0     1703 2024-03-09 08:14:35.000000 ncmlistdownloader-1.0.0.240309a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.152742 ncmlistdownloader-1.0.0.240404b4/
+-rw-rw-rw-   0        0        0    35181 2024-02-12 02:33:29.000000 ncmlistdownloader-1.0.0.240404b4/LICENSE
+-rw-rw-rw-   0        0        0       18 2024-02-15 05:12:55.000000 ncmlistdownloader-1.0.0.240404b4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2024-04-05 14:33:52.149741 ncmlistdownloader-1.0.0.240404b4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.083742 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1303 2024-04-05 14:31:49.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.126744 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2860 2024-04-05 14:16:11.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-04-05 14:06:36.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     1785 2024-04-04 13:09:20.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-04 13:40:40.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.129741 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-05 14:32:02.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.133744 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-04 14:16:10.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.136742 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     1660 2024-04-05 14:22:39.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.141744 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     6018 2024-04-05 14:31:02.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:33:52.146743 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1398 2024-04-05 14:33:51.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-04-05 14:33:52.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:33:51.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-05 14:33:51.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-05 14:33:51.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-05 14:33:51.000000 ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:33:52.152742 ncmlistdownloader-1.0.0.240404b4/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2024-04-05 14:33:15.000000 ncmlistdownloader-1.0.0.240404b4/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240309a1/LICENSE` & `ncmlistdownloader-1.0.0.240404b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240309a1/PKG-INFO` & `ncmlistdownloader-1.0.0.240404b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240309a1
+Version: 1.0.0.240404b4
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
-Home-page: https://github.com/Cooooldwind/163ListDownloader_NexT
+Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
@@ -20,13 +20,12 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
```

### Comparing `ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader/common/encode_sec_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 '''
 网易云WeAPI解码
-Core.Ver.1.0.0.231218a
+Core.Ver.1.0.0.240404b4-2
 Author: CooooldWind_, 半岛的孤城
 References: 
 1. 网易云解参数（获取网易云歌词，获取评论同理）[https://www.bilibili.com/read/cv12754897/]
 '''
 
 import random
 import json
 from base64 import b64encode
 import requests
 from Crypto.Cipher import AES
-from .global_args import USER_AGENTS, FUNC_F, SEC_KEY
+from ncmlistdownloader.common.global_args import USER_AGENTS, FUNC_F, SEC_KEY
 
 class NeteaseParams:
-    '''WeAPI解码类'''
+    '''
+    WeAPI解码类
+    ----------
+    参数：
+    1. `encode_data`: 传入的参数
+    2. `url`: API的URL
+    '''
     def __init__(self, encode_data, url):
         self.encode_data = encode_data
         self.url = url
         self.func_e = "010001"
         self.func_f = FUNC_F
         self.func_g = "0CoJUm6Qyw8W8jud"
         self.func_i = "vlgPRPyGhwA6F4Sq"
@@ -48,11 +54,12 @@
         get_data = {
             'params': self.get_params(json.dumps(self.encode_data)),
             'encSecKey': self.encode_sec_key
         }
         get_headers = {
             'User-Agent': random.choice(USER_AGENTS)
         }
-        return requests.post(self.url,
+        response = requests.post(self.url,
                              data = get_data,
                              headers = get_headers,
-                             timeout = 10).json()
+                             timeout = 10)
+        return response.json()
```

### Comparing `ncmlistdownloader-1.0.0.240309a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240404b4/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240309a1
+Version: 1.0.0.240404b4
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
-Home-page: https://github.com/Cooooldwind/163ListDownloader_NexT
+Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
@@ -20,13 +20,12 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
```

### Comparing `ncmlistdownloader-1.0.0.240309a1/setup.py` & `ncmlistdownloader-1.0.0.240404b4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -22,18 +22,17 @@
 		'Programming Language :: Python :: 3.6',
 		'Programming Language :: Python :: 3.7',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
-		'Programming Language :: Python :: 3.13',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240309a1",
+    version = "1.0.0.240404b4",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
-    url = 'https://github.com/Cooooldwind/163ListDownloader_NexT',
+    url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
-    entry_points = {'console_scripts': ['163ListDownloader = ncmlistdownloader.cmd_script:main']},
+    entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

