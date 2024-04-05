# Comparing `tmp/netmiko_mhrt-1.0.5.tar.gz` & `tmp/netmiko_mhrt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netmiko_mhrt-1.0.5.tar", last modified: Fri Apr  5 02:33:33 2024, max compression
+gzip compressed data, was "netmiko_mhrt-1.0.6.tar", last modified: Fri Apr  5 05:33:23 2024, max compression
```

## Comparing `netmiko_mhrt-1.0.5.tar` & `netmiko_mhrt-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:34.127053 netmiko_mhrt-1.0.5/
--rwxrwx---   0 root         (0) vboxsf     (994)    11357 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (994)       63 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/MANIFEST.in
--rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 02:33:34.082791 netmiko_mhrt-1.0.5/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (994)     2669 2024-02-13 10:48:24.000000 netmiko_mhrt-1.0.5/README.rst
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:33.530516 netmiko_mhrt-1.0.5/netmiko_mhrt/
--rwxrwx---   0 root         (0) vboxsf     (994)     4538 2024-04-05 01:57:25.000000 netmiko_mhrt-1.0.5/netmiko_mhrt/__init__.py
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:34.026562 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (994)      310 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-02-13 10:29:10.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/not-zip-safe
--rwxrwx---   0 root         (0) vboxsf     (994)       15 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (994)       13 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (994)      100 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/pyproject.toml
--rwxrwx---   0 root         (0) vboxsf     (994)       14 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (994)       38 2024-04-05 02:33:34.131544 netmiko_mhrt-1.0.5/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (994)     1105 2024-04-05 02:33:17.000000 netmiko_mhrt-1.0.5/setup.py
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 05:33:24.269593 netmiko_mhrt-1.0.6/
+-rwxrwx---   0 root         (0) vboxsf     (994)    11357 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.6/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (994)       63 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.6/MANIFEST.in
+-rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 05:33:24.226621 netmiko_mhrt-1.0.6/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (994)     2669 2024-02-13 10:48:24.000000 netmiko_mhrt-1.0.6/README.rst
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 05:33:23.400702 netmiko_mhrt-1.0.6/netmiko_mhrt/
+-rwxrwx---   0 root         (0) vboxsf     (994)     4540 2024-04-05 05:26:48.000000 netmiko_mhrt-1.0.6/netmiko_mhrt/__init__.py
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 05:33:24.189506 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 05:33:22.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (994)      310 2024-04-05 05:33:22.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-04-05 05:33:22.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-02-13 10:29:10.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/not-zip-safe
+-rwxrwx---   0 root         (0) vboxsf     (994)       15 2024-04-05 05:33:22.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)       13 2024-04-05 05:33:22.000000 netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)      100 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.6/pyproject.toml
+-rwxrwx---   0 root         (0) vboxsf     (994)       14 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.6/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)       38 2024-04-05 05:33:24.275467 netmiko_mhrt-1.0.6/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (994)     1105 2024-04-05 05:33:11.000000 netmiko_mhrt-1.0.6/setup.py
```

### Comparing `netmiko_mhrt-1.0.5/LICENSE` & `netmiko_mhrt-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netmiko_mhrt-1.0.5/PKG-INFO` & `netmiko_mhrt-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netmiko_mhrt
-Version: 1.0.5
+Version: 1.0.6
 Summary: a forked version of netmiko_multihop
 Home-page: https://github.com/1mmortalPhoenix/netmiko_mhrt
 Author: Felix Li
 Author-email: immphoenix@gmail.com
 License: ASL V2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `netmiko_mhrt-1.0.5/README.rst` & `netmiko_mhrt-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `netmiko_mhrt-1.0.5/netmiko_mhrt/__init__.py` & `netmiko_mhrt-1.0.6/netmiko_mhrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,21 +113,20 @@
         raise netmiko.ConfigInvalidException(f"Cannot jump to {target_ip}.")
 
     if ssh_accept_host_pattern in result:
         self.send_command(ssh_accept_host_command, ssh_password_pattern)
     self.write_channel(target_password + "\n")
     self.send_command("\n", r"(continue:)|(#)")
 
-
     self.__jump_device_list.append(
         {"ip": self.host, "device_type": self.device_type, "username": self.username}
     )
     netmiko.redispatch(self, target_device_type)
     self.find_prompt()
-    log.debug(
+    logger.debug(
         f"successfully jumped to {target_device_type} {target_username}@{target_ip}"
     )
     return self
 
 
 setattr(netmiko.BaseConnection, "jump_to", jump_to)
 setattr(netmiko.BaseConnection, "jump_back", jump_back)
```

### Comparing `netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/PKG-INFO` & `netmiko_mhrt-1.0.6/netmiko_mhrt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netmiko_mhrt
-Version: 1.0.5
+Version: 1.0.6
 Summary: a forked version of netmiko_multihop
 Home-page: https://github.com/1mmortalPhoenix/netmiko_mhrt
 Author: Felix Li
 Author-email: immphoenix@gmail.com
 License: ASL V2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `netmiko_mhrt-1.0.5/setup.py` & `netmiko_mhrt-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 from subprocess import check_output
 
 
-version = "1.0.5"
+version = "1.0.6"
 
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().split("\n")
```

