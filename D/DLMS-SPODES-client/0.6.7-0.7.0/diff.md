# Comparing `tmp/DLMS_SPODES_client-0.6.7.tar.gz` & `tmp/DLMS_SPODES_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.6.7.tar", last modified: Mon Apr  1 09:10:02 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.7.0.tar", last modified: Fri Apr  5 11:32:59 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.6.7.tar` & `DLMS_SPODES_client-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.599598 DLMS_SPODES_client-0.6.7/
--rw-rw-rw-   0        0        0      526 2024-04-01 09:10:02.598598 DLMS_SPODES_client-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.6.7/README.md
--rw-rw-rw-   0        0        0      836 2024-04-01 09:07:57.000000 DLMS_SPODES_client-0.6.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 09:10:02.599598 DLMS_SPODES_client-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.457596 DLMS_SPODES_client-0.6.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.473596 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   124160 2024-03-21 12:07:16.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.411489 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.490596 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.537604 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.592597 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.594598 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     4646 2024-03-27 10:40:49.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0    10450 2024-04-01 08:44:58.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.486596 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3206 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-01 09:10:02.000000 DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.6.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:10:02.596598 DLMS_SPODES_client-0.6.7/test/
--rw-rw-rw-   0        0        0     5227 2024-04-01 08:49:08.000000 DLMS_SPODES_client-0.6.7/test/test_Client.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.425579 DLMS_SPODES_client-0.7.0/
+-rw-rw-rw-   0        0        0      526 2024-04-05 11:32:59.424549 DLMS_SPODES_client-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.0/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-05 11:05:18.000000 DLMS_SPODES_client-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 11:32:59.425579 DLMS_SPODES_client-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.278544 DLMS_SPODES_client-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.294549 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   122710 2024-04-05 07:42:39.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/client.py
+-rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.231186 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.312546 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.362545 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.418579 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.420547 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0    35025 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.308578 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-05 11:32:59.000000 DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:32:59.422546 DLMS_SPODES_client-0.7.0/test/
+-rw-rw-rw-   0        0        0     7036 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.0/test/test_Client.py
```

### Comparing `DLMS_SPODES_client-0.6.7/PKG-INFO` & `DLMS_SPODES_client-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.6.7
+Version: 0.7.0
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.6.7/pyproject.toml` & `DLMS_SPODES_client-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.6.7"
+version = "0.7.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS-SPODES == 0.68.3",
+    "DLMS-SPODES == 0.69.3",
     "DLMS-SPODES-communications >= 1.2.3",
     "pycryptodomex>=3.15"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=['dlms', 'spodes', 'client']
