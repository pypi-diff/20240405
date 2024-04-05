# Comparing `tmp/linien-gui-1.0.2.tar.gz` & `tmp/linien-gui-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-gui-1.0.2.tar", last modified: Fri Apr  5 08:49:31 2024, max compression
+gzip compressed data, was "linien-gui-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:45 2024, max compression
```

## Comparing `linien-gui-1.0.2.tar` & `linien-gui-1.0.2rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:31.532631 linien-gui-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 08:49:31.532631 linien-gui-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:31.524630 linien-gui-1.0.2/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)   410598 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:31.532631 linien-gui-1.0.2/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    26298 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/logging_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/logging_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    42563 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 08:49:10.000000 linien-gui-1.0.2/linien_gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:31.532631 linien-gui-1.0.2/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:49:31.000000 linien-gui-1.0.2/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:49:31.532631 linien-gui-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-05 08:49:10.000000 linien-gui-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.811801 linien-gui-1.0.2rc1/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   410598 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/device_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26298 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/general_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42563 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/psd_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/ui/view_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/linien_gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:31:45.000000 linien-gui-1.0.2rc1/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:45.819801 linien-gui-1.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-05 08:31:26.000000 linien-gui-1.0.2rc1/setup.py
```

### Comparing `linien-gui-1.0.2/PKG-INFO` & `linien-gui-1.0.2rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 1.0.2
+Version: 1.0.2rc1
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
@@ -12,10 +12,10 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.1.2
 Requires-Dist: pyqtgraph>=0.10.0
 Requires-Dist: PyQt5>=5.12.0
 Requires-Dist: superqt>=0.2.3
-Requires-Dist: linien_client==1.0.2
+Requires-Dist: linien_client==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-gui-1.0.2/linien_gui/__init__.py` & `linien-gui-1.0.2rc1/linien_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/app.py` & `linien-gui-1.0.2rc1/linien_gui/app.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/config.py` & `linien-gui-1.0.2rc1/linien_gui/config.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/dialogs.py` & `linien-gui-1.0.2rc1/linien_gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/icon.ico` & `linien-gui-1.0.2rc1/linien_gui/icon.ico`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/threads.py` & `linien-gui-1.0.2rc1/linien_gui/threads.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/device_manager.py` & `linien-gui-1.0.2rc1/linien_gui/ui/device_manager.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/device_manager.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/device_manager.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/general_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/general_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/general_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/general_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/lock_status_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/lock_status_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/locking_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/locking_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/locking_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/logging_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/logging_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/logging_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/main_window.py` & `linien-gui-1.0.2rc1/linien_gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/main_window.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/modulation_sweep_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/modulation_sweep_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/modulation_sweep_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/new_device_dialog.py` & `linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/new_device_dialog.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/new_device_dialog.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/optimization_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/optimization_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/optimization_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/plot_widget.py` & `linien-gui-1.0.2rc1/linien_gui/ui/plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/psd_plot_widget.py` & `linien-gui-1.0.2rc1/linien_gui/ui/psd_plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/psd_table_widget.py` & `linien-gui-1.0.2rc1/linien_gui/ui/psd_table_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/psd_window.py` & `linien-gui-1.0.2rc1/linien_gui/ui/psd_window.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/psd_window.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/psd_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/right_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/right_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/spectroscopy_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/spectroscopy_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/spectroscopy_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/spin_box.py` & `linien-gui-1.0.2rc1/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/sweep_control.py` & `linien-gui-1.0.2rc1/linien_gui/ui/sweep_control.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/version_checker.py` & `linien-gui-1.0.2rc1/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/view_panel.py` & `linien-gui-1.0.2rc1/linien_gui/ui/view_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/ui/view_panel.ui` & `linien-gui-1.0.2rc1/linien_gui/ui/view_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/utils.py` & `linien-gui-1.0.2rc1/linien_gui/utils.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui/widgets.py` & `linien-gui-1.0.2rc1/linien_gui/widgets.py`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/linien_gui.egg-info/PKG-INFO` & `linien-gui-1.0.2rc1/linien_gui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 1.0.2
+Version: 1.0.2rc1
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
@@ -12,10 +12,10 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.1.2
 Requires-Dist: pyqtgraph>=0.10.0
 Requires-Dist: PyQt5>=5.12.0
 Requires-Dist: superqt>=0.2.3
-Requires-Dist: linien_client==1.0.2
+Requires-Dist: linien_client==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-gui-1.0.2/linien_gui.egg-info/SOURCES.txt` & `linien-gui-1.0.2rc1/linien_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-gui-1.0.2/setup.py` & `linien-gui-1.0.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-gui",
-    version="1.0.2",
+    version="1.0.2rc1",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Graphical user interface of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
@@ -38,14 +38,14 @@
     entry_points={"console_scripts": ["linien=linien_gui.app:run_application"]},
     python_requires=">=3.8",
     install_requires=[
         "click>=7.1.2",
         "pyqtgraph>=0.10.0",
         "PyQt5>=5.12.0",
         "superqt>=0.2.3",
-        "linien_client==1.0.2",
+        "linien_client==1.0.2rc1",
     ],
     package_data={
         # IMPORTANT: any changes have to be made in pyinstaller.spec, too
         "": ["*.ui", "*.ico"]
     },
 )
```

