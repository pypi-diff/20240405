# Comparing `tmp/xgt-1.8.0.tar.gz` & `tmp/xgt-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xgt-1.8.0.tar", last modified: Mon Aug 30 22:54:10 2021, max compression
+gzip compressed data, was "xgt-1.9.0.tar", last modified: Tue Nov  2 20:21:14 2021, max compression
```

## Comparing `xgt-1.8.0.tar` & `xgt-1.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 centos    (1000) centos    (1000)        0 2021-08-30 22:54:10.000000 xgt-1.8.0/
-drwxrwxr-x   0 centos    (1000) centos    (1000)        0 2021-08-30 22:54:10.000000 xgt-1.8.0/src/
-drwxrwxr-x   0 centos    (1000) centos    (1000)        0 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt/
-drwxrwxr-x   0 centos    (1000) centos    (1000)        0 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt/admin/
--rw-rw-r--   0 centos    (1000) centos    (1000)     1630 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/admin/__init__.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    48586 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/AdminService_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    18386 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/AdminService_pb2_grpc.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    44039 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/DataService_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     7098 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/DataService_pb2_grpc.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     7072 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/ErrorMessages_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    62521 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/GraphTypesService_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    18857 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/GraphTypesService_pb2_grpc.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    30973 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/JobService_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     7065 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/JobService_pb2_grpc.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     8927 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/MetricsService_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     4163 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/MetricsService_pb2_grpc.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    32154 2021-08-30 22:36:16.000000 xgt-1.8.0/src/xgt/SchemaMessages_pb2.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     7785 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/__init__.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     7662 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/common.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    65635 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/connection.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    52457 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/graph.py
--rw-rw-r--   0 centos    (1000) centos    (1000)    19396 2021-08-30 22:36:14.000000 xgt-1.8.0/src/xgt/job.py
--rw-rw-r--   0 centos    (1000) centos    (1000)      324 2021-08-30 22:35:46.000000 xgt-1.8.0/src/xgt/version.py
-drwxrwxr-x   0 centos    (1000) centos    (1000)        0 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/
--rw-rw-r--   0 centos    (1000) centos    (1000)     1107 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/PKG-INFO
--rw-rw-r--   0 centos    (1000) centos    (1000)      707 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/SOURCES.txt
--rw-rw-r--   0 centos    (1000) centos    (1000)        1 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/dependency_links.txt
--rw-rw-r--   0 centos    (1000) centos    (1000)       53 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/requires.txt
--rw-rw-r--   0 centos    (1000) centos    (1000)        4 2021-08-30 22:54:10.000000 xgt-1.8.0/src/xgt.egg-info/top_level.txt
--rw-rw-r--   0 centos    (1000) centos    (1000)       51 2021-08-30 22:36:15.000000 xgt-1.8.0/MANIFEST.in
--rw-rw-r--   0 centos    (1000) centos    (1000)      505 2021-08-30 22:36:15.000000 xgt-1.8.0/README
--rw-rw-r--   0 centos    (1000) centos    (1000)       53 2021-08-30 22:36:15.000000 xgt-1.8.0/requirements.txt
--rw-rw-r--   0 centos    (1000) centos    (1000)     2309 2021-08-30 22:35:46.000000 xgt-1.8.0/setup.py
--rw-rw-r--   0 centos    (1000) centos    (1000)     1107 2021-08-30 22:54:10.000000 xgt-1.8.0/PKG-INFO
--rw-rw-r--   0 centos    (1000) centos    (1000)       38 2021-08-30 22:54:10.000000 xgt-1.8.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-02 20:21:14.918541 xgt-1.9.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       51 2021-11-02 19:56:21.000000 xgt-1.9.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2021-11-02 20:21:14.914540 xgt-1.9.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      505 2021-11-02 19:56:21.000000 xgt-1.9.0/README
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2021-11-02 19:56:21.000000 xgt-1.9.0/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-11-02 20:21:14.918541 xgt-1.9.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2021-11-02 19:56:01.000000 xgt-1.9.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-02 20:21:14.910540 xgt-1.9.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-02 20:21:14.914540 xgt-1.9.0/src/xgt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48586 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/AdminService_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18386 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/AdminService_pb2_grpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    44039 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/DataService_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7098 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/DataService_pb2_grpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7072 2021-11-02 19:56:18.000000 xgt-1.9.0/src/xgt/ErrorMessages_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    62521 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/GraphTypesService_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18857 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/GraphTypesService_pb2_grpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22206 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/JobService_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7065 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/JobService_pb2_grpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8927 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/MetricsService_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/MetricsService_pb2_grpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42022 2021-11-02 19:56:21.000000 xgt-1.9.0/src/xgt/SchemaMessages_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2021-11-02 19:56:17.000000 xgt-1.9.0/src/xgt/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-02 20:21:14.914540 xgt-1.9.0/src/xgt/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2021-11-02 19:56:17.000000 xgt-1.9.0/src/xgt/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2021-11-02 19:56:17.000000 xgt-1.9.0/src/xgt/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    69246 2021-11-02 19:56:17.000000 xgt-1.9.0/src/xgt/connection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52669 2021-11-02 19:56:17.000000 xgt-1.9.0/src/xgt/graph.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19372 2021-11-02 19:56:18.000000 xgt-1.9.0/src/xgt/job.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      324 2021-11-02 19:56:01.000000 xgt-1.9.0/src/xgt/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-02 20:21:14.914540 xgt-1.9.0/src/xgt.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2021-11-02 20:21:14.000000 xgt-1.9.0/src/xgt.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      707 2021-11-02 20:21:14.000000 xgt-1.9.0/src/xgt.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-11-02 20:21:14.000000 xgt-1.9.0/src/xgt.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2021-11-02 20:21:14.000000 xgt-1.9.0/src/xgt.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2021-11-02 20:21:14.000000 xgt-1.9.0/src/xgt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xgt-1.8.0/src/xgt/admin/__init__.py` & `xgt-1.9.0/src/xgt/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/AdminService_pb2.py` & `xgt-1.9.0/src/xgt/AdminService_pb2.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/AdminService_pb2_grpc.py` & `xgt-1.9.0/src/xgt/AdminService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/DataService_pb2.py` & `xgt-1.9.0/src/xgt/DataService_pb2.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/DataService_pb2_grpc.py` & `xgt-1.9.0/src/xgt/DataService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/ErrorMessages_pb2.py` & `xgt-1.9.0/src/xgt/ErrorMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/GraphTypesService_pb2.py` & `xgt-1.9.0/src/xgt/GraphTypesService_pb2.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/GraphTypesService_pb2_grpc.py` & `xgt-1.9.0/src/xgt/GraphTypesService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/JobService_pb2.py` & `xgt-1.9.0/src/xgt/JobService_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: JobService.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
@@ -19,191 +18,19 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='JobService.proto',
   package='xgt',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x10JobService.proto\x12\x03xgt\x1a\x12\x41\x64minService.proto\x1a\x13\x45rrorMessages.proto\x1a\x14SchemaMessages.proto\"\xc3\x01\n\x10QueryEdgeMessage\x12/\n\x0e\x65\x64ge_direction\x18\x01 \x01(\x0e\x32\x17.xgt.QueryEdgeDirection\x12\x12\n\nedge_label\x18\x02 \x01(\t\x12\x12\n\nedge_frame\x18\x03 \x01(\t\x12\x14\n\x0csource_label\x18\x04 \x01(\t\x12\x14\n\x0csource_frame\x18\x05 \x01(\t\x12\x14\n\x0ctarget_label\x18\x06 \x01(\t\x12\x14\n\x0ctarget_frame\x18\x07 \x01(\t\"5\n\rQueryEdgeList\x12$\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x15.xgt.QueryEdgeMessage\":\n\tQueryPlan\x12-\n\x11plan_as_edge_list\x18\x01 \x03(\x0b\x32\x12.xgt.QueryEdgeList\"\xb7\x02\n\x19ScheduleJobsCypherRequest\x12\x14\n\x0c\x63ypher_query\x18\x01 \x03(\t\x12:\n\x06kwargs\x18\x05 \x03(\x0b\x32*.xgt.ScheduleJobsCypherRequest.KwargsEntry\x12\x42\n\nparameters\x18\x06 \x03(\x0b\x32..xgt.ScheduleJobsCypherRequest.ParametersEntry\x1a?\n\x0bKwargsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.xgt.ConfigValue:\x02\x38\x01\x1a\x43\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.xgt.ConfigValue:\x02\x38\x01\"\x7f\n\x1aScheduleJobsCypherResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus\x12\"\n\nquery_plan\x18\x03 \x01(\x0b\x32\x0e.xgt.QueryPlan\"#\n\x11\x43\x61ncelJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\"S\n\x12\x43\x61ncelJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus\" \n\x0eGetJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\"P\n\x0fGetJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x01(\x0b\x32\x0e.xgt.JobStatus\"2\n\x0fWaitJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\x12\x0f\n\x07timeout\x18\x02 \x01(\x03\"Q\n\x10WaitJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus*=\n\x12QueryEdgeDirection\x12\x0b\n\x07\x46ORWARD\x10\x00\x12\x0c\n\x08\x42\x41\x43KWARD\x10\x01\x12\x0c\n\x08NOT_EDGE\x10\x02\x32\x9b\x02\n\nJobService\x12W\n\x12ScheduleJobsCypher\x12\x1e.xgt.ScheduleJobsCypherRequest\x1a\x1f.xgt.ScheduleJobsCypherResponse\"\x00\x12?\n\nCancelJobs\x12\x16.xgt.CancelJobsRequest\x1a\x17.xgt.CancelJobsResponse\"\x00\x12\x38\n\x07GetJobs\x12\x13.xgt.GetJobsRequest\x1a\x14.xgt.GetJobsResponse\"\x00\x30\x01\x12\x39\n\x08WaitJobs\x12\x14.xgt.WaitJobsRequest\x1a\x15.xgt.WaitJobsResponse\"\x00\x62\x06proto3'
