# Comparing `tmp/blickfeld_qb2-1.9.0.tar.gz` & `tmp/blickfeld_qb2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blickfeld_qb2-1.9.0.tar", last modified: Wed Oct  4 23:05:54 2023, max compression
+gzip compressed data, was "blickfeld_qb2-2.0.7.tar", last modified: Thu Apr  4 06:18:50 2024, max compression
```

## Comparing `blickfeld_qb2-1.9.0.tar` & `blickfeld_qb2-2.0.7.tar`

### file list

```diff
@@ -1,138 +1,159 @@
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-10-04 23:05:47.000000 blickfeld_qb2-1.9.0/LICENSE.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/PKG-INFO
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      331 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/base/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/base/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/base/geometry/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/geometry/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4058 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/channel.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/device_ca_cert.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1045 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/_types.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/_version.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/casing.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/compile/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/compile/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/compile/importing.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/compile/naming.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/grpclib_client.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/grpclib_server.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/util/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/util/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/util/async_channel.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/__main__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/compiler.py
--rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/main.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/models.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/parser.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2229 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    14008 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    22989 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      858 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/detector/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      985 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1935 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5067 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1390 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    17829 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/flow/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7113 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/laser/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.368019 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10016 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3196 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    26019 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6620 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    18727 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/push/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/push/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/push/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3196 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/push/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/push/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/push/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/push/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/push/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/system/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/system/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/system/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10781 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/system/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/system/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6510 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/system/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/blickfeld_qb2/system/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    35909 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/blickfeld_qb2/system/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-10-04 23:05:54.364019 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-10-04 23:05:54.000000 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/PKG-INFO
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3277 2023-10-04 23:05:54.000000 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/SOURCES.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-10-04 23:05:54.000000 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/dependency_links.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-10-04 23:05:54.000000 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/requires.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-10-04 23:05:54.000000 blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/top_level.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-10-04 23:05:54.372020 blickfeld_qb2-1.9.0/setup.cfg
--rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-10-04 23:05:53.000000 blickfeld_qb2-1.9.0/setup.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2024-04-04 06:18:37.000000 blickfeld_qb2-2.0.7/LICENSE.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/PKG-INFO
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      493 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4464 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2253 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2411 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3394 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4319 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/channel.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/device_ca_cert.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      798 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1418 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4145 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    55198 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/_types.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/_version.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/casing.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/importing.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/naming.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_server.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/async_channel.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/__main__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/compiler.py
+-rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/main.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    28742 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/models.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     8046 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/parser.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/config/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      833 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/config/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2742 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    14010 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21357 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      860 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3979 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2566 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6691 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12120 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1066 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1392 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21734 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      701 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7115 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1855 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3845 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12464 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3652 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    27189 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    11738 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21372 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      757 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10548 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3198 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2330 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15034 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2725 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/token_factory.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5345 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1291 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    38039 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15151 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     8720 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    40554 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/PKG-INFO
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3703 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/SOURCES.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/dependency_links.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/requires.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/top_level.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/setup.cfg
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/setup.py
```

### Comparing `blickfeld_qb2-1.9.0/LICENSE.txt` & `blickfeld_qb2-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/base/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from . import data
+from . import config
+from . import geometry
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/base/options/access_control.proto, blickfeld/base/options/misc.proto, blickfeld/base/options/protocol_maturity.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 class AccessControlLevel(betterproto.Enum):
     """
-    Available access levels The levels are ordered ascending, which means that
-    each level also inherits the permissions of the levels above it.
+    Available access levels The levels are ordered in ascending order, which
+    means that each level also inherits the permissions of the levels above it.
     """
 
     LEVEL_UNSPECIFIED = 0
     """Access level is not specified"""
 
     LEVEL_PUBLIC = 1
     """
@@ -30,17 +34,16 @@
     ADMIN access level. If desired, the AUTHORIZED access level can be
     configured to act equally to the PUBLIC access level.
     """
 
     LEVEL_ADMIN = 3
     """
     Only administrative clients can access The corresponding entities are
-    mainly used to configure the access tokens of the AUTHORIZED access level.
-    It may also be used to manage configuration which might void the warranty
-    or specification of the device.
+    mainly used to configure the accounts with AUTHORIZED & ADMIN access
+    levels.
     """
 
     LEVEL_SUPPORT = 4
     """
     Only clients of the Blickfeld support can access The corresponding entities
     can only be accessed by Blickfeld Support Tools & clients. The access
     tokens are bound to devices.
@@ -55,39 +58,39 @@
     LEVEL_DEVELOPER = 6
     """Only Blickfeld developers can access"""
 
 
 class ProtocolMaturityLevel(betterproto.Enum):
     """
     This enumeration describes the maturity of a protocol. Please refer to the
-    individual values. [IMPORTANT] APIs marked with the EXPERIMENTAL &
+    individual values. [IMPORTANT] APIs marked with the EXPERIMENTAL and
     DEPRECATED flags have to be handled with care. Please read through the
     definition. Please report if the protocol maturity of a service, method,
     and field does not fit e.g. if an EXPERIMENTAL field is required in an
-    application & production use case.
+    application and production use case.
     """
 
     LEVEL_UNSPECIFIED = 0
     """
     Level is not set. Default level for services is EXPERIMENTAL. Default level
-    for methods & fields is INHERITED.
+    for methods and fields is INHERITED.
     """
 
     LEVEL_EXPERIMENTAL = 1
     """
     APIs marked with this flag should be handled with care. They might not
-    function as expected. Additionally it is not ensure that the APIs will ever
-    be moved to the MAINTAINED level. They might be altered or removed in any
-    upcoming release without further notice.
+    function as expected. Additionally it is not ensured that the APIs will
+    ever be moved to the MAINTAINED level. They might be altered or removed in
+    any upcoming release without further notice.
     """
 
     LEVEL_MAINTAINED = 2
     """
     APIs marked with this flag are actively maintained and released. They will
-    not change their behaviour without notices in the changelog. Breaking
+    not change their behavior without notices in the changelog. Breaking
     changes in a maintained APIs have to result in a major update of the
     module.
     """
 
     LEVEL_DEPRECATED = 3
     """
     APIs marked with this flag are no longer actively maintained. They will be
@@ -97,31 +100,34 @@
     LEVEL_INHERITED = 4
     """The protocol maturity is inherited from the parent"""
 
 
 @dataclass(eq=False, repr=False)
 class AccessControl(betterproto.Message):
     """
-    Access Control message which specifies the required access level and
-    licenses for protocol entities. Protocol entities are usually gRPC services
-    but can also be more fine grained on gRPC method and Protobuf field level.
+    The Access Control message specifies the required access level and licenses
+    for protocol entities. Protocol entities are usually gRPC services but can
+    also be more fine grained on gRPC method and Protobuf field level.
     """
 
     level: "AccessControlLevel" = betterproto.enum_field(1)
     """Minimum access level required for entity"""
 
+    read_only: bool = betterproto.bool_field(2)
+    """True if the entity can be accessed with read-only permissions"""
+
 
 @dataclass(eq=False, repr=False)
 class LinkData(betterproto.Message):
     type: str = betterproto.string_field(1)
     directory: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class ProtocolMaturity(betterproto.Message):
     """
-    This message specifies the maturity of a protocol for customer- &
+    This message specifies the maturity of a protocol for customer- and
     production-facing APIs.
     """
 
     level: "ProtocolMaturityLevel" = betterproto.enum_field(1)
     """Simple level which describes maturity"""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/base/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/base/data/health.proto, blickfeld/base/data/version.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 class HealthState(betterproto.Enum):
     """
-    High-level state which indicates the current health state of the module. If
-    the State is not OK, please refer to the details fields in the Health
+    A high-level state which indicates the current health state of the module.
+    If the State is not OK, please refer to the details fields in the Health
     message to trace the root cause.
     """
 
     STATE_UNSPECIFIED = 0
     """The current state is unknown."""
 
     STATE_OK = 1
@@ -33,29 +35,29 @@
     """The module is currently busy. Requests might get aborted or delayed."""
 
 
 @dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """
     The Health message and corresponding services are used to indicate their
-    health & status. They are available on different layers. Upstream / higher
-    layers usually aggregate the Health of their child modules. In the end, the
-    goal is, to get an aggregated product Health which reliably indicates if
+    health and status. They are available on different layers. Upstream or
+    higher layers usually aggregate the health of their child modules. The goal
+    is to provide an aggregated product health that reliably indicates if
     everything is functional.
     """
 
     pass
 
 
 @dataclass(eq=False, repr=False)
 class Version(betterproto.Message):
     """
-    General message which is used for version information.
-    https://semver.org[Semantic versioning] is used to identify a software
-    state. It additional adds the short hash of the corresponding commit.
+    A general message used for version information. https://semver.org[Semantic
+    versioning] is used to identify a software state. It additionaly adds the
+    short hash of the corresponding commit.
     """
 
     major: int = betterproto.uint32_field(1)
     """Increments when we make incompatible API changes."""
 
     minor: int = betterproto.uint32_field(2)
     """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/base/geometry/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/base/geometry/axis.proto, blickfeld/base/geometry/pose.proto, blickfeld/base/geometry/quaternion.proto, blickfeld/base/geometry/shape.proto, blickfeld/base/geometry/transform.proto, blickfeld/base/geometry/vector3.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
@@ -38,68 +40,83 @@
 
     w: float = betterproto.float_field(4)
     """The W component (real part)."""
 
 
 @dataclass(eq=False, repr=False)
 class Vector3(betterproto.Message):
-    """A vector with three components to represent a 3D coordiante."""
+    """A vector with three components to represent a 3D coordinate."""
 
     x: float = betterproto.float_field(1)
     """The X component."""
 
     y: float = betterproto.float_field(2)
     """The Y component."""
 
     z: float = betterproto.float_field(3)
     """The Z component."""
 
 
 @dataclass(eq=False, repr=False)
+class Transform(betterproto.Message):
+    """A rigid transformation"""
+
+    translation: "Vector3" = betterproto.message_field(1)
+    """A vector representing the position."""
+
+    rotation: "Quaternion" = betterproto.message_field(2)
+    """A quaternion representing the rotation."""
+
+
+@dataclass(eq=False, repr=False)
 class Pose(betterproto.Message):
     """A pose, consisting of a vector3 (3D coordinate) and a quaternion."""
 
     position: "Vector3" = betterproto.message_field(1)
     """A vector representing the position."""
 
     orientation: "Quaternion" = betterproto.message_field(2)
     """A quaternion representing the orientation."""
 
 
 @dataclass(eq=False, repr=False)
 class Shape(betterproto.Message):
-    """A shape that represent a geometrical figure."""
+    """A shape that represents a geometrical figure."""
 
     pose: "Pose" = betterproto.message_field(1)
     """
     Position and orientation of the center of the bounding box enclosing the
     shape.
     """
 
     box: "ShapeBox" = betterproto.message_field(2, group="shape_type")
     """Box shape"""
 
+    cone: "ShapeCone" = betterproto.message_field(3, group="shape_type")
+    """Cone shape"""
+
 
 @dataclass(eq=False, repr=False)
 class ShapeBox(betterproto.Message):
     """A 3 dimensional box."""
 
     dimensions: "Vector3" = betterproto.message_field(1)
     """The X, Y and Z dimension."""
 
 
 @dataclass(eq=False, repr=False)
-class Transform(betterproto.Message):
-    """A rigid transformation"""
-
-    translation: "Vector3" = betterproto.message_field(1)
-    """A vector representing the position."""
+class ShapeCone(betterproto.Message):
+    """A 3 dimensional cone."""
 
-    rotation: "Quaternion" = betterproto.message_field(2)
-    """A quaternion representing the rotation."""
+    dimensions: "Vector3" = betterproto.message_field(1)
+    """
+    The X, Y and Z dimension of the cone. X and Y dimensions of the cone define
+    the ellipsoid at the bottom of the cone. The cone is narrowing along the z
+    direction.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Axis(betterproto.Message):
     """Axis of a coordinate system."""
 
     type: "AxisType" = betterproto.enum_field(1)
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/channel.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ssl
 from grpclib.client import Channel as gRPClibChannel
+from grpclib.config import Configuration
 from tempfile import mkstemp
 from .device_ca_cert import ca_cert
 from grpclib.events import SendRequest, listen
 import inspect
 import os
 
 
