# Comparing `tmp/jedha_cli-1.1.6.tar.gz` & `tmp/jedha_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jedha_cli-1.1.6.tar", max compression
+gzip compressed data, was "jedha_cli-1.2.0.tar", max compression
```

## Comparing `jedha_cli-1.1.6.tar` & `jedha_cli-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,50 @@
--rw-r--r--   0        0        0    35149 2024-01-25 10:09:15.321100 jedha_cli-1.1.6/LICENSE
--rw-r--r--   0        0        0     1574 2024-01-25 10:09:15.321257 jedha_cli-1.1.6/README.md
--rw-r--r--   0        0        0      687 2024-04-02 15:57:11.587448 jedha_cli-1.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-25 10:09:15.322437 jedha_cli-1.1.6/src/__init__.py
--rw-r--r--   0        0        0      284 2024-04-02 15:56:48.428717 jedha_cli-1.1.6/src/labs/backdoor.yaml
--rw-r--r--   0        0        0      347 2024-02-22 16:27:32.696922 jedha_cli-1.1.6/src/labs/bypass-login.yaml
--rw-r--r--   0        0        0      571 2024-01-25 10:09:15.322806 jedha_cli-1.1.6/src/labs/dns_zone_transfer.yaml
--rw-r--r--   0        0        0      684 2024-02-19 14:17:57.490868 jedha_cli-1.1.6/src/labs/docker_evasion_1.yaml
--rw-r--r--   0        0        0      357 2024-02-19 14:17:57.491309 jedha_cli-1.1.6/src/labs/docker_evasion_2.yaml
--rw-r--r--   0        0        0      358 2024-02-19 14:17:57.491623 jedha_cli-1.1.6/src/labs/docker_evasion_3.yaml
--rw-r--r--   0        0        0      323 2024-02-22 16:27:32.697055 jedha_cli-1.1.6/src/labs/format_string.yaml
--rw-r--r--   0        0        0      295 2024-04-02 15:56:48.429028 jedha_cli-1.1.6/src/labs/gash.yaml
--rw-r--r--   0        0        0      318 2024-01-25 10:09:15.323286 jedha_cli-1.1.6/src/labs/hid.yaml
--rw-r--r--   0        0        0      359 2024-02-22 16:27:32.697156 jedha_cli-1.1.6/src/labs/idor.yaml
--rw-r--r--   0        0        0      356 2024-02-22 16:27:32.697260 jedha_cli-1.1.6/src/labs/insecure_design.yaml
--rw-r--r--   0        0        0      329 2024-01-25 10:44:56.612899 jedha_cli-1.1.6/src/labs/linux_privesc.yaml
--rw-r--r--   0        0        0      452 2024-04-02 15:56:48.429319 jedha_cli-1.1.6/src/labs/little_big_ctf.yaml
--rw-r--r--   0        0        0      353 2024-01-25 10:09:15.323660 jedha_cli-1.1.6/src/labs/manual_audit.yaml
--rw-r--r--   0        0        0      371 2024-03-07 14:30:23.918539 jedha_cli-1.1.6/src/labs/msf_1.yaml
--rw-r--r--   0        0        0      304 2024-02-22 16:27:32.697647 jedha_cli-1.1.6/src/labs/msf_2.yaml
--rw-r--r--   0        0        0      297 2024-04-02 15:56:48.429649 jedha_cli-1.1.6/src/labs/my_first_ctf.yaml
--rw-r--r--   0        0        0      300 2024-04-02 15:56:48.429968 jedha_cli-1.1.6/src/labs/my_second_ctf.yaml
--rw-r--r--   0        0        0      352 2024-02-22 16:27:32.697771 jedha_cli-1.1.6/src/labs/path_traversal.yaml
--rw-r--r--   0        0        0     2445 2024-03-15 13:38:48.454766 jedha_cli-1.1.6/src/labs/pentesting_network_services.yaml
--rw-r--r--   0        0        0      284 2024-04-02 15:56:48.430129 jedha_cli-1.1.6/src/labs/sambacry.yaml
--rw-r--r--   0        0        0      380 2024-02-22 16:27:32.698222 jedha_cli-1.1.6/src/labs/security_misconfiguration.yaml
--rw-r--r--   0        0        0      290 2024-04-02 15:56:48.430290 jedha_cli-1.1.6/src/labs/shellshock.yaml
--rw-r--r--   0        0        0      751 2024-03-13 10:00:54.999558 jedha_cli-1.1.6/src/labs/sqli.yaml
--rw-r--r--   0        0        0      893 2024-02-22 16:27:32.698691 jedha_cli-1.1.6/src/labs/ssrf.yaml
--rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699086 jedha_cli-1.1.6/src/labs/sudo_1.yaml
--rw-r--r--   0        0        0      276 2024-03-20 09:49:04.648517 jedha_cli-1.1.6/src/labs/sudo_2.yaml
--rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324618 jedha_cli-1.1.6/src/labs/sudo_3.yaml
--rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699334 jedha_cli-1.1.6/src/labs/suid.yaml
--rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324914 jedha_cli-1.1.6/src/labs/suid_2.yaml
--rw-r--r--   0        0        0      628 2024-02-22 16:27:32.699456 jedha_cli-1.1.6/src/labs/template_injection.yaml
--rw-r--r--   0        0        0      279 2024-04-02 15:56:48.430442 jedha_cli-1.1.6/src/labs/vim_fu.yaml
--rw-r--r--   0        0        0      998 2024-04-02 15:56:48.430606 jedha_cli-1.1.6/src/labs/vuln_web_app.yaml
--rw-r--r--   0        0        0     1119 2024-02-22 16:27:32.699708 jedha_cli-1.1.6/src/labs/vulnerable_and_outdated_software.yaml
--rw-r--r--   0        0        0      290 2024-01-25 10:09:15.325298 jedha_cli-1.1.6/src/labs/wifi_wpa2_cracking.yaml
--rw-r--r--   0        0        0      352 2024-01-25 10:09:15.325420 jedha_cli-1.1.6/src/labs/windows_box.yaml
--rw-r--r--   0        0        0      320 2024-02-22 16:27:32.699823 jedha_cli-1.1.6/src/labs/xss.yaml
--rw-r--r--   0        0        0     4563 2024-04-02 15:56:48.428362 jedha_cli-1.1.6/src/labs.yaml
--rw-r--r--   0        0        0     9009 2024-03-20 13:07:51.694200 jedha_cli-1.1.6/src/main.py
--rw-r--r--   0        0        0     6363 2024-03-13 14:11:35.442529 jedha_cli-1.1.6/src/misc.py
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 jedha_cli-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-25 10:09:15.321100 jedha_cli-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1574 2024-01-25 10:09:15.321257 jedha_cli-1.2.0/README.md
+-rw-r--r--   0        0        0      687 2024-04-05 15:17:06.206387 jedha_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-25 10:09:15.322437 jedha_cli-1.2.0/src/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-05 15:13:58.979330 jedha_cli-1.2.0/src/labs/backdoor.yaml
+-rw-r--r--   0        0        0      347 2024-02-22 16:27:32.696922 jedha_cli-1.2.0/src/labs/bypass-login.yaml
+-rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100571 jedha_cli-1.2.0/src/labs/covering-tracks-linux.yaml
+-rw-r--r--   0        0        0      675 2024-04-05 15:16:44.100708 jedha_cli-1.2.0/src/labs/covering-tracks.yaml
+-rw-r--r--   0        0        0      571 2024-01-25 10:09:15.322806 jedha_cli-1.2.0/src/labs/dns_zone_transfer.yaml
+-rw-r--r--   0        0        0      684 2024-02-19 14:17:57.490868 jedha_cli-1.2.0/src/labs/docker_evasion_1.yaml
+-rw-r--r--   0        0        0      357 2024-02-19 14:17:57.491309 jedha_cli-1.2.0/src/labs/docker_evasion_2.yaml
+-rw-r--r--   0        0        0      358 2024-02-19 14:17:57.491623 jedha_cli-1.2.0/src/labs/docker_evasion_3.yaml
+-rw-r--r--   0        0        0      323 2024-02-22 16:27:32.697055 jedha_cli-1.2.0/src/labs/format_string.yaml
+-rw-r--r--   0        0        0      295 2024-04-05 15:13:58.979678 jedha_cli-1.2.0/src/labs/gash.yaml
+-rw-r--r--   0        0        0      318 2024-01-25 10:09:15.323286 jedha_cli-1.2.0/src/labs/hid.yaml
+-rw-r--r--   0        0        0      359 2024-02-22 16:27:32.697156 jedha_cli-1.2.0/src/labs/idor.yaml
+-rw-r--r--   0        0        0      356 2024-02-22 16:27:32.697260 jedha_cli-1.2.0/src/labs/insecure_design.yaml
+-rw-r--r--   0        0        0      329 2024-01-25 10:44:56.612899 jedha_cli-1.2.0/src/labs/linux_privesc.yaml
+-rw-r--r--   0        0        0      452 2024-04-05 15:13:58.980008 jedha_cli-1.2.0/src/labs/little_big_ctf.yaml
+-rw-r--r--   0        0        0      353 2024-01-25 10:09:15.323660 jedha_cli-1.2.0/src/labs/manual_audit.yaml
+-rw-r--r--   0        0        0      371 2024-03-07 14:30:23.918539 jedha_cli-1.2.0/src/labs/msf_1.yaml
+-rw-r--r--   0        0        0      304 2024-02-22 16:27:32.697647 jedha_cli-1.2.0/src/labs/msf_2.yaml
+-rw-r--r--   0        0        0      297 2024-04-05 15:13:58.980275 jedha_cli-1.2.0/src/labs/my_first_ctf.yaml
+-rw-r--r--   0        0        0      300 2024-04-05 15:13:58.980554 jedha_cli-1.2.0/src/labs/my_second_ctf.yaml
+-rw-r--r--   0        0        0      352 2024-02-22 16:27:32.697771 jedha_cli-1.2.0/src/labs/path_traversal.yaml
+-rw-r--r--   0        0        0     2445 2024-03-15 13:38:48.454766 jedha_cli-1.2.0/src/labs/pentesting_network_services.yaml
+-rw-r--r--   0        0        0      322 2024-04-05 15:16:44.100841 jedha_cli-1.2.0/src/labs/pivoting-introduction.yaml
+-rw-r--r--   0        0        0      599 2024-04-05 15:16:44.100972 jedha_cli-1.2.0/src/labs/pivoting.yaml
+-rw-r--r--   0        0        0      280 2024-04-05 15:16:44.101115 jedha_cli-1.2.0/src/labs/reverse.yaml
+-rw-r--r--   0        0        0      284 2024-04-05 15:13:58.980672 jedha_cli-1.2.0/src/labs/sambacry.yaml
+-rw-r--r--   0        0        0      380 2024-02-22 16:27:32.698222 jedha_cli-1.2.0/src/labs/security_misconfiguration.yaml
+-rw-r--r--   0        0        0      290 2024-04-05 15:13:58.980788 jedha_cli-1.2.0/src/labs/shellshock.yaml
+-rw-r--r--   0        0        0      751 2024-03-13 10:00:54.999558 jedha_cli-1.2.0/src/labs/sqli.yaml
+-rw-r--r--   0        0        0      893 2024-02-22 16:27:32.698691 jedha_cli-1.2.0/src/labs/ssrf.yaml
+-rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699086 jedha_cli-1.2.0/src/labs/sudo_1.yaml
+-rw-r--r--   0        0        0      276 2024-03-20 09:49:04.648517 jedha_cli-1.2.0/src/labs/sudo_2.yaml
+-rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324618 jedha_cli-1.2.0/src/labs/sudo_3.yaml
+-rw-r--r--   0        0        0      272 2024-02-22 16:27:32.699334 jedha_cli-1.2.0/src/labs/suid.yaml
+-rw-r--r--   0        0        0      276 2024-01-25 10:09:15.324914 jedha_cli-1.2.0/src/labs/suid_2.yaml
+-rw-r--r--   0        0        0      628 2024-02-22 16:27:32.699456 jedha_cli-1.2.0/src/labs/template_injection.yaml
+-rw-r--r--   0        0        0      279 2024-04-05 15:13:58.980933 jedha_cli-1.2.0/src/labs/vim_fu.yaml
+-rw-r--r--   0        0        0      998 2024-04-05 15:13:58.981147 jedha_cli-1.2.0/src/labs/vuln_web_app.yaml
+-rw-r--r--   0        0        0     1119 2024-02-22 16:27:32.699708 jedha_cli-1.2.0/src/labs/vulnerable_and_outdated_software.yaml
+-rw-r--r--   0        0        0      290 2024-01-25 10:09:15.325298 jedha_cli-1.2.0/src/labs/wifi_wpa2_cracking.yaml
+-rw-r--r--   0        0        0      352 2024-01-25 10:09:15.325420 jedha_cli-1.2.0/src/labs/windows_box.yaml
+-rw-r--r--   0        0        0      320 2024-02-22 16:27:32.699823 jedha_cli-1.2.0/src/labs/xss.yaml
+-rw-r--r--   0        0        0     5075 2024-04-05 15:16:44.100417 jedha_cli-1.2.0/src/labs.yaml
+-rw-r--r--   0        0        0     9983 2024-04-05 15:13:58.981430 jedha_cli-1.2.0/src/main.py
+-rw-r--r--   0        0        0     6363 2024-03-13 14:11:35.442529 jedha_cli-1.2.0/src/misc.py
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 jedha_cli-1.2.0/PKG-INFO
```

### Comparing `jedha_cli-1.1.6/LICENSE` & `jedha_cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/README.md` & `jedha_cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/pyproject.toml` & `jedha_cli-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jedha-cli"
-version = "1.1.6"
+version = "1.2.0"
 description = "A CLI to start cybersecurity labs and practice your skills"
 authors = ["ademenet <alain@jedha.co>"]
 readme = "README.md"
 packages = [
     { include = "src" },
 ]