```

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 class Client:
     id_count = count()
     __status: Status
     log_file: TextIO
     media: Network | SerialPort | RS485 | BLE | AsyncNetwork | AsyncSerial | None
-    __lock: threading.Lock
+    lock: threading.Lock
     errors: Errors
     last_transfer_time: datetime.timedelta | None
     connection_time_release: int
     received_frames: Deque[frame.Frame]
     __stop_transfer: bool
     current_obj: InterfaceClass | None
     reply: GXReplyData
@@ -143,15 +143,15 @@
         self.__status = Status.READY
         # file_name = F"./Logs/{id_}.log"
         self.trace = TraceLevel.VERBOSE
         self.protocol_version = cdt.BitString('1')  # max 8 bit
         """ Protocol Version of the AARQ APDU """
         # TODO: REMOVE IT BULLSHIT
         self.invocationCounter = '0.0.43.1.0.255'
-        self.__lock = threading.Lock()
+        self.lock = threading.Lock()
         """ lock for exchange access to device """
         self.errors = Errors()   # last errors
         self.device_address = cdt.LongUnsigned(16)
         """physical address from HDLC setup, lower address in HDLC frame"""
         self.addr_size = frame.AddressLength(addr_size)
         """server address size, -1 is AUTO"""
         self.m_id = mechanism_id.MechanismIdElement(0)
@@ -990,30 +990,16 @@
                 case {SerialPort.__class__.__name__: dict_}:
                     self.media = eval(F"SerialPort({dict_})")
                 case _: raise ValueError(F"unknown type: {value.__class__.__name__} for set communication channel {self}")
             self.log(logL.INFO, F"set2 to {self} communication channel: {self.media}")
         except Exception as e:
             self.log(logL.ERR, F"not set to {self} communication channel by {value}")
 
-    def __unlock(self):
-        self.__lock.release()
-
-    def lock(self, value: str):
-        self.__lock.acquire()
-        self.locker_name = value
-
-    def unlock(self, value: str):
-        if self.locker_name == value:
-            self.__lock.release()
-        else:
-            raise exc.ITEApplication(F"can't unlock {self} by {value}, only by {self.locker_name}")
-
     async def connect(self, is_public: bool = False):
         """ connect to server with opening port"""
-        self.lock("for connect")
         self.__status = Status.EXCHANGE
         self.set_error(Transmit.OK, "Open port")
         # elif self.__lock.locked():
         #     self.log(logL.WARN, F"locked by {self.locker_name}")
         #     if isinstance(self.media, SerialPort):
         #         raise exc.NoTransport("temporary locked for serial port")
         # init SA, DA, device_address
@@ -1030,25 +1016,14 @@
             self.DA = frame.Address(
                 upper_address=int(self.server_SAP),
                 lower_address=int(self.device_address) if self.device_address else None,
                 length=self.addr_size
             )
             self.SA = frame.Address(upper_address=0x10 if is_public else int(self.SAP))
             self.log(logL.INFO, F"{self.SA=} {self.DA=}")
-            # open communication channel
-            await self.media.open()
-            self.set_error(Transmit.OK, "Open port")
-            self.log(logL.INFO, F"Open port communication channel: {self.media}")
-        except (ConnectionRefusedError, TimeoutError) as e:
-            self.__unlock()
-            raise exc.NoPort(F'communication channel: {self.media}. {e}')
-        except Exception as e:
-            self.__unlock()
-            raise ConnectionError(F"{e}")
-        try:
             # initialize connection
             self.reply.clear()
             if self.settings.cipher.security != Security.NONE:
                 self.log(logL.DEB, F"Security: {self.settings.cipher.security}/n"
                                    F"System title: {self.settings.cipher.systemTitle.hex()}"
                                    F"Authentication key: {self.settings.cipher.authenticationKey.hex()}"
                                    F"Block cipher key: {self.settings.cipher.blockCipherKey.hex()}")
@@ -1070,15 +1045,15 @@
                     self.current_association.associated_partners_id.client_SAP.set(0x10)
                     self.get_SNRM_request()
                     self.__status = Status.READ
                     await self.read_data_block()
                     self.objects.getIECHDLCSetup(self.get_channel_index()).set_from_info(self.reply.data.get_data())
                     self.settings.connected = ConnectionState.HDLC
                     self.reply.clear()
-                    self.aarqRequest()
+                    self.aarqRequest(self.m_id)
                     await self.read_data_block()
                     self.parseAareResponse(self.reply.data)
                     self.reply.clear()
                     self.read_attribute(IC, 2)
                     self.settings.cipher.invocationCounter = 1 + IC.value.decode()
                     self.log(logL.DEB, "Invocation counter: " + str(self.settings.cipher.invocationCounter))
                     # disconnect
@@ -1134,15 +1109,15 @@
             if self.settings.interfaceType == InterfaceType.HDLC:
                 self.get_SNRM_request()
                 self.__status = Status.READ
                 await self.read_data_block()
                 self.__status = Status.EXCHANGE
                 self.settings.connected = ConnectionState.HDLC
                 self.reply.clear()
-                self.aarqRequest()
+                self.aarqRequest(mechanism_id.NONE if is_public else self.m_id)
                 await self.read_data_block()
                 # await self.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
             match self.parseAareResponse(self.reply.data):
                 case AcseServiceUser.NULL:                                             self.log(logL.INFO, 'Authentication success')
                 case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public: self.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
                 case AcseServiceUser.AUTHENTICATION_REQUIRED:
                     self.reply.clear()
@@ -1160,45 +1135,33 @@
         except GXDLMSException as e:
             raise exc.UnknownError(F'При соединении {e}')
         except TimeoutError as e:
             raise exc.Timeout('При соединении')
 
     async def close(self):
         """ send DISC to server and after close media """
-        if self.media and self.media.is_open():
-            self.log(logL.DEB, "DisconnectRequest")
-            try:
-                # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
-                if self.settings.interfaceType == InterfaceType.WRAPPER or \
-                        (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
-                    self.releaseRequest()
-                    await self.read_data_block()
-            except Exception:
-                pass
-                #  All meters don't support release.
-            try:
-                await self.disconnect_request()
-            except Exception as e:
-                self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
-                self.received_frames.clear()  # for next exchange need clear all received frames
-            await self.media.close()
+        self.log(logL.DEB, "DisconnectRequest")
+        try:
+            # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
+            if self.settings.interfaceType == InterfaceType.WRAPPER or \
+                    (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
+                self.releaseRequest()
+                await self.read_data_block()
+        except Exception:
+            self.log(logL.WARN, "don't support release ReleaseRequest")
+            pass
+            #  All meters don't support release.
+        try:
+            await self.disconnect_request()
+        except Exception as e:
+            self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
         self.log(logL.DEB, F'Close communication channel: {self.media}')
-        self.__unlock()
         if self.__status == Status.CONNECTED:
             self.__status = Status.READY
 
-    async def force_disconnect(self):
-        """ force disconnect without timeout and disconnect request """
-        self.received_frames.clear()  # for next exchange need clear all received frames
-        await self.media.close()
-        self.log(logL.DEB, F'Close media: {self.media}')
-        if self.__lock.locked():
-            self.__unlock()
-        # self.__status = Status.READ
-
     async def disconnect_request(self, force=False):
         """ Sent to server DISC """
         # self.settings.maxPduSize = int(self.current_association.xDLMS_context_info.max_receive_pdu_size)
         if not force and self.settings.connected == ConnectionState.NONE:
             return
         if self.settings.interfaceType == InterfaceType.HDLC:
             self.settings.connected = ConnectionState.NONE
@@ -1727,15 +1690,15 @@
         if self.objects is None:
             ret = AuthenticationMechanismName()
             ret.mechanism_id_element.set(int(self.m_id))
             return ret.get_a_xdr()
         else:
             return self.current_association.authentication_mechanism_name.get_a_xdr()
 
-    def aarqRequest(self):
+    def aarqRequest(self, m_id: mechanism_id.MechanismIdElement):
         """ Generate AARQ request.  Because all_ meters can't read all_ data in one packet, the packet must be split first, by using SplitDataToPackets method.  AARQ request as
         byte array. @see GXDLMSClient#parseAareResponse """
         self.settings.connected = self.settings.connected & ~ConnectionState.DLMS
         info = bytes()
         self.settings.resetBlockIndex()
         self.settings.setStoCChallenge(None)
         # if self.auto_increase_invoke_ID:
@@ -1748,15 +1711,15 @@
             info += pack('2sBc', b'\x80\x02',
                          8 - len(self.protocol_version),
                          self.protocol_version.contents)
         #  Application context name tag. Where A1 - Tag, 09 - content name length, 06 - BerType.OBJECT_IDENTIFIER, 07 - info length
         info += b'\xa1\x09\x06\x07' + self.APP_CONTEXT_NAME.contents
         #  Add system title.
         ciphered = self.settings.cipher and self.settings.cipher.isCiphered()
-        if not self.settings.isServer and (ciphered or self.m_id == mechanism_id.HIGH_GMAC) or self.m_id == mechanism_id.HIGH_ECDSA:
+        if not self.settings.isServer and (ciphered or m_id == mechanism_id.HIGH_GMAC) or m_id == mechanism_id.HIGH_ECDSA:
             if len(self.settings.cipher.systemTitle) != 8:
                 raise ValueError("SystemTitle")
             #  Add calling-AP-title: BerType.CONTEXT | BerType.CONSTRUCTED | AARQapdu.CALLING_AP_TITLE + length + BerType.OCTET_STRING + length + systemTitle
             info += pack(F'cBcB{len(self.settings.cipher.systemTitle)}s',
                          b'\xa6',
                          2 + len(self.settings.cipher.systemTitle),
                          b'\x04',
@@ -1764,24 +1727,24 @@
                          self.settings.cipher.systemTitle)
         #  CallingAEInvocationId: BerType.CONTEXT | BerType.CONSTRUCTED | AARQapdu.CALLING_AE_INVOCATION_ID + length + BerType.INTEGER + length + userId
         if not self.settings.isServer and self.settings.userId != -1:
             info += pack(F'4sB',
                          b'\xa9\x03\x02\x01',
                          self.settings.userId)
         # Retrieves the string that indicates the level of authentication, if any.
-        if self.m_id != mechanism_id.NONE or (self.settings.cipher and self.settings.cipher.security != Security.NONE):
+        if m_id != mechanism_id.NONE or (self.settings.cipher and self.settings.cipher.security != Security.NONE):
             info += b'\x8a\x02\x07\x80'
             # Where: 8b - Tag(CONTEXT(0x80) + AARQ-apdu.MECHANISM_NAME(0x0b)), 07 - info length
             info += b'\x8b\x07' + self.mechanism_name
         #  Add Calling authentication information.
-        if self.m_id != mechanism_id.NONE:
-            if self.m_id == mechanism_id.LOW:
+        if m_id != mechanism_id.NONE:
+            if m_id == mechanism_id.LOW:
                 c_a_v = self.secret
                 """ calling-authentication-value """
-            elif self.m_id == mechanism_id.HIGH:
+            elif m_id == mechanism_id.HIGH:
                 self.settings.ctoSChallenge = os.urandom(16)
                 c_a_v = self.settings.ctoSChallenge
             else:
                 # TODO: must be 8..64 bytes length of urandom for different auth level
                 self.settings.ctoSChallenge = os.urandom(16)
                 c_a_v = self.settings.ctoSChallenge
             # BerType.CONTEXT | BerType.CONSTRUCTED | AARQ-apdu.CALLING_AUTHENTICATION_VALUE + length + context + info_len
```

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.6.7
+Version: 0.7.0
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.6.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.7.0/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.6.7/test/test_Client.py` & `DLMS_SPODES_client-0.7.0/test/test_Client.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,52 @@
 from DLMS_SPODES.types import cdt
 from src.DLMS_SPODES_client.client import Client, SerialPort, Network, AsyncNetwork, Collection, AppVersion, AsyncSerial
 from src.DLMS_SPODES_client.servers import TransactionServer
 from src.DLMS_SPODES_client import task
 
 
 class TestType(unittest.TestCase):
