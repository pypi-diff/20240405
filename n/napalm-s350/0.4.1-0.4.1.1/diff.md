# Comparing `tmp/napalm-s350-0.4.1.tar.gz` & `tmp/napalm-s350-0.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-s350-0.4.1.tar", last modified: Fri Mar 29 16:22:49 2024, max compression
+gzip compressed data, was "napalm-s350-0.4.1.1.tar", last modified: Fri Apr  5 06:17:16 2024, max compression
```

## Comparing `napalm-s350-0.4.1.tar` & `napalm-s350-0.4.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:22:49.181179 napalm-s350-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-03-29 16:22:49.181179 napalm-s350-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:22:49.177179 napalm-s350-0.4.1/napalm_s350/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/napalm_s350/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/napalm_s350/s350.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:22:49.177179 napalm-s350-0.4.1/napalm_s350/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/napalm_s350/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:22:49.177179 napalm-s350-0.4.1/napalm_s350/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/napalm_s350/utils/textfsm_templates/hosts.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:22:49.177179 napalm-s350-0.4.1/napalm_s350.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-03-29 16:22:49.000000 napalm-s350-0.4.1/napalm_s350.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-29 16:22:49.000000 napalm-s350-0.4.1/napalm_s350.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:22:49.000000 napalm-s350-0.4.1/napalm_s350.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-29 16:22:49.000000 napalm-s350-0.4.1/napalm_s350.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 16:22:49.000000 napalm-s350-0.4.1/napalm_s350.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 16:22:49.181179 napalm-s350-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-29 16:22:40.000000 napalm-s350-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.292621 napalm-s350-0.4.1.1/napalm_s350/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/s350.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/utils/textfsm_templates/hosts.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/setup.py
```

### Comparing `napalm-s350-0.4.1/LICENSE` & `napalm-s350-0.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-s350-0.4.1/PKG-INFO` & `napalm-s350-0.4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.4.1
+Version: 0.4.1.1
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: napalm<=4.0.0
-Requires-Dist: netmiko<=4.0.0
-Requires-Dist: netaddr<=1.2.1
+Requires-Dist: napalm>=4.0.0
+Requires-Dist: netmiko>=4.0.0
+Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
 NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
 
 ## Status
 Master: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=master&event=push)
```

### Comparing `napalm-s350-0.4.1/README.md` & `napalm-s350-0.4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napalm-s350-0.4.1/napalm_s350/__init__.py` & `napalm-s350-0.4.1.1/napalm_s350/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-s350-0.4.1/napalm_s350/s350.py` & `napalm-s350-0.4.1.1/napalm_s350/s350.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,26 +29,19 @@
 from netmiko import ConnectHandler
 from napalm.base import NetworkDriver
 from napalm.base.exceptions import (
     CommandErrorException,
     ConnectionClosedException,
 )
 from napalm.base.helpers import canonical_interface_name
+from napalm.base.netmiko_helpers import netmiko_args
 
 import napalm.base.constants as C
 import napalm.base.canonical_map
 
-# make may own base_interfaces for s350
-s350_base_interfaces = {
-    **napalm.base.canonical_map.base_interfaces,
-    "fa": "FastEthernet",
-    "gi": "GigabitEthernet",
-    "te": "TengigabitEthernet",
-}
-
 from typing import List
 
 
 class S350Driver(NetworkDriver):
     """Napalm driver for S350."""
 
     def __init__(self, hostname, username, password, timeout=60, optional_args=None):
@@ -61,39 +54,15 @@
 
         if optional_args is None:
             optional_args = {}
 
         self._dest_file_system = optional_args.get("dest_file_system", None)
 
         # Netmiko possible arguments
-        netmiko_argument_map = {
-            "port": None,
-            "secret": "",
-            "verbose": False,
-            "keepalive": 30,
-            "global_delay_factor": 1,
-            "use_keys": False,
-            "key_file": None,
-            "ssh_strict": False,
-            "system_host_keys": False,
-            "alt_host_keys": False,
-            "alt_key_file": "",
-            "ssh_config_file": None,
-            "allow_agent": False,
-            "session_log": None,
-            "read_timeout_override": None,
-        }
-
-        # Allow for passing additional Netmiko arguments
-        self.netmiko_optional_args = {}
-        for k, v in netmiko_argument_map.items():
-            try:
-                self.netmiko_optional_args[k] = optional_args[k]
-            except KeyError:
-                pass
+        self.netmiko_optional_args = netmiko_args(optional_args)
 
         self.platform = "s350"
         self.port = optional_args.get("port", 22)
         self.device = None
         self.force_no_enable = optional_args.get("force_no_enable", False)
 
     def open(self):
@@ -171,15 +140,15 @@
                 if1, if2, ip, mac, _ = line.split()
                 interface = "{} {}".format(if1, if2)
             elif len(line.split()) == 6:
                 _, _, interface, ip, mac, _ = line.split()
             else:
                 raise ValueError("Unexpected output: {}".format(line.split()))
 