```

### Comparing `jedha_cli-1.1.6/src/labs/dns_zone_transfer.yaml` & `jedha_cli-1.2.0/src/labs/dns_zone_transfer.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/docker_evasion_1.yaml` & `jedha_cli-1.2.0/src/labs/docker_evasion_1.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/pentesting_network_services.yaml` & `jedha_cli-1.2.0/src/labs/pentesting_network_services.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/sqli.yaml` & `jedha_cli-1.2.0/src/labs/sqli.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/ssrf.yaml` & `jedha_cli-1.2.0/src/labs/ssrf.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/template_injection.yaml` & `jedha_cli-1.2.0/src/labs/template_injection.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/vuln_web_app.yaml` & `jedha_cli-1.2.0/src/labs/vuln_web_app.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs/vulnerable_and_outdated_software.yaml` & `jedha_cli-1.2.0/src/labs/vulnerable_and_outdated_software.yaml`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/src/labs.yaml` & `jedha_cli-1.2.0/src/labs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,29 @@
   description: 'Can you gain access on jedha-vps2? (username: "root", password: "PwnMe", port: 2222)'
 - name: hid
   ip: "10.10.3.38"
   description: "A Bettercap instance!"
 - name: wifi_wpa2_cracking
   ip: "10.10.3.47"
   description: '(username: "exploit", password: "aircrack")'
+- name: pivoting-introduction
+  ip: "10.10.5.91"
+  description: "A gentle introduction to pivoting!"
+- name: reverse
+  ip: "10.10.5.10"
+  description: "Can you get a reverse shell?"
+- name: pivoting
+  ip: "10.10.5.11"
+  description: "Pivot through the network!"
+- name: covering-tracks-linux
+  ip: "10.10.5.21"
+  description: "Cover your tracks on a Linux machine! Connect with SSH with charles:Jedha2022"
+# - name: covering-tracks
+#   ip: "10.10.5.24"
+#   description: "Connect using Telnet with exploit:PwnMe"
 - name: gash
   ip: "10.10.3.78"
   description: 'GameShell: a "game" to teach the Unix shell'
 - name: my_first_ctf
   ip: "10.10.10.11"
   description: 'Your first CTF! Can you find the 9 flags? (username: "root", password: "password")'
 - name: vim_fu
```

