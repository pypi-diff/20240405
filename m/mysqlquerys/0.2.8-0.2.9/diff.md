# Comparing `tmp/mysqlquerys-0.2.8.tar.gz` & `tmp/mysqlquerys-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlquerys-0.2.8.tar", last modified: Mon Nov 20 11:19:55 2023, max compression
+gzip compressed data, was "mysqlquerys-0.2.9.tar", last modified: Mon Dec  4 16:35:44 2023, max compression
```

## Comparing `mysqlquerys-0.2.8.tar` & `mysqlquerys-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.139950 mysqlquerys-0.2.8/
--rw-rw-rw-   0        0        0       93 2023-10-30 09:57:46.000000 mysqlquerys-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      719 2023-11-20 11:19:55.139950 mysqlquerys-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-02-14 09:59:42.000000 mysqlquerys-0.2.8/README.md
--rw-rw-rw-   0        0        0      558 2023-11-19 21:20:07.000000 mysqlquerys-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0      741 2023-11-20 11:19:55.140947 mysqlquerys-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-05-27 06:07:35.000000 mysqlquerys-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.104216 mysqlquerys-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.120848 mysqlquerys-0.2.8/src/mysqlquerys/
--rw-rw-rw-   0        0        0        0 2022-11-14 10:44:12.000000 mysqlquerys-0.2.8/src/mysqlquerys/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-10-30 07:51:53.000000 mysqlquerys-0.2.8/src/mysqlquerys/connect.py
--rw-rw-rw-   0        0        0      786 2023-11-20 09:34:58.000000 mysqlquerys-0.2.8/src/mysqlquerys/control.py
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.126796 mysqlquerys-0.2.8/src/mysqlquerys/gui/
--rw-rw-rw-   0        0        0     4159 2023-10-30 10:46:38.000000 mysqlquerys-0.2.8/src/mysqlquerys/gui/filterWindow.ui
--rw-rw-rw-   0        0        0     1774 2023-10-27 12:27:47.000000 mysqlquerys-0.2.8/src/mysqlquerys/gui/gui.ui
--rw-rw-rw-   0        0        0    11086 2023-11-16 21:22:47.000000 mysqlquerys-0.2.8/src/mysqlquerys/gui/postgresql_gui.ui
--rw-rw-rw-   0        0        0    32810 2023-11-19 21:22:43.000000 mysqlquerys-0.2.8/src/mysqlquerys/gui.py
--rw-rw-rw-   0        0        0    27878 2023-11-20 11:16:58.000000 mysqlquerys-0.2.8/src/mysqlquerys/mysql_rm.py
--rw-rw-rw-   0        0        0        0 2023-10-27 13:11:39.000000 mysqlquerys-0.2.8/src/mysqlquerys/postgresql_rm.py
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.139950 mysqlquerys-0.2.8/src/mysqlquerys/sql/
--rw-rw-rw-   0        0        0     2111 2023-04-21 13:02:01.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/aeroclub.sql
--rw-rw-rw-   0        0        0    11387 2023-09-11 08:29:31.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/alimentari.sql
--rw-rw-rw-   0        0        0     2782 2023-04-21 13:04:02.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/apartament.sql
--rw-rw-rw-   0        0        0     3657 2023-04-21 13:04:07.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/asigurari.sql
--rw-rw-rw-   0        0        0     2078 2023-09-11 10:19:41.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/banca.sql
--rw-rw-rw-   0        0        0     2686 2023-04-21 13:04:11.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/expenses.sql
--rw-rw-rw-   0        0        0     2877 2023-04-21 13:04:16.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/income.sql
--rw-rw-rw-   0        0        0     1932 2023-04-21 13:04:20.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/intercontotrans.sql
--rw-rw-rw-   0        0        0     2107 2023-09-11 08:17:39.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/one_time_transactions.sql
--rw-rw-rw-   0        0        0     2144 2023-04-26 19:11:19.000000 mysqlquerys-0.2.8/src/mysqlquerys/sql/stat.sql
-drwxrwxrwx   0        0        0        0 2023-11-20 11:19:55.126796 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/
--rw-rw-rw-   0        0        0      719 2023-11-20 11:19:55.000000 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-11-20 11:19:55.000000 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 11:19:55.000000 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-11-20 11:19:55.000000 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-11-20 11:19:55.000000 mysqlquerys-0.2.8/src/mysqlquerys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.046624 mysqlquerys-0.2.9/
+-rw-rw-rw-   0        0        0       93 2023-10-30 09:57:46.000000 mysqlquerys-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      719 2023-12-04 16:35:44.046624 mysqlquerys-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2022-02-14 09:59:42.000000 mysqlquerys-0.2.9/README.md
+-rw-rw-rw-   0        0        0      558 2023-11-19 21:20:07.000000 mysqlquerys-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0      741 2023-12-04 16:35:44.046624 mysqlquerys-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-05-27 06:07:35.000000 mysqlquerys-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.014436 mysqlquerys-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.031954 mysqlquerys-0.2.9/src/mysqlquerys/
+-rw-rw-rw-   0        0        0        0 2022-11-14 10:44:12.000000 mysqlquerys-0.2.9/src/mysqlquerys/__init__.py
+-rw-rw-rw-   0        0        0     1605 2023-12-04 13:45:11.000000 mysqlquerys-0.2.9/src/mysqlquerys/connect.py
+-rw-rw-rw-   0        0        0     2690 2023-11-27 12:57:11.000000 mysqlquerys-0.2.9/src/mysqlquerys/control.py
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.044966 mysqlquerys-0.2.9/src/mysqlquerys/gui/
+-rw-rw-rw-   0        0        0     4159 2023-10-30 10:46:38.000000 mysqlquerys-0.2.9/src/mysqlquerys/gui/filterWindow.ui
+-rw-rw-rw-   0        0        0     1774 2023-10-27 12:27:47.000000 mysqlquerys-0.2.9/src/mysqlquerys/gui/gui.ui
+-rw-rw-rw-   0        0        0    11086 2023-11-16 21:22:47.000000 mysqlquerys-0.2.9/src/mysqlquerys/gui/postgresql_gui.ui
+-rw-rw-rw-   0        0        0    32810 2023-11-19 21:22:43.000000 mysqlquerys-0.2.9/src/mysqlquerys/gui.py
+-rw-rw-rw-   0        0        0    27804 2023-12-04 13:43:06.000000 mysqlquerys-0.2.9/src/mysqlquerys/mysql_rm.py
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:11:39.000000 mysqlquerys-0.2.9/src/mysqlquerys/postgresql_rm.py
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.046624 mysqlquerys-0.2.9/src/mysqlquerys/sql/
+-rw-rw-rw-   0        0        0     2111 2023-04-21 13:02:01.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/aeroclub.sql
+-rw-rw-rw-   0        0        0    11387 2023-09-11 08:29:31.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/alimentari.sql
+-rw-rw-rw-   0        0        0     2782 2023-04-21 13:04:02.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/apartament.sql
+-rw-rw-rw-   0        0        0     3657 2023-04-21 13:04:07.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/asigurari.sql
+-rw-rw-rw-   0        0        0     2078 2023-09-11 10:19:41.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/banca.sql
+-rw-rw-rw-   0        0        0     2686 2023-04-21 13:04:11.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/expenses.sql
+-rw-rw-rw-   0        0        0     2877 2023-04-21 13:04:16.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/income.sql
+-rw-rw-rw-   0        0        0     1932 2023-04-21 13:04:20.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/intercontotrans.sql
+-rw-rw-rw-   0        0        0     2107 2023-09-11 08:17:39.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/one_time_transactions.sql
+-rw-rw-rw-   0        0        0     2144 2023-04-26 19:11:19.000000 mysqlquerys-0.2.9/src/mysqlquerys/sql/stat.sql
+drwxrwxrwx   0        0        0        0 2023-12-04 16:35:44.046624 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/
+-rw-rw-rw-   0        0        0      719 2023-12-04 16:35:43.000000 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-12-04 16:35:43.000000 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-04 16:35:43.000000 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-12-04 16:35:43.000000 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-12-04 16:35:43.000000 mysqlquerys-0.2.9/src/mysqlquerys.egg-info/top_level.txt
```

### Comparing `mysqlquerys-0.2.8/PKG-INFO` & `mysqlquerys-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlquerys
-Version: 0.2.8
+Version: 0.2.9
 Summary: Query-uri personale pentru a scrie in MySQL
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysqlquerys-0.2.8/requirements.txt` & `mysqlquerys-0.2.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/setup.cfg` & `mysqlquerys-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7973 716c 7175 6572 7973 0d0a   = mysqlquerys..
-00000020: 7665 7273 696f 6e20 3d20 302e 322e 380d  version = 0.2.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 322e 390d  version = 0.2.9.
 00000030: 0a61 7574 686f 7220 3d20 5261 6475 204d  .author = Radu M
 00000040: 2e0d 0a61 7574 686f 725f 656d 6169 6c20  ...author_email 
 00000050: 3d20 7261 6475 2e6d 6972 6365 6140 7961  = radu.mircea@ya
 00000060: 686f 6f2e 636f 6d0d 0a64 6573 6372 6970  hoo.com..descrip
 00000070: 7469 6f6e 203d 2051 7565 7279 2d75 7269  tion = Query-uri
 00000080: 2070 6572 736f 6e61 6c65 2070 656e 7472   personale pentr
 00000090: 7520 6120 7363 7269 6520 696e 204d 7953  u a scrie in MyS