@@ -23,15 +24,21 @@
     :type port: uint
     :param device_ca_cert: String containing a root certificate for SSL connection
     :type device_ca_cert: str
     :param token: String containing an access token or an awaitable which is called on every method call
     """
 
     def __init__(
-        self, fqdn_or_ip: str, serial_number: str = None, port=55551, device_ca_cert=ca_cert, token=None, metadata=None
+        self,
+        fqdn_or_ip: str,
+        serial_number: str = None,
+        port: int = None,
+        device_ca_cert=ca_cert,
+        token=None,
+        metadata=None,
     ) -> None:
         # Store all properties to allow clone
         self.fqdn_or_ip = fqdn_or_ip
         self.serial_number = serial_number
         self.port = port
         self.device_ca_cert = device_ca_cert
         self.token = token
@@ -41,32 +48,35 @@
         fd, key_and_cert_file = mkstemp()
         with open(fd, "w") as f:
             f.write(device_ca_cert)
 
         # create SSL context for client
         ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)  # client side context
         ctx.verify_mode = ssl.CERT_REQUIRED  # TLS
-        ctx.check_hostname = False  # disable hostname check
+        ctx.check_hostname = serial_number is not None
         ctx.set_alpn_protocols(["h2"])
         try:
             ctx.load_verify_locations(cafile=key_and_cert_file)
         except ssl.SSLError as error:
             raise RuntimeError("Device CA certificate is of incorrect format:" + error.reason)
 
-        # TODO This always uses insecure connections as there is not detection yet
-        #      which checks if a secure connection would work.
-        if os.getenv("BF_ALLOW_INSECURE_CONNECTIONS") is not None:
-            print(f"Using insecure connection to {fqdn_or_ip} as BF_ALLOW_INSECURE_CONNECTIONS is set")
-            port = 50051
+        # Set name for hostname check to Qb2 device name
+        device_name = serial_number + ".qb2.blickfeld.com" if serial_number else None
+        config = Configuration(ssl_target_name_override=device_name) if device_name else None
+
+        # Establish TLS connection to verify connectivity
+        channel_port = port or 55551
+        if os.getenv("BF_ALLOW_INSECURE_CONNECTIONS") is not None and token is None:
+            print(f"Using insecure connection for {fqdn_or_ip} as BF_ALLOW_INSECURE_CONNECTIONS is set")
+            channel_port = port or 50051
             ctx = None
-
-        # TODO Check serial number. Authentication of device serial number is not yet implemented.
+            config = None
 
         # establish gRPC secured channel
-        super().__init__(host=fqdn_or_ip, port=port, ssl=ctx)
+        super().__init__(host=fqdn_or_ip, port=channel_port, ssl=ctx, config=config)
         # if token is provided -> inject it to every outgoing send request
         if token:
             listen(self, SendRequest, self.__inject_token)
 
         if metadata:
             listen(self, SendRequest, self.__inject_metadata)
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/base/grpc/device_ca_cert.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/device_ca_cert.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/beam_deflection_control/config/module.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/beam_deflection_control/data/health.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
@@ -18,17 +20,26 @@
 
     state: "__base_data__.HealthState" = betterproto.enum_field(1)
     """High-level state of module"""
 
     state_reason: str = betterproto.string_field(2)
     """Reason for given state. Is not set if state is OK."""
 
+    stats: "HealthStats" = betterproto.message_field(6)
+    """Stats giving basic information about the mirror operation"""
+
 
 @dataclass(eq=False, repr=False)
 class HealthStats(betterproto.Message):
     """
     This message defines the stats that can be retrieved from a beam deflection
     controller.
     """
 
     time: float = betterproto.float_field(1)
-    """Current time in s."""
+    """Time in seconds since last operation start."""
+
+    control_effort: float = betterproto.float_field(9)
+    """
+    Control effort usage. Relative value indicating how much of the maximum
+    available effort is currently used to control the deflection mirror.
+    """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/beam_deflection_control/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/beam_deflection_control/services/health.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -26,23 +28,23 @@
 
 
 @dataclass(eq=False, repr=False)
 class HealthGetResponse(betterproto.Message):
     """Message containing the health data for a single get request"""
 
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 @dataclass(eq=False, repr=False)
 class HealthWatchResponse(betterproto.Message):
     """Message containing the health data for a watch stream"""
 
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 class Health(betterproto.ServiceStub):
     """
     The health service provides methods to monitor the instant operational
     status of the beam deflection controller
     """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     # Groups several "one-of" fields together
     group: Optional[str] = None
     # Describes the wrapped type (e.g. when using google.protobuf.BoolValue)
     wraps: Optional[str] = None
     # Is the field optional
     optional: Optional[bool] = False
     # Numpy format
-    numpy_dtype : Optional[str] = None
+    numpy_dtype: Optional[str] = None
 
     @staticmethod
     def get(field: dataclasses.Field) -> "FieldMetadata":
         """Returns the field metadata for a dataclass field."""
         return field.metadata["betterproto"]
 
 
@@ -175,15 +175,15 @@
     number: int,
     proto_type: str,
     *,
     map_types: Optional[Tuple[str, str]] = None,
     group: Optional[str] = None,
     wraps: Optional[str] = None,
     optional: bool = False,
-    numpy_dtype: Optional[str] = None
+    numpy_dtype: Optional[str] = None,
 ) -> dataclasses.Field:
     """Creates a dataclass field with attached protobuf metadata."""
     return dataclasses.field(
         default=None if optional else PLACEHOLDER,
         metadata={
             "betterproto": FieldMetadata(
                 number, proto_type, map_types, group, wraps, optional, numpy_dtype
@@ -280,17 +280,22 @@
 def string_field(
     number: int, group: Optional[str] = None, optional: bool = False
 ) -> Any:
     return dataclass_field(number, TYPE_STRING, group=group, optional=optional)
 
 
 def bytes_field(
-    number: int, group: Optional[str] = None, optional: bool = False, numpy_dtype: Optional[str] = None
+    number: int,
+    group: Optional[str] = None,
+    optional: bool = False,
+    numpy_dtype: Optional[str] = None,
 ) -> Any:
-    return dataclass_field(number, TYPE_BYTES, group=group, optional=optional, numpy_dtype=numpy_dtype)
+    return dataclass_field(
+        number, TYPE_BYTES, group=group, optional=optional, numpy_dtype=numpy_dtype
+    )
 
 
 def message_field(
     number: int,
     group: Optional[str] = None,
     wraps: Optional[str] = None,
     optional: bool = False,
@@ -631,15 +636,14 @@
     def __post_init__(self) -> None:
         # Keep track of whether every field was default
         all_sentinel = True
 
         # Set current field of each group after `__init__` has already been run.
         group_current: Dict[str, Optional[str]] = {}
         for field_name, meta in self._betterproto.meta_by_field_name.items():
-
             if meta.group:
                 group_current.setdefault(meta.group)
 
             value = self.__raw_get(field_name)
             if value != PLACEHOLDER and not (meta.optional and value is None):
                 # Found a non-sentinel value
                 all_sentinel = False
@@ -783,16 +787,22 @@
             # set (or received empty).
             serialize_empty = isinstance(value, Message) and value._serialized_on_wire
 
             include_default_value_for_oneof = self._include_default_value_for_oneof(
                 field_name=field_name, meta=meta
             )
 
-            if type(value) is not np.ndarray and value == self._get_field_default(field_name) and not (
-                selected_in_group or serialize_empty or include_default_value_for_oneof
+            if (
+                type(value) is not np.ndarray
+                and value == self._get_field_default(field_name)
+                and not (
+                    selected_in_group
+                    or serialize_empty
+                    or include_default_value_for_oneof
+                )
             ):
                 # Default (zero) values are not serialized. Two exceptions are
                 # if this is the selected oneof item or if we know we have to
                 # serialize an empty message (i.e. zero value was explicitly
                 # set by the user).
                 continue
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/casing.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/compile/importing.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/grpclib_client.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/grpclib_server.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/grpc/util/async_channel.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/compiler.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/main.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/models.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,14 @@
         return get_comment(
             proto_file=self.source_file, path=self.path, indent=self.comment_indent
         )
 
 
 @dataclass
 class PluginRequestCompiler:
-
     plugin_request_obj: CodeGeneratorRequest
     output_packages: Dict[str, "OutputTemplate"] = field(default_factory=dict)
 
     @property
     def all_messages(self) -> List["MessageCompiler"]:
         """All of the messages in this request.
 
@@ -395,17 +394,22 @@
         """Construct string representation of this field as a field."""
         name = f"{self.py_name}"
         annotations = f": {self.annotation}"
         field_args = ", ".join(
             ([""] + self.betterproto_field_args) if self.betterproto_field_args else []
         )
         betterproto_field_type = (
-            f"betterproto.{self.field_type}_field({self.proto_obj.number}{field_args}, numpy_dtype='{self.proto_obj.options.blickfeld_base_numpy_dtype}')"
-        ) if self.field_type == "bytes" and self.proto_obj.options.blickfeld_base_numpy_dtype else (
-            f"betterproto.{self.field_type}_field({self.proto_obj.number}{field_args})"
+            (
+                f"betterproto.{self.field_type}_field({self.proto_obj.number}{field_args}, numpy_dtype='{self.proto_obj.options.blickfeld_base_numpy_dtype}')"
+            )
+            if self.field_type == "bytes"
+            and self.proto_obj.options.blickfeld_base_numpy_dtype
+            else (
+                f"betterproto.{self.field_type}_field({self.proto_obj.number}{field_args})"
+            )
         )
         if self.py_name in dir(builtins):
             self.parent.builtins_types.add(self.py_name)
         return f"{name}{annotations} = {betterproto_field_type}"
 
     @property
     def betterproto_field_args(self) -> List[str]:
@@ -684,15 +688,14 @@
     @property
     def py_name(self) -> str:
         return pythonize_class_name(self.proto_name)
 
 
 @dataclass
 class ServiceMethodCompiler(ProtoContentBase):
-
     source_file: FileDescriptorProto
     parent: ServiceCompiler
     proto_obj: MethodDescriptorProto
     path: List[int] = PLACEHOLDER
     comment_indent: int = 8
 
     def __post_init__(self) -> None:
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/betterproto/plugin/parser.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,16 +77,15 @@
         output_package_name = proto_file.package
         if output_package_name not in request_data.output_packages:
             # Create a new output if there is no output for this package
             request_data.output_packages[output_package_name] = OutputTemplate(
                 parent_request=request_data, package_proto_obj=proto_file
             )
         # Add this input file to the output corresponding to this package
-        request_data.output_packages[output_package_name].input_files.append(
-            proto_file)
+        request_data.output_packages[output_package_name].input_files.append(proto_file)
 
         if (
             proto_file.package == "google.protobuf"
             and "INCLUDE_GOOGLE" not in plugin_options
         ):
             # If not INCLUDE_GOOGLE,
             # skip outputting Google's well-known types
@@ -105,33 +104,46 @@
                     output_package=output_package,
                 )
 
     # Read Services
     for output_package_name, output_package in request_data.output_packages.items():
         for proto_input_file in output_package.input_files:
             for index, service in enumerate(proto_input_file.service):
-                read_protobuf_service(
-                    proto_input_file, service, index, output_package)
+                read_protobuf_service(proto_input_file, service, index, output_package)
 
     # Generate output files
     output_paths: Set[pathlib.Path] = set()
     for output_package_name, output_package in request_data.output_packages.items():
         if not output_package.output:
             continue
 
         # Add files to the response object
-        output_path = pathlib.Path(
-            *output_package_name.split("."), "__init__.py")
+        output_path = pathlib.Path(*output_package_name.split("."), "__init__.py")
         output_paths.add(output_path)
 
+        paths = map(
+            lambda k: pathlib.Path(*k.split("."), "__init__.py"),
+            request_data.output_packages.keys(),
+        )
+
+        content = (
+            "\n".join(
+                f"from . import {path.parent.name}"
+                for path in paths
+                if len(path.parents) > 1 and output_path.parent == list(path.parents)[1]
+            )
+            + "\n\n"
+            + outputfile_compiler(output_file=output_package)
+        )
+
         response.file.append(
             CodeGeneratorResponseFile(
                 name=str(output_path),
                 # Render and then format the output file
-                content=outputfile_compiler(output_file=output_package),
+                content=content,
             )
         )
 
     # Make each output directory a package with __init__ file
     init_files = {
         directory.joinpath("__init__.py")
         for path in output_paths
@@ -139,16 +151,25 @@
         if not directory.joinpath("__init__.py").exists()
     } - output_paths
 
     for init_file in init_files:
         output_paths.add(init_file)
 
     for init_file in init_files:
-        response.file.append(CodeGeneratorResponseFile(name=str(init_file), content="\n".join(
-            f"from . import {path.parent.name}" for path in output_paths if len(path.parents) > 1 and init_file.parent == list(path.parents)[1])))
+        response.file.append(
+            CodeGeneratorResponseFile(
+                name=str(init_file),
+                content="\n".join(
+                    f"from . import {path.parent.name}"
+                    for path in output_paths
+                    if len(path.parents) > 1
+                    and init_file.parent == list(path.parents)[1]
+                ),
+            )
+        )
 
     for output_package_name in sorted(output_paths.union(init_files)):
         print(f"Writing {output_package_name}", file=sys.stderr)
 
     return response
 
 
@@ -192,18 +213,25 @@
         # Enum
         EnumDefinitionCompiler(
             source_file=source_file, parent=output_package, proto_obj=item, path=path
         )
 
 
 def read_protobuf_service(
-    source_file: "FileDescriptorProto", service: ServiceDescriptorProto, index: int, output_package: OutputTemplate
+    source_file: "FileDescriptorProto",
+    service: ServiceDescriptorProto,
+    index: int,
+    output_package: OutputTemplate,
 ) -> None:
     service_data = ServiceCompiler(
-        source_file=source_file, parent=output_package, proto_obj=service, path=[
-            6, index]
+        source_file=source_file,
+        parent=output_package,
+        proto_obj=service,
+        path=[6, index],
     )
     for j, method in enumerate(service.method):
         ServiceMethodCompiler(
-            source_file=source_file, parent=service_data, proto_obj=method, path=[
-                6, index, 2, j]
+            source_file=source_file,
+            parent=service_data,
+            proto_obj=method,
+            path=[6, index, 2, j],
         )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,43 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/core_processing/config/demo_recording.proto, blickfeld/core_processing/config/health.proto, blickfeld/core_processing/config/point_cloud.proto
+# sources: blickfeld/core_processing/config/health.proto, blickfeld/core_processing/config/point_cloud.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from .. import data as _data__
 
 
-class DemoRecording(betterproto.Enum):
+class PointCloudFilterSorting(betterproto.Enum):
     """
-    Demo recording which can be replayed instead of the real sensor data. This
-    is also used for virtual devices which have no physical sensing unit.
-    WARNING: The recordings are still preliminary. The demo test data concept
-    will be refactored soon.
+    Configure sorting of return candidates. The sorting is always descending
+    thus the higher the value is, the lower is the return id.
     """
 
-    DEMO_RECORDING_UNSPECIFIED = 0
-    """No demo recoding is specified"""
-
-    DEMO_RECORDING_HIGH_RESOLUTION = 1
-    """High resolution recording in the office with 200 + 30 scanlines"""
+    SORTING_UNSPECIFIED = 0
+    """No sorting specified."""
 
-    DEMO_RECORDING_HIGH_FRAME_RATE = 2
-    """High resolution recording in the office with 30 + 30 scanlines"""
-
-
-@dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """Configuration parameters for the health message"""
+    SORTING_INTENSITY = 1
+    """Sort returns by intensity (integral of return pulse)."""
 
-    point_rate_lower_limit: int = betterproto.uint32_field(1)
+    SORTING_REFLECTIVITY = 2
     """
-    Set the point rate lower limit. If the point rate is lower than this limit,
-    the device is considered to be covered.
+    Sort returns by reflectivity (range-compensated intensity). This can
+    improve the SNR as closer points are getting a lower weight.
     """
 
-    point_cloud_alignment_deviation_norm_upper_limit: float = betterproto.float_field(2)
-    """The limit to detect the alignment has changed."""
-
-    point_cloud_reference_alignment: "_data__.Acceleration" = betterproto.message_field(
-        3
-    )
-    """Set the point cloud reference alignment."""
+    SORTING_RANGE = 3
+    """
+    Sort returns by range. This can improve the SNR for outdoor applications
+    with rain and snow.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class PointCloud(betterproto.Message):
     """Configuration parameters for the point cloud"""
 
     pass
@@ -58,7 +48,41 @@
     """Filter configuration which can be applied on point cloud frames."""
 
     maximum_returns_per_point: int = betterproto.uint32_field(1)
     """
     Set maximum number of returns per point. By default, secondary returns are
     disabled. Set this, e.g. to 2, to enable secondary returns.
     """
+
+    sorting: "PointCloudFilterSorting" = betterproto.enum_field(3)
+    """
+    Select sorting method for return candidates. The default sorting is by
+    intensity.
+    """
+
+    minimum_reflectivity: int = betterproto.uint32_field(4)
+    """
+    Set lower threshold for reflectivity. This can be tuned to improve the SNR
+    when low-reflectivity targets have a lower priority.
+    """
+
+    minimum_range: float = betterproto.float_field(5)
+    """Set lower threshold for range. Default value is 1m."""
+
+
+@dataclass(eq=False, repr=False)
+class Health(betterproto.Message):
+    """Configuration parameters for the health message"""
+
+    point_rate_lower_limit: int = betterproto.uint32_field(1)
+    """
+    Set the point rate lower limit. If the point rate is lower than this limit,
+    the device is considered to be covered.
+    """
+
+    point_cloud_alignment_deviation_norm_upper_limit: float = betterproto.float_field(2)
+    """The limit to detect the alignment has changed."""
+
+    point_cloud_reference_alignment: "_data__.Acceleration" = betterproto.message_field(
+        3
+    )
+    """Set the point cloud reference alignment."""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/core_processing/data/acceleration.proto, blickfeld/core_processing/data/acceleration_buffer.proto, blickfeld/core_processing/data/frame.proto, blickfeld/core_processing/data/health.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from typing import Dict
 
 import blickfeld_qb2.betterproto as betterproto
@@ -55,31 +57,14 @@
     """
 
     timestamp: np.ndarray = betterproto.bytes_field(6, numpy_dtype="<u8")
     """Unix timestamp of points. Type: UInt64"""
 
 
 @dataclass(eq=False, repr=False)
-class AccelerationBuffer(betterproto.Message):
-    """Buffer for multiple Acceleration samples"""
-
-    timestamp: int = betterproto.uint64_field(1)
-    """Timestamp of the first sample in the buffer."""
-
-    sampling_period: int = betterproto.uint64_field(2)
-    """Sampling period of the acceleration samples"""
-
-    cartesian: bytes = betterproto.bytes_field(3)
-    """
-    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
-    Type: Float32
-    """
-
-
-@dataclass(eq=False, repr=False)
 class Acceleration(betterproto.Message):
     """A measurement of the Accelerometer"""
 
     x: float = betterproto.float_field(1)
     """X component of acceleration vector"""
 
     y: float = betterproto.float_field(2)
@@ -420,7 +405,24 @@
     point_cloud_alignment_changed: bool = betterproto.bool_field(12)
     """
     The point cloud alignment deviates from the reference alignment. This might
     have an impact on the point cloud processing as e.g. the ground alignment
     got incorrect. If this is expected, the alignment can be reconfigured with
     the Health.SetConfig API method.
     """
