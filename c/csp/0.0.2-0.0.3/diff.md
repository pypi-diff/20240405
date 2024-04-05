# Comparing `tmp/csp-0.0.2.tar.gz` & `tmp/csp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp-0.0.2.tar", last modified: Thu Mar 14 15:22:38 2024, max compression
+gzip compressed data, was "csp-0.0.3.tar", last modified: Fri Apr  5 18:58:15 2024, max compression
```

## Comparing `csp-0.0.2.tar` & `csp-0.0.3.tar`

### file list

```diff
@@ -1,609 +1,626 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.905847 csp-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-03-14 15:22:08.000000 csp-0.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-14 15:22:08.000000 csp-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-14 15:22:08.000000 csp-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)   307468 2024-03-14 15:22:08.000000 csp-0.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    18926 2024-03-14 15:22:38.905847 csp-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-14 15:22:08.000000 csp-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.801847 csp-0.0.2/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.797847 csp-0.0.2/cpp/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.809847 csp-0.0.2/cpp/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindBrotli.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindCSP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindColor.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindDepsBase.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindDepsKafkaAdapter.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindDepsParquetAdapter.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindGRPC.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindNumpy.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindPyArrow.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindPythonHeaders.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/FindRdKafka.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/Findcsp_autogen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/Findlz4.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/cmake/modules/Findutf8proc.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.801847 csp-0.0.2/cpp/csp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.809847 csp-0.0.2/cpp/csp/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.813847 csp-0.0.2/cpp/csp/adapters/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaAdapterManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaAdapterManager.h
--rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaConsumer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaConsumer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaOutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaOutputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaPublisher.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaPublisher.h
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaSubscriber.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/kafka/KafkaSubscriber.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.817847 csp-0.0.2/cpp/csp/adapters/parquet/
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ArrowSingleColumnArrayBuilder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/DialectGenericListReaderInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/DialectGenericListWriterInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileReaderWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileReaderWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapperContainer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapperContainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    19969 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetInputAdapterManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetInputAdapterManager.h
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.h
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetReader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18634 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    38394 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetStatusUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/parquet/ParquetWriter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.821847 csp-0.0.2/cpp/csp/adapters/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/FileUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/JSONMessageStructConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/JSONMessageStructConverter.h
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/JSONMessageWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageEnums.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageEnums.h
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageStructConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageStructConverter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/MessageWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/ProtobufHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/ProtobufHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/ProtobufMessageStructConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/ProtobufMessageStructConverter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/RawBytesMessageStructConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/RawBytesMessageStructConverter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/StructAdapterInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/adapters/utils/ValueDispatcher.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.825847 csp-0.0.2/cpp/csp/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/BasicAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Config.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/DynamicBitSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Enum.h
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/EnumBitSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Exception.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Exception.h
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/FileUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Generator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Hash.h
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Likely.h
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Platform.h
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/QueueWaiter.h
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/SRMWLockFreeQueue.h
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/System.h
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/TaggedPointerUnion.h
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Time.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23465 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/core/Time.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.825847 csp-0.0.2/cpp/csp/cppnodes/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18952 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/baselibimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/basketlibimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/mathimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/statsimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    58142 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/cppnodes/statsimpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.837847 csp-0.0.2/cpp/csp/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/AdapterManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/AdapterManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/AlarmInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/BasketInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/BasketInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/ConstInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Consumer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Consumer.h
--rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CppNode.h
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CspEnum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CspEnum.h
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CspType.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12492 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CspType.h
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CycleStepTable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/CycleStepTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/DialectGenericType.h
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Dictionary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Dictionary.h
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/DynamicEngine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/DynamicEngine.h
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/DynamicNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/DynamicNode.h
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Engine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Engine.h
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Enums.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Enums.h
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/EventPropagator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/EventPropagator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Feedback.h
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/GraphOutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/GraphOutputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/InputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/InputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/InputId.h
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Node.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Node.h
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/OutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/OutputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PartialSwitchCspType.h
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PendingPushEvents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PendingPushEvents.h
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Profiler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PullInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PushEvent.h
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PushInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PushPullInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/PushPullInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/RootEngine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/RootEngine.h
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/StatusAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/StatusAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Struct.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    28073 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/Struct.h
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TickBuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TimeSeries.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TimeSeries.h
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TimeSeriesProvider.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TimeSeriesProvider.h
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TimerInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/TypeCast.h
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/VectorContainer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/VectorContainer.h
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/engine/WindowBuffer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.849847 csp-0.0.2/cpp/csp/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/Common.h
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/Conversions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/Conversions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/CspTypeFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/CspTypeFactory.h
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/Exception.h
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/InitHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/NumpyConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/NumpyConversions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/NumpyInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyAdapterManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyAdapterManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyAdapterManagerWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyAdapterManagerWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    29390 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyBasketInputProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyBasketInputProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyBasketOutputProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyBasketOutputProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyConstAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyConstants.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyConstants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCppNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCppNode.h
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCspEnum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCspEnum.h
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCspType.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyCspType.h
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyDynamicNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyEngine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyEngine.h
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyFeedbackAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyGraphOutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyGraphOutputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyInputAdapterWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyInputAdapterWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyInputProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyInputProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyManagedSimInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNode.h
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNodeWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNodeWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNumbaNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNumbaNode.h
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyNumpyAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyObjectPtr.h
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyOutputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyOutputAdapterWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyOutputAdapterWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyOutputProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyOutputProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyPullInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyPushInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyPushInputAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyPushPullInputAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38171 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyStruct.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyStruct.h
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/PyTimerAdapter.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.849847 csp-0.0.2/cpp/csp/python/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/kafkaadapterimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    26678 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/parquetadapterimpl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.801847 csp-0.0.2/cpp/csp/python/adapters/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.801847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.801847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.857847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/api.h
--rw-r--r--   0 runner    (1001) docker     (127)    92609 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.h
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_python_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/async.h
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.h
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.h
--rw-r--r--   0 runner    (1001) docker     (127)    23001 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.h
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.h
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.h
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.h
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.h
--rw-r--r--   0 runner    (1001) docker     (127)    23333 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.cc
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.h
--rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.cc
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.h
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.h
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/iterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib.h
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib_api.h
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.h
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_interop.h
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.h
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.h
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/platform.h
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.h
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_api.h
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.h
--rw-r--r--   0 runner    (1001) docker     (127)    45624 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.h
--rw-r--r--   0 runner    (1001) docker     (127)    32667 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.h
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/type_traits.h
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/visibility.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util_overflow.h
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/io_util.h
--rw-r--r--   0 runner    (1001) docker     (127)    18101 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/iterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/key_value_metadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/launder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/list_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/map.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/math_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/parallel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/pcg_random.h
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/print.h
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/range.h
--rw-r--r--   0 runner    (1001) docker     (127)    22395 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ree_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/regex.h
--rw-r--r--   0 runner    (1001) docker     (127)    31035 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rle_encoding.h
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rows_to_batches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/simd.h
--rw-r--r--   0 runner    (1001) docker     (127)    14421 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/small_vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/sort.h
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/spaced.h
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/span.h
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/stopwatch.h
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string.h
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string_builder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/task_group.h
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tdigest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/test_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/time.h
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tracing.h
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/trie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_fwd.h
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_traits.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ubsan.h
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/union_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/unreachable.h
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/uri.h
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/utf8.h
--rw-r--r--   0 runner    (1001) docker     (127)    29514 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/value_parsing.h
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/visibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_compatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_fixup.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/debug-trap.h
--rw-r--r--   0 runner    (1001) docker     (127)    48167 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/safe-math.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/
--rw-r--r--   0 runner    (1001) docker     (127)   253096 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspbaselibimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspbasketlibimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspmathimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspnpstatsimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/cspstatsimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/csptypesimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    44065 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/csp/python/npstatsimpl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_basic_allocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_dynamicbitset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_srmwlockfreequeue.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_tagged_pointer_union.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/core/test_time.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.869847 csp-0.0.2/cpp/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_dictionary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_engine_initial.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_partial_switch_csp_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_tick_buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_time_series.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-14 15:22:08.000000 csp-0.0.2/cpp/tests/engine/test_window_buffer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.873847 csp-0.0.2/csp/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-14 15:22:08.000000 csp-0.0.2/csp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.877847 csp-0.0.2/csp/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.877847 csp-0.0.2/csp/adapters/output_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/output_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/output_adapters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/output_adapters/parquet_utility_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15993 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/symphony.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-14 15:22:08.000000 csp-0.0.2/csp/adapters/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26853 2024-03-14 15:22:08.000000 csp-0.0.2/csp/baselib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-14 15:22:08.000000 csp-0.0.2/csp/basketlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.877847 csp-0.0.2/csp/build/
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-03-14 15:22:08.000000 csp-0.0.2/csp/build/csp_autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-14 15:22:08.000000 csp-0.0.2/csp/cache_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-14 15:22:08.000000 csp-0.0.2/csp/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10374 2024-03-14 15:22:08.000000 csp-0.0.2/csp/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.881847 csp-0.0.2/csp/impl/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/__cspimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/__csptypesimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/adaptermanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/builtin_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/genericpushadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.881847 csp-0.0.2/csp/impl/managed_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/aggregation_period_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/cache_partition_argument_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/cache_user_custom_object_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/dateset_name_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23137 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/managed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/managed_dataset_lock_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/managed_dataset_merge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/managed_dataset_path_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14306 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/managed_dataset/managed_parquet_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/mem_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/outputadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    28325 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pandas_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pandas_ext_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pandas_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pulladapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pushadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/pushpulladapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.885847 csp-0.0.2/csp/impl/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/autogen_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/common_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/container_type_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/generic_values_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    34727 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/instantiation_type_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/numpy_type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/tstype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/type_annotation_normalizer_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/types/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.889847 csp-0.0.2/csp/impl/wiring/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.889847 csp-0.0.2/csp/impl/wiring/cache_support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/cache_config_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/cache_type_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30753 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/dataset_partition_cached_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    32636 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/graph_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/partition_files_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/cache_support/runtime_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/delayed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/delayed_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    41137 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    19155 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_node_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.889847 csp-0.0.2/csp/impl/wiring/numba_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/csp_cpp_numba_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/csp_numba_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/csp_string_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/datetime_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/numba_utils/numba_type_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/special_output_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-14 15:22:08.000000 csp-0.0.2/csp/impl/wiring/threaded_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-03-14 15:22:08.000000 csp-0.0.2/csp/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    21094 2024-03-14 15:22:08.000000 csp-0.0.2/csp/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-03-14 15:22:08.000000 csp-0.0.2/csp/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-14 15:22:08.000000 csp-0.0.2/csp/showgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)   119200 2024-03-14 15:22:08.000000 csp-0.0.2/csp/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.893847 csp-0.0.2/csp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.897847 csp-0.0.2/csp/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/arrow_test_data.arrow
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/csv_test_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/kafka_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/parquet_test_data.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47885 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/adapters/test_symphony.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.897847 csp-0.0.2/csp/tests/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_dateframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_genericpushadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_numba_features_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_outputadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38448 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pandas_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18337 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pandas_ext_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pandas_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pulladapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pushadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_pushpulladapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    37103 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.901847 csp-0.0.2/csp/tests/impl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/utils/test_lock_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.901847 csp-0.0.2/csp/tests/impl/wiring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.901847 csp-0.0.2/csp/tests/impl/wiring/numba_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/numba_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/numba_utils/test_numba_datetime_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_basket_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/impl/wiring/test_threaded_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    51011 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_baselib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_basketlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_baskets.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)   171306 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    71950 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_graph_mem_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    43345 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_numba_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_numba_type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    70820 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_showgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)   175557 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/test_type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.901847 csp-0.0.2/csp/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/utils/test_object_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-14 15:22:08.000000 csp-0.0.2/csp/tests/utils/typed_curve_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-14 15:22:08.000000 csp-0.0.2/csp/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.905847 csp-0.0.2/csp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/classproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/csp_watch_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/file_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/lock_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    26396 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/object_factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/qualified_name_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-14 15:22:08.000000 csp-0.0.2/csp/utils/rm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:22:38.905847 csp-0.0.2/csp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18926 2024-03-14 15:22:38.000000 csp-0.0.2/csp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23781 2024-03-14 15:22:38.000000 csp-0.0.2/csp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:22:38.000000 csp-0.0.2/csp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-14 15:22:38.000000 csp-0.0.2/csp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-14 15:22:38.000000 csp-0.0.2/csp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-14 15:22:08.000000 csp-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:22:38.905847 csp-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-14 15:22:08.000000 csp-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-14 15:22:08.000000 csp-0.0.2/vcpkg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.022821 csp-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-05 18:57:42.000000 csp-0.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-05 18:57:42.000000 csp-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 18:57:42.000000 csp-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)   319767 2024-04-05 18:57:42.000000 csp-0.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    18926 2024-04-05 18:58:15.018821 csp-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-05 18:57:42.000000 csp-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.918822 csp-0.0.3/cpp/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindBrotli.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindCSP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindColor.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindDepsBase.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindDepsKafkaAdapter.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindDepsParquetAdapter.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    19510 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindGRPC.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindNumpy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindPyArrow.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindPythonHeaders.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/FindRdKafka.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/Findcsp_autogen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/Findlz4.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/cmake/modules/Findutf8proc.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/csp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.918822 csp-0.0.3/cpp/csp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.922822 csp-0.0.3/cpp/csp/adapters/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaAdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaAdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaConsumer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaConsumer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaOutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaPublisher.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaPublisher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaSubscriber.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/kafka/KafkaSubscriber.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.930822 csp-0.0.3/cpp/csp/adapters/parquet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ArrowSingleColumnArrayBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/DialectGenericListReaderInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/DialectGenericListWriterInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileReaderWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileReaderWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapperContainer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapperContainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19969 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetInputAdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetInputAdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38394 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetStatusUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/parquet/ParquetWriter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.930822 csp-0.0.3/cpp/csp/adapters/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/FileUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/JSONMessageStructConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/JSONMessageStructConverter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/JSONMessageWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageEnums.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageEnums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageStructConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageStructConverter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/MessageWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19750 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/ProtobufHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/ProtobufHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/ProtobufMessageStructConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/ProtobufMessageStructConverter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/RawBytesMessageStructConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/RawBytesMessageStructConverter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/StructAdapterInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/utils/ValueDispatcher.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.934822 csp-0.0.3/cpp/csp/adapters/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientAdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientAdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientHeaderUpdateAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientHeaderUpdateAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/ClientOutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/WebsocketEndpoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/adapters/websocket/WebsocketEndpoint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.938822 csp-0.0.3/cpp/csp/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/BasicAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/DynamicBitSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/EnumBitSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Exception.h
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/FileUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Generator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Hash.h
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Likely.h
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Platform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/QueueWaiter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/SRMWLockFreeQueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/System.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/TaggedPointerUnion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Time.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23465 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/core/Time.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.938822 csp-0.0.3/cpp/csp/cppnodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/baselibimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/basketlibimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/mathimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/statsimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    58148 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/cppnodes/statsimpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.950822 csp-0.0.3/cpp/csp/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/AdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/AdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/AlarmInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/BasketInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/BasketInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/ConstInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Consumer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Consumer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24199 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CppNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CspEnum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CspEnum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CspType.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CspType.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CycleStepTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/CycleStepTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/DialectGenericType.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Dictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Dictionary.h
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/DynamicEngine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/DynamicEngine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/DynamicNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/DynamicNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Engine.h
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/EventPropagator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/EventPropagator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Feedback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/GraphOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/GraphOutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/InputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/InputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/InputId.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Node.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Node.h
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/OutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/OutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PartialSwitchCspType.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PendingPushEvents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PendingPushEvents.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Profiler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PullInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PushEvent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PushInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PushPullInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/PushPullInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/RootEngine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/RootEngine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/StatusAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/StatusAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Struct.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28221 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/Struct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TickBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TimeSeries.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TimeSeries.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TimeSeriesProvider.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TimeSeriesProvider.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TimerInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/TypeCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/VectorContainer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/VectorContainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/engine/WindowBuffer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.962822 csp-0.0.3/cpp/csp/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/Common.h
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/Conversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24936 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/Conversions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/CspTypeFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/CspTypeFactory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/Exception.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/InitHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/NumpyConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/NumpyConversions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/NumpyInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyAdapterManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyAdapterManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyAdapterManagerWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyAdapterManagerWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29390 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyBasketInputProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyBasketInputProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyBasketOutputProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyBasketOutputProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyConstAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyConstants.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyConstants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCppNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCppNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCspEnum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCspEnum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCspType.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyCspType.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyDynamicNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyEngine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyEngine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyFeedbackAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyGraphOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyGraphOutputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyInputAdapterWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyInputAdapterWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyInputProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyInputProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyManagedSimInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNodeWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNodeWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNumbaNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNumbaNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyNumpyAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyObjectPtr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyOutputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyOutputAdapterWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyOutputAdapterWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyOutputProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyOutputProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyPullInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyPushInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyPushInputAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyPushPullInputAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39248 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyStruct.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyStruct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyStructToJson.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyStructToJson.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/PyTimerAdapter.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.962822 csp-0.0.3/cpp/csp/python/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/kafkaadapterimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26306 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/parquetadapterimpl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/csp/python/adapters/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.910822 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.974821 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/api.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92609 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_python_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/async.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23001 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23333 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/iterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib_api.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_interop.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/platform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_api.h
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45624 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32667 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/type_traits.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/visibility.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.982821 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util_overflow.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/io_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18101 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/iterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/key_value_metadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/launder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/list_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/math_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/parallel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/pcg_random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/print.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/range.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22395 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ree_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/regex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31035 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rle_encoding.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rows_to_batches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/simd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14421 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/small_vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/sort.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/spaced.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/span.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/stopwatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string_builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/task_group.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tdigest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/time.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tracing.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/trie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_traits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ubsan.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/union_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/unreachable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/uri.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29514 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/value_parsing.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/visibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_fixup.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.982821 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.982821 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/debug-trap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48167 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/safe-math.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.982821 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/
+-rw-r--r--   0 runner    (1001) docker     (127)   253096 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/adapters/websocketadapterimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspbaselibimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspbasketlibimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspmathimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspnpstatsimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/cspstatsimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/csptestlibimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/csptypesimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    44065 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/csp/python/npstatsimpl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.982821 csp-0.0.3/cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.986821 csp-0.0.3/cpp/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_basic_allocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_dynamicbitset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_srmwlockfreequeue.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_tagged_pointer_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/core/test_time.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.986821 csp-0.0.3/cpp/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_dictionary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_engine_initial.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_partial_switch_csp_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_tick_buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_time_series.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-05 18:57:42.000000 csp-0.0.3/cpp/tests/engine/test_window_buffer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.990821 csp-0.0.3/csp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-05 18:57:42.000000 csp-0.0.3/csp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.990821 csp-0.0.3/csp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.990821 csp-0.0.3/csp/adapters/output_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/output_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/output_adapters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/output_adapters/parquet_utility_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/symphony.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 18:57:42.000000 csp-0.0.3/csp/adapters/websocket_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26853 2024-04-05 18:57:42.000000 csp-0.0.3/csp/baselib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-05 18:57:42.000000 csp-0.0.3/csp/basketlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.990821 csp-0.0.3/csp/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-05 18:57:42.000000 csp-0.0.3/csp/build/csp_autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 18:57:42.000000 csp-0.0.3/csp/cache_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-05 18:57:42.000000 csp-0.0.3/csp/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2024-04-05 18:57:42.000000 csp-0.0.3/csp/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.994821 csp-0.0.3/csp/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/__cspimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/__csptypesimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/adaptermanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/builtin_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/genericpushadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.998821 csp-0.0.3/csp/impl/managed_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/aggregation_period_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/cache_partition_argument_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/cache_user_custom_object_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/dateset_name_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23137 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/managed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/managed_dataset_lock_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/managed_dataset_merge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/managed_dataset_path_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14306 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/managed_dataset/managed_parquet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/mem_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/outputadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28325 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pandas_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pandas_ext_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pandas_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pulladapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pushadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/pushpulladapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:14.998821 csp-0.0.3/csp/impl/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/autogen_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/common_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/container_type_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/generic_values_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34727 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/instantiation_type_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/numpy_type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/tstype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/type_annotation_normalizer_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/types/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.002821 csp-0.0.3/csp/impl/wiring/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.002821 csp-0.0.3/csp/impl/wiring/cache_support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/cache_config_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/cache_type_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30753 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/dataset_partition_cached_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32636 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/graph_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/partition_files_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/cache_support/runtime_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/delayed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/delayed_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41597 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/node_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19155 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_node_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.006821 csp-0.0.3/csp/impl/wiring/numba_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/csp_cpp_numba_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/csp_numba_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/csp_string_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/datetime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/numba_utils/numba_type_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/special_output_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-05 18:57:42.000000 csp-0.0.3/csp/impl/wiring/threaded_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-05 18:57:42.000000 csp-0.0.3/csp/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21094 2024-04-05 18:57:42.000000 csp-0.0.3/csp/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-05 18:57:42.000000 csp-0.0.3/csp/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-05 18:57:42.000000 csp-0.0.3/csp/showgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119200 2024-04-05 18:57:42.000000 csp-0.0.3/csp/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.010821 csp-0.0.3/csp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.010821 csp-0.0.3/csp/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/arrow_test_data.arrow
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/csv_test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/kafka_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/parquet_test_data.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/adapters/test_symphony.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.014821 csp-0.0.3/csp/tests/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_dateframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_genericpushadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_numba_features_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_outputadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38448 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pandas_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18337 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pandas_ext_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pandas_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pulladapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pushadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_pushpulladapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56082 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.014821 csp-0.0.3/csp/tests/impl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/utils/test_lock_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.014821 csp-0.0.3/csp/tests/impl/wiring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.014821 csp-0.0.3/csp/tests/impl/wiring/numba_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/numba_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/numba_utils/test_numba_datetime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_basket_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/impl/wiring/test_threaded_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51085 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_baselib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_basketlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171306 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74540 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_graph_mem_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43345 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_numba_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_numba_type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70820 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_showgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)   175557 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/test_type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.014821 csp-0.0.3/csp/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/utils/test_object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-05 18:57:42.000000 csp-0.0.3/csp/tests/utils/typed_curve_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 18:57:42.000000 csp-0.0.3/csp/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.018821 csp-0.0.3/csp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/csp_watch_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/file_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/lock_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26396 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/object_factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/qualified_name_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-05 18:57:42.000000 csp-0.0.3/csp/utils/rm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:58:15.018821 csp-0.0.3/csp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18926 2024-04-05 18:58:14.000000 csp-0.0.3/csp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24512 2024-04-05 18:58:14.000000 csp-0.0.3/csp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:58:14.000000 csp-0.0.3/csp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-05 18:58:14.000000 csp-0.0.3/csp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 18:58:14.000000 csp-0.0.3/csp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-05 18:57:42.000000 csp-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:58:15.022821 csp-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-05 18:57:42.000000 csp-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 18:57:42.000000 csp-0.0.3/vcpkg.json
```

### Comparing `csp-0.0.2/CMakeLists.txt` & `csp-0.0.3/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ###################################################################################################################################################
 # Project Configuration #
 #########################
 cmake_minimum_required(VERSION 3.20.0)
-project(csp VERSION "0.0.2")
+project(csp VERSION "0.0.3")
 set(CMAKE_CXX_STANDARD 17)
 
 ###################################################################################################################################################
 # CMake Dependencies #
 ######################
 include(CheckCCompilerFlag)
 include(CheckLinkerFlag)
@@ -67,14 +67,15 @@
 option(CSP_USE_VCPKG "Build with vcpkg dependencies" ON)
 option(CSP_USE_CCACHE "Build with ccache caching" OFF)
 option(CSP_USE_LD_CLASSIC_MAC "On macOS, link with ld_classic" OFF)
 
 # Extension options
 option(CSP_BUILD_KAFKA_ADAPTER "Build kafka adapter" ON)
 option(CSP_BUILD_PARQUET_ADAPTER "Build parquet adapter" ON)
+option(CSP_BUILD_WS_CLIENT_ADAPTER "Build ws client adapter" ON)
 
 # Normalize build type for downstream comparisons
 string(TOLOWER "${CMAKE_BUILD_TYPE}" CMAKE_BUILD_TYPE_LOWER)
 
 # Python library config
 set(BUILD_SHARED_LIBS TRUE)
 set(CMAKE_MACOSX_RPATH TRUE)
