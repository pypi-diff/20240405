# Comparing `tmp/cheltuieli-0.1.9.tar.gz` & `tmp/cheltuieli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheltuieli-0.1.9.tar", last modified: Sun Nov 19 21:13:36 2023, max compression
+gzip compressed data, was "cheltuieli-0.2.0.tar", last modified: Fri Apr  5 10:07:09 2024, max compression
```

## Comparing `cheltuieli-0.1.9.tar` & `cheltuieli-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.864605 cheltuieli-0.1.9/
--rw-rw-rw-   0        0        0       91 2023-09-01 10:44:32.000000 cheltuieli-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2023-11-19 21:13:36.864605 cheltuieli-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-05-27 06:30:20.000000 cheltuieli-0.1.9/README.md
--rw-rw-rw-   0        0        0      600 2022-02-14 09:29:30.000000 cheltuieli-0.1.9/requirements.txt
--rw-rw-rw-   0        0        0      703 2023-11-19 21:13:36.864605 cheltuieli-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-05-27 06:29:56.000000 cheltuieli-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.831285 cheltuieli-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.847587 cheltuieli-0.1.9/src/cheltuieli/
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.864605 cheltuieli-0.1.9/src/cheltuieli/GUI/
--rw-rw-rw-   0        0        0     2703 2022-02-10 15:17:59.000000 cheltuieli-0.1.9/src/cheltuieli/GUI/2del_check_expiration.ui
--rw-rw-rw-   0        0        0    11012 2023-09-11 11:28:42.000000 cheltuieli-0.1.9/src/cheltuieli/GUI/chelt_plan.ui
--rw-rw-rw-   0        0        0     9703 2022-02-10 15:17:59.000000 cheltuieli-0.1.9/src/cheltuieli/GUI/chelt_real.ui
--rw-rw-rw-   0        0        0     3244 2022-02-10 15:17:59.000000 cheltuieli-0.1.9/src/cheltuieli/GUI/filterWindow.ui
--rw-rw-rw-   0        0        0    14555 2022-02-10 15:17:59.000000 cheltuieli-0.1.9/src/cheltuieli/GUI/plan_vs_real.ui
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.864605 cheltuieli-0.1.9/src/cheltuieli/SQL/
--rw-rw-rw-   0        0        0     2111 2023-04-21 13:02:01.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/aeroclub.sql
--rw-rw-rw-   0        0        0    11387 2023-09-11 08:29:31.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/alimentari.sql
--rw-rw-rw-   0        0        0     2782 2023-04-21 13:04:02.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/apartament.sql
--rw-rw-rw-   0        0        0     3657 2023-04-21 13:04:07.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/asigurari.sql
--rw-rw-rw-   0        0        0     2078 2023-09-11 10:19:41.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/banca.sql
--rw-rw-rw-   0        0        0     2686 2023-04-21 13:04:11.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/expenses.sql
--rw-rw-rw-   0        0        0     2877 2023-04-21 13:04:16.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/income.sql
--rw-rw-rw-   0        0        0     1932 2023-04-21 13:04:20.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/intercontotrans.sql
--rw-rw-rw-   0        0        0     2107 2023-09-11 08:17:39.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/one_time_transactions.sql
--rw-rw-rw-   0        0        0     2144 2023-04-26 19:11:19.000000 cheltuieli-0.1.9/src/cheltuieli/SQL/stat.sql
--rw-rw-rw-   0        0        0       96 2021-11-05 12:45:32.000000 cheltuieli-0.1.9/src/cheltuieli/__init__.py
--rw-rw-rw-   0        0        0    18079 2023-11-15 19:11:23.000000 cheltuieli-0.1.9/src/cheltuieli/chelt_plan.py
--rw-rw-rw-   0        0        0    38742 2022-06-19 10:06:34.000000 cheltuieli-0.1.9/src/cheltuieli/chelt_real.py
--rw-rw-rw-   0        0        0      699 2023-11-19 21:01:06.000000 cheltuieli-0.1.9/src/cheltuieli/control.py
--rw-rw-rw-   0        0        0    24530 2023-09-11 13:14:14.000000 cheltuieli-0.1.9/src/cheltuieli/gui_desktop.py
--rw-rw-rw-   0        0        0     3090 2023-11-19 21:00:56.000000 cheltuieli-0.1.9/src/cheltuieli/masina.py
--rw-rw-rw-   0        0        0    47286 2021-11-05 12:47:06.000000 cheltuieli-0.1.9/src/cheltuieli/plan_vs_real.py
--rw-rw-rw-   0        0        0      964 2023-07-19 09:07:54.000000 cheltuieli-0.1.9/src/cheltuieli/salariu_prime.py
-drwxrwxrwx   0        0        0        0 2023-11-19 21:13:36.847587 cheltuieli-0.1.9/src/cheltuieli.egg-info/
--rw-rw-rw-   0        0        0      681 2023-11-19 21:13:36.000000 cheltuieli-0.1.9/src/cheltuieli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-11-19 21:13:36.000000 cheltuieli-0.1.9/src/cheltuieli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-19 21:13:36.000000 cheltuieli-0.1.9/src/cheltuieli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-11-19 21:13:36.000000 cheltuieli-0.1.9/src/cheltuieli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-19 21:13:36.000000 cheltuieli-0.1.9/src/cheltuieli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.590372 cheltuieli-0.2.0/
+-rw-rw-rw-   0        0        0      132 2023-12-04 11:41:42.000000 cheltuieli-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-04-05 10:07:09.590372 cheltuieli-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2022-05-27 06:30:20.000000 cheltuieli-0.2.0/README.md
+-rw-rw-rw-   0        0        0      594 2023-11-19 21:28:18.000000 cheltuieli-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0      703 2024-04-05 10:07:09.590372 cheltuieli-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-05-27 06:29:56.000000 cheltuieli-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.559491 cheltuieli-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.579460 cheltuieli-0.2.0/src/cheltuieli/
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.584098 cheltuieli-0.2.0/src/cheltuieli/GUI/
+-rw-rw-rw-   0        0        0     2703 2022-02-10 15:17:59.000000 cheltuieli-0.2.0/src/cheltuieli/GUI/2del_check_expiration.ui
+-rw-rw-rw-   0        0        0    11012 2023-09-11 11:28:42.000000 cheltuieli-0.2.0/src/cheltuieli/GUI/chelt_plan.ui
+-rw-rw-rw-   0        0        0     9703 2022-02-10 15:17:59.000000 cheltuieli-0.2.0/src/cheltuieli/GUI/chelt_real.ui
+-rw-rw-rw-   0        0        0     3244 2022-02-10 15:17:59.000000 cheltuieli-0.2.0/src/cheltuieli/GUI/filterWindow.ui
+-rw-rw-rw-   0        0        0    14555 2022-02-10 15:17:59.000000 cheltuieli-0.2.0/src/cheltuieli/GUI/plan_vs_real.ui
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.586603 cheltuieli-0.2.0/src/cheltuieli/SQL/
+-rw-rw-rw-   0        0        0    31937 2024-02-05 17:06:13.000000 cheltuieli-0.2.0/src/cheltuieli/SQL/cheltuieli_desktop.sql
+-rw-rw-rw-   0        0        0       96 2021-11-05 12:45:32.000000 cheltuieli-0.2.0/src/cheltuieli/__init__.py
+-rw-rw-rw-   0        0        0    33464 2024-02-15 11:49:47.000000 cheltuieli-0.2.0/src/cheltuieli/chelt_plan.py
+-rw-rw-rw-   0        0        0    38742 2022-06-19 10:06:34.000000 cheltuieli-0.2.0/src/cheltuieli/chelt_real.py
+-rw-rw-rw-   0        0        0     2550 2024-02-15 11:40:12.000000 cheltuieli-0.2.0/src/cheltuieli/control.py
+-rw-rw-rw-   0        0        0     4353 2024-02-15 13:06:42.000000 cheltuieli-0.2.0/src/cheltuieli/kalendar.py
+-rw-rw-rw-   0        0        0     6881 2024-02-26 14:49:14.000000 cheltuieli-0.2.0/src/cheltuieli/masina.py
+-rw-rw-rw-   0        0        0    47286 2021-11-05 12:47:06.000000 cheltuieli-0.2.0/src/cheltuieli/plan_vs_real.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.586603 cheltuieli-0.2.0/src/cheltuieli/static/
+-rw-rw-rw-   0        0        0      203 2023-12-04 11:11:36.000000 cheltuieli-0.2.0/src/cheltuieli/static/taxes.csv
+drwxrwxrwx   0        0        0        0 2024-04-05 10:07:09.589634 cheltuieli-0.2.0/src/cheltuieli.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-04-05 10:07:09.000000 cheltuieli-0.2.0/src/cheltuieli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-04-05 10:07:09.000000 cheltuieli-0.2.0/src/cheltuieli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 10:07:09.000000 cheltuieli-0.2.0/src/cheltuieli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 10:07:09.000000 cheltuieli-0.2.0/src/cheltuieli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 10:07:09.000000 cheltuieli-0.2.0/src/cheltuieli.egg-info/top_level.txt
```

### Comparing `cheltuieli-0.1.9/PKG-INFO` & `cheltuieli-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheltuieli
-Version: 0.1.9
+Version: 0.2.0
 Summary: cheltuielile mele
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cheltuieli-0.1.9/requirements.txt` & `cheltuieli-0.2.0/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ﻿cycler==0.11.0
 fonttools==4.29.1
 kiwisolver==1.3.2
 matplotlib==3.5.1
 mysql-connector-python==8.0.28
