# Comparing `tmp/function2widgets-0.6.3.tar.gz` & `tmp/function2widgets-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function2widgets-0.6.3.tar", max compression
+gzip compressed data, was "function2widgets-0.6.4.tar", max compression
```

## Comparing `function2widgets-0.6.3.tar` & `function2widgets-0.6.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.3/function2widgets/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-02 11:05:09.916571 function2widgets-0.6.3/function2widgets/common.py
--rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.3/function2widgets/factory.py
--rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.3/function2widgets/info.py
--rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.3/function2widgets/parser/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.3/function2widgets/parser/docstr_parser.py
--rw-r--r--   0        0        0     6513 2024-04-02 10:48:44.584355 function2widgets-0.6.3/function2widgets/parser/function_parser.py
--rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.3/function2widgets/parser/parameter_parser.py
--rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.3/function2widgets/parser/widgetconfigs_parser.py
--rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.3/function2widgets/widget.py
--rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.3/function2widgets/widgets/__init__.py
--rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.3/function2widgets/widgets/_sourcecodeedit.py
--rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.3/function2widgets/widgets/allwidgets.py
--rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.3/function2widgets/widgets/base.py
--rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.3/function2widgets/widgets/editor/__init__.py
--rw-r--r--   0        0        0     6028 2024-03-31 08:24:42.434438 function2widgets-0.6.3/function2widgets/widgets/editor/base.py
--rw-r--r--   0        0        0     2041 2024-03-31 08:24:42.435447 function2widgets-0.6.3/function2widgets/widgets/editor/codeeditor.py
--rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.3/function2widgets/widgets/editor/dicteditor.py
--rw-r--r--   0        0        0     4244 2024-03-31 08:24:42.437456 function2widgets-0.6.3/function2widgets/widgets/editor/jsoneditor.py
--rw-r--r--   0        0        0     1245 2024-03-31 08:24:42.437456 function2widgets-0.6.3/function2widgets/widgets/editor/listeditor.py
--rw-r--r--   0        0        0     1602 2024-03-31 08:24:42.438534 function2widgets-0.6.3/function2widgets/widgets/editor/tupleeditor.py
--rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.3/function2widgets/widgets/lineedit/__init__.py
--rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.3/function2widgets/widgets/lineedit/floatedit.py
--rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.3/function2widgets/widgets/lineedit/intedit.py
--rw-r--r--   0        0        0     2897 2024-03-31 08:24:42.441427 function2widgets-0.6.3/function2widgets/widgets/lineedit/stredit.py
--rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.3/function2widgets/widgets/misc/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.3/function2widgets/widgets/misc/coloredit.py
--rw-r--r--   0        0        0     3459 2024-04-02 11:35:30.993072 function2widgets-0.6.3/function2widgets/widgets/misc/dateedit.py
--rw-r--r--   0        0        0     4091 2024-04-02 11:33:20.900442 function2widgets-0.6.3/function2widgets/widgets/misc/datetimeedit.py
--rw-r--r--   0        0        0     3340 2024-04-02 11:27:28.576112 function2widgets-0.6.3/function2widgets/widgets/misc/timeedit.py
--rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.3/function2widgets/widgets/numberinput/__init__.py
--rw-r--r--   0        0        0     4498 2024-03-31 08:24:42.445444 function2widgets-0.6.3/function2widgets/widgets/numberinput/dial.py
--rw-r--r--   0        0        0     2852 2024-03-31 08:24:42.446444 function2widgets-0.6.3/function2widgets/widgets/numberinput/floatspin.py
--rw-r--r--   0        0        0     2591 2024-03-31 08:24:42.446444 function2widgets-0.6.3/function2widgets/widgets/numberinput/intspin.py
--rw-r--r--   0        0        0     4957 2024-03-31 08:24:42.447443 function2widgets-0.6.3/function2widgets/widgets/numberinput/slider.py
--rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.3/function2widgets/widgets/pathedit/__init__.py
--rw-r--r--   0        0        0     6027 2024-03-31 08:24:42.448967 function2widgets-0.6.3/function2widgets/widgets/pathedit/base.py
--rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.3/function2widgets/widgets/pathedit/dirpathedit.py
--rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.3/function2widgets/widgets/pathedit/filepathedit.py
--rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.3/function2widgets/widgets/selectwidget/__init__.py
--rw-r--r--   0        0        0     1640 2024-03-31 08:24:42.450995 function2widgets-0.6.3/function2widgets/widgets/selectwidget/checkbox.py
--rw-r--r--   0        0        0     2761 2024-03-31 08:24:42.451979 function2widgets-0.6.3/function2widgets/widgets/selectwidget/checkbox_group.py
--rw-r--r--   0        0        0     2923 2024-03-31 08:24:42.452993 function2widgets-0.6.3/function2widgets/widgets/selectwidget/combobox.py
--rw-r--r--   0        0        0     2205 2024-03-31 08:24:42.452993 function2widgets-0.6.3/function2widgets/widgets/selectwidget/combobox_edit.py
--rw-r--r--   0        0        0     3507 2024-03-31 08:24:42.454138 function2widgets-0.6.3/function2widgets/widgets/selectwidget/radiobutton_group.py
--rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.3/function2widgets/widgets/textedit/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.3/function2widgets/widgets/textedit/codeedit.py
--rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.3/function2widgets/widgets/textedit/plaintext.py
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.3/License
--rw-r--r--   0        0        0      714 2024-04-02 11:38:28.796640 function2widgets-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.3/README.md
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.4/function2widgets/__init__.py
+-rw-r--r--   0        0        0     3030 2024-04-02 11:05:09.916571 function2widgets-0.6.4/function2widgets/common.py
+-rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.4/function2widgets/factory.py
+-rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.4/function2widgets/info.py
+-rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.4/function2widgets/parser/__init__.py
+-rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.4/function2widgets/parser/docstr_parser.py
+-rw-r--r--   0        0        0     6513 2024-04-02 10:48:44.584355 function2widgets-0.6.4/function2widgets/parser/function_parser.py
+-rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.4/function2widgets/parser/parameter_parser.py
+-rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.4/function2widgets/parser/widgetconfigs_parser.py
+-rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.4/function2widgets/widget.py
+-rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.4/function2widgets/widgets/__init__.py
+-rw-r--r--   0        0        0     5681 2024-03-31 08:24:42.431426 function2widgets-0.6.4/function2widgets/widgets/_sourcecodeedit.py
+-rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.4/function2widgets/widgets/allwidgets.py
+-rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.4/function2widgets/widgets/base.py
+-rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.4/function2widgets/widgets/editor/__init__.py
+-rw-r--r--   0        0        0     6061 2024-04-05 05:18:47.514607 function2widgets-0.6.4/function2widgets/widgets/editor/base.py
+-rw-r--r--   0        0        0     2024 2024-04-05 05:17:03.984199 function2widgets-0.6.4/function2widgets/widgets/editor/codeeditor.py
+-rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.4/function2widgets/widgets/editor/dicteditor.py
+-rw-r--r--   0        0        0     4654 2024-04-05 05:20:20.545687 function2widgets-0.6.4/function2widgets/widgets/editor/jsoneditor.py
+-rw-r--r--   0        0        0     1245 2024-04-05 05:16:06.955595 function2widgets-0.6.4/function2widgets/widgets/editor/listeditor.py
+-rw-r--r--   0        0        0     1602 2024-03-31 08:24:42.438534 function2widgets-0.6.4/function2widgets/widgets/editor/tupleeditor.py
+-rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.4/function2widgets/widgets/lineedit/__init__.py
+-rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.4/function2widgets/widgets/lineedit/floatedit.py
+-rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.4/function2widgets/widgets/lineedit/intedit.py
+-rw-r--r--   0        0        0     2897 2024-03-31 08:24:42.441427 function2widgets-0.6.4/function2widgets/widgets/lineedit/stredit.py
+-rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.4/function2widgets/widgets/misc/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.4/function2widgets/widgets/misc/coloredit.py
+-rw-r--r--   0        0        0     3459 2024-04-02 11:35:30.993072 function2widgets-0.6.4/function2widgets/widgets/misc/dateedit.py
+-rw-r--r--   0        0        0     4091 2024-04-02 11:33:20.900442 function2widgets-0.6.4/function2widgets/widgets/misc/datetimeedit.py
+-rw-r--r--   0        0        0     3340 2024-04-02 11:27:28.576112 function2widgets-0.6.4/function2widgets/widgets/misc/timeedit.py
+-rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.4/function2widgets/widgets/numberinput/__init__.py
+-rw-r--r--   0        0        0     4498 2024-03-31 08:24:42.445444 function2widgets-0.6.4/function2widgets/widgets/numberinput/dial.py
+-rw-r--r--   0        0        0     2852 2024-03-31 08:24:42.446444 function2widgets-0.6.4/function2widgets/widgets/numberinput/floatspin.py
+-rw-r--r--   0        0        0     2591 2024-03-31 08:24:42.446444 function2widgets-0.6.4/function2widgets/widgets/numberinput/intspin.py
+-rw-r--r--   0        0        0     4957 2024-03-31 08:24:42.447443 function2widgets-0.6.4/function2widgets/widgets/numberinput/slider.py
+-rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.4/function2widgets/widgets/pathedit/__init__.py
+-rw-r--r--   0        0        0     6027 2024-03-31 08:24:42.448967 function2widgets-0.6.4/function2widgets/widgets/pathedit/base.py
+-rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.4/function2widgets/widgets/pathedit/dirpathedit.py
+-rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.4/function2widgets/widgets/pathedit/filepathedit.py
+-rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.4/function2widgets/widgets/selectwidget/__init__.py
+-rw-r--r--   0        0        0     1640 2024-03-31 08:24:42.450995 function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox.py
+-rw-r--r--   0        0        0     2761 2024-03-31 08:24:42.451979 function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox_group.py
+-rw-r--r--   0        0        0     2923 2024-03-31 08:24:42.452993 function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox.py
+-rw-r--r--   0        0        0     2205 2024-03-31 08:24:42.452993 function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox_edit.py
+-rw-r--r--   0        0        0     3507 2024-03-31 08:24:42.454138 function2widgets-0.6.4/function2widgets/widgets/selectwidget/radiobutton_group.py
+-rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.4/function2widgets/widgets/textedit/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.4/function2widgets/widgets/textedit/codeedit.py
+-rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.4/function2widgets/widgets/textedit/plaintext.py
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.4/License
+-rw-r--r--   0        0        0      714 2024-04-05 05:20:59.638337 function2widgets-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.4/README.md
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.4/PKG-INFO
```

### Comparing `function2widgets-0.6.3/function2widgets/common.py` & `function2widgets-0.6.4/function2widgets/common.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/factory.py` & `function2widgets-0.6.4/function2widgets/factory.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/info.py` & `function2widgets-0.6.4/function2widgets/info.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/parser/docstr_parser.py` & `function2widgets-0.6.4/function2widgets/parser/docstr_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/parser/function_parser.py` & `function2widgets-0.6.4/function2widgets/parser/function_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/parser/parameter_parser.py` & `function2widgets-0.6.4/function2widgets/parser/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/parser/widgetconfigs_parser.py` & `function2widgets-0.6.4/function2widgets/parser/widgetconfigs_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widget.py` & `function2widgets-0.6.4/function2widgets/widget.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/_sourcecodeedit.py` & `function2widgets-0.6.4/function2widgets/widgets/_sourcecodeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/allwidgets.py` & `function2widgets-0.6.4/function2widgets/widgets/allwidgets.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/base.py` & `function2widgets-0.6.4/function2widgets/widgets/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/base.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     _WidgetArgsClass = BaseCodeEditorArgs
 
     def __init__(self, args: BaseCodeEditorArgs, parent: Optional[QWidget] = None):
 
         self._value_widget: Optional[QPushButton] = None
         self._display_widget: Optional[QPlainTextEdit] = None