+
+
+@dataclass(eq=False, repr=False)
+class AccelerationBuffer(betterproto.Message):
+    """Buffer for multiple Acceleration samples"""
+
+    timestamp: int = betterproto.uint64_field(1)
+    """Timestamp of the first sample in the buffer."""
+
+    sampling_period: int = betterproto.uint64_field(2)
+    """Sampling period of the acceleration samples"""
+
+    cartesian: bytes = betterproto.bytes_field(3)
+    """
+    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
+    Type: Float32
+    """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/core_processing/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/core_processing/services/acceleration.proto, blickfeld/core_processing/services/distortion_correction.proto, blickfeld/core_processing/services/health.proto, blickfeld/core_processing/services/point_cloud.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -25,14 +27,64 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class PointCloudStreamRequest(betterproto.Message):
+    """Request for point cloud stream request"""
+
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudGetRequest(betterproto.Message):
+    """Request for point cloud get request"""
+
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudStreamResponse(betterproto.Message):
+    """Stream response to point cloud stream request"""
+
+    frame: "_data__.Frame" = betterproto.message_field(1)
+    """Point cloud frame"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudGetResponse(betterproto.Message):
+    """Response to point cloud get request"""
+
+    frame: "_data__.Frame" = betterproto.message_field(1)
+    """Point cloud frame"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudSetFilterRequest(betterproto.Message):
+    """Request for setting the filter configuration"""
+
+    filter: "_config__.PointCloudFilter" = betterproto.message_field(1)
+    """
+    Filter configuration which should be applied on the point cloud frames.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudGetFilterResponse(betterproto.Message):
+    """Response for retrieving the current filter configuration"""
+
+    filter: "_config__.PointCloudFilter" = betterproto.message_field(1)
+    """
+    Filter configuration which is currently applied on the point cloud frames.
+    """
+
+
+@dataclass(eq=False, repr=False)
 class AccelerationStreamResponse(betterproto.Message):
     """Stream response to acceleration stream request"""
 
     buffer: "_data__.AccelerationBuffer" = betterproto.message_field(1)
     """Buffer with acceleration"""
 
 
@@ -72,70 +124,208 @@
 class HealthGetConfigResponse(betterproto.Message):
     """Health get config response"""
 
     config: "_config__.Health" = betterproto.message_field(1)
     """Health parameters"""
 
 
-@dataclass(eq=False, repr=False)
-class PointCloudStreamRequest(betterproto.Message):
-    """Request for point cloud stream request"""
+class PointCloud(betterproto.ServiceStub):
+    """
+    Point Cloud service for core point cloud stream. It is the direct result of
+    the internal processing pipeline. The output is not post-processed further.
+    The post-processed output can be retrieved from the percept-processing
+    PointCloud service.
+    """
 
-    pass
+    async def async_stream(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
+        """
+        Stream a point cloud stream NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
+        request = PointCloudStreamRequest()
 