-            interface = canonical_interface_name(interface, s350_base_interfaces)
+            interface = canonical_interface_name(interface)
 
             entry = {
                 "interface": interface,
                 "mac": napalm.base.helpers.mac(mac),
                 "ip": ip,
                 "age": 0.0,
             }
@@ -290,15 +259,15 @@
         show_int_st = re.sub(
             r"(^-.*$|^Port .*$|^Ch .*$)|^\s.*$|^.*Flow.*$", "", show_int_st, flags=re.M
         )
         for line in show_int_st.splitlines():
             if not line:
                 continue
             interface = line.split()[0]
-            interface = canonical_interface_name(interface, s350_base_interfaces)
+            interface = canonical_interface_name(interface)
 
             interfaces.append(str(interface))
 
         return {
             "fqdn": str(fqdn),
             "hostname": str(hostname),
             "interface_list": interfaces,
@@ -470,15 +439,15 @@
                     "speed": float(speed),
                     "mtu": mtu,
                     "last_flapped": -1.0,
                     "description": description,
                     "mac_address": napalm.base.helpers.mac(mac),
                 }
 
-                interface = canonical_interface_name(interface, s350_base_interfaces)
+                interface = canonical_interface_name(interface)
 
                 interfaces[interface] = entry
 
         return interfaces
 
     def get_interfaces_ip(self):
         """Returns all configured interface IP addresses."""
@@ -508,15 +477,15 @@
 
             cidr = line_elems[0]
             interface = line_elems[1]
 
             ip = netaddr.IPNetwork(cidr)
             family = "ipv{0}".format(ip.version)
 
-            interface = canonical_interface_name(interface, s350_base_interfaces)
+            interface = canonical_interface_name(interface)
 
             interfaces[interface] = {family: {str(ip.ip): {"prefix_length": ip.prefixlen}}}
 
         return interfaces
 
     def _get_ip_int_line_to_fields(self, line, fields_end):
         """dynamic fields lenghts"""
@@ -566,15 +535,15 @@
                 remote_name = remote_name + line_elems[3]
                 # then reuse old values na rewrite previous entry
             else:
                 local_port = line_elems[0]
                 remote_port = line_elems[2]
                 remote_name = line_elems[3]
 
-            local_port = canonical_interface_name(local_port, s350_base_interfaces)
+            local_port = canonical_interface_name(local_port)
 
             neighbor = {
                 "hostname": remote_name,
                 "port": remote_port,
             }
             neighbor_list = [
                 neighbor,
@@ -620,22 +589,22 @@
         details = {}
 
         # First determine all interfaces with valid LLDP neighbors
         for local_port in self.get_lldp_neighbors().keys():
             if interface:
                 if interface == local_port:
                     entry = self._get_lldp_neighbors_detail_parse(local_port)
-                    local_port = canonical_interface_name(local_port, s350_base_interfaces)
+                    local_port = canonical_interface_name(local_port)
                     details[local_port] = [
                         entry,
                     ]
 
             else:
                 entry = self._get_lldp_neighbors_detail_parse(local_port)
-                local_port = canonical_interface_name(local_port, s350_base_interfaces)
+                local_port = canonical_interface_name(local_port)
                 details[local_port] = [
                     entry,
                 ]
 
         return details
 
     def _get_lldp_neighbors_detail_parse(self, local_port):
@@ -662,15 +631,15 @@
             elif line.startswith("System Name"):
                 remote_system_name = self._get_lldp_line_value(line)
             elif line.startswith("System description"):
                 remote_system_description = self._get_lldp_line_value(line)
             elif line.startswith("Capabilities"):
                 caps = self._get_lldp_neighbors_detail_capabilities_parse(line)
 
-        remote_port_id = canonical_interface_name(remote_port_id, s350_base_interfaces)
+        remote_port_id = canonical_interface_name(remote_port_id)
 
         entry = {
             "parent_interface": "N/A",
             "remote_port": remote_port_id,
             "remote_port_description": remote_port_description,
             "remote_chassis_id": remote_chassis_id,
             "remote_system_name": remote_system_name,
```

### Comparing `napalm-s350-0.4.1/napalm_s350.egg-info/PKG-INFO` & `napalm-s350-0.4.1.1/napalm_s350.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.4.1
+Version: 0.4.1.1
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: napalm<=4.0.0
-Requires-Dist: netmiko<=4.0.0
-Requires-Dist: netaddr<=1.2.1
+Requires-Dist: napalm>=4.0.0
+Requires-Dist: netmiko>=4.0.0
+Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
 NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
 
 ## Status
 Master: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=master&event=push)
```

### Comparing `napalm-s350-0.4.1/setup.py` & `napalm-s350-0.4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     reqs = [r for r in fs.read().splitlines() if (len(r) > 0 and not r.startswith("#"))]
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setup(
     name="napalm-s350",
-    version="0.4.1",
+    version="0.4.1.1",
     packages=find_packages(exclude=("test*",)),
     author="Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher",
     author_email="j@jasper.la, qaxi@seznam.cz, mail@phill93.de",
     description="NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