-        self._display_widget_text_tpl: str = QApplication.tr("{}")
+        self._display_widget_text_tpl: str = "{}"
 
         self._current_value = args.default
 
         super().__init__(args=args, parent=parent)
 
         if self._args.set_default_on_init:
             self.set_value(self._args.default)
@@ -154,15 +154,16 @@
         text = self._args.display_widget_text
         self._display_widget.setPlainText(text.format(type(value), str(value)))
 
     def get_value(self) -> Any:
         return super().get_value()
 
     def set_value(self, value: Any):
-        self._update_current_value_display(value)
+        if self._args.display_current_value:
+            self._update_current_value_display(value)
         super().set_value(value)
 
     def get_value_from_widget(self) -> Any:
         return self._current_value
 
     def set_value_to_widget(self, value: Any):
         self._current_value = value
```

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/codeeditor.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/codeeditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @property
     def _args(self) -> CodeEditorArgs:
         return cast(CodeEditorArgs, super()._args)
 
     def get_value(self) -> Optional[str]:
         return super().get_value()
 
-    def set_value(self, value: Optional[str], *args, **kwargs):
+    def set_value(self, value: Optional[str]):
         if value is not None and not isinstance(value, str):
             raise ValueError(self.tr(f"value must be str, got {type(value)}"))
         super().set_value(value)
 
     def source_code_dialog(self) -> CodeEditorDialog:
         configs = self._args.configs or {}
         window_title = self._args.window_title or ""
```

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/dicteditor.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/dicteditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/jsoneditor.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/jsoneditor.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,7 +121,19 @@
             parent=self,
         )
         dialog.set_value(self._current_value)
         return dialog
 
     def fetch_result_from_dialog(self, dialog: JsonEditorDialog):
         return dialog.current_value
