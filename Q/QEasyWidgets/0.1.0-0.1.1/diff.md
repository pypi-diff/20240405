# Comparing `tmp/QEasyWidgets-0.1.0.tar.gz` & `tmp/QEasyWidgets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.1.0.tar", last modified: Mon Apr  1 09:13:20 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.1.1.tar", last modified: Fri Apr  5 06:51:54 2024, max compression
```

## Comparing `QEasyWidgets-0.1.0.tar` & `QEasyWidgets-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.855284 QEasyWidgets-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       80 2024-04-01 09:01:22.000000 QEasyWidgets-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1708 2024-04-01 09:13:20.854284 QEasyWidgets-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.575451 QEasyWidgets-0.1.0/QEasyWidgets/
--rw-rw-rw-   0        0        0    14041 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0     9242 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/QFunctions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.513560 QEasyWidgets-0.1.0/QEasyWidgets/QSS/
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.835332 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/
--rw-rw-rw-   0        0        0      280 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Bar.qss
--rw-rw-rw-   0        0        0      497 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Button.qss
--rw-rw-rw-   0        0        0      760 2024-03-20 06:51:14.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Dialog.qss
--rw-rw-rw-   0        0        0      839 2024-02-02 04:44:20.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Edit.qss
--rw-rw-rw-   0        0        0     1014 2024-02-02 03:21:32.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Player.qss
--rw-rw-rw-   0        0        0     3092 2024-01-06 00:47:13.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Table.qss
--rw-rw-rw-   0        0        0      386 2023-12-18 13:00:14.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Dark/Window.qss
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.851994 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/
--rw-rw-rw-   0        0        0      280 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Bar.qss
--rw-rw-rw-   0        0        0      497 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Button.qss
--rw-rw-rw-   0        0        0      760 2024-03-20 06:50:31.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Dialog.qss
--rw-rw-rw-   0        0        0      839 2024-02-19 13:01:29.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Edit.qss
--rw-rw-rw-   0        0        0     1014 2024-02-02 03:21:06.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Player.qss
--rw-rw-rw-   0        0        0     3092 2024-01-06 00:47:03.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Table.qss
--rw-rw-rw-   0        0        0      386 2023-12-18 12:59:56.000000 QEasyWidgets-0.1.0/QEasyWidgets/QSS/Light/Window.qss
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0   136332 2024-04-01 00:45:35.000000 QEasyWidgets-0.1.0/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    27560 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    23215 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.0/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:13:20.784403 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1708 2024-04-01 09:13:20.000000 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-01 09:13:20.000000 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:13:20.000000 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-01 09:13:20.000000 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 09:13:20.000000 QEasyWidgets-0.1.0/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 09:05:29.000000 QEasyWidgets-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 09:13:20.855284 QEasyWidgets-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1530 2024-04-01 09:05:21.000000 QEasyWidgets-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:51:54.867100 QEasyWidgets-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:10.000000 QEasyWidgets-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:53.000000 QEasyWidgets-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-04-05 06:51:54.865109 QEasyWidgets-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 06:51:54.661600 QEasyWidgets-0.1.1/QEasyWidgets/
+-rw-rw-rw-   0        0        0    14041 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0     9285 2024-04-05 05:12:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0   153579 2024-04-05 03:36:08.000000 QEasyWidgets-0.1.1/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    27560 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    23215 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:05.000000 QEasyWidgets-0.1.1/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:51:54.829200 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-04-05 06:51:54.000000 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-04-05 06:51:54.000000 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 06:51:54.000000 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-05 06:51:54.000000 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 06:51:54.000000 QEasyWidgets-0.1.1/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:06.000000 QEasyWidgets-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:51:54.868097 QEasyWidgets-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-04-05 05:34:53.000000 QEasyWidgets-0.1.1/setup.py
```

### Comparing `QEasyWidgets-0.1.0/LICENSE` & `QEasyWidgets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.0/PKG-INFO` & `QEasyWidgets-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.0
+Version: 0.1.1
+Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
@@ -22,15 +23,15 @@
 </div>
 
 
 ## Description
 
 ### Overview
 
-A simple widget library based on Pyside6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
+A simple widget library based on PySide6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
 PS: The project was meant to be named as 'QSimpleWidgets', but sadly it has been registered.
 
 
 ## Consideration
 
 ### System
