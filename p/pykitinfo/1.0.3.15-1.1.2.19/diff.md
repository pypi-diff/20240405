# Comparing `tmp/pykitinfo-1.0.3.15-py3-none-any.whl.zip` & `tmp/pykitinfo-1.1.2.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 19883 bytes, number of entries: 17
--rw-r--r--  2.0 unx     1840 b- defN 24-Jan-23 08:01 pykitinfo/__init__.py
--rw-r--r--  2.0 unx     7061 b- defN 24-Jan-23 08:00 pykitinfo/detect_edbg_tools.py
--rw-r--r--  2.0 unx     1866 b- defN 24-Jan-23 08:00 pykitinfo/detect_legacy_pickit3_tools.py
--rw-r--r--  2.0 unx     6583 b- defN 24-Jan-23 08:00 pykitinfo/detect_microchip_tools.py
--rw-r--r--  2.0 unx     1752 b- defN 24-Jan-23 08:00 pykitinfo/logging.yaml
--rw-r--r--  2.0 unx     2155 b- defN 24-Jan-23 08:00 pykitinfo/pykitinfo.py
--rw-r--r--  2.0 unx     5608 b- defN 24-Jan-23 08:00 pykitinfo/pykitinfo_cli.py
--rw-r--r--  2.0 unx     5221 b- defN 24-Jan-23 08:00 pykitinfo/tools.py
--rw-r--r--  2.0 unx      977 b- defN 24-Jan-23 08:00 pykitinfo/winkernel32.py
--rw-r--r--  2.0 unx     5915 b- defN 24-Jan-23 08:00 pykitinfo/winsetupapi.py
--rw-r--r--  2.0 unx     6638 b- defN 24-Jan-23 08:00 pykitinfo/winusb.py
--rw-r--r--  2.0 unx     1107 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6293 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1422 b- defN 24-Jan-23 08:01 pykitinfo-1.0.3.15.dist-info/RECORD
-17 files, 54599 bytes uncompressed, 17541 bytes compressed:  67.9%
+Zip file size: 21285 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1855 b- defN 24-Mar-22 09:44 pykitinfo/__init__.py
+-rw-r--r--  2.0 unx     7061 b- defN 24-Mar-22 09:43 pykitinfo/detect_edbg_tools.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Mar-22 09:43 pykitinfo/detect_legacy_pickit3_tools.py
+-rw-r--r--  2.0 unx     3123 b- defN 24-Mar-22 09:43 pykitinfo/detect_mcp2221a_tools.py
+-rw-r--r--  2.0 unx     6583 b- defN 24-Mar-22 09:43 pykitinfo/detect_microchip_tools.py
+-rw-r--r--  2.0 unx     1752 b- defN 24-Mar-22 09:43 pykitinfo/logging.yaml
+-rw-r--r--  2.0 unx     2263 b- defN 24-Mar-22 09:43 pykitinfo/pykitinfo.py
+-rw-r--r--  2.0 unx     5608 b- defN 24-Mar-22 09:43 pykitinfo/pykitinfo_cli.py
+-rw-r--r--  2.0 unx     5221 b- defN 24-Mar-22 09:43 pykitinfo/tools.py
+-rw-r--r--  2.0 unx      977 b- defN 24-Mar-22 09:43 pykitinfo/winkernel32.py
+-rw-r--r--  2.0 unx     5915 b- defN 24-Mar-22 09:43 pykitinfo/winsetupapi.py
+-rw-r--r--  2.0 unx     6638 b- defN 24-Mar-22 09:43 pykitinfo/winusb.py
+-rw-r--r--  2.0 unx     1107 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6566 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1513 b- defN 24-Mar-22 09:44 pykitinfo-1.1.2.19.dist-info/RECORD
+18 files, 58243 bytes uncompressed, 18799 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: pykitinfo/detect_edbg_tools.py
 Comment: 
 
 Filename: pykitinfo/detect_legacy_pickit3_tools.py
 Comment: 
 
