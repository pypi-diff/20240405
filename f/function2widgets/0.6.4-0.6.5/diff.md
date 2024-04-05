# Comparing `tmp/function2widgets-0.6.4.tar.gz` & `tmp/function2widgets-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function2widgets-0.6.4.tar", max compression
+gzip compressed data, was "function2widgets-0.6.5.tar", max compression
```

## Comparing `function2widgets-0.6.4.tar` & `function2widgets-0.6.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.4/function2widgets/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-02 11:05:09.916571 function2widgets-0.6.4/function2widgets/common.py
--rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.4/function2widgets/factory.py
--rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.4/function2widgets/info.py
--rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.4/function2widgets/parser/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.4/function2widgets/parser/docstr_parser.py
--rw-r--r--   0        0        0     6513 2024-04-02 10:48:44.584355 function2widgets-0.6.4/function2widgets/parser/function_parser.py
--rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.4/function2widgets/parser/parameter_parser.py
--rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.4/function2widgets/parser/widgetconfigs_parser.py
--rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.4/function2widgets/widget.py
--rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.4/function2widgets/widgets/__init__.py
--rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.4/function2widgets/widgets/_sourcecodeedit.py
--rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.4/function2widgets/widgets/allwidgets.py
--rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.4/function2widgets/widgets/base.py
--rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.4/function2widgets/widgets/editor/__init__.py
--rw-r--r--   0        0        0     6061 2024-04-05 05:18:47.514607 function2widgets-0.6.4/function2widgets/widgets/editor/base.py
--rw-r--r--   0        0        0     2024 2024-04-05 05:17:03.984199 function2widgets-0.6.4/function2widgets/widgets/editor/codeeditor.py
--rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.4/function2widgets/widgets/editor/dicteditor.py
--rw-r--r--   0        0        0     4654 2024-04-05 05:20:20.545687 function2widgets-0.6.4/function2widgets/widgets/editor/jsoneditor.py
--rw-r--r--   0        0        0     1245 2024-04-05 05:16:06.955595 function2widgets-0.6.4/function2widgets/widgets/editor/listeditor.py
--rw-r--r--   0        0        0     1602 2024-03-31 08:24:42.438534 function2widgets-0.6.4/function2widgets/widgets/editor/tupleeditor.py
--rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.4/function2widgets/widgets/lineedit/__init__.py
--rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.4/function2widgets/widgets/lineedit/floatedit.py
--rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.4/function2widgets/widgets/lineedit/intedit.py
--rw-r--r--   0        0        0     2897 2024-03-31 08:24:42.441427 function2widgets-0.6.4/function2widgets/widgets/lineedit/stredit.py
--rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.4/function2widgets/widgets/misc/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.4/function2widgets/widgets/misc/coloredit.py
--rw-r--r--   0        0        0     3459 2024-04-02 11:35:30.993072 function2widgets-0.6.4/function2widgets/widgets/misc/dateedit.py
--rw-r--r--   0        0        0     4091 2024-04-02 11:33:20.900442 function2widgets-0.6.4/function2widgets/widgets/misc/datetimeedit.py
--rw-r--r--   0        0        0     3340 2024-04-02 11:27:28.576112 function2widgets-0.6.4/function2widgets/widgets/misc/timeedit.py
--rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.4/function2widgets/widgets/numberinput/__init__.py
--rw-r--r--   0        0        0     4498 2024-03-31 08:24:42.445444 function2widgets-0.6.4/function2widgets/widgets/numberinput/dial.py
--rw-r--r--   0        0        0     2852 2024-03-31 08:24:42.446444 function2widgets-0.6.4/function2widgets/widgets/numberinput/floatspin.py
--rw-r--r--   0        0        0     2591 2024-03-31 08:24:42.446444 function2widgets-0.6.4/function2widgets/widgets/numberinput/intspin.py
--rw-r--r--   0        0        0     4957 2024-03-31 08:24:42.447443 function2widgets-0.6.4/function2widgets/widgets/numberinput/slider.py
--rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.4/function2widgets/widgets/pathedit/__init__.py
--rw-r--r--   0        0        0     6027 2024-03-31 08:24:42.448967 function2widgets-0.6.4/function2widgets/widgets/pathedit/base.py
--rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.4/function2widgets/widgets/pathedit/dirpathedit.py
--rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.4/function2widgets/widgets/pathedit/filepathedit.py
--rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.4/function2widgets/widgets/selectwidget/__init__.py
--rw-r--r--   0        0        0     1640 2024-03-31 08:24:42.450995 function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox.py
--rw-r--r--   0        0        0     2761 2024-03-31 08:24:42.451979 function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox_group.py
--rw-r--r--   0        0        0     2923 2024-03-31 08:24:42.452993 function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox.py
--rw-r--r--   0        0        0     2205 2024-03-31 08:24:42.452993 function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox_edit.py
--rw-r--r--   0        0        0     3507 2024-03-31 08:24:42.454138 function2widgets-0.6.4/function2widgets/widgets/selectwidget/radiobutton_group.py
--rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.4/function2widgets/widgets/textedit/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.4/function2widgets/widgets/textedit/codeedit.py
--rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.4/function2widgets/widgets/textedit/plaintext.py
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.4/License
--rw-r--r--   0        0        0      714 2024-04-05 05:20:59.638337 function2widgets-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.4/README.md
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.5/function2widgets/__init__.py
+-rw-r--r--   0        0        0     3030 2024-04-02 11:05:09.916571 function2widgets-0.6.5/function2widgets/common.py
+-rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.5/function2widgets/factory.py
+-rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.5/function2widgets/info.py
+-rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.5/function2widgets/parser/__init__.py
+-rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.5/function2widgets/parser/docstr_parser.py
+-rw-r--r--   0        0        0     6513 2024-04-02 10:48:44.584355 function2widgets-0.6.5/function2widgets/parser/function_parser.py
+-rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.5/function2widgets/parser/parameter_parser.py
+-rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.5/function2widgets/parser/widgetconfigs_parser.py
+-rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.5/function2widgets/widget.py
+-rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.5/function2widgets/widgets/__init__.py
+-rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.5/function2widgets/widgets/_sourcecodeedit.py
+-rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.5/function2widgets/widgets/allwidgets.py
+-rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.5/function2widgets/widgets/base.py
+-rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.5/function2widgets/widgets/editor/__init__.py
+-rw-r--r--   0        0        0     6061 2024-04-05 05:18:47.514607 function2widgets-0.6.5/function2widgets/widgets/editor/base.py
+-rw-r--r--   0        0        0     2024 2024-04-05 05:17:03.984199 function2widgets-0.6.5/function2widgets/widgets/editor/codeeditor.py
+-rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.5/function2widgets/widgets/editor/dicteditor.py
+-rw-r--r--   0        0        0     4654 2024-04-05 05:20:20.545687 function2widgets-0.6.5/function2widgets/widgets/editor/jsoneditor.py
+-rw-r--r--   0        0        0     1245 2024-04-05 05:16:06.955595 function2widgets-0.6.5/function2widgets/widgets/editor/listeditor.py
+-rw-r--r--   0        0        0     1621 2024-04-05 08:35:32.821279 function2widgets-0.6.5/function2widgets/widgets/editor/tupleeditor.py
+-rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.5/function2widgets/widgets/lineedit/__init__.py
+-rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.5/function2widgets/widgets/lineedit/floatedit.py
+-rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.5/function2widgets/widgets/lineedit/intedit.py
+-rw-r--r--   0        0        0     3131 2024-04-05 08:44:44.617036 function2widgets-0.6.5/function2widgets/widgets/lineedit/stredit.py
+-rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.5/function2widgets/widgets/misc/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.5/function2widgets/widgets/misc/coloredit.py
+-rw-r--r--   0        0        0     3522 2024-04-05 08:39:38.679633 function2widgets-0.6.5/function2widgets/widgets/misc/dateedit.py
+-rw-r--r--   0        0        0     4070 2024-04-05 08:40:13.233230 function2widgets-0.6.5/function2widgets/widgets/misc/datetimeedit.py
+-rw-r--r--   0        0        0     3403 2024-04-05 08:40:44.115431 function2widgets-0.6.5/function2widgets/widgets/misc/timeedit.py
+-rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.5/function2widgets/widgets/numberinput/__init__.py
+-rw-r--r--   0        0        0     4693 2024-04-05 08:46:13.101173 function2widgets-0.6.5/function2widgets/widgets/numberinput/dial.py
+-rw-r--r--   0        0        0     3126 2024-04-05 08:48:36.095832 function2widgets-0.6.5/function2widgets/widgets/numberinput/floatspin.py
+-rw-r--r--   0        0        0     2788 2024-04-05 08:49:10.364397 function2widgets-0.6.5/function2widgets/widgets/numberinput/intspin.py
+-rw-r--r--   0        0        0     5162 2024-04-05 08:50:37.670447 function2widgets-0.6.5/function2widgets/widgets/numberinput/slider.py
+-rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.5/function2widgets/widgets/pathedit/__init__.py
+-rw-r--r--   0        0        0     6222 2024-04-05 08:52:36.809553 function2widgets-0.6.5/function2widgets/widgets/pathedit/base.py
+-rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.5/function2widgets/widgets/pathedit/dirpathedit.py
+-rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.5/function2widgets/widgets/pathedit/filepathedit.py
+-rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.5/function2widgets/widgets/selectwidget/__init__.py
+-rw-r--r--   0        0        0     1953 2024-04-05 08:56:12.887209 function2widgets-0.6.5/function2widgets/widgets/selectwidget/checkbox.py
+-rw-r--r--   0        0        0     2823 2024-04-05 08:58:14.255857 function2widgets-0.6.5/function2widgets/widgets/selectwidget/checkbox_group.py
+-rw-r--r--   0        0        0     2985 2024-04-05 08:58:25.987503 function2widgets-0.6.5/function2widgets/widgets/selectwidget/combobox.py
+-rw-r--r--   0        0        0     2268 2024-04-05 08:58:38.649153 function2widgets-0.6.5/function2widgets/widgets/selectwidget/combobox_edit.py
+-rw-r--r--   0        0        0     3569 2024-04-05 08:59:23.433045 function2widgets-0.6.5/function2widgets/widgets/selectwidget/radiobutton_group.py
+-rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.5/function2widgets/widgets/textedit/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.5/function2widgets/widgets/textedit/codeedit.py
+-rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.5/function2widgets/widgets/textedit/plaintext.py
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.5/License
+-rw-r--r--   0        0        0      714 2024-04-05 09:00:53.592701 function2widgets-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.5/README.md
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.5/PKG-INFO
```

### Comparing `function2widgets-0.6.4/function2widgets/common.py` & `function2widgets-0.6.5/function2widgets/common.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/factory.py` & `function2widgets-0.6.5/function2widgets/factory.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/info.py` & `function2widgets-0.6.5/function2widgets/info.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/parser/docstr_parser.py` & `function2widgets-0.6.5/function2widgets/parser/docstr_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/parser/function_parser.py` & `function2widgets-0.6.5/function2widgets/parser/function_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/parser/parameter_parser.py` & `function2widgets-0.6.5/function2widgets/parser/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/parser/widgetconfigs_parser.py` & `function2widgets-0.6.5/function2widgets/parser/widgetconfigs_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widget.py` & `function2widgets-0.6.5/function2widgets/widget.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/_sourcecodeedit.py` & `function2widgets-0.6.5/function2widgets/widgets/_sourcecodeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/allwidgets.py` & `function2widgets-0.6.5/function2widgets/widgets/allwidgets.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/base.py` & `function2widgets-0.6.5/function2widgets/widgets/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/base.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/codeeditor.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/codeeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/dicteditor.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/dicteditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/jsoneditor.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/jsoneditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/listeditor.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/listeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/editor/tupleeditor.py` & `function2widgets-0.6.5/function2widgets/widgets/editor/tupleeditor.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 
 class TupleEditor(JsonEditor):
     HIDE_DEFAULT_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = TupleEditorArgs
 
