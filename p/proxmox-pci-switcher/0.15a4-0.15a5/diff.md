# Comparing `tmp/proxmox-pci-switcher-0.15a4.tar.gz` & `tmp/proxmox-pci-switcher-0.15a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxmox-pci-switcher-0.15a4.tar", last modified: Thu May  5 10:24:20 2022, max compression
+gzip compressed data, was "proxmox-pci-switcher-0.15a5.tar", last modified: Thu May  5 10:52:30 2022, max compression
```

## Comparing `proxmox-pci-switcher-0.15a4.tar` & `proxmox-pci-switcher-0.15a5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/
--rw-r--r--   0 root         (0) root         (0)     1078 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5101 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4606 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/
--rw-r--r--   0 root         (0) root         (0)       71 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4715 2022-05-05 10:24:19.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/proxmox_pci_switcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/ui/
--rw-r--r--   0 root         (0) root         (0)       16 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3146 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5101 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      120 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-05 10:24:20.000000 proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-05 10:24:20.297470 proxmox-pci-switcher-0.15a4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1228 2022-05-05 10:24:04.000000 proxmox-pci-switcher-0.15a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:52:30.972336 proxmox-pci-switcher-0.15a5/
+-rw-r--r--   0 root         (0) root         (0)     1078 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5101 2022-05-05 10:52:30.972336 proxmox-pci-switcher-0.15a5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4606 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:52:30.968336 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/
+-rw-r--r--   0 root         (0) root         (0)       71 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4718 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/proxmox_pci_switcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:52:30.972336 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/ui/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 10:52:30.972336 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5101 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-05-05 10:52:30.000000 proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-05-05 10:52:30.972336 proxmox-pci-switcher-0.15a5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1228 2022-05-05 10:52:09.000000 proxmox-pci-switcher-0.15a5/setup.py
```

### Comparing `proxmox-pci-switcher-0.15a4/LICENSE` & `proxmox-pci-switcher-0.15a5/LICENSE`

 * *Files identical despite different names*

### Comparing `proxmox-pci-switcher-0.15a4/PKG-INFO` & `proxmox-pci-switcher-0.15a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxmox-pci-switcher
-Version: 0.15a4
+Version: 0.15a5
 Summary: Switch among Guest VMs organized by Resource Pool
 Home-page: https://github.com/rosineygp/proxmox-pci-switcher
 Author: Rosiney Gomes Pereira
 Author-email: rosiney.gp@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `proxmox-pci-switcher-0.15a4/README.md` & `proxmox-pci-switcher-0.15a5/README.md`

 * *Files identical despite different names*

### Comparing `proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/proxmox_pci_switcher.py` & `proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/proxmox_pci_switcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,27 +177,27 @@
 @arg(
     "-c",
     "--config",
     help="config file path",
     default=DEFAULT_LINUX_PATH,
 )
 def gui():
-    _gui_main = "/ui/main"
+    _gui_main = "/ui/main.py"
     if os.name == "nt":
         _gui_main = "\\ui\\main.py"
 
     # Dynamic ui load
     SourceFileLoader(
         "ui", f"{os.path.dirname(os.path.realpath(__file__))}{_gui_main}"
     ).load_module()
 
 
 @named("version")
 def cmd_version():
-    version = "v0.15a4"
+    version = "v0.15a5"
     print(version)
 
 
 def __main():
     dispatch_commands([cmd_list_resources, cmd_switch_vm, cmd_version, gui])
```

### Comparing `proxmox-pci-switcher-0.15a4/proxmox_pci_switcher/ui/main.py` & `proxmox-pci-switcher-0.15a5/proxmox_pci_switcher/ui/main.py`

 * *Files identical despite different names*

### Comparing `proxmox-pci-switcher-0.15a4/proxmox_pci_switcher.egg-info/PKG-INFO` & `proxmox-pci-switcher-0.15a5/proxmox_pci_switcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxmox-pci-switcher
-Version: 0.15a4
+Version: 0.15a5
 Summary: Switch among Guest VMs organized by Resource Pool
 Home-page: https://github.com/rosineygp/proxmox-pci-switcher
 Author: Rosiney Gomes Pereira
 Author-email: rosiney.gp@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `proxmox-pci-switcher-0.15a4/setup.py` & `proxmox-pci-switcher-0.15a5/setup.py`

 * *Files identical despite different names*