@@ -111,43 +112,17 @@
     # assume built-in pthreads on MacOS
     set(CMAKE_THREAD_LIBS_INIT "-lpthread")
     set(CMAKE_HAVE_THREADS_LIBRARY 1)
     set(CMAKE_USE_WIN32_THREADS_INIT 0)
     set(CMAKE_USE_PTHREADS_INIT 1)
     set(THREADS_PREFER_PTHREAD_FLAG ON)
 
-    # for exception unwinding on macOS
-    # TODO this does not work, which would be the
-    # proper cmake way of doing it, so instead we
-    # use a vanilla option
-    # check_linker_flag(CXX "-Wl,-ld_classic" CSP_USE_LD_CLASSIC_MAC)
-    if(CSP_USE_LD_CLASSIC_MAC)
-      set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -Wl,-ld_classic")
-      set(CMAKE_SHARED_LINKER_FLAGS "${CMAKE_SHARED_LINKER_FLAGS} -Wl,-ld_classic")
-    endif()
-
-    set(CMAKE_OSX_DEPLOYMENT_TARGET "10.13" CACHE STRING "Minimum OS X deployment version")
-
     # don't link against build python
     # https://blog.tim-smith.us/2015/09/python-extension-modules-os-x/
     set(CMAKE_SHARED_LINKER_FLAGS "${CMAKE_SHARED_LINKER_FLAGS} -undefined dynamic_lookup")
-
-    # Support cross build
-    check_c_compiler_flag("-arch x86_64" x86_64Supported)
-    check_c_compiler_flag("-arch arm64" arm64Supported)
-
-    if(x86_64Supported AND arm64Supported)
-        set(CMAKE_OSX_ARCHITECTURES "x86_64;arm64" CACHE STRING "Build universal architecture for OSX" FORCE)
-    elseif(x86_64Supported)
-        set(CMAKE_REQUIRED_LINK_OPTIONS "-arch;x86_64")
-        set(CMAKE_OSX_ARCHITECTURES "x86_64" CACHE STRING "Build universal architecture for OSX" FORCE)
-    elseif(arm64Supported)
-        set(CMAKE_REQUIRED_LINK_OPTIONS "-arch;arm64")
-        set(CMAKE_OSX_ARCHITECTURES "arm64" CACHE STRING "Build universal architecture for OSX" FORCE)
-    endif()
 endif()
 
 
 ###################################################################################################################################################
 # Version Information #
 #######################
 # Set version from cmake and extract latest hash if available
@@ -166,27 +141,24 @@
 endif()
 
 
 ###################################################################################################################################################
 # RPath #
 #########
 if(MACOS)
-    set(CMAKE_INSTALL_RPATH "@loader_path/:@loader_path/../lib")
+    set(CMAKE_INSTALL_RPATH "@loader_path/")
 elseif(LINUX)
-    set(CMAKE_INSTALL_RPATH "\$ORIGIN:\$ORIGIN/../lib")
+    set(CMAKE_INSTALL_RPATH "\$ORIGIN")
 endif()
 
 ###################################################################################################################################################
 # Flags #
 #########
 # Compiler version flags
-if(CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
-    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++17")
-endif()
-
+set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++17")
 
 # Optimization Flags
 if(WIN32)
     if(CMAKE_BUILD_TYPE_LOWER STREQUAL debug)
         set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} \
             /DEBUG \
             /Z7 \
@@ -226,17 +198,21 @@
     else()
         set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} \
         -O3 \
         -g0 \
         -Wall \
         -Wno-deprecated-declarations \
         -Wno-deprecated \
-        -Wno-maybe-uninitialized \
         ")
         add_definitions(-DNDEBUG)
+        if(CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
+            set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} \
+            -Wno-maybe-uninitialized \
+            ")
+        endif()
     endif()
 endif()
 
 # Other Flags
 if(WIN32)
     set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /EHsc /MP /bigobj")
     foreach(warning 4244 4251 4267 4275 4290 4786 4305 4996)
```

### Comparing `csp-0.0.2/LICENSE` & `csp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/MANIFEST.in` & `csp-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/NOTICE` & `csp-0.0.3/NOTICE`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CSP - Copyright 2024 Point72, L.P.
 This project contains software with the below copyrights
 
 
-vcpkg_installed/arm64-osx/share/abseil/copyright
+vcpkg_installed/x64-linux/share/abseil/copyright
 
 
 
                                  Apache License
                            Version 2.0, January 2004
                         https://www.apache.org/licenses/
 
@@ -206,15 +206,15 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 
 
-vcpkg_installed/arm64-osx/share/arrow/copyright
+vcpkg_installed/x64-linux/share/arrow/copyright
 
 
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
@@ -414,85 +414,14 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 --------------------------------------------------------------------------------
 
-src/plasma/fling.cc and src/plasma/fling.h: Apache 2.0
-
-Copyright 2013 Sharvil Nanavati
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
---------------------------------------------------------------------------------
-
-src/plasma/thirdparty/ae: Modified / 3-Clause BSD
-
-Copyright (c) 2006-2010, Salvatore Sanfilippo <antirez at gmail dot com>
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
- * Redistributions of source code must retain the above copyright notice,
-   this list of conditions and the following disclaimer.
- * Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
- * Neither the name of Redis nor the names of its contributors may be used
-   to endorse or promote products derived from this software without
-   specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-
---------------------------------------------------------------------------------
-
-src/plasma/thirdparty/dlmalloc.c: CC0
-
-This is a version (aka dlmalloc) of malloc/free/realloc written by
-Doug Lea and released to the public domain, as explained at
-http://creativecommons.org/publicdomain/zero/1.0/ Send questions,
-comments, complaints, performance data, etc to dl@cs.oswego.edu
-
---------------------------------------------------------------------------------
-
-src/plasma/common.cc (some portions)
-
-Copyright (c) Austin Appleby (aappleby (AT) gmail)
-
-Some portions of this file are derived from code in the MurmurHash project
-
-All code is released to the public domain. For business purposes, Murmurhash is
-under the MIT license.
-
-https://sites.google.com/site/murmurhash/
-
---------------------------------------------------------------------------------
-
 src/arrow/util (some portions): Apache 2.0, and 3-clause BSD
 
 Some portions of this module are derived from code in the Chromium project,
 copyright (c) Google inc and (c) The Chromium Authors and licensed under the
 Apache 2.0 License or the under the 3-clause BSD license:
 
   Copyright (c) 2013 The Chromium Authors. All rights reserved.
@@ -864,42 +793,14 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 --------------------------------------------------------------------------------
 
-The file cpp/src/arrow/vendored/string_view.hpp has the following license
-
-Boost Software License - Version 1.0 - August 17th, 2003
-
-Permission is hereby granted, free of charge, to any person or organization
-obtaining a copy of the software and accompanying documentation covered by
-this license (the "Software") to use, reproduce, display, distribute,
-execute, and transmit the Software, and to prepare derivative works of the
-Software, and to permit third-parties to whom the Software is furnished to
-do so, all subject to the following:
-
-The copyright notices in the Software and this entire statement, including
-the above license grant, this restriction and the following disclaimer,
-must be included in all copies of the Software, in whole or in part, and
-all derivative works of the Software, unless such copies or derivative
-works are solely in the form of machine-executable object code generated by
-a source language processor.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
-SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
-FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
---------------------------------------------------------------------------------
-
 The files in cpp/src/arrow/vendored/xxhash/ have the following license
 (BSD 2-Clause License)
 
 xxHash Library
 Copyright (c) 2012-2014, Yann Collet
 All rights reserved.
 
@@ -2199,25 +2100,14 @@
 --------------------------------------------------------------------------------
 
 Some source code from Ibis (https://github.com/cloudera/ibis) has been adapted
 for PyArrow. Ibis is released under the Apache License, Version 2.0.
 
 --------------------------------------------------------------------------------
 
-This project includes code from the autobrew project.
-
-* r/tools/autobrew and dev/tasks/homebrew-formulae/autobrew/apache-arrow.rb
-  are based on code from the autobrew project.
-
-Copyright (c) 2019, Jeroen Ooms
-License: MIT
-Homepage: https://github.com/jeroen/autobrew
-
---------------------------------------------------------------------------------
-
 dev/tasks/homebrew-formulae/apache-arrow.rb has the following license:
 
 BSD 2-Clause License
 
 Copyright (c) 2009-present, Homebrew contributors
 All rights reserved.
 
@@ -2268,42 +2158,14 @@
 
 3. This notice may not be removed or altered from any source distribution.
 
 René Nyffenegger rene.nyffenegger@adp-gmbh.ch
 
 --------------------------------------------------------------------------------
 
-The file cpp/src/arrow/vendored/optional.hpp has the following license
-
-Boost Software License - Version 1.0 - August 17th, 2003
-
-Permission is hereby granted, free of charge, to any person or organization
-obtaining a copy of the software and accompanying documentation covered by
-this license (the "Software") to use, reproduce, display, distribute,
-execute, and transmit the Software, and to prepare derivative works of the
-Software, and to permit third-parties to whom the Software is furnished to
-do so, all subject to the following:
-
-The copyright notices in the Software and this entire statement, including
-the above license grant, this restriction and the following disclaimer,
-must be included in all copies of the Software, in whole or in part, and
-all derivative works of the Software, unless such copies or derivative
-works are solely in the form of machine-executable object code generated by
-a source language processor.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
-SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
-FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
---------------------------------------------------------------------------------
-
 This project includes code from Folly.
 
  * cpp/src/arrow/vendored/ProducerConsumerQueue.h
 
 is based on Folly's
 
  * folly/Portability.h
@@ -2455,16 +2317,275 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
+--------------------------------------------------------------------------------
+
+The file src/arrow/util/io_util.cc contains code from the CPython project
+which is made available under the Python Software Foundation License Version 2.
+
+--------------------------------------------------------------------------------
+
+3rdparty dependency opentelemetry-cpp is statically linked in certain binary
+distributions. opentelemetry-cpp is made available under the Apache License 2.0.
+
+Copyright The OpenTelemetry Authors
+SPDX-License-Identifier: Apache-2.0
+
+--------------------------------------------------------------------------------
+
+ci/conan/ is based on code from Conan Package and Dependency Manager.
+
+Copyright (c) 2019 Conan.io
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+--------------------------------------------------------------------------------
+
+3rdparty dependency UCX is redistributed as a dynamically linked shared
+library in certain binary distributions. UCX has the following license:
+
+Copyright (c) 2014-2015      UT-Battelle, LLC. All rights reserved.
+Copyright (C) 2014-2020      Mellanox Technologies Ltd. All rights reserved.
+Copyright (C) 2014-2015      The University of Houston System. All rights reserved.
+Copyright (C) 2015           The University of Tennessee and The University
+                             of Tennessee Research Foundation. All rights reserved.
+Copyright (C) 2016-2020      ARM Ltd. All rights reserved.
+Copyright (c) 2016           Los Alamos National Security, LLC. All rights reserved.
+Copyright (C) 2016-2020      Advanced Micro Devices, Inc.  All rights reserved.
+Copyright (C) 2019           UChicago Argonne, LLC.  All rights reserved.
+Copyright (c) 2018-2020      NVIDIA CORPORATION. All rights reserved.
+Copyright (C) 2020           Huawei Technologies Co., Ltd. All rights reserved.
+Copyright (C) 2016-2020      Stony Brook University. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions
+are met:
+
+1. Redistributions of source code must retain the above copyright
+notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright
+notice, this list of conditions and the following disclaimer in the
+documentation and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the names of its
+contributors may be used to endorse or promote products derived from
+this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+--------------------------------------------------------------------------------
+
+The file dev/tasks/r/github.packages.yml contains code from
+
+https://github.com/ursa-labs/arrow-r-nightly
+
+which is made available under the Apache License 2.0.
+
+--------------------------------------------------------------------------------
+.github/actions/sync-nightlies/action.yml  (some portions)
+
+Some portions of this file are derived from code from
+
+https://github.com/JoshPiper/rsync-docker
+
+which is made available under the MIT license
+
+Copyright (c) 2020 Joshua Piper
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+--------------------------------------------------------------------------------
+.github/actions/sync-nightlies/action.yml (some portions)
+
+Some portions of this file are derived from code from
+
+https://github.com/burnett01/rsync-deployments
+
+which is made available under the MIT license
+
+Copyright (c) 2019-2022 Contention
+Copyright (c) 2019-2022 Burnett01
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+vcpkg_installed/x64-linux/share/boost-algorithm/copyright
+
+
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+vcpkg_installed/x64-linux/share/boost-align/copyright
+
+
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+vcpkg_installed/x64-linux/share/boost-array/copyright
+
+
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+vcpkg_installed/x64-linux/share/boost-asio/copyright
+
+
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
 
-vcpkg_installed/arm64-osx/share/boost-algorithm/copyright
+
+vcpkg_installed/x64-linux/share/boost-assert/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2484,15 +2605,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-align/copyright
+vcpkg_installed/x64-linux/share/boost-atomic/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2512,15 +2633,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-array/copyright
+vcpkg_installed/x64-linux/share/boost-bind/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2540,15 +2661,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-assert/copyright
+vcpkg_installed/x64-linux/share/boost-build/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2568,15 +2689,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-atomic/copyright
+vcpkg_installed/x64-linux/share/boost-chrono/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2596,15 +2717,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-bind/copyright
+vcpkg_installed/x64-linux/share/boost-concept-check/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2624,15 +2745,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-build/copyright
+vcpkg_installed/x64-linux/share/boost-config/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2652,15 +2773,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-chrono/copyright
+vcpkg_installed/x64-linux/share/boost-container/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2680,15 +2801,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-concept-check/copyright
+vcpkg_installed/x64-linux/share/boost-container-hash/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2708,15 +2829,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-config/copyright
+vcpkg_installed/x64-linux/share/boost-context/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2736,15 +2857,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-container-hash/copyright
+vcpkg_installed/x64-linux/share/boost-conversion/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2764,15 +2885,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-container/copyright
+vcpkg_installed/x64-linux/share/boost-core/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2792,15 +2913,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-conversion/copyright
+vcpkg_installed/x64-linux/share/boost-coroutine/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2820,15 +2941,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-core/copyright
+vcpkg_installed/x64-linux/share/boost-date-time/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2848,15 +2969,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-date-time/copyright
+vcpkg_installed/x64-linux/share/boost-describe/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2876,15 +2997,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-describe/copyright
+vcpkg_installed/x64-linux/share/boost-detail/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2904,15 +3025,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-detail/copyright
+vcpkg_installed/x64-linux/share/boost-dynamic-bitset/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2932,15 +3053,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-dynamic-bitset/copyright
+vcpkg_installed/x64-linux/share/boost-exception/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2960,15 +3081,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-exception/copyright
+vcpkg_installed/x64-linux/share/boost-filesystem/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -2988,15 +3109,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-filesystem/copyright
+vcpkg_installed/x64-linux/share/boost-functional/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3016,15 +3137,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-function-types/copyright
+vcpkg_installed/x64-linux/share/boost-function/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3044,15 +3165,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-function/copyright
+vcpkg_installed/x64-linux/share/boost-function-types/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3072,15 +3193,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-functional/copyright
+vcpkg_installed/x64-linux/share/boost-fusion/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3100,15 +3221,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-fusion/copyright
+vcpkg_installed/x64-linux/share/boost-integer/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3128,15 +3249,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-integer/copyright
+vcpkg_installed/x64-linux/share/boost-intrusive/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3156,15 +3277,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-intrusive/copyright
+vcpkg_installed/x64-linux/share/boost-io/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3184,15 +3305,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-io/copyright
+vcpkg_installed/x64-linux/share/boost-iterator/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3212,15 +3333,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-iterator/copyright
+vcpkg_installed/x64-linux/share/boost-lexical-cast/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3240,15 +3361,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-lexical-cast/copyright
+vcpkg_installed/x64-linux/share/boost-locale/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3268,15 +3389,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-locale/copyright
+vcpkg_installed/x64-linux/share/boost-math/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3296,15 +3417,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-math/copyright
+vcpkg_installed/x64-linux/share/boost-move/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3324,15 +3445,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-move/copyright
+vcpkg_installed/x64-linux/share/boost-mp11/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3352,15 +3473,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-mp11/copyright
+vcpkg_installed/x64-linux/share/boost-mpl/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3380,15 +3501,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-mpl/copyright
+vcpkg_installed/x64-linux/share/boost-multiprecision/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3408,15 +3529,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-multiprecision/copyright
+vcpkg_installed/x64-linux/share/boost-numeric-conversion/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3436,15 +3557,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-numeric-conversion/copyright
+vcpkg_installed/x64-linux/share/boost-optional/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3464,15 +3585,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-optional/copyright
+vcpkg_installed/x64-linux/share/boost-pool/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3492,15 +3613,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-predef/copyright
+vcpkg_installed/x64-linux/share/boost-predef/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3520,15 +3641,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-preprocessor/copyright
+vcpkg_installed/x64-linux/share/boost-preprocessor/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3548,15 +3669,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-random/copyright
+vcpkg_installed/x64-linux/share/boost-random/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3576,15 +3697,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-range/copyright
+vcpkg_installed/x64-linux/share/boost-range/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3604,15 +3725,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-ratio/copyright
+vcpkg_installed/x64-linux/share/boost-ratio/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3632,15 +3753,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-rational/copyright
+vcpkg_installed/x64-linux/share/boost-rational/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3660,15 +3781,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-regex/copyright
+vcpkg_installed/x64-linux/share/boost-regex/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3688,15 +3809,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-scope-exit/copyright
+vcpkg_installed/x64-linux/share/boost-scope-exit/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3716,15 +3837,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-smart-ptr/copyright
+vcpkg_installed/x64-linux/share/boost-smart-ptr/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3744,15 +3865,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-static-assert/copyright
+vcpkg_installed/x64-linux/share/boost-static-assert/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3772,15 +3893,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-system/copyright
+vcpkg_installed/x64-linux/share/boost-system/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3800,15 +3921,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-thread/copyright
+vcpkg_installed/x64-linux/share/boost-thread/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3828,15 +3949,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-throw-exception/copyright
+vcpkg_installed/x64-linux/share/boost-throw-exception/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3856,15 +3977,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-tokenizer/copyright
+vcpkg_installed/x64-linux/share/boost-tokenizer/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3884,15 +4005,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-tuple/copyright
+vcpkg_installed/x64-linux/share/boost-tuple/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3912,15 +4033,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-type-traits/copyright
+vcpkg_installed/x64-linux/share/boost-typeof/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3940,15 +4061,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-typeof/copyright
+vcpkg_installed/x64-linux/share/boost-type-traits/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3968,15 +4089,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-unordered/copyright
+vcpkg_installed/x64-linux/share/boost-unordered/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -3996,15 +4117,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-utility/copyright
+vcpkg_installed/x64-linux/share/boost-utility/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -4024,15 +4145,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-variant2/copyright
+vcpkg_installed/x64-linux/share/boost-variant2/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -4052,15 +4173,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-vcpkg-helpers/copyright
+vcpkg_installed/x64-linux/share/boost-vcpkg-helpers/copyright
 
 
 Copyright (c) Microsoft Corporation
 
 All rights reserved. 
 
 MIT License
@@ -4080,15 +4201,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/boost-winapi/copyright
+vcpkg_installed/x64-linux/share/boost-winapi/copyright
 
 
 Boost Software License - Version 1.0 - August 17th, 2003
 
 Permission is hereby granted, free of charge, to any person or organization
 obtaining a copy of the software and accompanying documentation covered by
 this license (the "Software") to use, reproduce, display, distribute,
@@ -4108,15 +4229,15 @@
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
 SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
 FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/brotli/copyright
+vcpkg_installed/x64-linux/share/brotli/copyright
 
 
 Copyright (c) 2009, 2010, 2013-2016 by the Brotli Authors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -4132,15 +4253,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/bzip2/copyright
+vcpkg_installed/x64-linux/share/bzip2/copyright
 
 
 
 --------------------------------------------------------------------------
 
 This program, "bzip2", the associated library "libbzip2", and all
 documentation, are copyright (C) 1996-2019 Julian R Seward.  All
@@ -4179,28 +4300,28 @@
 
 Julian Seward, jseward@acm.org
 bzip2/libbzip2 version 1.0.8 of 13 July 2019
 
 --------------------------------------------------------------------------
 
 
-vcpkg_installed/arm64-osx/share/exprtk/copyright
+vcpkg_installed/x64-linux/share/exprtk/copyright
 
 
 Copyright 1999-2022 Arash Partow
 https://www.partow.net/programming/exprtk/index.html
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/gflags/copyright
+vcpkg_installed/x64-linux/share/gflags/copyright
 
 
 Copyright (c) 2006, Google Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
@@ -4225,85 +4346,15 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-vcpkg_installed/arm64-osx/share/glog/copyright
-
-
-Copyright (c) 2008, Google Inc.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-    * Redistributions of source code must retain the above copyright
-notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above
-copyright notice, this list of conditions and the following disclaimer
-in the documentation and/or other materials provided with the
-distribution.
-    * Neither the name of Google Inc. nor the names of its
-contributors may be used to endorse or promote products derived from
-this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-A function gettimeofday in utilities.cc is based on
-
-http://www.google.com/codesearch/p?hl=en#dR3YEbitojA/COPYING&q=GetSystemTimeAsFileTime%20license:bsd
-
-The license of this code is:
-
-Copyright (c) 2003-2008, Jouni Malinen <j@w1.fi> and contributors
-All Rights Reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-
-3. Neither the name(s) of the above-listed copyright holder(s) nor the
-   names of its contributors may be used to endorse or promote products
-   derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-vcpkg_installed/arm64-osx/share/gtest/copyright
+vcpkg_installed/x64-linux/share/gtest/copyright
 
 
 Copyright 2008, Google Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
@@ -4328,15 +4379,15 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-vcpkg_installed/arm64-osx/share/libevent/copyright
+vcpkg_installed/x64-linux/share/libevent/copyright
 
 
 Libevent is available for use under the following license, commonly known
 as the 3-clause (or "modified") BSD license:
 
 ==============================
 Copyright (c) 2000-2007 Niels Provos <provos@citi.umich.edu>
@@ -4484,15 +4535,15 @@
 WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 This file is part of mbed TLS (https://tls.mbed.org)
 
 
-vcpkg_installed/arm64-osx/share/librdkafka/copyright
+vcpkg_installed/x64-linux/share/librdkafka/copyright
 
 
 LICENSE
 --------------------------------------------------------------
 librdkafka - Apache Kafka C driver library
 
 Copyright (c) 2012-2020, Magnus Edenhill
@@ -4881,15 +4932,15 @@
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
  * POSSIBILITY OF SUCH DAMAGE.
  */
 
 
 
 
-vcpkg_installed/arm64-osx/share/lz4/copyright
+vcpkg_installed/x64-linux/share/lz4/copyright
 
 
 LZ4 Library
 Copyright (c) 2011-2020, Yann Collet
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
@@ -4910,15 +4961,15 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-vcpkg_installed/arm64-osx/share/openssl/copyright
+vcpkg_installed/x64-linux/share/openssl/copyright
 
 
 
                                  Apache License
                            Version 2.0, January 2004
                         https://www.apache.org/licenses/
 
@@ -5092,15 +5143,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
 
-vcpkg_installed/arm64-osx/share/protobuf/copyright
+vcpkg_installed/x64-linux/share/protobuf/copyright
 
 
 Copyright 2008 Google Inc.  All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
@@ -5129,15 +5180,15 @@
 
 Code generated by the Protocol Buffer compiler is owned by the owner
 of the input file used when generating it.  This code is not
 standalone and requires a support library to be linked with it.  This
 support library is itself covered by the above license.
 
 
-vcpkg_installed/arm64-osx/share/rapidjson/copyright
+vcpkg_installed/x64-linux/share/rapidjson/copyright
 
 
 Tencent is pleased to support the open source community by making RapidJSON available. 
  
 Copyright (C) 2015 THL A29 Limited, a Tencent company, and Milo Yip.  All rights reserved.
 
 If you have downloaded a copy of the RapidJSON binary from Tencent, please note that the RapidJSON binary is licensed under the MIT License.
@@ -5191,15 +5242,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/re2/copyright
+vcpkg_installed/x64-linux/share/re2/copyright
 
 
 // Copyright (c) 2009 The RE2 Authors. All rights reserved.
 //
 // Redistribution and use in source and binary forms, with or without
 // modification, are permitted provided that the following conditions are
 // met:
@@ -5223,15 +5274,15 @@
 // LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 // DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 // THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 // (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 // OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-vcpkg_installed/arm64-osx/share/snappy/copyright
+vcpkg_installed/x64-linux/share/snappy/copyright
 
 
 Copyright 2011, Google Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
@@ -5282,15 +5333,15 @@
  - alice29.txt, asyoulik.txt, plrabn12.txt and lcet10.txt are from Project
    Gutenberg. The first three have expired copyrights and are in the public
    domain; the latter does not have expired copyright, but is still in the
    public domain according to the license information
    (http://www.gutenberg.org/ebooks/53).
 
 
-vcpkg_installed/arm64-osx/share/thrift/copyright
+vcpkg_installed/x64-linux/share/thrift/copyright
 
 
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
@@ -5593,15 +5644,15 @@
 
  * Copyright (c) 2008- Patrick Collison <patrick@collison.ie>
  * Copyright (c) 2006- Facebook
 
 ---------------------------------------------------
 
 
-vcpkg_installed/arm64-osx/share/utf8proc/copyright
+vcpkg_installed/x64-linux/share/utf8proc/copyright
 
 
 ## utf8proc license ##
 
 **utf8proc** is a software package originally developed
 by Jan Behrens and the rest of the Public Software Group, who
 deserve nearly all of the credit for this library, that is now maintained by the Julia-language developers.  Like the original utf8proc,
@@ -5691,15 +5742,15 @@
 authorization of the copyright holder.
 
 Unicode and the Unicode logo are trademarks of Unicode, Inc., and may be
 registered in some jurisdictions. All other trademarks and registered
 trademarks mentioned herein are the property of their respective owners.
 
 
-vcpkg_installed/arm64-osx/share/vcpkg-cmake-config/copyright
+vcpkg_installed/x64-linux/share/vcpkg-cmake-config/copyright
 
 
 Copyright (c) Microsoft Corporation
 
 All rights reserved. 
 
 MIT License
@@ -5719,15 +5770,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/vcpkg-cmake-get-vars/copyright
+vcpkg_installed/x64-linux/share/vcpkg-cmake/copyright
 
 
 MIT License
 
 Copyright (c) Microsoft Corporation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this
@@ -5744,15 +5795,15 @@
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/vcpkg-cmake/copyright
+vcpkg_installed/x64-linux/share/vcpkg-cmake-get-vars/copyright
 
 
 MIT License
 
 Copyright (c) Microsoft Corporation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this
@@ -5769,15 +5820,199 @@
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-vcpkg_installed/arm64-osx/share/zlib/copyright
+vcpkg_installed/x64-linux/share/websocketpp/copyright
+
+
+Main Library:
+
+Copyright (c) 2014, Peter Thorson. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of the WebSocket++ Project nor the
+      names of its contributors may be used to endorse or promote products
+      derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL PETER THORSON BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Bundled Libraries:
+
+****** Base 64 Library (base64/base64.hpp) ******
+base64.hpp is a repackaging of the base64.cpp and base64.h files into a
+single header suitable for use as a header only library. This conversion was
+done by Peter Thorson (webmaster@zaphoyd.com) in 2012. All modifications to
+the code are redistributed under the same license as the original, which is
+listed below.
+
+base64.cpp and base64.h
+
+Copyright (C) 2004-2008 René Nyffenegger
+
+This source code is provided 'as-is', without any express or implied
+warranty. In no event will the author be held liable for any damages
+arising from the use of this software.
+
+Permission is granted to anyone to use this software for any purpose,
+including commercial applications, and to alter it and redistribute it
+freely, subject to the following restrictions:
+
+1. The origin of this source code must not be misrepresented; you must not
+  claim that you wrote the original source code. If you use this source code
+  in a product, an acknowledgment in the product documentation would be
+  appreciated but is not required.
+
+2. Altered source versions must be plainly marked as such, and must not be
+  misrepresented as being the original source code.
+
+3. This notice may not be removed or altered from any source distribution.
+
+René Nyffenegger rene.nyffenegger@adp-gmbh.ch
+
+****** SHA1 Library (sha1/sha1.hpp) ******
+sha1.hpp is a repackaging of the sha1.cpp and sha1.h files from the shallsha1
+library (http://code.google.com/p/smallsha1/) into a single header suitable for
+use as a header only library. This conversion was done by Peter Thorson
+(webmaster@zaphoyd.com) in 2013. All modifications to the code are redistributed
+under the same license as the original, which is listed below.
+
+ Copyright (c) 2011, Micael Hildenborg
+ All rights reserved.
+
+ Redistribution and use in source and binary forms, with or without
+ modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of Micael Hildenborg nor the
+      names of its contributors may be used to endorse or promote products
+      derived from this software without specific prior written permission.
+
+ THIS SOFTWARE IS PROVIDED BY Micael Hildenborg ''AS IS'' AND ANY
+ EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+ WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+ DISCLAIMED. IN NO EVENT SHALL Micael Hildenborg BE LIABLE FOR ANY
+ DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+ (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+ LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+ (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+ SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+****** MD5 Library (common/md5.hpp) ******
+md5.hpp is a reformulation of the md5.h and md5.c code from
+http://www.opensource.apple.com/source/cups/cups-59/cups/md5.c to allow it to
+function as a component of a header only library. This conversion was done by
+Peter Thorson (webmaster@zaphoyd.com) in 2012 for the WebSocket++ project. The
+changes are released under the same license as the original (listed below)
+
+Copyright (C) 1999, 2002 Aladdin Enterprises.  All rights reserved.
+
+This software is provided 'as-is', without any express or implied
+warranty.  In no event will the authors be held liable for any damages
+arising from the use of this software.
+
+Permission is granted to anyone to use this software for any purpose,
+including commercial applications, and to alter it and redistribute it
+freely, subject to the following restrictions:
+
+1. The origin of this software must not be misrepresented; you must not
+ claim that you wrote the original software. If you use this software
+ in a product, an acknowledgment in the product documentation would be
+ appreciated but is not required.
+2. Altered source versions must be plainly marked as such, and must not be
+ misrepresented as being the original software.
+3. This notice may not be removed or altered from any source distribution.
+
+L. Peter Deutsch
+ghost@aladdin.com
+
+****** UTF8 Validation logic (utf8_validation.hpp) ******
+utf8_validation.hpp is adapted from code originally written by Bjoern Hoehrmann
+<bjoern@hoehrmann.de>. See http://bjoern.hoehrmann.de/utf-8/decoder/dfa/ for
+details.
+
+The original license:
+
+Copyright (c) 2008-2009 Bjoern Hoehrmann <bjoern@hoehrmann.de>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+vcpkg_installed/x64-linux/share/xsimd/copyright
+
+
+Copyright (c) 2016, Johan Mabille, Sylvain Corlay, Wolf Vollprecht and Martin Renou
+Copyright (c) 2016, QuantStack
+Copyright (c) 2018, Serge Guelton
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
+vcpkg_installed/x64-linux/share/zlib/copyright
 
 
 Copyright notice:
 
  (C) 1995-2022 Jean-loup Gailly and Mark Adler
 
   This software is provided 'as-is', without any express or implied
@@ -5796,15 +6031,15 @@
      misrepresented as being the original software.
   3. This notice may not be removed or altered from any source distribution.
 
   Jean-loup Gailly        Mark Adler
   jloup@gzip.org          madler@alumni.caltech.edu
 
 
-vcpkg_installed/arm64-osx/share/zstd/copyright
+vcpkg_installed/x64-linux/share/zstd/copyright
 
 
 ZSTD is dual licensed under BSD and GPLv2.
 
 LICENSE:
 
 BSD License
@@ -6179,15 +6414,15 @@
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
 
 
 
-vcpkg_installed/arm64-osx/tools/boost-build/src/engine/debian/copyright
+vcpkg_installed/x64-linux/tools/boost-build/src/engine/debian/copyright
 
 
 This package was debianized by Vladimir Prus <ghost@cs.msu.su> on
 Wed, 17 July 2002, 19:27:00 +0400.
 
 Copyright:
```

