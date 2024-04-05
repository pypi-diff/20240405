# Comparing `tmp/arclet-alconna-tools-0.7.1.tar.gz` & `tmp/arclet_alconna_tools-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.7.1.tar", last modified: Fri Mar 15 14:40:10 2024, max compression
+gzip compressed data, was "arclet_alconna_tools-0.7.2.tar", last modified: Fri Apr  5 06:52:39 2024, max compression
```

## Comparing `arclet-alconna-tools-0.7.1.tar` & `arclet_alconna_tools-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet-alconna-tools-0.7.1/LICENSE
--rw-r--r--   0        0        0     1041 2024-03-15 14:39:52.748155 arclet-alconna-tools-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet-alconna-tools-0.7.1/README.md
--rw-r--r--   0        0        0      991 2024-02-28 05:17:30.448506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2024-02-28 05:17:30.448506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     4679 2024-03-15 13:46:57.328430 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2024-02-28 05:17:30.449506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      822 2024-02-28 05:17:30.449506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      783 2024-02-28 05:17:30.449506 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4394 2024-02-28 05:33:46.955180 arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.2/LICENSE
+-rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.2/README.md
+-rw-r--r--   0        0        0     1032 2024-04-05 06:52:39.249832 arclet_alconna_tools-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      991 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     4703 2024-04-05 06:49:19.105061 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      822 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      783 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4394 2024-02-28 05:33:46.955180 arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 arclet_alconna_tools-0.7.2/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.7.1/LICENSE` & `arclet_alconna_tools-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/pyproject.toml` & `arclet_alconna_tools-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.7.1"
+version = "0.7.2"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nepattern<1.0.0,>=0.6.5",
-    "arclet-alconna>=1.8.6",
+    "arclet-alconna>=1.8.7",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.build]
 includes = [
     "src/arclet",
 ]
 
 [tool.pdm.dev-dependencies]
```

### Comparing `arclet-alconna-tools-0.7.1/README.md` & `arclet_alconna_tools-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/__init__.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/actions.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/checker.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/construct.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/construct.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/debug.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import traceback
 from collections import namedtuple
 from typing import Any, Literal
 
 from arclet.alconna._internal._analyser import Analyser, default_compiler
 from arclet.alconna._internal._handlers import analyse_args as ala
-from arclet.alconna._internal._handlers import analyse_header as alh
+from arclet.alconna._internal._handlers import HEAD_HANDLES
 from arclet.alconna._internal._handlers import analyse_option as alo
 from arclet.alconna._internal._header import Header
 from arclet.alconna.args import Args
 from arclet.alconna.argv import Argv
 from arclet.alconna.base import Option, Subcommand
 from arclet.alconna.config import Namespace
 from arclet.alconna.typing import DataCollection, CommandMeta
@@ -51,15 +51,15 @@
         argv.enter(kwargs)
         argv.build(["test"] + command)
         argv.next()
         return ala(argv, args)
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
-        return
+        return {}
 
 
 def analyse_header(
     headers: list[str | Any] | list[tuple[Any, str]],
     command_name: str,
     command: DataCollection[str | Any],
     sep: str = " ",
@@ -70,15 +70,15 @@
 ):
     meta = CommandMeta(keep_crlf=False, fuzzy_match=False, raise_exception=raise_exception, context_style=context_style)
     argv = Argv(meta, dev_space, separators=(sep,))
     command_header = Header.generate(command_name, headers, compact=compact)
     try:
         argv.enter(kwargs)
         argv.build(command)
-        return alh(command_header, argv)
+        return HEAD_HANDLES[command_header.flag](command_header, argv)
     except Exception as e:
         if raise_exception:
             traceback.print_exception(AnalyseError, e, e.__traceback__)
         return
 
 
 def analyse_option(
```

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/formatter.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/i18n/en-US.json` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/src/arclet/alconna/tools/pattern.py` & `arclet_alconna_tools-0.7.2/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.7.1/PKG-INFO` & `arclet_alconna_tools-0.7.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: Builtin Tools for Alconna
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
+Requires-Dist: nepattern<1.0.0,>=0.6.5
+Requires-Dist: arclet-alconna>=1.8.7
 Description-Content-Type: text/markdown
 
 # Alconna Tools
 
 Provider various tools for Alconna
 
 Extensions:
@@ -39,8 +41,7 @@
     alc()
 ```
 
 ```shell
 $ python constrcut.py -a -b -c abc
 {"alpha": ..., "beta": {}, "gamma": "abc"}
 ```
-
```

