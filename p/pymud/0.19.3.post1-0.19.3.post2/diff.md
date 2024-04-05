# Comparing `tmp/pymud-0.19.3.post1.tar.gz` & `tmp/pymud-0.19.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymud-0.19.3.post1.tar", last modified: Wed Apr  3 08:33:43 2024, max compression
+gzip compressed data, was "pymud-0.19.3.post2.tar", last modified: Fri Apr  5 05:02:47 2024, max compression
```

## Comparing `pymud-0.19.3.post1.tar` & `pymud-0.19.3.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:33:43.062746 pymud-0.19.3.post1/
--rw-rw-rw-   0        0        0    35823 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/LICENSE.txt
--rw-rw-rw-   0        0        0    67187 2024-04-03 08:33:43.059456 pymud-0.19.3.post1/PKG-INFO
--rw-rw-rw-   0        0        0    24657 2024-04-03 08:31:09.000000 pymud-0.19.3.post1/README.md
--rw-rw-rw-   0        0        0     2075 2024-04-03 08:31:15.000000 pymud-0.19.3.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 08:33:43.062746 pymud-0.19.3.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 08:33:42.872724 pymud-0.19.3.post1/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:33:42.945031 pymud-0.19.3.post1/src/pymud/
--rw-rw-rw-   0        0        0      422 2024-04-03 05:54:50.000000 pymud-0.19.3.post1/src/pymud/__init__.py
--rw-rw-rw-   0        0        0     4636 2024-03-25 06:44:52.000000 pymud-0.19.3.post1/src/pymud/__main__.py
--rw-rw-rw-   0        0        0     5596 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/src/pymud/dialogs.py
--rw-rw-rw-   0        0        0    42400 2024-04-03 08:16:37.000000 pymud-0.19.3.post1/src/pymud/extras.py
--rw-rw-rw-   0        0        0    38063 2024-04-03 07:08:32.000000 pymud-0.19.3.post1/src/pymud/objects.py
--rw-rw-rw-   0        0        0    11496 2024-03-10 00:23:03.000000 pymud-0.19.3.post1/src/pymud/pkuxkx.py
--rw-rw-rw-   0        0        0    49106 2024-04-03 03:07:55.000000 pymud-0.19.3.post1/src/pymud/protocol.py
--rw-rw-rw-   0        0        0    42936 2024-04-03 06:09:53.000000 pymud-0.19.3.post1/src/pymud/pymud.py
--rw-rw-rw-   0        0        0   114021 2024-04-02 10:44:13.000000 pymud-0.19.3.post1/src/pymud/session.py
--rw-rw-rw-   0        0        0     7092 2024-04-03 08:31:32.000000 pymud-0.19.3.post1/src/pymud/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:33:43.045133 pymud-0.19.3.post1/src/pymud.egg-info/
--rw-rw-rw-   0        0        0    67187 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-03 08:33:42.000000 pymud-0.19.3.post1/src/pymud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.190618 pymud-0.19.3.post2/
+-rw-rw-rw-   0        0        0    35823 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/LICENSE.txt
+-rw-rw-rw-   0        0        0    67271 2024-04-05 05:02:47.187091 pymud-0.19.3.post2/PKG-INFO
+-rw-rw-rw-   0        0        0    24743 2024-04-05 05:02:08.000000 pymud-0.19.3.post2/README.md
+-rw-rw-rw-   0        0        0     2075 2024-04-05 05:02:15.000000 pymud-0.19.3.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 05:02:47.190618 pymud-0.19.3.post2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.057567 pymud-0.19.3.post2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.118685 pymud-0.19.3.post2/src/pymud/
+-rw-rw-rw-   0        0        0      422 2024-04-03 05:54:50.000000 pymud-0.19.3.post2/src/pymud/__init__.py
+-rw-rw-rw-   0        0        0     4636 2024-03-25 06:44:52.000000 pymud-0.19.3.post2/src/pymud/__main__.py
+-rw-rw-rw-   0        0        0     5596 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/src/pymud/dialogs.py
+-rw-rw-rw-   0        0        0    42400 2024-04-03 08:16:37.000000 pymud-0.19.3.post2/src/pymud/extras.py
+-rw-rw-rw-   0        0        0    38063 2024-04-03 07:08:32.000000 pymud-0.19.3.post2/src/pymud/objects.py
+-rw-rw-rw-   0        0        0    11496 2024-03-10 00:23:03.000000 pymud-0.19.3.post2/src/pymud/pkuxkx.py
+-rw-rw-rw-   0        0        0    49106 2024-04-03 03:07:55.000000 pymud-0.19.3.post2/src/pymud/protocol.py
+-rw-rw-rw-   0        0        0    42928 2024-04-05 05:00:36.000000 pymud-0.19.3.post2/src/pymud/pymud.py
+-rw-rw-rw-   0        0        0   114021 2024-04-02 10:44:13.000000 pymud-0.19.3.post2/src/pymud/session.py
+-rw-rw-rw-   0        0        0     7092 2024-04-05 05:02:27.000000 pymud-0.19.3.post2/src/pymud/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:02:47.173761 pymud-0.19.3.post2/src/pymud.egg-info/
+-rw-rw-rw-   0        0        0    67271 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 05:02:47.000000 pymud-0.19.3.post2/src/pymud.egg-info/top_level.txt
```

### Comparing `pymud-0.19.3.post1/LICENSE.txt` & `pymud-0.19.3.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/PKG-INFO` & `pymud-0.19.3.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3.post1
+Version: 0.19.3.post2
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -956,7 +956,10 @@
 ### 0.19.3 (2024-03-27)
 + 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
 
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
 + 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