-MySQLquerys==0.0.10
 numpy==1.22.2
 packaging==21.3
 Pillow==9.0.1
 protobuf==3.19.4
 pyparsing==3.0.7
 PyQt5==5.15.6
 PyQt5-Qt5==5.15.2
 PyQt5-sip==12.9.1
 python-dateutil==2.8.2
 six==1.16.0
+mysqlquerys==0.2.7
```

### Comparing `cheltuieli-0.1.9/src/cheltuieli/GUI/2del_check_expiration.ui` & `cheltuieli-0.2.0/src/cheltuieli/GUI/2del_check_expiration.ui`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/GUI/chelt_plan.ui` & `cheltuieli-0.2.0/src/cheltuieli/GUI/chelt_plan.ui`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/GUI/chelt_real.ui` & `cheltuieli-0.2.0/src/cheltuieli/GUI/chelt_real.ui`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/GUI/filterWindow.ui` & `cheltuieli-0.2.0/src/cheltuieli/GUI/filterWindow.ui`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/GUI/plan_vs_real.ui` & `cheltuieli-0.2.0/src/cheltuieli/GUI/plan_vs_real.ui`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/chelt_real.py` & `cheltuieli-0.2.0/src/cheltuieli/chelt_real.py`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli/gui_desktop.py` & `cheltuieli-0.2.0/src/cheltuieli/chelt_plan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,515 +1,750 @@
-import sys
-import os
+import csv
+import os.path
 import traceback
-import decimal
-import datetime as dt
-from datetime import datetime, timedelta
 import numpy as np
-from PyQt5.QtWidgets import *
-from PyQt5 import uic
-from PyQt5 import QtCore
-from PyQt5.QtCore import *
-import sip
-import matplotlib.pyplot as plt
-from cheltuieli import chelt_plan
+from datetime import datetime, timedelta
+from dateutil.relativedelta import *
+import sys
 from mysqlquerys import connect
+from mysqlquerys import mysql_rm
 
+np.set_printoptions(linewidth=250)
+__version__ = 'V5'
 
-class MyApp(QMainWindow):
-    def __init__(self):
-        super(MyApp, self).__init__()
-        path2src, pyFileName = os.path.split(__file__)
-        uiFileName = 'chelt_plan.ui'
-        path2GUI = os.path.join(path2src, 'GUI', uiFileName)
-        Ui_MainWindow, QtBaseClass = uic.loadUiType(path2GUI)
-        self.ui = Ui_MainWindow()
-        self.ui.setupUi(self)
-        self.ini_file = r"D:\Python\MySQL\config.ini"
-        self.ui.GB_planned_expenses.setVisible(False)
-        self.gb_available_databases = self.ui.GB_databases
-        self.append_databases_to_box()
-
-        self.ui.cbActiveConto.currentIndexChanged.connect(self.get_table_info)
-        self.ui.CBMonths.currentIndexChanged.connect(self.populateDatesInterval)
-        self.ui.DEFrom.dateTimeChanged.connect(self.get_table_info)
-        self.ui.DEBis.dateTimeChanged.connect(self.get_table_info)
-        self.ui.planTable.horizontalHeader().sectionClicked.connect(self.sortPlan)
-        self.ui.PB_plotTablePie.clicked.connect(self.plotTablePie)
-        self.ui.PB_plotNamePie.clicked.connect(self.plotNamePie)
-        self.ui.PB_Plot.clicked.connect(self.plotGraf)
-        # self.ui.PB_export.clicked.connect(self.export)
 
+def calculate_last_day_of_month(mnth, year):
+    if mnth < 12:
+        # lastDayOfMonth = datetime(datetime.now().year, mnth + 1, 1) - timedelta(days=1)
+        lastDayOfMonth = datetime(year, mnth + 1, 1) - timedelta(days=1)
+        lastDayOfMonth = lastDayOfMonth.day
+    elif mnth == 12:
+        lastDayOfMonth = 31
+    return lastDayOfMonth
+
+
+def default_interval():
+    # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+    startDate = datetime(datetime.now().year, datetime.now().month, datetime.now().day)
+    if datetime.now().month != 12:
+        mnth = datetime.now().month + 1
+        lastDayOfMonth = datetime(datetime.now().year, mnth, 1) - timedelta(days=1)
+    else:
+        lastDayOfMonth = datetime(datetime.now().year + 1, 1, 1) - timedelta(days=1)
+
+    return startDate, lastDayOfMonth
+
+
+def get_monthly_interval(month:str, year):
+    # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+    mnth = datetime.strptime(month, "%B").month
+    startDate = datetime(year, mnth, 1)
+
+    if mnth != 12:
+        lastDayOfMonth = datetime(year, mnth + 1, 1) - timedelta(days=1)
+    else:
+        lastDayOfMonth = datetime(year + 1, 1, 1) - timedelta(days=1)
+
+    return startDate.date(), lastDayOfMonth.date()
+
+
+class Income:
+    def __init__(self, ini_file):
+        # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        self.ini_file = ini_file
+        pth2src = os.path.dirname(__file__)
+        # self.taxes_file = r"static\taxes.csv"
+        self.taxes_file = os.path.join(pth2src, 'static', 'taxes.csv')
+        self.tax_array, self.tax_header = self.conv_csv_to_np(skipHeader=1)
+        self.conf = connect.Config(self.ini_file)
+        self.income_table = mysql_rm.Table(self.conf.credentials, 'income')
+        self.selectedStartDate = None
+        self.selectedEndDate = None
+        self.conto = None
+        self.tableHead = None
+        self.income = None
+
+    def apply_taxes_to_salary(self):
+        for inc in self.incomes_for_time_interval:
+            if inc.is_salary:
+                print('####', inc.id, inc.name, inc.payments_for_interval)
+                inc.basic_brutto_35h_salary = inc.value
+                other_incomes_with_salary = self.find_other_incomes_with_salary_tax()
+                brutto = inc.basic_brutto_35h_salary
+                # print('******inc.basic_brutto_35h_salary', inc.basic_brutto_35h_salary)
+                for i in other_incomes_with_salary:
+                    if i.value:
+                        brutto += i.value
+                    else:
+                        brutto += inc.basic_brutto_35h_salary * float(i.proc)
+                inc.monthly_35h_brutto_salary = brutto
+                # print('******inc.monthly_35h_brutto_salary', inc.monthly_35h_brutto_salary)
+                taxes = ['lohnsteuer', 'rentenvers', 'arbeitslosvers', 'krankenvers', 'privatvers']
+                for tax in taxes:
+                    res = round(self.calculate_tax(inc, tax), 2)
+                    exec('inc.{} = {}'.format(tax, res))
+                inc.brutto = round(inc.brutto_monthly_salary, 2)
+
+        for inc in self.incomes_for_time_interval:
+            if inc.tax == 'bonus':
+                for payday in inc.payments_for_interval:
+                    income_with_same_payday = self.find_salary_with_same_payday(payday)
+                    if not income_with_same_payday:
+                        print(inc.id, inc.name, payday)
+                    inc.steuerklasse = income_with_same_payday.steuerklasse
+                    if not inc.value:
+                        inc.value = float(inc.proc) * income_with_same_payday.brutto_monthly_salary
+                    inc.brutto = round(float(inc.value), 2)
+
+                    taxes = ['lohnsteuer', 'rentenvers', 'arbeitslosvers']
+                    for tax in taxes:
+                        res = self.calculate_tax(inc, tax)
+                        exec('inc.{} = {}'.format(tax, res))
+            elif not inc.tax:
+                inc.brutto = round(float(inc.value), 2)
+
+    def find_salary_with_same_payday(self, payday):
+        for inc in self.incomes_for_time_interval:
+            if inc.is_salary:
+                if payday in inc.payments_for_interval:
+                    return inc
+
+    def calculate_tax(self, income, steuer):
+        indx_row = np.where((self.tax_array[:, self.tax_header.index('tax')] == income.tax) &
+                            (self.tax_array[:, self.tax_header.index('steuerklasse')].astype(int) == income.steuerklasse))
 
