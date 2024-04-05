# Comparing `tmp/komo-0.2.8.tar.gz` & `tmp/komo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komo-0.2.8.tar", last modified: Sun Mar 31 23:05:58 2024, max compression
+gzip compressed data, was "komo-0.2.9.tar", last modified: Mon Apr  1 00:51:49 2024, max compression
```

## Comparing `komo-0.2.8.tar` & `komo-0.2.9.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.770792 komo-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-31 23:05:58.770792 komo-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-31 23:05:46.000000 komo-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.762792 komo-0.2.8/komo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-31 23:05:46.000000 komo-0.2.8/komo/agent/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    16805 2024-03-31 23:05:46.000000 komo-0.2.8/komo/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-03-31 23:05:46.000000 komo-0.2.8/komo/aws/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo/cli/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/agent/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/agent/cmd_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/agent/cmd_setup_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo/cli/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/aws/cmd_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/cmd_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.770792 komo-0.2.8/komo/cli/machine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/cmd_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/cmd_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/cmd_terminate.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/cmd_vscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-31 23:05:46.000000 komo-0.2.8/komo/cli/machine/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 23:05:46.000000 komo-0.2.8/komo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-03-31 23:05:46.000000 komo-0.2.8/komo/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-31 23:05:46.000000 komo-0.2.8/komo/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-31 23:05:46.000000 komo-0.2.8/komo/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-31 23:05:46.000000 komo-0.2.8/komo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:05:58.766792 komo-0.2.8/komo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 23:05:58.000000 komo-0.2.8/komo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-31 23:05:58.770792 komo-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-31 23:05:46.000000 komo-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.940222 komo-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 00:51:49.940222 komo-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-01 00:51:37.000000 komo-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.936221 komo-0.2.9/komo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.936221 komo-0.2.9/komo/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-01 00:51:37.000000 komo-0.2.9/komo/agent/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16805 2024-04-01 00:51:37.000000 komo-0.2.9/komo/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.936221 komo-0.2.9/komo/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-01 00:51:37.000000 komo-0.2.9/komo/aws/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.940222 komo-0.2.9/komo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.940222 komo-0.2.9/komo/cli/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/agent/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/agent/cmd_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/agent/cmd_setup_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.940222 komo-0.2.9/komo/cli/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/aws/cmd_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/cmd_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.940222 komo-0.2.9/komo/cli/machine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_setup_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_terminate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/cmd_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-01 00:51:37.000000 komo-0.2.9/komo/cli/machine/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 00:51:37.000000 komo-0.2.9/komo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-01 00:51:37.000000 komo-0.2.9/komo/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 00:51:37.000000 komo-0.2.9/komo/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-01 00:51:37.000000 komo-0.2.9/komo/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-01 00:51:37.000000 komo-0.2.9/komo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:51:49.936221 komo-0.2.9/komo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 00:51:49.000000 komo-0.2.9/komo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 00:51:49.940222 komo-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-01 00:51:37.000000 komo-0.2.9/setup.py
```

### Comparing `komo-0.2.8/PKG-INFO` & `komo-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: komo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Komodo AI CLI
 Home-page: https://github.com/anishchopra/komo
 Author: Anish Chopra
 Author-email: anish@komodoai.dev
 License: BSD
 Description: 
         Komodo AI CLI
```

### Comparing `komo-0.2.8/komo/agent/core.py` & `komo-0.2.9/komo/agent/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     with tempfile.TemporaryDirectory() as td:
         script_file = os.path.join(td, "script.sh")
 
         with open(script_file, "w") as f:
             f.write(script)
 
         proc = subprocess.Popen(
-            ["/bin/sh", script_file],
+            ["bash", "-l", script_file],
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
 
         for line in proc.stdout:
             logger.log(line.decode("utf-8"))
```

### Comparing `komo-0.2.8/komo/api_client.py` & `komo-0.2.9/komo/api_client.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/aws/connect.py` & `komo-0.2.9/komo/aws/connect.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/cli/cli.py` & `komo-0.2.9/komo/cli/cli.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/cli/cmd_list.py` & `komo-0.2.9/komo/cli/cmd_list.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/cli/cmd_run.py` & `komo-0.2.9/komo/cli/cmd_run.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/cli/machine/cmd_create.py` & `komo-0.2.9/komo/cli/machine/cmd_create.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/cli/machine/cmd_list.py` & `komo-0.2.9/komo/cli/machine/cmd_list.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/core.py` & `komo-0.2.9/komo/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,17 @@
 def get_machine_notebook_url(machine_name):
     api_client = APIClient()
 
     machine = api_client.get_machine(machine_name)
     host_info = api_client.get_machine_host_info(machine_name)
     host_name = host_info["host_name"]
 
+    if not host_name.startswith("http"):
+        host_name = f"http://{host_name}"
+
     url = f"{host_name}:8888?token={machine.notebook_token}"
     return url
 
 
 def print_machine_setup_logs(machine_name: str, follow: bool):
     api_client = APIClient()
     machine = api_client.get_machine(machine_name)
```

### Comparing `komo-0.2.8/komo/types.py` & `komo-0.2.9/komo/types.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo/utils.py` & `komo-0.2.9/komo/utils.py`

 * *Files identical despite different names*

### Comparing `komo-0.2.8/komo.egg-info/PKG-INFO` & `komo-0.2.9/komo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: komo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Komodo AI CLI
 Home-page: https://github.com/anishchopra/komo
 Author: Anish Chopra
 Author-email: anish@komodoai.dev
 License: BSD
 Description: 
         Komodo AI CLI
```

### Comparing `komo-0.2.8/komo.egg-info/SOURCES.txt` & `komo-0.2.9/komo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,11 +35,13 @@
 komo/cli/agent/cmd_setup_machine.py
 komo/cli/aws/__init__.py
 komo/cli/aws/aws.py
 komo/cli/aws/cmd_connect.py
 komo/cli/machine/__init__.py
 komo/cli/machine/cmd_create.py
 komo/cli/machine/cmd_list.py
+komo/cli/machine/cmd_notebook.py
+komo/cli/machine/cmd_setup_logs.py
 komo/cli/machine/cmd_ssh.py
 komo/cli/machine/cmd_terminate.py
 komo/cli/machine/cmd_vscode.py
 komo/cli/machine/machine.py
```

### Comparing `komo-0.2.8/setup.py` & `komo-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt", "r") as f:
     dependencies = f.readlines()
 
 setup(
     name="komo",
-    version="0.2.8",
+    version="0.2.9",
     url="https://github.com/anishchopra/komo",
     license="BSD",
     author="Anish Chopra",
     author_email="anish@komodoai.dev",
     description="Komodo AI CLI",
     long_description=__doc__,
     packages=find_packages(exclude=["tests", "komoproj.yaml"], include=["*"]),
```

