# Comparing `tmp/ts-soup-0.0.4.tar.gz` & `tmp/ts-soup-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-49ur6kw4\ts-soup-0.0.4.tar", last modified: Fri Apr  5 12:54:20 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-uk6qaado\ts-soup-0.0.5.tar", last modified: Fri Apr  5 21:23:57 2024, max compression
```

## Comparing `ts-soup-0.0.4.tar` & `ts-soup-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:54:20.439699 ts-soup-0.0.4/
--rw-rw-rw-   0        0        0     1028 2024-04-05 12:54:20.438700 ts-soup-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 12:54:20.439699 ts-soup-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-05 12:54:17.000000 ts-soup-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:54:20.430700 ts-soup-0.0.4/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.4/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1392 2024-04-05 12:53:56.000000 ts-soup-0.0.4/ts_soup/app.py
--rw-rw-rw-   0        0        0    18079 2024-04-05 12:15:49.000000 ts-soup-0.0.4/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:54:20.436702 ts-soup-0.0.4/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.4/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.4/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.4/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:54:20.438700 ts-soup-0.0.4/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-05 12:54:20.000000 ts-soup-0.0.4/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-05 12:54:20.000000 ts-soup-0.0.4/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:54:20.000000 ts-soup-0.0.4/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 12:54:20.000000 ts-soup-0.0.4/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.287247 ts-soup-0.0.5/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 21:23:57.286234 ts-soup-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:23:57.287247 ts-soup-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-05 21:23:54.000000 ts-soup-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.277591 ts-soup-0.0.5/ts_soup/
+-rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.5/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1322 2024-04-05 21:23:28.000000 ts-soup-0.0.5/ts_soup/app.py
+-rw-rw-rw-   0        0        0    18041 2024-04-05 21:23:28.000000 ts-soup-0.0.5/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.284590 ts-soup-0.0.5/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.5/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.5/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.5/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.285594 ts-soup-0.0.5/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.4/PKG-INFO` & `ts-soup-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.4
+Version: 0.0.5
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.4/README.md` & `ts-soup-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.4/setup.py` & `ts-soup-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.4",
+  version="0.0.5",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.0.4/ts_soup/app.py` & `ts-soup-0.0.5/ts_soup/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import datetime
 import importlib
 import os
 import sys
-import types
 
 from dateutil.relativedelta import relativedelta
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--table',default=[],nargs='+')
 parser.add_argument('--time',default=[],nargs='+')
 args = parser.parse_args()
@@ -18,26 +17,26 @@
 
 def run_sync(db_infos:dict, sync_start_from=None, sync_delay:int=1):
     if sync_start_from is None:
         sync_start_from = {'months': 3}
     sync_end = datetime.datetime.now() + relativedelta(days=sync_delay)
     sync_start = (sync_end - relativedelta(**sync_start_from)).strftime('%Y-%m-%d')
     sync_end = sync_end.strftime('%Y-%m-%d')
-    TO_UPDATE_TABLES = __init(args.table, args.time, sync_start, sync_end, db_infos)
+    to_update_tables = __init(args.table, args.time, sync_start, sync_end, db_infos)
     cwd = os.getcwd()
     sys.path.append(os.path.join(cwd,'funcs'))
     modules = []
     for file in os.listdir(os.path.join(cwd,'funcs')):
         modules.append(importlib.import_module(file.split('.')[0]))
-    # funcs = importlib.import_module('boundary_funcs')
-    for table in TO_UPDATE_TABLES:
+    for table in to_update_tables:
         for module in modules:
             if table in dir(module):
-                exec(f"module.{table}()")
-    #检测是否异常
+                getattr(module,table)()
+
+    # 检测是否异常
     from ts_soup.common import EXECUTE_STATE
     if not EXECUTE_STATE:
         raise Exception("同步异常")
 
 
 
 if __name__ == '__main__':
```

### Comparing `ts-soup-0.0.4/ts_soup/common.py` & `ts-soup-0.0.5/ts_soup/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,51 +134,46 @@
     # 4、未指定时间，未指定表格:
     else:
         DATA_UPDATED_STATE = state_table
         return to_update_tables
 
 
 class BaseSource(ABC):
-
-    dbs = USABLE_DBS
-
     def __init__(self, db,index_field,empty_check):
         """
         :param db: 数据库名
         :param index_field: 数据源筛选日期的字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
         self.empty_check = empty_check
         if db:
-            self.db = self.dbs[db]
+            self.db = USABLE_DBS[db]
         else:
-            self.db = self.dbs['sources_default']
+            self.db = USABLE_DBS['sources_default']
         self.index_field = index_field
 
+
     @abstractmethod
     def build_source(self, to_update_date):
         pass
 
 class BaseTarget(ABC):
-
-    dbs = USABLE_DBS
-
     def __init__(self,tb,index_field, db, user_def_pro,drop_axis,drop_na_subset,drop_na_thresh,has_unique_idx,is_seperated):
         self.tb = tb
         self.user_def_pro = user_def_pro
         if user_def_pro is None:
             self.user_def_pro = []
 
         if db:
-            self.db = self.dbs[db]
-            self.db_pym = self.dbs[f'{db}_pym']
+            self.db = USABLE_DBS[db]
+            self.db_pym = USABLE_DBS[f'{db}_pym']
             self.db_str = db
         else:
-            self.db = self.dbs['targets_default']
-            self.db_pym = self.dbs['targets_default_pym']
+            self.db = USABLE_DBS['targets_default']
+            self.db_pym = USABLE_DBS['targets_default_pym']
             self.db_str = 'targets_default'
 
         self.is_seperated = is_seperated
         self.drop_axis = drop_axis
         self.drop_na_subset = drop_na_subset
         self.drop_na_thresh = drop_na_thresh
         self.has_unique_idx = has_unique_idx
```

### Comparing `ts-soup-0.0.4/ts_soup/workers/sources.py` & `ts-soup-0.0.5/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.4/ts_soup/workers/targets.py` & `ts-soup-0.0.5/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.4/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.0.5/ts_soup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.4
+Version: 0.0.5
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