```

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/connect.py` & `mysqlquerys-0.2.9/src/mysqlquerys/connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from configparser import ConfigParser
 import sys
 
 
 class Config:
     def __init__(self, fileName):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         self.fileName = fileName
         if len(self.sections) == 1:
             self.credentials = 0
 
     @property
     def credentials(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         parser = ConfigParser(empty_lines_in_values=False)
         parser.read(self.fileName)
         sections = parser.sections()
         sect = sections[self.sec_no]
         params = dict(parser.items(sect))
         return params
 
     @credentials.setter
     def credentials(self, sec_no):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         self.sec_no = sec_no
 
     @property
     def sections(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         parser = ConfigParser(empty_lines_in_values=False)
         parser.read(self.fileName)
         sections = parser.sections()
         return sections
 
     @property
     def db_type(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         parser = ConfigParser(empty_lines_in_values=False)
         parser.read(self.fileName)
         sections = parser.sections()
         type = sections[self.sec_no].split('_')[0]
         return type
```

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/gui/filterWindow.ui` & `mysqlquerys-0.2.9/src/mysqlquerys/gui/filterWindow.ui`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/gui/gui.ui` & `mysqlquerys-0.2.9/src/mysqlquerys/gui/gui.ui`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/gui/postgresql_gui.ui` & `mysqlquerys-0.2.9/src/mysqlquerys/gui/postgresql_gui.ui`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/gui.py` & `mysqlquerys-0.2.9/src/mysqlquerys/gui.py`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/mysql_rm.py` & `mysqlquerys-0.2.9/src/mysqlquerys/mysql_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os.path
+
 import mysql.connector as mysql
 import re
 import codecs
 import sys
 import traceback
 import numpy as np
 from mysqlquerys import connect
