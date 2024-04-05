# Comparing `tmp/mpflash-0.4.2.tar.gz` & `tmp/mpflash-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.4.2.tar", max compression
+gzip compressed data, was "mpflash-0.5.0.tar", max compression
```

## Comparing `mpflash-0.4.2.tar` & `mpflash-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.4.2/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.4.2/mpflash/__init__.py
--rw-r--r--   0        0        0     5248 2024-03-20 22:33:20.130001 mpflash-0.4.2/mpflash/ask_input.py
--rw-r--r--   0        0        0     2446 2024-03-20 21:36:30.723746 mpflash-0.4.2/mpflash/cli_download.py
--rw-r--r--   0        0        0     7237 2024-03-20 22:01:30.736652 mpflash-0.4.2/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1946 2024-03-20 21:46:16.907966 mpflash-0.4.2/mpflash/cli_group.py
--rw-r--r--   0        0        0     2832 2024-03-27 18:14:45.280335 mpflash-0.4.2/mpflash/cli_list.py
--rw-r--r--   0        0        0      529 2024-03-20 21:44:59.429778 mpflash-0.4.2/mpflash/cli_main.py
--rw-r--r--   0        0        0     5066 2024-03-26 21:17:44.038751 mpflash-0.4.2/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-03-19 23:55:54.108209 mpflash-0.4.2/mpflash/config.py
--rw-r--r--   0        0        0    10357 2024-03-20 21:15:24.579971 mpflash-0.4.2/mpflash/download.py
--rw-r--r--   0        0        0     5692 2024-03-20 21:18:04.789556 mpflash-0.4.2/mpflash/flash.py
--rw-r--r--   0        0        0     2396 2024-03-18 18:41:36.590406 mpflash-0.4.2/mpflash/flash_esp.py
--rw-r--r--   0        0        0      869 2024-03-15 14:55:22.828719 mpflash-0.4.2/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     4010 2024-03-12 22:57:35.914158 mpflash-0.4.2/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2509 2024-03-17 13:45:35.210978 mpflash-0.4.2/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2029 2024-03-15 15:46:23.966502 mpflash-0.4.2/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-03-05 22:17:23.940389 mpflash-0.4.2/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4298 2024-03-14 14:09:42.343080 mpflash-0.4.2/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1072 2024-03-14 14:09:42.343080 mpflash-0.4.2/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.4.2/mpflash/logger.py
--rw-r--r--   0        0        0     3143 2024-03-26 21:25:42.797035 mpflash-0.4.2/mpflash/mpboard_id/api.py
--rw-r--r--   0        0        0     1778 2024-03-12 12:49:58.741138 mpflash-0.4.2/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-03-17 23:08:19.329031 mpflash-0.4.2/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-03-17 23:08:19.327031 mpflash-0.4.2/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     4726 2024-03-13 16:28:38.858846 mpflash-0.4.2/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.4.2/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4583 2024-03-13 16:26:49.937127 mpflash-0.4.2/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-03-15 15:39:12.242892 mpflash-0.4.2/mpflash/vendored/dfu.py
--rw-r--r--   0        0        0    20542 2024-03-15 15:48:45.978919 mpflash-0.4.2/mpflash/vendored/pydfu.py
--rw-r--r--   0        0        0       86 2024-03-13 08:41:44.017018 mpflash-0.4.2/mpflash/vendored/readme.md
--rw-r--r--   0        0        0     1458 2024-03-30 22:24:21.862825 mpflash-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12272 2024-03-12 12:49:58.724383 mpflash-0.4.2/README.md
--rw-r--r--   0        0        0    13796 1970-01-01 00:00:00.000000 mpflash-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.5.0/mpflash/__init__.py
+-rw-r--r--   0        0        0     5248 2024-03-20 22:33:20.130001 mpflash-0.5.0/mpflash/ask_input.py
+-rw-r--r--   0        0        0     2446 2024-03-20 21:36:30.723746 mpflash-0.5.0/mpflash/cli_download.py
+-rw-r--r--   0        0        0     7341 2024-04-03 19:46:44.670186 mpflash-0.5.0/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1946 2024-03-20 21:46:16.907966 mpflash-0.5.0/mpflash/cli_group.py
+-rw-r--r--   0        0        0     2832 2024-03-27 18:14:45.280335 mpflash-0.5.0/mpflash/cli_list.py
+-rw-r--r--   0        0        0      529 2024-03-20 21:44:59.429778 mpflash-0.5.0/mpflash/cli_main.py
+-rw-r--r--   0        0        0     5066 2024-03-26 21:17:44.038751 mpflash-0.5.0/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-03-19 23:55:54.108209 mpflash-0.5.0/mpflash/config.py
+-rw-r--r--   0        0        0    10357 2024-03-20 21:15:24.579971 mpflash-0.5.0/mpflash/download.py
+-rw-r--r--   0        0        0     5692 2024-03-20 21:18:04.789556 mpflash-0.5.0/mpflash/flash.py
+-rw-r--r--   0        0        0     2396 2024-03-18 18:41:36.590406 mpflash-0.5.0/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      869 2024-03-15 14:55:22.828719 mpflash-0.5.0/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     4010 2024-03-12 22:57:35.914158 mpflash-0.5.0/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2509 2024-03-17 13:45:35.210978 mpflash-0.5.0/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2029 2024-03-15 15:46:23.966502 mpflash-0.5.0/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-03-05 22:17:23.940389 mpflash-0.5.0/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4298 2024-03-14 14:09:42.343080 mpflash-0.5.0/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1072 2024-03-14 14:09:42.343080 mpflash-0.5.0/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.5.0/mpflash/logger.py
+-rw-r--r--   0        0        0     3143 2024-03-26 21:25:42.797035 mpflash-0.5.0/mpflash/mpboard_id/api.py
+-rw-r--r--   0        0        0     1778 2024-03-12 12:49:58.741138 mpflash-0.5.0/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-03-17 23:08:19.329031 mpflash-0.5.0/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-03-17 23:08:19.327031 mpflash-0.5.0/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     4726 2024-03-13 16:28:38.858846 mpflash-0.5.0/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.5.0/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4583 2024-03-13 16:26:49.937127 mpflash-0.5.0/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-03-15 15:39:12.242892 mpflash-0.5.0/mpflash/vendored/dfu.py
+-rw-r--r--   0        0        0    20542 2024-03-15 15:48:45.978919 mpflash-0.5.0/mpflash/vendored/pydfu.py
+-rw-r--r--   0        0        0       86 2024-03-13 08:41:44.017018 mpflash-0.5.0/mpflash/vendored/readme.md
+-rw-r--r--   0        0        0     1628 2024-04-05 08:35:21.948203 mpflash-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12272 2024-03-12 12:49:58.724383 mpflash-0.5.0/README.md
+-rw-r--r--   0        0        0    13797 1970-01-01 00:00:00.000000 mpflash-0.5.0/PKG-INFO
```

### Comparing `mpflash-0.4.2/LICENSE` & `mpflash-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/ask_input.py` & `mpflash-0.5.0/mpflash/ask_input.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/cli_download.py` & `mpflash-0.5.0/mpflash/cli_download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/cli_flash.py` & `mpflash-0.5.0/mpflash/cli_flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
+from typing import List
 
 import rich_click as click
 from loguru import logger as log
 
