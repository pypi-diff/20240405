# Comparing `tmp/openobd-protocol-0.0.33.tar.gz` & `tmp/openobd-protocol-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-protocol-0.0.33.tar", last modified: Fri Mar 29 14:31:02 2024, max compression
+gzip compressed data, was "openobd-protocol-0.0.34.tar", last modified: Fri Apr  5 08:02:14 2024, max compression
```

## Comparing `openobd-protocol-0.0.33.tar` & `openobd-protocol-0.0.34.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.520406 openobd-protocol-0.0.33/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-29 14:31:02.520406 openobd-protocol-0.0.33/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 14:31:02.521406 openobd-protocol-0.0.33/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.456405 openobd-protocol-0.0.33/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.513405 openobd-protocol-0.0.33/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.516406 openobd-protocol-0.0.33/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2994 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/ModuleConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3706 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/ModuleConfiguration_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1958 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/ObdMessage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/ObdMessage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3032 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    14057 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.519406 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     2008 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6578 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3813 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-29 14:30:56.000000 openobd-protocol-0.0.33/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 14:31:02.520406 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-29 14:31:02.000000 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1485 2024-03-29 14:31:02.000000 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 14:31:02.000000 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-29 14:31:02.000000 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-29 14:31:02.000000 openobd-protocol-0.0.33/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.393140 openobd-protocol-0.0.34/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-05 08:02:14.392140 openobd-protocol-0.0.34/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 08:02:14.393140 openobd-protocol-0.0.34/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.376139 openobd-protocol-0.0.34/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.385140 openobd-protocol-0.0.34/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.388140 openobd-protocol-0.0.34/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    14057 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.391140 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6578 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.392140 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd-protocol-0.0.33/LICENSE` & `openobd-protocol-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/PKG-INFO` & `openobd-protocol-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.33
+Version: 0.0.34
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.33/pyproject.toml` & `openobd-protocol-0.0.34/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/Authentication_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/Authentication_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/BasicResponse_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/ModuleConfiguration_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/ModuleConfiguration_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/ObdMessage_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/ObdMessage_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/Status_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/Status_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2openobd_protocol/UserInterface/UserInterface.proto\x12+com.jifeline.OpenOBD.Protocol.UserInterface\x1a\x1dopenobd_protocol/Status.proto\"\xb0\x05\n\rUserInterface\x12J\n\x06target\x18\x01 \x01(\x0e\x32:.com.jifeline.OpenOBD.Protocol.UserInterface.InterfaceType\x12K\n\rcontrol_label\x18\x02 \x01(\x0b\x32\x32.com.jifeline.OpenOBD.Protocol.UserInterface.LabelH\x00\x12O\n\x0f\x63ontrol_options\x18\x03 \x01(\x0b\x32\x34.com.jifeline.OpenOBD.Protocol.UserInterface.OptionsH\x00\x12Q\n\x10\x63ontrol_continue\x18\x04 \x01(\x0b\x32\x35.com.jifeline.OpenOBD.Protocol.UserInterface.ContinueH\x00\x12K\n\rcontrol_yesno\x18\x05 \x01(\x0b\x32\x32.com.jifeline.OpenOBD.Protocol.UserInterface.YesNoH\x00\x12Q\n\x10\x63ontrol_freetext\x18\x06 \x01(\x0b\x32\x35.com.jifeline.OpenOBD.Protocol.UserInterface.FreeTextH\x00\x12N\n\x0e\x63ontrol_number\x18\x08 \x01(\x0b\x32\x34.com.jifeline.OpenOBD.Protocol.UserInterface.NumbersH\x00\x12I\n\x15user_interface_status\x18\x07 \x01(\x0b\x32%.com.jifeline.OpenOBD.Protocol.StatusH\x01\x88\x01\x01\x42\r\n\x0b\x43ontrolTypeB\x18\n\x16_user_interface_status\"R\n\x05Label\x12\r\n\x05label\x18\x01 \x01(\t\x12!\n\x14minimal_display_time\x18\x02 \x01(\rH\x00\x88\x01\x01\x42\x17\n\x15_minimal_display_time\"I\n\x07Options\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x03(\t\x12\x13\n\x06\x61nswer\x18\x03 \x01(\rH\x00\x88\x01\x01\x42\t\n\x07_answer\"\x19\n\x08\x43ontinue\x12\r\n\x05label\x18\x01 \x01(\t\"6\n\x05YesNo\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x61nswer\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\t\n\x07_answer\"9\n\x08\x46reeText\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x61nswer\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\t\n\x07_answer\"I\n\x07Numbers\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x03(\r\x12\x13\n\x06\x61nswer\x18\x03 \x01(\rH\x00\x88\x01\x01\x42\t\n\x07_answer*T\n\rInterfaceType\x12\x17\n\x13INTERFACE_UNDEFINED\x10\x00\x12\x12\n\x0eINTERFACE_USER\x10\x01\x12\x16\n\x12INTERFACE_OPERATOR\x10\x02\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2openobd_protocol/UserInterface/UserInterface.proto\x12+com.jifeline.OpenOBD.Protocol.UserInterface\x1a\x1dopenobd_protocol/Status.proto\"\xb0\x05\n\rUserInterface\x12J\n\x06target\x18\x01 \x01(\x0e\x32:.com.jifeline.OpenOBD.Protocol.UserInterface.InterfaceType\x12K\n\rcontrol_label\x18\x02 \x01(\x0b\x32\x32.com.jifeline.OpenOBD.Protocol.UserInterface.LabelH\x00\x12O\n\x0f\x63ontrol_options\x18\x03 \x01(\x0b\x32\x34.com.jifeline.OpenOBD.Protocol.UserInterface.OptionsH\x00\x12Q\n\x10\x63ontrol_continue\x18\x04 \x01(\x0b\x32\x35.com.jifeline.OpenOBD.Protocol.UserInterface.ContinueH\x00\x12K\n\rcontrol_yesno\x18\x05 \x01(\x0b\x32\x32.com.jifeline.OpenOBD.Protocol.UserInterface.YesNoH\x00\x12Q\n\x10\x63ontrol_freetext\x18\x06 \x01(\x0b\x32\x35.com.jifeline.OpenOBD.Protocol.UserInterface.FreeTextH\x00\x12N\n\x0e\x63ontrol_number\x18\x08 \x01(\x0b\x32\x34.com.jifeline.OpenOBD.Protocol.UserInterface.NumbersH\x00\x12I\n\x15user_interface_status\x18\x07 \x01(\x0b\x32%.com.jifeline.OpenOBD.Protocol.StatusH\x01\x88\x01\x01\x42\r\n\x0b\x43ontrolTypeB\x18\n\x16_user_interface_status\"t\n\x05Label\x12\r\n\x05label\x18\x01 \x01(\t\x12!\n\x14minimal_display_time\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\x17\n\x15_minimal_display_timeB\n\n\x08_timeout\"I\n\x07Options\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x03(\t\x12\x13\n\x06\x61nswer\x18\x03 \x01(\rH\x00\x88\x01\x01\x42\t\n\x07_answer\"\x19\n\x08\x43ontinue\x12\r\n\x05label\x18\x01 \x01(\t\"6\n\x05YesNo\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x61nswer\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\t\n\x07_answer\"9\n\x08\x46reeText\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x06\x61nswer\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\t\n\x07_answer\"Z\n\x07Numbers\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0f\n\x07minimum\x18\x02 \x01(\r\x12\x13\n\x06\x61nswer\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x0f\n\x07maximum\x18\x04 \x01(\rB\t\n\x07_answer*T\n\rInterfaceType\x12\x17\n\x13INTERFACE_UNDEFINED\x10\x00\x12\x12\n\x0eINTERFACE_USER\x10\x01\x12\x16\n\x12INTERFACE_OPERATOR\x10\x02\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.UserInterface.UserInterface_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_INTERFACETYPE']._serialized_start=1197
-  _globals['_INTERFACETYPE']._serialized_end=1281
+  _globals['_INTERFACETYPE']._serialized_start=1248
+  _globals['_INTERFACETYPE']._serialized_end=1332
   _globals['_USERINTERFACE']._serialized_start=131
   _globals['_USERINTERFACE']._serialized_end=819
   _globals['_LABEL']._serialized_start=821