@@ -11,37 +13,37 @@
     def __init__(self, credentials):
         self.db = mysql.connect(**credentials)
         # self.db.set_session(autocommit=True)
         self.cursor = self.db.cursor()
 
     @property
     def dataBaseVersion(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         self.cursor.execute('SELECT version()')
         db_version = self.cursor.fetchone()
         return db_version
 
     @property
     def allAvailableTablesInDatabase(self):
         """ get all tables in schema"""
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         cur = self.db.cursor()
         command = "SHOW TABLES"
         cur.execute(command)
         rows = cur.fetchall()
         tables = []
         for row in rows:
             tabName = row[0]
             tables.append(tabName)
         cur.close()
 
         return sorted(tables)
 
     def checkProcess(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         query = "SHOW PROCESSLIST"
         cur = self.db.cursor()
         cur.execute(query)
         records = cur.fetchall()
         return records
 
     def killProcess(self, processes):
@@ -50,15 +52,15 @@
             self.cursor.execute(query)
 
     def createTableFromFile(self, file):
         '''
         :param file: QFileDialog.getOpenFileName
         :return:
         '''
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         try:
             error = None
             command = ''
             # print ('createTableFromFile', file)
             f = open(file)
             # f = codecs.open(file, "r", "utf-8")
             for line in f.read().splitlines():
@@ -102,15 +104,15 @@
         return error
 
     def createTableList(self, fileList):
         '''
         :param fileList: QFileDialog.getOpenFileNames
         :return: Error if exists, else None
         '''
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         errList = []
         while fileList:
             for i, file in enumerate(fileList):
                 error = self.createTableFromFile(file)
                 if error:
                     if error[0] == 'Cannot add foreign key constraint' \
                             or re.search("^relation.*does not exist$", error[0]):
@@ -141,22 +143,22 @@
             print('remaining errs:')
             for i in errList:
                 print(i)
         else:
             print('Successfully')
 
     def drop_table(self, tableName):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         query = "DROP TABLE IF EXISTS {} CASCADE;".format(tableName)
         cur = self.db.cursor()
         cur.execute(query)
         cur.close()
 
     def drop_table_list(self, tableList):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         results = []
         while tableList:
             for i, tab in enumerate(tablelist):
                 if self.connectionType == 'mysql':
                     exists = self.checkIfTableExists(tab)
                     if not exists:
                         print('table {} does not exist in database {}'.format(tab, self.dataBaseName))
@@ -187,26 +189,25 @@
                 elif self.connectionType == 'postgresql':
                     res = self.drop_table(tab)
                     results.append(res)
                     tableList.pop(i)
         return results
 
     def rename_table(self, tableName, newName):
-        # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        # #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         query = ('RENAME TABLE {} TO {}'.format(tableName, newName))
         cur = self.db.cursor()
         try:
             cur.execute(query)
             cur.close
         except mysql.connector.Error as err:
             print(err.msg)
 
-
     def deleteAllDataInTable(self, tableList):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         cur = self.db.cursor()
         for tab in tableList:
             query = ('DELETE FROM {}'.format(tab))
             cur.execute(query)
             self.db.commit()
         cur.close()
 
@@ -214,15 +215,15 @@
 class Table(DataBase):
     def __init__(self, credentials, tableName):
         super().__init__(credentials)
         self.tableName = tableName
 
     @property
     def noOfRows(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         query = 'SELECT COUNT(*) FROM {}'.format(self.tableName)
         cursor = self.db.cursor()
         cursor.execute(query)
         noOfRows = cursor.fetchone()[0]
         # rowNo = cursor.rowcount
         cursor.close()
         return noOfRows
@@ -234,15 +235,15 @@
         lastId = cur.fetchonel()
         if lastId is None:
             return 0
         return lastId[0]
 
     @property
     def columnsNames(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         cursor = self.db.cursor()
         query = 'DESC {}'.format(self.tableName)
         cursor.execute(query)
         res = cursor.fetchall()
         cols = []
         for col in res:
             cols.append(col[0])
@@ -263,15 +264,15 @@
                 colType = str(colType.decode("utf-8"))
             cols[colName] = [colType, null, key, default, extra]
         cursor.close()
         return cols
 
     @property
     def columnsProperties(self):
-        print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
         cursor = self.db.cursor()
         query = ("SELECT table_name, column_name, data_type FROM INFORMATION_SCHEMA.COLUMNS WHERE table_name = '{}'").format(self.tableName)
         cursor.execute(query)
         res = cursor.fetchall()
         cols = {}
         for col in res:
             table_name, col_name, data_type = col
@@ -302,14 +303,20 @@
         query = 'DELETE FROM {} WHERE {} = {} '.format(self.tableName, colName, value)
         print(query)
         cursor = self.db.cursor()
         cursor.execute(query, value)
         self.db.commit()
         cursor.close()
 
+    def convertToBinaryData(self, filename):
+        # Convert digital data to binary format
+        with open(filename, 'rb') as file:
+            binaryData = file.read()
+        return binaryData
+
     def addNewRow(self, columns, values):
         # print(len(columns), len(values))
         strCols = (('{}, ' * len(columns)).format(*columns))
         strCols = '({})'.format(strCols[:-2])
         strVals = ('%s,'*len(columns))
         strVals = '({})'.format(strVals[:-1])
 
@@ -319,14 +326,21 @@
         for i in range(len(columns)):
             print(columns[i], values[i])
         #######
         if isinstance(values, int):
             values = (values, )
         elif isinstance(values, str):
             values = (values,)
+        elif isinstance(values, tuple):
+            new_vals = []
+            for v in values:
+                if os.path.isfile(v):
+                    v = self.convertToBinaryData(v)
+                new_vals.append(v)
+            values = tuple(new_vals)
 
         cursor = self.db.cursor()
         cursor.execute(query, values)
         self.db.commit()
         cursor.close()
 
         return cursor.lastrowid
@@ -346,23 +360,23 @@
         cur = self.db.cursor()
         query = ('SELECT * FROM {}'.format(self.tableName))
         cur.execute(query)
         records = cur.fetchall()
         return records
 
     def returnLastRecords(self, column, noOfRows2Return):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         cur = self.db.cursor()
         query = ('SELECT * FROM {} ORDER BY {} DESC LIMIT %s'.format(self.tableName, column))
         cur.execute(query, (noOfRows2Return,))
         rows = cur.fetchall()
         cur.close()
         return rows
 
-    def filterRows(self, matches):
+    def filterRows(self, matches, order_by=None):
         filterText = ''
         for match in matches:
             search_col, search_key = match
             if isinstance(search_key, tuple):
                 min, max = search_key
                 new = "{} > '{}' AND {} < '{}' AND ".format (search_col, min, search_col, max)
                 filterText += new
@@ -372,15 +386,18 @@
             elif search_key == 'None' or search_key is None:
                 new = "{} IS NULL AND ".format(search_col, search_key)
                 filterText += new
             else:
                 new = "{} = '{}' AND ".format(search_col, search_key)
                 filterText += new
         query = "SELECT * FROM {} WHERE ".format(self.tableName) + filterText[:-4]
-        # print (' {} '.format (query))
+        if order_by:
+            col, order = order_by
+            txt = 'ORDER BY {} {}'.format(col, order)
+            query += txt
         cur = self.db.cursor()
         cur.execute(query)
         records = cur.fetchall()
         cur.close()
         return records
 
     def returnRowsWhere(self, matches):
@@ -469,36 +486,14 @@
         cursor = self.db.cursor()
         if isinstance(query, str):
             commands = query.split(';')
         for command in commands:
             print('executing command: ', command)
             cursor.execute(command)
 
-    def filterRows(self, matches):
-        filterText = ''
-        for match in matches:
-            search_col, search_key = match
-            if isinstance(search_key, tuple):
-                min, max = search_key
-                new = "{} > '{}' AND {} < '{}' AND ".format(search_col, min, search_col, max)
-                filterText += new
-            elif isinstance(search_key, list):
-                new = "{} IN {} AND ".format(search_col, tuple(search_key))
-                filterText += new
-            else:
-                new = "{} = '{}' AND ".format(search_col, search_key)
-                filterText += new
-
-        query = "SELECT * FROM {} WHERE ".format(self.tableName) + filterText[:-4]
-        cursor = self.db.cursor()
-        cursor.execute(query)
-        records = cursor.fetchall()
-        cursor.close()
-        return records
-
     def importCSV(self, inpFile):
         with open(inpFile, 'r', encoding='unicode_escape', newline='') as csvfile:
             linereader = csv.reader(csvfile, delimiter=';', quotechar='|')
             for i, row in enumerate(linereader):
                 if i == 0:
                     tableHead = row
                     continue
@@ -690,14 +685,18 @@
         records = cursor.fetchall()
         cursor.close()
         values = []
         for i in records:
             values.append(i)
         return values
 
+    def write_file(self, data, filename):
+        # Convert binary data to proper format and write it on Hard Disk
+        with open(filename, 'wb') as file:
+            file.write(data)
 
 
 if __name__ == '__main__':
 
     # iniFile = r"D:\Python\MySQL\database.ini"
     iniFile = r"D:\Python\MySQL\web_db.ini"
     iniFile = r"D:\Python\MySQL\mysqlquerys\src\mysqlquerys\local.ini"
```

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/aeroclub.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/aeroclub.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/alimentari.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/alimentari.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/apartament.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/apartament.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/asigurari.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/asigurari.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/banca.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/banca.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/expenses.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/expenses.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/income.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/income.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/intercontotrans.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/intercontotrans.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/one_time_transactions.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/one_time_transactions.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys/sql/stat.sql` & `mysqlquerys-0.2.9/src/mysqlquerys/sql/stat.sql`

 * *Files identical despite different names*

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys.egg-info/PKG-INFO` & `mysqlquerys-0.2.9/src/mysqlquerys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlquerys
-Version: 0.2.8
+Version: 0.2.9
 Summary: Query-uri personale pentru a scrie in MySQL
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysqlquerys-0.2.8/src/mysqlquerys.egg-info/SOURCES.txt` & `mysqlquerys-0.2.9/src/mysqlquerys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

