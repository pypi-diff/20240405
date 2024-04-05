# Comparing `tmp/netmiko_mhrt-1.0.4.tar.gz` & `tmp/netmiko_mhrt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netmiko_mhrt-1.0.4.tar", last modified: Wed Feb 14 00:22:50 2024, max compression
+gzip compressed data, was "netmiko_mhrt-1.0.5.tar", last modified: Fri Apr  5 02:33:33 2024, max compression
```

## Comparing `netmiko_mhrt-1.0.4.tar` & `netmiko_mhrt-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-02-14 00:22:59.383224 netmiko_mhrt-1.0.4/
--rwxrwx---   0 root         (0) vboxsf     (994)    11357 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.4/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (994)       63 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.4/MANIFEST.in
--rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-02-14 00:22:59.352950 netmiko_mhrt-1.0.4/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (994)     2669 2024-02-13 10:48:24.000000 netmiko_mhrt-1.0.4/README.rst
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-02-14 00:22:59.023160 netmiko_mhrt-1.0.4/netmiko_mhrt/
--rwxrwx---   0 root         (0) vboxsf     (994)     4448 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.4/netmiko_mhrt/__init__.py
-drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-02-14 00:22:59.325611 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-02-14 00:22:58.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (994)      310 2024-02-14 00:22:58.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-02-14 00:22:58.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-02-13 10:29:10.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/not-zip-safe
--rwxrwx---   0 root         (0) vboxsf     (994)       15 2024-02-14 00:22:58.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (994)       13 2024-02-14 00:22:58.000000 netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (994)      100 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.4/pyproject.toml
--rwxrwx---   0 root         (0) vboxsf     (994)       14 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.4/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (994)       38 2024-02-14 00:22:59.386152 netmiko_mhrt-1.0.4/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (994)     1105 2024-02-14 00:22:34.000000 netmiko_mhrt-1.0.4/setup.py
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:34.127053 netmiko_mhrt-1.0.5/
+-rwxrwx---   0 root         (0) vboxsf     (994)    11357 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (994)       63 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/MANIFEST.in
+-rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 02:33:34.082791 netmiko_mhrt-1.0.5/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (994)     2669 2024-02-13 10:48:24.000000 netmiko_mhrt-1.0.5/README.rst
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:33.530516 netmiko_mhrt-1.0.5/netmiko_mhrt/
+-rwxrwx---   0 root         (0) vboxsf     (994)     4538 2024-04-05 01:57:25.000000 netmiko_mhrt-1.0.5/netmiko_mhrt/__init__.py
+drwxrwx---   0 root         (0) vboxsf     (994)        0 2024-04-05 02:33:34.026562 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (994)     3309 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (994)      310 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)        1 2024-02-13 10:29:10.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/not-zip-safe
+-rwxrwx---   0 root         (0) vboxsf     (994)       15 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)       13 2024-04-05 02:33:32.000000 netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)      100 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/pyproject.toml
+-rwxrwx---   0 root         (0) vboxsf     (994)       14 2024-02-13 10:24:54.000000 netmiko_mhrt-1.0.5/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (994)       38 2024-04-05 02:33:34.131544 netmiko_mhrt-1.0.5/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (994)     1105 2024-04-05 02:33:17.000000 netmiko_mhrt-1.0.5/setup.py
```

### Comparing `netmiko_mhrt-1.0.4/LICENSE` & `netmiko_mhrt-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netmiko_mhrt-1.0.4/PKG-INFO` & `netmiko_mhrt-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netmiko_mhrt
-Version: 1.0.4
+Version: 1.0.5
 Summary: a forked version of netmiko_multihop
 Home-page: https://github.com/1mmortalPhoenix/netmiko_mhrt
 Author: Felix Li
 Author-email: immphoenix@gmail.com
 License: ASL V2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `netmiko_mhrt-1.0.4/README.rst` & `netmiko_mhrt-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `netmiko_mhrt-1.0.4/netmiko_mhrt/__init__.py` & `netmiko_mhrt-1.0.5/netmiko_mhrt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import netmiko
 from copy import deepcopy
 import logging  # noqa
 