### Comparing `csp-0.0.2/PKG-INFO` & `csp-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp
-Version: 0.0.2
+Version: 0.0.3
 Summary: csp is a high performance reactive stream processing library, written in C++ and Python
 Author-email: the csp authors <CSPOpenSource@point72.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `csp-0.0.2/README.md` & `csp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindBrotli.cmake` & `csp-0.0.3/cpp/cmake/modules/FindBrotli.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindCSP.cmake` & `csp-0.0.3/cpp/cmake/modules/FindCSP.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # CSP_ENGINE_LIBRARY
 # CSP_TYPES_LIBRARY
 # CSP_TYPES_STATIC_LIBRARY
 # CSP_BASELIB_LIBARY
 # CSP_BASELIB_STATIC_LIBRARY
 # CSP_BASKETLIB_LIBRARY
 # CSP_BASKETLIB_STATIC_LIBRARY
+# CSP_TESTLIB_LIBRARY
+# CSP_MATH_LIBRARY
+# CSP_MATH_STATIC_LIBRARY
 # CSP_STATS_LIBRARY
 # CSP_STATS_STATIC_LIBRARY
 # CSP_NPSTATS_LIBRARY
 # CSP_ADAPTER_UTILS_LIBRARY
 # CSP_KAFKAADAPTER_LIBRARY
 # CSP_KAFKAADAPTER_STATIC_LIBRARY
 # CSP_PARQUETADAPTER_LIBRARY
@@ -68,14 +71,19 @@
 
 find_library(CSP_BASELIB_LIBARY NAMES _cspbaselibimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 find_library(CSP_BASELIB_STATIC_LIBRARY NAMES libbaselibimpl_static.a PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 
 find_library(CSP_BASKETLIB_LIBRARY NAMES _cspbasketlibimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 find_library(CSP_BASKETLIB_STATIC_LIBRARY NAMES libbasketlibimpl_static.a PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 
+find_library(CSP_TESTLIB_LIBRARY NAMES _csptestlibimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
+
+find_library(CSP_MATH_LIBRARY NAMES _cspmathimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
+find_library(CSP_MATH_STATIC_LIBRARY NAMES libmathimpl_static.a PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
+
 find_library(CSP_STATS_LIBRARY NAMES _cspstatsimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 find_library(CSP_STATS_STATIC_LIBRARY NAMES libstatsimpl_static.a PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 
 find_library(CSP_NPSTATS_LIBRARY NAMES _cspnpstatsimpl.so PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
 
 find_library(CSP_ADAPTER_UTILS_LIBRARY NAMES libcsp_adapter_utils_static.a PATHS "${__csp_lib_path}" NO_DEFAULT_PATH)
```

### Comparing `csp-0.0.2/cpp/cmake/modules/FindGRPC.cmake` & `csp-0.0.3/cpp/cmake/modules/FindGRPC.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindNumpy.cmake` & `csp-0.0.3/cpp/cmake/modules/FindNumpy.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindPyArrow.cmake` & `csp-0.0.3/cpp/cmake/modules/FindPyArrow.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindPythonHeaders.cmake` & `csp-0.0.3/cpp/cmake/modules/FindPythonHeaders.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/FindRdKafka.cmake` & `csp-0.0.3/cpp/cmake/modules/FindRdKafka.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/cmake/modules/Findcsp_autogen.cmake` & `csp-0.0.3/cpp/cmake/modules/Findcsp_autogen.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     if(ARGV4)
         set(CSP_AUTOGEN_EXTRA_ARGS "${ARGV4}")
     else()
         set(CSP_AUTOGEN_EXTRA_ARGS "")
     endif()
 
     add_custom_command(OUTPUT  "${CMAKE_CURRENT_BINARY_DIR}/csp_autogen/${DEST_FILENAME}.cpp" "${CMAKE_CURRENT_BINARY_DIR}/csp_autogen/${DEST_FILENAME}.h"
-        COMMAND ${CMAKE_COMMAND} -E env "PYTHONPATH=${PROJECT_BINARY_DIR}/lib:${CMAKE_SOURCE_DIR}:ext:$$PYTHONPATH" "LD_LIBRARY_PATH=${PROJECT_BINARY_DIR}/lib:$$LD_LIBRARY_PATH}" ${Python_EXECUTABLE} ${CSP_AUTOGEN} -m ${MODULE_NAME} -d ${CMAKE_CURRENT_BINARY_DIR}/csp_autogen -o ${DEST_FILENAME} ${CSP_AUTOGEN_EXTRA_ARGS}
+        COMMAND ${CMAKE_COMMAND} -E env "PYTHONPATH=${PROJECT_BINARY_DIR}/lib:${CMAKE_SOURCE_DIR}:$$PYTHONPATH" "LD_LIBRARY_PATH=${PROJECT_BINARY_DIR}/lib:$$LD_LIBRARY_PATH}" ${Python_EXECUTABLE} ${CSP_AUTOGEN} -m ${MODULE_NAME} -d ${CMAKE_CURRENT_BINARY_DIR}/csp_autogen -o ${DEST_FILENAME} ${CSP_AUTOGEN_EXTRA_ARGS}
             COMMENT "generating csp c++ types from module ${MODULE_NAME} ${PROJECT_BINARY_DIR} ${CSP_AUTOGEN}"
             DEPENDS mkdir_autogen_${MODULE_NAME} ${CMAKE_SOURCE_DIR}/${MODULE_FILENAME})
 
     set(${SOURCE_NAME_OUTVAR} "${CMAKE_CURRENT_BINARY_DIR}/csp_autogen/${DEST_FILENAME}.cpp" PARENT_SCOPE )
     set(${HEADER_NAME_OUTVAR} "${CMAKE_CURRENT_BINARY_DIR}/csp_autogen/${DEST_FILENAME}.h" PARENT_SCOPE )
 endfunction()
```

### Comparing `csp-0.0.2/cpp/cmake/modules/Findutf8proc.cmake` & `csp-0.0.3/cpp/cmake/modules/Findutf8proc.cmake`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/CMakeLists.txt` & `csp-0.0.3/cpp/csp/adapters/kafka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaAdapterManager.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaAdapterManager.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaAdapterManager.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaAdapterManager.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaConsumer.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaConsumer.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaConsumer.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaConsumer.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaInputAdapter.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaInputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaInputAdapter.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaOutputAdapter.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaOutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaOutputAdapter.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaOutputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaPublisher.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaPublisher.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaPublisher.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaPublisher.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaSubscriber.cpp` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaSubscriber.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/kafka/KafkaSubscriber.h` & `csp-0.0.3/cpp/csp/adapters/kafka/KafkaSubscriber.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileReaderWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ArrowIPCFileWriterWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ArrowSingleColumnArrayBuilder.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ArrowSingleColumnArrayBuilder.h`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 {
 public:
     using BaseTypedArrayBuilder<ValueType, ArrowBuilderType>::BaseTypedArrayBuilder;
 
 protected:
     void pushValueToArray()
     {
-        this -> m_builderPtr -> Append( *this -> m_value );
+        [[maybe_unused]] auto status = this -> m_builderPtr -> Append( *this -> m_value );        
     }
 };
 
 class StringArrayBuilder : public BaseTypedArrayBuilder<std::string, arrow::StringBuilder>
 {
 public:
     using BaseTypedArrayBuilder<std::string, arrow::StringBuilder>::BaseTypedArrayBuilder;
```

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/CMakeLists.txt` & `csp-0.0.3/cpp/csp/adapters/parquet/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/DialectGenericListReaderInterface.h` & `csp-0.0.3/cpp/csp/adapters/parquet/DialectGenericListReaderInterface.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/DialectGenericListWriterInterface.h` & `csp-0.0.3/cpp/csp/adapters/parquet/DialectGenericListWriterInterface.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileReaderWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/FileReaderWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileReaderWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/FileReaderWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapperContainer.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapperContainer.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/FileWriterWrapperContainer.h` & `csp-0.0.3/cpp/csp/adapters/parquet/FileWriterWrapperContainer.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetDictBasketOutputWriter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileReaderWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetFileWriterWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetInputAdapterManager.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetInputAdapterManager.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetInputAdapterManager.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetInputAdapterManager.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapter.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapter.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 {
 public:
     ParquetOutputHandler( ParquetWriter &parquetWriter, CspTypePtr &type )
             : m_type( type ), m_parquetWriter( parquetWriter )
     {
     }
 
+    virtual ~ParquetOutputHandler() {}
+
     uint32_t getChunkSize() const;
 
     virtual uint32_t getNumColumns() = 0;
     virtual std::shared_ptr<ArrowSingleColumnArrayBuilder> getColumnArrayBuilder( unsigned index ) = 0;
     virtual void writeValueFromTs( const TimeSeriesProvider *input ) = 0;
 
 protected:
```

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputAdapterManager.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetOutputFilenameAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetReader.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetReader.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetReader.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetReader.h`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         m_columnSubscriptionContainer.m_scalarColumnSubscriptions[column].push_back(ColumnSubscriberInfo{inputAdapter, symbol});
     }
 
     virtual void addListSubscriber( const std::string &column, ManagedSimInputAdapter *inputAdapter,
                                     const std::optional<utils::Symbol> &symbol, const DialectGenericListReaderInterface::Ptr &listReaderInterface ) override
     {
         ParquetReader::addListSubscriber( column, inputAdapter, symbol, listReaderInterface);
-        m_columnSubscriptionContainer.m_listColumnSubscriptions[column].push_back(ListColumnSubscriberInfo{inputAdapter, symbol, listReaderInterface});
+        m_columnSubscriptionContainer.m_listColumnSubscriptions[column].push_back(ListColumnSubscriberInfo{{inputAdapter, symbol}, listReaderInterface});
     }
 
 protected:
     void init();
     void setColumnAdaptersFromCurrentTable();
     virtual bool openNextFile() = 0;
     virtual bool readNextRowGroup() = 0;
```

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetReaderColumnAdapter.h`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     bool isNativeType() const override
     {
         CSP_THROW( csp::RuntimeException, "Trying to check type of a missing column " << getColumnName() );
     }
 
     bool isMissingColumn() const override{ return true; }
 
-    virtual CspTypePtr getNativeCspType() const
+    virtual CspTypePtr getNativeCspType() const override
     {
         CSP_THROW( csp::RuntimeException, "Trying to get native type of a missing column " << getColumnName() );
     }
 
     virtual void handleNewBatch( const std::shared_ptr<::arrow::ChunkedArray> &data ) override
     {
         CSP_THROW( csp::RuntimeException, "Trying to handle new batch for a missing column " << getColumnName() );
@@ -186,16 +186,15 @@
     std::optional<ValueType>        m_curValue;
 };
 
 template< typename ValueType, typename ArrowArrayType >
 class NativeTypeColumnAdapter : public BaseTypedColumnAdapter<ValueType, ArrowArrayType>
 {
 public:
-    using BASE = BaseTypedColumnAdapter<ValueType, ArrowArrayType>;
-    using BASE::BaseTypedColumnAdapter;
+    using BaseTypedColumnAdapter<ValueType, ArrowArrayType>::BaseTypedColumnAdapter;
     virtual CspTypePtr getNativeCspType() const override {return CspType::fromCType<ValueType>::type();}
 
 protected:
     void readCurValue() override;
 };
 
 template< long UNIT >
```

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetStatusUtils.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetStatusUtils.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetWriter.cpp` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetWriter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/parquet/ParquetWriter.h` & `csp-0.0.3/cpp/csp/adapters/parquet/ParquetWriter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/CMakeLists.txt` & `csp-0.0.3/cpp/csp/adapters/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/FileUtils.h` & `csp-0.0.3/cpp/csp/adapters/utils/FileUtils.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/JSONMessageStructConverter.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/JSONMessageStructConverter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -134,30 +134,31 @@
                 nestedEntry.sField -> setValue( struct_.get(), convertJSON( jit -> name.GetString(), *nestedEntry.sField -> type(), nestedEntry, jValue, static_cast<T*>( nullptr ) ) );
             } );
     }
 
     return struct_;
 }
 
-template<typename T>
-std::vector<T> JSONMessageStructConverter::convertJSON( const char * fieldname, const CspType & type, const FieldEntry &, const rapidjson::Value & jValue, std::vector<T> * x )
+template<typename StorageT>
+std::vector<StorageT> JSONMessageStructConverter::convertJSON( const char * fieldname, const CspType & type, const FieldEntry &, const rapidjson::Value & jValue, std::vector<StorageT> * x )
 {
     if( !jValue.IsArray() )
         CSP_THROW( TypeError, "expected ARRAY type for json field " << fieldname );
 
     auto jArray = jValue.GetArray();
 
     const CspType & elemType = *static_cast<const CspArrayType &>( type ).elemType();
 
-    std::vector<T> out;
+    using ElemT = typename CspType::Type::toCArrayElemType<StorageT>::type;
+    std::vector<StorageT> out;
     out.reserve( jArray.Size() );
     for( auto & v : jArray )
     {
         //note that we dont pass FieldEntry to convert here, this doesnt support arrays of structs
-        out.emplace_back( convertJSON( fieldname, elemType, {}, v, ( T * ) nullptr) );
+        out.emplace_back( convertJSON( fieldname, elemType, {}, v, ( ElemT * ) nullptr) );
     }
 
     return out;
 }
 
 JSONMessageStructConverter::JSONMessageStructConverter( const CspTypePtr & type,
                                                         const Dictionary & properties ) : MessageStructConverter( type, properties )
```

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/JSONMessageStructConverter.h` & `csp-0.0.3/cpp/csp/adapters/utils/JSONMessageStructConverter.h`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
     template<typename T>
     T convertJSON( const char * fieldname, const CspType & type, const FieldEntry & entry, const rapidjson::Value & v, T * foo )
     {
         return convertJSON( fieldname, v, foo );
     }
 
-    template<typename T>
-    std::vector<T> convertJSON( const char * fieldname, const CspType & type, const FieldEntry & entry, const rapidjson::Value & v, std::vector<T> * );
+    template<typename StorageT>
+    std::vector<StorageT> convertJSON( const char * fieldname, const CspType & type, const FieldEntry & entry, const rapidjson::Value & v, std::vector<StorageT> * );
 
     
     Fields           m_fields;
     DateTimeWireType m_datetimeType;
     std::list<std::string> m_jsonkeys; //intentionally stored as list so they dont invalidate on push
 };
```

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/JSONMessageWriter.h` & `csp-0.0.3/cpp/csp/adapters/utils/JSONMessageWriter.h`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         m_doc.GetAllocator().Clear();
         m_doc.SetObject();
 
         return {m_stringBuffer.GetString(),m_stringBuffer.GetSize()};
     }
 
 private:
-    void processTickImpl( const OutputDataMapper & dataMapper, const TimeSeriesProvider * sourcets )
+    void processTickImpl( const OutputDataMapper & dataMapper, const TimeSeriesProvider * sourcets ) override
     {
         dataMapper.apply( *this, sourcets );
     }
 
     template<typename T>
     inline auto convertValue( const T & value )
     { 
@@ -77,16 +77,16 @@
     template<typename T>
     inline auto convertValue( const T & value, const CspType & type, const FieldEntry & entry )
     {
         return convertValue( value );
     }
 
 
-    template<typename T>
-    auto convertValue( const std::vector<T> & value, const CspType & type, const FieldEntry & entry );
+    template<typename StorageT>
+    auto convertValue( const std::vector<StorageT> & value, const CspType & type, const FieldEntry & entry );
 
     rapidjson::Document     m_doc;
     rapidjson::StringBuffer m_stringBuffer;
     utils::DateTimeWireType m_datetimeWireType;
 };
 
 template<>
@@ -128,28 +128,30 @@
 
 template<>
 inline auto JSONMessageWriter::convertValue( const csp::CspEnum & value, const CspType & type, const FieldEntry & entry )
 {
     return rapidjson::StringRef( value.name().c_str() );
 }
 