+Filename: pykitinfo/detect_mcp2221a_tools.py
+Comment: 
+
 Filename: pykitinfo/detect_microchip_tools.py
 Comment: 
 
 Filename: pykitinfo/logging.yaml
 Comment: 
 
 Filename: pykitinfo/pykitinfo.py
@@ -27,26 +30,26 @@
 
 Filename: pykitinfo/winsetupapi.py
 Comment: 
 
 Filename: pykitinfo/winusb.py
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/LICENSE.txt
+Filename: pykitinfo-1.1.2.19.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/METADATA
+Filename: pykitinfo-1.1.2.19.dist-info/METADATA
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/WHEEL
+Filename: pykitinfo-1.1.2.19.dist-info/WHEEL
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/entry_points.txt
+Filename: pykitinfo-1.1.2.19.dist-info/entry_points.txt
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/top_level.txt
+Filename: pykitinfo-1.1.2.19.dist-info/top_level.txt
 Comment: 
 
-Filename: pykitinfo-1.0.3.15.dist-info/RECORD
+Filename: pykitinfo-1.1.2.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pykitinfo/__init__.py

```diff
@@ -13,14 +13,15 @@
     * read the changelog on pypi:  https://pypi.org/project/pykitinfo
 
 pykitinfo currently supports:
     * all PKOB nano (nEDBG), mEDBG and EDBG kits
     * Atmel-ICE, Power Debugger, JTAGICE3
     * PICkit3, PKOB
     * PICkit4, Snap, PKOB4, PICkit5
+    * MCP2221A
 
 CLI usage example
 ~~~~~~~~~~~~~~~~~
 See examples on pypi: https://pypi.org/project/pykitinfo
 
 Library usage example
 ~~~~~~~~~~~~~~~~~~~~~
@@ -40,14 +41,14 @@
         print("Found kit: '{}'".format(kit['debugger']['kitname']))
 
 """
 import logging
 
 # Build number part of version will be replaced by build number from Jenkins.
 # For local builds the build number is 0 and the 'snapshot' is added as Local Version Identifier
-__version__ = "1.0.3.15"
+__version__ = "1.1.2.19"
 
 # The GIT commit ID and build date are generated by Jenkins when building the package
-COMMIT_ID = '71880defe9ffe393e7e97f160b11154268ece1df'
-BUILD_DATE = '2024-01-23 08:01:30'
+COMMIT_ID = '5d9404b535b655a65ff0f863591e9c76f5cf5cf7'
+BUILD_DATE = '2024-03-22 09:44:32'
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

## pykitinfo/detect_legacy_pickit3_tools.py

```diff
@@ -14,15 +14,15 @@
     :param serialnumber: (partial) serial number to use
     :type serialnumber: str
     :return: kits and tools connected
     :rtype: list of dictionaries
     """
     logger = getLogger(__name__)
     logger.debug("Looking for PKoB/PICkit 3 kits")
-    PICKIT3_PRODUCT_NAMES = ["PICkit 3", "Curiosity"]
+    PICKIT3_PRODUCT_NAMES = ["PICkit 3", "Curiosity", "Explorer 16/32 PICkit on Board"]
     pickit_list = []
     devices = hid.enumerate(MICROCHIP_VID)
     for candidate in devices:
         candidate_serial = candidate['serial_number']
         # Filter out by serial number if specified
         if serialnumber and candidate_serial and not candidate_serial.endswith(serialnumber):
             continue
```

## pykitinfo/pykitinfo.py

```diff
@@ -2,14 +2,15 @@
 Python Kit Info
 """
 from logging import getLogger
 import json
 from .detect_microchip_tools import detect_microchip_tools
 from .detect_edbg_tools import detect_edbg_kits
 from .detect_legacy_pickit3_tools import detect_pickit3s
+from .detect_mcp2221a_tools import detect_mcp2221a_kits
 
 STATUS_SUCCESS = 0
 STATUS_FAILURE = 1
 
 from . import __version__ as VERSION
 from . import BUILD_DATE, COMMIT_ID
 