-    @property
-    def available_databases(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        con = connect.DbConnection(self.ini_file)
-        available_databases = con.databases
-        return available_databases
-
-    def append_databases_to_box(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        if self.gb_available_databases.layout() is not None:
-            self.delete_items_of_layout()
-        vbox = QVBoxLayout()
-        for i, db in enumerate(self.available_databases):
-            rb = QRadioButton(db)
-            rb.toggled.connect(self.connect_to_db)
-            vbox.addWidget(rb)
-        self.gb_available_databases.setLayout(vbox)
-
-    def delete_items_of_layout(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        layout_grupa = self.gb_available_databases.layout()
-        if layout_grupa is not None:
-            while layout_grupa.count():
-                item = layout_grupa.takeAt(0)
-                widget = item.widget()
-                if widget is not None:
-                    widget.setParent(None)
-                else:
-                    delete_items_of_layout(item.layout())
-            sip.delete(layout_grupa)
+        lohnteuer_proc = self.tax_array[indx_row, self.tax_header.index(steuer)]
+        lohnteuer_proc = float(lohnteuer_proc[0,0])/100
 
-    def connect_to_db(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        print('self.sender().objectName()', self.sender().text())
-        self.ui.GB_planned_expenses.setVisible(True)
-        self.populateCBMonths()
-        self.populateDatesInterval()
-        self.get_table_info(self.sender().text())
-        # self.populateCBConto()
-
-    def get_table_info(self, database_name):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        displayTableHead = ['table', 'name', 'value', 'myconto', 'payDay', 'freq']
-        selectedStartDate = self.ui.DEFrom.date().toPyDate()
-        selectedEndDate = self.ui.DEBis.date().toPyDate()
-        self.app = chelt_plan.CheltuieliPlanificate(self.ini_file, database_name)
-        tableHead, payments4Interval, income = self.app.prepareTablePlan(self.ui.cbActiveConto.currentText(), selectedStartDate, selectedEndDate)
-
-        self.populateExpensesPlan(tableHead, payments4Interval, displayTableHead)
-        self.populateTree(tableHead, payments4Interval)
-        self.populateIncomePlan(tableHead, income, displayTableHead)
-        self.totals()
-
-    # def export(self):
-    #     print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-    #     expName, _ = QFileDialog.getSaveFileName(self, "Save file", "", "Excel Files (*.xlsx)")
-    #     worksheets = [('Complete', datetime(datetime.now().year, 1, 1),datetime(datetime.now().year, 12, 31))]
-    #     for mnth in range(1, 13):
-    #         firstDayOfMonth = datetime(datetime.now().year, mnth, 1)
-    #         if mnth != 12:
-    #             lastDayOfMonth = datetime(datetime.now().year, mnth+1, 1) - timedelta(days=1)
-    #         else:
-    #             lastDayOfMonth = datetime(datetime.now().year + 1, 1, 1) - timedelta(days=1)
-    #
-    #         tup = (firstDayOfMonth.strftime("%B"), firstDayOfMonth, lastDayOfMonth)
-    #         worksheets.append(tup)
-    #
-    #     wb = Workbook()
-    #     ws = wb.active
-    #     for mnth, firstDayOfMonth, lastDayOfMonth in worksheets:
-    #         # print(mnth, firstDayOfMonth, lastDayOfMonth)
-    #         if mnth == 'Complete':
-    #             ws.title = mnth
-    #         else:
-    #             wb.create_sheet(mnth)
-    #         ws = wb[mnth]
-    #         self.ui.DEFrom.setDate(QDate(firstDayOfMonth))
-    #         self.ui.DEBis.setDate(QDate(lastDayOfMonth))
-    #         self.prepareTablePlan()
-    #
-    #         planExpenseTable, planExpenseTableHead = self.readPlanExpenses()
-    #         cheltData = np.insert(planExpenseTable, 0, planExpenseTableHead, 0)
-    #
-    #         for i, row in enumerate(cheltData):
-    #             for j, col in enumerate(row):
-    #                 ws.cell(row=i + 1, column=j + 1).value = cheltData[i][j]
-    #
-    #         firstRow = 1
-    #         firstCol = get_column_letter(1)
-    #         lastRow = len(cheltData)
-    #         lastCol = get_column_letter(len(cheltData[0]))
-    #
-    #         table_title = '{}_{}'.format('chelt', mnth )
-    #         new_text = ('{}{}:{}{}'.format(firstCol, firstRow, lastCol, lastRow))
-    #         tab = Table(displayName=table_title, ref=new_text)
-    #         # Add a default style with striped rows and banded columns
-    #         style = TableStyleInfo(name="TableStyleMedium9", showFirstColumn=False,
-    #                                showLastColumn=False, showRowStripes=True, showColumnStripes=True)
-    #         tab.tableStyleInfo = style
-    #         ws.add_table(tab)
-    #         ws.cell(row=lastRow + 1, column=1).value = 'Total Number of Expenses'
-    #         ws.cell(row=lastRow + 1, column=2).value = self.ui.LEtotalNoOfTransactions.text()
-    #         ws.cell(row=lastRow + 2, column=1).value = 'Total Expenses'
-    #         ws.cell(row=lastRow + 2, column=2).value = self.ui.LEtotalValue.text()
-    #         #######income
-    #
-    #         planIncomeTable, planIncomeTableHead = self.readPlanIncome()
-    #         incomeData = np.insert(planIncomeTable, 0, planIncomeTableHead, 0)
-    #         firstRow = lastRow + 5
-    #         firstCol = get_column_letter(1)
-    #         lastRow = firstRow + len(incomeData)
-    #         lastCol = get_column_letter(len(incomeData[0]))
-    #
-    #         for i, row in enumerate(incomeData):
-    #             for j, col in enumerate(row):
-    #                 ws.cell(row=i + firstRow, column=j + 1).value = incomeData[i][j]
-    #
-    #         table_title = '{}_{}'.format('income', mnth )
-    #         new_text1 = ('{}{}:{}{}'.format(firstCol, firstRow, lastCol, lastRow))
-    #         tab = Table(displayName=table_title, ref=new_text1)
-    #         # Add a default style with striped rows and banded columns
-    #         style = TableStyleInfo(name="TableStyleMedium9", showFirstColumn=False,
-    #                                showLastColumn=False, showRowStripes=True, showColumnStripes=True)
-    #         tab.tableStyleInfo = style
-    #         ws.add_table(tab)
-    #         ws.cell(row=lastRow + 1, column=1).value = 'Total Number of Incomes'
-    #         ws.cell(row=lastRow + 1, column=2).value = self.ui.LEtotalNoOfIncome.text()
-    #         ws.cell(row=lastRow + 2, column=1).value = 'Total Income'
-    #         ws.cell(row=lastRow + 2, column=2).value = self.ui.LEtotalIncome.text()
-    #
-    #     wb.save(expName)
-
-    def populateCBMonths(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        self.ui.CBMonths.addItem('interval')
-        months = [dt.date(2000, m, 1).strftime('%B') for m in range(1, 13)]
-        for month in months:
-            self.ui.CBMonths.addItem(month)
-
-    def populateCBConto(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        self.ui.cbActiveConto.addItem('all')
-        self.ui.cbActiveConto.addItems(self.app.myContos)
-
-    def populateDatesInterval(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        startDate = QDate(datetime.now().year, datetime.now().month, datetime.now().day)
-        if datetime.now().month != 12:
-            mnth = datetime.now().month + 1
-            lastDayOfMonth = datetime(datetime.now().year, mnth, 1) - timedelta(days=1)
+        if income.is_salary:
+            lohnteuer = float(income.brutto_monthly_salary) * lohnteuer_proc
         else:
-            lastDayOfMonth = datetime(datetime.now().year + 1, 1, 1) - timedelta(days=1)
+            lohnteuer = float(income.value) * lohnteuer_proc
+        return round(lohnteuer, 2)
 
-        if self.ui.CBMonths.currentText() != 'interval':
-            mnth = datetime.strptime(self.ui.CBMonths.currentText(), "%B").month
-            # print('****', mnth)
-            # if mnth == 1:
-            #     startDate = datetime(datetime.now().year - 1, 12, 30)
-            # elif mnth == 2:
-            #     startDate = datetime(datetime.now().year, mnth-1, 28)
-            # else:
-            #     startDate = datetime(datetime.now().year, mnth-1, 30)
-            #
-            # lastDayOfMonth = datetime(datetime.now().year, mnth, 29)
-
-            startDate = datetime(datetime.now().year, mnth, 1)
-            if mnth != 12:
-                lastDayOfMonth = datetime(datetime.now().year, mnth+1, 1) - timedelta(days=1)
-            else:
-                lastDayOfMonth = datetime(datetime.now().year + 1, 1, 1) - timedelta(days=1)
-
-            startDate = startDate - timedelta(days=2)
-            lastDayOfMonth = lastDayOfMonth - timedelta(days=2)
-
-            startDate = QDate(startDate)
-            lastDayOfMonth = QDate(lastDayOfMonth)
-
-        self.ui.DEFrom.setDate(startDate)
-        self.ui.DEBis.setDate(lastDayOfMonth)
-
-        self.ui.DEFrom.setCalendarPopup(True)
-        self.ui.DEBis.setCalendarPopup(True)
-
-    def populateTree(self, tableHead, table):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        self.ui.TWmnthVSIrreg.clear()
-        self.ui.TWmnthVSIrreg.setHeaderLabels(['freq', 'name', 'value'])
-        monthly_level = QTreeWidgetItem(self.ui.TWmnthVSIrreg)
-        monthly_level.setText(0, 'Monthly')
-        irregular_level = QTreeWidgetItem(self.ui.TWmnthVSIrreg)
-        irregular_level.setText(0, 'Irregular')
-        monthlyIndx = np.where(table[:, tableHead.index('freq')] == 1)
-        monthly = table[monthlyIndx]
-        for mnth in monthly:
-            mnth_item_level = QTreeWidgetItem(monthly_level)
-            mnth_item_level.setText(1, mnth[tableHead.index('name')])
-            mnth_item_level.setText(2, str(round(mnth[tableHead.index('value')])))
-
-        totalMonthly = table[monthlyIndx,tableHead.index('value')][0]
-        monthly_level.setText(1, 'Total')
-        monthly_level.setText(2, str(round(sum(totalMonthly), 2)))
-
-        irregIndx = np.where(table[:, tableHead.index('freq')] != 1)
-        irregular = table[irregIndx]
-        for irr in irregular:
-            irr_item_level = QTreeWidgetItem(irregular_level)
-            irr_item_level.setText(1, irr[tableHead.index('name')])
-            irr_item_level.setText(2, str(round(irr[tableHead.index('value')], 2)))
-
-        totalIrreg = table[irregIndx,tableHead.index('value')][0]
-        irregular_level.setText(1, 'Total')
-        irregular_level.setText(2, str(round(sum(totalIrreg), 2)))
-
-    def populateExpensesPlan(self, tableHead, table, displayTableHead=None):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        #
-        # print(tableHead)
-        # print(table)
-
-        if displayTableHead:
-            tableHead, table = self.convert_to_display_table(tableHead, table, displayTableHead)
-
-        self.ui.planTable.setColumnCount(len(tableHead))
-        self.ui.planTable.setHorizontalHeaderLabels(tableHead)
-        self.ui.planTable.setRowCount(table.shape[0])
-        for col in range(table.shape[1]):
-            for row in range(table.shape[0]):
-                if isinstance(table[row, col], int) or isinstance(table[row, col], float):
-                    item = QTableWidgetItem()
-                    item.setData(QtCore.Qt.DisplayRole, table[row, col])
-                elif isinstance(table[row, col], decimal.Decimal):
-                    val = float(table[row, col])
-                    item = QTableWidgetItem()
-                    item.setData(QtCore.Qt.DisplayRole, val)
-                else:
-                    item = QTableWidgetItem(str(table[row, col]))
-                self.ui.planTable.setItem(row, col, item)
-
-        if table.shape[1] > 0:
-            self.populate_expenses_summary(tableHead, table)
+    def convert_to_tabel(self):
+        table = [('table', 'name', 'brutto', 'taxes', 'netto', 'myconto', 'payDay', 'freq')]
+        for income in self.incomes_for_time_interval:
+            for datum in income.payments_for_interval:
+                if not income.brutto and not income.gesetzliche_abzuge and not income.netto:
+                    continue
+                tup = (income.table, income.name, income.brutto, income.gesetzliche_abzuge, income.netto, income.myconto, datum.date(), income.freq)
+                table.append(tup)
+        table = np.atleast_2d(table)
+        return table
+
+    def convert_to_salary_tabel(self):
+        table = [('table', 'name', 'brutto', 'lohnsteuer', 'rentenvers', 'arbeitslosvers', 'gesetzliche_abzuge',
+                  'netto', 'krankenvers', 'privatvers', 'abzuge', 'uberweisung', 'myconto', 'payDay', 'freq')]
+        brutto = 0
+        taxes = 0
+        netto = 0
+        abzuge = 0
+        uberweisung = 0
+        for income in self.incomes_for_time_interval:
+            if not income.in_salary:
+                print('++++++not in salary', income.name)
+                continue
+            for datum in income.payments_for_interval:
+                if not income.brutto and not income.gesetzliche_abzuge and not income.netto:
+                    continue
+                tup = (income.table,
+                       income.name,
+                       income.brutto,
+                       income.lohnsteuer,
+                       income.rentenvers,
+                       income.arbeitslosvers,
+                       income.gesetzliche_abzuge,
+                       income.netto,
+                       income.krankenvers,
+                       income.privatvers,
+                       income.abzuge,
+                       income.uberweisung,
+                       income.myconto,
+                       datum.date(),
+                       income.freq)
+                table.append(tup)
+                try:
+                    brutto += income.brutto
+                    if income.gesetzliche_abzuge:
+                        taxes += income.gesetzliche_abzuge
+                    if income.abzuge:
+                        abzuge += income.abzuge
+                    netto += float(income.netto)
+                    uberweisung += float(income.uberweisung)
+                except:
+                    print(income.name, income.brutto, income.netto)
+        table = np.atleast_2d(table)
+        return table, brutto, round(taxes, 2), netto, abzuge, uberweisung
+
+    def convert_to_total_income_tabel(self):
+        table = [('table', 'name', 'brutto', 'lohnsteuer', 'rentenvers', 'arbeitslosvers', 'gesetzliche_abzuge',
+                  'netto', 'krankenvers', 'privatvers', 'abzuge', 'uberweisung', 'myconto', 'payDay', 'freq',
+                  'in_salary')]
+        salary_brutto = 0
+        salary_gesetzliche_abzuge = 0
+        salary_netto = 0
+        salary_abzuge = 0
+        salary_uberweisung = 0
+        brutto = 0
+        taxes = 0
+        netto = 0
+        abzuge = 0
+        uberweisung = 0
+        for income in self.incomes_for_time_interval:
+            for datum in income.payments_for_interval:
+                if not income.brutto and not income.gesetzliche_abzuge and not income.netto:
+                    continue
+                tup = (income.table,
+                       income.name,
+                       income.brutto,
+                       income.lohnsteuer,
+                       income.rentenvers,
+                       income.arbeitslosvers,
+                       income.gesetzliche_abzuge,
+                       income.netto,
+                       income.krankenvers,
+                       income.privatvers,
+                       income.abzuge,
+                       income.uberweisung,
+                       income.myconto,
+                       datum.date(),
+                       income.freq,
+                       income.in_salary,
+                       )
+                table.append(tup)
+                try:
+                    if income.in_salary:
+                        salary_brutto += income.brutto
+                        if income.gesetzliche_abzuge:
+                            salary_gesetzliche_abzuge += income.gesetzliche_abzuge
+                        salary_netto += float(income.netto)
+                        if income.abzuge:
+                            salary_abzuge += income.abzuge
+                        salary_uberweisung += float(income.uberweisung)
+                    brutto += income.brutto
+                    if income.gesetzliche_abzuge:
+                        taxes += income.gesetzliche_abzuge
+                    if income.abzuge:
+                        abzuge += income.abzuge
+                    netto += float(income.netto)
+                    uberweisung += float(income.uberweisung)
+                except:
+                    print(income.name, income.brutto, income.netto)
+        table = np.atleast_2d(table)
+        result = (table, brutto, round(taxes, 2), netto, abzuge, uberweisung, salary_brutto, salary_gesetzliche_abzuge, salary_netto, salary_abzuge, salary_uberweisung)
+        return result
+
+    def conv_csv_to_np(self, delimiter=';', skipHeader=None):
+        array = []
+        header = []
+        with open(self.taxes_file, 'r') as file:
+            reader = csv.reader(file, delimiter=delimiter)
+            for i, row in enumerate(reader):
+                if skipHeader:
+                    if i < skipHeader:
+                        header.append(row)
+                        continue
+                array.append(row)
+            array = np.atleast_2d(array)
+        if skipHeader == 1:
+            header = header[0]
+
+        return array, header
+
+    def get_all_income_rows(self):
+        vals = self.income_table.returnAllRecordsFromTable()
+        all_incomes = []
+        for row in vals:
+            row = list(row)
+            income = Cheltuiala(row, self.income_table.columnsNames)
+            income.set_table(self.income_table.tableName)
+            all_incomes.append(income)
+        return all_incomes
+
+    def filter_income_for_interval(self, all_income_rows):
+        incomes_interval = []
+        for inc in all_income_rows:
+            payments_in_interval = None
+            if self.myconto == 'all':
+                payments_in_interval = inc.calculate_payments_in_interval(self.selectedStartDate, self.selectedEndDate)
+            elif self.myconto == inc.myconto:
+                payments_in_interval = inc.calculate_payments_in_interval(self.selectedStartDate, self.selectedEndDate)
+            if payments_in_interval:
+                inc.payments_for_interval = payments_in_interval
+                incomes_interval.append(inc)
+        return incomes_interval
+
+    def find_other_incomes_with_salary_tax(self):
+        other_incomes_with_salary = []
+        for i in self.incomes_for_time_interval:
+            if i.tax == 'salary' and i.name != 'Salariu':
+                other_incomes_with_salary.append(i)
+        return other_incomes_with_salary
+
+    def prepareTablePlan(self, conto, selectedStartDate, selectedEndDate):
+        self.selectedStartDate = selectedStartDate
+        self.selectedEndDate = selectedEndDate
+        self.myconto = conto
+
+        all_income_rows = self.get_all_income_rows()
+        self.incomes_for_time_interval = self.filter_income_for_interval(all_income_rows)
+        self.apply_taxes_to_salary()
+        # table = self.convert_to_tabel()
+        result = self.convert_to_total_income_tabel()
+        table, self.brutto, self.taxes, self.netto, self.abzuge, self.uberweisung, self.salary_brutto, \
+        self.salary_gesetzliche_abzuge, self.salary_netto, self.salary_abzuge, self.salary_uberweisung = result
+
+        self.tableHead, self.income = list(table[0]), table[1:]
+
+    def get_salary_income(self, month):
+        self.selectedStartDate, self.selectedEndDate = get_monthly_interval(month)
+        self.myconto = 'EC'
+
+        all_income_rows = self.get_all_income_rows()
+        self.incomes_for_time_interval = self.filter_income_for_interval(all_income_rows)
+        self.apply_taxes_to_salary()
+        table, brutto, taxes, netto, abzuge, uberweisung = self.convert_to_salary_tabel()
+        return table, brutto, taxes, netto, abzuge, uberweisung
+
+    def get_total_monthly_income(self, month):
+        self.selectedStartDate, self.selectedEndDate = get_monthly_interval(month)
+        self.myconto = 'all'
+
+        all_income_rows = self.get_all_income_rows()
+        self.incomes_for_time_interval = self.filter_income_for_interval(all_income_rows)
+        self.apply_taxes_to_salary()
+        table, brutto, taxes, netto, abzuge, uberweisung = self.convert_to_total_income_tabel()
+        return table, brutto, taxes, netto, abzuge, uberweisung
 
     def convert_to_display_table(self, tableHead, table, displayTableHead):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
         newTableData = np.empty([table.shape[0], len(displayTableHead)], dtype=object)
         for i, col in enumerate(displayTableHead):
             indxCol = tableHead.index(col)
             newTableData[:,i] = table[:, indxCol]
 
         return displayTableHead, newTableData
 
-    def populate_expenses_summary(self, tableHead, table):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        allValues = table[:, tableHead.index('value')]
-        if None in allValues:
-            allValues = allValues[allValues != np.array(None)]
-        totalVal = round(sum(allValues.astype(float)), 2)
-        self.ui.LEtotalNoOfTransactions.setText(str(len(table)))
-        self.ui.LEtotalValue.setText(str(totalVal))
+    @property
+    def monthly_income(self):
+        monthly_income = 0
+        for row in self.income:
+            if row[self.tableHead.index('freq')] == 1:
 
-        indxMonthly = np.where(table[:,tableHead.index('freq')] == 1)[0]
-        monthly = table[indxMonthly, tableHead.index('value')]
-        if None in monthly:
-            monthly = monthly[monthly != np.array(None)]
-        totalMonthly = round(sum(monthly.astype(float)), 2)
-        self.ui.LEnoOfMonthly.setText(str(monthly.shape[0]))
-        self.ui.LEtotalMonthly.setText(str(totalMonthly))
+                monthly_income += float(row[self.tableHead.index('netto')])
+        return round(monthly_income, 2)
 
-        indxIrregular = np.where(table[:,tableHead.index('freq')] != 1)[0]
-        irregular = table[indxIrregular, tableHead.index('value')]
-        if None in irregular:
-            irregular = irregular[irregular != np.array(None)]
-        totalIrregular = round(sum(irregular.astype(float)), 2)
-        self.ui.LEnoOfIrregular.setText(str(irregular.shape[0]))
-        self.ui.LEirregular.setText(str(totalIrregular))
-
-    def populateIncomePlan(self, tableHead, table, displayTableHead=None):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        if displayTableHead:
-            tableHead, table = self.convert_to_display_table(tableHead, table, displayTableHead)
-
-        self.ui.planTableIncome.setColumnCount(len(tableHead))
-        self.ui.planTableIncome.setHorizontalHeaderLabels(tableHead)
-        self.ui.planTableIncome.setRowCount(table.shape[0])
-        for col in range(table.shape[1]):
-            for row in range(table.shape[0]):
-                if isinstance(table[row, col], int) or isinstance(table[row, col], float):
-                    item = QTableWidgetItem()
-                    item.setData(QtCore.Qt.DisplayRole, table[row, col])
-                elif isinstance(table[row, col], decimal.Decimal):
-                    val = float(table[row, col])
-                    item = QTableWidgetItem()
-                    item.setData(QtCore.Qt.DisplayRole, val)
-                else:
-                    item = QTableWidgetItem(str(table[row, col]))
-                self.ui.planTableIncome.setItem(row, col, item)
+    @property
+    def irregular_income(self):
+        irregular_income = 0
+        for row in self.income:
+            if row[self.tableHead.index('freq')] > 1:
+                irregular_income += float(row[self.tableHead.index('netto')])
+        return round(irregular_income, 2)
+
+
+class Cheltuiala:
+    def __init__(self, row, tableHead):
+        # print('#####', tableHead)
+        self.tableHead = tableHead
+        self.read_row(row)
+        self.lohnsteuer = None
+        self.rentenvers = None
+        self.arbeitslosvers = None
+        self.krankenvers = None
+        self.privatvers = None
+        self.brutto = None
+
+    def read_row(self, row):
+        for col in self.tableHead:
+            exec('self.{} = row[self.tableHead.index("{}")]'.format(col, col))
 
-        if table.shape[1] > 0:
-            self.populate_income_summary(tableHead, table)
+        if self.pay_day is None:
+            self.pay_day = calculate_last_day_of_month(self.valid_from.month, self.valid_from.year)
 
-    def populate_income_summary(self, tableHead, table):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        allValues = table[:, tableHead.index('value')]
-        if None in allValues:
-            allValues = allValues[allValues != np.array(None)]
-        # for i in allValues:
-        #     print(i, type(i))
-        totalVal = sum(allValues.astype(float))
-        totalVal = round((totalVal), 2)
-        self.ui.LEtotalNoOfIncome.setText(str(len(table)))
-        self.ui.LEtotalIncome.setText(str(totalVal))
-
-    def totals(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        if self.ui.LEtotalNoOfTransactions.text():
-            expensesTrans = int(self.ui.LEtotalNoOfTransactions.text())
+        if self.auto_ext is None or self.auto_ext == 0:
+            self.auto_ext = False
         else:
-            expensesTrans = 0
-        if self.ui.LEtotalNoOfIncome.text():
-            incomeTrans = int(self.ui.LEtotalNoOfIncome.text())
+            self.auto_ext = True
+
+    def set_table(self, table_name):
+        self.table = table_name
+
+    @property
+    def first_payment(self):
+        try:
+            first_payment = datetime(self.valid_from.year, self.valid_from.month, self.pay_day)
+        except:
+            # print(self.id, self.table, self.name)
+            # print(self.valid_from.year, self.valid_from.month, self.pay_day)
+            # first_payment = calculate_last_day_of_month(selectedStartDate.month)
+            first_payment = datetime(self.valid_from.year, self.valid_from.month, calculate_last_day_of_month(self.valid_from.month, self.valid_from.year))
+        return first_payment
+
+    @property
+    def is_salary(self):
+        if self.name == 'Salariu' and self.freq == 1 and self.value:
+            is_salary = True
         else:
-            incomeTrans = 0
+            is_salary = False
+        return is_salary
+
+    @property
+    def basic_brutto_35h_salary(self):
+        return self.val
+
+    @basic_brutto_35h_salary.setter
+    def basic_brutto_35h_salary(self, income):
+        self.val = float(income)
+
+    @property
+    def monthly_35h_brutto_salary(self):
+        return self.val
+
+    @monthly_35h_brutto_salary.setter
+    def monthly_35h_brutto_salary(self, income):
+        self.val = float(income)
+
+    @property
+    def hourly_salary(self):
+        hourly_salary = self.monthly_35h_brutto_salary / 4 / 35
+        return hourly_salary
+
+    @property
+    def brutto_monthly_salary(self):
+        val = self.hourly_salary * self.hours * 4
+        return val
+
+    @property
+    def gesetzliche_abzuge(self):
+        try:
+            gesetzliche_abzuge = round(self.lohnsteuer +self.rentenvers + self.arbeitslosvers, 2)
+        except:
+            return None
+        return gesetzliche_abzuge
 
-        if self.ui.LEtotalValue.text():
-            expenses = float(self.ui.LEtotalValue.text())
+    @property
+    def abzuge(self):
+        try:
+            abzuge = round(self.krankenvers + self.privatvers, 2)
+        except:
+            return None
+        return abzuge
+
+    @property
+    def netto(self):
+        if self.gesetzliche_abzuge and self.brutto:
+            netto = round(self.brutto - self.gesetzliche_abzuge, 2)
         else:
-            expenses = 0
-        if self.ui.LEtotalIncome.text():
-            income = float(self.ui.LEtotalIncome.text())
+            netto = self.brutto
+        return netto
+
+    @property
+    def uberweisung(self):
+        if self.netto and self.is_salary:
+            uberweisung = round(float(self.netto) - self.abzuge, 2)
         else:
-            income = 0
+            uberweisung = self.netto
+        return uberweisung
 
-        trans = expensesTrans + incomeTrans
-        total = round(expenses + income, 2)
+    def list_of_payments_valid_from_till_selected_end_date(self, selectedEndDate):
+        list_of_payments_till_selected_end_date = []
+        if self.valid_from <= self.first_payment.date() <= selectedEndDate:
+            list_of_payments_till_selected_end_date.append(self.first_payment)
+
+        next_payment = self.first_payment + relativedelta(months=self.freq)
+        if next_payment.day != self.pay_day:
+            try:
+                next_payment = datetime(next_payment.year, next_payment.month, self.pay_day)
+            except:
+                next_payment = datetime(next_payment.year, next_payment.month, calculate_last_day_of_month(next_payment.month, next_payment.year))
+        if self.valid_from <= next_payment.date() <= selectedEndDate:
+            list_of_payments_till_selected_end_date.append(next_payment)
+
+        while next_payment.date() <= selectedEndDate:
+            next_payment = next_payment + relativedelta(months=self.freq)
+            if next_payment.day != self.pay_day:
+                try:
+                    next_payment = datetime(next_payment.year, next_payment.month, self.pay_day)
+                except:
+                    # print('#####', next_payment.year, next_payment.month,
+                    #                         calculate_last_day_of_month(next_payment.month, next_payment.year))
+                    next_payment = datetime(next_payment.year, next_payment.month,
+                                            calculate_last_day_of_month(next_payment.month, next_payment.year))
+            if self.valid_from <= next_payment.date() <= selectedEndDate:
+                list_of_payments_till_selected_end_date.append(next_payment)
+        return list_of_payments_till_selected_end_date
+
+    def cut_all_before_selectedStartDate(self, lista, selectedStartDate):
+        new_list = []
+        for date in lista:
+            if date.date() >= selectedStartDate:
+                new_list.append(date)
+        return new_list
+
+    def cut_all_after_valid_to(self, lista):
+        new_list = []
+        for date in lista:
+            if date.date() <= self.valid_to:
+                new_list.append(date)
+        return new_list
+
+    def calculate_payments_in_interval(self, selectedStartDate, selectedEndDate):
+        list_of_payments_valid_from_till_selected_end_date = self.list_of_payments_valid_from_till_selected_end_date(selectedEndDate)
+        # print(20*'*')
+        # for i in list_of_payments_valid_from_till_selected_end_date:
+        #     print(i)
+        # print(20*'*')
+
+        list_of_payments_selected_start_date_till_selected_end_date = self.cut_all_before_selectedStartDate(list_of_payments_valid_from_till_selected_end_date, selectedStartDate)
+        # print(20*'*')
+        # for i in list_of_payments_selected_start_date_till_selected_end_date:
+        #     print(i)
+        # print(20*'*')
+
+        if self.valid_to and self.valid_to < selectedEndDate and not self.auto_ext:
+            list_of_payments_selected_start_date_till_selected_end_date = self.cut_all_after_valid_to(list_of_payments_selected_start_date_till_selected_end_date)
+            # print(20*'*')
+            # for i in list_of_payments_selected_start_date_till_selected_end_date:
+            #     print(i)
+            # print(20*'*')
 
-        self.ui.LEtotalNo.setText(str(trans))
-        self.ui.LEtotalVa.setText(str(total))
+        return list_of_payments_selected_start_date_till_selected_end_date
 
-    def sortPlan(self, logical_index):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        header = self.ui.planTable.horizontalHeader()
-        order = Qt.DescendingOrder
-        if not header.isSortIndicatorShown():
-            header.setSortIndicatorShown(True)
-        elif header.sortIndicatorSection() == logical_index:
-            order = header.sortIndicatorOrder()
-        header.setSortIndicator(logical_index, order)
-        self.ui.planTable.sortItems(logical_index, order)
-
-    def readPlanExpenses(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        rows = self.ui.planTable.rowCount()
-        cols = self.ui.planTable.columnCount()
-        planExpenseTable = np.empty((rows, cols), dtype=object)
-        planExpenseTableHead = []
-        for row in range(rows):
-            for column in range(cols):
-                cell = self.ui.planTable.item(row, column)
-                planExpenseTable[row, column] = cell.text()
-                colName = self.ui.planTable.horizontalHeaderItem(column).text()
-                if colName not in planExpenseTableHead:
-                    planExpenseTableHead.append(colName)
-
-        return planExpenseTable, planExpenseTableHead
-
-    def readPlanIncome(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        rows = self.ui.planTableIncome.rowCount()
-        cols = self.ui.planTableIncome.columnCount()
-        planIncomeTable = np.empty((rows, cols), dtype=object)
-        planIncomeTableHead = []
-        for row in range(rows):
-            for column in range(cols):
-                cell = self.ui.planTableIncome.item(row, column)
-                planIncomeTable[row, column] = cell.text()
-                colName = self.ui.planTableIncome.horizontalHeaderItem(column).text()
-                if colName not in planIncomeTableHead:
-                    planIncomeTableHead.append(colName)
-
-        return planIncomeTable, planIncomeTableHead
-
-    def plotTablePie(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        realExpenseTable, realExpenseTableHead = self.readPlanExpenses()
-        allValues = realExpenseTable[:, realExpenseTableHead.index('value')].astype(float)
+    @property
+    def first_payment_date(self):
+        first_payment_date = datetime(self.valid_from.year, self.valid_from.month, self.pay_day)
+        return first_payment_date
+
+    @property
+    def payments_for_interval(self):
+        return self.pfi
+
+    @payments_for_interval.setter
+    def payments_for_interval(self, payments_days):
+        self.pfi= payments_days
+
+
+class CheltuieliPlanificate:
+    def __init__(self, ini_file):
+        # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        self.ini_file = ini_file
+        self.conf = connect.Config(self.ini_file)
+        self.tableHead = ['id', 'name', 'value', 'myconto', 'freq', 'pay_day', 'valid_from', 'valid_to', 'auto_ext']
+        self.myAccountsTable = self.sql_rm.Table(self.conf.credentials, 'banca')
+        self.myContos = self.myAccountsTable.returnColumn('name')
+
+        try:
+            self.dataBase = self.sql_rm.DataBase(self.conf.credentials)
+        except Exception as err:
+            print(traceback.format_exc())
+
+    @property
+    def sql_rm(self):
+        # print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        if self.conf.db_type == 'mysql':
+            sql_rm = mysql_rm
+        return sql_rm
+
+    def tot_no_of_irregular_expenses(self):
+        indxMonthly = np.where(self.expenses[:,self.tableHead.index('freq')] != 1)[0]
+        monthly = self.expenses[indxMonthly, self.tableHead.index('value')]
+        return monthly.shape[0]
+
+    def tot_val_of_irregular_expenses(self):
+        indxMonthly = np.where(self.expenses[:,self.tableHead.index('freq')] != 1)[0]
+        monthly = self.expenses[indxMonthly, self.tableHead.index('value')]
+        if None in monthly:
+            monthly = monthly[monthly != np.array(None)]
+        totalMonthly = round(sum(monthly.astype(float)), 2)
+        return totalMonthly
+
+    def tot_no_of_monthly_expenses(self):
+        indxMonthly = np.where(self.expenses[:,self.tableHead.index('freq')] == 1)[0]
+        monthly = self.expenses[indxMonthly, self.tableHead.index('value')]
+        return monthly.shape[0]
+
+    def tot_val_of_monthly_expenses(self):
+        indxMonthly = np.where(self.expenses[:,self.tableHead.index('freq')] == 1)[0]
+        monthly = self.expenses[indxMonthly, self.tableHead.index('value')]
+        if None in monthly:
+            monthly = monthly[monthly != np.array(None)]
+        totalMonthly = round(sum(monthly.astype(float)), 2)
+        return totalMonthly
+
+    def tot_no_of_expenses(self):
+        allValues = self.expenses[:,self.tableHead.index('value')]
+        if None in allValues:
+            allValues = allValues[allValues != np.array(None)]
+        return len(allValues)
+
+    def tot_val_of_expenses(self):
+        allValues = self.expenses[:,self.tableHead.index('value')]
+        if None in allValues:
+            allValues = allValues[allValues != np.array(None)]
+        totalVal = round(sum(allValues.astype(float)), 2)
+        return totalVal
+
+    def tot_no_of_income(self):
+        allValues = self.income[:,self.tableHead.index('value')]
         if None in allValues:
             allValues = allValues[allValues != np.array(None)]
-        totalVal = sum(allValues)
+        return len(allValues)
+
+    def tot_val_of_income(self):
+        allValues = self.income[:,self.tableHead.index('value')]
+        if None in allValues:
+            allValues = allValues[allValues != np.array(None)]
+        totalVal = round(sum(allValues.astype(float)), 2)
+        return totalVal
 
-        colTableName = realExpenseTable[:, realExpenseTableHead.index('table')]
-        labels = []
-        sizes = []
-        for table in np.unique(colTableName):
-            indx = np.where(realExpenseTable[:, realExpenseTableHead.index('table')]==table)
-            smallArray = realExpenseTable[indx]
-            values = sum(smallArray[:, realExpenseTableHead.index('value')].astype(float))
-            txt = '{} = {:.2f}'.format(table, values)
-            labels.append(txt)
-            size = (values/totalVal)*100
-            sizes.append(size)
-
-        fig1, ax1 = plt.subplots()
-        ax1.pie(sizes, labels=labels, autopct='%1.2f%%', startangle=90)
-        ax1.axis('equal')
-        plt.legend(title='Total: {:.2f}'.format(totalVal))
-
-        plt.show()
-
-    def plotNamePie(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        realExpenseTable, realExpenseTableHead = self.readPlanExpenses()
-        allValues = realExpenseTable[:, realExpenseTableHead.index('value')].astype(float)
+    def tot_no_of_expenses_income(self):
+        allExpenses = self.expenses[:,self.tableHead.index('value')]
+        allIncome = self.income[:,self.tableHead.index('value')]
+        tot = len(allExpenses) + len(allIncome)
+        return tot
+
+    def tot_val_of_expenses_income(self):
+        allValues = self.income[:,self.tableHead.index('value')]
+        if None in allValues:
+            allValues = allValues[allValues != np.array(None)]
+        totalIncome = round(sum(allValues.astype(float)), 2)
+        allValues = self.expenses[:,self.tableHead.index('value')]
         if None in allValues:
             allValues = allValues[allValues != np.array(None)]
-        totalVal = sum(allValues)
+        totalExpenses = round(sum(allValues.astype(float)), 2)
+        return round(totalIncome + totalExpenses, 2)
+
+    def get_all_sql_vals(self):
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        all_chelt = []
+        for table in self.dataBase.allAvailableTablesInDatabase:
+            if table == 'income':
+                continue
+            active_table = self.sql_rm.Table(self.conf.credentials, table)
+            active_table_head = active_table.columnsNames
+            if 'table' in self.tableHead:
+                self.tableHead.remove('table')
+            if 'payDay' in self.tableHead:
+                self.tableHead.remove('payDay')
+            check = all(item in active_table_head for item in self.tableHead)
+            if check:
+                # vals = active_table.returnColumns(self.tableHead)
+                vals = active_table.returnAllRecordsFromTable()
+                for row in vals:
+                    row = list(row)
+                    chelt = Cheltuiala(row, active_table.columnsNames)
+                    chelt.set_table(table)
+                    all_chelt.append(chelt)
+        return all_chelt
+
+    def filter_dates(self, all_chelt, selectedStartDate, selectedEndDate):
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        remaining = []
+        for chelt in all_chelt:
+            # print(chelt.table, chelt.name, chelt.id, chelt.pay_day)
+            payments_in_interval = chelt.calculate_payments_in_interval(selectedStartDate, selectedEndDate)
+            # print(payments_in_interval)
+            # if chelt.name == 'Steuererklärung_2022':
+            #     print(chelt.table, chelt.name, chelt.id, chelt.pay_day, payments_in_interval)
+            if isinstance(payments_in_interval, list):
+                chelt.payments_for_interval = payments_in_interval
+                # print(chelt.table, chelt.name, chelt.id, chelt.pay_day, chelt.payments_for_interval)
+                if chelt.payments_for_interval:
+                    remaining.append(chelt)
+        return remaining
+
+    def filter_conto(self, chelt_list, conto):
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        remaining = []
+        for ch in chelt_list:
+            if conto == 'all' and ch.table != 'intercontotrans':
+                remaining.append(ch)
+            elif ch.myconto == conto:
+                remaining.append(ch)
+
+        return remaining
+
+    def split_expenses_income(self, chelt):
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        arr_expenses = []
+        arr_income = []
+        for ch in chelt:
+            if ch.value == 0:
+                continue
+            for payment_day in ch.payments_for_interval:
+                # if ch.value and ch.value > 0:
+                #     incomeTable = self.sql_rm.Table(self.conf.credentials, ch.table)
+                #     full_row = list(incomeTable.returnRowsWhere(('id', ch.id))[0])
+                #     venit_instance = Income(full_row, incomeTable.columnsNames)
+                #     ch.value = venit_instance.calculate_income()
+
+                variables = vars(ch)
+                row = [ch.table]
+                for col in self.tableHead:
+                    val = variables[col]
+                    row.append(val)
+                # print('######', payment_day, type(payment_day))
+                row.append(payment_day.date())
+                if ch.value and ch.value > 0:
+                    arr_income.append(row)
+                else:
+                    arr_expenses.append(row)
+        arr_expenses = np.atleast_2d(arr_expenses)
+        arr_income = np.atleast_2d(arr_income)
+        self.tableHead.insert(0, 'table')
+        self.tableHead.append('payDay')
+        return arr_expenses, arr_income
+
+    def prepareTablePlan(self, conto, selectedStartDate, selectedEndDate):
+        #print('Module: {}, Class: {}, Def: {}, Caller: {}'.format(__name__, __class__, sys._getframe().f_code.co_name, sys._getframe().f_back.f_code.co_name))
+        print(selectedStartDate, selectedEndDate)
+        all_chelt = self.get_all_sql_vals()
+        # for i in all_chelt:
+        #     print(i.freq)
+        # all_chelt = self.get_one_time_transactions(all_chelt)
+
+        chelt_in_time_interval = self.filter_dates(all_chelt, selectedStartDate, selectedEndDate)
+        # for chelt in chelt_in_time_interval:
+        #     print(chelt.table, chelt.name, chelt.id, chelt.pay_day, chelt.conto, chelt.payments_for_interval)
+
+        chelt_after_contofilter = self.filter_conto(chelt_in_time_interval, conto)
+        # for chelt in chelt_after_contofilter:
+        #     print(chelt.table, chelt.name, chelt.id, chelt.pay_day, chelt.conto, chelt.payments_for_interval)
+
+        self.expenses, self.income = self.split_expenses_income(chelt_after_contofilter)
+        if self.expenses.shape == (1, 0):
+            expenses = np.empty((0, len(self.tableHead)))
+        if self.income.shape == (1, 0):
+            income = np.empty((0, len(self.tableHead)))
 
-        colTableName = realExpenseTable[:, realExpenseTableHead.index('name')]
-        labels = []
-        sizes = []
-        for table in np.unique(colTableName):
-            indx = np.where(realExpenseTable[:, realExpenseTableHead.index('name')]==table)
-            smallArray = realExpenseTable[indx]
-            values = sum(smallArray[:, realExpenseTableHead.index('value')].astype(float))
-            txt = '{} = {:.2f}'.format(table, values)
-            labels.append(txt)
-            size = (values/totalVal)*100
-            sizes.append(size)
-
-        fig1, ax1 = plt.subplots()
-        ax1.pie(sizes, labels=labels, autopct='%1.2f%%', startangle=90)
-        ax1.axis('equal')
-        plt.legend(title='Total: {:.2f}'.format(totalVal))
-
-        plt.show()
-
-    def plotGraf(self):
-        print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
-        realExpenseTable, realExpenseTableHead = self.readPlanExpenses()
-        planIncomeTable, planIncomeTableHead = self.readPlanIncome()
-        x_exp = []
-        y_exp = []
-        for date in np.unique(realExpenseTable[:, realExpenseTableHead.index('payDay')]):
-            indx = np.where(realExpenseTable[:, realExpenseTableHead.index('payDay')] == date)
-            arr = realExpenseTable[indx, realExpenseTableHead.index('value')].astype(float)
-            x_exp.append(date)
-            y_exp.append(abs(sum(arr[0])))
-
-        x_inc = []
-        y_inc = []
-        for date in np.unique(planIncomeTable[:, planIncomeTableHead.index('payDay')]):
-            indx = np.where(planIncomeTable[:, planIncomeTableHead.index('payDay')] == date)
-            arr = planIncomeTable[indx, planIncomeTableHead.index('value')].astype(float)
-            x_inc.append(date)
-            y_inc.append(abs(sum(arr[0])))
-
-        fig1, ax1 = plt.subplots()
-        ax1.plot(x_exp, y_exp)
-        ax1.plot(x_inc, y_inc)
-        # plt.setp(plt.get_xticklabels(), rotation=30, ha="right")
-        fig1.autofmt_xdate()
-        plt.grid()
-        plt.show()
-
-
-def main():
-    app = QApplication(sys.argv)
-    window = MyApp()
-    window.show()
-    # sys.exit(app.exec_())
-    app.exec_()
+    def convert_to_display_table(self, tableHead, table, displayTableHead):
+        #print('Module: {}, Class: {}, Def: {}'.format(__name__, __class__, sys._getframe().f_code.co_name))
+        newTableData = np.empty([table.shape[0], len(displayTableHead)], dtype=object)
+        for i, col in enumerate(displayTableHead):
+            indxCol = tableHead.index(col)
+            newTableData[:,i] = table[:, indxCol]
 
+        return displayTableHead, newTableData
+
+
+class CheltPlusIncome:
+    def __init__(self, ini_file, conto, dataFrom, dataBis):
+        self.income = Income(ini_file)
+        self.income.prepareTablePlan(conto, dataFrom, dataBis)
 
-if __name__ == '__main__':
-    main()
+        self.chelt = CheltuieliPlanificate(ini_file)
+        self.chelt.prepareTablePlan(conto, dataFrom, dataBis)
+
+    @property
+    def summary_table(self):
+        total_dif = round(self.income.netto + self.chelt.tot_val_of_expenses(), 2)
+        monthly_dif = round(self.income.monthly_income + self.chelt.tot_val_of_monthly_expenses(), 2)
+        irregular_dif = round(self.income.irregular_income + self.chelt.tot_val_of_irregular_expenses())
+        arr = [('', 'Income', 'Expenses', 'Diff'),
+               ('Total', self.income.netto, self.chelt.tot_val_of_expenses(), total_dif),
+               ('Monthly', self.income.monthly_income, self.chelt.tot_val_of_monthly_expenses(), monthly_dif),
+               ('Irregular', self.income.irregular_income, self.chelt.tot_val_of_irregular_expenses(), irregular_dif),
+               ]
+        arr = np.atleast_2d(arr)
+        return arr
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheltuieli-0.1.9/src/cheltuieli/plan_vs_real.py` & `cheltuieli-0.2.0/src/cheltuieli/plan_vs_real.py`

 * *Files identical despite different names*

### Comparing `cheltuieli-0.1.9/src/cheltuieli.egg-info/PKG-INFO` & `cheltuieli-0.2.0/src/cheltuieli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheltuieli
-Version: 0.1.9
+Version: 0.2.0
 Summary: cheltuielile mele
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cheltuieli-0.1.9/src/cheltuieli.egg-info/SOURCES.txt` & `cheltuieli-0.2.0/src/cheltuieli.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,31 +3,22 @@
 requirements.txt
 setup.cfg
 setup.py
 src/cheltuieli/__init__.py
 src/cheltuieli/chelt_plan.py
 src/cheltuieli/chelt_real.py
 src/cheltuieli/control.py
-src/cheltuieli/gui_desktop.py
+src/cheltuieli/kalendar.py
 src/cheltuieli/masina.py
 src/cheltuieli/plan_vs_real.py
-src/cheltuieli/salariu_prime.py
 src/cheltuieli.egg-info/PKG-INFO
 src/cheltuieli.egg-info/SOURCES.txt
 src/cheltuieli.egg-info/dependency_links.txt
 src/cheltuieli.egg-info/requires.txt
 src/cheltuieli.egg-info/top_level.txt
 src/cheltuieli/GUI/2del_check_expiration.ui
 src/cheltuieli/GUI/chelt_plan.ui
 src/cheltuieli/GUI/chelt_real.ui
 src/cheltuieli/GUI/filterWindow.ui
 src/cheltuieli/GUI/plan_vs_real.ui
-src/cheltuieli/SQL/aeroclub.sql
-src/cheltuieli/SQL/alimentari.sql
-src/cheltuieli/SQL/apartament.sql
-src/cheltuieli/SQL/asigurari.sql
-src/cheltuieli/SQL/banca.sql
-src/cheltuieli/SQL/expenses.sql
-src/cheltuieli/SQL/income.sql
-src/cheltuieli/SQL/intercontotrans.sql
-src/cheltuieli/SQL/one_time_transactions.sql
-src/cheltuieli/SQL/stat.sql
+src/cheltuieli/SQL/cheltuieli_desktop.sql
+src/cheltuieli/static/taxes.csv
```