-from mpflash.mpboard_id.api import find_mp_board
-
 from .ask_input import FlashParams, ask_missing_params
 from .cli_download import connected_ports_boards
 from .cli_group import cli
 from .cli_list import show_mcus
 from .common import clean_version
 from .config import config
 from .flash import WorkList, auto_update, enter_bootloader, find_firmware
 from .flash_esp import flash_esp
 from .flash_stm32 import flash_stm32
 from .flash_uf2 import flash_uf2
+from .mpboard_id.api import find_mp_board
 from .mpremoteboard import MPRemoteBoard
 
 # #########################################################################################################
 # CLI
 # #########################################################################################################
 
 
@@ -81,15 +81,15 @@
     help="The CPU type to flash. If not specified will try to read the CPU from the connected MCU.",
     metavar="CPU",
 )
 @click.option(
     "--erase/--no-erase",
     default=True,
     show_default=True,
-    help="""Erase flash before writing new firmware. (not on UF2 boards)""",
+    help="""Erase flash before writing new firmware. (Not supported on UF2 boards)""",
 )
 @click.option(
     "--bootloader/--no-bootloader",
     default=True,
     is_flag=True,
     show_default=True,
     help="""Enter micropython bootloader mode before flashing.""",
@@ -153,22 +153,22 @@
     version: str,
     fw_folder: Path,
     serial_port: str,
     # preview: bool,
 ) -> WorkList:
     """Create a worklist for a single serial-port."""
     conn_boards = [MPRemoteBoard(serial_port)]