-@dataclass(eq=False, repr=False)
-class PointCloudGetRequest(betterproto.Message):
-    """Request for point cloud get request"""
+        async for response in self._unary_stream(
+            "/blickfeld.core_processing.services.PointCloud/Stream",
+            request,
+            PointCloudStreamResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
 
-    pass
+    def stream(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["PointCloudStreamResponse"]:
+        """
+        Stream a point cloud stream NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
+        loop = asyncio.get_event_loop()
+        ait = self.async_stream(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
 
-@dataclass(eq=False, repr=False)
-class PointCloudStreamResponse(betterproto.Message):
-    """Stream response to point cloud stream request"""
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
 
-    frame: "_data__.Frame" = betterproto.message_field(1)
-    """Point cloud frame"""
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PointCloudGetResponse":
+        """
+        Get a single point cloud NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
-@dataclass(eq=False, repr=False)
-class PointCloudGetResponse(betterproto.Message):
-    """Response to point cloud get request"""
+        request = PointCloudGetRequest()
 
-    frame: "_data__.Frame" = betterproto.message_field(1)
-    """Point cloud frame"""
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.PointCloud/Get",
+            request,
+            PointCloudGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PointCloudGetResponse":
+        """
+        Get a single point cloud NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
-@dataclass(eq=False, repr=False)
-class PointCloudEnableDemoRequest(betterproto.Message):
-    """Response to point cloud enable demo request"""
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-    recording: "_config__.DemoRecording" = betterproto.enum_field(1)
-    """Select demo recording"""
+    async def async_set_filter(
+        self,
+        *,
+        filter: "_config__.PointCloudFilter" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set the filter configuration which is to be applied on the point cloud
+        data
+        """
 
+        request = PointCloudSetFilterRequest()
+        if filter is not None:
+            request.filter = filter
 
-@dataclass(eq=False, repr=False)
-class PointCloudSetFilterRequest(betterproto.Message):
-    """Request for setting the filter configuration"""
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.PointCloud/SetFilter",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-    filter: "_config__.PointCloudFilter" = betterproto.message_field(1)
-    """
-    Filter configuration which should be applied on the point cloud frames.
-    """
+    def set_filter(
+        self,
+        *,
+        filter: "_config__.PointCloudFilter" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set the filter configuration which is to be applied on the point cloud
+        data
+        """
 
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_set_filter(
+                filter=filter,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-@dataclass(eq=False, repr=False)
-class PointCloudGetFilterResponse(betterproto.Message):
-    """Response for retrieving the current filter configuration"""
+    async def async_get_filter(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PointCloudGetFilterResponse":
+        """
+        Get the filter configuration which is currently applied on the point
+        cloud data
+        """
 
-    filter: "_config__.PointCloudFilter" = betterproto.message_field(1)
-    """
-    Filter configuration which is currently applied on the point cloud frames.
-    """
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.PointCloud/GetFilter",
+            request,
+            PointCloudGetFilterResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_filter(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PointCloudGetFilterResponse":
+        """
+        Get the filter configuration which is currently applied on the point
+        cloud data
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get_filter(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class DistortionCorrection(betterproto.ServiceStub):
     """
     Service interface for managing the point cloud distortion correction.
     """
 
@@ -505,245 +695,7 @@
         return loop.run_until_complete(
             self.async_get_config(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
-
-
-class PointCloud(betterproto.ServiceStub):
-    """
-    Point Cloud service for core point cloud stream. It is the direct result of
-    the internal processing pipeline. The output is not post-processed further.
-    The post-processed output can be retrieved from the percept-processing
-    PointCloud service.
-    """
-
-    async def async_stream(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
-        """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
-        """
-
-        request = PointCloudStreamRequest()
-
-        async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.PointCloud/Stream",
-            request,
-            PointCloudStreamResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def stream(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["PointCloudStreamResponse"]:
-        """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_stream(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
-        """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
-        """
-
-        request = PointCloudGetRequest()
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/Get",
-            request,
-            PointCloudGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
-        """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_enable_demo(
-        self,
-        *,
-        recording: "_config__.DemoRecording" = 0,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Enable demo data set It will be re-played on Stream requests"""
-
-        request = PointCloudEnableDemoRequest()
-        request.recording = recording
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/EnableDemo",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def enable_demo(
-        self,
-        *,
-        recording: "_config__.DemoRecording" = 0,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Enable demo data set It will be re-played on Stream requests"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_enable_demo(
-                recording=recording,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_set_filter(
-        self,
-        *,
-        filter: "_config__.PointCloudFilter" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set the filter configuration which is to be applied on the point cloud
-        data
-        """
-
-        request = PointCloudSetFilterRequest()
-        if filter is not None:
-            request.filter = filter
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/SetFilter",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def set_filter(
-        self,
-        *,
-        filter: "_config__.PointCloudFilter" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set the filter configuration which is to be applied on the point cloud
-        data
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_set_filter(
-                filter=filter,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_get_filter(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetFilterResponse":
-        """
-        Get the filter configuration which is currently applied on the point
-        cloud data
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/GetFilter",
-            request,
-            PointCloudGetFilterResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get_filter(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetFilterResponse":
-        """
-        Get the filter configuration which is currently applied on the point
-        cloud data
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_filter(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/detector/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/detector/data/health.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/detector/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/detector/services/health.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -26,23 +28,23 @@
 
 
 @dataclass(eq=False, repr=False)
 class HealthGetResponse(betterproto.Message):
     """Response message for get health request."""
 
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 @dataclass(eq=False, repr=False)
 class HealthWatchResponse(betterproto.Message):
     """Response message for watch health request."""
 
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 class Health(betterproto.ServiceStub):
     """
     The health service provides methods to monitor the instant operational
     status of the detector module
     """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/diagnostics/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,80 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/diagnostics/data/self_test_report.proto
+# sources: blickfeld/base/config/geolocation.proto, blickfeld/base/config/range.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
-from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
-from .. import config as _config__
 
+@dataclass(eq=False, repr=False)
+class Geolocation(betterproto.Message):
+    """
+    Geolocation in the geographic coordinate system. Is used to geo-reference
+    device coordinate systems and produced data.
+    """
 
-class SelfTestReportResultFlag(betterproto.Enum):
-    """Result flags which indicates if test was sucessful."""
+    latitude: float = betterproto.float_field(1)
+    """Latitude angle"""
 
-    FLAG_UNSPECIFIED = 0
-    """Unknown result."""
+    longitude: float = betterproto.float_field(2)
+    """Longitude angle"""
 
-    FLAG_SUCCESS = 1
-    """The test was successful."""
+    metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(100)
+    """Arbitrary metadata storage for client applications"""
 
-    FLAG_WARNING = 2
+
+@dataclass(eq=False, repr=False)
+class Range(betterproto.Message):
     """
-    The test suceeded but it raised some warnings. Please report if this
-    happens during production and the root-cause is unknown.
+    This section defines ranges for numerical types. They can be used to define
+    minimum and maximum values.
     """
 
-    FLAG_FAILURE = 3
-    """The test failed. The tested module is most probably not functional."""
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class SelfTestReport(betterproto.Message):
-    """Report which contains the results of the selected self tests."""
+class RangeUint32(betterproto.Message):
+    """An unsigned integer range"""
 
-    result_flag: "SelfTestReportResultFlag" = betterproto.enum_field(1)
-    """
-    Aggregated result flag which is FLAG_SUCCESS if all tests passed without
-    warnings
-    """
+    minimum: int = betterproto.uint32_field(1)
+    """An unsigned integer minimum value"""
 
-    results: List["SelfTestReportResult"] = betterproto.message_field(2)
-    """List of test results"""
+    maximum: int = betterproto.uint32_field(2)
+    """An unsigned integer maximum value"""
 
 
 @dataclass(eq=False, repr=False)
-class SelfTestReportResult(betterproto.Message):
-    """Result of test."""
+class RangeInt32(betterproto.Message):
+    """A signed integer range"""
 
-    test: "_config__.SelfTest" = betterproto.enum_field(1)
-    """Test case"""
+    minimum: int = betterproto.int32_field(1)
+    """A signed integer minimum value"""
 
-    identifier: str = betterproto.string_field(5)
-    """Unique identifier of test case"""
+    maximum: int = betterproto.int32_field(2)
+    """A signed integer maximum value"""
 
-    flag: "SelfTestReportResultFlag" = betterproto.enum_field(2)
-    """Flag which states test result"""
 
-    reason: str = betterproto.string_field(3)
-    """
-    Human-readable reason for test warning or failure. Is not set if test was
-    successful.
-    """
+@dataclass(eq=False, repr=False)
+class RangeFloat(betterproto.Message):
+    """A single precision float range"""
+
+    minimum: float = betterproto.float_field(1)
+    """A single precision float minimum"""
+
+    maximum: float = betterproto.float_field(2)
+    """A single precision float maximum"""
+
+
+@dataclass(eq=False, repr=False)
+class RangeDouble(betterproto.Message):
+    """A double precision float range"""
+
+    minimum: float = betterproto.double_field(1)
+    """A double precision float minimum"""
 
-    duration: float = betterproto.float_field(4)
-    """Duration of test run"""
+    maximum: float = betterproto.double_field(2)
+    """A double precision float maximum"""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/flow/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/flow/config/flow.proto, blickfeld/flow/config/node_red_json.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 @dataclass(eq=False, repr=False)
+class NodeRedJson(betterproto.Message):
+    """Simple container for the node red import / export format"""
+
+    nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(1)
+    """List of JSON nodes"""
+
+
+@dataclass(eq=False, repr=False)
 class Flow(betterproto.Message):
     """
     Blickfeld Flow configuration This container is used to control high-level
     attributes of NodeRed flows.
     """
 
     name: str = betterproto.string_field(1)
@@ -28,15 +38,7 @@
     """Is it a subflow?"""
 
     metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(5)
     """Other arbitrary metadata"""
 
     nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(6)
     """All nodes contained in the flow"""
-
-
-@dataclass(eq=False, repr=False)
-class NodeRedJson(betterproto.Message):
-    """Simple container for the node red import / export format"""
-
-    nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(1)
-    """List of JSON nodes"""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/flow/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,77 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/flow/services/credentials.proto, blickfeld/flow/services/flow.proto, blickfeld/flow/services/settings.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
+    AsyncIterator,
     Dict,
+    Iterator,
     List,
     Optional,
 )
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import grpclib
 from blickfeld_qb2.betterproto.grpc.grpclib_server import ServiceBase
 
+from ...config import data as __config_data__
 from .. import config as _config__
 
 
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class SettingsSetRequest(betterproto.Message):
+    """Settings set request"""
+
+    settings: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """
+    Settings which should be stored Generic JSON format which is defined by
+    NodeRed.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class SettingsGetResponse(betterproto.Message):
+    """Settings get request"""
+
+    settings: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """Current settings Generic JSON format which is defined by NodeRed."""
+
+
+@dataclass(eq=False, repr=False)
+class CredentialsSetRequest(betterproto.Message):
+    """Credentials set request"""
+
+    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """
+    Credentials which should be stored Generic JSON format which is defined by
+    NodeRed.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class CredentialsGetResponse(betterproto.Message):
+    """Credentails get response"""
+
+    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """Current credentials Generic JSON format which is defined by NodeRed."""
+
+
+@dataclass(eq=False, repr=False)
 class FlowGetRequest(betterproto.Message):
     """Flow get request"""
 
     id: str = betterproto.string_field(1)
     """Flow id"""
 
     as_node_red_json: bool = betterproto.bool_field(2)
@@ -81,14 +124,44 @@
     """Flow delete request"""
 
     id: str = betterproto.string_field(1)
     """Id of Blickfeld Flow"""
 
 
 @dataclass(eq=False, repr=False)
+class FlowWatchRequest(betterproto.Message):
+    """Flow watch request"""
+
+    as_node_red_json: bool = betterproto.bool_field(1)
+    """
+    If true, the request returns the NodeRed JSON format which can be directly
+    imported.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class FlowWatchResponse(betterproto.Message):
+    """Per change, a response is emitted"""
+
+    id: str = betterproto.string_field(1)
+    """Id of Blickfeld Flow"""
+
+    flow: "_config__.Flow" = betterproto.message_field(2, group="kind")
+    """Blickfeld Flow config with well-defined high-level attributes"""
+
+    node_red_json: "_config__.NodeRedJson" = betterproto.message_field(3, group="kind")
+    """
+    NodeRed JSON format which can be directly exported from NodeRED Admin UI
+    """
+
+    type: "__config_data__.WatchEventType" = betterproto.enum_field(4)
+    """Type of change"""
+
+
+@dataclass(eq=False, repr=False)
 class FlowStoreGlobalNodesRequest(betterproto.Message):
     """Flow store global nodes request"""
 
     node_red_json: "_config__.NodeRedJson" = betterproto.message_field(1)
     """NodeRed JSON format of all global configuration nodes"""
 
 
@@ -97,49 +170,215 @@
     """Flow get global nodes response"""
 
     node_red_json: "_config__.NodeRedJson" = betterproto.message_field(1)
     """NodeRed JSON format of all global configuration nodes"""
 
 
 @dataclass(eq=False, repr=False)
-class SettingsSetRequest(betterproto.Message):
-    """Settings set request"""
+class FlowWatchGlobalNodesResponse(betterproto.Message):
+    """Flow watch global nodes response"""
 
-    settings: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    node_red_json: "_config__.NodeRedJson" = betterproto.message_field(1)
+    """NodeRed JSON format of all global configuration nodes"""
+
+
+class Settings(betterproto.ServiceStub):
     """
-    Settings which should be stored Generic JSON format which is defined by
-    NodeRed.
+    Configuration service to store the NodeRed Settings. It is used to
+    implement the custom storage API: https://nodered.org/docs/api/storage/
     """
 
+    async def async_set(
+        self,
+        *,
+        settings: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set settings Used by https://nodered.org/docs/api/storage/methods/#stor
+        agesavesettingssettings
+        """
 
-@dataclass(eq=False, repr=False)
-class SettingsGetResponse(betterproto.Message):
-    """Settings get request"""
+        request = SettingsSetRequest()
+        if settings is not None:
+            request.settings = settings
 
-    settings: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
-    """Current settings Generic JSON format which is defined by NodeRed."""
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Settings/Set",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def set(
+        self,
+        *,
+        settings: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set settings Used by https://nodered.org/docs/api/storage/methods/#stor
+        agesavesettingssettings
+        """
 
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_set(
+                settings=settings,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-@dataclass(eq=False, repr=False)
-class CredentialsSetRequest(betterproto.Message):
-    """Credentials set request"""
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "SettingsGetResponse":
+        """
+        Get settings Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetsettings
+        """
 
-    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Settings/Get",
+            request,
+            SettingsGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "SettingsGetResponse":
+        """
+        Get settings Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetsettings
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+
+class Credentials(betterproto.ServiceStub):
     """
-    Credentials which should be stored Generic JSON format which is defined by
-    NodeRed.
+    Service to store the NodeRed credentials. It is used to implement the
+    custom storage API: https://nodered.org/docs/api/storage/
     """
 
+    async def async_set(
+        self,
+        *,
+        credentials: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
+        toragesavecredentialscredentials
+        """
 
-@dataclass(eq=False, repr=False)
-class CredentialsGetResponse(betterproto.Message):
-    """Credentails get response"""
+        request = CredentialsSetRequest()
+        if credentials is not None:
+            request.credentials = credentials
 
-    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
-    """Current credentials Generic JSON format which is defined by NodeRed."""
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Credentials/Set",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def set(
+        self,
+        *,
+        credentials: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
+        toragesavecredentialscredentials
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_set(
+                credentials=credentials,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "CredentialsGetResponse":
+        """
+        Get credentials Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Credentials/Get",
+            request,
+            CredentialsGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "CredentialsGetResponse":
+        """
+        Get credentials Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class Flow(betterproto.ServiceStub):
     """
     Service to store and control Blickfeld flows. It is used to implement the
     custom storage API: https://nodered.org/docs/api/storage/
     """
@@ -316,281 +555,175 @@
                 id=id,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_store_global_nodes(
+    async def async_watch(
         self,
         *,
-        node_red_json: "_config__.NodeRedJson" = None,
+        as_node_red_json: bool = False,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store global nodes"""
+    ) -> AsyncIterator["FlowWatchResponse"]:
+        """Watch flow changes"""
 
-        request = FlowStoreGlobalNodesRequest()
-        if node_red_json is not None:
-            request.node_red_json = node_red_json
+        request = FlowWatchRequest()
+        request.as_node_red_json = as_node_red_json
 
-        return await self._unary_unary(
-            "/blickfeld.flow.services.Flow/StoreGlobalNodes",
+        async for response in self._unary_stream(
+            "/blickfeld.flow.services.Flow/Watch",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            FlowWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    def store_global_nodes(
+    def watch(
         self,
         *,
-        node_red_json: "_config__.NodeRedJson" = None,
+        as_node_red_json: bool = False,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store global nodes"""
+    ) -> Iterator["FlowWatchResponse"]:
+        """Watch flow changes"""
 
         loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_store_global_nodes(
-                node_red_json=node_red_json,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_get_global_nodes(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FlowGetGlobalNodesResponse":
-        """Get global nodes"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.flow.services.Flow/GetGlobalNodes",
-            request,
-            FlowGetGlobalNodesResponse,
+        ait = self.async_watch(
+            as_node_red_json=as_node_red_json,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ).__aiter__()
 
-    def get_global_nodes(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FlowGetGlobalNodesResponse":
-        """Get global nodes"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_global_nodes(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class Settings(betterproto.ServiceStub):
-    """
-    Configuration service to store the NodeRed Settings. It is used to
-    implement the custom storage API: https://nodered.org/docs/api/storage/
-    """
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
-    async def async_set(
+    async def async_store_global_nodes(
         self,
         *,
-        settings: "betterproto_lib_google_protobuf.Struct" = None,
+        node_red_json: "_config__.NodeRedJson" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set settings Used by https://nodered.org/docs/api/storage/methods/#stor
-        agesavesettingssettings
-        """
+        """Store global nodes"""
 
-        request = SettingsSetRequest()
-        if settings is not None:
-            request.settings = settings
+        request = FlowStoreGlobalNodesRequest()
+        if node_red_json is not None:
+            request.node_red_json = node_red_json
 
         return await self._unary_unary(
-            "/blickfeld.flow.services.Settings/Set",
+            "/blickfeld.flow.services.Flow/StoreGlobalNodes",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set(
+    def store_global_nodes(
         self,
         *,
-        settings: "betterproto_lib_google_protobuf.Struct" = None,
+        node_red_json: "_config__.NodeRedJson" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set settings Used by https://nodered.org/docs/api/storage/methods/#stor
-        agesavesettingssettings
-        """
+        """Store global nodes"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                settings=settings,
+            self.async_store_global_nodes(
+                node_red_json=node_red_json,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get(
+    async def async_get_global_nodes(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "SettingsGetResponse":
-        """
-        Get settings Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetsettings
-        """
+    ) -> "FlowGetGlobalNodesResponse":
+        """Get global nodes"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.flow.services.Settings/Get",
+            "/blickfeld.flow.services.Flow/GetGlobalNodes",
             request,
-            SettingsGetResponse,
+            FlowGetGlobalNodesResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def get_global_nodes(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "SettingsGetResponse":
-        """
-        Get settings Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetsettings
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class Credentials(betterproto.ServiceStub):
-    """
-    Service to store the NodeRed credentials. It is used to implement the
-    custom storage API: https://nodered.org/docs/api/storage/
-    """
-
-    async def async_set(
-        self,
-        *,
-        credentials: "betterproto_lib_google_protobuf.Struct" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
-        toragesavecredentialscredentials
-        """
-
-        request = CredentialsSetRequest()
-        if credentials is not None:
-            request.credentials = credentials
-
-        return await self._unary_unary(
-            "/blickfeld.flow.services.Credentials/Set",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def set(
-        self,
-        *,
-        credentials: "betterproto_lib_google_protobuf.Struct" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
-        toragesavecredentialscredentials
-        """
+    ) -> "FlowGetGlobalNodesResponse":
+        """Get global nodes"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                credentials=credentials,
+            self.async_get_global_nodes(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get(
+    async def async_watch_global_nodes(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "CredentialsGetResponse":
-        """
-        Get credentials Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
-        """
+    ) -> "FlowWatchGlobalNodesResponse":
+        """Watch global nodes"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.flow.services.Credentials/Get",
+            "/blickfeld.flow.services.Flow/WatchGlobalNodes",
             request,
-            CredentialsGetResponse,
+            FlowWatchGlobalNodesResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def watch_global_nodes(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "CredentialsGetResponse":
-        """
-        Get credentials Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
-        """
+    ) -> "FlowWatchGlobalNodesResponse":
+        """Watch global nodes"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_watch_global_nodes(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/hardware/config/identification.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/hardware/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/hardware/services/compute_module.proto, blickfeld/hardware/services/device_operation.proto, blickfeld/hardware/services/identification.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -27,57 +29,14 @@
 class IdentificationGetResponse(betterproto.Message):
     """Response message for the identification get command"""
 
     identification: "_config__.Identification" = betterproto.message_field(1)
     """The current identification"""
 
 
-class Identification(betterproto.ServiceStub):
-    """
-    The identification service provides methods to set and read out
-    identification data of the Qb2 device.
-    """
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.hardware.services.Identification/Get",
-            request,
-            IdentificationGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
 class DeviceOperation(betterproto.ServiceStub):
     """
     This service is used for starting and stopping the device operation.
     Normally, the device is started and stopped based on the client
     connections. If there is a client using the Qb2, the device will start and
     stay in operation until all clients disconnected. The start function of
     this service overrides this behaviour, i.e. when started using the start
@@ -211,7 +170,50 @@
         return loop.run_until_complete(
             self.async_reboot(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
+
+
+class Identification(betterproto.ServiceStub):
+    """
+    The identification service provides methods to set and read out
+    identification data of the Qb2 device.
+    """
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.hardware.services.Identification/Get",
+            request,
+            IdentificationGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/laser/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/laser/data/health.proto
+# sources: blickfeld/percept_toolkit/data/health.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from ...base import data as __base_data__
 
 
 @dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
+    """A health message that contains information about the toolkit status."""
+
     state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module"""
+    """High-level state of module."""
 
     state_reason: str = betterproto.string_field(2)
-    """Reason for given state. Is not set if state is OK."""
+    """
+    Reason for the given state. Needs to be set if state is not STATE_OK.
+    """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/laser/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/laser/services/health.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -24,21 +26,21 @@
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
 class HealthGetResponse(betterproto.Message):
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 @dataclass(eq=False, repr=False)
 class HealthWatchResponse(betterproto.Message):
     health: "_data__.Health" = betterproto.message_field(1)
-    """Please refer to <<data.Health>>"""
+    """Health state"""
 
 
 class Health(betterproto.ServiceStub):
     """
     The health service provides methods to monitor the instant operational
     status of laser module
     """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,80 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/percept_pipeline/config/background_subtraction.proto, blickfeld/percept_pipeline/config/data_source.proto, blickfeld/percept_pipeline/config/perception.proto, blickfeld/percept_pipeline/config/point_cloud_filter.proto, blickfeld/percept_pipeline/config/zone_algorithm.proto
+# sources: blickfeld/percept_pipeline/config/background_subtraction.proto, blickfeld/percept_pipeline/config/clustering.proto, blickfeld/percept_pipeline/config/data_source.proto, blickfeld/percept_pipeline/config/object_size.proto, blickfeld/percept_pipeline/config/perception.proto, blickfeld/percept_pipeline/config/point_cloud_filter.proto, blickfeld/percept_pipeline/config/zone_algorithm.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
-from ...base import geometry as __base_geometry__
+from ...base import (
+    config as __base_config__,
+    geometry as __base_geometry__,
+)
+
+
+class ObjectSize(betterproto.Enum):
+    """The size of an object"""
+
+    OBJECT_SIZE_UNSPECIFIED = 0
+    """The zero value should not be used"""
+
+    OBJECT_SIZE_SMALL = 1
+    """Small object size: small animals, birds, etc"""
+
+    OBJECT_SIZE_MEDIUM = 2
+    """Medium object size: free standing human, single human, etc"""
+
+    OBJECT_SIZE_LARGE = 3
+    """Large object size: cars, group of people, large animals, etc"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudFilter(betterproto.Message):
+    """Algorithm for filtering point clouds"""
+
+    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
+        1, group="point_cloud_filter_type"
+    )
+    """Use radius outlier filter for noise reduction on point clouds"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudFilterRadiusOutlier(betterproto.Message):
+    """Filter points based on the number of neighbors in a certain radius"""
+
+    min_neighbor_points: int = betterproto.uint32_field(1)
+    """Minimum number of neighbors a point has to have to be retained"""
+
+    neighbor_radius: float = betterproto.double_field(2)
+    """All points within this radius are considered neighbors of a point"""
 
 
 @dataclass(eq=False, repr=False)
 class DataSource(betterproto.Message):
     """
     The configuration storing the sources to retrieve the point cloud data for
     further processing.
     """
 
-    cube1_setup: "DataSourceCube1Setup" = betterproto.message_field(
-        1, group="data_source_type"
-    )
-    """Use Cube 1 lidars to retrieve point clouds"""
-
     qb2_setup: "DataSourceQb2Setup" = betterproto.message_field(
         3, group="data_source_type"
     )
     """Use Qb2 lidars to retrieve point clouds"""
 
-
-@dataclass(eq=False, repr=False)
-class DataSourceCube1(betterproto.Message):
-    """Configuration for retrieving point clouds from a Cube 1"""
-
-    fqdn: str = betterproto.string_field(1)
-    """The fully qualified domain name of the Cube 1"""
-
-    map_from_lidar: "__base_geometry__.Transform" = betterproto.message_field(2)
+    geolocation_of_map: "__base_config__.Geolocation" = betterproto.message_field(4)
     """
-    Transformation from the lidar frame to the map frame. If this transform is
-    not set, this will be interpreted as identify transformation. Transforming
-    all point cloud topics into the map frame results in a globally consistent
-    combined point cloud in map frame.
+    Geolocation of data source. This references the map coordinate system of
+    this data source to the world. Individual lidars are referenced to the map
+    coordinate system via their `map_from_lidar` transform. [NOTE] If the
+    map_from_lidar transform is not an identity transformation, this is not the
+    geolocation of an individual sensor.
     """
 
 
 @dataclass(eq=False, repr=False)
 class DataSourceQb2(betterproto.Message):
     """Configuration for retrieving point clouds from a Qb2"""
 
@@ -59,31 +89,29 @@
     """
     Transformation from the lidar frame to the map frame. If this transform is
     not set, this will be interpreted as identify transformation. Transforming
     all point cloud topics into the map frame results in a globally consistent
     combined point cloud in map frame.
     """
 
+    application_key: str = betterproto.string_field(3)
+    """
+    Application key with authorized access level. Required if user-management
+    is enabled on externally connected devices.
+    """
 
-@dataclass(eq=False, repr=False)
-class DataSourceCube1Setup(betterproto.Message):
-    """The configuration of a Cube 1 setup of the LiDAR devices"""
-
-    lidars: List["DataSourceCube1"] = betterproto.message_field(1)
-    """Cube1 lidars to retrieve the point clouds from"""
-
-    enable_time_sync: bool = betterproto.bool_field(2)
+    serial_number: str = betterproto.string_field(4)
     """
-    If true: The same NTP server needs to be configured for each device before
-    starting. The lidar clock and and scan-patterns will be continously
-    synchronized. Recommended in multi-sensor setups. If false: the lidar
-    measurements are timestamps with the receive time by the system. The
-    receive time is less accurate if the network is not reliable.
+    Serial number. Required if user-management is enabled on externally
+    connected devices.
     """
 
+    metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(100)
+    """Arbitrary metadata storage for client applications"""
+
 
 @dataclass(eq=False, repr=False)
 class DataSourceTrigger(betterproto.Message):
     """
     Configuration of Trigger Mode. In trigger mode the processing pipeline will
     reduce the frequency at which point clouds and state lists are getting
     computed to reduce the amount of data transmitted between the processing
@@ -168,56 +196,70 @@
 
     num_initialization_frames: int = betterproto.uint32_field(1)
     """
     How many frames of the first received frames are used to build the
     background Reasonable default: 10
     """
 
-    octree_resolution: float = betterproto.float_field(2)
-    """
-    Resolution for the octree storing a static background. Reasonable default:
-    0.15
-    """
-
 
 @dataclass(eq=False, repr=False)
-class PointCloudFilter(betterproto.Message):
-    """Algorithm for filtering point clouds"""
+class Clustering(betterproto.Message):
+    """
+    Algorithms for detecting objects as clustered points in the foreground
+    scene.
+    """
 
-    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
-        1, group="point_cloud_filter_type"
-    )
-    """Use radius outlier filter for noise reduction on point clouds"""
+    db_scan: "ClusteringDbScan" = betterproto.message_field(1, group="clustering_type")
+    """Use db-scan for clustering the foreground"""
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudFilterRadiusOutlier(betterproto.Message):
-    """Filter points based on the number of neighbors in a certain radius"""
+class ClusteringDbScan(betterproto.Message):
+    """
+    Density-based spatial clustering algorithm using the euclidean distance
+    between points
+    """
 
-    min_neighbor_points: int = betterproto.uint32_field(1)
-    """Minimum number of neighbors a point has to have to be retained"""
+    min_points: int = betterproto.uint32_field(1)
+    """
+    Minimum amount of points required to define an object-cluster Reasonable
+    default: 10
+    """
 
-    neighbor_radius: float = betterproto.double_field(2)
-    """All points within this radius are considered neighbors of a point"""
+    radius: float = betterproto.float_field(2)
+    """
+    Controls how far away points belonging to the same object-cluster can be.
+    Reasonable default: 0.2
+    """
+
+    distance_dependent_radius: float = betterproto.float_field(3)
+    """
+    Multiply the given radius with the range of a point and add it to the
+    radius. This significantly improves the clustering for close-range scenes.
+    Reasonable default: 0.025
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Perception(betterproto.Message):
     """
     The configuration of perception algorithms used to run e.g. security zones
     """
 
     background_subtraction: "BackgroundSubtraction" = betterproto.message_field(1)
     """Extract the foreground point cloud of the scene"""
 
-    foreground_point_cloud_filters: List[
-        "PointCloudFilter"
-    ] = betterproto.message_field(2)
+    foreground_point_cloud_filters: List["PointCloudFilter"] = (
+        betterproto.message_field(2)
+    )
     """Filter the foreground point cloud"""
 
+    clustering: "Clustering" = betterproto.message_field(8)
+    """Segment the foreground point cloud into clusters"""
+
 
 @dataclass(eq=False, repr=False)
 class ZoneAlgorithm(betterproto.Message):
     """An algorithm that monitors the area within and around a zone."""
 
     name: str = betterproto.string_field(1)
     """The user readable zone algorithm name"""
@@ -227,22 +269,35 @@
 
     shape: "__base_geometry__.Shape" = betterproto.message_field(3)
     """
     Geometric shape (usually a Box) in which the algorithm detects certain
     behaviors/scenarios
     """
 
+    metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(100)
+    """Arbitrary metadata storage for client applications"""
+
     volume: "ZoneAlgorithmVolume" = betterproto.message_field(9, group="algorithm_type")
     """Run volume monitoring within the zone"""
 
     security: "ZoneAlgorithmSecurity" = betterproto.message_field(
         7, group="algorithm_type"
     )
     """Run alarm detection within the zone"""
 
+    exclusion: "ZoneAlgorithmExclusion" = betterproto.message_field(
+        10, group="algorithm_type"
+    )
+    """Run exclusion zone"""
+
+    object_based_security: "ZoneAlgorithmObjectBasedSecurity" = (
+        betterproto.message_field(11, group="algorithm_type")
+    )
+    """Run object-based alarm detection within the zone"""
+
 
 @dataclass(eq=False, repr=False)
 class ZoneAlgorithmVolume(betterproto.Message):
     """
     Algorithm that measure the volume of a zone The volume of a zone is
     approximated by computing a 'volume map' from the input point clouds. The
     volume map discretize the zone into 'tiles' in the xy-plane with a side-
@@ -272,7 +327,35 @@
     """
 
     min_points: int = betterproto.uint32_field(1)
     """
     Minimum number of (foreground) points in the security zone to trigger the
     alarm. Reasonable default: 10
     """
+
+    max_points: int = betterproto.uint32_field(2)
+    """
+    Maximum number of (foreground) points in the security zone that still
+    triggers an alarm. More points will disable the alarm. This logic can be
+    disabled by setting max_points to '0'. Default: 0
+    """
+
+
+@dataclass(eq=False, repr=False)
+class ZoneAlgorithmObjectBasedSecurity(betterproto.Message):
+    """
+    Algorithm that triggers an alarm when an object of one of the selected
+    sizes is in the zone
+    """
+
+    alarm_sizes: List["ObjectSize"] = betterproto.enum_field(1)
+    """
+    Selection of sizes which trigger an alarm. Each size in the array will only
+    trigger an alarm for the interval of that size.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class ZoneAlgorithmExclusion(betterproto.Message):
+    """Algorithm that excludes points from the input point cloud"""
+
+    pass
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/percept_pipeline/data/coordinate_system.proto, blickfeld/percept_pipeline/data/health.proto, blickfeld/percept_pipeline/data/point_cloud_type.proto, blickfeld/percept_pipeline/data/state.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
@@ -26,14 +28,32 @@
 
     POINT_CLOUD_TYPE_FULL_OPTIMIZED = 3
     """
     Same as 'POINT_CLOUD_TYPE_FULL' but with reduced point cloud density to
     reduce the size of the point cloud
     """
 
+    POINT_CLOUD_TYPE_FILTERED = 4
+    """
+    Same as 'POINT_CLOUD_TYPE_FULL' but with all points excluded that are in
+    exclusion zones
+    """
+
+    POINT_CLOUD_TYPE_FILTERED_FOREGROUND = 5
+    """
+    Same as 'POINT_CLOUD_TYPE_FOREGROUND' but with all points excluded that are
+    in exclusion zones
+    """
+
+    POINT_CLOUD_TYPE_BACKGROUND = 6
+    """
+    Point cloud containing the points representing the background model/point
+    cloud
+    """
+
 
 class State(betterproto.Enum):
     """The states of pipeline"""
 
     STATE_UNSPECIFIED = 0
     """State field is not set"""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_pipeline/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/percept_pipeline/services/data_source.proto, blickfeld/percept_pipeline/services/health.proto, blickfeld/percept_pipeline/services/perception.proto, blickfeld/percept_pipeline/services/zone.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -26,14 +28,70 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class ZoneListResponse(betterproto.Message):
+    """Response containing the configured list of zones"""
+
+    zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
+    """The currently configured zones"""
+
+
+@dataclass(eq=False, repr=False)
+class ZoneStoreRequest(betterproto.Message):
+    """Request to store or update an existing zone"""
+
+    zone: "_config__.ZoneAlgorithm" = betterproto.message_field(1)
+    """
+    The new zone to be added. If there is a zone with the same uuid, that zone
+    will get updated with this configuration.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class ZoneDeleteRequest(betterproto.Message):
+    """Request to delete a zone"""
+
+    uuid: str = betterproto.string_field(1)
+    """The uuid of the zone to be deleted"""
+
+
+@dataclass(eq=False, repr=False)
+class ZoneWatchResponse(betterproto.Message):
+    """Continuous response on zone list changes"""
+
+    zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
+    """The current/updated list of zones"""
+
+
+@dataclass(eq=False, repr=False)
+class ZoneGetTareVolumeRequest(betterproto.Message):
+    """Request for the raw volume to be used for taring a volume zone"""
+
+    zone_uuid: str = betterproto.string_field(1)
+    """The uuid of the volume zone"""
+
+
+@dataclass(eq=False, repr=False)
+class ZoneGetTareVolumeResponse(betterproto.Message):
+    """Response containing the raw volume of the requested zone"""
+
+    tare_volume: float = betterproto.float_field(1)
+    """
+    The raw volume of the volume zone without any offsets/modifications. The
+    value is supposed to be configured as 'empty_volume' value of a volume
+    zone. As a result the current volume of the zone will be '0' until more
+    volume is added.
+    """
+
+
+@dataclass(eq=False, repr=False)
 class DataSourceGetResponse(betterproto.Message):
     """Response containing the current data source"""
 
     data_source: "_config__.DataSource" = betterproto.message_field(1)
     """The currently set data source"""
 
 
@@ -122,68 +180,230 @@
     """
     If the list is empty, the background models of all data sources are reset.
     If the background models of only specific devices should be rebuilt, the
     'fqdn' of the respective devices has to be mentioned in the 'fqdns' list.
     """
 
 
-@dataclass(eq=False, repr=False)
-class ZoneListResponse(betterproto.Message):
-    """Response containing the configured list of zones"""
+class Zone(betterproto.ServiceStub):
+    """
+    The zone service allows getting, configuring, deleting and receiving
+    updates of the configured zones.
+    """
 
-    zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
-    """The currently configured zones"""
+    async def async_list(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "ZoneListResponse":
+        """Returns the configured zones"""
 
+        request = betterproto_lib_google_protobuf.Empty()
 
-@dataclass(eq=False, repr=False)
-class ZoneStoreRequest(betterproto.Message):
-    """Request to store or update an existing zone"""
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Zone/List",
+            request,
+            ZoneListResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-    zone: "_config__.ZoneAlgorithm" = betterproto.message_field(1)
-    """
-    The new zone to be added. If there is a zone with the same uuid, that zone
-    will get updated with this configuration.
-    """
+    def list(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "ZoneListResponse":
+        """Returns the configured zones"""
 
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_list(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-@dataclass(eq=False, repr=False)
-class ZoneDeleteRequest(betterproto.Message):
-    """Request to delete a zone"""
+    async def async_store(
+        self,
+        *,
+        zone: "_config__.ZoneAlgorithm" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Store / Update a zone"""
 
-    uuid: str = betterproto.string_field(1)
-    """The uuid of the zone to be deleted"""
+        request = ZoneStoreRequest()
+        if zone is not None:
+            request.zone = zone
 
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Zone/Store",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-@dataclass(eq=False, repr=False)
-class ZoneWatchResponse(betterproto.Message):
-    """Continuous response on zone list changes"""
+    def store(
+        self,
+        *,
+        zone: "_config__.ZoneAlgorithm" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Store / Update a zone"""
 
-    zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
-    """The current/updated list of zones"""
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_store(
+                zone=zone,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
+    async def async_delete(
+        self,
+        *,
+        uuid: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Delete a zone"""
 
-@dataclass(eq=False, repr=False)
-class ZoneGetTareVolumeRequest(betterproto.Message):
-    """Request for the raw volume to be used for taring a volume zone"""
+        request = ZoneDeleteRequest()
+        request.uuid = uuid
 
-    zone_uuid: str = betterproto.string_field(1)
-    """The uuid of the volume zone"""
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Zone/Delete",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
+    def delete(
+        self,
+        *,
+        uuid: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Delete a zone"""
 
-@dataclass(eq=False, repr=False)
-class ZoneGetTareVolumeResponse(betterproto.Message):
-    """Response containing the raw volume of the requested zone"""
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_delete(
+                uuid=uuid,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-    tare_volume: float = betterproto.float_field(1)
-    """
-    The raw volume of the volume zone without any offsets/modifications. The
-    value is supposed to be configured as 'empty_volume' value of a volume
-    zone. As a result the current volume of the zone will be '0' until more
-    volume is added.
-    """
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["ZoneWatchResponse"]:
+        """Watch configuration for zone list"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.percept_pipeline.services.Zone/Watch",
+            request,
+            ZoneWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["ZoneWatchResponse"]:
+        """Watch configuration for zone list"""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_get_tare_volume(
+        self,
+        *,
+        zone_uuid: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ZoneGetTareVolumeResponse":
+        """Computes raw volume within a volume zone without any offsets."""
+
+        request = ZoneGetTareVolumeRequest()
+        request.zone_uuid = zone_uuid
+
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Zone/GetTareVolume",
+            request,
+            ZoneGetTareVolumeResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_tare_volume(
+        self,
+        *,
+        zone_uuid: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ZoneGetTareVolumeResponse":
+        """Computes raw volume within a volume zone without any offsets."""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get_tare_volume(
+                zone_uuid=zone_uuid,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class DataSource(betterproto.ServiceStub):
     """
     The data source service allows getting, configuring and receiving updates
     of the data source used for processing pipelines. The data source
     configuration specifies where to retrieve the point cloud data for further
@@ -265,14 +485,50 @@
                 data_source=data_source,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
+    async def async_reset(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Resets the data_source configuration to factory values"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.DataSource/Reset",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def reset(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Resets the data_source configuration to factory values"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_reset(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
     async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> AsyncIterator["DataSourceWatchResponse"]:
         """Watch configuration for data_source"""
@@ -625,225 +881,7 @@
             self.async_reset_background(
                 fqdns=fqdns,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
-
-
-class Zone(betterproto.ServiceStub):
-    """
-    The zone service allows getting, configuring, deleting and receiving
-    updates of the configured zones.
-    """
-
-    async def async_list(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "ZoneListResponse":
-        """Returns the configured zones"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/List",
-            request,
-            ZoneListResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def list(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "ZoneListResponse":
-        """Returns the configured zones"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_list(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_store(
-        self,
-        *,
-        zone: "_config__.ZoneAlgorithm" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store / Update a zone"""
-
-        request = ZoneStoreRequest()
-        if zone is not None:
-            request.zone = zone
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/Store",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def store(
-        self,
-        *,
-        zone: "_config__.ZoneAlgorithm" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store / Update a zone"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_store(
-                zone=zone,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_delete(
-        self,
-        *,
-        uuid: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete a zone"""
-
-        request = ZoneDeleteRequest()
-        request.uuid = uuid
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/Delete",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def delete(
-        self,
-        *,
-        uuid: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete a zone"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_delete(
-                uuid=uuid,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["ZoneWatchResponse"]:
-        """Watch configuration for zone list"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.Zone/Watch",
-            request,
-            ZoneWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["ZoneWatchResponse"]:
-        """Watch configuration for zone list"""
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get_tare_volume(
-        self,
-        *,
-        zone_uuid: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "ZoneGetTareVolumeResponse":
-        """Computes raw volume within a volume zone without any offsets."""
-
-        request = ZoneGetTareVolumeRequest()
-        request.zone_uuid = zone_uuid
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/GetTareVolume",
-            request,
-            ZoneGetTareVolumeResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get_tare_volume(
-        self,
-        *,
-        zone_uuid: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "ZoneGetTareVolumeResponse":
-        """Computes raw volume within a volume zone without any offsets."""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_tare_volume(
-                zone_uuid=zone_uuid,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,220 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/percept_processing/data/data_type.proto, blickfeld/percept_processing/data/health.proto, blickfeld/percept_processing/data/state.proto, blickfeld/percept_processing/data/states.proto, blickfeld/percept_processing/data/volume_map.proto
+# sources: blickfeld/diagnostics/data/health.proto, blickfeld/diagnostics/data/log.proto, blickfeld/diagnostics/data/self_test_report.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
-from typing import Dict
+from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
-import numpy as np
 
-from ...base import (
-    data as __base_data__,
-    geometry as __base_geometry__,
-)
-from ...percept_pipeline import data as __percept_pipeline_data__
+from ...base import data as __base_data__
+from .. import config as _config__
+
 
+class SelfTestReportResultFlag(betterproto.Enum):
+    """Result flags which indicate if test was successful."""
 
-class DataType(betterproto.Enum):
-    """The type of data that the stream contains"""
+    FLAG_UNSPECIFIED = 0
+    """Unknown result."""
 
-    DATA_TYPE_UNSPECIFIED = 0
-    """The zero value should not be used"""
+    FLAG_SUCCESS = 1
+    """The test was successful."""
 
-    DATA_TYPE_HEALTH = 1
+    FLAG_WARNING = 2
     """
-    Health data type: this contains information about the health of the
-    pipeline and of the module
+    The test succeeded but it raised some warnings. Please report if this
+    happens during production and the root-cause is unknown.
     """
 
-    DATA_TYPE_POINT_CLOUD = 2
-    """Point cloud data type: a complete point cloud message is streamed"""
+    FLAG_FAILURE = 3
+    """The test failed. The tested module is most probably not functional."""
+
+
+class LogEntryLevel(betterproto.Enum):
+    """The log level represents the priority of the log."""
+
+    LEVEL_UNSPECIFIED = 0
+    """No level is set"""
 
-    DATA_TYPE_STATES = 5
+    LEVEL_ERROR = 1
     """
-    States data type: a map of states generated by the system as configured in
-    the pipeline
+    An error condition was detected Includes the systemd levels: EMERGENCY,
+    ALERT, CRITICAL, ERROR
     """
 
-    DATA_TYPE_VOLUME_MAP = 6
+    LEVEL_WARNING = 2
     """
-    Volume map data type: a volume map generated by one volume zone configured
-    in the pipeline
+    The message indicates that an error will occur if no action is taken
+    Includes the systemd levels: NOTICE, WARNING
+    """
+
+    LEVEL_INFO = 3
+    """
+    Normal operational messages that require no action Includes the systemd
+    levels: INFORMATIONAL
     """
 
 
 @dataclass(eq=False, repr=False)
-class State(betterproto.Message):
+class Health(betterproto.Message):
+    """Qb2 modules"""
+
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
     """
-    A state transmits high-level information about the scene or setup. The
-    information it contains depends on the configuration. States will get
-    calculated on every frame of measurement.
+    High-level aggregated health state of the device (if one of the modules
+    reports FAILED -> aggregated state is also FAILED)
     """
 
-    generator_name: str = betterproto.string_field(8)
-    """The name of the entity generating this state"""
-
-    security: "StateSecurity" = betterproto.message_field(5, group="state_type")
-    """The security state contains intrusion information of a zone"""
+    state_reason: str = betterproto.string_field(2)
+    """
+    Reason for given state (user-friendly). Is not set if state is STATE_OK.
+    Aggregated string from modules state reasons
+    """
 
-    volume: "StateVolume" = betterproto.message_field(7, group="state_type")
-    """Current volume measured in the selected zone"""
+    module: "HealthModule" = betterproto.message_field(3)
+    """Qb2 modules"""
 
 
 @dataclass(eq=False, repr=False)
-class StateSecurity(betterproto.Message):
-    """A message containing an alarm state of a zone."""
+class HealthModule(betterproto.Message):
+    """Qb2 modules"""
+
+    laser: "HealthModuleHealth" = betterproto.message_field(1)
+    """health of laser module"""
+
+    detector: "HealthModuleHealth" = betterproto.message_field(2)
+    """health of detector module"""
+
+    beam_deflection_control_vertical: "HealthModuleHealth" = betterproto.message_field(
+        3
+    )
+    """health of beam deflection control module (vertical)"""
+
+    beam_deflection_control_horizontal: "HealthModuleHealth" = (
+        betterproto.message_field(4)
+    )
+    """health of beam deflection control module (horizontal)"""
+
+    system: "HealthModuleHealth" = betterproto.message_field(6)
+    """health of the Blickfeld system module"""
 
-    alarm: bool = betterproto.bool_field(1)
-    """If there is an alarm or not in the zone"""
+    core_processing: "HealthModuleHealth" = betterproto.message_field(7)
+    """health of the Blickfeld core processing module"""
 
-    num_detected_points: int = betterproto.uint32_field(2)
-    """The current number of lidar points detected in the zone"""
+    percept_processing: "HealthModuleHealth" = betterproto.message_field(8)
+    """health of percept processing"""
+
+    percept_pipeline: "HealthModuleHealth" = betterproto.message_field(9)
+    """health of percept pipeline"""
+
+    push: "HealthModuleHealth" = betterproto.message_field(10)
+    """Health of the Blickfeld Push module"""
+
+    secure: "HealthModuleHealth" = betterproto.message_field(11)
+    """Health of the Blickfeld Secure module"""
 
 
 @dataclass(eq=False, repr=False)
-class StateVolume(betterproto.Message):
+class HealthModuleHealth(betterproto.Message):
+    """Message representing health of a Qb2 module"""
+
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
+    """High-level health state of the module"""
+
+    state_reason: str = betterproto.string_field(2)
     """
-    A message containing the volume state of a zone. This is based on one
-    volume zone.
+    Reason for given state (user-friendly). Is not set if state is STATE_OK.
     """
 
-    volume: float = betterproto.float_field(1)
-    """The current numerical volume of the zone."""
-
 
 @dataclass(eq=False, repr=False)
-class States(betterproto.Message):
+class SelfTestReport(betterproto.Message):
+    """Report which contains the results of the selected self tests."""
+
+    result_flag: "SelfTestReportResultFlag" = betterproto.enum_field(1)
     """
-    A message that contains a map of states. A state is an information
-    generated by the system based on the select zone type or device. For
-    example, a state can contain information about the volume or the intrusion
-    in the zone.
+    Aggregated result flag which is FLAG_SUCCESS if all tests passed without
+    warnings
     """
 
-    timestamp: int = betterproto.uint64_field(1)
-    """The timestamp of the measurement(s) used to compute the states."""
-
-    states: Dict[str, "State"] = betterproto.map_field(
-        2, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-    """Map of states where the key is the generator UUID of the state."""
+    results: List["SelfTestReportResult"] = betterproto.message_field(2)
+    """List of test results"""
 
 
 @dataclass(eq=False, repr=False)
-class VolumeMap(betterproto.Message):
-    """A message containing the volume map of one volume zone."""
+class SelfTestReportResult(betterproto.Message):
+    """Result of test."""
 
-    timestamp: int = betterproto.uint64_field(1)
-    """Timestamp of the lidar frame in which the volume map was calculated"""
+    test: "_config__.SelfTest" = betterproto.enum_field(1)
+    """Test case"""
 
-    generator_uuid: str = betterproto.string_field(2)
-    """The uuid of the entity generating this state"""
+    identifier: str = betterproto.string_field(5)
+    """Unique identifier of test case"""
 
-    generator_name: str = betterproto.string_field(3)
-    """The name of the entity generating this state"""
+    flag: "SelfTestReportResultFlag" = betterproto.enum_field(2)
+    """Flag which states test result"""
 
-    shape: "__base_geometry__.Shape" = betterproto.message_field(4)
+    reason: str = betterproto.string_field(3)
     """
-    The shape of the volume map, defining the pose and the dimension of the
-    volume map in world frame. The shape is similar to the shape of the input
-    zone with the following difference: - shape.pose.position:
-    (x=zone.pose.position.x, y=zone.pose.position.y, z=0) -
-    shape.pose.rotation: (roll=0, pitch=0, yaw=zone.pose.rotation.yaw) -
-    shape.box.dimension: (x=zone.box.dimension.x, y=zone.box.dimension.y,z=0)
+    Human-readable reason for test warning or failure. Is not set if test was
+    successful.
     """
 
-    tiles: "VolumeMapTiles" = betterproto.message_field(5)
-    """
-    Volume map 'tiles' as defined in Tiles, providing information for each tile
-    in the volume map.
-    """
+    duration: float = betterproto.float_field(4)
+    """Duration of test run"""
+
 
-    tile_size: float = betterproto.float_field(6)
+@dataclass(eq=False, repr=False)
+class Log(betterproto.Message):
     """
-    The tile size of the volume map (dimension of one tile in x and y
-    direction)
+    This message aggregates the data structures related to the log service.
     """
 
-    volume: float = betterproto.float_field(7)
-    """The current volume of the zone"""
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class VolumeMapTiles(betterproto.Message):
-    """Tiles of the volume map"""
+class LogEntry(betterproto.Message):
+    """The log entry contains the message and metadata of a log."""
+
+    boot_uuid: str = betterproto.string_field(1)
+    """UUID of the boot during which the log was written."""
 
-    length: int = betterproto.uint32_field(1)
-    """Number of tiles"""
+    cursor: "LogEntryCursor" = betterproto.message_field(2)
+    """Cursor used to index log entries and to navigate through the logs."""
 
-    index: np.ndarray = betterproto.bytes_field(2, numpy_dtype="(2,)<i2")
+    timestamp: int = betterproto.uint64_field(3)
     """
-    Volume Map Tile Index X (Int16) and Y (Int16) (can be negative and
-    positive) The indices of Volume Tiles are expressed w.r.t the Volume Map
-    coordinate system. The tile with index (0,0) will contain the points from
-    [0, tile_size), [0, tile_size). That means that (0,0,0) of the Volume Map
-    frame does not coincide with the center of the tile with index (0,0) but
-    with the crossing of the 4 tiles [(0,0), (0, -1,), (-1,-1), (-1,0)]. Type:
-    (Int16, Int16)
+    The wallclock time at the point in time the entry was received by the
+    journal, in nanoseconds since the epoch UTC.
     """
 
-    height: np.ndarray = betterproto.bytes_field(3, numpy_dtype="<f4")
-    """Height per tile, ordered ascending Type: Float32"""
+    module: "_config__.LogFilterSoftwareModule" = betterproto.enum_field(4)
+    """The module which has written the log."""
 
-    std_deviation: np.ndarray = betterproto.bytes_field(4, numpy_dtype="<f4")
-    """Standard Deviation per tile Type: Float32"""
+    level: "LogEntryLevel" = betterproto.enum_field(5)
+    """The log level of the log."""
 
-    number_points: np.ndarray = betterproto.bytes_field(5, numpy_dtype="<u2")
-    """Number Points per tile Type: UInt16"""
+    message: str = betterproto.string_field(6)
+    """The message which has been logged."""
 
 
 @dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
+class LogEntryCursor(betterproto.Message):
+    """The cursor uniquely identifies a log entry in the logs."""
+
+    sequence_number_id: str = betterproto.string_field(1)
     """
-    A health message that contains information about the pipeline status and
-    the module itself.
+    The sequence number ID is used to reference a set of log entries generated
+    by the same systemd-journald instance.
     """
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module."""
-
-    state_reason: str = betterproto.string_field(2)
-    """Reason for the given state. It is not set if state is STATE_OK."""
-
-    pipeline_state: "__percept_pipeline_data__.State" = betterproto.enum_field(4)
+    sequence_number: int = betterproto.uint64_field(2)
     """
-    Current state of the pipeline. It indicates if the pipeline is stable,
-    unstable or broken, based on the frequency of the data that is processed
-    and published.
+    The sequence number is assigned to a log entry by the systemd-journald
+    instance when they are written to disk. Every instance numbers their
+    entries sequentially, starting from 1 for the first entry written after
+    subsystem initialization.
     """
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_processing/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/percept_processing/services/health.proto, blickfeld/percept_processing/services/pipeline.proto, blickfeld/percept_processing/services/point_cloud.proto, blickfeld/percept_processing/services/states.proto, blickfeld/percept_processing/services/volume_map.proto
+# sources: blickfeld/percept_processing/services/health.proto, blickfeld/percept_processing/services/objects.proto, blickfeld/percept_processing/services/pipeline.proto, blickfeld/percept_processing/services/point_cloud.proto, blickfeld/percept_processing/services/states.proto, blickfeld/percept_processing/services/volume_map.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
     Dict,
@@ -13,37 +15,27 @@
 )
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import grpclib
 from blickfeld_qb2.betterproto.grpc.grpclib_server import ServiceBase
 
+from ...base import geometry as __base_geometry__
 from ...core_processing import data as __core_processing_data__
 from ...percept_pipeline import data as __percept_pipeline_data__
 from .. import data as _data__
 
 
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class StatesStreamResponse(betterproto.Message):
-    """
-    A response for getting a stream of states messages from the running
-    pipeline
-    """
-
-    states: "_data__.States" = betterproto.message_field(1)
-    """The current states with the information detected in the scene."""
-
-
-@dataclass(eq=False, repr=False)
 class VolumeMapStreamRequest(betterproto.Message):
     """A request to receive a stream of state list messages"""
 
     zone_uuid: str = betterproto.string_field(2)
     """Volume zone uuid"""
 
 
@@ -84,36 +76,14 @@
     """
 
     data_types: List["_data__.DataType"] = betterproto.enum_field(1)
     """A list of the data types available for streaming"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """
-    A response for getting a stream of health messages about the pipeline
-    """
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """
-    The current health message with information about the state of the pipeline
-    """
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """A response for getting an health message about the pipeline"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """
-    The current health message with information about the state of the pipeline
-    """
-
-
-@dataclass(eq=False, repr=False)
 class PointCloudStreamRequest(betterproto.Message):
     """
     A request to receive a stream of point cloud messages. Different point
     clouds can be streamed depending on the set fields: - combined point cloud
     (the full point cloud of all the available devices combined) in the map
     coordinate system - the foreground of the combined point cloud in the map
     coordinate system - the complete raw point cloud coming from one device,
@@ -132,79 +102,68 @@
     The coordinate system the point cloud should be expressed in (local or
     transformed/map)
     """
 
     fqdn: str = betterproto.string_field(3, group="point_cloud_source")
     """fqdn of the data source to get the point cloud from"""
 
+    crop: "__base_geometry__.Shape" = betterproto.message_field(5)
+    """If set, point cloud is cropped to given shape"""
+
 
 @dataclass(eq=False, repr=False)
 class PointCloudStreamResponse(betterproto.Message):
     """A response for getting a stream of point cloud messages"""
 
     point_cloud: "__core_processing_data__.Frame" = betterproto.message_field(1)
     """The required point cloud, based on the fields set in the request"""
 
 
-class States(betterproto.ServiceStub):
+@dataclass(eq=False, repr=False)
+class ObjectsStreamResponse(betterproto.Message):
     """
-    An RPC service to request a stream of states messages. If a pipeline is
-    already running, it will be used to stream the data. If no pipeline is
-    running, it will be started first and then the stream will start. NOTE: in
-    this second case, the pipeline will also be automatically stopped once
-    there are no more clients requesting any stream type from the module.
+    A response for getting a stream of objects messages from the running
+    pipeline
     """
 
-    async def async_stream(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["StatesStreamResponse"]:
-        """A method to get a stream of states messages from the pipeline"""
+    objects: "_data__.Objects" = betterproto.message_field(1)
+    """The current objects detected in the scene."""
 
-        request = betterproto_lib_google_protobuf.Empty()
 
-        async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.States/Stream",
-            request,
-            StatesStreamResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """
+    A response for getting a stream of health messages about the pipeline
+    """
 
-    def stream(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["StatesStreamResponse"]:
-        """A method to get a stream of states messages from the pipeline"""
+    health: "_data__.Health" = betterproto.message_field(1)
+    """
+    The current health message with information about the state of the pipeline
+    """
 
-        loop = asyncio.get_event_loop()
-        ait = self.async_stream(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
 
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """A response for getting an health message about the pipeline"""
 
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+    health: "_data__.Health" = betterproto.message_field(1)
+    """
+    The current health message with information about the state of the pipeline
+    """
+
+
+@dataclass(eq=False, repr=False)
+class StatesStreamResponse(betterproto.Message):
+    """
+    A response for getting a stream of states messages from the running
+    pipeline
+    """
+
+    states: "_data__.States" = betterproto.message_field(1)
+    """The current states with the information detected in the scene."""
 
 
 class VolumeMap(betterproto.ServiceStub):
     """An RPC service to request a stream of volume map messages."""
 
     async def async_stream(
         self,
@@ -400,14 +359,158 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
+class PointCloud(betterproto.ServiceStub):
+    """
+    An RPC service to request a stream of point cloud messages. If a pipeline
+    is already running, it will be used to stream the data. If no pipeline is
+    running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once the
+    this second case, the pipeline will also be automatically stopped once
+    there are no more clients requesting any stream type from the module.
+    """
+
+    async def async_stream(
+        self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
+        crop: "__base_geometry__.Shape" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
+
+        request = PointCloudStreamRequest()
+        request.point_cloud_type = point_cloud_type
+        request.coordinate_system = coordinate_system
+        request.fqdn = fqdn
+        if crop is not None:
+            request.crop = crop
+
+        async for response in self._unary_stream(
+            "/blickfeld.percept_processing.services.PointCloud/Stream",
+            request,
+            PointCloudStreamResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def stream(
+        self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
+        crop: "__base_geometry__.Shape" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> Iterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_stream(
+            point_cloud_type=point_cloud_type,
+            coordinate_system=coordinate_system,
+            fqdn=fqdn,
+            crop=crop,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
+class Objects(betterproto.ServiceStub):
+    """
+    An RPC service to request a stream of objects messages. If a pipeline is
+    already running, it will be used to stream the data. If no pipeline is
+    running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once
+    there are no more clients requesting any stream type from the module.
+    """
+
+    async def async_stream(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["ObjectsStreamResponse"]:
+        """A method to get a stream of objects messages from the pipeline"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.percept_processing.services.Objects/Stream",
+            request,
+            ObjectsStreamResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def stream(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["ObjectsStreamResponse"]:
+        """A method to get a stream of objects messages from the pipeline"""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_stream(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
 class Health(betterproto.ServiceStub):
     """
     An RPC service to request information about the state of the pipeline and
     of the module.
     """
 
     async def async_watch(
@@ -503,76 +606,53 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class PointCloud(betterproto.ServiceStub):
+class States(betterproto.ServiceStub):
     """
-    An RPC service to request a stream of point cloud messages. If a pipeline
-    is already running, it will be used to stream the data. If no pipeline is
+    An RPC service to request a stream of states messages. If a pipeline is
+    already running, it will be used to stream the data. If no pipeline is
     running, it will be started first and then the stream will start. NOTE: in
-    this second case, the pipeline will also be automatically stopped once the
     this second case, the pipeline will also be automatically stopped once
     there are no more clients requesting any stream type from the module.
     """
 
     async def async_stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
-        """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["StatesStreamResponse"]:
+        """A method to get a stream of states messages from the pipeline"""
 
-        request = PointCloudStreamRequest()
-        request.point_cloud_type = point_cloud_type
-        request.coordinate_system = coordinate_system
-        request.fqdn = fqdn
+        request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.PointCloud/Stream",
+            "/blickfeld.percept_processing.services.States/Stream",
             request,
-            PointCloudStreamResponse,
+            StatesStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> Iterator["PointCloudStreamResponse"]:
-        """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["StatesStreamResponse"]:
+        """A method to get a stream of states messages from the pipeline"""
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
-            point_cloud_type=point_cloud_type,
-            coordinate_system=coordinate_system,
-            fqdn=fqdn,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/percept_toolkit/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/percept_toolkit/services/geometry.proto, blickfeld/percept_toolkit/services/health.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -28,14 +30,30 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Health Stream response of the toolkit module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The current health state of the module"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Health Get response of the toolkit module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The current health state of the module"""
+
+
+@dataclass(eq=False, repr=False)
 class GeometryComputeGroundAlignmentRequest(betterproto.Message):
     """
     Request for estimating alignment to ground/gravity based on imu-data and
     optional point cloud frame.
     """
 
     accelerometer_data: "__core_processing_data__.Acceleration" = (
@@ -92,28 +110,106 @@
     """
     Refined transformations. The array sequence is equal to the sequence in
     which the requests were received. The first element in the array
     corresponds to the lidar frame received in the first client stream message.
     """
 
 
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Health Stream response of the toolkit module"""
+class Health(betterproto.ServiceStub):
+    """An gRPC service to request the health of toolkit"""
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The current health state of the module"""
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        Streams health messages in regular intervals containing the state of
+        toolkit
+        """
 
+        request = betterproto_lib_google_protobuf.Empty()
 
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Health Get response of the toolkit module"""
+        async for response in self._unary_stream(
+            "/blickfeld.percept_toolkit.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The current health state of the module"""
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        Streams health messages in regular intervals containing the state of
+        toolkit
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Return health messages containing the state of toolkit"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_toolkit.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Return health messages containing the state of toolkit"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class Geometry(betterproto.ServiceStub):
     """Service offering on-demand geometric processing tasks."""
 
     async def async_compute_ground_alignment(
         self,
@@ -193,119 +289,27 @@
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     def compute_registration_refinement(
         self,
+        request_iterator: Iterable["GeometryComputeRegistrationRefinementRequest"],
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "GeometryComputeRegistrationRefinementResponse":
         """
         Refines the point cloud registration based on provided initial
         transformations. If the method succeeds, the refined transformation is
         returned. Otherwise an exception will be thrown.
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.async_compute_registration_refinement(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class Health(betterproto.ServiceStub):
-    """An gRPC service to request the health of toolkit"""
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Streams health messages in regular intervals containing the state of
-        toolkit
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.percept_toolkit.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Streams health messages in regular intervals containing the state of
-        toolkit
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Return health messages containing the state of toolkit"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_toolkit.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Return health messages containing the state of toolkit"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
+                request_iterator,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/push/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/push/config/authentication.proto, blickfeld/push/config/destination.proto, blickfeld/push/config/payload.proto, blickfeld/push/config/push.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
@@ -22,14 +24,25 @@
     """json representation of protobuf messages"""
 
     ENCODING_JSON_FLATTENED = 3
     """flattened json representation of protobuf messages"""
 
 
 @dataclass(eq=False, repr=False)
+class Payload(betterproto.Message):
+    """defines what type of data stream to use as payload"""
+
+    encoding: "PayloadEncoding" = betterproto.enum_field(1)
+    """payload encoding"""
+
+    data_type: "__percept_processing_data__.DataType" = betterproto.enum_field(3)
+    """payload data type to stream"""
+
+
+@dataclass(eq=False, repr=False)
 class Authentication(betterproto.Message):
     """Authentication definition"""
 
     user: str = betterproto.string_field(1)
     """the user name used for authentication"""
 
     password: str = betterproto.string_field(2)
@@ -76,25 +89,14 @@
     mqtt topic - if empty the
     'blickfeld/{data_type}/{encoding_type}/{config_name}' pattern is used as a
     default
     """
 
 
 @dataclass(eq=False, repr=False)
-class Payload(betterproto.Message):
-    """defines what type of data stream to use as payload"""
-
-    encoding: "PayloadEncoding" = betterproto.enum_field(1)
-    """payload encoding"""
-
-    data_type: "__percept_processing_data__.DataType" = betterproto.enum_field(3)
-    """payload data type to stream"""
-
-
-@dataclass(eq=False, repr=False)
 class Push(betterproto.Message):
     """defines a combination of stream and destination"""
 
     name: str = betterproto.string_field(1)
     """name of push"""
 
     payload: "Payload" = betterproto.message_field(2)
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/push/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/push/data/health.proto, blickfeld/push/data/status.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Dict
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/push/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/push/services/destination.proto, blickfeld/push/services/health.proto, blickfeld/push/services/push.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -25,30 +27,14 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """request get the health of the configured publisher"""
-
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """request watch the health of the configured publisher"""
-
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
-
-
-@dataclass(eq=False, repr=False)
 class PushStoreRequest(betterproto.Message):
     """request to add a push configuration"""
 
     uuid: str = betterproto.string_field(1)
     """the uuid of the configuration (has to be generated on client side!)"""
 
     push_config: "_config__.Push" = betterproto.message_field(2)
@@ -96,107 +82,35 @@
     """request to disable the push configuration with the given uuid"""
 
     uuid: str = betterproto.string_field(1)
     """configuration uuid to disable"""
 
 
 @dataclass(eq=False, repr=False)
-class DestinationValidateRequest(betterproto.Message):
-    """request to validate a configured destination"""
-
-    destination: "_config__.Destination" = betterproto.message_field(1)
-    """the current (possibly incomplete) configuration entered"""
-
-
-class Health(betterproto.ServiceStub):
-    """An gRPC service to request the status of push configurations"""
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.push.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
+class HealthGetResponse(betterproto.Message):
+    """request get the health of the configured publisher"""
 
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
 
-        request = betterproto_lib_google_protobuf.Empty()
 
-        async for response in self._unary_stream(
-            "/blickfeld.push.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """request watch the health of the configured publisher"""
 
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
 
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
 
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
+@dataclass(eq=False, repr=False)
+class DestinationValidateRequest(betterproto.Message):
+    """request to validate a configured destination"""
 
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+    destination: "_config__.Destination" = betterproto.message_field(1)
+    """the current (possibly incomplete) configuration entered"""
 
 
 class Push(betterproto.ServiceStub):
     """An gRPC service to configure multiple push settings"""
 
     async def async_store(
         self,
@@ -452,14 +366,102 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
+class Health(betterproto.ServiceStub):
+    """An gRPC service to request the status of push configurations"""
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.push.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.push.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
 class Destination(betterproto.ServiceStub):
     """An gRPC service to configure multiple push settings"""
 
     async def async_validate(
         self,
         *,
         destination: "_config__.Destination" = None,
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/system/config/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,63 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/system/config/device.proto, blickfeld/system/config/network.proto, blickfeld/system/config/scan_pattern.proto, blickfeld/system/config/time_synchronization.proto
 # plugin: python-betterproto
+import warnings
 from dataclasses import dataclass
 from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
+from ...eye_safety import data as __eye_safety_data__
+
 
 class DeviceClass(betterproto.Enum):
     """Enum to distinguish different device classes"""
 
     CLASS_UNKNOWN = 0
     CUBE = 1
     CUBE_RANGE = 2
     QB2 = 3
 
 
+class ScanPatternFrameMode(betterproto.Enum):
+    """
+    The frame mode specifies the point cloud frame's composition and can be
+    used to fine tune the LiDAR to specific use cases.
+    """
+
+    FRAME_MODE_UNSPECIFIED = 0
+    """Unspecified frame mode"""
+
+    FRAME_MODE_UP_DOWN = 1
+    """
+    The laser will trigger both during up and downramping phase and a point
+    cloud frame is the combination of the two. Points that are close in azimuth
+    and elevation in both phases will be recorded up to two seconds apart, this
+    mode is therefore recommended only for high frame rates or scenes without
+    fast objects.
+    """
+
+    FRAME_MODE_UP = 2
+    """
+    The laser will only trigger during the upramping phase. Because no laser is
+    fired during the downramping phase, this mode results in a more uniform
+    motion deformation for fast objects.
+    """
+
+    FRAME_MODE_SEPARATE = 3
+    """
+    The laser will trigger both during up and downramping phase but separate
+    point cloud frames will be emitted, which maximizes frame rate.
+    """
+
+
 @dataclass(eq=False, repr=False)
 class Network(betterproto.Message):
     """
     * The "Network" protocol message allows to define and setup the network
     configuration of the Qb2 device which can be further applied by
     "SetConfig()" service API. The message specifies the desired network
     configuration mode: "dhcp", "link-local","static" or their combination, and
@@ -143,32 +180,58 @@
     Password of the wireless network [NOTE] If the password is not set and the
     SSID did not change, the existing password is used. This mechanism is
     applied as the password is never returned via the GetConfig API.
     """
 
 
 @dataclass(eq=False, repr=False)
+class Device(betterproto.Message):
+    """This message describes a Blickfeld Lidar device"""
+
+    fqdn_or_ip: str = betterproto.string_field(1)
+    """Fully-qualified-domain-name / Hostname or IP address"""
+
+    name: str = betterproto.string_field(2)
+    """
+    Human-readable name of the device Optional: Is filled out by the service if
+    not given.
+    """
+
+    serial_number: str = betterproto.string_field(3)
+    """
+    Serial number of the device Optional: Is filled out by the service if not
+    given.
+    """
+
+    class_: "DeviceClass" = betterproto.enum_field(4)
+    """Device class Optional: Is filled out by the service if not given."""
+
+
+@dataclass(eq=False, repr=False)
 class ScanPattern(betterproto.Message):
     """
     * The scan pattern defines the movement of the mirrors. The key parameters
     of the pattern are the horizontal and vertical fields of view (FoV) as well
     as the number of scan lines per frame. The frame rate is defined by the
     total number of scan lines and the oscillation frequency of the mirrors
-    which is fixed and device-spcific.
+    which is fixed and device-specific.
     """
 
     horizontal: "ScanPatternHorizontal" = betterproto.message_field(1)
     vertical: "ScanPatternVertical" = betterproto.message_field(2)
     pulse: "ScanPatternPulse" = betterproto.message_field(3)
     read_only: bool = betterproto.bool_field(4)
     """
     this is an read_only flag and it will be set if this is a default scan
     pattern, which can't be changed or deleted.
     """
 
+    frame_rate: "ScanPatternFrameRate" = betterproto.message_field(5)
+    frame_mode: "ScanPatternFrameMode" = betterproto.enum_field(6)
+
 
 @dataclass(eq=False, repr=False)
 class ScanPatternHorizontal(betterproto.Message):
     """
     * This section defines the movement of the horizontal mirror. The mirror
     moves continuously with its own frequency. Each half-oscillation period of
     the mirror results in one scan line.
@@ -214,35 +277,121 @@
     scanlines_down: int = betterproto.uint32_field(3)
     """
     * Configures the amount of scan lines required for the down-ramping phase.
     During the down-ramping phase, the vertical mirror decreases its amplitude
     from the target FoV to 0 degrees. Default: 30
     """
 
+    foveation: "ScanPatternVerticalFoveation" = betterproto.message_field(4)
+    """Optionally configures a foveated region."""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternVerticalFoveation(betterproto.Message):
+    """
+    Configures a vertical field of view foveation. This enables the user to
+    specify a region of interest with a different scanline density which is
+    defined as the number of scanlines per degree of vertical field of view.
+    For constant frame rate this allows increasing the resolution in the region
+    of interest without having to reduce the vertical field of view.
+    """
+
+    fraction: float = betterproto.float_field(1)
+    """
+    The fraction of the field of view that the density factor is applies to.
+    The allowed value range is [0.15, 0.85].
+    """
+
+    density_factor: float = betterproto.float_field(2)
+    """
+    The foveation density factor defines the ratio of scanline density and
+    consequently point density inside the foveated region compared to outside
+    of it.
+    """
+
+    scanlines: int = betterproto.uint32_field(3)
+    """
+    Read-only parameter showing the number of scanlines in the foveated region.
+    If the frame mode is set to up-down or separate, this applies to both the
+    up-ramping and down-ramping phase individually.
+    """
+
 
 @dataclass(eq=False, repr=False)
 class ScanPatternPulse(betterproto.Message):
     """
-    * This section defines the pattern in which the laser pulses and captures
+    This section defines the pattern in which the laser pulses and captures
     sample points
     """
 
     angle_spacing: float = betterproto.float_field(1)
     """
     * Unit: [rad] – This defines the angle within which the horizontal mirror
     moves between two laser pulses. This parameter therefore defines the
     horizontal sampling resolution.
     """
 
+    uniform: "ScanPatternPulseUniform" = betterproto.message_field(2)
+    """Optional configure a uniform scan pattern"""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternPulseUniform(betterproto.Message):
+    """
+    Configure the uniform scan pattern The classic scan pattern does not
+    benefit uniformly from increasing the scanline count in a frame. The
+    uniform scan pattern is an optimization that tries to provide an optimally
+    homogeneous point cloud given the system's constraints. To configure the
+    scan pattern, the vertical field of view, the target frame rate and the
+    pulse mode are used.
+    """
+
+    pulse_mode: "__eye_safety_data__.PulseMode" = betterproto.enum_field(1)
+    """
+    Pulse mode to use for the uniform scan pattern. This will overwrite the
+    horizontal angle spacing.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternFrameRate(betterproto.Message):
+    """This section defines the frame rate of a scan pattern"""
+
+    target: float = betterproto.double_field(1)
+    """
+    Target frame rate used to synchronize the point clouds of multiple LiDAR
+    devices in a sensor setup
+    """
+
+    actual: float = betterproto.double_field(4)
+    """
+    Read-only parameter for the actual frame rate the LiDAR is currently
+    running at
+    """
+
+    maximum: float = betterproto.double_field(2)
+    """
+    IMPORTANT: This field is deprecated. It has been replaced by "actual" and
+    will not be supported in future releases. Read-only parameter for maximum
+    achievable frame rate of the scan pattern
+    """
+
+    def __post_init__(self) -> None:
+        super().__post_init__()
+        if self.is_set("maximum"):
+            warnings.warn(
+                "ScanPatternFrameRate.maximum is deprecated", DeprecationWarning
+            )
+
 
 @dataclass(eq=False, repr=False)
 class NamedScanPattern(betterproto.Message):
     """
-    Temporary container used for config storage TODO Remove when daedalus-
-    config supports map type.
+    Temporary container used for config storage TODO Remove when map type is
+    supported.
     """
 
     name: str = betterproto.string_field(1)
     scan_pattern: "ScanPattern" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
@@ -258,30 +407,7 @@
 
 @dataclass(eq=False, repr=False)
 class TimeSynchronizationNtp(betterproto.Message):
     """Configuration message for NTP time synchronization"""
 
     servers: List[str] = betterproto.string_field(1)
     """List of NTP time servers which are to be used"""
-
-
-@dataclass(eq=False, repr=False)
-class Device(betterproto.Message):
-    """This message describes a Blickfeld Lidar device"""
-
-    fqdn_or_ip: str = betterproto.string_field(1)
-    """Fully-qualified-domain-name / Hostname or IP address"""
-
-    name: str = betterproto.string_field(2)
-    """
-    Human-readable name of the device Optional: Is filled out by the service if
-    not given.
-    """
-
-    serial_number: str = betterproto.string_field(3)
-    """
-    Serial number of the device Optional: Is filled out by the service if not
-    given.
-    """
-
-    class_: "DeviceClass" = betterproto.enum_field(4)
-    """Device class Optional: Is filled out by the service if not given."""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/system/data/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/system/data/firmware.proto, blickfeld/system/data/health.proto, blickfeld/system/data/network_status.proto
+# sources: blickfeld/system/data/firmware.proto, blickfeld/system/data/health.proto, blickfeld/system/data/network_status.proto, blickfeld/system/data/scan_pattern.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
-from ...base import data as __base_data__
+from ...base import (
+    config as __base_config__,
+    data as __base_data__,
+)
 from .. import config as _config__
 
 
 @dataclass(eq=False, repr=False)
 class Firmware(betterproto.Message):
     """
     The Firmware data message contains all relevant information about the
@@ -122,14 +127,99 @@
     installation
     """
 
     pass
 
 
 @dataclass(eq=False, repr=False)
+class NetworkStatus(betterproto.Message):
+    """
+    Carries information about active connection: current statistics and network
+    configuration
+    """
+
+    active_config: "_config__.Network" = betterproto.message_field(1)
+    """Brings configuration information about currently active connection"""
+
+    statistics: "NetworkStatusStatistics" = betterproto.message_field(2)
+    """Brings statistical information about currently active connection"""
+
+
+@dataclass(eq=False, repr=False)
+class NetworkStatusStatistics(betterproto.Message):
+    """
+    (WIP) Carries statistical information about currently active connection
+    """
+
+    speed: str = betterproto.string_field(1)
+    """Link speed"""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternLimits(betterproto.Message):
+    """
+    This section contains limits for configurable parameters of a scan pattern
+    """
+
+    horizontal: "ScanPatternLimitsHorizontal" = betterproto.message_field(1)
+    vertical: "ScanPatternLimitsVertical" = betterproto.message_field(2)
+    frame_rate: "ScanPatternLimitsFrameRate" = betterproto.message_field(3)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternLimitsHorizontal(betterproto.Message):
+    """
+    This section defines the value limits for the horizontal configuration
+    """
+
+    field_of_view: "__base_config__.RangeFloat" = betterproto.message_field(1)
+    """The field of view limits"""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternLimitsVertical(betterproto.Message):
+    """This section defines the value limits for the vertical configuration"""
+
+    field_of_view: "__base_config__.RangeFloat" = betterproto.message_field(1)
+    """The field of view limits"""
+
+    scanlines_up: "__base_config__.RangeUint32" = betterproto.message_field(2)
+    """The up-ramping scanline limits"""
+
+    scanlines_down: "__base_config__.RangeUint32" = betterproto.message_field(3)
+    """The down-ramping scanline limits"""
+
+    foveation: "ScanPatternLimitsVerticalFoveation" = betterproto.message_field(4)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternLimitsVerticalFoveation(betterproto.Message):
+    """This section defines the limits for the foveation configuration"""
+
+    fraction: "__base_config__.RangeFloat" = betterproto.message_field(1)
+    """The foveation fraction limit"""
+
+    density_factor: "__base_config__.RangeFloat" = betterproto.message_field(2)
+    """The density factor limits"""
+
+    scanlines: "__base_config__.RangeUint32" = betterproto.message_field(3)
+    """The foveated scanlines limits"""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternLimitsFrameRate(betterproto.Message):
+    """
+    This section defines the value limits for the frame rate configuration
+    """
+
+    target: "__base_config__.RangeDouble" = betterproto.message_field(1)
+    """The target frame rate limit"""
+
+
+@dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """Message representing health"""
 
     state: "__base_data__.HealthState" = betterproto.enum_field(1)
     """High-level state of module"""
 
     state_reason: str = betterproto.string_field(2)
@@ -173,31 +263,7 @@
     """Time delay from NTP request until server response is received"""
 
     jitter: float = betterproto.float_field(5)
     """Jitter between multiple time comparisons"""
 
     precision: float = betterproto.float_field(6)
     """Precision of the NTP time synchronization"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkStatus(betterproto.Message):
-    """
-    Carries information about active connection: current statistics and network
-    configuration
-    """
-
-    active_config: "_config__.Network" = betterproto.message_field(1)
-    """Brings configuration information about currently active connection"""
-
-    statistics: "NetworkStatusStatistics" = betterproto.message_field(2)
-    """Brings statistical information about currently active connection"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkStatusStatistics(betterproto.Message):
-    """
-    (WIP) Carries statistical information about currently active connection
-    """
-
-    speed: str = betterproto.string_field(1)
-    """Link speed"""
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2/system/services/__init__.py` & `blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/system/services/firmware.proto, blickfeld/system/services/health.proto, blickfeld/system/services/network.proto, blickfeld/system/services/scan_pattern.proto, blickfeld/system/services/time_synchronization.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
@@ -15,14 +17,15 @@
 )
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import grpclib
 from blickfeld_qb2.betterproto.grpc.grpclib_server import ServiceBase
 
+from ...base import data as __base_data__
 from .. import (
     config as _config__,
     data as _data__,
 )
 
 
 if TYPE_CHECKING:
@@ -100,43 +103,52 @@
     """
     Please refer to <<_blickfeld_system_services_FirmwareInstallResponse,
     FirmwareInstallResponse>>.
     """
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareGetStatusResponse(betterproto.Message):
-    """Response with snapshot of current status."""
+class FirmwareFetchAndInstallRequest(betterproto.Message):
+    """Request for fetch & install request"""
 
-    status: "_data__.FirmwareStatus" = betterproto.message_field(1)
-    """Current firmware status"""
+    version: "__base_data__.Version" = betterproto.message_field(1, group="source")
+    """Select version to install"""
+
+    url: str = betterproto.string_field(2, group="source")
+    """Pass url to firmware bundle"""
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareWatchStatusResponse(betterproto.Message):
-    """Continuous response with status"""
+class FirmwareFetchAndInstallResponse(betterproto.Message):
+    """
+    Please refer to <<_blickfeld_system_services_FirmwareInstallResponse,
+    FirmwareInstallResponse>>.
+    """
 
     status: "_data__.FirmwareStatus" = betterproto.message_field(1)
-    """Current firmware status"""
+    """
+    Please refer to <<_blickfeld_system_services_FirmwareInstallResponse,
+    FirmwareInstallResponse>>.
+    """
 
 
 @dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request"""
+class FirmwareGetStatusResponse(betterproto.Message):
+    """Response with snapshot of current status."""
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
+    status: "_data__.FirmwareStatus" = betterproto.message_field(1)
+    """Current firmware status"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response to health watch request"""
+class FirmwareWatchStatusResponse(betterproto.Message):
+    """Continuous response with status"""
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
+    status: "_data__.FirmwareStatus" = betterproto.message_field(1)
+    """Current firmware status"""
 
 
 @dataclass(eq=False, repr=False)
 class ScanPatternGetResponse(betterproto.Message):
     name: str = betterproto.string_field(1)
     scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
 
@@ -170,14 +182,40 @@
 
 @dataclass(eq=False, repr=False)
 class ScanPatternDeleteRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
+class ScanPatternGetLimitsRequest(betterproto.Message):
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternGetLimitsResponse(betterproto.Message):
+    scan_pattern_limits: "_data__.ScanPatternLimits" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Response to health get request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response to health watch request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
 class NetworkValidateRequest(betterproto.Message):
     """Request to validate method"""
 
     config: "_config__.Network" = betterproto.message_field(1)
     """Configuration which should be validated"""
 
 
@@ -245,26 +283,28 @@
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     def upload(
         self,
+        request_iterator: Iterable["FirmwareUploadRequest"],
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "FirmwareUploadResponse":
         """
         Upload the firmware bundle from the client to the device. Fails if the
         uploaded firmware bundle is not valid.
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.async_upload(
+                request_iterator,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
     async def async_install(
@@ -344,22 +384,24 @@
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def upload_and_install(
         self,
+        request_iterator: Iterable["FirmwareUploadAndInstallRequest"],
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> Iterator["FirmwareUploadAndInstallResponse"]:
         """Combines the Upload and Install steps in a single method."""
 
         loop = asyncio.get_event_loop()
         ait = self.async_upload_and_install(
+            request_iterator,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -370,92 +412,61 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    async def async_get_status(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareGetStatusResponse":
-        """
-        Get the current firmware status which includes the currently installed
-        firmware but also ongoing or failed installations.
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.system.services.Firmware/GetStatus",
-            request,
-            FirmwareGetStatusResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get_status(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareGetStatusResponse":
-        """
-        Get the current firmware status which includes the currently installed
-        firmware but also ongoing or failed installations.
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_status(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch_status(
+    async def async_fetch_and_install(
         self,
+        *,
+        version: "__base_data__.Version" = None,
+        url: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["FirmwareWatchStatusResponse"]:
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["FirmwareFetchAndInstallResponse"]:
         """
-        Continously watch the status stream and get updates on changes. This
-        can be used to attach to an ongoing installation.
+        Fetch a firmware bundle from a static file server and perform
+        installation.
         """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = FirmwareFetchAndInstallRequest()
+        if version is not None:
+            request.version = version
+        request.url = url
 
         async for response in self._unary_stream(
-            "/blickfeld.system.services.Firmware/WatchStatus",
+            "/blickfeld.system.services.Firmware/FetchAndInstall",
             request,
-            FirmwareWatchStatusResponse,
+            FirmwareFetchAndInstallResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
-    def watch_status(
+    def fetch_and_install(
         self,
+        *,
+        version: "__base_data__.Version" = None,
+        url: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["FirmwareWatchStatusResponse"]:
+        metadata: Optional["MetadataLike"] = None
+    ) -> Iterator["FirmwareFetchAndInstallResponse"]:
         """
-        Continously watch the status stream and get updates on changes. This
-        can be used to attach to an ongoing installation.
+        Fetch a firmware bundle from a static file server and perform
+        installation.
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch_status(
+        ait = self.async_fetch_and_install(
+            version=version,
+            url=url,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -466,93 +477,92 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-
-class Health(betterproto.ServiceStub):
-    """
-    The health service provides methods to monitor operational status of the
-    systen module
-    """
-
-    async def async_get(
+    async def async_get_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the systen module"""
+    ) -> "FirmwareGetStatusResponse":
+        """
+        Get the current firmware status which includes the currently installed
+        firmware but also ongoing or failed installations.
+        """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Health/Get",
+            "/blickfeld.system.services.Firmware/GetStatus",
             request,
-            HealthGetResponse,
+            FirmwareGetStatusResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def get_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the systen module"""
+    ) -> "FirmwareGetStatusResponse":
+        """
+        Get the current firmware status which includes the currently installed
+        firmware but also ongoing or failed installations.
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_get_status(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_watch(
+    async def async_watch_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
+    ) -> AsyncIterator["FirmwareWatchStatusResponse"]:
         """
-        Can be used to attach to the health monitoring status information of
-        the systen module
+        Continously watch the status stream and get updates on changes. This
+        can be used to attach to an ongoing installation.
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.system.services.Health/Watch",
+            "/blickfeld.system.services.Firmware/WatchStatus",
             request,
-            HealthWatchResponse,
+            FirmwareWatchStatusResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
-    def watch(
+    def watch_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
+    ) -> Iterator["FirmwareWatchStatusResponse"]:
         """
-        Can be used to attach to the health monitoring status information of
-        the systen module
+        Continously watch the status stream and get updates on changes. This
+        can be used to attach to an ongoing installation.
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch(
+        ait = self.async_watch_status(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -821,14 +831,154 @@
                 name=name,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
+    async def async_get_limits(
+        self,
+        *,
+        scan_pattern: "_config__.ScanPattern" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ScanPatternGetLimitsResponse":
+        """Get a scan pattern's parameter limits"""
+
+        request = ScanPatternGetLimitsRequest()
+        if scan_pattern is not None:
+            request.scan_pattern = scan_pattern
+
+        return await self._unary_unary(
+            "/blickfeld.system.services.ScanPattern/GetLimits",
+            request,
+            ScanPatternGetLimitsResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_limits(
+        self,
+        *,
+        scan_pattern: "_config__.ScanPattern" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ScanPatternGetLimitsResponse":
+        """Get a scan pattern's parameter limits"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get_limits(
+                scan_pattern=scan_pattern,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+
+class Health(betterproto.ServiceStub):
+    """
+    The health service provides methods to monitor operational status of the
+    systen module
+    """
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the systen module"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.system.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the systen module"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        Can be used to attach to the health monitoring status information of
+        the systen module
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.system.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        Can be used to attach to the health monitoring status information of
+        the systen module
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
 
 class Network(betterproto.ServiceStub):
     """
     The network service allows to setup network configuration of Qb2 device.
     The exact structure of configuration settings is defined by "Network"
     protocol message. Service provides "SetConfig()" and "GetConfig()" API
     which allow to apply and read out configuration settings at run-time. The
```

### Comparing `blickfeld_qb2-1.9.0/blickfeld_qb2.egg-info/SOURCES.txt` & `blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 blickfeld_qb2/__init__.py
 blickfeld_qb2.egg-info/PKG-INFO
 blickfeld_qb2.egg-info/SOURCES.txt
 blickfeld_qb2.egg-info/dependency_links.txt
 blickfeld_qb2.egg-info/requires.txt
 blickfeld_qb2.egg-info/top_level.txt
 blickfeld_qb2/base/__init__.py
+blickfeld_qb2/base/config/__init__.py
 blickfeld_qb2/base/data/__init__.py
 blickfeld_qb2/base/geometry/__init__.py
 blickfeld_qb2/base/grpc/__init__.py
 blickfeld_qb2/base/grpc/channel.py
 blickfeld_qb2/base/grpc/device_ca_cert.py
 blickfeld_qb2/beam_deflection_control/__init__.py
 blickfeld_qb2/beam_deflection_control/config/__init__.py
@@ -34,25 +35,29 @@
 blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
 blickfeld_qb2/betterproto/plugin/__init__.py
 blickfeld_qb2/betterproto/plugin/__main__.py
 blickfeld_qb2/betterproto/plugin/compiler.py
 blickfeld_qb2/betterproto/plugin/main.py
 blickfeld_qb2/betterproto/plugin/models.py
 blickfeld_qb2/betterproto/plugin/parser.py
+blickfeld_qb2/config/__init__.py
+blickfeld_qb2/config/data/__init__.py
 blickfeld_qb2/core_processing/__init__.py
 blickfeld_qb2/core_processing/config/__init__.py
 blickfeld_qb2/core_processing/data/__init__.py
 blickfeld_qb2/core_processing/services/__init__.py
 blickfeld_qb2/detector/__init__.py
 blickfeld_qb2/detector/data/__init__.py
 blickfeld_qb2/detector/services/__init__.py
 blickfeld_qb2/diagnostics/__init__.py
 blickfeld_qb2/diagnostics/config/__init__.py
 blickfeld_qb2/diagnostics/data/__init__.py
 blickfeld_qb2/diagnostics/services/__init__.py
+blickfeld_qb2/eye_safety/__init__.py
+blickfeld_qb2/eye_safety/data/__init__.py
 blickfeld_qb2/flow/__init__.py
 blickfeld_qb2/flow/config/__init__.py
 blickfeld_qb2/flow/services/__init__.py
 blickfeld_qb2/hardware/__init__.py
 blickfeld_qb2/hardware/config/__init__.py
 blickfeld_qb2/hardware/services/__init__.py
 blickfeld_qb2/laser/__init__.py
@@ -68,11 +73,17 @@
 blickfeld_qb2/percept_toolkit/__init__.py
 blickfeld_qb2/percept_toolkit/data/__init__.py
 blickfeld_qb2/percept_toolkit/services/__init__.py
 blickfeld_qb2/push/__init__.py
 blickfeld_qb2/push/config/__init__.py
 blickfeld_qb2/push/data/__init__.py
 blickfeld_qb2/push/services/__init__.py
+blickfeld_qb2/secure/__init__.py
+blickfeld_qb2/secure/client/__init__.py
+blickfeld_qb2/secure/client/token_factory.py
+blickfeld_qb2/secure/config/__init__.py
+blickfeld_qb2/secure/data/__init__.py
+blickfeld_qb2/secure/services/__init__.py
 blickfeld_qb2/system/__init__.py
 blickfeld_qb2/system/config/__init__.py
 blickfeld_qb2/system/data/__init__.py
 blickfeld_qb2/system/services/__init__.py
```

### Comparing `blickfeld_qb2-1.9.0/setup.py` & `blickfeld_qb2-2.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="blickfeld_qb2",
-    version="1.9.0",
+    version="2.0.7",
     author="Blickfeld GmbH",
     author_email="opensource@blickfeld.com",
     url="https://github.com/Blickfeld/blickfeld-qb2",
     description="Python package to communicate securely with Qb2 LiDAR devices of the Blickfeld GmbH",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