-template<typename T>
-inline auto JSONMessageWriter::convertValue( const std::vector<T> & value, const CspType & type, const FieldEntry & entry )
+template<typename StorageT>
+inline auto JSONMessageWriter::convertValue( const std::vector<StorageT> & value, const CspType & type, const FieldEntry & entry )
 {
     auto & allocator = m_doc.GetAllocator();
     rapidjson::Value array( rapidjson::kArrayType );
     size_t sz = value.size();
 
     const CspType & elemType = *static_cast<const CspArrayType &>( type ).elemType();
 
+    using ElemT = typename CspType::Type::toCArrayElemType<StorageT>::type;
+
     //iterating by index for vector<bool> support
     for( size_t index = 0; index < sz; ++index )
     {
         //Note this passes an empty FieldEntry / wont work on vector of structs
-        array.PushBack( convertValue( value[index], elemType, {} ), allocator );
+        array.PushBack( convertValue<ElemT>( value[index], elemType, {} ), allocator );
     }
     return array;
 }
 
 template<>
 inline auto JSONMessageWriter::convertValue( const StructPtr & struct_, const CspType & type, const FieldEntry & entry )
 {
```

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/MessageEnums.h` & `csp-0.0.3/cpp/csp/adapters/utils/MessageEnums.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/MessageStructConverter.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/MessageStructConverter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/MessageStructConverter.h` & `csp-0.0.3/cpp/csp/adapters/utils/MessageStructConverter.h`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 namespace csp::adapters::utils
 {
 
 class MessageStructConverter
 {
 public:
     MessageStructConverter( const CspTypePtr & type, const Dictionary & properties );
+    virtual ~MessageStructConverter() {}
+    
     virtual csp::StructPtr asStruct( void * bytes, size_t size ) = 0;
 
     virtual MsgProtocol protocol() const = 0;
 
     StructMetaPtr structMeta() { return m_structMeta; }
 
 protected:
```

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/MessageWriter.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/MessageWriter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/MessageWriter.h` & `csp-0.0.3/cpp/csp/adapters/utils/MessageWriter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/ProtobufHelper.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/ProtobufHelper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -364,20 +364,21 @@
             case CspType::Type::ARRAY:
             {
                 int count = protoAccess -> FieldSize( protoMsg, pField );
 
                 auto elemType = static_cast<const CspArrayType &>( *sField -> type() ).elemType();
                 SupportedArrayCspTypeSwitch::invoke( elemType.get(), [&count,&protoMsg,&pField,&sField,&struct_]( auto tag )
                                                      {
-                                                         using T = typename decltype(tag)::type;
-                                                         std::vector<T> data;
+                                                         using ElemT    = typename decltype(tag)::type;
+                                                         using StorageT = typename CspType::Type::toCArrayStorageType<ElemT>::type;
+                                                         std::vector<StorageT> data;
                                                          data.reserve( count );
                                                          for( int i = 0; i < count; ++i )
-                                                             data.emplace_back( extractRepeatedValue<T>( protoMsg, pField, i ) );
-                                                         sField -> setValue<std::vector<T>>( struct_.get(), std::move( data ) );
+                                                             data.emplace_back( extractRepeatedValue<ElemT>( protoMsg, pField, i ) );
+                                                         sField -> setValue<std::vector<StorageT>>( struct_.get(), std::move( data ) );
                                                      } );
                 break;
             }
 
             default:
                 CSP_THROW( TypeError, "Struct field type " << sField -> type() -> type() << " not currently mappable to proto field" );
         }
```

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/ProtobufHelper.h` & `csp-0.0.3/cpp/csp/adapters/utils/ProtobufHelper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/ProtobufMessageStructConverter.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/ProtobufMessageStructConverter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/ProtobufMessageStructConverter.h` & `csp-0.0.3/cpp/csp/adapters/utils/ProtobufMessageStructConverter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/RawBytesMessageStructConverter.cpp` & `csp-0.0.3/cpp/csp/adapters/utils/RawBytesMessageStructConverter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/RawBytesMessageStructConverter.h` & `csp-0.0.3/cpp/csp/adapters/utils/RawBytesMessageStructConverter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/StructAdapterInfo.h` & `csp-0.0.3/cpp/csp/adapters/utils/StructAdapterInfo.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/adapters/utils/ValueDispatcher.h` & `csp-0.0.3/cpp/csp/adapters/utils/ValueDispatcher.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/BasicAllocator.h` & `csp-0.0.3/cpp/csp/core/BasicAllocator.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/CMakeLists.txt` & `csp-0.0.3/cpp/csp/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/DynamicBitSet.h` & `csp-0.0.3/cpp/csp/core/DynamicBitSet.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Enum.h` & `csp-0.0.3/cpp/csp/core/Enum.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/EnumBitSet.h` & `csp-0.0.3/cpp/csp/core/EnumBitSet.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Exception.cpp` & `csp-0.0.3/cpp/csp/core/Exception.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Exception.h` & `csp-0.0.3/cpp/csp/core/Exception.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/FileUtils.h` & `csp-0.0.3/cpp/csp/core/FileUtils.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Generator.h` & `csp-0.0.3/cpp/csp/core/Generator.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Hash.h` & `csp-0.0.3/cpp/csp/core/Hash.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/QueueWaiter.h` & `csp-0.0.3/cpp/csp/core/QueueWaiter.h`

 * *Files 14% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     }
 
     bool wait( TimeDelta maxWaitTime )
     {
         std::unique_lock<std::mutex> lock( m_lock );
         bool rv = false;
         if( !m_eventsPending && maxWaitTime.asNanoseconds() > 0 )
-        {
-            rv = ( m_condition.wait_for( lock, std::chrono::nanoseconds( maxWaitTime.asNanoseconds() ) ) == std::cv_status::no_timeout );
-        }
-        m_eventsPending = false;
+            rv = m_condition.wait_for( lock, std::chrono::nanoseconds( maxWaitTime.asNanoseconds() ), [this]() { return m_eventsPending; } );
+
+        if( rv )
+            m_eventsPending = false;
         return rv;
     }
 
 private:
     std::mutex              m_lock;
     std::condition_variable m_condition;
     bool                    m_eventsPending;
```

### Comparing `csp-0.0.2/cpp/csp/core/SRMWLockFreeQueue.h` & `csp-0.0.3/cpp/csp/core/SRMWLockFreeQueue.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/System.h` & `csp-0.0.3/cpp/csp/core/System.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/TaggedPointerUnion.h` & `csp-0.0.3/cpp/csp/core/TaggedPointerUnion.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Time.cpp` & `csp-0.0.3/cpp/csp/core/Time.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/core/Time.h` & `csp-0.0.3/cpp/csp/core/Time.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/cppnodes/CMakeLists.txt` & `csp-0.0.3/cpp/csp/cppnodes/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/cppnodes/baselibimpl.cpp` & `csp-0.0.3/cpp/csp/cppnodes/baselibimpl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
     INVOKE()
     {
         //single switch up front, no need to do it multiple times
         switchCspType( elemType, [this]( auto tag )
         {
             using ElemT  = typename decltype(tag)::type;
-            using ArrayT = typename CspType::Type::toCType<CspType::Type::ARRAY,ElemT>::type;
+            using ArrayT = typename CspType::Type::toCArrayType<ElemT>::type;
 
             if( csp.ticked( x ) )
             {
                 auto & v = x.lastValue<ArrayT>();
                 size_t sz = v.size();
                 if( likely( sz > 0 ) )
                 {
@@ -442,15 +442,15 @@
     INVOKE()
     {
         //single switch up front, no need to do it multiple times
         //we expect all elements to be of the same type
         switchCspType( elemType, [this]( auto tag )
                        {
                            using ElemT  = typename decltype(tag)::type;
-                           using ArrayT = typename CspType::Type::toCType<CspType::Type::ARRAY,ElemT>::type;
+                           using ArrayT = typename CspType::Type::toCArrayType<ElemT>::type;
 
                            ArrayT & out = unnamed_output().reserveSpace<ArrayT>();
                            out.clear();
                            for( auto it = x.tickedinputs(); it; ++it )
                                out.emplace_back( it -> lastValueTyped<ElemT>() );
                        } );
     }
```

### Comparing `csp-0.0.2/cpp/csp/cppnodes/basketlibimpl.cpp` & `csp-0.0.3/cpp/csp/cppnodes/basketlibimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/cppnodes/mathimpl.cpp` & `csp-0.0.3/cpp/csp/cppnodes/mathimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/cppnodes/statsimpl.cpp` & `csp-0.0.3/cpp/csp/cppnodes/statsimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/cppnodes/statsimpl.h` & `csp-0.0.3/cpp/csp/cppnodes/statsimpl.h`

 * *Files 0% similar despite different names*

```diff
@@ -1159,15 +1159,15 @@
                 return std::numeric_limits<double>::quiet_NaN();
             }
 
             double target = std::get<double>( m_quants[index]._data ) * ( m_tree.size() - 1 );
             int ft = floor( target );
             int ct = ceil( target );
 
-            double qtl;
+            double qtl = 0.0;
         #ifndef __clang__
             switch ( m_interpolation )
             {
                 case LINEAR:
                     if( ft == target )
                     {
                         qtl = *m_tree.find_by_order( ft );
```

### Comparing `csp-0.0.2/cpp/csp/engine/AdapterManager.cpp` & `csp-0.0.3/cpp/csp/engine/AdapterManager.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                                                 AdapterManager *manager,
                                                 PushMode pushMode ) : InputAdapter( engine, type, pushMode ),
                                                                       m_manager( manager ),
                                                                       m_lastCycleCount( 0 )
 {
 }
 
-AdapterManager::AdapterManager( csp::Engine * engine ) : m_engine( engine ), m_statusAdapter( nullptr )
+AdapterManager::AdapterManager( csp::Engine * engine ) : m_engine( engine ), m_statusAdapter( nullptr ), m_started( false )
 {
     if( !m_engine -> isRootEngine() )
         CSP_THROW( NotImplemented, "AdapterManager support is not currently available in dynamic graphs" );
 }
 
 AdapterManager::~AdapterManager()
 {
```

### Comparing `csp-0.0.2/cpp/csp/engine/AdapterManager.h` & `csp-0.0.3/cpp/csp/engine/AdapterManager.h`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,17 @@
     const Engine * engine() const   { return m_engine; }
 
     RootEngine * rootEngine()             { return m_engine -> rootEngine(); }
     const RootEngine * rootEngine() const { return m_engine -> rootEngine(); }
 
     DateTime starttime() const      { return m_starttime; }
     DateTime endtime() const        { return m_endtime; }
+    
+    void setStarted()               { m_started = true; }
+    bool started() const            { return m_started; }
 
     StatusAdapter *createStatusAdapter( CspTypePtr &type, PushMode pushMode );
     void pushStatus( int64_t level, int64_t errCode, const std::string &errMsg, PushBatch *batch = nullptr ) const;
 
 protected:
     //for adapters that want status adapter synced to a PushGroup
     virtual PushGroup * statusPushGroup() { return nullptr; }
@@ -130,14 +133,15 @@
     
     void processSimTimerCB();
 
     csp::Engine   * m_engine;
     DateTime        m_starttime;
     DateTime        m_endtime;
     StatusAdapter * m_statusAdapter;
+    bool            m_started;
 };
 
 inline void AdapterManager::scheduleTimerCB( DateTime next )
 {
     try
     {
         rootEngine() -> scheduleCallback( next, [ this ](){ processSimTimerCB(); return nullptr; } );
```

### Comparing `csp-0.0.2/cpp/csp/engine/AlarmInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/AlarmInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/BasketInfo.cpp` & `csp-0.0.3/cpp/csp/engine/BasketInfo.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/BasketInfo.h` & `csp-0.0.3/cpp/csp/engine/BasketInfo.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/CMakeLists.txt` & `csp-0.0.3/cpp/csp/engine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/ConstInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/ConstInputAdapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#ifndef _IN_CSP_ENGINE_ALARMINPUTADAPTER_H
+#ifndef _IN_CSP_ENGINE_CONSTINPUTADAPTER_H
 #define _IN_CSP_ENGINE_CONSTINPUTADAPTER_H
 
 #include <csp/engine/InputAdapter.h>
 
 namespace csp
 {
```

### Comparing `csp-0.0.2/cpp/csp/engine/Consumer.h` & `csp-0.0.3/cpp/csp/engine/Consumer.h`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
     Engine * engine() const         { return m_engine; }
     RootEngine * rootEngine() const { return m_engine -> rootEngine(); }
 
     DateTime now() const            { return rootEngine() -> now(); }
     uint64_t cycleCount() const     { return rootEngine() -> cycleCount(); }
 
+    void setStarted()               { m_started = true; }
+    bool started() const            { return m_started; }
+
     //called when input timeseries has an event, schedules in
     //step propagation.  See if we can do better than virtual per tick...
     virtual void handleEvent( InputId id )
     {
         m_engine -> scheduleConsumer( this );
     }
 
@@ -122,12 +125,13 @@
 
     Engine * m_engine;
 
     //for intrusive linked list
     Consumer * m_next;
     
     int32_t  m_rank;
+    bool     m_started;
 };
 
 };
 
 #endif
```

### Comparing `csp-0.0.2/cpp/csp/engine/CppNode.h` & `csp-0.0.3/cpp/csp/engine/CppNode.h`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,17 @@
     template<typename T>
     class TypedInputWrapper : public InputWrapper
     {
     public:
         using InputWrapper::InputWrapper;
 
         operator const T &() { return lastValue(); }
-        const T & lastValue() const { return ts() -> lastValueTyped<T>(); }
+        const T & lastValue() const { return ts() -> template lastValueTyped<T>(); }
 
-        const T & valueAtIndex( int32_t index ) const { return ts() -> valueAtIndex<T>( index ); }
+        const T & valueAtIndex( int32_t index ) const { return ts() -> template valueAtIndex<T>( index ); }
     };
 
     template<typename ElemWrapperT>
     class BasketInputWrapper
     {
     public:
         BasketInputWrapper( const char * name, const CppNode & node ) : m_node( node )
@@ -375,15 +375,15 @@
         void output( const T & value )
         {
             ts() -> outputTickTyped( m_node.cycleCount(), m_node.now(), value );
         }
 
         T & reserveSpace()
         {
-            return ts() -> reserveTickTyped<T>( m_node.cycleCount(), m_node.now() );
+            return ts() -> template reserveTickTyped<T>( m_node.cycleCount(), m_node.now() );
         }
     };
 
     //this is for nodes that dont actually inspect the data, they get 'T' in
     //and return 'T' out
     class GenericOutputWrapper : public OutputWrapper
     {
@@ -640,15 +640,15 @@
     { \
         auto * out = engine -> createOwnedObject<Class>( nodedef );   \
         out -> resetNodeDef(); \
         return out;             \
     }
 
 #define INIT_CPPNODE_WITH_NAME( Class, Name )       \
-    CSP csp; \
+    [[maybe_unused]] CSP csp; \
 public:                                                      \
     const char * name() const override { return #Name; } \
     _STATIC_CREATE_METHOD( Class ) \
     Class( csp::Engine * engine, const csp::CppNode::NodeDef & nodedef ) : csp::CppNode( engine, nodedef )
 
 #define INIT_CPPNODE( Class )                       INIT_CPPNODE_WITH_NAME( Class, Class )
```

### Comparing `csp-0.0.2/cpp/csp/engine/CspEnum.cpp` & `csp-0.0.3/cpp/csp/engine/CspEnum.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/CspEnum.h` & `csp-0.0.3/cpp/csp/engine/CspEnum.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/CspType.cpp` & `csp-0.0.3/cpp/csp/engine/CspType.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/CspType.h` & `csp-0.0.3/cpp/csp/engine/CspType.h`

 * *Files 13% similar despite different names*

```diff
@@ -53,17 +53,29 @@
 
             NUM_TYPES
         };
 
         template< typename T >
         struct fromCType;
 
-        template< uint8_t T, typename ELEM_T=void >
+        template< uint8_t T >
         struct toCType;
 
+        //We store bool vectors as vector<uint8_t> to account for oddities with vector<bool> across build environments
+        //toCArrayElemType means from the array's storage type to csp element type ( ie uint8_t -> bool ), otherwise its just Storage.
+        //toCArrayStorageType is the inverse
+        template< typename StorageT >
+        struct toCArrayElemType;
+
+        template< typename ElemT >
+        struct toCArrayStorageType;
+
+        template< typename ElemT >
+        struct toCArrayType;
+
     protected:
         _enum m_value;
     };
 
     using Type = Enum<TypeTraits>;
 
     CspType( Type t ) : m_type( t ) {}
@@ -86,15 +98,15 @@
     static Ptr & TIMEDELTA()       { static auto s_type = std::make_shared<const CspType>( Type::TIMEDELTA );       return s_type; }
     static Ptr & DATE()            { static auto s_type = std::make_shared<const CspType>( Type::DATE );            return s_type; }
     static Ptr & TIME()            { static auto s_type = std::make_shared<const CspType>( Type::TIME );            return s_type; }
     static Ptr & STRING();
     static Ptr & BYTES();
     static Ptr & DIALECT_GENERIC() { static auto s_type = std::make_shared<const CspType>( Type::DIALECT_GENERIC ); return s_type; }
 
-    static constexpr bool isNative( Type t ) { return t <= Type::MAX_NATIVE_TYPE; }
+    static constexpr bool isNative( TypeTraits::_enum t ) { return t <= TypeTraits::MAX_NATIVE_TYPE; }
 
     bool isNative() const { return isNative( m_type ); }
 
     template<typename T>
     struct fromCType;
 
     using StringCType = std::string;
@@ -169,55 +181,69 @@
     //returns CspArrayType with the given elemType
     static CspTypePtr & create( const CspTypePtr & elemType );
 
 private:
     CspTypePtr m_elemType;
 };
 
-template<> struct CspType::Type::fromCType<std::_Bit_reference>      { static constexpr CspType::Type type = CspType::Type::BOOL;            };
-template<> struct CspType::Type::fromCType<bool>                     { static constexpr CspType::Type type = CspType::Type::BOOL;            };
-template<> struct CspType::Type::fromCType<int8_t>                   { static constexpr CspType::Type type = CspType::Type::INT8;            };
-template<> struct CspType::Type::fromCType<uint8_t>                  { static constexpr CspType::Type type = CspType::Type::UINT8;           };
-template<> struct CspType::Type::fromCType<int16_t>                  { static constexpr CspType::Type type = CspType::Type::INT16;           };
-template<> struct CspType::Type::fromCType<uint16_t>                 { static constexpr CspType::Type type = CspType::Type::UINT16;          };
-template<> struct CspType::Type::fromCType<int32_t>                  { static constexpr CspType::Type type = CspType::Type::INT32;           };
-template<> struct CspType::Type::fromCType<uint32_t>                 { static constexpr CspType::Type type = CspType::Type::UINT32;          };
-template<> struct CspType::Type::fromCType<int64_t>                  { static constexpr CspType::Type type = CspType::Type::INT64;           };
-template<> struct CspType::Type::fromCType<uint64_t>                 { static constexpr CspType::Type type = CspType::Type::UINT64;          };
-template<> struct CspType::Type::fromCType<double>                   { static constexpr CspType::Type type = CspType::Type::DOUBLE;          };
-template<> struct CspType::Type::fromCType<DateTime>                 { static constexpr CspType::Type type = CspType::Type::DATETIME;        };
-template<> struct CspType::Type::fromCType<TimeDelta>                { static constexpr CspType::Type type = CspType::Type::TIMEDELTA;       };
-template<> struct CspType::Type::fromCType<Date>                     { static constexpr CspType::Type type = CspType::Type::DATE;            };
-template<> struct CspType::Type::fromCType<Time>                     { static constexpr CspType::Type type = CspType::Type::TIME;            };
-template<> struct CspType::Type::fromCType<CspEnum>                  { static constexpr CspType::Type type = CspType::Type::ENUM;            };
-template<> struct CspType::Type::fromCType<CspType::StringCType>     { static constexpr CspType::Type type = CspType::Type::STRING;          };
-template<> struct CspType::Type::fromCType<StructPtr>                { static constexpr CspType::Type type = CspType::Type::STRUCT;          };
-template<typename T> struct CspType::Type::fromCType<TypedStructPtr<T>> { static constexpr CspType::Type type = CspType::Type::STRUCT;       };
-template<> struct CspType::Type::fromCType<DialectGenericType>       { static constexpr CspType::Type type = CspType::Type::DIALECT_GENERIC; };
-template<typename T> struct CspType::Type::fromCType<std::vector<T>> { static constexpr CspType::Type type = CspType::Type::ARRAY; };
-
-template<> struct CspType::Type::toCType<CspType::Type::BOOL,void>            { using type = bool;      };
-template<> struct CspType::Type::toCType<CspType::Type::INT8,void>            { using type = int8_t;    };
-template<> struct CspType::Type::toCType<CspType::Type::UINT8,void>           { using type = uint8_t;   };
-template<> struct CspType::Type::toCType<CspType::Type::INT16,void>           { using type = int16_t;   };
-template<> struct CspType::Type::toCType<CspType::Type::UINT16,void>          { using type = uint16_t;  };
-template<> struct CspType::Type::toCType<CspType::Type::INT32,void>           { using type = int32_t;   };
-template<> struct CspType::Type::toCType<CspType::Type::UINT32,void>          { using type = uint32_t;  };
-template<> struct CspType::Type::toCType<CspType::Type::INT64,void>           { using type = int64_t;   };
-template<> struct CspType::Type::toCType<CspType::Type::UINT64,void>          { using type = uint64_t;  };
-template<> struct CspType::Type::toCType<CspType::Type::DOUBLE,void>          { using type = double;    };
-template<> struct CspType::Type::toCType<CspType::Type::DATETIME,void>        { using type = DateTime;  };
-template<> struct CspType::Type::toCType<CspType::Type::TIMEDELTA,void>       { using type = TimeDelta; };
-template<> struct CspType::Type::toCType<CspType::Type::DATE,void>            { using type = Date; };
-template<> struct CspType::Type::toCType<CspType::Type::TIME,void>            { using type = Time; };
-template<> struct CspType::Type::toCType<CspType::Type::ENUM,void>            { using type = CspEnum; };
-template<> struct CspType::Type::toCType<CspType::Type::STRING,void>          { using type = CspType::StringCType; };
-template<> struct CspType::Type::toCType<CspType::Type::STRUCT,void>          { using type = StructPtr; };
-template<> struct CspType::Type::toCType<CspType::Type::DIALECT_GENERIC,void> { using type = DialectGenericType; };
-template<typename T> struct CspType::Type::toCType<CspType::Type::ARRAY,T> { using type = std::vector<T>; };
+template<> struct CspType::TypeTraits::fromCType<bool>                     { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::BOOL;            };
+template<> struct CspType::TypeTraits::fromCType<int8_t>                   { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::INT8;            };
+template<> struct CspType::TypeTraits::fromCType<uint8_t>                  { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::UINT8;           };
+template<> struct CspType::TypeTraits::fromCType<int16_t>                  { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::INT16;           };
+template<> struct CspType::TypeTraits::fromCType<uint16_t>                 { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::UINT16;          };
+template<> struct CspType::TypeTraits::fromCType<int32_t>                  { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::INT32;           };
+template<> struct CspType::TypeTraits::fromCType<uint32_t>                 { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::UINT32;          };
+template<> struct CspType::TypeTraits::fromCType<int64_t>                  { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::INT64;           };
+template<> struct CspType::TypeTraits::fromCType<uint64_t>                 { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::UINT64;          };
+template<> struct CspType::TypeTraits::fromCType<double>                   { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::DOUBLE;          };
+template<> struct CspType::TypeTraits::fromCType<DateTime>                 { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::DATETIME;        };
+template<> struct CspType::TypeTraits::fromCType<TimeDelta>                { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::TIMEDELTA;       };
+template<> struct CspType::TypeTraits::fromCType<Date>                     { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::DATE;            };
+template<> struct CspType::TypeTraits::fromCType<Time>                     { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::TIME;            };
+template<> struct CspType::TypeTraits::fromCType<CspEnum>                  { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::ENUM;            };
+template<> struct CspType::TypeTraits::fromCType<CspType::StringCType>     { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::STRING;          };
+template<> struct CspType::TypeTraits::fromCType<StructPtr>                { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::STRUCT;          };
+template<typename T> struct CspType::TypeTraits::fromCType<TypedStructPtr<T>> { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::STRUCT;       };
+template<> struct CspType::TypeTraits::fromCType<DialectGenericType>       { static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::DIALECT_GENERIC; };
+template<typename StorageT> struct CspType::TypeTraits::fromCType<std::vector<StorageT>>
+{ 
+    static_assert( !std::is_same<StorageT,bool>::value, "vector<bool> should not be getting instantiated" );
+    static constexpr CspType::TypeTraits::_enum type = CspType::TypeTraits::ARRAY;
+};
+
+template<> struct CspType::TypeTraits::fromCType<std::vector<bool>>
+{ 
+};
+
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::BOOL>            { using type = bool;      };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::INT8>            { using type = int8_t;    };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::UINT8>           { using type = uint8_t;   };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::INT16>           { using type = int16_t;   };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::UINT16>          { using type = uint16_t;  };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::INT32>           { using type = int32_t;   };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::UINT32>          { using type = uint32_t;  };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::INT64>           { using type = int64_t;   };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::UINT64>          { using type = uint64_t;  };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::DOUBLE>          { using type = double;    };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::DATETIME>        { using type = DateTime;  };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::TIMEDELTA>       { using type = TimeDelta; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::DATE>            { using type = Date; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::TIME>            { using type = Time; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::ENUM>            { using type = CspEnum; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::STRING>          { using type = CspType::StringCType; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::STRUCT>          { using type = StructPtr; };
+template<> struct CspType::TypeTraits::toCType<CspType::TypeTraits::DIALECT_GENERIC> { using type = DialectGenericType; };
+
+template<typename ElemT> struct CspType::TypeTraits::toCArrayStorageType       { using type = ElemT; };
+template<> struct CspType::TypeTraits::toCArrayStorageType<bool>               { using type = uint8_t; };
+
+template<typename StorageT> struct CspType::TypeTraits::toCArrayElemType       { using type = StorageT; };
+template<> struct CspType::TypeTraits::toCArrayElemType<uint8_t>               { using type = bool; };
+
+template<typename T> struct CspType::TypeTraits::toCArrayType    { using type = std::vector<typename CspType::TypeTraits::toCArrayStorageType<T>::type>; };
 
 template<> struct CspType::fromCType<bool>                 { static CspTypePtr & type() { return CspType::BOOL();      } };
 template<> struct CspType::fromCType<int8_t>               { static CspTypePtr & type() { return CspType::INT8();      } };
 template<> struct CspType::fromCType<uint8_t>              { static CspTypePtr & type() { return CspType::UINT8();     } };
 template<> struct CspType::fromCType<int16_t>              { static CspTypePtr & type() { return CspType::INT16();     } };
 template<> struct CspType::fromCType<uint16_t>             { static CspTypePtr & type() { return CspType::UINT16();    } };
 template<> struct CspType::fromCType<int32_t>              { static CspTypePtr & type() { return CspType::INT32();     } };
```

### Comparing `csp-0.0.2/cpp/csp/engine/CycleStepTable.cpp` & `csp-0.0.3/cpp/csp/engine/CycleStepTable.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/CycleStepTable.h` & `csp-0.0.3/cpp/csp/engine/CycleStepTable.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/DialectGenericType.h` & `csp-0.0.3/cpp/csp/engine/DialectGenericType.h`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     bool operator==( const DialectGenericType & rhs ) const;
     bool operator!=( const DialectGenericType & rhs ) const { return !( (*this)==rhs); }
 
     size_t hash() const;
 
 private:
-    void* m_data;
+    [[maybe_unused]] void* m_data;
 };
 
 std::ostream & operator<<( std::ostream & o, const DialectGenericType & obj );
 
 }
 
 namespace std
```

### Comparing `csp-0.0.2/cpp/csp/engine/Dictionary.cpp` & `csp-0.0.3/cpp/csp/engine/Dictionary.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Dictionary.h` & `csp-0.0.3/cpp/csp/engine/Dictionary.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/DynamicEngine.cpp` & `csp-0.0.3/cpp/csp/engine/DynamicEngine.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/DynamicEngine.h` & `csp-0.0.3/cpp/csp/engine/DynamicEngine.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #ifndef _IN_CSP_ENGINE_DYNAMICENGINE_H
-#define _IN_CSP_ENGINE_DUNAMICENGINE_H
+#define _IN_CSP_ENGINE_DYNAMICENGINE_H
 
 #include <csp/engine/Engine.h>
 #include <csp/engine/OutputAdapter.h>
 #include <string>
 #include <unordered_map>
 
 namespace csp
```

### Comparing `csp-0.0.2/cpp/csp/engine/DynamicNode.cpp` & `csp-0.0.3/cpp/csp/engine/DynamicNode.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/DynamicNode.h` & `csp-0.0.3/cpp/csp/engine/DynamicNode.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Engine.cpp` & `csp-0.0.3/cpp/csp/engine/Engine.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -152,58 +152,87 @@
 {
     int32_t maxRank = computeRanks();
     m_cycleStepTable.resize( maxRank );
 
     auto start = std::max( m_rootEngine -> now(), m_rootEngine -> startTime() );
     auto end   = m_rootEngine -> endTime();
 
-
     //start up managers
     for( auto & manager : m_adapterManagers )
+    {
         manager -> start( start, end );
+        manager -> setStarted();
+    }
 
     //start up output adapters
     for( auto & adapter : m_outputAdapters )
+    {
         adapter -> start();
+        adapter -> setStarted();
+    }
 
     for( auto & entry : m_graphOutputs )
     {
-        if( entry.second -> engine() == this )
-            entry.second -> start();
+        auto & graphOutputAdapter = entry.second;
+        if( graphOutputAdapter -> engine() == this )
+        {
+            graphOutputAdapter -> start();
+            graphOutputAdapter -> setStarted();
+        }
     }
 
     //start up input adapters
     for( auto & adapter : m_inputAdapters )
+    {
         adapter -> start( start, end );
+        adapter -> setStarted();
+    }
 
     //see registerOwnedObject( AdapterManager ) above, we register adapter managers with root.  At this point we dont
     //need the list of mgrs created in a dynamic engine anymore, so we clear out the mem ( and effetively take them out of the stop() list for dynamic shutdown )
     if( !isRootEngine() )
         m_adapterManagers.clear();
 
     //startup nodes
     for( auto & node : m_nodes )
+    {
         node -> start();
+        node -> setStarted();
+    }
 }
 
 void Engine::stop()
 {
+    // Ensure we only stop nodes/adapters that have started in the case an exception occurs during startup
     for( auto & node : m_nodes )
-        node -> stop();
+    {
+        if( node -> started() )
+            node -> stop();
+    }
 
     for( auto & adapter : m_inputAdapters )
-        adapter -> stop();
+    {
+        if( adapter -> started() )
+            adapter -> stop();
+    }
 
     for( auto & entry : m_graphOutputs )
     {
-        if( entry.second -> engine() == this )
-            entry.second -> stop();
+        auto & graphOutputAdapter = entry.second;
+        if( graphOutputAdapter -> started() && graphOutputAdapter -> engine() == this )
+            graphOutputAdapter -> stop();
     }
 
     for( auto & adapter : m_outputAdapters )
-        adapter -> stop();
+    {
+        if( adapter -> started() )
+            adapter -> stop();
+    }
 
     for( auto & manager : m_adapterManagers )
-        manager -> stop();
+    {
+        if( manager -> started() )
+            manager -> stop();
+    }
 }
 
 }
```

### Comparing `csp-0.0.2/cpp/csp/engine/Engine.h` & `csp-0.0.3/cpp/csp/engine/Engine.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/EventPropagator.cpp` & `csp-0.0.3/cpp/csp/engine/EventPropagator.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/EventPropagator.h` & `csp-0.0.3/cpp/csp/engine/EventPropagator.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Feedback.h` & `csp-0.0.3/cpp/csp/engine/Feedback.h`

 * *Files 4% similar despite different names*

```diff
@@ -58,13 +58,13 @@
         CSP_THROW( TypeError, "FeedbackOutputAdapter expected boundInput of type FeedbackOutputAdapter<T> ( " <<
                    typeid(T).name() << " ) got " << typeid( *boundInput ).name() );
 }
 
 template<typename T>
 inline void FeedbackOutputAdapter<T>::executeImpl()
 {
-    m_boundInput -> pushTick( input() -> lastValueTyped<T>() );
+    m_boundInput -> pushTick( input() -> template lastValueTyped<T>() );
 }
 
 }
 
 #endif
```

### Comparing `csp-0.0.2/cpp/csp/engine/GraphOutputAdapter.cpp` & `csp-0.0.3/cpp/csp/engine/GraphOutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/GraphOutputAdapter.h` & `csp-0.0.3/cpp/csp/engine/GraphOutputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/InputAdapter.h` & `csp-0.0.3/cpp/csp/engine/InputAdapter.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,29 @@
     template<typename T>
     bool consumeTick( const T & value );
 
     RootEngine * rootEngine() { return m_rootEngine; }
 
     PushMode pushMode() const { return m_pushMode; }
 
+    void setStarted()         { m_started = true; }
+    bool started() const      { return m_started; }
+
     //if adapter is BURST this will return the type of the data, rather than the BURST vector<Data>
     const CspType * dataType() const
     {
         if( m_pushMode == PushMode::BURST )
             return static_cast<const CspArrayType *>( type() ) -> elemType().get();
         return type();
     }
 
 protected:
     RootEngine * m_rootEngine;
     PushMode     m_pushMode;
+    bool         m_started;
 };
 
 template<typename T>
 bool InputAdapter::consumeTick( const T & value )
 {
     switch( pushMode() )
     {
@@ -63,15 +67,15 @@
         }
 
         case PushMode::BURST:
         {
             CSP_ASSERT( type() -> type() == CspType::Type::ARRAY );
             CSP_ASSERT( static_cast<const CspArrayType * >( type() ) -> elemType() -> type() == CspType::Type::fromCType<T>::type );
 
-            using ArrayT = typename CspType::Type::toCType<CspType::Type::ARRAY,T>::type;
+            using ArrayT = typename CspType::Type::toCArrayType<T>::type;
             if( likely( rootEngine() -> cycleCount() != lastCycleCount() ) )
             {
                 //ensure we reuse vector memory in our buffer by using reserve api and 
                 //clearing existing value if any
                 reserveTickTyped<ArrayT>( rootEngine() -> cycleCount(), rootEngine() -> now() ).clear();
             }
```

### Comparing `csp-0.0.2/cpp/csp/engine/InputId.h` & `csp-0.0.3/cpp/csp/engine/InputId.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Node.cpp` & `csp-0.0.3/cpp/csp/engine/Node.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Node.h` & `csp-0.0.3/cpp/csp/engine/Node.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/OutputAdapter.cpp` & `csp-0.0.3/cpp/csp/engine/OutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/OutputAdapter.h` & `csp-0.0.3/cpp/csp/engine/OutputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PartialSwitchCspType.h` & `csp-0.0.3/cpp/csp/engine/PartialSwitchCspType.h`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 {
     using TagType = CspType::Type::toCType<V1>;
 };
 
 template< csp::CspType::Type::_enum U1 >
 struct SwitchCTypeResolver<csp::CspType::Type::ARRAY, U1>
 {
-    using TagType = CspType::Type::toCType<csp::CspType::Type::ARRAY, typename CspType::Type::toCType<U1>::type>;
+    using TagType = CspType::Type::toCArrayType<typename CspType::Type::toCType<U1>::type>;
 };
 
 template< csp::CspType::Type::_enum V1, csp::CspType::Type::_enum ...Vs >
 struct PartialSwitchCspType<V1, Vs...>
 {
     template< csp::CspType::Type::_enum ...ExtraVs >
     using Extend=PartialSwitchCspType<Vs..., ExtraVs...>;
@@ -148,15 +148,15 @@
             std::enable_if_t<isSupportedType<T>(), int> = 1 >
     static R_T handleArrayType( const CspType *type, F &&f )
     {
         const auto *arrayType = static_cast<const CspArrayType *>( type );
 
         return ArraySubTypeSwitchT::invoke( arrayType -> elemType().get(), [ &f ]( auto tag )
         {
-            return f( CspType::Type::toCType<T, typename decltype(tag)::type>());
+            return f( CspType::Type::toCArrayType<typename decltype(tag)::type>());
         } );
     }
 
     template< typename F,
             typename R_T,
             typename ArraySubTypeSwitchT,
             csp::CspType::Type::_enum T = CspType::Type::ARRAY,
@@ -330,16 +330,16 @@
 
 template<>
 struct ConstructibleTypeSwitchAux<std::string>
 {
     using type = PartialSwitchCspType<csp::CspType::Type::STRING>;
 };
 
-template< typename T >
-struct ConstructibleTypeSwitchAux<std::vector<T>>
+template< typename StorageT >
+struct ConstructibleTypeSwitchAux<std::vector<StorageT>>
 {
     using type = PartialSwitchCspType<csp::CspType::Type::ARRAY>;
 };
 
 template<>
 struct ConstructibleTypeSwitchAux<StructPtr>
 {
```

### Comparing `csp-0.0.2/cpp/csp/engine/PendingPushEvents.cpp` & `csp-0.0.3/cpp/csp/engine/PendingPushEvents.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PendingPushEvents.h` & `csp-0.0.3/cpp/csp/engine/PendingPushEvents.h`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 #include <csp/engine/PushEvent.h>
 #include <unordered_map>
 
 namespace csp
 {
 
-class PushGroup;
+struct PushGroup;
 class PushInputAdapters;
 
 class PendingPushEvents
 {
 public:
     PendingPushEvents();
     ~PendingPushEvents();
```

### Comparing `csp-0.0.2/cpp/csp/engine/Profiler.h` & `csp-0.0.3/cpp/csp/engine/Profiler.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PullInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/PullInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PushEvent.h` & `csp-0.0.3/cpp/csp/engine/PushEvent.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PushInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/PushInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/PushPullInputAdapter.cpp` & `csp-0.0.3/cpp/csp/engine/PushPullInputAdapter.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,14 @@
                                        }
 
                                        return true;
                                    } );
 
     if( consumed && m_nextPullEvent )
     {
-        if( m_adjustOutOfOrderTime )
-            m_nextPullEvent->time = std::max( m_nextPullEvent -> time, rootEngine() -> now() );
-
         m_timerHandle = rootEngine() -> scheduleCallback( m_nextPullEvent->time,
                                                           [this]() { return processNextPullEvent() ? nullptr : this; } );
     }
 
     return consumed;
 }
 
@@ -79,11 +76,15 @@
     {
         std::lock_guard<std::mutex> g( m_queueMutex );
         m_threadQueue.swap( m_poppedPullEvents );
     }
 
     auto * event = m_poppedPullEvents.front();
     m_poppedPullEvents.pop();
+
+    if( m_adjustOutOfOrderTime )
+        event -> time = std::max( event -> time, rootEngine() -> now() );
+
     return event;    
 }
 
 }
```

### Comparing `csp-0.0.2/cpp/csp/engine/PushPullInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/PushPullInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/RootEngine.cpp` & `csp-0.0.3/cpp/csp/engine/RootEngine.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -156,28 +156,33 @@
         ~DialectReleaseGIL()                              { engine -> dialectLockGIL(); }
         RootEngine * engine;
     };
 
     std::vector<PushGroup *> dirtyGroups;
 
     m_inRealtime = true;
+    bool haveEvents = false;
     while( m_state == State::RUNNING && !g_SIGNALED )
     {
         TimeDelta waitTime;
         if( !m_pendingPushEvents.hasEvents() )
         {
             DateTime now = DateTime::now();
             waitTime = std::min( m_endTime - now, m_settings.queueWaitTime );
             if( m_scheduler.hasEvents() )
                 waitTime = std::min( m_scheduler.nextTime() - DateTime::now(), waitTime );
         }
 
+        if( !haveEvents )
         {
+            //We keep the haveEvents flag in case there were events, but we only decided to execute
+            //timers in the previous cycle, then we shouldnt wait again ( which can actually lead to cases
+            //where we miss triggers )
             DialectReleaseGIL release( this );
-            m_pushEventQueue.wait( waitTime );
+            haveEvents = m_pushEventQueue.wait( waitTime );
         }
 
         //grab time after waitForEvents so that we dont grab events with time > now
         m_now = DateTime::now();
         if( m_now > end )
             break;
 
@@ -197,14 +202,15 @@
             processPendingPushEvents( dirtyGroups );
             processPushEventQueue( events, dirtyGroups );
 
             for( auto * group : dirtyGroups )
                 group -> state = PushGroup::NONE;
             
             dirtyGroups.clear();
+            haveEvents = false;
         }
 
         m_cycleStepTable.executeCycle( m_profiler.get() );
 
         processEndCycle();
     }
```

### Comparing `csp-0.0.2/cpp/csp/engine/RootEngine.h` & `csp-0.0.3/cpp/csp/engine/RootEngine.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 {
 
 class Dictionary;
 
 class EndCycleListener
 {
 public:
+    virtual ~EndCycleListener() {};
     virtual void onEndCycle() = 0;
     
     bool isDirty() const  { return m_dirty; }
     void setDirtyFlag()   { m_dirty = true; }
     void clearDirtyFlag() { m_dirty = false; }
 
 private:
```

### Comparing `csp-0.0.2/cpp/csp/engine/Scheduler.cpp` & `csp-0.0.3/cpp/csp/engine/Scheduler.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Scheduler.h` & `csp-0.0.3/cpp/csp/engine/Scheduler.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 #define _IN_CSP_ENGINE_SCHEDULER_H
 
 #include <csp/core/BasicAllocator.h>
 #include <csp/core/Time.h>
 #include <cassert>
 #include <functional>
 #include <map>
+#include <unordered_map>
 #include <unordered_set>
 
 namespace csp
 {
 
 class InputAdapter;
 
 class Scheduler
 {
     struct Event;
 
 public:
-    //For non-collapsing inputs, the callback should return a pointer to the input adapter that is 
+    //For non-collapsing inputs, the callback should return a pointer to the input adapter that is
     //unrolling / not collapsing.  This will ensure pending events for a given input adapter will get deferred
-    //to the next cycle until its completely unrolled.  This avoids a O(n^2) loop of reprocessing multiple pending events on 
+    //to the next cycle until its completely unrolled.  This avoids a O(n^2) loop of reprocessing multiple pending events on
     //a given input adapter.  If the callback isnt for an input adapter or if it is able to consume / process the tick, return nullptr
     using Callback = std::function<const InputAdapter *()>;
 
     class Handle
     {
     public:
         Handle() { reset(); }
         Handle( const Handle & rhs ) = default;
         bool expired() const;
         bool active() const { return !expired(); }
-    
+
         operator bool() const { return active(); }
 
         //Only valid if handle is active, otherwise returns NONE
         DateTime time() const;
 
-        void reset() 
+        void reset()
         {
             event = nullptr;
             id = 0;
         }
 
         size_t hash() const { return id; }
 
@@ -66,25 +67,25 @@
     private:
         Scheduler & m_scheduler;
         Event     * m_lastEvent;
         DateTime    m_now;
     };
 
     Scheduler();
-    ~Scheduler();  
+    ~Scheduler();
 
-    //Callback can return false which means it should stick around 
+    //Callback can return false which means it should stick around
     //and re-execute next engine cycle
     Handle scheduleCallback( Handle reserved, DateTime time, Callback &&cb );
     Handle scheduleCallback( DateTime time, Callback &&cb );
     Handle rescheduleCallback( Handle handle, DateTime time );
     bool   cancelCallback( Handle handle );
 
     //useful to break circular dep of a callback needing its own handle
-    Handle reserveHandle(); 
+    Handle reserveHandle();
 
     bool hasEvents()           { return !m_map.empty() || m_pendingEvents.hasEvents(); }
     DateTime nextTime() const  { return m_pendingEvents.hasEvents() ? m_pendingEvents.time() : m_map.begin() -> first; }
 
     void executeNextEvents( DateTime now, Event * start = nullptr );
 
 private:
@@ -100,15 +101,15 @@
 
         T * allocate( std::size_t n )
         {
             assert( n == 1 );
             return m_allocator.allocate();
         }
 
-        void deallocate( T* p, std::size_t n ) noexcept 
+        void deallocate( T* p, std::size_t n ) noexcept
         {
             assert( n == 1 );
             m_allocator.free( p );
         }
 
     private:
         TypedBasicAllocator<T> m_allocator;
@@ -156,15 +157,15 @@
 
         bool hasEvents() const { return !m_pendingEvents.empty(); }
 
         DateTime time() const { return m_time; }
 
     private:
         //NOTE the reason that this isnt simply kept as an unordered_map<InputAdapter*,Event> list is to ensure
-        //simulated runs have complete reproducibility and are deterministic.  If we key by InputAdapter * pointer, ordering of 
+        //simulated runs have complete reproducibility and are deterministic.  If we key by InputAdapter * pointer, ordering of
         //invocations will vary across runs ( this generally wouldnt matter if all code was side-effect free, but even so basket input
         //tickeditems() order depends on order of basket elemnt ticks in a given cycle )
         //Instead we maintain an unordered_map<InputAdapter*, list iterator> to ensure we keep an adapter once in the m_pendingEvents list
         //The list itself is the one used for iteration and execution of events, which should alwys be deterministic
 
         //EventList for a single input adapter
         struct PendingEventList
@@ -173,15 +174,15 @@
 
             //sentinels
             Event head;
             Event tail;
         };
 
         //time of all pending events
-        DateTime m_time; 
+        DateTime m_time;
 
         //Every list entry is *PER ADAPTER*, each entry will have a linked list of Event objects
         std::list<PendingEventList> m_pendingEvents;
 
         std::unordered_map<const InputAdapter *, std::list<PendingEventList>::iterator> m_pendingAdapters;
         Scheduler & m_scheduler;
     };
```

### Comparing `csp-0.0.2/cpp/csp/engine/StatusAdapter.h` & `csp-0.0.3/cpp/csp/engine/StatusAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Struct.cpp` & `csp-0.0.3/cpp/csp/engine/Struct.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/Struct.h` & `csp-0.0.3/cpp/csp/engine/Struct.h`

 * *Files 1% similar despite different names*

```diff
@@ -271,30 +271,30 @@
 
     void setValue( Struct * s, const CType & str ) const
     {
         *reinterpret_cast<CType*>( valuePtr( s ) ) = str;
         setIsSet( s );
     }
 
-    virtual void copyFrom( const Struct * src, Struct * dest ) const
+    virtual void copyFrom( const Struct * src, Struct * dest ) const override
     {
         value( dest ) = value( src );
     }
 
-    virtual void deepcopyFrom( const Struct * src, Struct * dest ) const
+    virtual void deepcopyFrom( const Struct * src, Struct * dest ) const override
     {
         value( dest ) = value( src );
     }
 
-    virtual bool isEqual( const Struct * x, const Struct * y ) const
+    virtual bool isEqual( const Struct * x, const Struct * y ) const override
     {
         return value( x ) == value( y );
     }
 
-    virtual size_t hash( const Struct * x ) const
+    virtual size_t hash( const Struct * x ) const override
     {
         return std::hash<CType>()( value( x ) );
     }
 
 private:
 
     CType & value( Struct * s ) const
@@ -304,26 +304,26 @@
 
     void clearValueImpl( Struct * s ) const override
     {
         value( s ).clear();
     }
 };
 
-template<typename ElemT>
+template<typename CType>
 class ArrayStructField : public NonNativeStructField
 {
-    using CType = typename csp::CspType::Type::toCType<CspType::Type::ARRAY,ElemT>::type;
+    using ElemT = typename CType::value_type;
 
     //template<typename T, std::enable_if_t<CspType::isNative(CspType::fromCType<T>::type), bool> = true>
     template<typename T>
     static std::enable_if_t<CspType::isNative(CspType::Type::fromCType<T>::type), void> deepcopy( const std::vector<T> & src, std::vector<T> & dest )
     {
         dest = src;
     }
-
+        
     static void deepcopy( const std::vector<std::string> & src, std::vector<std::string> & dest )
     {
         dest = src;
     }
 
     //Declared at end of file since StructPtr isnt defined yet
     static void deepcopy( const std::vector<StructPtr> & src, std::vector<StructPtr> & dest );
@@ -896,17 +896,20 @@
 template<> struct StructField::upcast<TimeDelta> { using type = TimeDeltaStructField; };
 template<> struct StructField::upcast<Date>      { using type = DateStructField; };
 template<> struct StructField::upcast<Time>      { using type = TimeStructField; };
 template<> struct StructField::upcast<CspEnum>   { using type = CspEnumStructField; };
 
 template<> struct StructField::upcast<typename StringStructField::CType> { using type = StringStructField; };
 template<> struct StructField::upcast<StructPtr>                         { using type = StructStructField; };
-
-template<typename T> struct StructField::upcast<std::vector<T>>          { using type = ArrayStructField<T>; };
-template<> struct StructField::upcast<csp::DialectGenericType> { using type = DialectGenericStructField; };
+template<> struct StructField::upcast<csp::DialectGenericType>           { using type = DialectGenericStructField; };
+template<typename StorageT> struct StructField::upcast<std::vector<StorageT>>
+{ 
+    static_assert( !std::is_same<StorageT,bool>::value, "vector<bool> should not be getting instantiated" );
+    using type = ArrayStructField<std::vector<StorageT>>;
+};
 
 }
 
 namespace std
 {
 
 template<>
```

### Comparing `csp-0.0.2/cpp/csp/engine/TickBuffer.h` & `csp-0.0.3/cpp/csp/engine/TickBuffer.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/TimeSeries.h` & `csp-0.0.3/cpp/csp/engine/TimeSeries.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/TimeSeriesProvider.cpp` & `csp-0.0.3/cpp/csp/engine/TimeSeriesProvider.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/TimeSeriesProvider.h` & `csp-0.0.3/cpp/csp/engine/TimeSeriesProvider.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/TimerInputAdapter.h` & `csp-0.0.3/cpp/csp/engine/TimerInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/TypeCast.h` & `csp-0.0.3/cpp/csp/engine/TypeCast.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/VectorContainer.cpp` & `csp-0.0.3/cpp/csp/engine/VectorContainer.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 std::unique_ptr<VectorContainer> VectorContainer::createForCspType(CspTypePtr &type, bool optionalValues)
 {
     return createForCspType(type.get());
 }
 
 std::unique_ptr<VectorContainer> VectorContainer::createForCspType( const CspType *type, bool optionalValues )
 {
-    return AllCspTypeSwitch::invoke(type, [type, optionalValues]( auto tag )
+    return AllCspTypeSwitch::invoke(type, [optionalValues]( auto tag )
     {
         if(optionalValues)
         {
             return std::unique_ptr<VectorContainer>( new TypedVectorContainer<std::optional<typename decltype(tag)::type>> );
         }
         else
         {
```

### Comparing `csp-0.0.2/cpp/csp/engine/VectorContainer.h` & `csp-0.0.3/cpp/csp/engine/VectorContainer.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/engine/WindowBuffer.h` & `csp-0.0.3/cpp/csp/engine/WindowBuffer.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/CMakeLists.txt` & `csp-0.0.3/cpp/csp/python/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,18 @@
         PyStruct.h)
 
 add_library(csptypesimpl
             csptypesimpl.cpp
             CspTypeFactory.cpp
             PyCspEnum.cpp
             PyCspType.cpp
-            PyStruct.cpp)
+            PyStruct.cpp
+            PyStructToJson.cpp)
 set_target_properties(csptypesimpl PROPERTIES PUBLIC_HEADER "${CSPTYPESIMPL_PUBLIC_HEADERS}")
+target_compile_definitions(csptypesimpl PUBLIC RAPIDJSON_HAS_STDSTRING=1)
 target_link_libraries(csptypesimpl csp_core csp_types)
 
 set(CSPIMPL_PUBLIC_HEADERS
         Common.h
         Conversions.h
         Exception.h
         InitHelper.h
@@ -32,15 +34,16 @@
         PyCppNode.h
         PyNode.h
         PyNodeWrapper.h
         PyNumbaNode.h
         PyObjectPtr.h
         PyOutputAdapterWrapper.h
         PyOutputProxy.h
-        PyConstants.h)
+        PyConstants.h
+        PyStructToJson.h)
 
 add_library(cspimpl SHARED
         cspimpl.cpp
         Conversions.cpp
         NumpyConversions.cpp
         PyAdapterManager.cpp
         PyAdapterManagerWrapper.cpp
@@ -89,19 +92,23 @@
 add_library(cspmathimpl SHARED cspmathimpl.cpp)
 target_link_libraries(cspmathimpl cspimpl mathimpl)
 
 ## Stats c++ module
 add_library(cspstatsimpl SHARED cspstatsimpl.cpp)
 target_link_libraries(cspstatsimpl cspimpl statsimpl)
 
+## Testlib c++ module
+add_library(csptestlibimpl SHARED csptestlibimpl.cpp)
+target_link_libraries(csptestlibimpl cspimpl)
+
 ## NumPy stats c++ module
 add_library(npstatsimpl STATIC npstatsimpl.cpp)
 add_library(cspnpstatsimpl SHARED cspnpstatsimpl.cpp)
 target_link_libraries(cspnpstatsimpl cspimpl npstatsimpl)
 target_include_directories(npstatsimpl PRIVATE ${NUMPY_INCLUDE_DIRS})
 target_include_directories(cspnpstatsimpl PRIVATE ${NUMPY_INCLUDE_DIRS})
 
-install(TARGETS csptypesimpl cspimpl cspbaselibimpl cspbasketlibimpl cspmathimpl cspstatsimpl cspnpstatsimpl
+install(TARGETS csptypesimpl cspimpl cspbaselibimpl cspbasketlibimpl cspmathimpl cspstatsimpl csptestlibimpl cspnpstatsimpl
         PUBLIC_HEADER DESTINATION include/csp/python
         RUNTIME DESTINATION bin/
         LIBRARY DESTINATION lib/
        )
```

### Comparing `csp-0.0.2/cpp/csp/python/Common.h` & `csp-0.0.3/cpp/csp/python/Common.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/Conversions.cpp` & `csp-0.0.3/cpp/csp/python/Conversions.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/Conversions.h` & `csp-0.0.3/cpp/csp/python/Conversions.h`

 * *Files 2% similar despite different names*

```diff
@@ -702,28 +702,14 @@
     PyObject * pylist = PyList_New( v.size() );
     for( size_t i = 0; i < v.size(); i++ )
         PyList_SET_ITEM( pylist, i, toPython( v[i]._data ) );
 
     return pylist;
 }
 
-template<typename T>
-inline PyObject * toPython( const std::vector<T> & v, const CspType & type )
-{
-    assert( type.type() == CspType::Type::ARRAY );
-
-    const CspType & elemType = *static_cast<const CspArrayType &>( type ).elemType();
-    size_t size = v.size();
-    PyObjectPtr list = PyObjectPtr::check( PyList_New( size ) );
-
-    for( size_t idx = 0; idx < size; ++idx )
-        PyList_SET_ITEM( list.ptr(), idx, toPython<T>( v[idx], elemType ) );
-    return list.release();
-}
-
 template<>
 inline PyObject * toPython( const Dictionary::Value & value )
 {
     switch( static_cast<int64_t>( value.index() ) )
     {
         case Dictionary::DictDataType::MONOSTATE:          CSP_THROW( ValueError, "Monostate value is not convertible to a Python type");
         case Dictionary::DictDataType::BOOL:               return toPython( std::get<bool>( value ) );
@@ -755,46 +741,65 @@
     {
         PyObject* val = toPython( it.getUntypedValue() ); // will recurse on nested dictionaries
         PyDict_SetItemString( pydict, it.key().c_str(), PyObjectPtr::own( val ).get() );
     }
     return pydict;
 }
 
-template<typename T>
-struct FromPython<std::vector<T>>
+template<typename StorageT>
+inline PyObject * toPython( const std::vector<StorageT> & v, const CspType & type )
 {
-    static std::vector<T> impl( PyObject * o, const CspType & type )
+    assert( type.type() == CspType::Type::ARRAY );
+
+    const CspType & elemType = *static_cast<const CspArrayType &>( type ).elemType();
+    size_t size = v.size();
+    PyObjectPtr list = PyObjectPtr::check( PyList_New( size ) );
+
+    for( size_t idx = 0; idx < size; ++idx )
+    {
+        using ElemT = typename CspType::Type::toCArrayElemType<StorageT>::type;
+        PyList_SET_ITEM( list.ptr(), idx, toPython<ElemT>( v[idx], elemType ) );
+    }
+    return list.release();
+}
+
+template<typename StorageT>
+struct FromPython<std::vector<StorageT>>
+{
+    static std::vector<StorageT> impl( PyObject * o, const CspType & type )
     {
         assert( type.type() == CspType::Type::ARRAY );
         const CspType & elemType = *static_cast<const CspArrayType &>( type ).elemType();
 
-        std::vector<T> out;
+        using ElemT = typename CspType::Type::toCArrayElemType<StorageT>::type;
+
+        std::vector<StorageT> out;
         //fast path list and tuples since we can size up front
         if( PyList_Check( o ) )
         {
             size_t size = PyList_GET_SIZE( o );
             out.reserve( size );
             for( size_t i = 0; i < size; ++i )
-                out.emplace_back( fromPython<T>( PyList_GET_ITEM( o, i ), elemType ) );
+                out.emplace_back( fromPython<ElemT>( PyList_GET_ITEM( o, i ), elemType ) );
         }
         else if( PyTuple_Check( o ) )
         {
             size_t size = PyTuple_GET_SIZE( o );
             out.reserve( size );
             for( size_t i = 0; i < size; ++i )
-                out.emplace_back( fromPython<T>( PyTuple_GET_ITEM( o, i ), elemType ) );
+                out.emplace_back( fromPython<ElemT>( PyTuple_GET_ITEM( o, i ), elemType ) );
         }
         //allow iteratables
         else if( o -> ob_type -> tp_iter )
         {
             PyObjectPtr iter = PyObjectPtr::own( o -> ob_type -> tp_iter( o ) );
             PyObject * value;
             while( ( value = iter -> ob_type -> tp_iternext( iter.get() ) ) )
             {
-                out.emplace_back( fromPython<T>( value, elemType ) );
+                out.emplace_back( fromPython<ElemT>( value, elemType ) );
                 Py_DECREF( value );
             }
             if( PyErr_Occurred() )
             {
                 if( PyErr_ExceptionMatches(PyExc_StopIteration))
                     PyErr_Clear();
                 else
```

### Comparing `csp-0.0.2/cpp/csp/python/CspTypeFactory.cpp` & `csp-0.0.3/cpp/csp/python/CspTypeFactory.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/Exception.h` & `csp-0.0.3/cpp/csp/python/Exception.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/InitHelper.h` & `csp-0.0.3/cpp/csp/python/InitHelper.h`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     };
 
     return cb;
 }
 
 inline InitHelper::InitCallback InitHelper::moduleMethod( const char * name, PyCFunction func, int flags, const char * doc )
 {
-    PyMethodDef defs[2]{ { name, func, flags, doc }, nullptr };
+    PyMethodDef defs[2]{ { name, func, flags, doc }, { nullptr } };
 
     //Note that we rely on the lambda closure to keep the lifetime of defs which is kept by ptr
     //m_callbacks will keep the InitCallback around for the life of the program
     InitCallback cb = [defs]( PyObject * module ) {
         if( PyModule_AddFunctions( module, ( PyMethodDef * ) defs ) < 0 )
             return false;
         return true;
```

### Comparing `csp-0.0.2/cpp/csp/python/NumpyConversions.cpp` & `csp-0.0.3/cpp/csp/python/NumpyConversions.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/NumpyConversions.h` & `csp-0.0.3/cpp/csp/python/NumpyConversions.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/NumpyInputAdapter.h` & `csp-0.0.3/cpp/csp/python/NumpyInputAdapter.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyAdapterManager.cpp` & `csp-0.0.3/cpp/csp/python/PyAdapterManager.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyAdapterManagerWrapper.cpp` & `csp-0.0.3/cpp/csp/python/PyAdapterManagerWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyAdapterManagerWrapper.h` & `csp-0.0.3/cpp/csp/python/PyAdapterManagerWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyBasketInputProxy.cpp` & `csp-0.0.3/cpp/csp/python/PyBasketInputProxy.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyBasketInputProxy.h` & `csp-0.0.3/cpp/csp/python/PyBasketInputProxy.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyBasketOutputProxy.cpp` & `csp-0.0.3/cpp/csp/python/PyBasketOutputProxy.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyBasketOutputProxy.h` & `csp-0.0.3/cpp/csp/python/PyBasketOutputProxy.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyConstAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyConstAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyConstants.cpp` & `csp-0.0.3/cpp/csp/python/PyConstants.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyCppNode.cpp` & `csp-0.0.3/cpp/csp/python/PyCppNode.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyCppNode.h` & `csp-0.0.3/cpp/csp/python/PyCppNode.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyCspEnum.cpp` & `csp-0.0.3/cpp/csp/python/PyCspEnum.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyCspEnum.h` & `csp-0.0.3/cpp/csp/python/PyCspEnum.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyCspType.cpp` & `csp-0.0.3/cpp/csp/python/PyCspType.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyDynamicNode.cpp` & `csp-0.0.3/cpp/csp/python/PyDynamicNode.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyEngine.cpp` & `csp-0.0.3/cpp/csp/python/PyEngine.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyEngine.h` & `csp-0.0.3/cpp/csp/python/PyEngine.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyFeedbackAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyFeedbackAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyGraphOutputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyGraphOutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyInputAdapterWrapper.cpp` & `csp-0.0.3/cpp/csp/python/PyInputAdapterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyInputAdapterWrapper.h` & `csp-0.0.3/cpp/csp/python/PyInputAdapterWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyInputProxy.cpp` & `csp-0.0.3/cpp/csp/python/PyInputProxy.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyInputProxy.h` & `csp-0.0.3/cpp/csp/python/PyInputProxy.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyIterator.h` & `csp-0.0.3/cpp/csp/python/PyIterator.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyManagedSimInputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyManagedSimInputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNode.cpp` & `csp-0.0.3/cpp/csp/python/PyNode.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNode.h` & `csp-0.0.3/cpp/csp/python/PyNode.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNodeWrapper.cpp` & `csp-0.0.3/cpp/csp/python/PyNodeWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNumbaNode.cpp` & `csp-0.0.3/cpp/csp/python/PyNumbaNode.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNumbaNode.h` & `csp-0.0.3/cpp/csp/python/PyNumbaNode.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyNumpyAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyNumpyAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyObjectPtr.h` & `csp-0.0.3/cpp/csp/python/PyObjectPtr.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyOutputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyOutputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyOutputAdapterWrapper.cpp` & `csp-0.0.3/cpp/csp/python/PyOutputAdapterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyOutputAdapterWrapper.h` & `csp-0.0.3/cpp/csp/python/PyOutputAdapterWrapper.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyOutputProxy.cpp` & `csp-0.0.3/cpp/csp/python/PyOutputProxy.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyOutputProxy.h` & `csp-0.0.3/cpp/csp/python/PyOutputProxy.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyPullInputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyPullInputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyPushInputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyPushInputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyPushPullInputAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyPushPullInputAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyStruct.cpp` & `csp-0.0.3/cpp/csp/python/PyStruct.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #include <csp/python/Conversions.h>
 #include <csp/python/CspTypeFactory.h>
 #include <csp/python/InitHelper.h>
 #include <csp/python/PyObjectPtr.h>
 #include <csp/python/PyStruct.h>
+#include <csp/python/PyStructToJson.h>
+
 #include <unordered_set>
 #include <type_traits>
 
 namespace csp::python { class PyObjectStructField; }
 
 namespace csp::python
 {
@@ -132,15 +134,16 @@
                 case csp::CspType::Type::STRUCT:    field = std::make_shared<StructStructField>( csptype, keystr ); break;
                 case csp::CspType::Type::ARRAY:
                 {
                     const CspArrayType & arrayType = static_cast<const CspArrayType&>( *csptype );
                     field = ArraySubTypeSwitch::invoke( arrayType.elemType(), [csptype,keystr]( auto tag ) -> std::shared_ptr<StructField>
                     {
                         using CElemType = typename decltype(tag)::type;
-                        return std::make_shared<ArrayStructField<CElemType>>( csptype, keystr );
+                        using CType = typename CspType::Type::toCArrayType<CElemType>::type;
+                        return std::make_shared<ArrayStructField<CType>>( csptype, keystr );
                     } );
 
                     break;
                 }
 
                 case csp::CspType::Type::DIALECT_GENERIC: field = std::make_shared<PyObjectStructField>( keystr, PyTypeObjectPtr::incref( ( PyTypeObject * ) type ) ); break;
                 default:
@@ -165,17 +168,17 @@
                 CSP_THROW( TypeError, "Struct " << name << " defined with multiple struct bases.  Only single-struct hierarchy is supported" );
             metabase = ( ( PyStructMeta * ) base ) -> structMeta;
         }
     }
 
     /*back reference to the struct type that will be accessible on the csp struct -> meta()
       DialectStructMeta will hold a borrowed reference to the type to avoid a circular dep
-      
+
       This is the layout of references between all these types
-                              StructMeta (shared_ptr) <-------- strong ref 
+                              StructMeta (shared_ptr) <-------- strong ref
                                   |                              |
                            DialectStructMeta ---> weak ref to PyStructMeta ( the PyType )
                                  /\                              /\
                                   |                              |
                                   | (strong ref )                |
                               Struct (shared_ptr)            python ref to its PyType
                                  /\                              |
@@ -529,15 +532,15 @@
         {
             auto const * arrayType = static_cast<const CspArrayType*>( field -> type().get() );
             const CspType * elemType = arrayType -> elemType().get();
 
             switchCspType( elemType, [ field, struct_, &arrayType, &tl_repr, show_unset ]( auto tag )
             {
                 using CElemType = typename decltype( tag )::type;
-                using ArrayType = typename std::vector<CElemType>;
+                using ArrayType = typename CspType::Type::toCArrayType<CElemType>::type;
                 const ArrayType & val = field -> value<ArrayType>( struct_ );
                 repr_array( val, *arrayType, tl_repr, show_unset );
             } );
 
             break;
         }
         case CspType::Type::DATETIME:
@@ -553,17 +556,18 @@
         }
         case CspType::Type::UNKNOWN:
         case CspType::Type::NUM_TYPES:
             break;
     }
 }
 
-template<typename ElemT>
-void repr_array( const std::vector<ElemT> & val, const CspArrayType & arrayType, std::string & tl_repr, bool show_unset )
+template<typename StorageT>
+void repr_array( const std::vector<StorageT> & val, const CspArrayType & arrayType, std::string & tl_repr, bool show_unset )
 {
+    using ElemT = typename CspType::Type::toCArrayElemType<StorageT>::type;
     tl_repr += "[";
 
     bool first = true;
     for( auto it = val.begin(); it != val.end(); it++ )
     {
         if( unlikely( first ) ) first = false;
         else tl_repr += ", ";
@@ -853,15 +857,15 @@
 }
 
 PyObject * PyStruct_deepcopy( PyStruct * self )
 {
     CSP_BEGIN_METHOD;
     //Note that once tp_alloc is called, the object will get added to GC
     //deepcopy traversal may kick in a GC collect, so we have to call that first before the PyStruct is created
-    //of it may traverse a partially consturcted object and crash 
+    //of it may traverse a partially consturcted object and crash
     auto deepcopy = self -> struct_ -> deepcopy();
     PyObject * pyDeepcopy = self -> ob_type -> tp_alloc( self -> ob_type, 0 );
     new ( pyDeepcopy ) PyStruct( deepcopy );
     return pyDeepcopy;
     CSP_RETURN_NULL;
 }
 
@@ -906,23 +910,48 @@
 }
 
 PyObject * PyStruct_all_fields_set( PyStruct * self )
 {
     return toPython( self -> struct_ -> allFieldsSet() );
 }
 
+PyObject * PyStruct_to_json( PyStruct * self, PyObject * args, PyObject * kwargs )
+{
+    CSP_BEGIN_METHOD;
+
+    // NOTE: Consider grouping customization properties into a dictionary
+    PyObject * callable = nullptr;
+
+    if( PyArg_ParseTuple( args, "O:to_json", &callable ) )
+    {
+        if( !PyCallable_Check( callable ) )
+        {
+            CSP_THROW( TypeError, "Parameter must be callable" );
+        }
+    }
+    else
+    {
+        CSP_THROW( TypeError, "Expected a callable as the argument" );
+    }
+    auto struct_ptr = self -> struct_;
+    auto buffer = structToJson( struct_ptr, callable );
+    return toPython( buffer );
+    CSP_RETURN_NULL;
+}
+
 static PyMethodDef PyStruct_methods[] = {
     { "copy",           (PyCFunction) PyStruct_copy,           METH_NOARGS, "make a shallow copy of the struct" },
     { "deepcopy",       (PyCFunction) PyStruct_deepcopy,       METH_NOARGS, "make a deep copy of the struct" },
     { "clear",          (PyCFunction) PyStruct_clear,          METH_NOARGS, "clear all fields" },
     { "copy_from",      (PyCFunction) PyStruct_copy_from,      METH_O,      "copy from struct. struct must be same type or a derived type. unset fields will copy over" },
     { "deepcopy_from",  (PyCFunction) PyStruct_deepcopy_from,  METH_O,      "deepcopy from struct. struct must be same type or a derived type. unset fields will copy over" },
     { "update_from",    (PyCFunction) PyStruct_update_from,    METH_O,      "update from struct. struct must be same type or a derived type. unset fields will be not be copied" },
     { "update",         (PyCFunction) PyStruct_update,         METH_VARARGS | METH_KEYWORDS, "update from key=val.  given fields will be set on struct.  other fields will remain as is in struct" },
     { "all_fields_set", (PyCFunction) PyStruct_all_fields_set, METH_NOARGS, "return true if all fields on the struct are set" },
+    { "to_json",        (PyCFunction) PyStruct_to_json,        METH_VARARGS | METH_KEYWORDS, "return a json string of the struct by recursively converting struct members into json format" },
     { NULL}
 };
 
 PyTypeObject PyStruct::PyType = {
     PyVarObject_HEAD_INIT(nullptr, 0)
     "_cspimpl.PyStruct",       /* tp_name */
     sizeof(PyStruct),          /* tp_basicsize */
```

### Comparing `csp-0.0.2/cpp/csp/python/PyStruct.h` & `csp-0.0.3/cpp/csp/python/PyStruct.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/PyTimerAdapter.cpp` & `csp-0.0.3/cpp/csp/python/PyTimerAdapter.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/CMakeLists.txt` & `csp-0.0.3/cpp/csp/python/adapters/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,7 +29,13 @@
         ${VENDORED_PYARROW_ROOT}/arrow/python/csv.cc
         ${VENDORED_PYARROW_ROOT}/arrow/python/filesystem.cc)
     add_library(parquetadapterimpl SHARED parquetadapterimpl.cpp ${ARROW_PYTHON_SRCS})
     target_link_libraries(parquetadapterimpl csp_core csp_engine cspimpl csp_parquet_adapter)
     target_include_directories(parquetadapterimpl PUBLIC ${ARROW_INCLUDE_DIR} ${PARQUET_INCLUDE_DIR} "${VENDORED_PYARROW_ROOT}")
     install(TARGETS parquetadapterimpl RUNTIME DESTINATION bin/ LIBRARY DESTINATION lib/)
 endif()
+
+if(CSP_BUILD_WS_CLIENT_ADAPTER)
+	add_library(websocketadapterimpl SHARED websocketadapterimpl.cpp)
+	target_link_libraries(websocketadapterimpl csp_core csp_engine cspimpl csp_websocket_client_adapter)
+	install(TARGETS websocketadapterimpl RUNTIME DESTINATION bin/ LIBRARY DESTINATION lib/)
+endif()
```

### Comparing `csp-0.0.2/cpp/csp/python/adapters/kafkaadapterimpl.cpp` & `csp-0.0.3/cpp/csp/python/adapters/kafkaadapterimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/parquetadapterimpl.cpp` & `csp-0.0.3/cpp/csp/python/adapters/parquetadapterimpl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -252,16 +252,15 @@
 private:
     PyArray_Descr *m_expectedArrayDesc;
 };
 
 class NumpyUnicodeArrayWriter : public TypedDialectGenericListWriterInterface<std::string>
 {
 public:
-    NumpyUnicodeArrayWriter( PyArray_Descr *expectedArrayDesc )
-            : m_expectedArrayDesc( expectedArrayDesc )
+    NumpyUnicodeArrayWriter()
     {
     }
 
     void writeItems( const csp::DialectGenericType &listObject ) override
     {
         PyObject *object = csp::python::toPythonBorrowed( listObject );
 
@@ -326,16 +325,15 @@
                 {
                     using CValueType = typename decltype(tag)::type;
                     auto numpy_dtype = PyArray_DescrFromType(
                             csp::python::NPY_TYPE<CValueType>::value );
 
                     if( numpy_dtype -> type_num == NPY_UNICODE )
                     {
-                        return std::make_shared<NumpyUnicodeArrayWriter>(
-                                numpy_dtype );
+                        return std::make_shared<NumpyUnicodeArrayWriter>();
                     }
                     else
                     {
                         return std::make_shared<NumpyArrayWriterImpl<CValueType>>(
                                 numpy_dtype );
                     }
                 }
@@ -379,28 +377,27 @@
 
     virtual V *getRawDataBuffer( const csp::DialectGenericType &list ) const override
     {
         auto arrayObject = reinterpret_cast<PyArrayObject *>(csp::python::toPythonBorrowed(list));
         return reinterpret_cast<V *>(PyArray_DATA( arrayObject ));
     }
 
-    virtual void setValue(const csp::DialectGenericType& list, int index, const V& value)
+    virtual void setValue(const csp::DialectGenericType& list, int index, const V& value) override
     {
         getRawDataBuffer(list)[index] = value;
     }
 
 private:
     PyArray_Descr *m_expectedArrayDesc;
 };
 
 class NumpyUnicodeReaderImpl final : public TypedDialectGenericListReaderInterface<std::string>
 {
 public:
-    NumpyUnicodeReaderImpl( PyArray_Descr *expectedArrayDesc )
-            : m_expectedArrayDesc( expectedArrayDesc )
+    NumpyUnicodeReaderImpl()
     {
     }
 
     virtual csp::DialectGenericType create( uint32_t size ) override
     {
         CSP_NOT_IMPLEMENTED;
     }
@@ -433,17 +430,14 @@
         auto arrayObject = reinterpret_cast<PyArrayObject *>(csp::python::toPythonBorrowed( list ));
         std::wstring_convert<std::codecvt_utf8<wchar_t>> converter;
         auto elementSize = PyArray_DESCR( arrayObject ) -> elsize;
         auto wideValue = converter.from_bytes( value );
         auto nElementsToCopy = std::min( int(elementSize / sizeof(wchar_t)), int( wideValue.size() + 1 ) );
         std::copy_n( wideValue.c_str(), nElementsToCopy, reinterpret_cast<wchar_t *>(PyArray_GETPTR1( arrayObject, index )) );
     }
-
-private:
-    PyArray_Descr *m_expectedArrayDesc;
 };
 
 
 inline DialectGenericListReaderInterface::Ptr create_numpy_array_reader_impl( const csp::CspTypePtr &type )
 
 {
     try
@@ -454,16 +448,15 @@
                                                                                {
                                                                                    using CValueType = typename decltype(tag)::type;
                                                                                    auto numpy_dtype = PyArray_DescrFromType(
                                                                                            csp::python::NPY_TYPE<CValueType>::value );
 
                                                                                    if( numpy_dtype -> type_num == NPY_UNICODE )
                                                                                    {
-                                                                                       return std::make_shared<NumpyUnicodeReaderImpl>(
-                                                                                               numpy_dtype );
+                                                                                       return std::make_shared<NumpyUnicodeReaderImpl>();
                                                                                    }
                                                                                    else
                                                                                    {
                                                                                        return std::make_shared<NumpyArrayReaderImpl<CValueType>>(
                                                                                                numpy_dtype );
                                                                                    }
                                                                                }
```

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/CMakeLists.txt` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/api.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/api.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_python_internal.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_python_internal.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/async.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/async.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/common.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/csv.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/datetime.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/decimal.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/deserialize.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/extension_type.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/filesystem.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/flight.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/gdb.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/helpers.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/inference.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/init.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/io.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/ipc.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/iterators.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/iterators.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib_api.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/lib_api.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_convert.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_internal.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_internal.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_interop.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_interop.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/numpy_to_arrow.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/parquet_encryption.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pch.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pch.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/platform.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/platform.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_api.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_api.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_lib.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/pyarrow_lib.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_test.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/python_to_arrow.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/serialize.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/type_traits.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/type_traits.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.cc` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.cc`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/udf.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/visibility.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/visibility.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util_overflow.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/int_util_overflow.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/io_util.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/io_util.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/iterator.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/iterator.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/key_value_metadata.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/key_value_metadata.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/launder.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/launder.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/list_util.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/list_util.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/logging.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/logging.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/macros.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/macros.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/map.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/map.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/math_constants.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/math_constants.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/memory.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/memory.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/mutex.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/mutex.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/parallel.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/parallel.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/pcg_random.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/pcg_random.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/print.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/print.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/queue.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/queue.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/range.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/range.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ree_util.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ree_util.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/regex.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/regex.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rle_encoding.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rle_encoding.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rows_to_batches.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/rows_to_batches.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/simd.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/simd.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/small_vector.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/small_vector.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/sort.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/sort.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/spaced.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/spaced.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/span.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/span.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/stopwatch.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/stopwatch.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string_builder.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/string_builder.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/task_group.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/task_group.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tdigest.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tdigest.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/test_common.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/test_common.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/thread_pool.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/thread_pool.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/time.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/time.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tracing.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/tracing.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/trie.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/trie.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_fwd.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_fwd.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_traits.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/type_traits.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ubsan.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/ubsan.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/union_util.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/union_util.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/unreachable.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/unreachable.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/uri.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/uri.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/utf8.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/utf8.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/value_parsing.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/value_parsing.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/vector.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/vector.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/visibility.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/visibility.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_compatibility.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_compatibility.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_fixup.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/util/windows_fixup.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/debug-trap.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/debug-trap.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/safe-math.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/portable-snippets/safe-math.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/xxhash.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash/xxhash.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash.h` & `csp-0.0.3/cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/vendored/xxhash.h`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/cspbaselibimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspbaselibimpl.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             {
                 s_valuesContainer.push_back( std::make_unique<NumpyArrayValueContainer>() );
             }
             else
             {
                 PartialSwitchCspType<CspType::Type::STRING, CspType::Type::DOUBLE>::invoke(
                         typ,
-                        [ this, &inputName ]( auto tag )
+                        [ this ]( auto tag )
                         {
                             s_valuesContainer.push_back( std::make_unique<ValueContainer<typename decltype(tag)::type>>() );
                         } );
             }
 
             all_registered &= s_valuesContainer.back() -> registerValue( symbolTable, inputName );
         }
```

### Comparing `csp-0.0.2/cpp/csp/python/cspbasketlibimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspbasketlibimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/cspimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspimpl.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     {"_csp_now",                    (PyCFunction) _csp_now,                   METH_O, "current engine time"},
     {"_csp_engine_start_time",      (PyCFunction) _engine_start_time,         METH_O, "engine start time"},
     {"_csp_engine_end_time",        (PyCFunction) _engine_end_time,           METH_O, "engine end time"},
     {"_csp_stop_engine",            (PyCFunction) _csp_stop_engine,           METH_VARARGS | METH_KEYWORDS, "stop engine"},
     {"create_traceback",            (PyCFunction) _create_traceback,          METH_VARARGS,   "internal"},
     {"_csp_engine_stats",           (PyCFunction) _engine_stats,              METH_O, "engine statistics"},
     {"set_capture_cpp_backtrace",   (PyCFunction) _set_capture_cpp_backtrace, METH_VARARGS,   "internal"},
-    nullptr
+    {nullptr}
 };
 
 static PyModuleDef _cspimpl_module = {
     PyModuleDef_HEAD_INIT,
     "_cspimpl",
     "_cspimpl c++ module",
     -1,
```

### Comparing `csp-0.0.2/cpp/csp/python/cspmathimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspmathimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/cspnpstatsimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspnpstatsimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/cspstatsimpl.cpp` & `csp-0.0.3/cpp/csp/python/cspstatsimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/csptypesimpl.cpp` & `csp-0.0.3/cpp/csp/python/csptypesimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/csp/python/npstatsimpl.cpp` & `csp-0.0.3/cpp/csp/python/npstatsimpl.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/CMakeLists.txt` & `csp-0.0.3/cpp/tests/core/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-find_library(GTest REQUIRED)
+find_package(GTest CONFIG REQUIRED)
 
 add_executable(test_basic_allocator test_basic_allocator.cpp)
 target_link_libraries(test_basic_allocator GTest::gtest GTest::gtest_main)
 
 add_executable(test_dynamicbitset test_dynamicbitset.cpp)
-target_link_libraries(test_dynamicbitset gtest gtest_main)
+target_link_libraries(test_dynamicbitset GTest::gtest GTest::gtest_main)
 
 add_executable(test_enum test_enum.cpp)
 target_link_libraries(test_enum csp_core csp_engine GTest::gtest GTest::gtest_main)
 
 add_executable(test_srmwlockfreequeue test_srmwlockfreequeue.cpp )
 target_link_libraries(test_srmwlockfreequeue csp_core GTest::gtest GTest::gtest_main)
 
 add_executable(test_tagged_pointer_union test_tagged_pointer_union.cpp )
 target_link_libraries(test_tagged_pointer_union csp_core GTest::gtest GTest::gtest_main)
 
 add_executable(test_time test_time.cpp )
-target_link_libraries(test_time csp_core GTest::gtest GTest::gtest_main rt)
+target_link_libraries(test_time csp_core GTest::gtest GTest::gtest_main)
 
 
 install(TARGETS test_basic_allocator
                 test_dynamicbitset
                 test_enum
-                test_srmwlockfreequeue 
-                test_tagged_pointer_union 
+                test_srmwlockfreequeue
+                test_tagged_pointer_union
                 test_time
         RUNTIME DESTINATION tests/bin/
         LIBRARY DESTINATION tests/lib/
         ARCHIVE DESTINATION tests/lib/)
```

### Comparing `csp-0.0.2/cpp/tests/core/test_basic_allocator.cpp` & `csp-0.0.3/cpp/tests/core/test_basic_allocator.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/test_dynamicbitset.cpp` & `csp-0.0.3/cpp/tests/core/test_dynamicbitset.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/test_enum.cpp` & `csp-0.0.3/cpp/tests/core/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/test_srmwlockfreequeue.cpp` & `csp-0.0.3/cpp/tests/core/test_srmwlockfreequeue.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/test_tagged_pointer_union.cpp` & `csp-0.0.3/cpp/tests/core/test_tagged_pointer_union.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/core/test_time.cpp` & `csp-0.0.3/cpp/tests/core/test_time.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -155,27 +155,29 @@
     ASSERT_EQ( ex2.minute(), 59 );
     ASSERT_EQ( ex2.second(), 59 );
 
     ASSERT_EQ( ex2.milliseconds(), 123 );
     ASSERT_EQ( ex2.microseconds(), 123456 );
     ASSERT_EQ( ex2.nanoseconds(),  123456789 );
 
+#ifdef __linux__
     dt = DateTime( 1888, 11, 15, 23, 15, 59, 999999999 );
     DateTimeEx ex3( dt );
 
     ASSERT_EQ( ex3.year(),   1888 );
     ASSERT_EQ( ex3.month(),  11 );
     ASSERT_EQ( ex3.day(),    15 );
     ASSERT_EQ( ex3.hour(),   23 );
     ASSERT_EQ( ex3.minute(), 15 );
     ASSERT_EQ( ex3.second(), 59 );
 
     ASSERT_EQ( ex3.milliseconds(), 999 );
     ASSERT_EQ( ex3.microseconds(), 999999 );
     ASSERT_EQ( ex3.nanoseconds(),  999999999 );
+#endif
 }
 
 TEST( TimeTest, test_basic_functionality )
 {
     Time t( 14, 1, 2, 123456789 );
     ASSERT_EQ( t.hour(),       14 );
     ASSERT_EQ( t.minute(),     1 );
```

### Comparing `csp-0.0.2/cpp/tests/engine/CMakeLists.txt` & `csp-0.0.3/cpp/tests/engine/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-find_library(GTest REQUIRED)
+find_package(GTest CONFIG REQUIRED)
 
 add_executable(test_dictionary test_dictionary.cpp )
-target_link_libraries(test_dictionary csp_engine GTest::gtest GTest::gtest_main rt)
+target_link_libraries(test_dictionary csp_engine GTest::gtest GTest::gtest_main)
 
 add_executable(test_tick_buffer test_tick_buffer.cpp)
 target_link_libraries(test_tick_buffer csp_engine GTest::gtest GTest::gtest_main)
 
 add_executable(test_time_series test_time_series.cpp)
-target_link_libraries(test_time_series csp_engine_static gtest gtest_main pthread)
+target_link_libraries(test_time_series csp_engine GTest::gtest GTest::gtest_main pthread)
 
 add_executable(test_partial_switch_csp_type test_partial_switch_csp_type.cpp)
 target_link_libraries(test_partial_switch_csp_type csp_engine GTest::gtest GTest::gtest_main)
 
 add_executable(test_window_buffer test_window_buffer.cpp)
 target_link_libraries(test_window_buffer csp_engine GTest::gtest GTest::gtest_main)
```

### Comparing `csp-0.0.2/cpp/tests/engine/test_dictionary.cpp` & `csp-0.0.3/cpp/tests/engine/test_dictionary.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/engine/test_engine_initial.cpp` & `csp-0.0.3/cpp/tests/engine/test_engine_initial.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/engine/test_partial_switch_csp_type.cpp` & `csp-0.0.3/cpp/tests/engine/test_partial_switch_csp_type.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -230,19 +230,19 @@
     } );
     csp::PartialSwitchCspType<csp::CspType::Type::ARRAY>::invoke( uint64ArrayType.get(), []( auto tag )
     {
         verifySameTypes<typename decltype(tag)::type, std::vector<std::uint64_t>>();
     } );
     csp::PartialSwitchCspType<csp::CspType::Type::ARRAY>::invoke( boolArrayType.get(), []( auto tag )
     {
-        verifySameTypes<typename decltype(tag)::type, std::vector<bool>>();
+        verifySameTypes<typename decltype(tag)::type, std::vector<uint8_t>>();
     } );
 
     csp::PartialSwitchCspType<csp::CspType::Type::ARRAY>::invoke<csp::PartialSwitchCspType<csp::CspType::Type::BOOL>>(
-            boolArrayType.get(), []( auto tag ) { verifySameTypes<typename decltype(tag)::type, std::vector<bool>>(); } );
+            boolArrayType.get(), []( auto tag ) { verifySameTypes<typename decltype(tag)::type, std::vector<uint8_t>>(); } );
     csp::PartialSwitchCspType<csp::CspType::Type::ARRAY>::invoke<csp::PartialSwitchCspType<csp::CspType::Type::UINT64>>(
             uint64ArrayType.get(), []( auto tag ) { verifySameTypes<typename decltype(tag)::type, std::vector<std::uint64_t>>(); } );
 
     // Should raise since we support only array of bool
     ASSERT_THROW( csp::PartialSwitchCspType<csp::CspType::Type::ARRAY>::invoke<csp::PartialSwitchCspType<csp::CspType::Type::BOOL>>(
             uint64ArrayType.get(), []( auto tag ) {} ), csp::UnsupportedSwitchType );
```

### Comparing `csp-0.0.2/cpp/tests/engine/test_tick_buffer.cpp` & `csp-0.0.3/cpp/tests/engine/test_tick_buffer.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/engine/test_time_series.cpp` & `csp-0.0.3/cpp/tests/engine/test_time_series.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/cpp/tests/engine/test_window_buffer.cpp` & `csp-0.0.3/cpp/tests/engine/test_window_buffer.cpp`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/__init__.py` & `csp-0.0.3/csp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 )
 from csp.impl.wiring.context import clear_global_context, new_global_context
 from csp.math import *
 from csp.showgraph import show_graph
 
 from . import cache_support, stats
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 def get_include_path():
     return os.path.join(os.path.dirname(__file__), "include")
 
 
 def get_lib_path():
```

### Comparing `csp-0.0.2/csp/adapters/csv.py` & `csp-0.0.3/csp/adapters/csv.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/db.py` & `csp-0.0.3/csp/adapters/db.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/kafka.py` & `csp-0.0.3/csp/adapters/kafka.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/output_adapters/parquet.py` & `csp-0.0.3/csp/adapters/output_adapters/parquet.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/output_adapters/parquet_utility_nodes.py` & `csp-0.0.3/csp/adapters/output_adapters/parquet_utility_nodes.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/parquet.py` & `csp-0.0.3/csp/adapters/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import io
 import numpy
-import platform
 import pyarrow
 import pyarrow.parquet
 from importlib.metadata import PackageNotFoundError, version as get_package_version
 from packaging import version
 from typing import TypeVar
 
 import csp
@@ -97,17 +96,14 @@
             self._properties["symbol_column"] = symbol_column
         if time_column:
             self._properties["time_column"] = time_column
         if tz:
             self._properties["tz"] = tz.zone
         if binary_arrow:
             self._properties["is_arrow_ipc"] = True
-        if not binary_arrow and platform.system() == "Darwin":
-            # TKP fix parquet reading on darwin
-            raise RuntimeError("Cannot read parquet files on macOS yet")
         if start_time:
             self._properties["start_time"] = start_time
         if end_time:
             self._properties["end_time"] = end_time
 
         self._properties["read_from_memory_tables"] = read_from_memory_tables
         if allow_overlapping_periods:
```

### Comparing `csp-0.0.2/csp/adapters/perspective.py` & `csp-0.0.3/csp/adapters/perspective.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/slack.py` & `csp-0.0.3/csp/adapters/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 from logging import getLogger
 from queue import Queue
+from ssl import SSLContext
 from threading import Thread
 from time import sleep
-from typing import Dict, List, TypeVar
+from typing import Dict, List, Optional, TypeVar
 
 import csp
 from csp.impl.adaptermanager import AdapterManagerImpl
 from csp.impl.outputadapter import OutputAdapter
 from csp.impl.pushadapter import PushInputAdapter
 from csp.impl.struct import Struct
 from csp.impl.types.tstype import ts
@@ -49,23 +50,23 @@
 
 def mention_user(userid: str) -> str:
     """Convenience method, more difficult to do in symphony but we want slack to be symmetric"""
     return f"<@{userid}>"
 
 
 class SlackAdapterManager(AdapterManagerImpl):
-    def __init__(self, app_token: str, bot_token: str):
+    def __init__(self, app_token: str, bot_token: str, ssl: Optional[SSLContext] = None):
         if not _HAVE_SLACK_SDK:
             raise RuntimeError("Could not find slack-sdk installation")
         if not app_token.startswith("xapp-") or not bot_token.startswith("xoxb-"):
             raise RuntimeError("Slack app token or bot token looks malformed")
 
         self._slack_client = SocketModeClient(
             app_token=app_token,
-            web_client=WebClient(token=bot_token),
+            web_client=WebClient(token=bot_token, ssl=ssl),
         )
         self._slack_client.socket_mode_request_listeners.append(self._process_slack_message)
 
         # down stream edges
         self._subscribers = []
         self._publishers = []
```

### Comparing `csp-0.0.2/csp/adapters/symphony.py` & `csp-0.0.3/csp/adapters/symphony.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/utils.py` & `csp-0.0.3/csp/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/adapters/websocket.py` & `csp-0.0.3/csp/adapters/websocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 import logging
 import math
 import threading
 import typing
 import urllib
 from collections import defaultdict
-from datetime import date, datetime
+from datetime import date, datetime, timedelta
+from typing import Dict, List
 
 import csp
 from csp import ts
+from csp.adapters.status import Status
+from csp.adapters.utils import (
+    BytesMessageProtoMapper,
+    DateTimeType,
+    JSONTextMessageMapper,
+    MsgMapper,
+    RawBytesMessageMapper,
+    RawTextMessageMapper,
+)
+from csp.impl.wiring import input_adapter_def, output_adapter_def, status_adapter_def
 from csp.impl.wiring.delayed_node import DelayedNodeWrapperDef
+from csp.lib import _websocketadapterimpl
+
+from .websocket_types import WebsocketHeaderUpdate
+
+_ = (
+    BytesMessageProtoMapper,
+    DateTimeType,
+    JSONTextMessageMapper,
+    RawBytesMessageMapper,
+    RawTextMessageMapper,
+)
+T = typing.TypeVar("T")
+
 
 try:
     import tornado.ioloop
     import tornado.web
     import tornado.websocket
 except ImportError:
     raise ImportError("websocket adapter requires tornado package")
@@ -351,7 +375,95 @@
 
     def _instantiate(self):
         manager = TableManager(self._tables, self._delta_updates)
         for table_name, table in self._tables.items():
             _apply_updates(manager, table_name, table.columns)
 
         _launch_application(self._port, manager, csp.const("stub"))
+
+
+class WebsocketAdapterManager:
+    def __init__(
+        self,
+        uri: str,
+        verbose_log: bool = False,
+        reconnect_interval: timedelta = timedelta(seconds=2),
+        headers: Dict[str, str] = None,
+    ):
+        """
+        uri: str
+            where to connect
+        verbose_log: bool = False
+            should the websocket client also log using the builtin
+        reconnect_interval: timedelta = timedelta(seconds=2)
+            time interval to wait before trying to reconnect (must be >= 1 second)
+        headers: Dict[str, str] = None
+            headers to apply to the request during the handshake
+        """
+        assert reconnect_interval >= timedelta(seconds=1)
+        self._properties = dict(
+            uri=uri,
+            verbose_log=verbose_log,
+            reconnect_interval=reconnect_interval,
+            headers=headers if headers else {},
+            use_tls=uri.startswith("wss"),
+        )
+
+    def subscribe(
+        self,
+        ts_type: type,
+        msg_mapper: MsgMapper,
+        field_map: typing.Union[dict, str] = None,
+        meta_field_map: dict = None,
+        push_mode: csp.PushMode = csp.PushMode.NON_COLLAPSING,
+    ):
+        field_map = field_map or {}
+        meta_field_map = meta_field_map or {}
+        if isinstance(field_map, str):
+            field_map = {field_map: ""}
+
+        if not field_map and issubclass(ts_type, csp.Struct):
+            field_map = ts_type.default_field_map()
+
+        properties = msg_mapper.properties.copy()
+        properties["field_map"] = field_map
+        properties["meta_field_map"] = meta_field_map
+
+        return _websocket_input_adapter_def(self, ts_type, properties, push_mode)
+
+    def send(self, x: ts["T"]):
+        return _websocket_output_adapter_def(self, x)
+
+    def update_headers(self, x: ts[List[str]]):
+        return _websocket_header_update_adapter_def(self, x)
+
+    def status(self, push_mode=csp.PushMode.NON_COLLAPSING):
+        ts_type = Status
+        return status_adapter_def(self, ts_type, push_mode)
+
+    def _create(self, engine, memo):
+        """method needs to return the wrapped c++ adapter manager"""
+        return _websocketadapterimpl._websocket_adapter_manager(engine, self._properties)
+
+
+_websocket_input_adapter_def = input_adapter_def(
+    "websocket_input_adapter",
+    _websocketadapterimpl._websocket_input_adapter,
+    ts["T"],
+    WebsocketAdapterManager,
+    typ="T",
+    properties=dict,
+)
+
+_websocket_output_adapter_def = output_adapter_def(
+    "websocket_output_adapter",
+    _websocketadapterimpl._websocket_output_adapter,
+    WebsocketAdapterManager,
+    input=ts["T"],
+)
+
+_websocket_header_update_adapter_def = output_adapter_def(
+    "websocket_header_update_adapter",
+    _websocketadapterimpl._websocket_header_update_adapter,
+    WebsocketAdapterManager,
+    input=ts[List[WebsocketHeaderUpdate]],
+)
```

### Comparing `csp-0.0.2/csp/baselib.py` & `csp-0.0.3/csp/baselib.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/basketlib.py` & `csp-0.0.3/csp/basketlib.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/build/csp_autogen.py` & `csp-0.0.3/csp/build/csp_autogen.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/cache_support.py` & `csp-0.0.3/csp/cache_support.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/curve.py` & `csp-0.0.3/csp/curve.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/dataframe.py` & `csp-0.0.3/csp/dataframe.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/adaptermanager.py` & `csp-0.0.3/csp/impl/adaptermanager.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/builtin_functions.py` & `csp-0.0.3/csp/impl/builtin_functions.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/config.py` & `csp-0.0.3/csp/impl/config.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/enum.py` & `csp-0.0.3/csp/impl/enum.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/error_handling.py` & `csp-0.0.3/csp/impl/error_handling.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/genericpushadapter.py` & `csp-0.0.3/csp/impl/genericpushadapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/aggregation_period_utils.py` & `csp-0.0.3/csp/impl/managed_dataset/aggregation_period_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/cache_partition_argument_serializer.py` & `csp-0.0.3/csp/impl/managed_dataset/cache_partition_argument_serializer.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/dataset_metadata.py` & `csp-0.0.3/csp/impl/managed_dataset/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/managed_dataset.py` & `csp-0.0.3/csp/impl/managed_dataset/managed_dataset.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/managed_dataset_lock_file_util.py` & `csp-0.0.3/csp/impl/managed_dataset/managed_dataset_lock_file_util.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/managed_dataset_merge_utils.py` & `csp-0.0.3/csp/impl/managed_dataset/managed_dataset_merge_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/managed_dataset_path_resolver.py` & `csp-0.0.3/csp/impl/managed_dataset/managed_dataset_path_resolver.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/managed_dataset/managed_parquet_writer.py` & `csp-0.0.3/csp/impl/managed_dataset/managed_parquet_writer.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/mem_cache.py` & `csp-0.0.3/csp/impl/mem_cache.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/pandas.py` & `csp-0.0.3/csp/impl/pandas.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/pandas_accessor.py` & `csp-0.0.3/csp/impl/pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/pandas_ext_type.py` & `csp-0.0.3/csp/impl/pandas_ext_type.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/pandas_perspective.py` & `csp-0.0.3/csp/impl/pandas_perspective.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/pulladapter.py` & `csp-0.0.3/csp/impl/pulladapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/struct.py` & `csp-0.0.3/csp/impl/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
     @classmethod
     def from_dict(cls, json: dict):
         return cls._obj_from_python(json, cls)
 
     def to_dict(self):
         return self._obj_to_python(self)
 
+    def to_json(self, callback=lambda x: x):
+        return super().to_json(callback)
+
     def to_yaml(self):
         string_io = io.StringIO()
         g_YAML.dump(self.to_dict(), string_io)
         return string_io.getvalue()
 
     @classmethod
     def default_field_map(cls):
```

### Comparing `csp-0.0.2/csp/impl/types/autogen_types.py` & `csp-0.0.3/csp/impl/types/autogen_types.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/common_definitions.py` & `csp-0.0.3/csp/impl/types/common_definitions.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/container_type_normalizer.py` & `csp-0.0.3/csp/impl/types/container_type_normalizer.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/generic_values_resolver.py` & `csp-0.0.3/csp/impl/types/generic_values_resolver.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/instantiation_type_resolver.py` & `csp-0.0.3/csp/impl/types/instantiation_type_resolver.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/tstype.py` & `csp-0.0.3/csp/impl/types/tstype.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/type_annotation_normalizer_transformer.py` & `csp-0.0.3/csp/impl/types/type_annotation_normalizer_transformer.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/types/typing_utils.py` & `csp-0.0.3/csp/impl/types/typing_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/warnings.py` & `csp-0.0.3/csp/impl/warnings.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/__init__.py` & `csp-0.0.3/csp/impl/wiring/__init__.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/adapters.py` & `csp-0.0.3/csp/impl/wiring/adapters.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/ast_utils.py` & `csp-0.0.3/csp/impl/wiring/ast_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/base_parser.py` & `csp-0.0.3/csp/impl/wiring/base_parser.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/cache_config_resolver.py` & `csp-0.0.3/csp/impl/wiring/cache_support/cache_config_resolver.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/cache_type_mapper.py` & `csp-0.0.3/csp/impl/wiring/cache_support/cache_type_mapper.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/dataset_partition_cached_data.py` & `csp-0.0.3/csp/impl/wiring/cache_support/dataset_partition_cached_data.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/graph_building.py` & `csp-0.0.3/csp/impl/wiring/cache_support/graph_building.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/partition_files_container.py` & `csp-0.0.3/csp/impl/wiring/cache_support/partition_files_container.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/cache_support/runtime_cache_manager.py` & `csp-0.0.3/csp/impl/wiring/cache_support/runtime_cache_manager.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/context.py` & `csp-0.0.3/csp/impl/wiring/context.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/delayed_edge.py` & `csp-0.0.3/csp/impl/wiring/delayed_edge.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/delayed_node.py` & `csp-0.0.3/csp/impl/wiring/delayed_node.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/dynamic.py` & `csp-0.0.3/csp/impl/wiring/dynamic.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/edge.py` & `csp-0.0.3/csp/impl/wiring/edge.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/feedback.py` & `csp-0.0.3/csp/impl/wiring/feedback.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/graph.py` & `csp-0.0.3/csp/impl/wiring/graph.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/graph_parser.py` & `csp-0.0.3/csp/impl/wiring/graph_parser.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/node.py` & `csp-0.0.3/csp/impl/wiring/node.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/node_parser.py` & `csp-0.0.3/csp/impl/wiring/node_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,25 +837,31 @@
         self._validate_return_statements()
 
         # apply transform to stateblock and startblock after signature is ready for alarms and passive calls
         self._stateblock = [self.visit(node) for node in self._stateblock]
         self._startblock = [self.visit(node) for node in self._startblock]
 
         init_block = node_proxy + ts_in_proxies + ts_out_proxies + ts_vars
-
-        # Yield before start block so we can setup stack frame before executing
-        startblock = [ast.Expr(value=ast.Yield(value=None))] + self._stateblock + self._startblock
-
-        start_and_body = startblock + [ast.While(test=ast.NameConstant(value=True), orelse=[], body=innerbody)]
+        startblock = self._stateblock + self._startblock
+        body = [ast.While(test=ast.NameConstant(value=True), orelse=[], body=innerbody)]
 
         if self._stopblock:
             self._stopblock = [self.visit(node) for node in self._stopblock]
-            # For stop we wrap start and body in a try / finally ( not the init block, if that fails it's unrecoverable )
-            start_and_body = [ast.Try(body=start_and_body, finalbody=self._stopblock, handlers=[], orelse=[])]
 
+            # For stop we wrap the body of a node in a try / finally
+            # If the init block fails it's unrecoverable, and if the start block raises we don't want to stop that specific node
+            start_and_body = startblock + [ast.Try(body=body, finalbody=self._stopblock, handlers=[], orelse=[])]
+
+        else:
+            start_and_body = startblock + body
+
+        # Yield before start block so we can setup stack frame before executing
+        # However, this initial yield shouldn't be within the try-finally block, since if a node does not start, it's stop() logic should not be invoked
+        # This avoids an issue where one node raises an exception upon start(), and then other nodes execute their stop() without having ever started
+        start_and_body = [ast.Expr(value=ast.Yield(value=None))] + start_and_body
         newbody = init_block + start_and_body
 
         newfuncdef = ast.FunctionDef(name=self._name, body=newbody, returns=None)
         newfuncdef.args = self._create_ast_args(
             posonlyargs=[], args=[], kwonlyargs=[], defaults=[], vararg=None, kwarg=None, kw_defaults=[]
         )
         newfuncdef.decorator_list = []
```

### Comparing `csp-0.0.2/csp/impl/wiring/numba_node.py` & `csp-0.0.3/csp/impl/wiring/numba_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,25 @@
     def _create(self, engine, memo):
         from csp.impl.wiring.numba_utils.csp_cpp_numba_interface import NumbaTSTypedFunctionResolver, ffi_ptr_to_int
         from csp.impl.wiring.numba_utils.numba_type_resolver import NumbaTypeResolver
 
         exposed_utility_values = {}
         cache_key = [self._impl]
         for (ts_idx, basket_idx), input in self.ts_inputs():
-            exposed_utility_values[
-                NumbaNodeParser.get_ts_input_value_getter_name(ts_idx)
-            ] = NumbaTSTypedFunctionResolver.get_value_getter_function(input.tstype.typ)
+            exposed_utility_values[NumbaNodeParser.get_ts_input_value_getter_name(ts_idx)] = (
+                NumbaTSTypedFunctionResolver.get_value_getter_function(input.tstype.typ)
+            )
             cache_key.append(input.tstype)
 
         for output in self._outputs:
             assert output.kind.is_single_ts()
             ts_idx = output.ts_idx
-            exposed_utility_values[
-                NumbaNodeParser.get_ts_out_value_return_name(ts_idx)
-            ] = NumbaTSTypedFunctionResolver.get_value_returner_function(output.typ.typ)
+            exposed_utility_values[NumbaNodeParser.get_ts_out_value_return_name(ts_idx)] = (
+                NumbaTSTypedFunctionResolver.get_value_returner_function(output.typ.typ)
+            )
 
         numba_scalar_types = []
         for i in self._signature.raw_inputs():
             if i.kind.is_scalar():
                 resolved_python_type = GenericValuesResolver.resolve_generic_values(i.typ, self._tvars)
                 numba_type = NumbaTypeResolver.resolve_numba_type(resolved_python_type)
                 exposed_utility_values[NumbaNodeParser.get_arg_type_var_name(i.name)] = numba_type
```

### Comparing `csp-0.0.2/csp/impl/wiring/numba_node_parser.py` & `csp-0.0.3/csp/impl/wiring/numba_node_parser.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/numba_utils/csp_cpp_numba_interface.py` & `csp-0.0.3/csp/impl/wiring/numba_utils/csp_cpp_numba_interface.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/numba_utils/csp_numba_functions.py` & `csp-0.0.3/csp/impl/wiring/numba_utils/csp_numba_functions.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/numba_utils/csp_string_extension.py` & `csp-0.0.3/csp/impl/wiring/numba_utils/csp_string_extension.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/numba_utils/datetime_extension.py` & `csp-0.0.3/csp/impl/wiring/numba_utils/datetime_extension.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/numba_utils/numba_type_resolver.py` & `csp-0.0.3/csp/impl/wiring/numba_utils/numba_type_resolver.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/outputs.py` & `csp-0.0.3/csp/impl/wiring/outputs.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/runtime.py` & `csp-0.0.3/csp/impl/wiring/runtime.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/signature.py` & `csp-0.0.3/csp/impl/wiring/signature.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/impl/wiring/threaded_runtime.py` & `csp-0.0.3/csp/impl/wiring/threaded_runtime.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/math.py` & `csp-0.0.3/csp/math.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/profiler.py` & `csp-0.0.3/csp/profiler.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/random.py` & `csp-0.0.3/csp/random.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/showgraph.py` & `csp-0.0.3/csp/showgraph.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/stats.py` & `csp-0.0.3/csp/stats.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/arrow_test_data.arrow` & `csp-0.0.3/csp/tests/adapters/arrow_test_data.arrow`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/kafka_utils.py` & `csp-0.0.3/csp/tests/adapters/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/parquet_test_data.parquet` & `csp-0.0.3/csp/tests/adapters/parquet_test_data.parquet`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_csv.py` & `csp-0.0.3/csp/tests/adapters/test_csv.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_db.py` & `csp-0.0.3/csp/tests/adapters/test_db.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_kafka.py` & `csp-0.0.3/csp/tests/adapters/test_kafka.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_numpy.py` & `csp-0.0.3/csp/tests/adapters/test_numpy.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_parquet.py` & `csp-0.0.3/csp/tests/adapters/test_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
 import numpy
 import os
 import pandas
-import platform
 import polars
 import pyarrow
 import pyarrow.parquet
-import pytest
 import pytz
 import tempfile
 import unittest
 from datetime import datetime, timedelta
 
 import csp
 from csp.adapters.output_adapters.parquet import ParquetOutputConfig
@@ -30,15 +28,14 @@
     side: str
 
 
 parquet_filename = os.path.join(os.path.dirname(__file__), "parquet_test_data.parquet")
 arrow_filename = os.path.join(os.path.dirname(__file__), "arrow_test_data.arrow")
 
 
-@pytest.mark.skipif(platform.system() == "Darwin", reason="Does not run on macOS")
 class TestParquetReader(unittest.TestCase):
     def do_test_body(self, filename, arrow=False):
         @csp.graph
         def write_ts_to_file(x: csp.ts["T"]):
             temp_file = tempfile.NamedTemporaryFile(prefix="csp_unit_tests", mode="w")
             temp_file.close()
             csp.schedule_on_engine_stop(lambda: os.unlink(temp_file.name))
```

### Comparing `csp-0.0.2/csp/tests/adapters/test_slack.py` & `csp-0.0.3/csp/tests/adapters/test_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from datetime import timedelta
+from ssl import create_default_context
 from unittest.mock import MagicMock, call, patch
 
 import csp
 from csp import ts
 from csp.adapters.slack import SlackAdapterManager, SlackMessage, mention_user
 
 
@@ -151,15 +152,15 @@
                     {"name": "a private channel", "id": "EFGH"},
                     {"name": "a new channel", "id": "new_channel"},
                 ]
             }
             clientmock.return_value.web_client.conversations_list.return_value = mock_list_response
 
             def graph():
-                am = SlackAdapterManager("xapp-1-dummy", "xoxb-dummy")
+                am = SlackAdapterManager("xapp-1-dummy", "xoxb-dummy", ssl=create_default_context())
 
                 # send a fake slack message to the app
                 stop = send_fake_message(clientmock, reqmock, am)
 
                 # send a response
                 resp = hello(csp.unroll(am.subscribe()))
                 am.publish(resp)
```

### Comparing `csp-0.0.2/csp/tests/adapters/test_status.py` & `csp-0.0.3/csp/tests/adapters/test_status.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/adapters/test_symphony.py` & `csp-0.0.3/csp/tests/adapters/test_symphony.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_dateframe.py` & `csp-0.0.3/csp/tests/impl/test_dateframe.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_enum.py` & `csp-0.0.3/csp/tests/impl/test_enum.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_genericpushadapter.py` & `csp-0.0.3/csp/tests/impl/test_genericpushadapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_numba_features_support.py` & `csp-0.0.3/csp/tests/impl/test_numba_features_support.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_outputadapter.py` & `csp-0.0.3/csp/tests/impl/test_outputadapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pandas.py` & `csp-0.0.3/csp/tests/impl/test_pandas.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pandas_accessor.py` & `csp-0.0.3/csp/tests/impl/test_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pandas_ext_type.py` & `csp-0.0.3/csp/tests/impl/test_pandas_ext_type.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pandas_perspective.py` & `csp-0.0.3/csp/tests/impl/test_pandas_perspective.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pulladapter.py` & `csp-0.0.3/csp/tests/impl/test_pulladapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pushadapter.py` & `csp-0.0.3/csp/tests/impl/test_pushadapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/test_pushpulladapter.py` & `csp-0.0.3/csp/tests/impl/test_pushpulladapter.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/utils/test_lock_file.py` & `csp-0.0.3/csp/tests/impl/utils/test_lock_file.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/numba_utils/test_numba_datetime_extension.py` & `csp-0.0.3/csp/tests/impl/wiring/numba_utils/test_numba_datetime_extension.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/test_alarms.py` & `csp-0.0.3/csp/tests/impl/wiring/test_alarms.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/test_basket_outputs.py` & `csp-0.0.3/csp/tests/impl/wiring/test_basket_outputs.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/test_edge.py` & `csp-0.0.3/csp/tests/impl/wiring/test_edge.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/test_state.py` & `csp-0.0.3/csp/tests/impl/wiring/test_state.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/impl/wiring/test_threaded_runtime.py` & `csp-0.0.3/csp/tests/impl/wiring/test_threaded_runtime.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_baselib.py` & `csp-0.0.3/csp/tests/test_baselib.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,14 +883,15 @@
             d: datetime
             t: timedelta
             dt: date
             e: MyEnum
             st: MyStruct
             o: MyObject
             l: [int]
+            lb: [bool]
 
         @csp.node
         def random_gen(trigger: ts[object], typ: "T") -> ts["T"]:
             if csp.ticked(trigger):
                 v = 1000 * random.random()
                 if typ is MyStruct:
                     return MyStruct(value=v)
@@ -905,15 +906,16 @@
                 if typ is timedelta:
                     return timedelta(seconds=v)
                 if typ is date:
                     return date.today() + timedelta(days=v)
                 if typ is MyEnum:
                     return MyEnum(int(v) % 5)
                 if isinstance(typ, list):
-                    return [int(v), int(v * 2)]
+                    elem_type = typ[0]
+                    return [elem_type(v), elem_type(v * 2)]
                 return typ(v)
 
         @csp.node
         def random_gen_nan(trigger: ts[object]) -> ts[float]:
             if csp.ticked(trigger):
                 if random.random() < 0.2:
                     return float("nan")
```

### Comparing `csp-0.0.2/csp/tests/test_basketlib.py` & `csp-0.0.3/csp/tests/test_basketlib.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_baskets.py` & `csp-0.0.3/csp/tests/test_baskets.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_build.py` & `csp-0.0.3/csp/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_caching.py` & `csp-0.0.3/csp/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_curve.py` & `csp-0.0.3/csp/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_dynamic.py` & `csp-0.0.3/csp/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_engine.py` & `csp-0.0.3/csp/tests/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from datetime import datetime, timedelta
 
 import csp
 from csp import PushMode, ts
 from csp.impl.types.instantiation_type_resolver import ArgTypeMismatchError, TSArgTypeMismatchError
 from csp.impl.wiring.delayed_node import DelayedNodeWrapperDef
 from csp.impl.wiring.runtime import build_graph
+from csp.lib import _csptestlibimpl
 
 
 @csp.graph
 def _dummy_graph():
     raise NotImplementedError()
 
 
@@ -1329,15 +1330,15 @@
         """range check when converting datetime"""
         for d in [
             datetime(2020, 12, 24, 1, 2, 3, 123456),
             datetime(1970, 1, 1),
             datetime(1969, 5, 6, 2, 3, 4),
             datetime(1969, 5, 6, 2, 3, 4, 123456),
             # Edge cases, DateTime MIN / MAX
-            datetime(1678, 1, 1),
+            datetime(1678, 1, 1) if sys.platform == "linux" else datetime(1970, 1, 1),
             datetime(2261, 12, 31, 23, 59, 59, 999999),
             timedelta(days=1, seconds=3600, microseconds=123456),
             timedelta(days=-1, seconds=3600, microseconds=123456),
         ]:
             res = csp.run(csp.const(d), starttime=datetime(2020, 12, 24))[0][0][1]
             self.assertEqual(res, d, f"date: {d}")
 
@@ -1974,10 +1975,95 @@
                     my_node(c)
                     data = MyPullAdapter()
                     csp.add_graph_output(str(i), data)
 
         with self.assertRaisesRegex(RuntimeError, "all good"):
             csp.run(g, starttime=datetime(2023, 1, 1), endtime=timedelta(1))
 
+    def test_stop_cannot_be_called_without_start(self):
+        """
+        Was a BUG where one node raising an exception during its start block led to other nodes exeucting their stop block without ever starting
+        """
+        status = {"foo_started": False, "foo_stopped": False, "bar_started": False, "bar_stopped": False}
+
+        # Python nodes (use try-finally logic for stopping)
+
+        @csp.node
+        def foo():
+            with csp.start():
+                status["foo_started"] = True
+                raise RuntimeError("foo!")
+
+            with csp.stop():
+                status["foo_stopped"] = True
+
+        @csp.node
+        def bar():
+            with csp.start():
+                status["bar_started"] = True
+
+            with csp.stop():
+                status["bar_stopped"] = True
+
+        @csp.graph
+        def my_graph():
+            foo()
+            bar()
+
+        with self.assertRaises(RuntimeError):
+            csp.run(my_graph, realtime=True)
+
+        self.assertTrue(status["foo_started"] and not status["foo_stopped"])
+        self.assertFalse(status["bar_started"] or status["bar_stopped"])
+
+        # C++ nodes (stop is initiated by the engine)
+
+        class RunInfo:
+            def __init__(self):
+                self.n1_started = False
+                self.n2_started = False
+                self.n1_stopped = False
+                self.n2_stopped = False
+
+        @csp.node(cppimpl=_csptestlibimpl.start_n1_set_value)
+        def n1(obj_: RunInfo):
+            return
+
+        @csp.node(cppimpl=_csptestlibimpl.start_n2_throw)
+        def n2(obj_: RunInfo):
+            return
+
+        myd = RunInfo()
+
+        @csp.graph
+        def g():
+            n1(myd)
+            n2(myd)
+
+        with self.assertRaises(ValueError):
+            csp.run(g, realtime=True)
+
+        self.assertTrue(myd.n1_started and myd.n1_stopped)
+        self.assertFalse(myd.n2_started or myd.n2_stopped)
+
+        # Test case where node starts, never ticks, and then stops
+        status = {"started": False, "stopped": False}
+
+        @csp.node
+        def n3(x: ts[int]) -> ts[int]:
+            with csp.start():
+                status["started"] = True
+            with csp.stop():
+                status["stopped"] = True
+
+            return 0
+
+        @csp.graph
+        def g() -> ts[int]:
+            return n3(csp.null_ts(int))
+
+        csp.run(g, starttime=datetime(2020, 1, 1), endtime=timedelta())
+        self.assertTrue(status["started"] and status["stopped"])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `csp-0.0.2/csp/tests/test_examples.py` & `csp-0.0.3/csp/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_graph_mem_cache.py` & `csp-0.0.3/csp/tests/test_graph_mem_cache.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_history.py` & `csp-0.0.3/csp/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_math.py` & `csp-0.0.3/csp/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_numba_features.py` & `csp-0.0.3/csp/tests/test_numba_features.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_numba_type_checking.py` & `csp-0.0.3/csp/tests/test_numba_type_checking.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_parsing.py` & `csp-0.0.3/csp/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_profiler.py` & `csp-0.0.3/csp/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_random.py` & `csp-0.0.3/csp/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_showgraph.py` & `csp-0.0.3/csp/tests/test_showgraph.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_stats.py` & `csp-0.0.3/csp/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/test_type_checking.py` & `csp-0.0.3/csp/tests/test_type_checking.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/utils/test_object_factory.py` & `csp-0.0.3/csp/tests/utils/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/tests/utils/typed_curve_generator.py` & `csp-0.0.3/csp/tests/utils/typed_curve_generator.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/typing.py` & `csp-0.0.3/csp/typing.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/utils/csp_watch_profile.py` & `csp-0.0.3/csp/utils/csp_watch_profile.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/utils/file_permissions.py` & `csp-0.0.3/csp/utils/file_permissions.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/utils/lock_file.py` & `csp-0.0.3/csp/utils/lock_file.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/utils/object_factory_registry.py` & `csp-0.0.3/csp/utils/object_factory_registry.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp/utils/qualified_name_utils.py` & `csp-0.0.3/csp/utils/qualified_name_utils.py`

 * *Files identical despite different names*

### Comparing `csp-0.0.2/csp.egg-info/PKG-INFO` & `csp-0.0.3/csp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp
-Version: 0.0.2
+Version: 0.0.3
 Summary: csp is a high performance reactive stream processing library, written in C++ and Python
 Author-email: the csp authors <CSPOpenSource@point72.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `csp-0.0.2/csp.egg-info/SOURCES.txt` & `csp-0.0.3/csp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,25 @@
 cpp/csp/adapters/utils/ProtobufHelper.h
 cpp/csp/adapters/utils/ProtobufMessageStructConverter.cpp
 cpp/csp/adapters/utils/ProtobufMessageStructConverter.h
 cpp/csp/adapters/utils/RawBytesMessageStructConverter.cpp
 cpp/csp/adapters/utils/RawBytesMessageStructConverter.h
 cpp/csp/adapters/utils/StructAdapterInfo.h
 cpp/csp/adapters/utils/ValueDispatcher.h
+cpp/csp/adapters/websocket/CMakeLists.txt
+cpp/csp/adapters/websocket/ClientAdapterManager.cpp
+cpp/csp/adapters/websocket/ClientAdapterManager.h
+cpp/csp/adapters/websocket/ClientHeaderUpdateAdapter.cpp
+cpp/csp/adapters/websocket/ClientHeaderUpdateAdapter.h
+cpp/csp/adapters/websocket/ClientInputAdapter.cpp
+cpp/csp/adapters/websocket/ClientInputAdapter.h
+cpp/csp/adapters/websocket/ClientOutputAdapter.cpp
+cpp/csp/adapters/websocket/ClientOutputAdapter.h
+cpp/csp/adapters/websocket/WebsocketEndpoint.cpp
+cpp/csp/adapters/websocket/WebsocketEndpoint.h
 cpp/csp/core/BasicAllocator.h
 cpp/csp/core/CMakeLists.txt
 cpp/csp/core/Config.h.in
 cpp/csp/core/DynamicBitSet.h
 cpp/csp/core/Enum.h
 cpp/csp/core/EnumBitSet.h
 cpp/csp/core/Exception.cpp
@@ -234,26 +245,30 @@
 cpp/csp/python/PyOutputProxy.h
 cpp/csp/python/PyPullInputAdapter.cpp
 cpp/csp/python/PyPushInputAdapter.cpp
 cpp/csp/python/PyPushInputAdapter.h
 cpp/csp/python/PyPushPullInputAdapter.cpp
 cpp/csp/python/PyStruct.cpp
 cpp/csp/python/PyStruct.h
+cpp/csp/python/PyStructToJson.cpp
+cpp/csp/python/PyStructToJson.h
 cpp/csp/python/PyTimerAdapter.cpp
 cpp/csp/python/cspbaselibimpl.cpp
 cpp/csp/python/cspbasketlibimpl.cpp
 cpp/csp/python/cspimpl.cpp
 cpp/csp/python/cspmathimpl.cpp
 cpp/csp/python/cspnpstatsimpl.cpp
 cpp/csp/python/cspstatsimpl.cpp
+cpp/csp/python/csptestlibimpl.cpp
 cpp/csp/python/csptypesimpl.cpp
 cpp/csp/python/npstatsimpl.cpp
 cpp/csp/python/adapters/CMakeLists.txt
 cpp/csp/python/adapters/kafkaadapterimpl.cpp
 cpp/csp/python/adapters/parquetadapterimpl.cpp
+cpp/csp/python/adapters/websocketadapterimpl.cpp
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/CMakeLists.txt
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/api.h
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.cc
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_pandas.h
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/arrow_to_python_internal.h
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/async.h
 cpp/csp/python/adapters/vendored/pyarrow-15.0.0/arrow/python/benchmark.cc
@@ -405,14 +420,15 @@
 csp/adapters/parquet.py
 csp/adapters/perspective.py
 csp/adapters/slack.py
 csp/adapters/status.py
 csp/adapters/symphony.py
 csp/adapters/utils.py
 csp/adapters/websocket.py
+csp/adapters/websocket_types.py
 csp/adapters/output_adapters/__init__.py
 csp/adapters/output_adapters/parquet.py
 csp/adapters/output_adapters/parquet_utility_nodes.py
 csp/build/csp_autogen.py
 csp/impl/__cspimpl.py
 csp/impl/__csptypesimpl.py
 csp/impl/__init__.py
```

### Comparing `csp-0.0.2/pyproject.toml` & `csp-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "csp"
 authors = [{name = "the csp authors", email = "CSPOpenSource@point72.com"}]
 description="csp is a high performance reactive stream processing library, written in C++ and Python"
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.8"
 
 dependencies = [
     "backports.zoneinfo; python_version<'3.9'",
     "numpy",
     "packaging",
     "pandas",
@@ -118,15 +118,15 @@
 include_trailing_comma = true
 line_length = 120
 profile = "black"
 
 default_section = "THIRDPARTY"
 sections = "FUTURE,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
-known_first_party = "nbprint"
+known_first_party = "csp"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 testpaths = "csp/tests"
 
 [tool.ruff]
 line-length = 120
```