+  serialized_pb=b'\n\x10JobService.proto\x12\x03xgt\x1a\x12\x41\x64minService.proto\x1a\x13\x45rrorMessages.proto\x1a\x14SchemaMessages.proto\"\xb7\x02\n\x19ScheduleJobsCypherRequest\x12\x14\n\x0c\x63ypher_query\x18\x01 \x03(\t\x12:\n\x06kwargs\x18\x05 \x03(\x0b\x32*.xgt.ScheduleJobsCypherRequest.KwargsEntry\x12\x42\n\nparameters\x18\x06 \x03(\x0b\x32..xgt.ScheduleJobsCypherRequest.ParametersEntry\x1a?\n\x0bKwargsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.xgt.ConfigValue:\x02\x38\x01\x1a\x43\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.xgt.ConfigValue:\x02\x38\x01\"[\n\x1aScheduleJobsCypherResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus\"#\n\x11\x43\x61ncelJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\"S\n\x12\x43\x61ncelJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus\" \n\x0eGetJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\"P\n\x0fGetJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x01(\x0b\x32\x0e.xgt.JobStatus\"2\n\x0fWaitJobsRequest\x12\x0e\n\x06job_id\x18\x01 \x03(\x04\x12\x0f\n\x07timeout\x18\x02 \x01(\x03\"Q\n\x10WaitJobsResponse\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\"\n\njob_status\x18\x02 \x03(\x0b\x32\x0e.xgt.JobStatus2\x9b\x02\n\nJobService\x12W\n\x12ScheduleJobsCypher\x12\x1e.xgt.ScheduleJobsCypherRequest\x1a\x1f.xgt.ScheduleJobsCypherResponse\"\x00\x12?\n\nCancelJobs\x12\x16.xgt.CancelJobsRequest\x1a\x17.xgt.CancelJobsResponse\"\x00\x12\x38\n\x07GetJobs\x12\x13.xgt.GetJobsRequest\x1a\x14.xgt.GetJobsResponse\"\x00\x30\x01\x12\x39\n\x08WaitJobs\x12\x14.xgt.WaitJobsRequest\x1a\x15.xgt.WaitJobsResponse\"\x00\x62\x06proto3'
   ,
   dependencies=[AdminService__pb2.DESCRIPTOR,ErrorMessages__pb2.DESCRIPTOR,SchemaMessages__pb2.DESCRIPTOR,])
 
-_QUERYEDGEDIRECTION = _descriptor.EnumDescriptor(
-  name='QueryEdgeDirection',
-  full_name='xgt.QueryEdgeDirection',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='FORWARD', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='BACKWARD', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='NOT_EDGE', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=1217,
-  serialized_end=1278,
-)
-_sym_db.RegisterEnumDescriptor(_QUERYEDGEDIRECTION)
 