-  _globals['_LABEL']._serialized_end=903
-  _globals['_OPTIONS']._serialized_start=905
-  _globals['_OPTIONS']._serialized_end=978
-  _globals['_CONTINUE']._serialized_start=980
-  _globals['_CONTINUE']._serialized_end=1005
-  _globals['_YESNO']._serialized_start=1007
-  _globals['_YESNO']._serialized_end=1061
-  _globals['_FREETEXT']._serialized_start=1063
-  _globals['_FREETEXT']._serialized_end=1120
-  _globals['_NUMBERS']._serialized_start=1122
-  _globals['_NUMBERS']._serialized_end=1195
+  _globals['_LABEL']._serialized_end=937
+  _globals['_OPTIONS']._serialized_start=939
+  _globals['_OPTIONS']._serialized_end=1012
+  _globals['_CONTINUE']._serialized_start=1014
+  _globals['_CONTINUE']._serialized_end=1039
+  _globals['_YESNO']._serialized_start=1041
+  _globals['_YESNO']._serialized_end=1095
+  _globals['_FREETEXT']._serialized_start=1097
+  _globals['_FREETEXT']._serialized_end=1154
+  _globals['_NUMBERS']._serialized_start=1156
+  _globals['_NUMBERS']._serialized_end=1246
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,22 @@
     control_yesno: YesNo
     control_freetext: FreeText
     control_number: Numbers
     user_interface_status: _Status_pb2.Status
     def __init__(self, target: _Optional[_Union[InterfaceType, str]] = ..., control_label: _Optional[_Union[Label, _Mapping]] = ..., control_options: _Optional[_Union[Options, _Mapping]] = ..., control_continue: _Optional[_Union[Continue, _Mapping]] = ..., control_yesno: _Optional[_Union[YesNo, _Mapping]] = ..., control_freetext: _Optional[_Union[FreeText, _Mapping]] = ..., control_number: _Optional[_Union[Numbers, _Mapping]] = ..., user_interface_status: _Optional[_Union[_Status_pb2.Status, _Mapping]] = ...) -> None: ...
 
 class Label(_message.Message):