```

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.1.1/QEasyWidgets/ComponentsCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.1.1/QEasyWidgets/QFunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union, Optional
 from ctypes import c_int, byref, windll
 from PySide6.QtCore import Qt, QObject, QFile, QRect, QRectF, QSize, Signal, Slot, QPropertyAnimation, QParallelAnimationGroup, QEasingCurve, QUrl
 from PySide6.QtGui import QGuiApplication, QColor, QRgba64, QIcon, QPainter, QDesktopServices
 from PySide6.QtWidgets import *
 
 from .Utils import *
+from .Sources import *
 
 ##############################################################################################################################
 
 class CustomSignals_ComponentsCustomizer(QObject):
     '''
     Set up signals for components
     '''
@@ -40,18 +41,21 @@
 
     Theme: str | None
         Type of theme
     '''
     if Theme not in ('Dark', 'Light'):
         Theme = darkdetect.theme()
 
-    File = QFile(os.path.join(os.path.dirname(os.path.abspath(__file__)), f'QSS/{Theme}/{Widget}.qss'))
+    Prefix = 'QSS'
+    FilePath = f'QSS/{Theme}/{Widget}.qss'
+    File = QFile(Path(f':/{Prefix}').joinpath(FilePath))
     File.open(QFile.ReadOnly | QFile.Text)
     QSS = str(File.readAll(), encoding = 'utf-8')
     File.close()
+
     return QSS
 
 
 def Function_DrawIcon(
     Icon: Union[str, QIcon],
     Painter: QPainter,
     Rect: Union[QRect, QRectF]
```

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.1.1/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/Sources.py` & `QEasyWidgets-0.1.1/QEasyWidgets/Sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,592 @@
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 6.6.2
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
+\x00\x00\x01\xf1\
+T\
+oolButtonBase {\x0d\
+\x0a\x09text-align: ce\
+nter;\x0d\x0a\x09/*color:\
+ rgb(0, 0, 0);*/\
+\x0d\x0a\x09background-co\
+lor: transparent\
+;\x0d\x0a\x09padding-top:\
+ 3px;\x0d\x0a\x09padding-\
+left: 6px;\x0d\x0a\x09pad\
+ding-bottom: 3px\
+;\x0d\x0a\x09padding-righ\
+t: 6px;\x0d\x0a\x09border\
+-width: 1.2px;\x0d\x0a\
+\x09border-radius: \
+6px;\x0d\x0a\x09border-st\
+yle: solid;\x0d\x0a\x09bo\
+rder-color: rgba\
+(201, 210, 222, \
+123);\x0d\x0a}\x0d\x0aToolBu\
+ttonBase:hover {\
+\x0d\x0a\x09border-color:\
+ rgba(201, 210, \
+222, 210);\x0d\x0a}\x0d\x0a\x0d\
+\x0a\x0d\x0aQToolTip {\x0d\x0a \
+   color: rgb(21\
+0, 222, 234);\x0d\x0a \
+   background-co\
+lor: transparent\
+;\x0d\x0a\x09border-width\
+: 0px;\x0d\x0a\x09border-\
+style: solid;\x0d\x0a}\
+\
+\x00\x00\x01\x18\
+Q\
+Widget {\x0d\x0a    ba\
+ckground-color: \
+qlineargradient(\
+spread: pad, x1:\
+0, y1:0, x2:0, y\
+2:1, stop:0 rgba\
+(51, 51, 51, 246\
+), stop:1 rgba(4\
+8, 48, 48, 246))\
+;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolT\
+ip {\x0d\x0a    color:\
+ rgb(210, 222, 2\
+34);\x0d\x0a    backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-style: so\
+lid;\x0d\x0a}\
+\x00\x00\x01\x82\
+Q\
+Widget {\x0d\x0a    co\
+lor: rgb(210, 22\
+2, 234);\x0d\x0a}\x0d\x0a\x0d\x0aQ\
+Widget#CentralWi\
+dget {\x0d\x0a    back\
+ground-color: ql\
+ineargradient(sp\
+read: pad, x1:0,\
+ y1:0, x2:0, y2:\
+1, stop:0 rgba(5\
+1, 51, 51, 246),\
+ stop:1 rgba(21,\
+ 21, 21, 246));\x0d\
+\x0a\x09border-width: \
+0px;\x0d\x0a\x09border-st\
+yle: solid;\x0d\x0a}\x0d\x0a\
+\x0d\x0a\x0d\x0aQToolTip {\x0d\x0a\
+    color: rgb(2\
+10, 222, 234);\x0d\x0a\
+    background-c\
+olor: transparen\
+t;\x0d\x0a\x09border-widt\
+h: 0px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+}\
+\x00\x00\x03G\
+L\
+ineEditBase {\x0d\x0a \
+   background-co\
+lor: transparent\
+;\x0d\x0a    padding: \
+0px;\x0d\x0a    border\
+-width: 1.2px;\x0d\x0a\
+    border-radiu\
+s: 6px;\x0d\x0a    bor\
+der-style: solid\
+;\x0d\x0a    border-co\
+lor: rgba(201, 2\
+10, 222, 123);\x0d\x0a\
+}\x0d\x0aLineEditBase:\
+hover {\x0d\x0a    bor\
+der-color: rgba(\
+201, 210, 222, 2\
+10);\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aLin\
+eEditBase QLineE\
+dit {\x0d\x0a\x09backgrou\
+nd-color: transp\
+arent;\x0d\x0a\x09padding\
+-top: 3px;\x0d\x0a\x09pad\
+ding-left: 6px;\x0d\
+\x0a\x09padding-bottom\
+: 3px;\x0d\x0a\x09padding\
+-right: 6px;\x0d\x0a\x09b\
+order-width: 0px\
+;\x0d\x0a\x09border-style\
+: solid;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\
+\x0aLineEditBase QP\
+ushButton {\x0d\x0a\x09im\
+age: url(:/Butto\
+n_Icon/Sources/O\
+penedFolder.png)\
+;\x0d\x0a\x09background-c\
+olor: transparen\
+t;\x0d\x0a\x09border-widt\
+h: 0px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+}\x0d\x0aLineEditBase \
+QPushButton:hove\
+r {\x0d\x0a\x09background\
+-color: rgba(201\
+, 210, 222, 33);\
+\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolTi\
+p {\x0d\x0a    color: \
+rgb(210, 222, 23\
+4);\x0d\x0a    backgro\
+und-color: trans\
+parent;\x0d\x0a\x09border\
+-width: 0px;\x0d\x0a\x09b\
+order-style: sol\
+id;\x0d\x0a}\
+\x00\x00\x03\xf6\
+M\
+ediaPlayerBase Q\
+PushButton {\x0d\x0a  \
+  background-col\
+or: transparent;\
+\x0d\x0a    border-wid\
+th: 0px;\x0d\x0a    bo\
+rder-radius: 12p\
+x;\x0d\x0a    border-s\
+tyle: solid;\x0d\x0a}\x0d\
+\x0aMediaPlayerBase\
+ QPushButton:hov\
+er {\x0d\x0a    backgr\
+ound-color: rgba\
+(201, 210, 222, \
+33);\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aMed\
+iaPlayerBase QSl\
+ider::groove:hor\
+izontal {\x0d\x0a\x09heig\
+ht: 1.2px;\x0d\x0a\x09bac\
+kground-color: r\
+gba(201, 210, 22\
+2, 123);\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-radius: 6\
+px;\x0d\x0a\x09border-sty\
+le: solid;\x0d\x0a}\x0d\x0aM\
+ediaPlayerBase Q\
+Slider::groove:h\
+orizontal:hover \
+{\x0d\x0a\x09background-c\
+olor: rgba(201, \
+210, 222, 210);\x0d\
+\x0a}\x0d\x0a\x0d\x0aMediaPlaye\
+rBase QSlider::h\
+andle:horizontal\
+ {\x0d\x0a\x09width: 12px\
+;\x0d\x0a\x09height: 12px\
+;\x0d\x0a\x09background-c\
+olor: rgba(201, \
+210, 222, 210);\x0d\
+\x0a\x09margin-top: -6\
+px;\x0d\x0a\x09margin-bot\
+tom: -6px;\x0d\x0a\x09bor\
+der-width: 1.2px\
+;\x0d\x0a\x09border-radiu\
+s: 6px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+\x09border-color: t\
+ransparent\x0d\x0a}\x0d\x0aM\
+ediaPlayerBase Q\
+Slider::handle:h\
+orizontal:hover \
+{\x0d\x0a\x09background-c\
+olor: rgba(210, \
+222, 234, 234);\x0d\
+\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolTip\
+ {\x0d\x0a    color: r\
+gb(210, 222, 234\
+);\x0d\x0a    backgrou\
+nd-color: transp\
+arent;\x0d\x0a\x09border-\
+width: 0px;\x0d\x0a\x09bo\
+rder-style: soli\
+d;\x0d\x0a}\
+\x00\x00\x02\xf8\
+M\
+essageBoxBase {\x0d\
+\x0a    background-\
+color: rgba(60, \
+60, 60, 240);\x0d\x0a \
+   padding: 0px;\
+\x0d\x0a    border-wid\
+th: 0px;\x0d\x0a    bo\
+rder-radius: 6px\
+;\x0d\x0a    border-st\
+yle: solid;\x0d\x0a}\x0d\x0a\
+\x0d\x0aMessageBoxBase\
+ QLabel {\x0d\x0a    t\
+ext-align: cente\
+r;\x0d\x0a    font-siz\
+e: 9.9pt;\x0d\x0a    c\
+olor: rgb(210, 2\
+22, 234);\x0d\x0a    b\
+ackground-color:\
+ transparent;\x0d\x0a}\
+\x0d\x0a\x0d\x0aMessageBoxBa\
+se QPushButton {\
+\x0d\x0a    text-align\
+: center;\x0d\x0a    f\
+ont-size: 9.9pt;\
+\x0d\x0a    color: rgb\
+(210, 222, 234);\
+\x0d\x0a    background\
+-color: rgba(90,\
+ 90, 90, 120);\x0d\x0a\
+    border-width\
+: 0px;\x0d\x0a    bord\
+er-radius: 6px;\x0d\
+\x0a    border-styl\
+e: solid;\x0d\x0a}\x0d\x0aMe\
+ssageBoxBase QPu\
+shButton:hover {\
+\x0d\x0a    background\
+-color: rgba(120\
+, 120, 120, 120)\
+;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolT\
+ip {\x0d\x0a    color:\
+ rgb(210, 222, 2\
+34);\x0d\x0a    backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-style: so\
+lid;\x0d\x0a}\
+\x00\x00\x02$\
+\x00\
+\x00\x0c\x14x\xda\xd5VMO\xe30\x10=\xa7R\xff\
+\x83\xb9Q\xa9AI`\x9107N\x5c\xd1V\xdc\x9d\
+x6\xb1\xd6\xb5#\xc7\x05vW\xfcw\xec\xb8!\xae\
+\x9b\xa6\x05\x8a\xaa\x8d\xe4\xc8\x8a3\x1f\xef\xcd\xf3\xd8\x0f\
+\xf7@(\xa8G\x06\xcf\xe8\xdft\x82\xcc\x93\x93\xe2w\
+\xa9\xe4J\xd0\xb8\x90\x5c*\x8c\xb4\x22\xa2\xa9\x89\x02\xa1\
+o\xa7\x93\xd7\xe9d:y\xe8\xed0n\xa0\xd0L\x0a\
+\xeb \xd2\xf0\xa2c\xc2Y)0\xe2\xf0\xcb\x1aD\xfb\
+<\xb6Q\xa52\xfe\xe2gFu\x85Qz\x91\xd5/\
+\xad\xa9\xfb\xdc\xe8?\x1c0j$g\xd4\xfb\xbc\xf6\xa6\
+\xca\x9c\x9cgI:GY\x9a\x98W\x96\xcdQ\x9a]\
+\xce\xbadM\xba\x0b\x92s\xe8P~:I\xc25(\
+A4\xc4\x87\xfc\xdd\x00w\xc4\x1c\xf4w\xa9\x18\xe5L\
+\xc0\x01\xa0\xa2q\xb2\x14\xa1l\xd5`t}D\x0a{\
+\x021f\x1a\x96\xefbq^\xb4\xac\xbbl\x926\xaa\
+\xb7\xa6XY\xe9\xcd\xd5.x.\xb5\x96\xcb\x10\x87g\
+k\x8b3l\xfa\x158!\x18\xab`[*\xa0\xad:\
+\xf6\xbb2\xb3]\xae\xce\xde5\x82\xcf|\xaf\x16T/\
+\xc7\x9f\x85\x92\x9c\xdf\x11\x85\xf1\x13(\xcd\x0a\xc2\xdb\xd0\
+k\xa87k\xa8[\xb21\xc9\x9c_\xfd\x98#7\x86\
+\xb4\xf0e%l*3Z\x12U2\xd1\xb1\xff:\x9c\
+;\xae\xa4\x99:\xf2\x06s\xbe6\xcc\xb9\xd1+\xca\xf3\
+C(\x8d\xad\xf67\xc9\xa8\xc0*\xa7/\xfc\x9eM\x14\
+5\xab\xbc\x90B\x1b\xafq-\x1bfw\x1eFNb\
+\xc1\xb24\x9a\xb4\xa0\x1c\xb8m\x16\x93A\x16G\x05\xb8\
+\x85\xc9\x84\xfb.Lf\xb7\x9d\x00\x90-RM\xca\x1e\
+\xd0\x1c\x85x7\x96}A\xaf#}\x10\xfdV\x0a\x15\
+\x11\x94\x07\x11\x86\x05wc\xc4\xe6\xc6\xecXl\x8c$\
+\xb2W\xffi\x96\xd8\x06\xe4^\xfe\xb9\xe4\xfb4E\xfc\
+k\xea\x19(\xe5\x7f\xe9\x05}\xfaG\xeb\x06\x01#A\
+\xf5>\xb5u\xba\xd3\xfeT\xcd\xe0\x1b \xb5\xe7\xeb)\
+\xfbA\x8fiGG\x18\x05}\xa4\x9e\x10\xc48eW\
+\xf8\xc0N\xd8\xd9\x17\x16R\xf2\x05\xab\xbb\x9b\x83g\xe2\
+\xddB.\xaff\xb7\x87\xdd\xd9G\xa1\x86\xa0\xde\x00P\
+\x8a\xd6\xff\
+\x00\x00\x01\xf1\
+T\
+oolButtonBase {\x0d\
+\x0a\x09text-align: ce\
+nter;\x0d\x0a\x09/*color:\
+ rgb(0, 0, 0);*/\
+\x0d\x0a\x09background-co\
+lor: transparent\
+;\x0d\x0a\x09padding-top:\
+ 3px;\x0d\x0a\x09padding-\
+left: 6px;\x0d\x0a\x09pad\
+ding-bottom: 3px\
+;\x0d\x0a\x09padding-righ\
+t: 6px;\x0d\x0a\x09border\
+-width: 1.2px;\x0d\x0a\
+\x09border-radius: \
+6px;\x0d\x0a\x09border-st\
+yle: solid;\x0d\x0a\x09bo\
+rder-color: rgba\
+(201, 210, 222, \
+123);\x0d\x0a}\x0d\x0aToolBu\
+ttonBase:hover {\
+\x0d\x0a\x09border-color:\
+ rgba(201, 210, \
+222, 210);\x0d\x0a}\x0d\x0a\x0d\
+\x0a\x0d\x0aQToolTip {\x0d\x0a \
+   color: rgb(21\
+0, 222, 234);\x0d\x0a \
+   background-co\
+lor: transparent\
+;\x0d\x0a\x09border-width\
+: 0px;\x0d\x0a\x09border-\
+style: solid;\x0d\x0a}\
+\
+\x00\x00\x01\x18\
+Q\
+Widget {\x0d\x0a    ba\
+ckground-color: \
+qlineargradient(\
+spread: pad, x1:\
+0, y1:0, x2:0, y\
+2:1, stop:0 rgba\
+(51, 51, 51, 246\
+), stop:1 rgba(4\
+8, 48, 48, 246))\
+;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolT\
+ip {\x0d\x0a    color:\
+ rgb(210, 222, 2\
+34);\x0d\x0a    backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-style: so\
+lid;\x0d\x0a}\
+\x00\x00\x01\x82\
+Q\
+Widget {\x0d\x0a    co\
+lor: rgb(210, 22\
+2, 234);\x0d\x0a}\x0d\x0a\x0d\x0aQ\
+Widget#CentralWi\
+dget {\x0d\x0a    back\
+ground-color: ql\
+ineargradient(sp\
+read: pad, x1:0,\
+ y1:0, x2:0, y2:\
+1, stop:0 rgba(5\
+1, 51, 51, 246),\
+ stop:1 rgba(21,\
+ 21, 21, 246));\x0d\
+\x0a\x09border-width: \
+0px;\x0d\x0a\x09border-st\
+yle: solid;\x0d\x0a}\x0d\x0a\
+\x0d\x0a\x0d\x0aQToolTip {\x0d\x0a\
+    color: rgb(2\
+10, 222, 234);\x0d\x0a\
+    background-c\
+olor: transparen\
+t;\x0d\x0a\x09border-widt\
+h: 0px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+}\
+\x00\x00\x03G\
+L\
+ineEditBase {\x0d\x0a \
+   background-co\
+lor: transparent\
+;\x0d\x0a    padding: \
+0px;\x0d\x0a    border\
+-width: 1.2px;\x0d\x0a\
+    border-radiu\
+s: 6px;\x0d\x0a    bor\
+der-style: solid\
+;\x0d\x0a    border-co\
+lor: rgba(201, 2\
+10, 222, 123);\x0d\x0a\
+}\x0d\x0aLineEditBase:\
+hover {\x0d\x0a    bor\
+der-color: rgba(\
+201, 210, 222, 2\
+10);\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aLin\
+eEditBase QLineE\
+dit {\x0d\x0a\x09backgrou\
+nd-color: transp\
+arent;\x0d\x0a\x09padding\
+-top: 3px;\x0d\x0a\x09pad\
+ding-left: 6px;\x0d\
+\x0a\x09padding-bottom\
+: 3px;\x0d\x0a\x09padding\
+-right: 6px;\x0d\x0a\x09b\
+order-width: 0px\
+;\x0d\x0a\x09border-style\
+: solid;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\
+\x0aLineEditBase QP\
+ushButton {\x0d\x0a\x09im\
+age: url(:/Butto\
+n_Icon/Sources/O\
+penedFolder.png)\
+;\x0d\x0a\x09background-c\
+olor: transparen\
+t;\x0d\x0a\x09border-widt\
+h: 0px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+}\x0d\x0aLineEditBase \
+QPushButton:hove\
+r {\x0d\x0a\x09background\
+-color: rgba(201\
+, 210, 222, 33);\
+\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolTi\
+p {\x0d\x0a    color: \
+rgb(210, 222, 23\
+4);\x0d\x0a    backgro\
+und-color: trans\
+parent;\x0d\x0a\x09border\
+-width: 0px;\x0d\x0a\x09b\
+order-style: sol\
+id;\x0d\x0a}\
+\x00\x00\x03\xf6\
+M\
+ediaPlayerBase Q\
+PushButton {\x0d\x0a  \
+  background-col\
+or: transparent;\
+\x0d\x0a    border-wid\
+th: 0px;\x0d\x0a    bo\
+rder-radius: 12p\
+x;\x0d\x0a    border-s\
+tyle: solid;\x0d\x0a}\x0d\
+\x0aMediaPlayerBase\
+ QPushButton:hov\
+er {\x0d\x0a    backgr\
+ound-color: rgba\
+(201, 210, 222, \
+33);\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aMed\
+iaPlayerBase QSl\
+ider::groove:hor\
+izontal {\x0d\x0a\x09heig\
+ht: 1.2px;\x0d\x0a\x09bac\
+kground-color: r\
+gba(201, 210, 22\
+2, 123);\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-radius: 6\
+px;\x0d\x0a\x09border-sty\
+le: solid;\x0d\x0a}\x0d\x0aM\
+ediaPlayerBase Q\
+Slider::groove:h\
+orizontal:hover \
+{\x0d\x0a\x09background-c\
+olor: rgba(201, \
+210, 222, 210);\x0d\
+\x0a}\x0d\x0a\x0d\x0aMediaPlaye\
+rBase QSlider::h\
+andle:horizontal\
+ {\x0d\x0a\x09width: 12px\
+;\x0d\x0a\x09height: 12px\
+;\x0d\x0a\x09background-c\
+olor: rgba(201, \
+210, 222, 210);\x0d\
+\x0a\x09margin-top: -6\
+px;\x0d\x0a\x09margin-bot\
+tom: -6px;\x0d\x0a\x09bor\
+der-width: 1.2px\
+;\x0d\x0a\x09border-radiu\
+s: 6px;\x0d\x0a\x09border\
+-style: solid;\x0d\x0a\
+\x09border-color: t\
+ransparent\x0d\x0a}\x0d\x0aM\
+ediaPlayerBase Q\
+Slider::handle:h\
+orizontal:hover \
+{\x0d\x0a\x09background-c\
+olor: rgba(210, \
+222, 234, 234);\x0d\
+\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolTip\
+ {\x0d\x0a    color: r\
+gb(210, 222, 234\
+);\x0d\x0a    backgrou\
+nd-color: transp\
+arent;\x0d\x0a\x09border-\
+width: 0px;\x0d\x0a\x09bo\
+rder-style: soli\
+d;\x0d\x0a}\
+\x00\x00\x02\xf8\
+M\
+essageBoxBase {\x0d\
+\x0a    background-\
+color: rgba(60, \
+60, 60, 240);\x0d\x0a \
+   padding: 0px;\
+\x0d\x0a    border-wid\
+th: 0px;\x0d\x0a    bo\
+rder-radius: 6px\
+;\x0d\x0a    border-st\
+yle: solid;\x0d\x0a}\x0d\x0a\
+\x0d\x0aMessageBoxBase\
+ QLabel {\x0d\x0a    t\
+ext-align: cente\
+r;\x0d\x0a    font-siz\
+e: 9.9pt;\x0d\x0a    c\
+olor: rgb(210, 2\
+22, 234);\x0d\x0a    b\
+ackground-color:\
+ transparent;\x0d\x0a}\
+\x0d\x0a\x0d\x0aMessageBoxBa\
+se QPushButton {\
+\x0d\x0a    text-align\
+: center;\x0d\x0a    f\
+ont-size: 9.9pt;\
+\x0d\x0a    color: rgb\
+(210, 222, 234);\
+\x0d\x0a    background\
+-color: rgba(90,\
+ 90, 90, 120);\x0d\x0a\
+    border-width\
+: 0px;\x0d\x0a    bord\
+er-radius: 6px;\x0d\
+\x0a    border-styl\
+e: solid;\x0d\x0a}\x0d\x0aMe\
+ssageBoxBase QPu\
+shButton:hover {\
+\x0d\x0a    background\
+-color: rgba(120\
+, 120, 120, 120)\
+;\x0d\x0a}\x0d\x0a\x0d\x0a\x0d\x0aQToolT\
+ip {\x0d\x0a    color:\
+ rgb(210, 222, 2\
+34);\x0d\x0a    backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r-width: 0px;\x0d\x0a\x09\
+border-style: so\
+lid;\x0d\x0a}\
+\x00\x00\x02$\
+\x00\
+\x00\x0c\x14x\xda\xd5VMO\xe30\x10=\xa7R\xff\
+\x83\xb9Q\xa9AI`\x9107N\x5c\xd1V\xdc\x9d\
+x6\xb1\xd6\xb5#\xc7\x05vW\xfcw\xec\xb8!\xae\
+\x9b\xa6\x05\x8a\xaa\x8d\xe4\xc8\x8a3\x1f\xef\xcd\xf3\xd8\x0f\
+\xf7@(\xa8G\x06\xcf\xe8\xdft\x82\xcc\x93\x93\xe2w\
+\xa9\xe4J\xd0\xb8\x90\x5c*\x8c\xb4\x22\xa2\xa9\x89\x02\xa1\
+o\xa7\x93\xd7\xe9d:y\xe8\xed0n\xa0\xd0L\x0a\
+\xeb \xd2\xf0\xa2c\xc2Y)0\xe2\xf0\xcb\x1aD\xfb\
+<\xb6Q\xa52\xfe\xe2gFu\x85Qz\x91\xd5/\
+\xad\xa9\xfb\xdc\xe8?\x1c0j$g\xd4\xfb\xbc\xf6\xa6\
+\xca\x9c\x9cgI:GY\x9a\x98W\x96\xcdQ\x9a]\
+\xce\xbadM\xba\x0b\x92s\xe8P~:I\xc25(\
+A4\xc4\x87\xfc\xdd\x00w\xc4\x1c\xf4w\xa9\x18\xe5L\
+\xc0\x01\xa0\xa2q\xb2\x14\xa1l\xd5`t}D\x0a{\
+\x021f\x1a\x96\xefbq^\xb4\xac\xbbl\x926\xaa\
+\xb7\xa6XY\xe9\xcd\xd5.x.\xb5\x96\xcb\x10\x87g\
+k\x8b3l\xfa\x158!\x18\xab`[*\xa0\xad:\
+\xf6\xbb2\xb3]\xae\xce\xde5\x82\xcf|\xaf\x16T/\
+\xc7\x9f\x85\x92\x9c\xdf\x11\x85\xf1\x13(\xcd\x0a\xc2\xdb\xd0\
+k\xa87k\xa8[\xb21\xc9\x9c_\xfd\x98#7\x86\
+\xb4\xf0e%l*3Z\x12U2\xd1\xb1\xff:\x9c\
+;\xae\xa4\x99:\xf2\x06s\xbe6\xcc\xb9\xd1+\xca\xf3\
+C(\x8d\xad\xf67\xc9\xa8\xc0*\xa7/\xfc\x9eM\x14\
+5\xab\xbc\x90B\x1b\xafq-\x1bfw\x1eFNb\
+\xc1\xb24\x9a\xb4\xa0\x1c\xb8m\x16\x93A\x16G\x05\xb8\
+\x85\xc9\x84\xfb.Lf\xb7\x9d\x00\x90-RM\xca\x1e\
+\xd0\x1c\x85x7\x96}A\xaf#}\x10\xfdV\x0a\x15\
+\x11\x94\x07\x11\x86\x05wc\xc4\xe6\xc6\xecXl\x8c$\
+\xb2W\xffi\x96\xd8\x06\xe4^\xfe\xb9\xe4\xfb4E\xfc\
+k\xea\x19(\xe5\x7f\xe9\x05}\xfaG\xeb\x06\x01#A\
+\xf5>\xb5u\xba\xd3\xfeT\xcd\xe0\x1b \xb5\xe7\xeb)\
+\xfbA\x8fiGG\x18\x05}\xa4\x9e\x10\xc48eW\
+\xf8\xc0N\xd8\xd9\x17\x16R\xf2\x05\xab\xbb\x9b\x83g\xe2\
+\xddB.\xaff\xb7\x87\xdd\xd9G\xa1\x86\xa0\xde\x00P\
+\x8a\xd6\xff\
 \x00\x00\x09\x09\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00B\x00\x00\x00B\x08\x06\x00\x00\x00\xe3T\x00\xe8\
 \x00\x00\x00\x09pHYs\x00\x00.#\x00\x00.#\
 \x01x\xa5?v\x00\x00\x072iTXtXML\
 :com.adobe.xmp\x00\x00\
@@ -4946,14 +5524,54 @@
 \x06\xd0q>\
 \x00B\
 \x00u\x00t\x00t\x00o\x00n\x00_\x00I\x00c\x00o\x00n\
 \x00\x0d\
 \x02$\xe0^\
 \x00C\
 \x00o\x00m\x00b\x00o\x00B\x00o\x00x\x00_\x00I\x00c\x00o\x00n\
+\x00\x03\
+\x00\x00V\x83\
+\x00Q\
+\x00S\x00S\
+\x00\x04\
+\x00\x04\xa8\x8b\
+\x00D\
+\x00a\x00r\x00k\
+\x00\x05\
+\x00R\xfd\xf4\
+\x00L\
+\x00i\x00g\x00h\x00t\
+\x00\x0a\
+\x0bha\xc3\
+\x00B\
+\x00u\x00t\x00t\x00o\x00n\x00.\x00q\x00s\x00s\
+\x00\x07\
+\x08\x85X#\
+\x00B\
+\x00a\x00r\x00.\x00q\x00s\x00s\
+\x00\x0a\
+\x0be\x98#\
+\x00W\
+\x00i\x00n\x00d\x00o\x00w\x00.\x00q\x00s\x00s\
+\x00\x08\
+\x0b\x07Q\xc3\
+\x00E\
+\x00d\x00i\x00t\x00.\x00q\x00s\x00s\
+\x00\x0a\
+\x0f\xcf\xbd\xa3\
+\x00P\
+\x00l\x00a\x00y\x00e\x00r\x00.\x00q\x00s\x00s\
+\x00\x0a\
+\x03S\x07\xa3\
+\x00D\
+\x00i\x00a\x00l\x00o\x00g\x00.\x00q\x00s\x00s\
+\x00\x09\
+\x09(\xecC\
+\x00T\
+\x00a\x00b\x00l\x00e\x00.\x00q\x00s\x00s\
 \x00\x07\
 \x0al\x89c\
 \x00S\
 \x00o\x00u\x00r\x00c\x00e\x00s\
 \x00\x0d\
 \x0f\xb6\x07G\
 \x00D\
@@ -5094,106 +5712,142 @@
 \x00\x0d\
 \x0e\x1b\x05g\
 \x00D\
 \x00o\x00w\x00n\x00C\x00a\x00r\x00e\x00t\x00.\x00p\x00n\x00g\
 "
 
 qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x04\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x05\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x01\x00\x00\x00/\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00j\x00\x02\x00\x00\x00\x01\x00\x00\x00+\
+\x00\x00\x00j\x00\x02\x00\x00\x00\x01\x00\x00\x00,\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00$\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00%\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00 \x00\x02\x00\x00\x00\x01\x00\x00\x00!\
+\x00\x00\x00 \x00\x02\x00\x00\x00\x01\x00\x00\x00\x22\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x01\x00\x00\x00\x05\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x01\x00\x00\x00\x06\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x1b\x00\x00\x00\x06\
+\x00\x00\x01^\x00\x02\x00\x00\x00\x1b\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x02\xca\x00\x00\x00\x00\x00\x01\x00\x00\xa8\x5c\
+\x00\x00\x03\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xca\x5c\
 \x00\x00\x01\x8b\xe1\xc9z\xd3\
-\x00\x00\x02`\x00\x00\x00\x00\x00\x01\x00\x00\x89d\
+\x00\x00\x034\x00\x00\x00\x00\x00\x01\x00\x00\xabd\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x02~\x00\x00\x00\x00\x00\x01\x00\x00\x90\xfa\
+\x00\x00\x03R\x00\x00\x00\x00\x00\x01\x00\x00\xb2\xfa\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x12\x16\
+\x00\x00\x01\xae\x00\x00\x00\x00\x00\x01\x00\x004\x16\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x03z\x00\x00\x00\x00\x00\x01\x00\x00\xe1\x1b\
+\x00\x00\x04N\x00\x00\x00\x00\x00\x01\x00\x01\x03\x1b\
 \x00\x00\x01\x8b\xe1\xd1tV\
-\x00\x00\x01\xb6\x00\x00\x00\x00\x00\x01\x00\x00W\xbc\
+\x00\x00\x02\x8a\x00\x00\x00\x00\x00\x01\x00\x00y\xbc\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x01,\x00\x00\x00\x00\x00\x01\x00\x00)\x17\
+\x00\x00\x02\x00\x00\x00\x00\x00\x00\x01\x00\x00K\x17\
 \x00\x00\x01\x8e\x97\x04\xd90\
-\x00\x00\x01B\x00\x00\x00\x00\x00\x01\x00\x000\xfe\
+\x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x00R\xfe\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x01\xf2\x00\x00\x00\x00\x00\x01\x00\x00g\xf6\
+\x00\x00\x02\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x89\xf6\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x01\x16\x00\x00\x00\x00\x00\x01\x00\x00!!\
+\x00\x00\x01\xea\x00\x00\x00\x00\x00\x01\x00\x00C!\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x03d\x00\x00\x00\x00\x00\x01\x00\x00\xd8\xaf\
+\x00\x00\x048\x00\x00\x00\x00\x00\x01\x00\x00\xfa\xaf\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x03H\x00\x00\x00\x00\x00\x01\x00\x00\xd1\x05\
+\x00\x00\x04\x1c\x00\x00\x00\x00\x00\x01\x00\x00\xf3\x05\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x02\x94\x00\x00\x00\x00\x00\x01\x00\x00\x98\xbe\
+\x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x00\xba\xbe\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x01\xda\x00\x00\x00\x00\x00\x01\x00\x00_\xcb\
+\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00\x81\xcb\
 \x00\x00\x01\x8e\x97\x04\xd9(\
-\x00\x00\x01r\x00\x00\x00\x00\x00\x01\x00\x00@\x91\
+\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x00b\x91\
 \x00\x00\x01\x8b\xe1\xcc\xde\x1f\
-\x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x00\xa0a\
+\x00\x00\x03\x8a\x00\x00\x00\x00\x00\x01\x00\x00\xc2a\
 \x00\x00\x01\x8e\x97\x04\xd9!\
-\x00\x00\x030\x00\x00\x00\x00\x00\x01\x00\x00\xc8\xb9\
+\x00\x00\x04\x04\x00\x00\x00\x00\x00\x01\x00\x00\xea\xb9\
 \x00\x00\x01\x8e\x97\x04\xd9!\
-\x00\x00\x02\xf2\x00\x00\x00\x00\x00\x01\x00\x00\xb8q\
+\x00\x00\x03\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xdaq\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x02\x22\x00\x00\x00\x00\x00\x01\x00\x00x\xd8\
+\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9a\xd8\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\x19\xd6\
+\x00\x00\x01\xd4\x00\x00\x00\x00\x00\x01\x00\x00;\xd6\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x01\x88\x00\x00\x00\x00\x00\x01\x00\x00G\xcb\
+\x00\x00\x02\x5c\x00\x00\x00\x00\x00\x01\x00\x00i\xcb\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x02\x0a\x00\x00\x00\x00\x00\x01\x00\x00q\x00\
+\x00\x00\x02\xde\x00\x00\x00\x00\x00\x01\x00\x00\x93\x00\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x01X\x00\x00\x00\x00\x00\x01\x00\x008\xfb\
+\x00\x00\x02,\x00\x00\x00\x00\x00\x01\x00\x00Z\xfb\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x02@\x00\x00\x00\x00\x00\x01\x00\x00\x81\xbb\
+\x00\x00\x03\x14\x00\x00\x00\x00\x00\x01\x00\x00\xa3\xbb\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x02\xda\x00\x00\x00\x00\x00\x01\x00\x00\xb05\
+\x00\x00\x03\xae\x00\x00\x00\x00\x00\x01\x00\x00\xd25\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x01\x9c\x00\x00\x00\x00\x00\x01\x00\x00O\x7f\
+\x00\x00\x02p\x00\x00\x00\x00\x00\x01\x00\x00q\x7f\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x03\x12\x00\x00\x00\x00\x00\x01\x00\x00\xc0\x18\
+\x00\x00\x03\xe6\x00\x00\x00\x00\x00\x01\x00\x00\xe2\x18\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x02\x00\x00\x00\x22\
+\x00\x00\x01^\x00\x02\x00\x00\x00\x02\x00\x00\x00#\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\xbe\x00\x00\x00\x00\x00\x01\x00\x00\xf1\xf1\
+\x00\x00\x01\x92\x00\x00\x00\x00\x00\x01\x00\x01\x13\xf1\
 \x00\x00\x01\x8e\x97\x04\xd90\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xe8\xe4\
+\x00\x00\x01r\x00\x00\x00\x00\x00\x01\x00\x01\x0a\xe4\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x06\x00\x00\x00%\
+\x00\x00\x01^\x00\x02\x00\x00\x00\x06\x00\x00\x00&\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x01\x1cE\
+\x00\x00\x04\xf2\x00\x00\x00\x00\x00\x01\x00\x01>E\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x03\x9c\x00\x00\x00\x00\x00\x01\x00\x00\xfa\xfa\
+\x00\x00\x04p\x00\x00\x00\x00\x00\x01\x00\x01\x1c\xfa\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x01\x13P\
+\x00\x00\x04\xd0\x00\x00\x00\x00\x00\x01\x00\x015P\
 \x00\x00\x01\x8e\x97\x04\xd9-\
-\x00\x00\x03\xe2\x00\x00\x00\x00\x00\x01\x00\x01\x0b\xfc\
+\x00\x00\x04\xb6\x00\x00\x00\x00\x00\x01\x00\x01-\xfc\
 \x00\x00\x01\x8e\x97\x04\xd9.\
-\x00\x00\x03\xba\x00\x00\x00\x00\x00\x01\x00\x01\x04;\
+\x00\x00\x04\x8e\x00\x00\x00\x00\x00\x01\x00\x01&;\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x04>\x00\x00\x00\x00\x00\x01\x00\x01%\xaf\
+\x00\x00\x05\x12\x00\x00\x00\x00\x00\x01\x00\x01G\xaf\
 \x00\x00\x01\x8e\x97\x04\xd9&\
-\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x02\x00\x00\x00,\
+\x00\x00\x01^\x00\x02\x00\x00\x00\x02\x00\x00\x00-\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\xbe\x00\x00\x00\x00\x00\x01\x00\x00\x09\x0d\
+\x00\x00\x01\x92\x00\x00\x00\x00\x00\x01\x00\x00+\x0d\
 \x00\x00\x01\x8e\x97\x04\xd90\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01r\x00\x00\x00\x00\x00\x01\x00\x00\x22\x00\
 \x00\x00\x01\x8e\x97\x04\xd9&\
+\x00\x00\x00\x8a\x00\x02\x00\x00\x00\x02\x00\x00\x000\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x96\x00\x02\x00\x00\x00\x07\x00\x00\x009\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\xa4\x00\x02\x00\x00\x00\x07\x00\x00\x002\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x01,\x00\x00\x00\x00\x00\x01\x00\x00\x0b\xdc\
+\x00\x00\x01\x8eZ\xa0/6\
+\x00\x00\x00\xce\x00\x00\x00\x00\x00\x01\x00\x00\x01\xf5\
+\x00\x00\x01\x8cC\x9b%\xc5\
+\x00\x00\x01F\x00\x01\x00\x00\x00\x01\x00\x00\x0e\xd8\
+\x00\x00\x01\x8c\xdc<\xd6\xe5\
+\x00\x00\x00\xfc\x00\x00\x00\x00\x00\x01\x00\x00\x04\x97\
+\x00\x00\x01\x8d\xc1u\x0a\x02\
+\x00\x00\x00\xe2\x00\x00\x00\x00\x00\x01\x00\x00\x03\x11\
+\x00\x00\x01\x8c}\x02\xfb\x03\
+\x00\x00\x00\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x8cC\x9b%\xc5\
+\x00\x00\x01\x12\x00\x00\x00\x00\x00\x01\x00\x00\x07\xe2\
+\x00\x00\x01\x8dg\xd5\x94\x0b\
+\x00\x00\x01,\x00\x00\x00\x00\x00\x01\x00\x00\x1c\xdc\
+\x00\x00\x01\x8eZ\xa0\xd9\xd4\
+\x00\x00\x00\xce\x00\x00\x00\x00\x00\x01\x00\x00\x12\xf5\
+\x00\x00\x01\x8cC\x9b%\xc3\
+\x00\x00\x01F\x00\x01\x00\x00\x00\x01\x00\x00\x1f\xd8\
+\x00\x00\x01\x8c\xdc<\xfc_\
+\x00\x00\x00\xfc\x00\x00\x00\x00\x00\x01\x00\x00\x15\x97\
+\x00\x00\x01\x8dh!\xc6\x87\
+\x00\x00\x00\xe2\x00\x00\x00\x00\x00\x01\x00\x00\x14\x11\
+\x00\x00\x01\x8c}\x03A\x88\
+\x00\x00\x00\xb4\x00\x00\x00\x00\x00\x01\x00\x00\x11\x00\
+\x00\x00\x01\x8cC\x9b%\xc3\
+\x00\x00\x01\x12\x00\x00\x00\x00\x00\x01\x00\x00\x18\xe2\
+\x00\x00\x01\x8dg\xd5\xf6\xf1\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/Utils.py` & `QEasyWidgets-0.1.1/QEasyWidgets/Utils.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.1.1/QEasyWidgets/WindowCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.0/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.1.1/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.0
+Version: 0.1.1
+Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
@@ -22,15 +23,15 @@
 </div>
 
 
 ## Description
 
 ### Overview
 
-A simple widget library based on Pyside6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
+A simple widget library based on PySide6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
 PS: The project was meant to be named as 'QSimpleWidgets', but sadly it has been registered.
 
 
 ## Consideration
 
 ### System
```

### Comparing `QEasyWidgets-0.1.0/README.md` & `QEasyWidgets-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 </div>
 
 
 ## Description
 
 ### Overview
 
-A simple widget library based on Pyside6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
+A simple widget library based on PySide6, which is currently used to serve for [Easy Voice Toolkit](https://github.com/Spr-Aachen/Easy-Voice-Toolkit).
 PS: The project was meant to be named as 'QSimpleWidgets', but sadly it has been registered.
 
 
 ## Consideration
 
 ### System
```

### Comparing `QEasyWidgets-0.1.0/setup.py` & `QEasyWidgets-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.1.0',
-    description = '',
+    version = '0.1.1',
+    description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
     project_urls = {
```