-    TYPE_RESTRICTIONS = (list, tuple, _NoneType)
+    TYPE_RESTRICTIONS = (list, set, tuple, _NoneType)
 
     def __init__(self, args: TupleEditorArgs, parent: Optional[QWidget] = None):
         args = dataclasses.replace(args, top_level_types=self.TYPE_RESTRICTIONS)
 
         super().__init__(args=args, parent=parent)
 
     @property
     def _args(self) -> TupleEditorArgs:
         return cast(TupleEditorArgs, super()._args)
 
     def set_value(self, value: Optional[tuple]):
-        if isinstance(value, list):
+        if isinstance(value, (list, set)):
             value = tuple(value)
         super().set_value(value)
 
     def get_value(self) -> Optional[tuple]:
         value = super().get_value()
         if value is None:
             return None
-        elif isinstance(value, list):
+        elif isinstance(value, (list, set)):
             return tuple(value)
         elif isinstance(value, tuple):
             return value
         else:
             raise ValueError(
                 f"value '{value}' is not one of the following types: {self._args.top_level_types}"
             )
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/lineedit/floatedit.py` & `function2widgets-0.6.5/function2widgets/widgets/lineedit/floatedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/lineedit/intedit.py` & `function2widgets-0.6.5/function2widgets/widgets/lineedit/intedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/lineedit/stredit.py` & `function2widgets-0.6.5/function2widgets/widgets/lineedit/stredit.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,18 +41,26 @@
         super().__init__(args=args, parent=parent)
 
         self._setup_value_widget()
 
         if self._args.set_default_on_init:
             self.set_value(self._args.default)
 