-    __slots__ = ("label", "minimal_display_time")
+    __slots__ = ("label", "minimal_display_time", "timeout")
     LABEL_FIELD_NUMBER: _ClassVar[int]
     MINIMAL_DISPLAY_TIME_FIELD_NUMBER: _ClassVar[int]
+    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     label: str
     minimal_display_time: int
-    def __init__(self, label: _Optional[str] = ..., minimal_display_time: _Optional[int] = ...) -> None: ...
+    timeout: int
+    def __init__(self, label: _Optional[str] = ..., minimal_display_time: _Optional[int] = ..., timeout: _Optional[int] = ...) -> None: ...
 
 class Options(_message.Message):
     __slots__ = ("label", "options", "answer")
     LABEL_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     ANSWER_FIELD_NUMBER: _ClassVar[int]
     label: str
@@ -73,15 +75,17 @@
     LABEL_FIELD_NUMBER: _ClassVar[int]
     ANSWER_FIELD_NUMBER: _ClassVar[int]
     label: str
     answer: str
     def __init__(self, label: _Optional[str] = ..., answer: _Optional[str] = ...) -> None: ...
 
 class Numbers(_message.Message):
-    __slots__ = ("label", "options", "answer")
+    __slots__ = ("label", "minimum", "answer", "maximum")
     LABEL_FIELD_NUMBER: _ClassVar[int]
-    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    MINIMUM_FIELD_NUMBER: _ClassVar[int]
     ANSWER_FIELD_NUMBER: _ClassVar[int]
+    MAXIMUM_FIELD_NUMBER: _ClassVar[int]
     label: str
-    options: _containers.RepeatedScalarFieldContainer[int]
+    minimum: int
     answer: int
-    def __init__(self, label: _Optional[str] = ..., options: _Optional[_Iterable[int]] = ..., answer: _Optional[int] = ...) -> None: ...
+    maximum: int
+    def __init__(self, label: _Optional[str] = ..., minimum: _Optional[int] = ..., answer: _Optional[int] = ..., maximum: _Optional[int] = ...) -> None: ...
```

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol.egg-info/PKG-INFO` & `openobd-protocol-0.0.34/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.33
+Version: 0.0.34
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.33/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd-protocol-0.0.34/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