+    def test_connect(self):
+        t_server = TransactionServer(
+            clients=[
+                client := Client(addr_size=1)
+            ],
+            tsk=task.Dummy()
+        )
+        client.device_address.set(0)
+        client.media = AsyncSerial(
+            port="COM13",
+            inactivity_timeout=3
+        )
+        t_server.start()
+
+    def test_Loop(self):
+        def foo(res):
+            return res == cdt.Long(4)
+
+        t_server = TransactionServer(
+            clients=[
+                client := Client(addr_size=1)
+            ],
+            tsk=task.Loop(
+                task=task.ReadAttribute(
+                    ln="0.0.1.0.0.255",
+                    index=3),
+                func=lambda res: res == cdt.Long(4),
+                delay=2,
+                attempt_amount=5
+            )
+        )
+        client.device_address.set(0)
+        client.media = AsyncSerial(
+            port="COM13",
+            inactivity_timeout=3
+        )
+        t_server.start()
+
     def test_async_network(self):
         client = Client(
             secret="00 00 00 00 00 00 00 00",
             addr_size=1,
             conformance="010000000001111000011101")
         type_ = "4d324d5f31"
         ver = "1.5.7"
@@ -112,21 +150,21 @@
         print(t_server)
 
     def test_write(self):
         client = Client(
             secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 30",
             addr_size=1,
             conformance="010000000001111000011101")