@@ -58,8 +59,10 @@
     :return: kits and tools connected
     :rtype: list of dictionaries
     """
     kit_list = []
     kit_list += detect_edbg_kits(serialnumber)
     kit_list += detect_pickit3s(serialnumber)
     kit_list += detect_microchip_tools(serialnumber)
+    kit_list += detect_mcp2221a_kits(serialnumber)
+
     return kit_list
```

## Comparing `pykitinfo-1.0.3.15.dist-info/LICENSE.txt` & `pykitinfo-1.1.2.19.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pykitinfo-1.0.3.15.dist-info/METADATA` & `pykitinfo-1.1.2.19.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pykitinfo
-Version: 1.0.3.15
+Version: 1.1.2.19
 Summary: A provider of information about connected Microchip development kits
 Author-email: Microchip Technology <support@microchip.com>
 License: MIT
 Project-URL: Homepage, https://github.com/microchip-pic-avr-tools/pykitinfo
-Keywords: Microchip,Xplained Pro,EDBG,nEDBG,Curiosity Nano,PKOB nano,debugger
+Keywords: Microchip,Xplained Pro,EDBG,nEDBG,Curiosity Nano,PKOB nano,debugger,MCP2221A
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -49,14 +49,15 @@
 * read API documentation on github: https://microchip-pic-avr-tools.github.io/pykitinfo
 
 pykitinfo currently supports:
 * all PKOB nano (nEDBG), mEDBG and EDBG kits
 * Atmel-ICE, Power Debugger, JTAGICE3
 * PICkit3, PKOB
 * PICkit4, Snap, PKOB4, PICkit5
+* MCP2221A
 
 ## Usage
 pykitinfo can be used as a library or as a CLI
 
 ## Example - simple list of connected kits
 ```bash
 pykitinfo
@@ -64,21 +65,23 @@
 Displays a simple list of kits in the form:
 Kit SERIAL-NUMBER: 'KIT-NAME' (DEVICE-NAME) on SERIAL-PORT
 
 For example:
 ```bash
 pykitinfo
 Looking for Microchip kits...
-Compatible kits detected: 6
+Compatible kits detected: 8
 Kit MCHP3349011800000000: 'AVR-IoT WA' (ATmega4808) on COM21
 Kit MCHP3280021800000000: 'AVR128DA48 Curiosity Nano' (AVR128DA48) on COM17
 Kit ATML2241020200000000: 'SAM L21 Xplained Pro' (ATSAML21J18A) on COM34
 Kit J41800000000: 'Atmel-ICE CMSIS-DAP' () on N/A
 Kit J50200000000: 'Power Debugger CMSIS-DAP' () on N/A
 Kit ATML2323040200000000: 'mEDBG' (ATmega328P) on COM26
+Kit BUR180115004: 'Explorer 16/32 PICkit on Board' () on N/A
+Kit 020063002RYN000091: 'Curiosity Nano Explorer' (N/A) on COM74
 ```
 
 ## Example - simple list of connected kits with specific serial number
 ```bash
 pykitinfo -s <serialnumber ending>
 ```
 Displays a simple list of kits in the form:
@@ -167,14 +170,20 @@
     print("Found kit: '{}'".format(kit['debugger']['kitname']))
 ```
 
 ## Notes for Linux® systems
 This package uses pyedbglib and other libraries for USB transport and some udev rules are required. For details see the pyedbglib package: https://pypi.org/project/pyedbglib
 # Changelog
 
+## [1.1.2] - April 2024
+
+### Added
+- DSG-7105 added support for Explorer 16/32 kit
+- DSG-7181 added support for MCP2221A kits
+
 ## [1.0.3] - January 2024
 
 ### Added
 - DSG-5792 added brief mode for reporting serial port only
 - DSG-6091 added support for reading out nEDBG extension information
 - DSG-6444 added support for PICkit 5
```

## Comparing `pykitinfo-1.0.3.15.dist-info/RECORD` & `pykitinfo-1.1.2.19.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-pykitinfo/__init__.py,sha256=a5H6jrhChyiltDEnxOhwgsJYoo3-T1-OnixowQNP5ps,1840
+pykitinfo/__init__.py,sha256=ZGe6gZsmnKS0HTgHJY426HBWTr2g3vdttRsWWDGkH1I,1855
 pykitinfo/detect_edbg_tools.py,sha256=EFha0hOdQwPDboC0nmvcNrndJWmBNvRyXHb1aZdandU,7061
-pykitinfo/detect_legacy_pickit3_tools.py,sha256=JnlUDHVd7bUbDV_J20xkX1uHm8eWvpy74D_zaw52p90,1866
+pykitinfo/detect_legacy_pickit3_tools.py,sha256=k-hJcdhhg2v6fgD0aNzY5yrQ1HB5e5GI2H1Nry05Wio,1900
+pykitinfo/detect_mcp2221a_tools.py,sha256=GRUbXXZIICRqZwl1ojJUpws-51oUbs9e3R54xL3zgis,3123
 pykitinfo/detect_microchip_tools.py,sha256=WEqc8P4zPVJcNFHalAVF7lDoVn0Z7Dd0acf73eUlMGE,6583
 pykitinfo/logging.yaml,sha256=6aQ6G-yvpRWyPRKE8DEyDzrJxjs89LciUzEkRAasDIs,1752
-pykitinfo/pykitinfo.py,sha256=xgFwM8xEbqOnDlK8_iqLoXlFT_eWh_ePprg2frYZR7Q,2155
+pykitinfo/pykitinfo.py,sha256=5z331k0gaOcFSJHJ98NjV3J2W-RD-eAAkdDWfrM-4Yk,2263
 pykitinfo/pykitinfo_cli.py,sha256=srTZpil_UvugWY8uhxdUlfdQTMUb5vQTwzgv9x-DR0o,5608
 pykitinfo/tools.py,sha256=RM2c-AmNZEGHMo-d6Nhkwr09KdE9N6e1ocHJqxxA0TM,5221
 pykitinfo/winkernel32.py,sha256=qxib_5I050QGG_7avZiis8Z_H7qew-j5n9xal6fjXME,977
 pykitinfo/winsetupapi.py,sha256=lDZTTuJD3R4CzOiziLCQcp73_Cw5owYiLkeqz9TfaRA,5915
 pykitinfo/winusb.py,sha256=KwhKW17iFEvbTX57PVQOM1UPk1m55G56RTRcmfRCINU,6638
-pykitinfo-1.0.3.15.dist-info/LICENSE.txt,sha256=QQ6tPdTIUYxb_NYYGTDSbKPoYpZLCkNoqMqOk7kFxRg,1107
-pykitinfo-1.0.3.15.dist-info/METADATA,sha256=x3nHWXRZNB3HZxSjAXT5a0ccOPYYNF_tVwO4iJkGRR4,6293
-pykitinfo-1.0.3.15.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pykitinfo-1.0.3.15.dist-info/entry_points.txt,sha256=tIN5ybLg6uIOIg_vNTsP3FJWAroW1jc8kuyYr0Qu9Ic,59
-pykitinfo-1.0.3.15.dist-info/top_level.txt,sha256=4-6dCuZRmPHDSrogAyAxw_OCQOMtGfQwvrFj25I2Jbc,10
-pykitinfo-1.0.3.15.dist-info/RECORD,,
+pykitinfo-1.1.2.19.dist-info/LICENSE.txt,sha256=QQ6tPdTIUYxb_NYYGTDSbKPoYpZLCkNoqMqOk7kFxRg,1107
+pykitinfo-1.1.2.19.dist-info/METADATA,sha256=GwAP5dOP5a5rjqH8A_U3UMFoLmFmeAAXUZMitTf6lQ0,6566
+pykitinfo-1.1.2.19.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pykitinfo-1.1.2.19.dist-info/entry_points.txt,sha256=tIN5ybLg6uIOIg_vNTsP3FJWAroW1jc8kuyYr0Qu9Ic,59
+pykitinfo-1.1.2.19.dist-info/top_level.txt,sha256=4-6dCuZRmPHDSrogAyAxw_OCQOMtGfQwvrFj25I2Jbc,10
+pykitinfo-1.1.2.19.dist-info/RECORD,,
```