+
+### 0.19.3post2 （2024-04-05）
++ 问题修复: 修复退出程序时的小bug
```

### Comparing `pymud-0.19.3.post1/README.md` & `pymud-0.19.3.post2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -250,8 +250,11 @@
 
 ### 0.19.3 (2024-03-27)
 + 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
 
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
-+ 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
++ 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
+
+### 0.19.3post2 （2024-04-05）
++ 问题修复: 修复退出程序时的小bug
```

### Comparing `pymud-0.19.3.post1/pyproject.toml` & `pymud-0.19.3.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pymud"  # Required
-version = "0.19.3post1"  # Required
+version = "0.19.3post2"  # Required
 description = "a MUD Client written in Python"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["MUD", "multi-user dungeon", "client"]  # Optional
 authors = [
   {name = "newstart@pkuxkx", email = "crapex@crapex.cc" } # Optional
```

### Comparing `pymud-0.19.3.post1/src/pymud/__main__.py` & `pymud-0.19.3.post2/src/pymud/__main__.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/dialogs.py` & `pymud-0.19.3.post2/src/pymud/dialogs.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/extras.py` & `pymud-0.19.3.post2/src/pymud/extras.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/objects.py` & `pymud-0.19.3.post2/src/pymud/objects.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/pkuxkx.py` & `pymud-0.19.3.post2/src/pymud/pkuxkx.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/protocol.py` & `pymud-0.19.3.post2/src/pymud/protocol.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/pymud.py` & `pymud-0.19.3.post2/src/pymud/pymud.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,16 +693,16 @@
                         while ss.connected:
                             await asyncio.sleep(0.1)
 
                         for plugin in self._plugins.values():
                             if isinstance(plugin, Plugin):
                                 plugin.onSessionDestroy(ss)
 
-                    else:
-                        return
+                else:
+                    return
                 
             self.app.exit()
 
         asyncio.ensure_future(coroutine())
 
     def act_about(self):
         "菜单: 关于"
```

### Comparing `pymud-0.19.3.post1/src/pymud/session.py` & `pymud-0.19.3.post2/src/pymud/session.py`

 * *Files identical despite different names*

### Comparing `pymud-0.19.3.post1/src/pymud/settings.py` & `pymud-0.19.3.post2/src/pymud/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     # 下列内容为APP的常量定义，请勿修改
     __appname__   = "PYMUD"
     "APP 名称, 默认PYMUD"
     __appdesc__   = "a MUD client written in Python"
     "APP 简要描述"
     __version__   = "0.19.3"
     "APP 当前版本"
-    __release__   = "2024-04-03"
+    __release__   = "2024-04-05"
     "APP 当前版本发布日期"
     __author__    = "本牛(newstart)@北侠"
     "APP 作者"
     __email__     = "crapex@crapex.cc"
     "APP 作者邮箱"
     __website__     = "https://pymud.readthedocs.org/"
     "帮助文档发布网址"
```

### Comparing `pymud-0.19.3.post1/src/pymud.egg-info/PKG-INFO` & `pymud-0.19.3.post2/src/pymud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymud
-Version: 0.19.3.post1
+Version: 0.19.3.post2
 Summary: a MUD Client written in Python
 Author-email: "newstart@pkuxkx" <crapex@crapex.cc>
 Maintainer-email: "newstart@pkuxkx" <crapex@crapex.cc>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -956,7 +956,10 @@
 ### 0.19.3 (2024-03-27)
 + 问题修复: 一次发送多个命令时，发送顺序可能不正确的情况
 
 ### 0.19.3post1 (2024-04-03)
 + 功能增加: 新增一个exec_async函数，是exec函数的异步形式。可以在其他会话中异步执行一段代码
 + 帮助完善: 帮助文档逻辑完善，已完成整个包的内置文档的编写和修改
 + 注: 由于我没弄太明白 readthedocs.io 网站对于读取github源代码的逻辑，目前只能通过新发布正式版本的形式来使 readthedocs.io 网站的文档中的类参考自动更新。
+
+### 0.19.3post2 （2024-04-05）
++ 问题修复: 修复退出程序时的小bug
```