+
+    def set_value(self, value: Any):
+        if not isinstance(value, self._args.top_level_types):
+            raise InvalidValueError(
+                self.tr(
+                    f"value '{value}' is not one of the following types: {self._args.top_level_types}"
+                )
+            )
+        super().set_value(value)
+
+    def get_value(self) -> Any:
+        return super().get_value()
```

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/listeditor.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/listeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/editor/tupleeditor.py` & `function2widgets-0.6.4/function2widgets/widgets/editor/tupleeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/lineedit/floatedit.py` & `function2widgets-0.6.4/function2widgets/widgets/lineedit/floatedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/lineedit/intedit.py` & `function2widgets-0.6.4/function2widgets/widgets/lineedit/intedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/lineedit/stredit.py` & `function2widgets-0.6.4/function2widgets/widgets/lineedit/stredit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/misc/dateedit.py` & `function2widgets-0.6.4/function2widgets/widgets/misc/dateedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/misc/datetimeedit.py` & `function2widgets-0.6.4/function2widgets/widgets/misc/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/misc/timeedit.py` & `function2widgets-0.6.4/function2widgets/widgets/misc/timeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/numberinput/dial.py` & `function2widgets-0.6.4/function2widgets/widgets/numberinput/dial.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/numberinput/floatspin.py` & `function2widgets-0.6.4/function2widgets/widgets/numberinput/floatspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/numberinput/intspin.py` & `function2widgets-0.6.4/function2widgets/widgets/numberinput/intspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/numberinput/slider.py` & `function2widgets-0.6.4/function2widgets/widgets/numberinput/slider.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/pathedit/base.py` & `function2widgets-0.6.4/function2widgets/widgets/pathedit/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/pathedit/dirpathedit.py` & `function2widgets-0.6.4/function2widgets/widgets/pathedit/dirpathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/pathedit/filepathedit.py` & `function2widgets-0.6.4/function2widgets/widgets/pathedit/filepathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/selectwidget/checkbox.py` & `function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/selectwidget/checkbox_group.py` & `function2widgets-0.6.4/function2widgets/widgets/selectwidget/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/selectwidget/combobox.py` & `function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/selectwidget/combobox_edit.py` & `function2widgets-0.6.4/function2widgets/widgets/selectwidget/combobox_edit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/selectwidget/radiobutton_group.py` & `function2widgets-0.6.4/function2widgets/widgets/selectwidget/radiobutton_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/textedit/codeedit.py` & `function2widgets-0.6.4/function2widgets/widgets/textedit/codeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/function2widgets/widgets/textedit/plaintext.py` & `function2widgets-0.6.4/function2widgets/widgets/textedit/plaintext.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/License` & `function2widgets-0.6.4/License`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/pyproject.toml` & `function2widgets-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "function2widgets"
-version = "0.6.3"
+version = "0.6.4"
 description = ""
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 packages = [
     {include="function2widgets"}
 ]
```

### Comparing `function2widgets-0.6.3/README.md` & `function2widgets-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.3/PKG-INFO` & `function2widgets-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function2widgets
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Home-page: https://github.com/zimolab/function2widgets
 License: GPL-3.0
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

