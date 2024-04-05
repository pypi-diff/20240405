# Comparing `tmp/shipyard_sftp-0.3.1.tar.gz` & `tmp/shipyard_sftp-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sftp-0.3.1.tar", max compression
+gzip compressed data, was "shipyard_sftp-0.3.1a0.tar", max compression
```

## Comparing `shipyard_sftp-0.3.1.tar` & `shipyard_sftp-0.3.1a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.3.1/README.md
--rw-r--r--   0        0        0      551 2024-04-05 19:32:29.480602 shipyard_sftp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.3.1/shipyard_sftp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.3.1/shipyard_sftp/cli/__init__.py
--rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.3.1/shipyard_sftp/cli/authtest.py
--rw-r--r--   0        0        0     3363 2024-04-04 19:39:49.116994 shipyard_sftp-0.3.1/shipyard_sftp/cli/delete_file.py
--rw-r--r--   0        0        0     4130 2024-04-05 19:33:27.343854 shipyard_sftp-0.3.1/shipyard_sftp/cli/download_file.py
--rw-r--r--   0        0        0     4027 2024-04-04 19:39:49.117861 shipyard_sftp-0.3.1/shipyard_sftp/cli/move_file.py
--rw-r--r--   0        0        0     3387 2024-04-04 19:39:49.118165 shipyard_sftp-0.3.1/shipyard_sftp/cli/upload_file.py
--rw-r--r--   0        0        0     3387 2024-04-04 15:32:48.428604 shipyard_sftp-0.3.1/shipyard_sftp/exceptions.py
--rw-r--r--   0        0        0    14108 2024-04-05 19:24:34.339285 shipyard_sftp-0.3.1/shipyard_sftp/sftp.py
--rw-r--r--   0        0        0     1638 2024-04-04 15:32:48.429805 shipyard_sftp-0.3.1/shipyard_sftp/utils.py
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 shipyard_sftp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.3.1a0/README.md
+-rw-r--r--   0        0        0      553 2024-04-05 19:24:46.730311 shipyard_sftp-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.3.1a0/shipyard_sftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/__init__.py
+-rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/authtest.py
+-rw-r--r--   0        0        0     3363 2024-04-04 19:39:49.116994 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/delete_file.py
+-rw-r--r--   0        0        0     4160 2024-04-05 19:24:34.330870 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/download_file.py
+-rw-r--r--   0        0        0     4027 2024-04-04 19:39:49.117861 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/move_file.py
+-rw-r--r--   0        0        0     3387 2024-04-04 19:39:49.118165 shipyard_sftp-0.3.1a0/shipyard_sftp/cli/upload_file.py
+-rw-r--r--   0        0        0     3387 2024-04-04 15:32:48.428604 shipyard_sftp-0.3.1a0/shipyard_sftp/exceptions.py
+-rw-r--r--   0        0        0    14108 2024-04-05 19:24:34.339285 shipyard_sftp-0.3.1a0/shipyard_sftp/sftp.py
+-rw-r--r--   0        0        0     1638 2024-04-04 15:32:48.429805 shipyard_sftp-0.3.1a0/shipyard_sftp/utils.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.3.1a0/PKG-INFO
```

### Comparing `shipyard_sftp-0.3.1/pyproject.toml` & `shipyard_sftp-0.3.1a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sftp"
-version = "0.3.1"
+version = "0.3.1a0"
 description = "A local client for connecting and working with SFTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_sftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/cli/delete_file.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/cli/delete_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/cli/download_file.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/cli/download_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     sftp = None
     try:
         args = get_args()
 
         try:
             connection_args, key_path = setup_connection(args)
 
-            if args.password:
+            if args.password: # Use password authentication
                 transport = paramiko.Transport((args.host, int(args.port)))
                 transport.default_window_size = DEFAULT_WINDOW_SIZE
                 transport.packetizer.REKEY_BYTES = DEFAULT_REKEY_BYTES
                 transport.packetizer.REKEY_PACKETS = DEFAULT_REKEY_PACKETS
                 transport.connect(None, args.username, args.password)
                 connection_args["transport"] = transport
```

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/cli/move_file.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/cli/move_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/cli/upload_file.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/cli/upload_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/exceptions.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/sftp.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/sftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/shipyard_sftp/utils.py` & `shipyard_sftp-0.3.1a0/shipyard_sftp/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.3.1/PKG-INFO` & `shipyard_sftp-0.3.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sftp
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: A local client for connecting and working with SFTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

