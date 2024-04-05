# Comparing `tmp/linien-common-1.0.2rc1.tar.gz` & `tmp/linien-common-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:32 2024, max compression
+gzip compressed data, was "linien-common-2.0.0rc1.tar", last modified: Fri Apr  5 13:10:23 2024, max compression
```

## Comparing `linien-common-1.0.2rc1.tar` & `linien-common-2.0.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:10:23.000000 linien-common-2.0.0rc1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-05 13:10:16.000000 linien-common-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:10:23.052651 linien-common-2.0.0rc1/setup.cfg
```

### Comparing `linien-common-1.0.2rc1/linien_common/__init__.py` & `linien-common-2.0.0rc1/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.2rc1/linien_common/common.py` & `linien-common-2.0.0rc1/linien_common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 
 """This file contains stuff that is required by the server as well as the client."""
 
-from enum import Enum, IntEnum
+from enum import IntEnum
 from time import time
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from scipy.signal import correlate, resample
 
 MHz = 0x10000000 / 8
@@ -50,17 +50,17 @@
 
 class AutolockMode(IntEnum):
     AUTO_DETECT = 0
     ROBUST = 1
     SIMPLE = 2
 
 
-class PSDAlgorithm(str, Enum):
-    WELCH = "welch"
-    LPSD = "lpsd"
+class PSDAlgorithm(IntEnum):
+    WELCH = 0
+    LPSD = 1
 
 
 class SpectrumUncorrelatedException(Exception):
     pass
 
 
 def downsample_history(
@@ -289,15 +289,15 @@
             (a_factor * a + b_factor * b) >> chain_factor_width
             for a, b in zip(*error_signals)
         ]
 
     return np.array([v + combined_offset for v in signal])
 
 
-def check_plot_data(is_locked: bool, plot_data) -> bool:
+def check_plot_data(is_locked: bool, plot_data: Dict[str, np.ndarray]) -> bool:
     if is_locked:
         if "error_signal" not in plot_data or "control_signal" not in plot_data:
             return False
     else:
         if "error_signal_1" not in plot_data:
             return False
     return True
```

### Comparing `linien-common-1.0.2rc1/linien_common/config.py` & `linien-common-2.0.0rc1/linien_common/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from appdirs import AppDirs
 
 ACQUISITION_PORT = 19321
-DEFAULT_SERVER_PORT = 18862
+SERVER_PORT = 18862
 DEFAULT_SWEEP_SPEED = (125 * 2048) << 6
 
 USER_DATA_PATH = Path(AppDirs("linien").user_data_dir)
 USER_DATA_PATH.mkdir(parents=True, exist_ok=True)
 
 LOG_FILE_PATH = USER_DATA_PATH / "linien.log"
 LOG_FILE_PATH.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `linien-common-1.0.2rc1/linien_common/influxdb.py` & `linien-common-2.0.0rc1/linien_common/influxdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,46 +13,31 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
+from dataclasses import dataclass
 
 from .config import USER_DATA_PATH
 
 CREDENTIAL_STORE_FILENAME = "influxdb_credentials.json"
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
+@dataclass
 class InfluxDBCredentials:
-    def __init__(
-        self,
-        url: str = "http://localhost:8086",
-        org: str = "my-org",
-        token: str = "my-token",
-        bucket: str = "my-bucket",
-        measurement: str = "my-measurement",
-    ) -> None:
-        self.url = url
-        self.org = org
-        self.token = token
-        self.bucket = bucket
-        self.measurement = measurement
-
-    def __str__(self) -> str:
-        return "url: %s, org: %s, token: %s, bucket: %s, measurement: %s" % (
-            self.url,
-            self.org,
-            self.token,
-            self.bucket,
-            self.measurement,
-        )
+    url: str = "http://localhost:8086"
+    org: str = "my-org"
+    token: str = "my-token"
+    bucket: str = "my-bucket"
+    measurement: str = "my-measurement"
 
 
 def save_credentials(credentials: InfluxDBCredentials) -> None:
     """Save the credentials to disk."""
     filename = str(USER_DATA_PATH / CREDENTIAL_STORE_FILENAME)
     with open(filename, "w") as f:
         json.dump(
@@ -62,15 +47,15 @@
                 "token": credentials.token,
                 "bucket": credentials.bucket,
                 "measurement": credentials.measurement,
             },
             f,
             indent=2,
         )
-    logger.info("Saved InfluxDB credentials to %s" % filename)
+    logger.info(f"Saved InfluxDB credentials to {filename}")
 
 
 def restore_credentials() -> InfluxDBCredentials:
     """When the server starts, it tries to restore the credentials."""
     filename = USER_DATA_PATH / CREDENTIAL_STORE_FILENAME
     try:
         with open(str(filename), "r") as f:
```