-QueryEdgeDirection = enum_type_wrapper.EnumTypeWrapper(_QUERYEDGEDIRECTION)
-FORWARD = 0
-BACKWARD = 1
-NOT_EDGE = 2
-
-
-
-_QUERYEDGEMESSAGE = _descriptor.Descriptor(
-  name='QueryEdgeMessage',
-  full_name='xgt.QueryEdgeMessage',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='edge_direction', full_name='xgt.QueryEdgeMessage.edge_direction', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='edge_label', full_name='xgt.QueryEdgeMessage.edge_label', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='edge_frame', full_name='xgt.QueryEdgeMessage.edge_frame', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='source_label', full_name='xgt.QueryEdgeMessage.source_label', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='source_frame', full_name='xgt.QueryEdgeMessage.source_frame', index=4,
-      number=5, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='target_label', full_name='xgt.QueryEdgeMessage.target_label', index=5,
-      number=6, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='target_frame', full_name='xgt.QueryEdgeMessage.target_frame', index=6,
-      number=7, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=89,
-  serialized_end=284,
-)
-
-
-_QUERYEDGELIST = _descriptor.Descriptor(
-  name='QueryEdgeList',
-  full_name='xgt.QueryEdgeList',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='edges', full_name='xgt.QueryEdgeList.edges', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=286,
-  serialized_end=339,
-)
-
-
-_QUERYPLAN = _descriptor.Descriptor(
-  name='QueryPlan',
-  full_name='xgt.QueryPlan',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='plan_as_edge_list', full_name='xgt.QueryPlan.plan_as_edge_list', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=341,
-  serialized_end=399,
-)
 
 
 _SCHEDULEJOBSCYPHERREQUEST_KWARGSENTRY = _descriptor.Descriptor(
   name='KwargsEntry',
   full_name='xgt.ScheduleJobsCypherRequest.KwargsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -232,16 +59,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=581,
-  serialized_end=644,
+  serialized_start=268,
+  serialized_end=331,
 )
 
 _SCHEDULEJOBSCYPHERREQUEST_PARAMETERSENTRY = _descriptor.Descriptor(
   name='ParametersEntry',
   full_name='xgt.ScheduleJobsCypherRequest.ParametersEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -270,16 +97,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=646,
-  serialized_end=713,
+  serialized_start=333,
+  serialized_end=400,
 )
 
 _SCHEDULEJOBSCYPHERREQUEST = _descriptor.Descriptor(
   name='ScheduleJobsCypherRequest',
   full_name='xgt.ScheduleJobsCypherRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -315,16 +142,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=402,
-  serialized_end=713,
+  serialized_start=89,
+  serialized_end=400,
 )
 
 
 _SCHEDULEJOBSCYPHERRESPONSE = _descriptor.Descriptor(
   name='ScheduleJobsCypherResponse',
   full_name='xgt.ScheduleJobsCypherResponse',
   filename=None,
@@ -342,35 +169,28 @@
     _descriptor.FieldDescriptor(
       name='job_status', full_name='xgt.ScheduleJobsCypherResponse.job_status', index=1,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='query_plan', full_name='xgt.ScheduleJobsCypherResponse.query_plan', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=715,
-  serialized_end=842,
+  serialized_start=402,
+  serialized_end=493,
 )
 
 
 _CANCELJOBSREQUEST = _descriptor.Descriptor(
   name='CancelJobsRequest',
   full_name='xgt.CancelJobsRequest',
   filename=None,
@@ -393,16 +213,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=844,
-  serialized_end=879,
+  serialized_start=495,
+  serialized_end=530,
 )
 
 
 _CANCELJOBSRESPONSE = _descriptor.Descriptor(
   name='CancelJobsResponse',
   full_name='xgt.CancelJobsResponse',
   filename=None,
@@ -432,16 +252,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=881,
-  serialized_end=964,
+  serialized_start=532,
+  serialized_end=615,
 )
 
 
 _GETJOBSREQUEST = _descriptor.Descriptor(
   name='GetJobsRequest',
   full_name='xgt.GetJobsRequest',
   filename=None,
@@ -464,16 +284,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=966,
-  serialized_end=998,
+  serialized_start=617,
+  serialized_end=649,
 )
 
 
 _GETJOBSRESPONSE = _descriptor.Descriptor(
   name='GetJobsResponse',
   full_name='xgt.GetJobsResponse',
   filename=None,
@@ -503,16 +323,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1000,
-  serialized_end=1080,
+  serialized_start=651,
+  serialized_end=731,
 )
 
 
 _WAITJOBSREQUEST = _descriptor.Descriptor(
   name='WaitJobsRequest',
   full_name='xgt.WaitJobsRequest',
   filename=None,
@@ -542,16 +362,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1082,
-  serialized_end=1132,
+  serialized_start=733,
+  serialized_end=783,
 )
 
 
 _WAITJOBSRESPONSE = _descriptor.Descriptor(
   name='WaitJobsResponse',
   full_name='xgt.WaitJobsResponse',
   filename=None,
@@ -581,71 +401,42 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1134,
-  serialized_end=1215,
+  serialized_start=785,
+  serialized_end=866,
 )
 
-_QUERYEDGEMESSAGE.fields_by_name['edge_direction'].enum_type = _QUERYEDGEDIRECTION
-_QUERYEDGELIST.fields_by_name['edges'].message_type = _QUERYEDGEMESSAGE
-_QUERYPLAN.fields_by_name['plan_as_edge_list'].message_type = _QUERYEDGELIST
 _SCHEDULEJOBSCYPHERREQUEST_KWARGSENTRY.fields_by_name['value'].message_type = AdminService__pb2._CONFIGVALUE
 _SCHEDULEJOBSCYPHERREQUEST_KWARGSENTRY.containing_type = _SCHEDULEJOBSCYPHERREQUEST
 _SCHEDULEJOBSCYPHERREQUEST_PARAMETERSENTRY.fields_by_name['value'].message_type = AdminService__pb2._CONFIGVALUE
 _SCHEDULEJOBSCYPHERREQUEST_PARAMETERSENTRY.containing_type = _SCHEDULEJOBSCYPHERREQUEST
 _SCHEDULEJOBSCYPHERREQUEST.fields_by_name['kwargs'].message_type = _SCHEDULEJOBSCYPHERREQUEST_KWARGSENTRY
 _SCHEDULEJOBSCYPHERREQUEST.fields_by_name['parameters'].message_type = _SCHEDULEJOBSCYPHERREQUEST_PARAMETERSENTRY
 _SCHEDULEJOBSCYPHERRESPONSE.fields_by_name['error'].message_type = ErrorMessages__pb2._ERROR
 _SCHEDULEJOBSCYPHERRESPONSE.fields_by_name['job_status'].message_type = SchemaMessages__pb2._JOBSTATUS
-_SCHEDULEJOBSCYPHERRESPONSE.fields_by_name['query_plan'].message_type = _QUERYPLAN
 _CANCELJOBSRESPONSE.fields_by_name['error'].message_type = ErrorMessages__pb2._ERROR
 _CANCELJOBSRESPONSE.fields_by_name['job_status'].message_type = SchemaMessages__pb2._JOBSTATUS
 _GETJOBSRESPONSE.fields_by_name['error'].message_type = ErrorMessages__pb2._ERROR
 _GETJOBSRESPONSE.fields_by_name['job_status'].message_type = SchemaMessages__pb2._JOBSTATUS
 _WAITJOBSRESPONSE.fields_by_name['error'].message_type = ErrorMessages__pb2._ERROR
 _WAITJOBSRESPONSE.fields_by_name['job_status'].message_type = SchemaMessages__pb2._JOBSTATUS
-DESCRIPTOR.message_types_by_name['QueryEdgeMessage'] = _QUERYEDGEMESSAGE
-DESCRIPTOR.message_types_by_name['QueryEdgeList'] = _QUERYEDGELIST
-DESCRIPTOR.message_types_by_name['QueryPlan'] = _QUERYPLAN
 DESCRIPTOR.message_types_by_name['ScheduleJobsCypherRequest'] = _SCHEDULEJOBSCYPHERREQUEST
 DESCRIPTOR.message_types_by_name['ScheduleJobsCypherResponse'] = _SCHEDULEJOBSCYPHERRESPONSE
 DESCRIPTOR.message_types_by_name['CancelJobsRequest'] = _CANCELJOBSREQUEST
 DESCRIPTOR.message_types_by_name['CancelJobsResponse'] = _CANCELJOBSRESPONSE
 DESCRIPTOR.message_types_by_name['GetJobsRequest'] = _GETJOBSREQUEST
 DESCRIPTOR.message_types_by_name['GetJobsResponse'] = _GETJOBSRESPONSE
 DESCRIPTOR.message_types_by_name['WaitJobsRequest'] = _WAITJOBSREQUEST
 DESCRIPTOR.message_types_by_name['WaitJobsResponse'] = _WAITJOBSRESPONSE
-DESCRIPTOR.enum_types_by_name['QueryEdgeDirection'] = _QUERYEDGEDIRECTION
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-QueryEdgeMessage = _reflection.GeneratedProtocolMessageType('QueryEdgeMessage', (_message.Message,), {
-  'DESCRIPTOR' : _QUERYEDGEMESSAGE,
-  '__module__' : 'JobService_pb2'
-  # @@protoc_insertion_point(class_scope:xgt.QueryEdgeMessage)
-  })
-_sym_db.RegisterMessage(QueryEdgeMessage)
-
-QueryEdgeList = _reflection.GeneratedProtocolMessageType('QueryEdgeList', (_message.Message,), {
-  'DESCRIPTOR' : _QUERYEDGELIST,
-  '__module__' : 'JobService_pb2'
-  # @@protoc_insertion_point(class_scope:xgt.QueryEdgeList)
-  })
-_sym_db.RegisterMessage(QueryEdgeList)
-
-QueryPlan = _reflection.GeneratedProtocolMessageType('QueryPlan', (_message.Message,), {
-  'DESCRIPTOR' : _QUERYPLAN,
-  '__module__' : 'JobService_pb2'
-  # @@protoc_insertion_point(class_scope:xgt.QueryPlan)
-  })
-_sym_db.RegisterMessage(QueryPlan)
-
 ScheduleJobsCypherRequest = _reflection.GeneratedProtocolMessageType('ScheduleJobsCypherRequest', (_message.Message,), {
 
   'KwargsEntry' : _reflection.GeneratedProtocolMessageType('KwargsEntry', (_message.Message,), {
     'DESCRIPTOR' : _SCHEDULEJOBSCYPHERREQUEST_KWARGSENTRY,
     '__module__' : 'JobService_pb2'
     # @@protoc_insertion_point(class_scope:xgt.ScheduleJobsCypherRequest.KwargsEntry)
     })
@@ -721,16 +512,16 @@
 _JOBSERVICE = _descriptor.ServiceDescriptor(
   name='JobService',
   full_name='xgt.JobService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1281,
-  serialized_end=1564,
+  serialized_start=869,
+  serialized_end=1152,
   methods=[
   _descriptor.MethodDescriptor(
     name='ScheduleJobsCypher',
     full_name='xgt.JobService.ScheduleJobsCypher',
     index=0,
     containing_service=None,
     input_type=_SCHEDULEJOBSCYPHERREQUEST,
```

### Comparing `xgt-1.8.0/src/xgt/JobService_pb2_grpc.py` & `xgt-1.9.0/src/xgt/JobService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/MetricsService_pb2.py` & `xgt-1.9.0/src/xgt/MetricsService_pb2.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/MetricsService_pb2_grpc.py` & `xgt-1.9.0/src/xgt/MetricsService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/src/xgt/SchemaMessages_pb2.py` & `xgt-1.9.0/src/xgt/SchemaMessages_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='SchemaMessages.proto',
   package='xgt',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14SchemaMessages.proto\x12\x03xgt\x1a\x13\x45rrorMessages.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"[\n\x08Property\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\tdata_type\x18\x02 \x01(\x0e\x32\x11.xgt.UvalTypeEnum\x12\x1b\n\x04role\x18\x03 \x01(\x0e\x32\r.xgt.RoleEnum\")\n\x06Schema\x12\x1f\n\x08property\x18\x01 \x03(\x0b\x32\r.xgt.Property\"7\n\nTableFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\"8\n\x0bVertexFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\"\x8c\x01\n\tEdgeFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\x12\x15\n\rsource_vertex\x18\x03 \x01(\t\x12\x15\n\rtarget_vertex\x18\x04 \x01(\t\x12\x12\n\nsource_key\x18\x05 \x01(\t\x12\x12\n\ntarget_key\x18\x06 \x01(\t\"\x8b\x01\n\x08\x41nyFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\x12\x15\n\rsource_vertex\x18\x03 \x01(\t\x12\x15\n\rtarget_vertex\x18\x04 \x01(\t\x12\x12\n\nsource_key\x18\x05 \x01(\t\x12\x12\n\ntarget_key\x18\x06 \x01(\t\"\x97\x03\n\tJobStatus\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\x0e\n\x06job_id\x18\x02 \x01(\x04\x12\"\n\x06status\x18\x03 \x01(\x0e\x32\x12.xgt.JobStatusEnum\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04user\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x37\n\rvisited_edges\x18\x08 \x03(\x0b\x32 .xgt.JobStatus.VisitedEdgesEntry\x12\x0e\n\x06timing\x18\t \x03(\t\x12\x1b\n\x06schema\x18\n \x01(\x0b\x32\x0b.xgt.Schema\x12\x12\n\ntotal_rows\x18\x0b \x01(\x04\x12\x0b\n\x03row\x18\x0c \x03(\t\x1a\x33\n\x11VisitedEdgesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01*\xac\x01\n\x0cUvalTypeEnum\x12\x15\n\x11UNKNOWN_UVAL_TYPE\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\x07\n\x03INT\x10\x03\x12\t\n\x05\x46LOAT\x10\x04\x12\x08\n\x04\x44\x41TE\x10\x05\x12\x08\n\x04TIME\x10\x06\x12\x0c\n\x08\x44\x41TETIME\x10\x07\x12\r\n\tIPADDRESS\x10\x08\x12\x08\n\x04TEXT\x10\t\x12\x10\n\x0c\x43ONTAINER_ID\x10\n\x12\n\n\x06JOB_ID\x10\x0b*q\n\x08RoleEnum\x12\x0c\n\x08PROPERTY\x10\x00\x12\x0e\n\nVERTEX_KEY\x10\x01\x12\x13\n\x0f\x45\x44GE_SOURCE_KEY\x10\x02\x12\x13\n\x0f\x45\x44GE_TARGET_KEY\x10\x03\x12\x1d\n\x19\x41SSOCIATIVE_CONTAINER_KEY\x10\x04*F\n\rFrameTypeEnum\x12\t\n\x05TABLE\x10\x00\x12\n\n\x06VERTEX\x10\x01\x12\x08\n\x04\x45\x44GE\x10\x02\x12\x14\n\x10UVAL_ASSOCIATIVE\x10\x03*z\n\rJobStatusEnum\x12\x16\n\x12UNKNOWN_JOB_STATUS\x10\x00\x12\r\n\tSCHEDULED\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\r\n\tCOMPLETED\x10\x03\x12\x0c\n\x08\x43\x41NCELED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0c\n\x08ROLLBACK\x10\x06\x62\x06proto3'
+  serialized_pb=b'\n\x14SchemaMessages.proto\x12\x03xgt\x1a\x13\x45rrorMessages.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x95\x01\n\x08Property\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\tdata_type\x18\x02 \x01(\x0e\x32\x11.xgt.UvalTypeEnum\x12\x1b\n\x04role\x18\x03 \x01(\x0e\x32\r.xgt.RoleEnum\x12$\n\tleaf_type\x18\x04 \x01(\x0e\x32\x11.xgt.UvalTypeEnum\x12\x12\n\nlist_depth\x18\x05 \x01(\x04\")\n\x06Schema\x12\x1f\n\x08property\x18\x01 \x03(\x0b\x32\r.xgt.Property\"7\n\nTableFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\"8\n\x0bVertexFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\"\x8c\x01\n\tEdgeFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\x12\x15\n\rsource_vertex\x18\x03 \x01(\t\x12\x15\n\rtarget_vertex\x18\x04 \x01(\t\x12\x12\n\nsource_key\x18\x05 \x01(\t\x12\x12\n\ntarget_key\x18\x06 \x01(\t\"\x8b\x01\n\x08\x41nyFrame\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x06schema\x18\x02 \x01(\x0b\x32\x0b.xgt.Schema\x12\x15\n\rsource_vertex\x18\x03 \x01(\t\x12\x15\n\rtarget_vertex\x18\x04 \x01(\t\x12\x12\n\nsource_key\x18\x05 \x01(\t\x12\x12\n\ntarget_key\x18\x06 \x01(\t\"\xc3\x01\n\x10QueryEdgeMessage\x12/\n\x0e\x65\x64ge_direction\x18\x01 \x01(\x0e\x32\x17.xgt.QueryEdgeDirection\x12\x12\n\nedge_label\x18\x02 \x01(\t\x12\x12\n\nedge_frame\x18\x03 \x01(\t\x12\x14\n\x0csource_label\x18\x04 \x01(\t\x12\x14\n\x0csource_frame\x18\x05 \x01(\t\x12\x14\n\x0ctarget_label\x18\x06 \x01(\t\x12\x14\n\x0ctarget_frame\x18\x07 \x01(\t\"5\n\rQueryEdgeList\x12$\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x15.xgt.QueryEdgeMessage\":\n\tQueryPlan\x12-\n\x11plan_as_edge_list\x18\x01 \x03(\x0b\x32\x12.xgt.QueryEdgeList\"\xbb\x03\n\tJobStatus\x12\x19\n\x05\x65rror\x18\x01 \x03(\x0b\x32\n.xgt.Error\x12\x0e\n\x06job_id\x18\x02 \x01(\x04\x12\"\n\x06status\x18\x03 \x01(\x0e\x32\x12.xgt.JobStatusEnum\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04user\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x37\n\rvisited_edges\x18\x08 \x03(\x0b\x32 .xgt.JobStatus.VisitedEdgesEntry\x12\x0e\n\x06timing\x18\t \x03(\t\x12\x1b\n\x06schema\x18\n \x01(\x0b\x32\x0b.xgt.Schema\x12\x12\n\ntotal_rows\x18\x0b \x01(\x04\x12\x0b\n\x03row\x18\x0c \x03(\t\x12\"\n\nquery_plan\x18\r \x01(\x0b\x32\x0e.xgt.QueryPlan\x1a\x33\n\x11VisitedEdgesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01*\xb6\x01\n\x0cUvalTypeEnum\x12\x15\n\x11UNKNOWN_UVAL_TYPE\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\x07\n\x03INT\x10\x03\x12\t\n\x05\x46LOAT\x10\x04\x12\x08\n\x04\x44\x41TE\x10\x05\x12\x08\n\x04TIME\x10\x06\x12\x0c\n\x08\x44\x41TETIME\x10\x07\x12\r\n\tIPADDRESS\x10\x08\x12\x08\n\x04TEXT\x10\t\x12\x10\n\x0c\x43ONTAINER_ID\x10\n\x12\n\n\x06JOB_ID\x10\x0b\x12\x08\n\x04LIST\x10\x0c*q\n\x08RoleEnum\x12\x0c\n\x08PROPERTY\x10\x00\x12\x0e\n\nVERTEX_KEY\x10\x01\x12\x13\n\x0f\x45\x44GE_SOURCE_KEY\x10\x02\x12\x13\n\x0f\x45\x44GE_TARGET_KEY\x10\x03\x12\x1d\n\x19\x41SSOCIATIVE_CONTAINER_KEY\x10\x04*F\n\rFrameTypeEnum\x12\t\n\x05TABLE\x10\x00\x12\n\n\x06VERTEX\x10\x01\x12\x08\n\x04\x45\x44GE\x10\x02\x12\x14\n\x10UVAL_ASSOCIATIVE\x10\x03*z\n\rJobStatusEnum\x12\x16\n\x12UNKNOWN_JOB_STATUS\x10\x00\x12\r\n\tSCHEDULED\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\r\n\tCOMPLETED\x10\x03\x12\x0c\n\x08\x43\x41NCELED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0c\n\x08ROLLBACK\x10\x06*=\n\x12QueryEdgeDirection\x12\x0b\n\x07\x46ORWARD\x10\x00\x12\x0c\n\x08\x42\x41\x43KWARD\x10\x01\x12\x0c\n\x08NOT_EDGE\x10\x02\x62\x06proto3'
   ,
   dependencies=[ErrorMessages__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 _UVALTYPEENUM = _descriptor.EnumDescriptor(
   name='UvalTypeEnum',
   full_name='xgt.UvalTypeEnum',
   filename=None,
@@ -89,19 +89,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='JOB_ID', index=11, number=11,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='LIST', index=12, number=12,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1030,
-  serialized_end=1202,
+  serialized_start=1438,
+  serialized_end=1620,
 )
 _sym_db.RegisterEnumDescriptor(_UVALTYPEENUM)
 
 UvalTypeEnum = enum_type_wrapper.EnumTypeWrapper(_UVALTYPEENUM)
 _ROLEENUM = _descriptor.EnumDescriptor(
   name='RoleEnum',
   full_name='xgt.RoleEnum',
@@ -133,16 +138,16 @@
       name='ASSOCIATIVE_CONTAINER_KEY', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1204,
-  serialized_end=1317,
+  serialized_start=1622,
+  serialized_end=1735,
 )
 _sym_db.RegisterEnumDescriptor(_ROLEENUM)
 
 RoleEnum = enum_type_wrapper.EnumTypeWrapper(_ROLEENUM)
 _FRAMETYPEENUM = _descriptor.EnumDescriptor(
   name='FrameTypeEnum',
   full_name='xgt.FrameTypeEnum',
@@ -169,16 +174,16 @@
       name='UVAL_ASSOCIATIVE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1319,
-  serialized_end=1389,
+  serialized_start=1737,
+  serialized_end=1807,
 )
 _sym_db.RegisterEnumDescriptor(_FRAMETYPEENUM)
 
 FrameTypeEnum = enum_type_wrapper.EnumTypeWrapper(_FRAMETYPEENUM)
 _JOBSTATUSENUM = _descriptor.EnumDescriptor(
   name='JobStatusEnum',
   full_name='xgt.JobStatusEnum',
@@ -220,32 +225,64 @@
       name='ROLLBACK', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1391,
-  serialized_end=1513,
+  serialized_start=1809,
+  serialized_end=1931,
 )
 _sym_db.RegisterEnumDescriptor(_JOBSTATUSENUM)
 
 JobStatusEnum = enum_type_wrapper.EnumTypeWrapper(_JOBSTATUSENUM)
+_QUERYEDGEDIRECTION = _descriptor.EnumDescriptor(
+  name='QueryEdgeDirection',
+  full_name='xgt.QueryEdgeDirection',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='FORWARD', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='BACKWARD', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='NOT_EDGE', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=1933,
+  serialized_end=1994,
+)
+_sym_db.RegisterEnumDescriptor(_QUERYEDGEDIRECTION)
+
+QueryEdgeDirection = enum_type_wrapper.EnumTypeWrapper(_QUERYEDGEDIRECTION)
 UNKNOWN_UVAL_TYPE = 0
 UNKNOWN = 1
 BOOLEAN = 2
 INT = 3
 FLOAT = 4
 DATE = 5
 TIME = 6
 DATETIME = 7
 IPADDRESS = 8
 TEXT = 9
 CONTAINER_ID = 10
 JOB_ID = 11
+LIST = 12
 PROPERTY = 0
 VERTEX_KEY = 1
 EDGE_SOURCE_KEY = 2
 EDGE_TARGET_KEY = 3
 ASSOCIATIVE_CONTAINER_KEY = 4
 TABLE = 0
 VERTEX = 1
@@ -254,14 +291,17 @@
 UNKNOWN_JOB_STATUS = 0
 SCHEDULED = 1
 RUNNING = 2
 COMPLETED = 3
 CANCELED = 4
 FAILED = 5
 ROLLBACK = 6
+FORWARD = 0
+BACKWARD = 1
+NOT_EDGE = 2
 
 
 
 _PROPERTY = _descriptor.Descriptor(
   name='Property',
   full_name='xgt.Property',
   filename=None,
@@ -286,28 +326,42 @@
     _descriptor.FieldDescriptor(
       name='role', full_name='xgt.Property.role', index=2,
       number=3, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='leaf_type', full_name='xgt.Property.leaf_type', index=3,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='list_depth', full_name='xgt.Property.list_depth', index=4,
+      number=5, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=83,
-  serialized_end=174,
+  serialized_start=84,
+  serialized_end=233,
 )
 
 
 _SCHEMA = _descriptor.Descriptor(
   name='Schema',
   full_name='xgt.Schema',
   filename=None,
@@ -330,16 +384,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=176,
-  serialized_end=217,
+  serialized_start=235,
+  serialized_end=276,
 )
 
 
 _TABLEFRAME = _descriptor.Descriptor(
   name='TableFrame',
   full_name='xgt.TableFrame',
   filename=None,
@@ -369,16 +423,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=219,
-  serialized_end=274,
+  serialized_start=278,
+  serialized_end=333,
 )
 
 
 _VERTEXFRAME = _descriptor.Descriptor(
   name='VertexFrame',
   full_name='xgt.VertexFrame',
   filename=None,
@@ -408,16 +462,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=276,
-  serialized_end=332,
+  serialized_start=335,
+  serialized_end=391,
 )
 
 
 _EDGEFRAME = _descriptor.Descriptor(
   name='EdgeFrame',
   full_name='xgt.EdgeFrame',
   filename=None,
@@ -475,16 +529,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=335,
-  serialized_end=475,
+  serialized_start=394,
+  serialized_end=534,
 )
 
 
 _ANYFRAME = _descriptor.Descriptor(
   name='AnyFrame',
   full_name='xgt.AnyFrame',
   filename=None,
@@ -542,16 +596,154 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=478,
-  serialized_end=617,
+  serialized_start=537,
+  serialized_end=676,
+)
+
+
+_QUERYEDGEMESSAGE = _descriptor.Descriptor(
+  name='QueryEdgeMessage',
+  full_name='xgt.QueryEdgeMessage',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='edge_direction', full_name='xgt.QueryEdgeMessage.edge_direction', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='edge_label', full_name='xgt.QueryEdgeMessage.edge_label', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='edge_frame', full_name='xgt.QueryEdgeMessage.edge_frame', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='source_label', full_name='xgt.QueryEdgeMessage.source_label', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='source_frame', full_name='xgt.QueryEdgeMessage.source_frame', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='target_label', full_name='xgt.QueryEdgeMessage.target_label', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='target_frame', full_name='xgt.QueryEdgeMessage.target_frame', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=679,
+  serialized_end=874,
+)
+
+
+_QUERYEDGELIST = _descriptor.Descriptor(
+  name='QueryEdgeList',
+  full_name='xgt.QueryEdgeList',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='edges', full_name='xgt.QueryEdgeList.edges', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=876,
+  serialized_end=929,
+)
+
+
+_QUERYPLAN = _descriptor.Descriptor(
+  name='QueryPlan',
+  full_name='xgt.QueryPlan',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='plan_as_edge_list', full_name='xgt.QueryPlan.plan_as_edge_list', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=931,
+  serialized_end=989,
 )
 
 
 _JOBSTATUS_VISITEDEDGESENTRY = _descriptor.Descriptor(
   name='VisitedEdgesEntry',
   full_name='xgt.JobStatus.VisitedEdgesEntry',
   filename=None,
@@ -581,16 +773,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=976,
-  serialized_end=1027,
+  serialized_start=1384,
+  serialized_end=1435,
 )
 
 _JOBSTATUS = _descriptor.Descriptor(
   name='JobStatus',
   full_name='xgt.JobStatus',
   filename=None,
   file=DESCRIPTOR,
@@ -677,55 +869,71 @@
     _descriptor.FieldDescriptor(
       name='row', full_name='xgt.JobStatus.row', index=11,
       number=12, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='query_plan', full_name='xgt.JobStatus.query_plan', index=12,
+      number=13, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_JOBSTATUS_VISITEDEDGESENTRY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=620,
-  serialized_end=1027,
+  serialized_start=992,
+  serialized_end=1435,
 )
 
 _PROPERTY.fields_by_name['data_type'].enum_type = _UVALTYPEENUM
 _PROPERTY.fields_by_name['role'].enum_type = _ROLEENUM
+_PROPERTY.fields_by_name['leaf_type'].enum_type = _UVALTYPEENUM
 _SCHEMA.fields_by_name['property'].message_type = _PROPERTY
 _TABLEFRAME.fields_by_name['schema'].message_type = _SCHEMA
 _VERTEXFRAME.fields_by_name['schema'].message_type = _SCHEMA
 _EDGEFRAME.fields_by_name['schema'].message_type = _SCHEMA
 _ANYFRAME.fields_by_name['schema'].message_type = _SCHEMA
+_QUERYEDGEMESSAGE.fields_by_name['edge_direction'].enum_type = _QUERYEDGEDIRECTION
+_QUERYEDGELIST.fields_by_name['edges'].message_type = _QUERYEDGEMESSAGE
+_QUERYPLAN.fields_by_name['plan_as_edge_list'].message_type = _QUERYEDGELIST
 _JOBSTATUS_VISITEDEDGESENTRY.containing_type = _JOBSTATUS
 _JOBSTATUS.fields_by_name['error'].message_type = ErrorMessages__pb2._ERROR
 _JOBSTATUS.fields_by_name['status'].enum_type = _JOBSTATUSENUM
 _JOBSTATUS.fields_by_name['start_time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _JOBSTATUS.fields_by_name['end_time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _JOBSTATUS.fields_by_name['visited_edges'].message_type = _JOBSTATUS_VISITEDEDGESENTRY
 _JOBSTATUS.fields_by_name['schema'].message_type = _SCHEMA
+_JOBSTATUS.fields_by_name['query_plan'].message_type = _QUERYPLAN
 DESCRIPTOR.message_types_by_name['Property'] = _PROPERTY
 DESCRIPTOR.message_types_by_name['Schema'] = _SCHEMA
 DESCRIPTOR.message_types_by_name['TableFrame'] = _TABLEFRAME
 DESCRIPTOR.message_types_by_name['VertexFrame'] = _VERTEXFRAME
 DESCRIPTOR.message_types_by_name['EdgeFrame'] = _EDGEFRAME
 DESCRIPTOR.message_types_by_name['AnyFrame'] = _ANYFRAME
+DESCRIPTOR.message_types_by_name['QueryEdgeMessage'] = _QUERYEDGEMESSAGE
+DESCRIPTOR.message_types_by_name['QueryEdgeList'] = _QUERYEDGELIST
+DESCRIPTOR.message_types_by_name['QueryPlan'] = _QUERYPLAN
 DESCRIPTOR.message_types_by_name['JobStatus'] = _JOBSTATUS
 DESCRIPTOR.enum_types_by_name['UvalTypeEnum'] = _UVALTYPEENUM
 DESCRIPTOR.enum_types_by_name['RoleEnum'] = _ROLEENUM
 DESCRIPTOR.enum_types_by_name['FrameTypeEnum'] = _FRAMETYPEENUM
 DESCRIPTOR.enum_types_by_name['JobStatusEnum'] = _JOBSTATUSENUM
+DESCRIPTOR.enum_types_by_name['QueryEdgeDirection'] = _QUERYEDGEDIRECTION
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Property = _reflection.GeneratedProtocolMessageType('Property', (_message.Message,), {
   'DESCRIPTOR' : _PROPERTY,
   '__module__' : 'SchemaMessages_pb2'
   # @@protoc_insertion_point(class_scope:xgt.Property)
   })
@@ -762,14 +970,35 @@
 AnyFrame = _reflection.GeneratedProtocolMessageType('AnyFrame', (_message.Message,), {
   'DESCRIPTOR' : _ANYFRAME,
   '__module__' : 'SchemaMessages_pb2'
   # @@protoc_insertion_point(class_scope:xgt.AnyFrame)
   })
 _sym_db.RegisterMessage(AnyFrame)
 
+QueryEdgeMessage = _reflection.GeneratedProtocolMessageType('QueryEdgeMessage', (_message.Message,), {
+  'DESCRIPTOR' : _QUERYEDGEMESSAGE,
+  '__module__' : 'SchemaMessages_pb2'
+  # @@protoc_insertion_point(class_scope:xgt.QueryEdgeMessage)
+  })
+_sym_db.RegisterMessage(QueryEdgeMessage)
+
+QueryEdgeList = _reflection.GeneratedProtocolMessageType('QueryEdgeList', (_message.Message,), {
+  'DESCRIPTOR' : _QUERYEDGELIST,
+  '__module__' : 'SchemaMessages_pb2'
+  # @@protoc_insertion_point(class_scope:xgt.QueryEdgeList)
+  })
+_sym_db.RegisterMessage(QueryEdgeList)
+
+QueryPlan = _reflection.GeneratedProtocolMessageType('QueryPlan', (_message.Message,), {
+  'DESCRIPTOR' : _QUERYPLAN,
+  '__module__' : 'SchemaMessages_pb2'
+  # @@protoc_insertion_point(class_scope:xgt.QueryPlan)
+  })
+_sym_db.RegisterMessage(QueryPlan)
+
 JobStatus = _reflection.GeneratedProtocolMessageType('JobStatus', (_message.Message,), {
 
   'VisitedEdgesEntry' : _reflection.GeneratedProtocolMessageType('VisitedEdgesEntry', (_message.Message,), {
     'DESCRIPTOR' : _JOBSTATUS_VISITEDEDGESENTRY,
     '__module__' : 'SchemaMessages_pb2'
     # @@protoc_insertion_point(class_scope:xgt.JobStatus.VisitedEdgesEntry)
     })
```

### Comparing `xgt-1.8.0/src/xgt/__init__.py` & `xgt-1.9.0/src/xgt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 # environment variable needs to be set. The grpc version must be 1.15 or later.
 # See here: https://groups.google.com/forum/#!topic/grpc-io/1ABEo5e-HsU.
 import os
 os.environ["GRPC_ENABLE_FORK_SUPPORT"] = "1"
 
 
 from .common import (
-  BOOLEAN, INT, FLOAT, DATE, TIME, DATETIME, IPADDRESS, TEXT,
+  BOOLEAN, INT, FLOAT, DATE, TIME, DATETIME, IPADDRESS, TEXT, LIST,
   XgtError, XgtNotImplemented, XgtInternalError,
   XgtIOError, XgtServerMemoryError, XgtConnectionError,
   XgtSyntaxError, XgtTypeError, XgtValueError, XgtNameError,
   XgtArithmeticError, XgtFrameDependencyError, XgtTransactionError,
   XgtSecurityError
 )
 from .connection import Connection
```

### Comparing `xgt-1.8.0/src/xgt/common.py` & `xgt-1.9.0/src/xgt/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 INT = 'int'
 FLOAT = 'float'
 DATE = 'date'
 TIME = 'time'
 DATETIME = 'datetime'
 IPADDRESS = 'ipaddress'
 TEXT = 'text'
+LIST = 'list'
 
 # Send in 2MB chunks (grpc recommends 16-64 KB, but this got the best performance locally)
 # FYI: by default grpc only supports up to 4MB.
 MAX_PACKET_SIZE = 2097152
 
 class XgtError(Exception):
   """
@@ -119,56 +120,72 @@
   processing, we canonicalize these into a list of string-type pairs,
   performing validation along the way.
   '''
   # Validate the shape first
   try:
     if len(obj) < 1:
       raise XgtTypeError('A schema must not be empty.')
-    for pairlike in obj:
-      assert len(pairlike) == 2
+    for col in obj:
+      assert len(col) >= 2
+      if (_validated_property_type(col[1]) == "LIST"):
+        assert (len(col) <= 4 and len(col) >= 3)
+      else:
+        assert len(col) == 2
   except:
     raise XgtTypeError('A schema must be a non-empty list of (property, type) pairs.')
   # Looks good. Return a canonical schema.
-  return [(_validated_property_name(name), _validated_property_type(xgt_type))
-          for name,xgt_type in obj]
+  schema_returned = []
+  for col in obj:
+    val_type = _validated_property_type(col[1])
+    if val_type != "LIST":
+      schema_returned.append((_validated_property_name(col[0]), val_type))
+    else:
+      leaf_type = _validated_property_type(col[2])
+      if (len(col) != 4):
+        schema_returned.append((_validated_property_name(col[0]),
+                               val_type, leaf_type))
+      else:
+        schema_returned.append((_validated_property_name(col[0]),
+                                val_type, leaf_type, col[3]))
+  return schema_returned
 
 def _validated_frame_name(obj):
   '''Takes a user-supplied object and returns a unicode frame name string.'''
-  _assert_isstring(obj) 
+  _assert_isstring(obj)
   name = str(obj)
   if len(name) < 1:
     raise XgtNameError('Frame names cannot be empty.')
   if '.' in name:
     raise XgtNameError('Frame names cannot contain periods: '+name)
   return name
 
 def _validated_namespace_name(obj):
   '''Takes a user-supplied object and returns a unicode frame name string.'''
-  _assert_isstring(obj) 
+  _assert_isstring(obj)
   name = str(obj)
   if len(name) < 1:
     raise XgtNameError('Namespace names cannot be empty.')
   if '.' in name:
     raise XgtNameError('Namespace names cannot contain periods: '+name)
   return name
 
 def _validated_property_name(obj):
   '''Takes a user-supplied object and returns a unicode proprty name string.'''
-  _assert_isstring(obj) 
+  _assert_isstring(obj)
   return str(obj)
 
 def _get_valid_property_types_to_create():
-  return [BOOLEAN, INT, FLOAT, DATE, TIME, DATETIME, IPADDRESS, TEXT]
+  return [BOOLEAN, INT, FLOAT, DATE, TIME, DATETIME, IPADDRESS, TEXT, LIST]
 
 def _get_valid_property_types_for_return_only():
   return ['container_id', 'job_id']
 
 def _validated_property_type(obj):
   '''Takes a user-supplied object and returns an xGT schema type.'''
-  _assert_isstring(obj) 
+  _assert_isstring(obj)
   prop_type = str(obj)
   valid_prop_types = _get_valid_property_types_to_create()
   if prop_type.lower() not in valid_prop_types:
     if prop_type.lower in _get_valid_property_types_for_return_only():
       raise XgtTypeError('Invalid property type "'+prop_type+'". This type '
                          'cannot be used when creating a frame.')
     else:
```

### Comparing `xgt-1.8.0/src/xgt/connection.py` & `xgt-1.9.0/src/xgt/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,15 +107,15 @@
   Parameters
   ----------
   host : str
     IP address of the computer where the server is running.
   port : int
     Port where the server is listening on for RPC calls.
   userid : str
-    The user name to authenticate as.
+    The username to authenticate as.
   credentials : str
     Credentials used to authenticate.
   flags: dict
     Dictionary containing flags. Possible flags are:
 
     aws_access_key_id : str
       Amazon Access Key ID, used for authentication when loading data
@@ -126,15 +126,15 @@
     ssl : boolean
       If true use ssl authentication for secure server channels.
       The default is False.
     ssl_root_dir : str
       Path to the root folder for ssl certificates and private keys.
       Defaults to the user's home directory.
     ssl_server_cn : str
-      Common name on the certificate of the server to connect to.
+      The Common Name (CN) on the certificate of the server to connect to.
       The default is the hostname.
   """
 
   _GIB = 1024 * 1024 * 1024
 
   def __init__(self, host='127.0.0.1', port=4367, flags=None, userid='',
                credentials=''):
@@ -284,18 +284,15 @@
     request = job_proto.ScheduleJobsCypherRequest()
     request.cypher_query.extend([query])
     if 'parameters' in kwargs and kwargs['parameters'] != None:
       self._process_parameters(request, kwargs['parameters'])
     self._process_kwargs(request, kwargs)
     response = self._call(request, self._job_svc.ScheduleJobsCypher)
     one_job = response.job_status[0]
-    if response.HasField('query_plan'):
-      return Job(self, one_job, response.query_plan)
-    else:
-      return Job(self, one_job)
+    return Job(self, one_job)
 
   #------------------------- Housekeeping Methods
   @property
   def server_version(self):
     """
     Obtains the current product version from the server.
 
@@ -402,15 +399,24 @@
     response = self._call(request, self._graph_svc.GetTableFrames)
 
     frames = []
     for data in response.container:
       schema = []
       for prop in data.schema.property:
         prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-        schema.append([prop.name, prop_type])
+        if prop_type == 'list':
+          leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+          if (prop.list_depth == 0):
+            schema.append([prop.name, prop_type, leaf_type])
+          else:
+            schema.append([prop.name, prop_type, leaf_type,
+                           prop.list_depth + 1])
+        else:
+          schema.append([prop.name, prop_type])
       frames.append(TableFrame(self, data.name, schema))
     return frames
 
   def get_table_frame(self, name):
     """
     Get a TableFrame object that allows interaction with a table present in the xGT server.
 
@@ -529,15 +535,25 @@
     frames = []
     for data in response.container:
       schema = []
       vertex_key_val = sch_proto.RoleEnum.Value('VERTEX_KEY')
       key = None
       for prop in data.schema.property:
         prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-        schema.append([prop.name, prop_type])
+        if prop_type == 'list':
+          leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+          if (prop.list_depth == 0):
+            schema.append([prop.name, prop_type, leaf_type])
+          else:
+            schema.append([prop.name, prop_type, leaf_type,
+                           prop.list_depth + 1])
+        else:
+          schema.append([prop.name, prop_type])
+
         if prop.role == vertex_key_val:
           key = prop.name
       frames.append(VertexFrame(self, data.name, schema, key))
     return frames
 
   def get_vertex_frame(self, name):
     """
@@ -653,15 +669,24 @@
       request.namespace_name = _validated_namespace_name(namespace)
     response = self._call(request, self._graph_svc.GetEdgeFrames)
     frames = []
     for data in response.container:
       schema = []
       for prop in data.schema.property:
         prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-        schema.append([prop.name, prop_type])
+        if prop_type == 'list':
+          leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+          if (prop.list_depth == 0):
+            schema.append([prop.name, prop_type, leaf_type])
+          else:
+            schema.append([prop.name, prop_type, leaf_type,
+                           prop.list_depth + 1])
+        else:
+          schema.append([prop.name, prop_type])
       frames.append(EdgeFrame(self, data.name, schema,
                               data.source_vertex, data.target_vertex,
                               data.source_key, data.target_key))
     return frames
 
   def get_edge_frame(self, name):
     """
@@ -775,22 +800,23 @@
     ----------
     name : str
       The name of the namespace to create.
     frame_labels : dictionary
       A dictionary mapping a string to a list of strings. The key represents
       the permission type. The value represents the labels required for this
       permission. Permission types are "create", "read", "update", and "delete".
-      By default no labels are required.
+      By default, no labels are required.
     security_labels : dictionary
       same as frame_labels (DEPRECATED)
     row_label_universe :  array
       **NOT yet supported**.
       An array of all possible labels to be used for rows inside this namespace.
       A maximum of 128 labels are supported for rows in each frame.
-      By default no row labels are required.
+      By default, no row labels are required.
+      (since version 1.5.0)
     attempts : int
       Number of times to attempt the creation of the namespace.
       It will be retried if it fails due to transactional conflicts.
       (since version 1.4.1)
 
     Raises
     -------
@@ -839,21 +865,21 @@
       it will use the default namespace.
     schema : list of pairs
       List of pairs associating property names with xGT data types.
     frame_labels : dictionary
       A dictionary mapping a string to a list of strings. The key represents
       the permission type. The value represents the labels required for this
       permission. Permission types are create, read, update, and delete.
-      By default no labels are required.
+      By default, no labels are required.
     security_labels : dictionary
       same as frame_labels (DEPRECATED)
     row_label_universe :  array
       An array of all possible labels to be used for rows inside this table frame.
       A maximum of 128 labels are supported for rows in each frame.
-      By default no row labels are required.
+      By default, no row labels are required.
       (since version 1.5.0)
     attempts : int
       Number of times to attempt the creation of the TableFrame.
       It will be retried if it fails due to transactional conflicts.
       (since version 1.4.1)
 
     Returns
@@ -886,32 +912,57 @@
     name = _validated_frame_name(name)
     schema = _validated_schema(schema)
 
     request = graph_proto.CreateFrameRequest()
     request.type = sch_proto.FrameTypeEnum.Value('TABLE')
     request.frame_name = name
 
-    for col_name,col_type in schema:
+    for col in schema:
       prop = sch_proto.Property()
-      prop.name = col_name
-      prop.data_type = sch_proto.UvalTypeEnum.Value(col_type)
+      prop.name = col[0]
+      prop.data_type = sch_proto.UvalTypeEnum.Value(col[1])
       prop.role = sch_proto.RoleEnum.Value('PROPERTY')
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        prop.leaf_type = sch_proto.UvalTypeEnum.Value(col[2])
+
+        if (len(col) > 3):
+          if col[3] > 1:
+            prop.list_depth = col[3] - 1
+          elif col[3] == 1:
+            prop.list_depth = 0
+          else:
+            raise XgtTypeError("A list cannot have a depth less than one.")
+        else:
+          prop.list_depth = 0
+
       request.schema.property.extend([prop])
 
     request = self._container_labels_helper(request, frame_labels,
-                                            security_labels, row_label_universe)
+                                            security_labels,
+                                            row_label_universe)
 
     self._process_kwargs(request, {'attempts':attempts})
     response =  self._call(request, self._graph_svc.CreateFrame)
 
     data = response.container[0]
     schema_returned = []
     for prop in data.schema.property:
       prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-      schema_returned.append([prop.name, prop_type])
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+        if (prop.list_depth == 0):
+          schema_returned.append([prop.name, prop_type, leaf_type])
+        else:
+          schema_returned.append([prop.name, prop_type, leaf_type,
+                                  prop.list_depth + 1])
+      else:
+        schema_returned.append([prop.name, prop_type])
 
     frame = TableFrame(self, data.name, schema_returned)
     return frame
 
   def create_vertex_frame(self, name, schema, key, frame_labels = None,
                           security_labels = None,
                           row_label_universe = None, attempts = 1):
@@ -935,21 +986,21 @@
       The property name used to uniquely identify vertices in the graph.
       This is the name of one of the properties from the schema and
       must be unique for each vertex in the frame.
     frame_labels : dictionary
       A dictionary mapping a string to a list of strings. The key represents
       the permission type. The value represents the labels required for this
       permission. Permission types are create, read, update, and delete.
-      By default no labels are required.
+      By default, no labels are required.
     security_labels : dictionary
       same as frame_labels (DEPRECATED)
     row_label_universe :  array
       An array of all possible labels to be used for rows inside this vertex frame.
       A maximum of 128 labels are supported for rows in each frame.
-      By default no row labels are required.
+      By default, no row labels are required.
       (since version 1.5.0)
     attempts : int
       Number of times to attempt the creation of the VertexFrame.
       It will be retried if it fails due to transactional conflicts.
       (since version 1.4.1)
 
     Returns
@@ -982,32 +1033,50 @@
 
     """
     name = _validated_frame_name(name)
     schema = _validated_schema(schema)
     key = _validated_property_name(key)
 
     key_found = False
-    if key not in [prop for prop,_ in schema]:
+    for col in schema:
+      if key == col[0]:
+        key_found = True
+
+    if not key_found:
       msg = 'The vertex key "{0}" does not match any schema property ' \
             'name in this frame.'
       raise XgtNameError(msg.format(key))
 
     request = graph_proto.CreateFrameRequest()
     request.type = sch_proto.FrameTypeEnum.Value('VERTEX')
     request.frame_name = name
 
-    for col_name,col_type in schema:
+    for col in schema:
       prop = sch_proto.Property()
-      prop.name = col_name
-      prop.data_type = sch_proto.UvalTypeEnum.Value(col_type)
+      prop.name = col[0]
+      prop.data_type = sch_proto.UvalTypeEnum.Value(col[1])
 
-      if col_name == key:
+      if prop.name == key:
         prop.role = sch_proto.RoleEnum.Value('VERTEX_KEY')
       else:
         prop.role = sch_proto.RoleEnum.Value('PROPERTY')
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        prop.leaf_type = sch_proto.UvalTypeEnum.Value(col[2])
+
+        if (len(col) > 3):
+          if col[3] > 1:
+            prop.list_depth = col[3] - 1
+          elif col[3] == 1:
+            prop.list_depth = 0
+          else:
+            raise XgtTypeError("A list cannot have a depth less than one.")
+        else:
+          prop.list_depth = 0
+
       request.schema.property.extend([prop])
 
     request = self._container_labels_helper(request, frame_labels,
                                             security_labels, row_label_universe)
 
     self._process_kwargs(request, {'attempts':attempts})
     response =  self._call(request, self._graph_svc.CreateFrame)
@@ -1015,15 +1084,26 @@
     data = response.container[0]
     schema_returned = []
     vertex_key_val = sch_proto.RoleEnum.Value('VERTEX_KEY')
     key_returned = None
 
     for prop in data.schema.property:
       prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-      schema_returned.append([prop.name, prop_type])
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+        if (prop.list_depth == 0):
+          schema_returned.append([prop.name, prop_type, leaf_type])
+        else:
+          schema_returned.append([prop.name, prop_type, leaf_type,
+                                  prop.list_depth + 1])
+      else:
+        schema_returned.append([prop.name, prop_type])
+
       if prop.role == vertex_key_val:
         key_returned = prop.name
 
     frame = VertexFrame(self, data.name, schema_returned, key_returned)
     return frame
 
 
@@ -1069,21 +1149,21 @@
     target_key : str
       The edge property name that identifies the target vertex of an edge.
       This is one of the properties from the schema.
     frame_labels : dictionary
       A dictionary mapping a string to a list of strings. The key represents
       the permission type. The value represents the labels required for this
       permission. Permission types are create, read, update, and delete.
-      By default no labels are required.
+      By default, no labels are required.
     security_labels : dictionary
       same as frame_labels (DEPRECATED)
     row_label_universe :  array
       An array of all possible labels to be used for rows inside this edge frame.
       A maximum of 128 labels are supported for rows in each frame.
-      By default no row labels are required.
+      By default, no row labels are required.
       (since version 1.5.0)
     attempts : int
       Number of times to attempt the creation of the EdgeFrame.
       It will be retried if it fails due to transactional conflicts.
       (since version 1.4.1)
 
     Returns
@@ -1135,19 +1215,28 @@
 
     """
     name = _validated_frame_name(name)
     schema = _validated_schema(schema)
     source_key = _validated_property_name(source_key)
     target_key = _validated_property_name(target_key)
 
-    if source_key not in [prop for prop, _ in schema]:
+    found_source = False
+    found_target = False
+
+    for col in schema:
+      if source_key == col[0]:
+        found_source = True
+      if target_key == col[0]:
+        found_target = True
+
+    if not found_source:
       msg = 'The source key "{0}" does not match any schema property ' \
             'name in this frame.'
       raise XgtNameError(msg.format(source_key))
-    if target_key not in [prop for prop, _ in schema]:
+    if not found_target:
       msg = 'The target key "{0}" does not match any schema property ' \
             'name in this frame.'
       raise XgtNameError(msg.format(target_key))
 
     if isinstance(source, VertexFrame):
       source_name = source.name
     else:
@@ -1161,38 +1250,62 @@
     request.type = sch_proto.FrameTypeEnum.Value('EDGE')
     request.frame_name = name
     request.source_key = source_key
     request.target_key = target_key
     request.source_vertex = source_name
     request.target_vertex = target_name
 
-    for col_name, col_type in schema:
+    for col in schema:
       prop = sch_proto.Property()
-      prop.name = col_name
-      prop.data_type = sch_proto.UvalTypeEnum.Value(col_type)
+      prop.name = col[0]
+      prop.data_type = sch_proto.UvalTypeEnum.Value(col[1])
 
-      if col_name == source_key:
+      if prop.name == source_key:
         prop.role = sch_proto.RoleEnum.Value('EDGE_SOURCE_KEY')
-      elif col_name == target_key:
+      elif prop.name == target_key:
         prop.role = sch_proto.RoleEnum.Value('EDGE_TARGET_KEY')
       else:
         prop.role = sch_proto.RoleEnum.Value('PROPERTY')
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        prop.leaf_type = sch_proto.UvalTypeEnum.Value(col[2])
+
+        if (len(col) > 3):
+          if col[3] > 1:
+            prop.list_depth = col[3] - 1
+          elif col[3] == 1:
+            prop.list_depth = 0
+          else:
+            raise XgtTypeError("A list cannot have a depth less than one.")
+        else:
+          prop.list_depth = 0
+
       request.schema.property.extend([prop])
 
     request = self._container_labels_helper(request, frame_labels,
                                             security_labels, row_label_universe)
 
     self._process_kwargs(request, {'attempts':attempts})
     response =  self._call(request, self._graph_svc.CreateFrame)
 
     data = response.container[0]
     schema_returned = []
     for prop in data.schema.property:
       prop_type = sch_proto.UvalTypeEnum.Name(prop.data_type).lower()
-      schema_returned.append([prop.name, prop_type])
+
+      if (prop.data_type == sch_proto.UvalTypeEnum.Value('LIST')):
+        leaf_type = sch_proto.UvalTypeEnum.Name(prop.leaf_type).lower()
+
+        if (prop.list_depth == 0):
+          schema_returned.append([prop.name, prop_type, leaf_type])
+        else:
+          schema_returned.append([prop.name, prop_type, leaf_type,
+                                  prop.list_depth + 1])
+      else:
+        schema_returned.append([prop.name, prop_type])
 
     frame = EdgeFrame(self, data.name, schema_returned, data.source_vertex,
                       data.target_vertex, data.source_key, data.target_key)
     return frame
 
   def drop_namespace(self, namespace, force_drop = False, attempts = 10):
     """
@@ -1266,15 +1379,15 @@
     -------
     bool
       True if frame was found and dropped and False if frame was not found.
 
     Raises
     -------
     XgtFrameDependencyError
-      If another frame depends on this frame. The depending frame should be
+      If another frame depends on this frame. The dependent frame should be
       dropped first.
     XgtNameError
       If the name provided is not a correct frame name.
     XgtSecurityError
       If the user does not have required permissions for this action.
     XgtTransactionError
       If a conflict with another transaction occurs.
@@ -1355,16 +1468,16 @@
     Get a list of Job objects, each representing the state of
     the job on the server at the point in time of the
     invocation of this function.
 
     Parameters
     ----------
     jobids : list of ints
-      A list of job ids for which to return Job objects.
-      By default all jobs are returned.
+      A list of job IDs for which to return Job objects.
+      By default, all jobs are returned.
 
     Returns
     -------
     list
       A list of Job objects, each representing the state
       of a job in the server.
 
@@ -1835,15 +1948,15 @@
       If the provided string is not valid.
     XgtSecurityError
       If the user does not have required permissions for this action.
 
     Examples
     --------
     >>> conn = xgt.Connection()
-    >>> conn.set_default("mynamespace")
+    >>> conn.set_default_namespace("mynamespace")
     """
 
     if (default_namespace is None):
       default_namespace = ''
 
     request = admin_proto.SetDefaultNamespaceRequest()
     request.default_namespace = default_namespace
```

### Comparing `xgt-1.8.0/src/xgt/graph.py` & `xgt-1.9.0/src/xgt/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,19 +131,19 @@
     """
     self._conn = conn
     self._name = name
     # Check the schema against the valid property types.
     valid_prop_types = _get_valid_property_types_to_create() + \
                        _get_valid_property_types_for_return_only()
 
-    for _, prop_type in schema:
-      if prop_type not in valid_prop_types:
-        raise XgtTypeError('Invalid property type "' + prop_type + '"')
+    for col in schema:
+      if col[1] not in valid_prop_types:
+        raise XgtTypeError('Invalid property type "' + col[1] + '"')
 
-    self._schema = [[c[0], c[1]] for c in schema]
+    self._schema = schema
 
   @property
   def name(self):
     """str: Name of the frame."""
     return self._name
 
   @property
@@ -155,35 +155,38 @@
   def connection(self):
     """Connection object: The connection used when constructing the frame."""
     return self._conn
 
   def load(self, paths, headerMode = HeaderMode.NONE, record_history = True,
            row_labels = None, row_label_columns = None, delimiter = ','):
     """
-    Loads data from one or more CSV files specified in the list of paths.
+    Loads data from one or more files specified in the list of paths.
+    These files may be CSV, Parquet, or compressed CSV.
+    Some limitations exist for Parquet and compressed CSV.
+    See docs.trovares.com for more details.
     Each path may have its own protocol as described below.
 
     Parameters
     ----------
     paths : list or string
-      A single path or a list of paths to CSV files.
+      A single path or a list of paths to files.
 
       ==================== =====================================
-                      Syntax for one CSV file path
+                      Syntax for one file path
       ----------------------------------------------------------
           Resource type                 Path syntax
       ==================== =====================================
-          local to Python: '<path to csv file>'
-                           'xgt://<path to csv file>'
-          xGT server:      'xgtd://<path to csv file>'
-          AWS s3:          's3://<path to csv file>'
-          https site:      'https://<path to csv file>'
-          http site:       'http://<path to csv file>'
-          ftps server:     'ftps://<path to csv file>'
-          ftp server:      'ftp://<path to csv file>'
+          local to Python: '<path to file>'
+                           'xgt://<path to file>'
+          xGT server:      'xgtd://<path to file>'
+          AWS s3:          's3://<path to file>'
+          https site:      'https://<path to file>'
+          http site:       'http://<path to file>'
+          ftps server:     'ftps://<path to file>'
+          ftp server:      'ftp://<path to file>'
       ==================== =====================================
 
     headerMode : str
       Indicates how the file header should be processed:
         - HeaderMode.NONE:
           No header exists.
         - HeaderMode.IGNORE:
@@ -195,14 +198,15 @@
           is ignored.
         - HeaderMode.STRICT:
           Process the header in strict mode. The name of each header column
           should correspond to a schema column, a security label column, or be
           named IGNORE. Each schema column must appear in the file.
 
       Optional. Default=HeaderMode.NONE.
+      Only applies to CSV files.
 
     record_history : bool
       If true, records the history of the job.
       (since version 1.4.0)
 
     row_labels : list
       A list of security labels to attach to each row inserted with the load.
@@ -217,15 +221,16 @@
       NONE or IGNORE, this must be a list of integer column indices. If the
       header mode is NORMAL or STRICT, this must be a list of string column
       names. Note: Only one of row_labels and
       row_label_columns must be passed.
       (since version 1.5.0)
 
     delimiter : str
-      Delimiter for data.
+      Delimiter for CSV data.
+      Only applies to CSV files.
       (since version 1.5.1)
 
     Returns
     -------
     Job
       A Job object representing the job that has executed the load.
 
@@ -286,16 +291,16 @@
                           source_vertex_row_labels, target_vertex_row_labels,
                           delimiter, record_history = record_history, **kwargs)
 
   def save(self, path, offset = 0, length = None, headers = False,
            record_history = True, include_row_labels = False,
            row_label_column_header = None, preserve_order = False):
     """
-    Writes the rows from the frame to a CSV file in the path and the
-    computer indicated by the path.
+    Writes the rows from the frame to a CSV file in the location indicated
+    by the path parameter.
 
     Parameters
     ----------
     path : str
       Path to the CSV file.
 
       ==================== =====================================
@@ -378,91 +383,74 @@
     if len(server_paths) > 0:
       return self._egest(server_paths[0], headers,
                          record_history=record_history,
                          include_row_labels = include_row_labels,
                          row_label_column_header = row_label_column_header,
                          preserve_order = preserve_order, **kwargs)
 
+  def _create_insert_packet (self, frame_name, data, row_labels,
+                             row_label_columns, source_vertex_row_labels,
+                             target_vertex_row_labels):
+    request = data_proto.UploadDataRequest()
+    request.frame_name = self._name.encode('utf-8')
+    request.content_type = data_proto.CSV
+    request.header_mode = data_proto.NONE
+    request.content = data.encode('utf-8')
+    request.implicit_vertices = True
+    request.delimiter = ','
+    request.is_python_insert = True
+    request = _row_level_labels_helper(request, row_labels,
+                                       row_label_columns,
+                                       source_vertex_row_labels,
+                                       target_vertex_row_labels,
+                                       HeaderMode.NONE)
+    return request
+
   def _insert_packet_generator(self, data, is_pandas,
                                row_labels = None,
                                row_label_columns = None,
                                source_vertex_row_labels = None,
                                target_vertex_row_labels = None):
-    columns = []
-    column_types = {}
-    for item in self.schema:
-      columns.append(item[0])
-      column_types[item[0]] = item[1]
-    schemasize = len(columns)
     nrow = len(data)
-    col_names = '"' + ('","'.join(columns)) + '"'
+    buffer = ''
+    schema_size = len(self.schema)
+    col_type = [_[1] for _ in self.schema]
 
     try:
-      tbl = ''
-      for i in range(nrow):
-        row = ''
-        data_row = ''
-        if is_pandas:
-          length = len(data.columns)
-        else:
-          length = len(data[i])
-        for j in range(length):
-          if is_pandas:
-            col = data[columns[j]][i]
-          else:
-            col = data[i][j]
-          if j < schemasize:
-            col_type = column_types[columns[j]]
-            if col is None:
-              strcol = ''
-            else:
-              strcol = str(col)
-              if isinstance(col, bool):
-                  strcol = strcol.lower()
-              if isinstance(col, str):
-                  strcol = '"' + strcol + '"'
-            row = row + strcol + ','
-          else:
-            if col is None:
-              row = row + ','
-            else:
-              row = row + str(col) + ','
-        tbl = tbl + row[:-1] + '\n'
-        if len(tbl) >= MAX_PACKET_SIZE:
-          request = data_proto.UploadDataRequest()
-          request.frame_name = self._name.encode('utf-8')
-          request.content_type = data_proto.CSV
-          request.header_mode = data_proto.NONE
-          request.content = tbl.encode('utf-8')
-          request.implicit_vertices = True
-          request.delimiter = ','
-          request.is_python_insert = True
-          request = _row_level_labels_helper(request, row_labels,
-                                             row_label_columns,
-                                             source_vertex_row_labels,
-                                             target_vertex_row_labels,
-                                             HeaderMode.NONE)
-          yield request
-          tbl = ''
-      if len(tbl) > 0:
-        request = data_proto.UploadDataRequest()
-        request.frame_name = self._name.encode('utf-8')
-        request.content_type = data_proto.CSV
-        request.header_mode = data_proto.NONE
-        request.content = tbl.encode('utf-8')
-        request.implicit_vertices = True
-        request.delimiter = ','
-        request.is_python_insert = True
-        request = _row_level_labels_helper(request, row_labels,
-                                           row_label_columns,
+      if is_pandas:
+        import pandas
+        table = data.values
+      else:
+        table = data
+      for row in table:
+        row_str = [str(_) for _ in row]
+        for j in range(len(row)):
+          col = row[j]
+          if (is_pandas and j < schema_size and
+              col_type[j] == 'int' and pandas.isna(col)):
+            row_str[j] = ""
+          elif col is None:
+            row_str[j] = ""
+          elif isinstance(col, bool):
+            row_str[j] = row_str[j].lower()
+          elif isinstance(col, str):
+            row_str[j] = '"' + row_str[j] + '"'
+        buffer += ",".join(row_str) + '\n'
+        if len(buffer) >= MAX_PACKET_SIZE:
+          yield self._create_insert_packet(self._name, buffer,
+                                           row_labels, row_label_columns,
                                            source_vertex_row_labels,
-                                           target_vertex_row_labels,
-                                           HeaderMode.NONE)
-        yield request
-        tbl = ''
+                                           target_vertex_row_labels)
+          buffer = ''
+      if len(buffer) > 0:
+        yield self._create_insert_packet(self._name, buffer,
+                                         row_labels, row_label_columns,
+                                         source_vertex_row_labels,
+                                         target_vertex_row_labels)
+        buffer = ''
     except:
       #Print the error and don't throw since grpc will give an unknown error.
       traceback.print_exc(file=sys.stderr)
       sys.stderr.write("\n")
       pass
 
   def insert(self, data, row_labels = None,
@@ -1035,15 +1023,15 @@
   The source vertex of each edge in an EdgeFrame must belong to the same
   VertexFrame. This name of this VertexFrame is given by `EdgeFrame.source_name`.
   The targe vertex of each edge in an EdgeFrame must belong to the same
   VertexFrame. This name of this VertexFrame is given by `EdgeFrame.target_name`.
 
   For each edge in the EdgeFrame, its source vertex is identified by
   the edge property name given by `EdgeFrame.source_key`, which is
-  be one of the properties listed in the schema. The edge target vertex
+  one of the properties listed in the schema. The edge target vertex
   is identified by the property name given by `EdgeFrame.target_key`.
 
   Parameters
   ----------
   conn : Connection
     An open connection to an xGT server.
   name : str
@@ -1128,76 +1116,85 @@
     return print_frame
 
   def load(self, paths, headerMode = HeaderMode.NONE, record_history = True,
            row_labels = None, row_label_columns = None,
            source_vertex_row_labels = None, target_vertex_row_labels = None,
            delimiter = ','):
     """
-    Loads data from one or more CSV files specified in the list of paths.
+    Loads data from one or more files specified in the list of paths.
+    These files may be CSV, Parquet, or compressed CSV.
+    Some limitations exist for Parquet and compressed CSV.
+    See docs.trovares.com for more details.
     Each path may have its own protocol as described below.
 
     Parameters
     ----------
     paths : list or string
-      A single path or a list of paths to CSV files.
+      A single path or a list of paths to files.
 
       ==================== =====================================
-                      Syntax for one CSV file path
+                      Syntax for one file path
       ----------------------------------------------------------
           Resource type                 Path syntax
       ==================== =====================================
-          local to Python: '<path to csv file>'
-                           'xgt://<path to csv file>'
-          xGT server:      'xgtd://<path to csv file>'
-          AWS s3:          's3://<path to csv file>'
-          https site:      'https://<path to csv file>'
-          http site:       'http://<path to csv file>'
-          ftps server:     'ftps://<path to csv file>'
-          ftp server:      'ftp://<path to csv file>'
+          local to Python: '<path to file>'
+                           'xgt://<path to file>'
+          xGT server:      'xgtd://<path to file>'
+          AWS s3:          's3://<path to file>'
+          https site:      'https://<path to file>'
+          http site:       'http://<path to file>'
+          ftps server:     'ftps://<path to file>'
+          ftp server:      'ftp://<path to file>'
       ==================== =====================================
 
     headerMode : str
-      Indicates if the files contain headers:
+      Indicates if the CSV files contain headers:
         - HeaderMode.NONE
         - HeaderMode.IGNORE
         - HeaderMode.NORMAL
         - HeaderMode.STRICT
 
       Optional. Default=HeaderMode.NONE.
+      Only applies to CSV files.
 
     record_history : bool
       If true, records the history of the job.
       (since version 1.4.0)
 
     row_labels : list
       A list of security labels to attach to each row inserted with the load.
       Each label must have been passed in to the row_label_universe
       parameter when creating the frame. Note: Only one of row_labels
       and row_label_columns must be passed.
+      (since version 1.5.0)
 
     row_label_columns: list
       A list of columns indicating which columns in the CSV file contain
       security labels to attach to the inserted row. If the header mode is
       NONE or IGNORE, this must be a list of integer column indices. If the
       header mode is NORMAL or STRICT, this must be a list of string column
       names. Note: Only one of row_labels and
       row_label_columns must be passed.
+      (since version 1.5.0)
 
     source_vertex_row_labels : list
       A list of security labels to attach to each source vertex that is
       implicitly inserted. Each label must have been passed in to the
       row_label_universe parameter when creating the frame.
+      (since version 1.5.0)
 
     target_vertex_row_labels : list
       A list of security labels to attach to each target vertex that is
       implicitly inserted. Each label must have been passed in to the
       row_label_universe parameter when creating the frame.
+      (since version 1.5.0)
 
     delimiter : str
-      Delimiter for data.
+      Delimiter for CSV data.
+      Only applies to CSV files.
       (since version 1.5.1)
 
     Returns
     -------
     Job
       A Job object representing the job that has executed the load.
 
@@ -1358,7 +1355,11 @@
   return client_paths, server_paths, url_paths
 
 def _validate_client_path(one_path):
   if one_path.endswith('.gz') or one_path.endswith('.bz2'):
     msg = 'Loading compressed files from a local filesystem is ' \
           'not supported: {0}'.format(one_path)
     raise XgtNotImplemented(msg)
+  elif one_path.endswith('.parquet'):
+    msg = 'Loading parquet files from a local filesystem is ' \
+          'not supported: {0}'.format(one_path)
+    raise XgtNotImplemented(msg)
```

### Comparing `xgt-1.8.0/src/xgt/job.py` & `xgt-1.9.0/src/xgt/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __str__(self):
       return "(" + self._label + ":" + self._frame + ")"
 
   class _QueryPlanEdge(object):
     def __init__(self, query_edge_message):
       if query_edge_message.edge_direction == \
-         job_proto.QueryEdgeDirection.Value('FORWARD'):
+         sch_proto.QueryEdgeDirection.Value('FORWARD'):
         self.forward_edge = True
       else:
         self.forward_edge = False
       self._source_label = query_edge_message.source_label
       self._source_frame = query_edge_message.source_frame
       self._edge_label = query_edge_message.edge_label
       self._edge_frame = query_edge_message.edge_frame
@@ -88,15 +88,15 @@
     # that starts with MATCH in cypher and contains elements representing
     # edges or (if only a single frame was matched), a vertex or table.
     self._plan = []
     for query in query_plan_response.plan_as_edge_list:
       query_representation = []
       for element in query.edges:
         if element.edge_direction == \
-           job_proto.QueryEdgeDirection.Value('NOT_EDGE'):
+           sch_proto.QueryEdgeDirection.Value('NOT_EDGE'):
           query_representation.append(self._QueryPlanSingleFrame(element))
         else:
           query_representation.append(self._QueryPlanEdge(element))
       self._plan.append(query_representation)
 
   def __str__(self):
     as_string = ""
@@ -164,24 +164,24 @@
   server.
 
   The job_response parameter is a single element of the array returned by the
   output of a job creation gRPC call.  Each individual element in the array will
   be constructed as a separate `Job` object.
 
   """
-  def __init__(self, conn, job_response, query_plan = None):
+  def __init__(self, conn, job_response):
     """
     Constructor for Job. Called when Job is created.
     """
     self._conn = conn
     self._id = job_response.job_id
     self._user = job_response.user
-    self._data = self._parse_job_data(job_response, query_plan)
+    self._data = self._parse_job_data(job_response)
 
-  def _parse_job_data(self, job_response, query_plan = None):
+  def _parse_job_data(self, job_response):
     job_data = {
       'jobid': job_response.job_id,
       'user': job_response.user,
       'status': sch_proto.JobStatusEnum.Name(job_response.status).lower(),
       'start_time': job_response.start_time.ToDatetime().isoformat(),
       'end_time': job_response.end_time.ToDatetime().isoformat(),
       'error_type': None,
@@ -198,16 +198,16 @@
     if job_response.row and len(job_response.row) > 0:
       job_data['rows'] = [data for data in job_response.row]
     if job_response.error and len(job_response.error) > 0:
         error_code_name = err_proto.ErrorCodeEnum.Name(job_response.error[0].code)
         job_data['error_type'] = _code_error_map[error_code_name]
         job_data['error'] = ', '.join([e.message for e in job_response.error])
         job_data['trace'] = ', '.join([e.detail for e in job_response.error])
-    if query_plan is not None:
-      job_data['query_plan'] =  _QueryPlan(query_plan)
+    if job_response.HasField('query_plan'):
+      job_data['query_plan'] =  _QueryPlan(job_response.query_plan)
 
     return job_data
 
   def _get_job_data(self):
     request = job_proto.GetJobsRequest()
     request.job_id.extend([self._id])
     responses = self._conn._call(request, self._conn._job_svc.GetJobs)
```

### Comparing `xgt-1.8.0/src/xgt.egg-info/PKG-INFO` & `xgt-1.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: xgt
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Python interface to the Trovares xGT graph analytics engine.
 Home-page: http://www.trovares.com/
 Author: Trovares, Inc.
 Author-email: support@trovares.com
 License: apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
 
 
 xGT is a high-performance property graph engine designed to support extremely large in-memory graphs, and the `xgt` library is the client-side interface which controls it.
```

### Comparing `xgt-1.8.0/src/xgt.egg-info/SOURCES.txt` & `xgt-1.9.0/src/xgt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xgt-1.8.0/setup.py` & `xgt-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ## Documentation
 
 The `xgt` library is self-documenting, and all external methods and classes have docstrings accessible through `help()`.
 A formatted version of the same is available online on the Trovares documentation site: [docs.trovares.com](http://docs.trovares.com/)
 '''
 
 setup(name='xgt',
-      version='1.8.0',
+      version='1.9.0',
       author='Trovares, Inc.',
       author_email='support@trovares.com',
       description='The Python interface to the Trovares xGT graph analytics engine.',
       license='apache2',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://www.trovares.com/',
@@ -48,12 +48,15 @@
       install_requires=requirements,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Database',
         'Topic :: Database :: Front-Ends',
       ]
 )
```

### Comparing `xgt-1.8.0/PKG-INFO` & `xgt-1.9.0/src/xgt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: xgt
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Python interface to the Trovares xGT graph analytics engine.
 Home-page: http://www.trovares.com/
 Author: Trovares, Inc.
 Author-email: support@trovares.com
 License: apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
 
 
 xGT is a high-performance property graph engine designed to support extremely large in-memory graphs, and the `xgt` library is the client-side interface which controls it.
```