-log = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 platforms = {
     "linux": {
         "ssh_base_cmd": "/usr/bin/ssh",
         "ssh_cmd_str": "{ssh_base_cmd} {ssh_verbose_option} -p {port} {optional_parameters} {username}@{ip}",
         "ssh_password_pattern": "[pP]assword:",
         "ssh_accept_host_pattern": "yes/no",
@@ -51,15 +51,15 @@
         raise Exception("No previous host to jump back to")
 
     self.write_channel(
         platforms.get(self.device_type, platforms["linux"])["ssh_disconnect_sequence"]
     )
     netmiko.redispatch(self, prev_platform["device_type"])
     self.find_prompt()
-    log.debug(
+    logger.debug(
         f"successfully jumped back to {prev_platform['device_type']} {prev_platform['username']}@{prev_platform['ip']}"
     )
 
     return self
 
 
 def jump_to(self, **kwargs):
@@ -84,43 +84,44 @@
     except KeyError:
         target_device_type = "linux"
 
     if not hasattr(self, "__jump_device_list"):
         self.__jump_device_list = []
 
     no_log = {"password": target_password}
-    log.addFilter(netmiko.base_connection.SecretsFilter(no_log=no_log))
+    logger.addFilter(netmiko.base_connection.SecretsFilter(no_log=no_log))
 
     ssh_accept_host_pattern = platforms[self.device_type]["ssh_accept_host_pattern"]
     ssh_password_pattern = platforms[self.device_type]["ssh_password_pattern"]
     ssh_accept_host_command = platforms[self.device_type]["ssh_accept_host_command"]
     cfg = deepcopy(platforms[self.device_type])
     for k, v in kwargs.items():
         cfg[k] = v
 
     if "vrf" in kwargs:
         cfg[
             "vrf_str"
         ] = f"{platforms[self.device_type].get('vrf_prefix', '')}{kwargs['vrf']}"
 
     ssh_cmd_str = platforms[self.device_type]["ssh_cmd_str"].format(**cfg)
-    log.debug(ssh_cmd_str)
-
+    logger.debug(ssh_cmd_str)
+    logger.info(f"Jumping to next hop device with IP address {target_ip}...")
     try:
         result = self.send_command(
             ssh_cmd_str, f"({ssh_password_pattern})|({ssh_accept_host_pattern})"
         )
     except Exception:
         raise netmiko.ConfigInvalidException(f"Cannot jump to {target_ip}.")
 
     if ssh_accept_host_pattern in result:
         self.send_command(ssh_accept_host_command, ssh_password_pattern)
     self.write_channel(target_password + "\n")
     self.send_command("\n", r"(continue:)|(#)")
 
+
     self.__jump_device_list.append(
         {"ip": self.host, "device_type": self.device_type, "username": self.username}
     )
     netmiko.redispatch(self, target_device_type)
     self.find_prompt()
     log.debug(
         f"successfully jumped to {target_device_type} {target_username}@{target_ip}"
```

### Comparing `netmiko_mhrt-1.0.4/netmiko_mhrt.egg-info/PKG-INFO` & `netmiko_mhrt-1.0.5/netmiko_mhrt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netmiko_mhrt
-Version: 1.0.4
+Version: 1.0.5
 Summary: a forked version of netmiko_multihop
 Home-page: https://github.com/1mmortalPhoenix/netmiko_mhrt
 Author: Felix Li
 Author-email: immphoenix@gmail.com
 License: ASL V2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `netmiko_mhrt-1.0.4/setup.py` & `netmiko_mhrt-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 from subprocess import check_output
 
 
-version = "1.0.4"
+version = "1.0.5"
 
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().split("\n")
```