-        type_ = "4d324d5f31"
-        ver = "1.5.7"
-        man = b"KPZ"
-        client.objects = collection.get(
-            m=man,
-            t=cdt.OctetString(type_),
-            ver=AppVersion.from_str(ver))
+        # type_ = "4d324d5f31"
+        # ver = "1.5.7"
+        # man = b"KPZ"
+        # client.objects = collection.get(
+        #     m=man,
+        #     t=cdt.OctetString(type_),
+        #     ver=AppVersion.from_str(ver))
         client.SAP.set(0x30)
         client.m_id.set(2)
         client.device_address.set(0)
         client.media = AsyncSerial(
             port="COM13",
             inactivity_timeout=3
         )
@@ -146,8 +184,31 @@
         # t_server.abort()
         # time.sleep(1)
         # t_server.abort()
         print(t_server.results.ok_results)
         while not t_server.results.is_complete():
             time.sleep(1)
         a = t_server.results[0]
-        print(t_server)
+        print(t_server)
+
+    def test_firmware_update(self):
+        client = Client(
+            secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 30",
+            addr_size=1,
+            conformance="010000000001111000011101")
+        client.SAP.set(0x30)
+        client.m_id.set(2)
+        client.device_address.set(0)
+        client.media = AsyncSerial(
+            port="COM13",
+            inactivity_timeout=3
+        )
+        t_server = TransactionServer(
+            clients=[client],
+            tsk=task.UpdateFirmware())
+        t_server.start()
+
+        while not t_server.results.is_complete():
+            time.sleep(1)
+            print(f"{t_server.results.is_complete()=}")
+        a = t_server.results[0]
+        print(t_server)
```