-    todo = auto_update(conn_boards, version, fw_folder)
-    show_mcus(conn_boards)
+    todo = auto_update(conn_boards, version, fw_folder)  # type: ignore # List / list
+    show_mcus(conn_boards)  # type: ignore
     return todo
 
 
 def auto_worklist(version: str, fw_folder: Path) -> WorkList:
     conn_boards = [MPRemoteBoard(sp) for sp in MPRemoteBoard.connected_boards() if sp not in config.ignore_ports]
-    return auto_update(conn_boards, version, fw_folder)
+    return auto_update(conn_boards, version, fw_folder)  # type: ignore
 
 
 def manual_worklist(
     version: str,
     fw_folder: Path,
     serial_port: str,
     board: str,
@@ -182,15 +182,15 @@
     mcu.cpu = port if port.startswith("esp") else ""
     mcu.board = board
     firmwares = find_firmware(fw_folder=fw_folder, board=board, version=version, port=port)
     if not firmwares:
         log.error(f"No firmware found for {port} {board} version {version}")
         return []
         # use the most recent matching firmware
-    return [(mcu, firmwares[-1])]
+    return [(mcu, firmwares[-1])]  # type: ignore
 
 
 def flash_list(
     todo: WorkList,
     fw_folder: Path,
     erase: bool,
     bootloader: bool,
```

### Comparing `mpflash-0.4.2/mpflash/cli_group.py` & `mpflash-0.5.0/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/cli_list.py` & `mpflash-0.5.0/mpflash/cli_list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/cli_main.py` & `mpflash-0.5.0/mpflash/cli_main.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/common.py` & `mpflash-0.5.0/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/download.py` & `mpflash-0.5.0/mpflash/download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash.py` & `mpflash-0.5.0/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_esp.py` & `mpflash-0.5.0/mpflash/flash_esp.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_stm32.py` & `mpflash-0.5.0/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_stm32_cube.py` & `mpflash-0.5.0/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_stm32_dfu.py` & `mpflash-0.5.0/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_uf2.py` & `mpflash-0.5.0/mpflash/flash_uf2.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_uf2_linux.py` & `mpflash-0.5.0/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/flash_uf2_windows.py` & `mpflash-0.5.0/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/logger.py` & `mpflash-0.5.0/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpboard_id/api.py` & `mpflash-0.5.0/mpflash/mpboard_id/api.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpboard_id/board_id.py` & `mpflash-0.5.0/mpflash/mpboard_id/board_id.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpboard_id/board_info.csv` & `mpflash-0.5.0/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpboard_id/board_info.json` & `mpflash-0.5.0/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpremoteboard/__init__.py` & `mpflash-0.5.0/mpflash/mpremoteboard/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.5.0/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/mpremoteboard/runner.py` & `mpflash-0.5.0/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/vendored/dfu.py` & `mpflash-0.5.0/mpflash/vendored/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/mpflash/vendored/pydfu.py` & `mpflash-0.5.0/mpflash/vendored/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/pyproject.toml` & `mpflash-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.4.2"
+version = "0.5.0"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
@@ -14,15 +14,15 @@
     "Topic :: Software Development :: Build Tools",
 ]
 
 [tool.poetry.scripts]
 mpflash = "mpflash.cli_main:mpflash"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python =  ">=3.8.1,<4.0"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
 loguru = "^0.7.2"
 esptool = "^4.7.0"
 jsonlines = "^4.0.0"
 bincopy = "^20.0.0"
 strip-ansi = "^0.1.1"
@@ -34,18 +34,24 @@
 pyusb = "^1.2.1"
 packaging = "23.2"
 tenacity = "8.2.3"
 mpremote = "^1.22.0"
 inquirer = "^3.2.4"
 libusb = {version = "^1.0.27", platform = "win32"}
 
-[tool.poetry.group.dev.dependencies]
-types-beautifulsoup4 = "^4.12.0.20240106"
-pytest = "^8.1.1"
-pytest-mock = "^3.14.0"
-mock = "^5.1.0"
+[tool.poetry.group.test]
+optional = true
+[tool.poetry.group.test.dependencies]
 coverage = ">=6.4.3,<8.0.0"
+pytest = "^7.1.2"
+pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
+pytest-json-report = "^1.5.0"
+pytest-metadata = ">=2.0.2,<4.0.0"
+pytest-mock = "^3.10.0"
+mock = "^4.0.3"
+distro = "^1.8.0"
+fasteners = "^0.19"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpflash-0.4.2/README.md` & `mpflash-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mpflash-0.4.2/PKG-INFO` & `mpflash-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.4.2
+Version: 0.5.0
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