-    def set_value_to_widget(self, value: Any):
+    def get_value(self) -> str:
+        return super().get_value()
+
+    def set_value(self, value: Any):
+        if not isinstance(value, str) and value is not None:
+            value = str(value)
+        super().set_value(value)
+
+    def set_value_to_widget(self, value: str):
         if value is None:
             value = ""
-        self._value_widget.setText(str(value))
+        self._value_widget.setText(value)
 
     def get_value_from_widget(self) -> str:
         return self._value_widget.text()
 
     @property
     def _args(self) -> LineEditArgs:
         return cast(LineEditArgs, super()._args)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/misc/dateedit.py` & `function2widgets-0.6.5/function2widgets/widgets/misc/dateedit.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime, date
 from typing import Optional, cast, Union
 
 from PyQt6.QtCore import Qt, QDate
 from PyQt6.QtWidgets import QWidget, QVBoxLayout, QDateEdit
 
 from function2widgets.common import to_date
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 from function2widgets.widgets.misc.datetimeedit import DEFAULT_TIME_SPEC, TIME_SPECS
 
 DEFAULT_DISPLAY_FORMAT = "yyyy/M/d"
@@ -74,15 +75,15 @@
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
         center_widget_layout.addWidget(self._value_widget)
 
     def set_value(self, value: Union[date, QDate, None]):
         if not isinstance(value, (date, QDate, str)) and value is not None:
-            raise TypeError(
+            raise InvalidValueError(
                 f"value must be date or QDate or a date string, got {type(value)}"
             )
         display_format = self._args.display_format or DEFAULT_DISPLAY_FORMAT
         if isinstance(value, str):
             value = to_date(value, display_format)
         super().set_value(value)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/misc/datetimeedit.py` & `function2widgets-0.6.5/function2widgets/widgets/misc/datetimeedit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 from datetime import datetime
 from typing import Optional, cast, Union
 
 from PyQt6.QtCore import Qt, QDateTime
 from PyQt6.QtWidgets import QWidget, QDateTimeEdit, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 from function2widgets.common import to_datetime
 
 DEFAULT_DISPLAY_FORMAT = "yyyy/M/d H:mm"
@@ -88,19 +89,17 @@
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
         center_widget_layout.addWidget(self._value_widget)
 
     def set_value(self, value: Union[datetime, QDateTime, None]):
         if not isinstance(value, (datetime, QDateTime, str)) and value is not None:
-            raise TypeError(
+            raise InvalidValueError(
                 f"value must be datetime or QDateTime or a datetime string, got {type(value)}"
             )
-        # if isinstance(value, datetime):
-        #     value = QDateTime(value)d
         display_format = self._args.display_format or DEFAULT_DISPLAY_FORMAT
         if isinstance(value, str):
             value = to_datetime(value, display_format)
         super().set_value(value)
 
     def get_value(self) -> Optional[datetime]:
         return super().get_value()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/misc/timeedit.py` & `function2widgets-0.6.5/function2widgets/widgets/misc/timeedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime, time
 from typing import Optional, cast, Union
 
 from PyQt6.QtCore import Qt, QTime
 from PyQt6.QtWidgets import QWidget, QVBoxLayout, QTimeEdit
 
 from function2widgets.common import to_time
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 from function2widgets.widgets.misc.datetimeedit import DEFAULT_TIME_SPEC, TIME_SPECS
 
 DEFAULT_DISPLAY_FORMAT = "HH:mm"
@@ -71,15 +72,15 @@
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
         center_widget_layout.addWidget(self._value_widget)
 
     def set_value(self, value: Union[time, QTime, None]):
         if not isinstance(value, (time, QTime, str)) and value is not None:
-            raise TypeError(
+            raise InvalidValueError(
                 f"value must be time or QTime or a time string, got {type(value)}"
             )
         display_format = self._args.display_format or DEFAULT_DISPLAY_FORMAT
         if isinstance(value, str):
             value = to_time(value, display_format)
         super().set_value(value)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/numberinput/dial.py` & `function2widgets-0.6.5/function2widgets/widgets/numberinput/dial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from typing import Optional, cast
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QDial, QLabel, QWidget, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -97,14 +98,16 @@
             self._setup_value_label(center_widget_layout)
             self._update_value_label(self._value_widget.value())
 
     def get_value(self) -> Optional[int]:
         return super().get_value()
 
     def set_value(self, value: Optional[int]):
+        if not isinstance(value, int) and value is not None:
+            raise InvalidValueError(f"value must be int, got {type(value)}")
         super().set_value(value)
 
     def set_value_to_widget(self, value: int):
         self._value_widget.setValue(value)
 
     def get_value_from_widget(self) -> int:
         return self._value_widget.value()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/numberinput/floatspin.py` & `function2widgets-0.6.5/function2widgets/widgets/numberinput/floatspin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, cast
 
 from PyQt6.QtWidgets import QWidget, QDoubleSpinBox, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -73,14 +74,18 @@
             self._value_widget.setDecimals(decimals)
         self._value_widget.setAccelerated(accelerated is True)
 
     def get_value(self) -> Optional[float]:
         return super().get_value()
 
     def set_value(self, value: Optional[float]):
+        if not isinstance(value, (float, int)) and value is not None:
+            raise InvalidValueError(f"value must be a number, not {type(value)}")
+        if value is not None:
+            value = float(value)
         super().set_value(value)
 
     def set_value_to_widget(self, value: float):
         if self._value_widget is not None:
             self._value_widget.setValue(value)
 
     def get_value_from_widget(self) -> float:
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/numberinput/intspin.py` & `function2widgets-0.6.5/function2widgets/widgets/numberinput/intspin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, cast
 
 from PyQt6.QtWidgets import QWidget, QSpinBox, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -67,14 +68,16 @@
         if suffix:
             self._value_widget.setSuffix(suffix)
 
     def get_value(self) -> Optional[int]:
         return super().get_value()
 
     def set_value(self, value: Optional[int]):
+        if not isinstance(value, int) and value is not None:
+            raise InvalidValueError(f"value must be a int, got {type(value)}")
         super().set_value(value)
 
     def set_value_to_widget(self, value: int):
         if value is None:
             self._value_widget.setValue(0)
         else:
             self._value_widget.setValue(value)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/numberinput/slider.py` & `function2widgets-0.6.5/function2widgets/widgets/numberinput/slider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from typing import Optional, cast
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QSlider, QWidget, QLabel, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 TickPosition = {
     "None": QSlider.TickPosition.NoTicks,
@@ -110,14 +111,16 @@
             self._setup_value_label(center_widget_layout)
             self._update_value_label(self._value_widget.value())
 
     def get_value(self) -> Optional[int]:
         return super().get_value()
 
     def set_value(self, value: Optional[int]):
+        if not isinstance(value, int) and value is not None:
+            raise InvalidValueError(f"value must be an int number, got {type(value)}")
         super().set_value(value)
 
     def set_value_to_widget(self, value: int):
         self._value_widget.setValue(value)
 
     def get_value_from_widget(self) -> int:
         return self._value_widget.value()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/pathedit/base.py` & `function2widgets-0.6.5/function2widgets/widgets/pathedit/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     QLineEdit,
     QPushButton,
     QHBoxLayout,
     QFileDialog,
     QApplication,
 )
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 PATH_TYPE_OPEN_FILE = 0
 PATH_TYPE_OPEN_FILES = 1
@@ -87,14 +88,16 @@
         center_widget_layout.setStretch(0, 8)
         center_widget_layout.setStretch(1, 2)
 
     def get_value(self) -> Optional[str]:
         return super().get_value()
 
     def set_value(self, value: Optional[str]):
+        if value is not None and not isinstance(value, str):
+            raise InvalidValueError(f"value must be str, not {type(value)}")
         super().set_value(value)
 
     def set_value_to_widget(self, value: str):
         self._value_widget.setText(value)
 
     def get_value_from_widget(self) -> Any:
         return self._value_widget.text()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/pathedit/dirpathedit.py` & `function2widgets-0.6.5/function2widgets/widgets/pathedit/dirpathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/pathedit/filepathedit.py` & `function2widgets-0.6.5/function2widgets/widgets/pathedit/filepathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox.py` & `function2widgets-0.6.5/function2widgets/widgets/selectwidget/checkbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Optional, cast
+from typing import Optional, cast, Any
 
 from PyQt6.QtWidgets import QWidget, QCheckBox, QApplication, QVBoxLayout
 
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
@@ -43,12 +43,23 @@
 
         center_widget_layout = QVBoxLayout(center_widget)
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
         center_widget_layout.addWidget(self._checkbox)
 
+    def set_value(self, value: Optional[bool]):
+        if value is not None:
+            value = bool(value)
+        super().set_value(value)
+
+    def get_value(self) -> Optional[bool]:
+        ret = super().get_value()
+        if ret is not None:
+            ret = bool(ret)
+        return ret
+
     def set_value_to_widget(self, value: bool):
         self._checkbox.setChecked(value is True)
 
     def get_value_from_widget(self) -> bool:
         return self._checkbox.isChecked()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox_group.py` & `function2widgets-0.6.5/function2widgets/widgets/selectwidget/checkbox_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, List, cast
 
 from PyQt6.QtWidgets import QWidget, QGridLayout, QCheckBox
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -69,13 +70,13 @@
         for checkbox in self._checkbox_buttons:
             if checkbox.text() in value:
                 checkbox.setChecked(True)
             else:
                 checkbox.setChecked(False)
 
     def set_value(self, value: Optional[List[str]]):
-        if value is not None and not isinstance(value, list):
-            raise ValueError(f"value must be a list, got {type(value)}")
+        if not isinstance(value, list) and value is not None:
+            raise InvalidValueError(f"value must be a list, got {type(value)}")
         super().set_value(value)
 
     def get_value(self) -> Optional[List[str]]:
         return super().get_value()
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox.py` & `function2widgets-0.6.5/function2widgets/widgets/selectwidget/combobox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, List, Union, Tuple, cast, Any
 
 from PyQt6.QtWidgets import QWidget, QComboBox, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -64,15 +65,15 @@
         center_widget.setLayout(center_widget_layout)
 
     def get_value(self) -> Any:
         return super().get_value()
 
     def set_value(self, value: Optional[str]):
         if value is not None and value not in self._items_with_data.keys():
-            raise ValueError(f"value {value} is not in items")
+            raise InvalidValueError(f"value {value} is not in items")
         super().set_value(value)
 
     def set_value_to_widget(self, value: Optional[str]):
         if value is None:
             self._value_widget.setCurrentIndex(-1)
         else:
             self._value_widget.setCurrentText(value)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox_edit.py` & `function2widgets-0.6.5/function2widgets/widgets/selectwidget/combobox_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, List, cast
 
 from PyQt6.QtWidgets import QWidget, QComboBox, QVBoxLayout
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidgetArgs,
     CommonParameterWidget,
 )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -46,15 +47,15 @@
         center_widget_layout = QVBoxLayout(center_widget)
         center_widget_layout.addWidget(self._value_widget)
         center_widget_layout.setContentsMargins(0, 0, 0, 0)
         center_widget.setLayout(center_widget_layout)
 
     def set_value(self, value: str):
         if value is not None and not isinstance(value, str):
-            raise TypeError(f"value must be str, got {type(value)}")
+            raise InvalidValueError(f"value must be str, got {type(value)}")
         super().set_value(value)
 
     def get_value(self) -> Optional[str]:
         return super().get_value()
 
     def set_value_to_widget(self, value: str):
         if value is None:
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/selectwidget/radiobutton_group.py` & `function2widgets-0.6.5/function2widgets/widgets/selectwidget/radiobutton_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 from typing import Optional, List, cast
 
 from PyQt6.QtWidgets import QWidget, QButtonGroup, QGridLayout, QRadioButton
 
+from function2widgets.widget import InvalidValueError
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
 
 CLEAR_ALL = object()
 
@@ -78,15 +79,15 @@
             self._button_group.setExclusive(False)
             for btn in self._button_group.buttons():
                 btn.setChecked(False)
             self._button_group.setExclusive(True)
             return
 
         if value is not None and value not in self._args.items:
-            raise ValueError(f"value must be one of {self._args.items}")
+            raise InvalidValueError(f"value must be one of {self._args.items}")
         super().set_value(value)
 
     def set_value_to_widget(self, value: str):
         radio_btn = self._get_radio_button(value)
         if radio_btn is None:
             return
         radio_btn.setChecked(True)
```

### Comparing `function2widgets-0.6.4/function2widgets/widgets/textedit/codeedit.py` & `function2widgets-0.6.5/function2widgets/widgets/textedit/codeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/function2widgets/widgets/textedit/plaintext.py` & `function2widgets-0.6.5/function2widgets/widgets/textedit/plaintext.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/License` & `function2widgets-0.6.5/License`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/pyproject.toml` & `function2widgets-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "function2widgets"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 packages = [
     {include="function2widgets"}
 ]
```

### Comparing `function2widgets-0.6.4/README.md` & `function2widgets-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.4/PKG-INFO` & `function2widgets-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function2widgets
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Home-page: https://github.com/zimolab/function2widgets
 License: GPL-3.0
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