### Comparing `jedha_cli-1.1.6/src/main.py` & `jedha_cli-1.2.0/src/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/python3
 
 import os
 import subprocess
-from typing import Annotated, Optional
+from typing import Annotated, Optional, List
 
 import typer
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from yaml import safe_load
 
@@ -64,14 +64,43 @@
     filename_array = get_yaml_labs()
     table = Table("Name", "IP", "Description", show_lines=True, title="Available Labs")
     for i in filename_array:
         table.add_row(i["name"], i["ip"], i["description"])
     console.print(table)
 
 
+@app.command("dl", help="Download (but not start) one or more lab(s) environment.")
+def download(labnames: List[str]):
+    """
+    Download a lab.
+
+    Args:
+        labnames (List[str]): List of the lab names.
+    """
+    if not is_docker_running():
+        print("Docker is not running. Please start Docker and try again.")
+        raise typer.Exit(1)
+
+    for labname in labnames:
+        lab_config_file = get_lab_config_file(labname)
+        if not lab_config_file or not os.path.exists(lab_config_file):
+            print("Docker Compose file not found for the specified lab.")
+            return
+
+        try:
+            command = get_docker_compose_command(["--file", lab_config_file, "pull"])
+            subprocess.run(
+                command,
+                check=True,
+            )
+            print(f"Lab {labname} downloaded successfully.")
+        except subprocess.CalledProcessError as e:
+            print(f"Failed to download lab {labname}.")
+
+
 @app.command(
     "status",
     help="Show the running labs. If a lab name is provided, it will show the status of that lab.",
 )
 def status(labname: Annotated[Optional[str], typer.Argument()] = None):
     """
     Show the list of running labs.
```

### Comparing `jedha_cli-1.1.6/src/misc.py` & `jedha_cli-1.2.0/src/misc.py`

 * *Files identical despite different names*

### Comparing `jedha_cli-1.1.6/PKG-INFO` & `jedha_cli-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jedha-cli
-Version: 1.1.6
+Version: 1.2.0
 Summary: A CLI to start cybersecurity labs and practice your skills
 Author: ademenet
 Author-email: alain@jedha.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

