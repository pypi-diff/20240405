# Comparing `tmp/ebs-linuxnode-gui-kivy-marquee-3.4.tar.gz` & `tmp/ebs-linuxnode-gui-kivy-marquee-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebs-linuxnode-gui-kivy-marquee-3.4.tar", last modified: Sun Mar 31 08:06:21 2024, max compression
+gzip compressed data, was "ebs-linuxnode-gui-kivy-marquee-3.5.tar", last modified: Fri Apr  5 14:23:50 2024, max compression
```

## Comparing `ebs-linuxnode-gui-kivy-marquee-3.4.tar` & `ebs-linuxnode-gui-kivy-marquee-3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      646 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/marquee/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/marquee/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7468 2024-03-31 07:39:02.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/marquee/mixin.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      646 2024-03-31 08:06:21.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      490 2024-03-31 08:06:21.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-03-31 08:06:21.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       79 2024-03-31 08:06:21.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2024-03-31 08:06:21.000000 ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2024-03-31 08:06:21.688428 ebs-linuxnode-gui-kivy-marquee-3.4/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      999 2024-03-30 18:50:23.000000 ebs-linuxnode-gui-kivy-marquee-3.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      646 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.493464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/marquee/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:16:39.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/marquee/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7367 2024-04-01 06:20:31.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/marquee/mixin.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      646 2024-04-05 14:23:50.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      490 2024-04-05 14:23:50.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-05 14:23:50.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       79 2024-04-05 14:23:50.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2024-04-05 14:23:50.000000 ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2024-04-05 14:23:50.497464 ebs-linuxnode-gui-kivy-marquee-3.5/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      999 2024-03-30 18:50:23.000000 ebs-linuxnode-gui-kivy-marquee-3.5/setup.py
```

### Comparing `ebs-linuxnode-gui-kivy-marquee-3.4/.gitignore` & `ebs-linuxnode-gui-kivy-marquee-3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-gui-kivy-marquee-3.4/PKG-INFO` & `ebs-linuxnode-gui-kivy-marquee-3.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-gui-kivy-marquee
-Version: 3.4
+Version: 3.5
 Summary: Marquee for EBS Linuxnode Kivy Applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-kivy-marquee
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-gui-kivy-marquee-3.4/ebs/linuxnode/gui/kivy/marquee/mixin.py` & `ebs-linuxnode-gui-kivy-marquee-3.5/ebs/linuxnode/gui/kivy/marquee/mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
             return self._marquee_default_text
         elif isinstance(self._marquee_default_text, list):
             return ' | '.join(self._marquee_default_text)
 
     @marquee_default_text.setter
     def marquee_default_text(self, value):
         restart = False
-        self.log.error(f"Setting text {value}")
         if value != self._marquee_default_text:
             if self._marquee_default_task:
                 self._marquee_default_task.stop()
                 self._marquee_default_task = None
             if self._marquee_is_default:
                 self.marquee_stop()
             restart = True
@@ -145,15 +144,14 @@
 
     @property
     def marquee_default_frequency(self):
         return self._marquee_default_frequency or 0
 
     @marquee_default_frequency.setter
     def marquee_default_frequency(self, value):
-        self.log.error(f"Setting frequency {value}")
         restart = False
         if value != self._marquee_default_frequency:
             if self._marquee_default_task:
                 self._marquee_default_task.stop()
                 self._marquee_default_task = None
             if self._marquee_is_default:
                 self.marquee_stop()
```

### Comparing `ebs-linuxnode-gui-kivy-marquee-3.4/ebs_linuxnode_gui_kivy_marquee.egg-info/PKG-INFO` & `ebs-linuxnode-gui-kivy-marquee-3.5/ebs_linuxnode_gui_kivy_marquee.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-gui-kivy-marquee
-Version: 3.4
+Version: 3.5
 Summary: Marquee for EBS Linuxnode Kivy Applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-kivy-marquee
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-gui-kivy-marquee-3.4/setup.py` & `ebs-linuxnode-gui-kivy-marquee-3.5/setup.py`

 * *Files identical despite different names*

