# Comparing `tmp/ebs-linuxnode-gui-kivy-gallery-2.1.tar.gz` & `tmp/ebs-linuxnode-gui-kivy-gallery-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ebs-linuxnode-gui-kivy-gallery-2.1.tar", last modified: Mon Apr 18 18:56:24 2022, max compression
+gzip compressed data, was "ebs-linuxnode-gui-kivy-gallery-2.2.tar", last modified: Fri Apr  5 14:57:37 2024, max compression
```

## Comparing `ebs-linuxnode-gui-kivy-gallery-2.1.tar` & `ebs-linuxnode-gui-kivy-gallery-2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2020-03-20 07:51:16.000000 ebs-linuxnode-gui-kivy-gallery-2.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      710 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-03-29 10:58:27.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       42 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/constants.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7502 2022-04-18 14:36:17.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/managers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      997 2022-04-18 15:02:44.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/mixin.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/models.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2167 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/resources.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2022-03-29 11:14:14.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/gallery/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-03-29 10:58:52.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/gallery/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1512 2022-04-18 13:52:28.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/gallery/mixin.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      710 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      679 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      147 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-04-18 18:56:24.000000 ebs-linuxnode-gui-kivy-gallery-2.1/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1085 2022-04-18 18:54:18.000000 ebs-linuxnode-gui-kivy-gallery-2.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      654 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       42 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/constants.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7610 2024-04-05 14:41:20.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/managers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1108 2024-04-05 14:51:02.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/mixin.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/models.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2167 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/resources.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/gallery/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/gallery/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1668 2024-04-05 14:52:31.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/gallery/mixin.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      654 2024-04-05 14:57:37.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      679 2024-04-05 14:57:37.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-05 14:57:37.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      147 2024-04-05 14:57:37.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2024-04-05 14:57:37.000000 ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2024-04-05 14:57:37.236831 ebs-linuxnode-gui-kivy-gallery-2.2/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1085 2023-03-15 17:18:19.000000 ebs-linuxnode-gui-kivy-gallery-2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/.gitignore` & `ebs-linuxnode-gui-kivy-gallery-2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/PKG-INFO` & `ebs-linuxnode-gui-kivy-gallery-2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ebs-linuxnode-gui-kivy-gallery
-Version: 2.1
+Version: 2.2
 Summary: Image Gallery infrastructure linuxnode applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-kivy-gallery
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/managers.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/managers.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,18 @@
                                       source=self)
         return self._log
 
     @property
     def default_duration(self):
         return self._default_duration
 
+    @default_duration.setter
+    def default_duration(self, value):
+        self._default_duration = value
+
     def flush(self, force=False):
         self.log.debug("Flushing gallery resources")
         self._items = []
         if force:
             self._trigger_transition()
 
     def _load(self, items):
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/mixin.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
     def gallery_manager(self, gmid):
         if gmid not in self._gallery_managers.keys():
             self.log.info("Initializing gallery manager {gmid}", gmid=gmid)
             self._gallery_managers[gmid] = GalleryManager(self, gmid, self.gui_gallery)
         return self._gallery_managers[gmid]
 
+    def gallery_default_duration(self, value):
+        self.gallery_manager(SIDEBAR).default_duration = value
+
     def gallery_load(self, items):
         self.gallery_manager(SIDEBAR).load(items)
 
     def gallery_start(self):
         self.gallery_manager(SIDEBAR).start()
 
     def gallery_stop(self):
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/models.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/models.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gallery/resources.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gallery/resources.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs/linuxnode/gui/kivy/gallery/mixin.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs/linuxnode/gui/kivy/gallery/mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 
 from kivy.uix.relativelayout import RelativeLayout
 from kivy_garden.ebs.gallery import ImageGallery
 
 from ebs.linuxnode.gui.kivy.core.basenode import BaseIoTNodeGui
 from ebs.linuxnode.gallery.mixin import GalleryMixin
+from kivy_garden.ebs.core.colors import color_set_alpha
 
 
 class GalleryGuiMixin(GalleryMixin, BaseIoTNodeGui):
     _media_extentions_image = ['.png', '.jpg', '.bmp', '.gif', '.jpeg']
 
     def __init__(self, *args, **kwargs):
         self._gallery = None
@@ -24,14 +25,17 @@
 
     def _gui_gallery_sidebar_control(self, *args):
         if self.gui_gallery.visible:
             self.gui_sidebar_show('gallery')
         else:
             self.gui_sidebar_hide('gallery')
 
+    def gallery_bgcolor(self, value):
+        self.gui_gallery.bgcolor = color_set_alpha(value, 1)
+
     @property
     def gui_gallery(self):
         if not self._gallery:
             params = {'parent_layout': self.gui_gallery_parent}
             if self.config.portrait:
                 params['animation_vector'] = (1, 0)
             else:
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/PKG-INFO` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ebs-linuxnode-gui-kivy-gallery
-Version: 2.1
+Version: 2.2
 Summary: Image Gallery infrastructure linuxnode applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-kivy-gallery
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/ebs_linuxnode_gui_kivy_gallery.egg-info/SOURCES.txt` & `ebs-linuxnode-gui-kivy-gallery-2.2/ebs_linuxnode_gui_kivy_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-gui-kivy-gallery-2.1/setup.py` & `ebs-linuxnode-gui-kivy-gallery-2.2/setup.py`

 * *Files identical despite different names*

