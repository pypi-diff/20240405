# Comparing `tmp/linien-server-1.0.2rc1.tar.gz` & `tmp/linien-server-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:36 2024, max compression
+gzip compressed data, was "linien-server-2.0.0rc1.tar", last modified: Fri Apr  5 13:10:27 2024, max compression
```

## Comparing `linien-server-1.0.2rc1.tar` & `linien-server-2.0.0rc1.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.631796 linien-server-1.0.2rc1/linien_server/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.631796 linien-server-1.0.2rc1/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (127)  2083740 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/gateware.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_install_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_start_server.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_stop_server.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/noise_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/approach_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:27.904646 linien-server-2.0.0rc1/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/mdio_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/noise_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29168 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15684 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 13:10:27.000000 linien-server-2.0.0rc1/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 13:10:16.000000 linien-server-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:10:27.908646 linien-server-2.0.0rc1/setup.cfg
```

### Comparing `linien-server-1.0.2rc1/linien_server/__init__.py` & `linien-server-2.0.0rc1/linien_server/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2rc1/linien_server/acquisition.py` & `linien-server-2.0.0rc1/linien_server/acquisition.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import pickle
-import shutil
 import subprocess
 from pathlib import Path
 from random import random
 from threading import Event, Thread
 from time import sleep
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Optional
 
 import numpy as np
 from linien_common.common import DECIMATION, MAX_N_POINTS, N_POINTS
 from linien_common.config import ACQUISITION_PORT
 from linien_server.csr import PythonCSR
 from pyrp3.board import RedPitaya  # type: ignore
 from pyrp3.instrument import TriggerSource  # type: ignore
@@ -36,28 +35,28 @@
 from rpyc.utils.server import ThreadedServer
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class AcquisitionService(Service):
-    def __init__(self):
+    def __init__(self) -> None:
         super(AcquisitionService, self).__init__()
         stop_nginx()
         flash_fpga()
 
         self.red_pitaya = RedPitaya()
         self.csr = PythonCSR(self.red_pitaya)
-        self.csr_queue = []
-        self.csr_iir_queue = []
+        self.csr_queue: list[tuple[str, int]] = []
+        self.csr_iir_queue: list[tuple[str, list[float], list[float]]] = []
 
-        self.data = pickle.dumps(None)
+        self.data: bytes | None = pickle.dumps(None)
         self.data_was_raw = False
-        self.data_hash = None
-        self.data_uuid = None
+        self.data_hash: float | None = None
+        self.data_uuid: float | None = None
 
         self.locked = False
         self.exposed_set_sweep_speed(9)
         # when self.locked is set to True, this doesn't mean that the lock is really on.
         # It just means that the lock is requested and that the gateware waits until the
         # sweep is at the correct position for the lock. Therefore, when self.locked is
         # set, the acquisition process waits for confirmation from the gateware that the
@@ -90,20 +89,20 @@
     ) -> None:
         while not stop_event.is_set():
             while self.csr_queue:
                 key, value = self.csr_queue.pop(0)
                 self.csr.set(key, value)
 
             while self.csr_iir_queue:
-                args = self.csr_iir_queue.pop(0)
-                self.csr.set_iir(*args)
+                name, b, a = self.csr_iir_queue.pop(0)
+                self.csr.set_iir(name, b, a)
 
             if self.locked and not self.confirmed_that_in_lock:
-                self.confirmed_that_in_lock = self.csr.get(
-                    "logic_autolock_lock_running"
+                self.confirmed_that_in_lock = bool(
+                    self.csr.get("logic_autolock_lock_running")
                 )
                 if not self.confirmed_that_in_lock:
                     sleep(0.05)
                     continue
 
             if pause_event.is_set():
                 sleep(0.05)
@@ -138,15 +137,15 @@
                 else:
                     self.data = pickle.dumps(data)
                 self.data_was_raw = is_raw
                 self.data_hash = random()
 
             self.program_acquisition_and_rearm()
 
-    def read_data(self) -> Dict[str, np.ndarray]:
+    def read_data(self) -> dict[str, np.ndarray]:
         signals = []
 
         channel_offsets = [0x10000]
         if self.fetch_additional_signals or self.locked:
             channel_offsets.append(0x20000)
 
         for channel_offset in channel_offsets:
@@ -185,15 +184,15 @@
         slow_out = slow_out if slow_out <= 8191 else slow_out - 16384
         signals_named["slow_control_signal"] = slow_out
 
         return signals_named
 
     def read_data_raw(
         self, offset: int, addr: int, data_length: int
-    ) -> Tuple[Any, ...]:
+    ) -> tuple[Any, ...]:
         max_data_length = 16383
         if data_length + addr > max_data_length:
             to_read_later = data_length + addr - max_data_length
             data_length -= to_read_later
         else:
             to_read_later = 0
 
@@ -236,22 +235,20 @@
 
         else:
             self.red_pitaya.scope.data_decimation = 1
             self.red_pitaya.scope.trigger_delay = int(trigger_delay / DECIMATION) - 1
 
         self.red_pitaya.scope.rearm(trigger_source=TriggerSource.ext_posedge)
 
-    def exposed_return_data(
-        self, last_hash: Optional[float]
-    ) -> Tuple[
+    def exposed_return_data(self, last_hash: Optional[float]) -> tuple[
         bool,
-        Union[float, None],
-        Union[bool, None],
-        Union[bytes, None],
-        Union[float, None],
+        float | None,
+        bool | None,
+        bytes | None,
+        float | None,
     ]:
         no_data_available = self.data_hash is None
         data_not_changed = self.data_hash == last_hash
         if data_not_changed or no_data_available or self.pause_event.is_set():
             return False, None, None, None, None
         else:
             return True, self.data_hash, self.data_was_raw, self.data, self.data_uuid
@@ -275,16 +272,16 @@
 
     def exposed_set_dual_channel(self, dual_channel):
         self.dual_channel = dual_channel
 
     def exposed_set_csr(self, key: str, value: int) -> None:
         self.csr_queue.append((key, value))
 
-    def exposed_set_iir_csr(self, *args):
-        self.csr_iir_queue.append(args)
+    def exposed_set_iir_csr(self, name: str, b: list[float], a: list[float]) -> None:
+        self.csr_iir_queue.append((name, b, a))
 
     def exposed_stop_acquisition(self) -> None:
         self.stop_event.set()
         self.thread.join()
         start_nginx()
 
     def exposed_pause_acquisition(self):
@@ -307,34 +304,24 @@
             self.skip_next_data_event.clear()
         else:
             self.skip_next_data_event.set()
 
 
 def flash_fpga():
     filepath = Path(__file__).resolve().parent / "gateware.bin"
-
-    # On redpitaya os < 2, flashing fpga works by copying the bit file /dev/xdevcfg. On
-    # recent versions, there is a dedicated command for this
-    # cf. https://forum.redpitaya.com/viewtopic.php?p=33494&sid=5132bf6e33709b1a7daa948f8e8dcdb1#p33494  # noqa: E501
-    fpga_dev_file = Path("/dev/xdevcfg")
-
-    if fpga_dev_file.exists():
-        logger.info("Copying gateware to %s" % fpga_dev_file)
-        shutil.copy(str(filepath), str(fpga_dev_file))
-    else:
-        logger.info("Using fpgautil to deploy gateware.")
-        subprocess.Popen(["/opt/redpitaya/bin/fpgautil", "-b", str(filepath)]).wait()
+    logger.info("Using fpgautil to deploy gateware.")
+    subprocess.Popen(["/opt/redpitaya/bin/fpgautil", "-b", str(filepath)]).wait()
 
 
 def start_nginx():
     subprocess.Popen(["systemctl", "start", "redpitaya_nginx.service"])
 
 
 def stop_nginx():
     subprocess.Popen(["systemctl", "stop", "redpitaya_nginx.service"]).wait()
     subprocess.Popen(["systemctl", "stop", "redpitaya_scpi.service"]).wait()
 
 
 if __name__ == "__main__":
     threaded_server = ThreadedServer(AcquisitionService(), port=ACQUISITION_PORT)
-    logger.info("Starting AcquisitionService on port %s" % ACQUISITION_PORT)
+    logger.info(f"Starting AcquisitionService on port {ACQUISITION_PORT}")
     threaded_server.start()
```

### Comparing `linien-server-1.0.2rc1/linien_server/autolock/algorithm_selection.py` & `linien-server-2.0.0rc1/linien_server/autolock/algorithm_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             additional = self.spectra[1:]
             abs_shifts = [
                 abs(determine_shift_by_correlation(1, ref, spectrum)[0] * N_POINTS)
                 for spectrum in additional
             ]
             max_shift = max(abs_shifts)
             logger.debug(
-                "jitter / line width ratio: %s" % (max_shift / (self.line_width / 2))
+                f"jitter / line width ratio: {max_shift / (self.line_width / 2)}"
             )
 
             if max_shift <= self.line_width / 2:
                 self.mode = AutolockMode.SIMPLE
             else:
                 self.mode = AutolockMode.ROBUST
```

### Comparing `linien-server-1.0.2rc1/linien_server/autolock/autolock.py` & `linien-server-2.0.0rc1/linien_server/autolock/autolock.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,31 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import pickle
 
-from linien_common.common import check_plot_data, combine_error_signal, get_lock_point
+from linien_common.common import (
+    SpectrumUncorrelatedException,
+    check_plot_data,
+    combine_error_signal,
+    get_lock_point,
+)
 from linien_server.autolock.algorithm_selection import AutolockAlgorithmSelector
 from linien_server.autolock.robust import RobustAutolock
 from linien_server.autolock.simple import SimpleAutolock
+from linien_server.parameters import Parameters
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class Autolock:
-    def __init__(self, control, parameters):
+    def __init__(self, control, parameters: Parameters) -> None:
         self.control = control
         self.parameters = parameters
 
         self.first_error_signal = None
         self.first_error_signal_rolled = None
         self.parameters.autolock_running.value = False
         self.parameters.autolock_retrying.value = False
@@ -56,18 +62,18 @@
             self.parameters.autolock_watching.value = False
 
     def run(
         self,
         x0,
         x1,
         spectrum,
-        should_watch_lock=False,
-        auto_offset=True,
+        should_watch_lock: bool = False,
+        auto_offset: bool = True,
         additional_spectra=None,
-    ):
+    ) -> None:
         """
         Start the autolock.
 
         If `should_watch_lock` is specified, the autolock continuously monitors the
         control and error signals after the lock was successful and tries to relock
         automatically using the spectrum that was recorded in the first run of the lock.
         """
@@ -99,26 +105,26 @@
                 additional_spectra,
                 self.line_width,
             )
 
             if self.autolock_mode_detector.done:
                 self.start_autolock(self.autolock_mode_detector.mode)
 
-        except Exception:
+        except SpectrumUncorrelatedException:
             # This may happen if `additional_spectra` contain uncorrelated data. Then
             # either autolock algorithm selector or `start_autolock` may raise a
             # spectrum uncorrelated exception
             logger.exception("Error while starting autolock")
             self.parameters.autolock_failed.value = True
-            return self.exposed_stop()
+            self.exposed_stop()
 
         self.add_data_listener()
 
     def start_autolock(self, mode):
-        logger.debug("start autolock with mode %s" % mode)
+        logger.debug(f"Start autolock with mode {mode}")
         self.parameters.autolock_mode.value = mode
 
         self.algorithm = [None, RobustAutolock, SimpleAutolock][mode](
             self.control,
             self.parameters,
             self.first_error_signal,
             self.first_error_signal_rolled,
@@ -126,23 +132,21 @@
             self.peak_idxs[1],
             additional_spectra=self.additional_spectra,
         )
 
     def add_data_listener(self):
         if not self._data_listener_added:
             self._data_listener_added = True
-            self.parameters.to_plot.add_callback(
-                self.react_to_new_spectrum, call_with_first_value=False
-            )
+            self.parameters.to_plot.add_callback(self.react_to_new_spectrum)
 
-    def remove_data_listener(self):
+    def remove_data_listener(self) -> None:
         self._data_listener_added = False
         self.parameters.to_plot.remove_callback(self.react_to_new_spectrum)
 
-    def react_to_new_spectrum(self, plot_data):
+    def react_to_new_spectrum(self, plot_data: bytes) -> None:
         """
         React to new spectrum data.
 
         If this is executed for the first time, a reference spectrum is recorded.
 
         If the autolock is approaching the desired line, a correlation function of the
         spectrum with the reference spectrum is calculated and the laser current is
@@ -156,29 +160,32 @@
         """
         if self.parameters.pause_acquisition.value:
             return
 
         if plot_data is None or not self.parameters.autolock_running.value:
             return
 
-        plot_data = pickle.loads(plot_data)
-        if plot_data is None:
+        plot_data_unpickled = pickle.loads(plot_data)
+        if plot_data_unpickled is None:
             return
 
         is_locked = self.parameters.lock.value
 
         # check that `plot_data` contains the information we need otherwise skip this
         # round
-        if not check_plot_data(is_locked, plot_data):
+        if not check_plot_data(is_locked, plot_data_unpickled):
             return
 
         try:
             if not is_locked:
                 combined_error_signal = combine_error_signal(
-                    (plot_data["error_signal_1"], plot_data.get("error_signal_2")),
+                    (
+                        plot_data_unpickled["error_signal_1"],
+                        plot_data_unpickled.get("error_signal_2"),
+                    ),
                     self.parameters.dual_channel.value,
                     self.parameters.channel_mixing.value,
                     self.parameters.combined_offset.value,
                 )
 
                 if (
                     self.autolock_mode_detector is not None
@@ -190,22 +197,25 @@
                     self.additional_spectra.append(combined_error_signal)
 
                     if self.autolock_mode_detector.done:
                         self.start_autolock(self.autolock_mode_detector.mode)
                     else:
                         return
 
-                return self.algorithm.handle_new_spectrum(combined_error_signal)
+                if self.algorithm is not None:
+                    return self.algorithm.handle_new_spectrum(combined_error_signal)
 
             else:
-                error_signal = plot_data["error_signal"]
-                control_signal = plot_data["control_signal"]
+                error_signal = plot_data_unpickled["error_signal"]
+                control_signal = plot_data_unpickled["control_signal"]
 
                 return self.after_lock(
-                    error_signal, control_signal, plot_data.get("slow_control_signal")
+                    error_signal,
+                    control_signal,
+                    plot_data_unpickled.get("slow_control_signal"),
                 )
 
         except Exception:
             logger.exception("Error while handling new spectrum")
             self.parameters.autolock_failed.value = True
             self.exposed_stop()
 
@@ -261,15 +271,15 @@
         self.reset_properties()
         self._reset_scan()
 
         # add a listener that listens for new spectrum data and consequently # tries to
         # relock.
         self.add_data_listener()
 
-    def exposed_stop(self):
+    def exposed_stop(self) -> None:
         """Abort any operation."""
         self.parameters.autolock_preparing.value = False
         self.parameters.autolock_percentage.value = 0
         self.parameters.autolock_running.value = False
         self.parameters.autolock_locked.value = False
         self.parameters.autolock_watching.value = False
         self.parameters.fetch_additional_signals.value = True
```

### Comparing `linien-server-1.0.2rc1/linien_server/autolock/robust.py` & `linien-server-2.0.0rc1/linien_server/autolock/robust.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
             t1 = time()
             description, final_wait_time, time_scale = calculate_autolock_instructions(
                 self.spectra, (self.x0, self.x1)
             )
             t2 = time()
             dt = t2 - t1
-            logger.debug("calculation of autolock description took %s" % dt)
+            logger.debug(f"Calculation of autolock description took {dt}")
 
             # sets up a timeout: if the lock doesn't finish within a certain time span,
             # throw an error
             self.setup_timeout()
 
             # first reset lock in case it was True. This ensures that autolock starts
             # properly once all parameters are set
@@ -131,16 +131,16 @@
 
             self.parameters.autolock_preparing.value = False
 
             self._done = True
 
         else:
             logger.error(
-                "not enough spectra collected: %d of %d"
-                % (len(self.spectra), self.N_spectra_required)
+                "Not enough spectra collected:"
+                f"{len(self.spectra)} of {self.N_spectra_required}"
             )
 
     def setup_timeout(self, N_acquisitions_to_wait=5):
         """
         Robust autolock just programs the FPGA image with a set of instructions. The
         FPGA image then uses these instructions in order to actually turn on the lock
         once all conditions are met. However, it may happen that the FPGA image is
@@ -150,15 +150,15 @@
         self._timeout_start_time = time()
         self._timeout_time_to_wait = (
             N_acquisitions_to_wait
             * 2
             * sweep_speed_to_time(self.parameters.sweep_speed.value)
         )
 
-        self.parameters.ping.add_callback(self.check_for_timeout)
+        self.parameters.ping.add_callback(self.check_for_timeout, call_immediately=True)
 
     def check_for_timeout(self, ping):
         min_time_to_wait = 5
 
         if time() - self._timeout_start_time > max(
             self._timeout_time_to_wait, min_time_to_wait
         ):
@@ -178,24 +178,24 @@
 
     target_idxs = [idx - crop_left for idx in target_idxs]
 
     time_scale = int(
         round(np.mean([get_time_scale(spectrum, target_idxs) for spectrum in spectra]))
     )
 
-    logger.debug("x scale is %d" % time_scale)
+    logger.debug(f"x scale is {time_scale}")
 
     prepared_spectrum = get_diff_at_time_scale(sum_up_spectrum(spectra[0]), time_scale)
     peaks = get_all_peaks(prepared_spectrum, target_idxs)
     y_scale = peaks[0][1]
 
     lock_regions = [get_lock_region(spectrum, target_idxs) for spectrum in spectra]
 
     for tolerance_factor in [0.95, 0.9, 0.85, 0.8, 0.75, 0.7, 0.65, 0.6, 0.55, 0.5]:
-        logger.debug("try out tolerance %s" % tolerance_factor)
+        logger.debug(f"Try out tolerance {tolerance_factor}")
         peaks_filtered = [
             (peak_position, peak_height * tolerance_factor)
             for peak_position, peak_height in peaks
         ]
         # it is important to do the filtering that happens here after the previous
         # line as the previous line shrinks the values
         peaks_filtered = [
@@ -212,15 +212,15 @@
         while True:
             current_idx -= 1
             if np.abs(prepared_spectrum[current_idx]) < np.abs(
                 target_peak_described_height
             ):
                 break
         final_wait_time = target_peak_idx - current_idx
-        logger.debug("final wait time is %d samples" % final_wait_time)
+        logger.debug(f"final wait time is {final_wait_time} samples")
 
         description = []
 
         last_peak_position = 0
         for peak_position, peak_height in list(reversed(peaks_filtered)):
             # TODO: this .9 factor is very arbitrary.
             description.append(
@@ -243,20 +243,18 @@
 
         if does_work:
             break
     else:
         raise UnableToFindDescription()
 
     if len(description) > AUTOLOCK_MAX_N_INSTRUCTIONS:
-        logger.warning(
-            "warning: autolock description too long. Cropping! %s" % len(description)
-        )
+        logger.warning(f"Autolock description too long. Cropping! {description}")
         description = description[-AUTOLOCK_MAX_N_INSTRUCTIONS:]
 
-    logger.debug("description is %s" % description)
+    logger.debug(f"Description is {description}")
     return description, final_wait_time, time_scale
 
 
 def get_lock_position_from_autolock_instructions(
     spectrum, description, time_scale, initial_spectrum, final_wait_time
 ):
     summed = sum_up_spectrum(spectrum)
```

### Comparing `linien-server-1.0.2rc1/linien_server/autolock/simple.py` & `linien-server-2.0.0rc1/linien_server/autolock/simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
             return
 
         lock_point = int(
             round((shift * (-1)) * self.parameters.sweep_amplitude.value * 8191)
         )
 
-        logger.debug("lock point is %s, shift is %s" % (lock_point, shift))
+        logger.debug(f"lock point is {lock_point}, shift is {shift}")
 
         self.parameters.autolock_target_position.value = int(lock_point)
         self.parameters.autolock_preparing.value = False
         self.control.exposed_write_registers()
         self.control.exposed_start_lock()
 
         self._done = True
```

### Comparing `linien-server-1.0.2rc1/linien_server/autolock/utils.py` & `linien-server-2.0.0rc1/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2rc1/linien_server/csr.py` & `linien-server-2.0.0rc1/linien_server/csr.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,32 @@
 
 
 class PythonCSR:
     map = csrmap.csr
     constants = csrmap.csr_constants
     offset = 0x40300000
 
-    def __init__(self, rp):
+    def __init__(self, rp) -> None:
         self.rp = rp
 
-    def set_one(self, addr: str, value: int) -> None:
+    def set_one(self, addr: int, value: int) -> None:
         self.rp.write(addr, value)
 
-    def get_one(self, addr):
+    def get_one(self, addr: int):
         return int(self.rp.read(addr))
 
-    def set(self, name, value):
+    def set(self, name: str, value: int) -> None:
         map, addr, width, wr = self.map[name]
         assert wr, name
 
         ma = 1 << width
         bit_mask = ma - 1
         val = value & bit_mask
         assert value == val or ma + value == val, (
-            "value for %s out of range" % name,
+            f"Value for {name} out of range",
             (value, val, ma),
         )
 
         b = (width + 8 - 1) // 8
         for i in range(b):
             v = (val >> (8 * (b - i - 1))) & 0xFF
             self.set_one(self.offset + (map << 11) + ((addr + i) << 2), v)
@@ -62,24 +62,23 @@
         b = (nr + 8 - 1) // 8
         for i in range(b):
             v |= self.get_one(self.offset + (map << 11) + ((addr + i) << 2)) << 8 * (
                 b - i - 1
             )
         return v
 
-    def set_iir(self, prefix, b, a, z=0):
+    def set_iir(self, prefix: str, b: list[float], a: list[float]) -> None:
         shift = self.get(prefix + "_shift") or 16
         width = self.get(prefix + "_width") or 18
-        interval = self.get(prefix + "_interval") or 1
-        b, a, params = get_params(b, a, shift, width, interval)
+        bb, _, params = get_params(b, a, shift, width)
 
         for k in sorted(params):
             self.set(prefix + "_" + k, params[k])
-        self.set(prefix + "_z0", z)
-        for i in range(len(b), 3):
-            n = prefix + "_b%i" % i
+        self.set(prefix + "_z0", 0)
+        for i in range(len(bb), 3):
+            n = prefix + f"_b{i}"
             if n in self.map:
                 self.set(n, 0)
-                self.set(prefix + "_a%i" % i, 0)
+                self.set(prefix + f"_a{i}", 0)
 
     def states(self, *names):
         return sum(1 << csrmap.states.index(name) for name in names)
```

### Comparing `linien-server-1.0.2rc1/linien_server/csrmap.py` & `linien-server-2.0.0rc1/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2rc1/linien_server/iir_coeffs.py` & `linien-server-2.0.0rc1/linien_server/iir_coeffs.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien. If not, see <http://www.gnu.org/licenses/>.
 
 import warnings
 from math import ceil, log2, pi
+from typing import Optional
 
 from scipy import signal
 
 
-def make_filter(name, k=1.0, f=0.0, g=1e20, q=0.5):
+def make_filter(
+    name: str, k: float = 1.0, f: float = 0.0, g: float = 1e20, q: float = 0.5
+) -> tuple[list[float], list[float]]:
     f *= pi
 
     if name == "LP":  # k/(s + 1)
         b = [f * k / (f + 2), f * k / (f + 2)]
         a = [1, (f - 2) / (f + 2)]
 
     elif name == "HP":  # k/(1 + 1/s)
@@ -105,47 +108,51 @@
             / (q * (f**2 * g**2 + 4 * f * g + 4)),
         ]
         a = [1, 4 / (-f * g - 2), (-f * g + 2) / (f * g + 2)]
 
     return b, a
 
 
-def quantize_filter(b, a, shift=None, width=25):
+def quantize_filter(
+    b: list[float], a: list[float], shift: Optional[int] = None, width: int = 25
+) -> tuple[list[int], list[int], int]:
     b, a = [i / a[0] for i in b], [i / a[0] for i in a]
 
     if shift is None:
         shift = width
         for i in b + a:
             m = ceil(log2(abs(i)))
             if i > 0 and int(m) == m:
                 m += 1
             shift = min(shift, int(width - 1 - m))
     s = 1 << shift
 
-    b = [int(round(i * s)) for i in b]
-    a = [int(round(i * s)) for i in a]
+    bb = [int(round(i * s)) for i in b]
+    aa = [int(round(i * s)) for i in a]
 
     m = 1 << (width - 1)
-    for i in b + a:
-        assert -m <= i < m, (hex(i), hex(m))
+    for i in bb + aa:
+        assert -m <= i < m, (hex(int(i)), hex(int(m)))
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=signal.BadCoefficients)
         warnings.simplefilter("ignore", category=RuntimeWarning)
-        z, p, k = signal.tf2zpk(b, a)
+        z, p, k = signal.tf2zpk(bb, aa)
     if any(abs(_) > 1 for _ in p):
         warnings.warn(
             "unstable filter: z={}, p={}, k={}".format(z, p, k), RuntimeWarning
         )
 
-    return b, a, shift
+    return bb, aa, shift
 
 
-def get_params(b, a, shift=None, width=25, interval=1):
-    b, a, shift = quantize_filter(b, a, shift, width)
+def get_params(
+    b: list[float], a: list[float], shift: Optional[int] = None, width: int = 25
+) -> tuple[list[int], list[int], dict[str, int]]:
+    bb, aa, shift = quantize_filter(b, a, shift, width)
     params = {}
-    for i, (ai, bi) in enumerate(zip(a, b)):
-        params["a%i" % i] = int(-ai)
-        params["b%i" % i] = int(bi)
+    for i, (ai, bi) in enumerate(zip(aa, bb)):
+        params[f"a{i}"] = int(-ai)
+        params[f"b{i}"] = int(bi)
     del params["a0"]
     # params["shift"] = shift
-    return b, a, params
+    return bb, aa, params
```

### Comparing `linien-server-1.0.2rc1/linien_server/influxdb.py` & `linien-server-2.0.0rc1/linien_server/influxdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,53 +13,63 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from threading import Event, Thread
 from time import sleep
-from typing import Tuple
 
-import requests
+from influxdb_client import InfluxDBClient
+from influxdb_client.client.write_api import SYNCHRONOUS
+from linien_common.communication import ParameterValues
 from linien_common.influxdb import InfluxDBCredentials, save_credentials
 from linien_server.parameters import Parameters
 
 
 class InfluxDBLogger:
     def __init__(
         self, credentials: InfluxDBCredentials, parameters: Parameters
     ) -> None:
-        self.credentials = credentials
-        self.parameters = parameters
+        self.credentials: InfluxDBClient = credentials
+        self.parameters: Parameters = parameters
         self.stop_event = Event()
         self.stop_event.set()
+        self.update_connection()
 
     @property
     def credentials(self) -> InfluxDBCredentials:
         return self._credentials
 
     @credentials.setter
     def credentials(self, value: InfluxDBCredentials) -> None:
         self._credentials = value
         save_credentials(value)
 
+    def update_connection(self) -> InfluxDBClient:
+        client = InfluxDBClient(
+            url=self.credentials.url,
+            token=self.credentials.token,
+            org=self.credentials.org,
+        )
+        self.write_api = client.write_api(write_options=SYNCHRONOUS)
+
     def start_logging(self, interval: float) -> None:
         conn_success, status_code, message = self.test_connection(self.credentials)
         self.thread = Thread(
             target=self._logging_loop,
             args=(interval,),
             daemon=True,
         )
         if conn_success:
             self.stop_event.clear()
             self.thread.start()
         else:
             raise ConnectionError(
-                "Failed to connect to InfluxDB database: %s (Status code: %s)"
-                % (message, status_code)
+                "Failed to connect to InfluxDB database: "
+                f" {message} (Status code: {status_code})"
             )
 
     def stop_logging(self) -> None:
         self.stop_event.set()
         self.thread.join()
 
     def _logging_loop(self, interval: float) -> None:
@@ -73,52 +83,33 @@
                     else:
                         data[name] = param.value
             self.write_data(self.credentials, data)
             sleep(interval)
 
     def test_connection(
         self, credentials: InfluxDBCredentials
-    ) -> Tuple[bool, int, str]:
+    ) -> tuple[bool, int, str]:
         """Write empty data to the server to test the connection"""
-        try:
-            response = self.write_data(credentials, data={})
-            success = response.status_code == 204
-            status_code = response.status_code
-            text = response.text
-        except requests.exceptions.ConnectionError:
-            success = False
-            status_code = 404
-            text = "Failed to establish connection."
-        return success, status_code, text
+        client = InfluxDBClient(
+            url=credentials.url,
+            token=credentials.token,
+            org=credentials.org,
+        )
+
+        # FIXME: This does not test the credentials, yet.
+        status_code = 0
+        message = ""
+        success = client.ping()
+        return success, status_code, message
 
     def write_data(
-        self, credentials: InfluxDBCredentials, data: dict
-    ) -> requests.Response:
+        self, credentials: InfluxDBCredentials, fields: dict[str, ParameterValues]
+    ) -> None:
         """Write data to the database"""
-        endpoint = credentials.url + "/api/v2/write"
-        headers = {
-            "Authorization": "Token " + credentials.token,
-            "Content-Type": "text/plain; charset=utf-8",
-            "Accept": "application/json",
-        }
-        params = {
-            "org": credentials.org,
-            "bucket": credentials.bucket,
-            "precision": "ns",
-        }
-
-        point = self._convert_to_line_protocol(data)
-
-        response = requests.post(endpoint, headers=headers, params=params, data=point)
-        return response
-
-    def _convert_to_line_protocol(self, data: dict) -> str:
-        if not data:
-            return ""
-        point = self.credentials.measurement
-        for i, (key, value) in enumerate(data.items()):
-            if i == 0:
-                point += " "
-            else:
-                point += ","
-            point += "%s=%s" % (key, value)
-        return point
+        self.write_api.write(
+            bucket=credentials.bucket,
+            org=credentials.org,
+            record={
+                "measurement": credentials.measurement,
+                "fields": fields,
+            },
+        )
```

### Comparing `linien-server-1.0.2rc1/linien_server/noise_analysis.py` & `linien-server-2.0.0rc1/linien_server/noise_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,31 +17,32 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import pickle
 import random
 import string
 from time import sleep, time
-from typing import Tuple
 
 import numpy as np
 from linien_common.common import PSDAlgorithm
 from linien_server.optimization.engine import MultiDimensionalOptimizationEngine
 from pylpsd import lpsd
 from scipy import signal
 
+from .parameters import Parameters
+
 ALL_DECIMATIONS = list(range(32))
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 def calculate_psd(
     sig: np.ndarray, fs: float, algorithm: PSDAlgorithm
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Calculate the power spectral density.
 
     :param sig: The signal to calculate the PSD for.
     :param fs: The sampling frequency.
     :param algorithm: The PSD algorithm to use.
     :return: One-sided power spectral density.
@@ -98,14 +99,16 @@
 
 
 def generate_curve_uuid():
     return "".join(random.choice(string.ascii_lowercase) for i in range(10))
 
 
 class PSDAcquisition:
+    parameters: Parameters
+
     def __init__(self, control, parameters, is_child=False):
         self.decimation_index = 0
 
         self.recorded_signals_by_decimation = {}
         self.recorded_psds_by_decimation = {}
 
         self.running = True
@@ -122,15 +125,15 @@
             self.parameters.psd_acquisition_running.value = True
         except Exception as e:
             self.cleanup()
             raise e
 
     def add_callbacks(self):
         self.parameters.acquisition_raw_data.add_callback(
-            self.react_to_new_signal, call_with_first_value=False
+            self.react_to_new_signal, call_immediately=False
         )
 
     def cleanup(self):
         self.running = False
         self.parameters.psd_acquisition_running.value = False
 
         self.parameters.acquisition_raw_data.remove_callback(self.react_to_new_signal)
@@ -147,16 +150,16 @@
         try:
             if not self.running or self.parameters.pause_acquisition.value:
                 return
 
             data = pickle.loads(data_pickled)
 
             current_decimation = self.parameters.acquisition_raw_decimation.value
-            logger.debug("recorded signal for decimation %s" % current_decimation)
-            logger.debug("recording took %s s" % (time() - self.time_decimation_set))
+            logger.debug(f"Recorded signal for decimation {current_decimation}")
+            logger.debug(f"Recording took {time()-self.time_decimation_set} s")
             self.recorded_signals_by_decimation[current_decimation] = data
             self.recorded_psds_by_decimation[current_decimation] = residual_freq_noise(
                 1 / (125e6) * (2 ** (current_decimation)),
                 data[0],
                 algorithm=self.parameters.psd_algorithm.value,
             )
 
@@ -169,15 +172,15 @@
                 > self.parameters.psd_acquisition_max_decimation.value
             )
 
             self.publish_psd_data(complete)
 
             if not complete:
                 new_decimation = self.decimation_index
-                logger.debug("set new decimation %s" % new_decimation)
+                logger.debug(f"Set new decimation {new_decimation}")
                 self.set_decimation(new_decimation)
             else:
                 self.cleanup()
 
         except Exception as e:
             self.cleanup()
             raise e
@@ -222,26 +225,28 @@
         self.control.exposed_continue_acquisition()
 
     def exposed_stop(self):
         self.cleanup()
 
 
 class PIDOptimization:
+    parameters: Parameters
+
     def __init__(self, control, parameters):
         self.control = control
         self.parameters = parameters
 
         self.engine = MultiDimensionalOptimizationEngine(
             [[100, 4000], [100, 4000]], x0=[2000, 2000]
         )
 
     def run(self):
         try:
             self.parameters.psd_data_complete.add_callback(
-                self.psd_data_received, call_with_first_value=False
+                self.psd_data_received, call_immediately=False
             )
             self.parameters.psd_optimization_running.value = True
             self.start_single_psd_measurement()
         except Exception as e:
             self.cleanup()
             raise e
 
@@ -262,15 +267,15 @@
     def psd_data_received(self, psd_data_pickled):
         try:
             # psd data doesn't have to be stored here as a client that is interested
             # in it may listen to parameters.psd_data change events
             psd_data = pickle.loads(psd_data_pickled)
 
             params = (psd_data["p"], psd_data["i"])
-            logger.debug("received fitness %s, %s" % (psd_data["fitness"], params))
+            logger.debug(f"Received fitness {psd_data['fitness']}, {params}")
 
             self.engine.tell(psd_data["fitness"], params)
 
             self.start_single_psd_measurement()
 
             done = self.engine.finished()
             if done:
```

### Comparing `linien-server-1.0.2rc1/linien_server/optimization/approach_line.py` & `linien-server-2.0.0rc1/linien_server/optimization/approach_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         # now, we calculate the correlation to find the shift
         shift, zoomed_ref, zoomed_err = determine_shift_by_correlation(
             self.zoom_factor, self.first_error_signal, error_signal
         )
         shift *= initial_sweep_amplitude
         self.history.append((zoomed_ref, zoomed_err))
-        self.history.append("shift %f" % (-1 * shift))
+        self.history.append(f"shift {-1 * shift}")
 
         if self.N_at_this_zoom == 0:
             # if we are at the final zoom, we should be very quick.
             # Therefore, we just correct the current and turn the lock on
             # immediately. We skip the rest of this method (drift detection etc.)
             next_step_is_lock = self.zoom_factor >= self.target_zoom
             if next_step_is_lock:
```

### Comparing `linien-server-1.0.2rc1/linien_server/optimization/engine.py` & `linien-server-2.0.0rc1/linien_server/optimization/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                         self.parameters.modulation_frequency: 0,
                         self.parameters.modulation_amplitude: 1,
                     }[param]
                     complete_parameter_set[idx] = value
 
             params.optimization_optimized_parameters.value = complete_parameter_set
 
-        logger.debug("improvement %d" % (improvement * 100))
+        logger.debug(f"improvement {improvement * 100}")
 
         fitness = math.log(1 / optimized_slope)
 
         if self.last_parameters_internal is not None:
             self.opt.tell(fitness, self.last_parameters_internal)
 
     def use_best_parameters(self):
```

### Comparing `linien-server-1.0.2rc1/linien_server/optimization/general.py` & `linien-server-2.0.0rc1/linien_server/optimization/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 """Module providing the Optimizer interface class."""
 
-from typing import List, NewType
+from typing import NewType
 
-Params = NewType("Params", List[float])
+Params = NewType("Params", list[float])
 """A type alias for actual optmizer params. """
 
 
 class Optimizer:
     """Interface for the "Optimizer" type classes."""
 
     def __init__(self):
```

### Comparing `linien-server-1.0.2rc1/linien_server/optimization/optimization.py` & `linien-server-2.0.0rc1/linien_server/optimization/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,30 +58,30 @@
         max_idx = np.argmax(cropped)
         self.x0, self.x1 = x0 + min_idx, x0 + max_idx
 
         self.record_first_error_signal(spectrum)
 
         params = self.parameters
         self.engine = OptimizerEngine(self.control, params)
-        params.to_plot.add_callback(self.react_to_new_spectrum)
+        params.to_plot.add_callback(self.react_to_new_spectrum, call_immediately=True)
         params.optimization_running.value = True
         params.optimization_improvement.value = 0
 
     def record_first_error_signal(self, error_signal):
         (
             mean_signal,
             _2,
             target_zoom,
             rolled_error_signal,
             line_width,
             peak_idxs,
         ) = get_lock_point(
             error_signal,
             *list(sorted([self.x0, self.x1])),
-            final_zoom_factor=FINAL_ZOOM_FACTOR
+            final_zoom_factor=FINAL_ZOOM_FACTOR,
         )
 
         self.target_zoom = target_zoom
         self.first_error_signal = rolled_error_signal
 
         self.approacher = Approacher(
             self.control,
@@ -99,16 +99,16 @@
         try:
             params = self.parameters
 
             dual_channel = params.dual_channel.value
             channel = params.optimization_channel.value
             spectrum_idx = 1 if not dual_channel else (1, 2)[channel]
             unpickled = pickle.loads(spectrum)
-            spectrum = unpickled["error_signal_%d" % spectrum_idx]
-            quadrature = unpickled["error_signal_%d_quadrature" % spectrum_idx]
+            spectrum = unpickled[f"error_signal_{spectrum_idx}"]
+            quadrature = unpickled[f"error_signal_{spectrum_idx}_quadrature"]
 
             if self.parameters.optimization_approaching.value:
                 approaching_finished = self.approacher.approach_line(spectrum)
                 if approaching_finished:
                     self.parameters.optimization_approaching.value = False
             else:
                 self.iteration += 1
```

### Comparing `linien-server-1.0.2rc1/linien_server/optimization/utils.py` & `linien-server-2.0.0rc1/linien_server/optimization/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 from scipy import optimize, stats
 
-# after the line was centered, its width will be 1/FINAL_ZOOM_FACTOR of the
-# view.
+# after the line was centered, its width will be 1/FINAL_ZOOM_FACTOR of the view.
 FINAL_ZOOM_FACTOR = 20
 
 
 def get_max_slope(signal, final_zoom_factor):
     line_width = len(signal) / final_zoom_factor
     window_width = 1.5 * line_width
     center = len(signal) / 2
```

### Comparing `linien-server-1.0.2rc1/linien_server/parameters.py` & `linien-server-2.0.0rc1/linien_server/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
 from time import time
-from typing import Any, Callable, Dict, Iterator, List, Tuple
+from typing import Any, Callable, Iterator
 
 import linien_server
 from linien_common.common import AutolockMode, MHz, PSDAlgorithm, Vpp
 from linien_common.config import USER_DATA_PATH
 
-PARAMETER_STORE_FILENAME = "linien_parameters.json"
+PARAMETER_STORE_FILENAME = "parameters.json"
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class Parameter:
     """Represents a single parameter and is used by `Parameters`."""
@@ -78,21 +78,19 @@
         for callback in self._callbacks.copy():
             callback(value)
 
     def reset(self):
         self.value = self._start
 
     def add_callback(
-        self,
-        function: Callable[[Any], None],
-        call_with_first_value: bool = True,
+        self, function: Callable[[Any], None], call_immediately: bool = False
     ) -> None:
         self._callbacks.add(function)
 
-        if call_with_first_value:
+        if call_immediately:
             if self._value is not None:
                 function(self._value)
 
     def remove_callback(self, function: Callable[[Any], None]) -> None:
         if function in self._callbacks:
             self._callbacks.remove(function)
 
@@ -117,23 +115,23 @@
 
     On the client side, access happens through `RemoteParameters` which
     transparently mimics the behavior of this class. Have a look at the comments
     below for a description of each parameter.
     """
 
     def __init__(self):
-        # Dict[str, List[Tuple[str, Any]]]
+        # dict[str, list[tuple[str, Any]]]
         self._changed_parameters_queue = {}
-        # Dict[Tuple[Parameter, Callable[[Any], None]]]
+        # dict[tuple[Parameter, Callable[[Any], None]]]
         self._remote_listener_callbacks = {}
 
         self.to_plot = Parameter(sync=False)
         """
-        The `to_plot` parameter is a pickled dictionary that contains signalsvthat may
-        be plotted. Depending on the locking state, it may contain thesevsignals:
+        The `to_plot` parameter is a pickled dictionary that contains signals that may
+        be plotted. Depending on the locking state, it may contain these signals:
         Unlocked state:
           - `error_signal_1` and `error_signal_1_quadrature`:
               IQ-demodulated and low-pass-filtered error signals from ANALOG IN 0
           - `error_signal_2` and `error_signal_2_quadrature`:
               IQ-demodulated and low-pass-filtered error signals from ANALOG IN 1. These
               signals are only available if in dual-channel spectroscopy mode is
               enabled. Otherwise the un-demodulated monitor_signal` is shown.
@@ -590,22 +588,22 @@
         self.psd_algorithm = Parameter(start=PSDAlgorithm.LPSD)
         self.psd_acquisition_running = Parameter(start=False)
         self.psd_optimization_running = Parameter(start=False)
         self.psd_acquisition_max_decimation = Parameter(
             start=18, min_=1, max_=32, restorable=True
         )
 
-    def __iter__(self) -> Iterator[Tuple[str, Parameter]]:
+    def __iter__(self) -> Iterator[tuple[str, Parameter]]:
         for name, param in self.__dict__.items():
             if isinstance(param, Parameter):
                 yield name, param
 
     def init_parameter_sync(
         self, uuid: str
-    ) -> Iterator[Tuple[str, Any, bool, bool, bool, bool]]:
+    ) -> Iterator[tuple[str, Any, bool, bool, bool, bool]]:
         """
         To be called by a remote client: Yields all parameters as well as their values
         and if the parameters are suited to be cached registers a listener that pushes
         changes of these parameters to the client.
         """
         for name, param in self:
             yield (
@@ -624,31 +622,29 @@
         self._remote_listener_callbacks.setdefault(uuid, [])
 
         def append_changed_values_to_queue(value: Any) -> None:
             """Appends changed values to the queue of a specific client."""
             if uuid in self._changed_parameters_queue:
                 self._changed_parameters_queue[uuid].append((param_name, value))
 
-        param = getattr(self, param_name)
-        param.add_callback(append_changed_values_to_queue)
+        param: Parameter = getattr(self, param_name)
+        param.add_callback(append_changed_values_to_queue, call_immediately=True)
 
         self._remote_listener_callbacks[uuid].append(
             (param, append_changed_values_to_queue)
         )
 
     def unregister_remote_listeners(self, uuid: str):
         for param, callback in self._remote_listener_callbacks[uuid]:
             param.remove_callback(callback)
 
         del self._changed_parameters_queue[uuid]
         del self._remote_listener_callbacks[uuid]
 
-    def get_changed_parameters_queue(
-        self, uuid: str
-    ) -> Dict[str, List[Tuple[str, Any]]]:
+    def get_changed_parameters_queue(self, uuid: str) -> list[tuple[str, Any]]:
         """Get the queue of parameter changes for a specific client."""
         queue = self._changed_parameters_queue.get(uuid, [])
         self._changed_parameters_queue[uuid] = []
 
         # filter out multiple values for collapsible parameters
         already_has_value = []
         for idx in reversed(range(len(queue))):
@@ -662,25 +658,27 @@
 
 
 def restore_parameters(parameters: Parameters) -> Parameters:
     """When the server starts, this method restores previously saved parameters."""
     filename = str(USER_DATA_PATH / PARAMETER_STORE_FILENAME)
     try:
         with open(filename, "r") as f:
+            logger.info(f"Restoring parameters from {filename}")
             data = json.load(f)
     except FileNotFoundError:
+        logger.info(f"Couldn't find {filename}. Using default parameters.")
         return parameters
 
     for name, attributes in data["parameters"].items():
         try:
             getattr(parameters, name).value = attributes["value"]
             getattr(parameters, name).log = attributes["log"]
         except AttributeError:  # ignore parameters that don't exist (anymore)
             continue
-    logger.info("Restored parameters from %s" % filename)
+    logger.info(f"Restored parameters from {filename}")
     return parameters
 
 
 def save_parameters(parameters: Parameters) -> None:
     """Gather all parameters and store them on disk."""
 
     parameters_dict = {}
@@ -695,8 +693,8 @@
                 "version": linien_server.__version__,
                 "time": time(),
                 "parameters": parameters_dict,
             },
             f,
             indent=2,
         )
-    logger.info("Saved parameters to %s" % filename)
+    logger.info(f"Saved parameters to {filename}")
```

### Comparing `linien-server-1.0.2rc1/linien_server/registers.py` & `linien-server-2.0.0rc1/linien_server/registers.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,32 @@
             self.acquisition = AcquisitionService()
         else:
             # AcquisitionService has to be started manually on the Red Pitaya
             self.acquisition = rpyc.connect(host, ACQUISITION_PORT).root
 
         self._last_sweep_speed = None
         self._last_raw_acquisition_settings = None
-        self._iir_cache = {}  # type: ignore[var-annotated]
+        self._iir_cache: dict[str, tuple[list[float], list[float]]] = {}
 
         self.parameters.lock.add_callback(self.acquisition.exposed_set_lock_status)
         self.parameters.fetch_additional_signals.add_callback(
-            self.acquisition.exposed_set_fetch_additional_signals  # noqa: E501
+            self.acquisition.exposed_set_fetch_additional_signals, call_immediately=True
         )
         self.parameters.dual_channel.add_callback(
-            self.acquisition.exposed_set_dual_channel
+            self.acquisition.exposed_set_dual_channel, call_immediately=True
         )
 
     def write_registers(self):
         """Writes data from `parameters` to the FPGA."""
 
-        max_ = lambda val: val if np.abs(val) <= 8191 else (8191 * val / np.abs(val))
-        phase_to_delay = lambda phase: int(phase / 360 * (1 << 14))
+        def max_(val):
+            return val if np.abs(val) <= 8191 else (8191 * val / np.abs(val))
+
+        def phase_to_delay(phase):
+            return int(phase / 360 * (1 << 14))
 
         if not self.parameters.dual_channel.value:
             factor_a = 256
             factor_b = 0
         else:
             factor_a, factor_b = convert_channel_mixing_value(
                 self.parameters.channel_mixing.value
@@ -95,21 +98,25 @@
                 DEFAULT_SWEEP_SPEED
                 * self.parameters.sweep_amplitude.value
                 / (2**self.parameters.sweep_speed.value)
             ),
             # NOTE: Sweep center is set by `logic_out_offset`.
             logic_sweep_min=-1 * max_(self.parameters.sweep_amplitude.value * 8191),
             logic_sweep_max=max_(self.parameters.sweep_amplitude.value * 8191),
-            logic_mod_freq=self.parameters.modulation_frequency.value
-            if not self.parameters.pid_only_mode.value
-            else 0,
-            logic_mod_amp=self.parameters.modulation_amplitude.value
-            if (self.parameters.modulation_frequency.value > 0)
-            and (not self.parameters.pid_only_mode.value)
-            else 0,
+            logic_mod_freq=(
+                self.parameters.modulation_frequency.value
+                if not self.parameters.pid_only_mode.value
+                else 0
+            ),
+            logic_mod_amp=(
+                self.parameters.modulation_amplitude.value
+                if (self.parameters.modulation_frequency.value > 0)
+                and (not self.parameters.pid_only_mode.value)
+                else 0
+            ),
             logic_dual_channel=int(self.parameters.dual_channel.value),
             logic_pid_only_mode=int(self.parameters.pid_only_mode.value),
             logic_chain_a_factor=factor_a,
             logic_chain_b_factor=factor_b,
             logic_chain_a_offset=twos_complement(
                 int(self.parameters.offset_a.value), 14
             ),
@@ -132,32 +139,32 @@
             logic_autolock_autolock_mode=self.parameters.autolock_mode.value,
             logic_autolock_robust_N_instructions=len(
                 self.parameters.autolock_instructions.value
             ),
             logic_autolock_robust_time_scale=self.parameters.autolock_time_scale.value,
             logic_autolock_robust_final_wait_time=self.parameters.autolock_final_wait_time.value,  # noqa: E501
             # channel A
-            fast_a_demod_delay=phase_to_delay(
-                self.parameters.demodulation_phase_a.value
-            )
-            if (self.parameters.modulation_frequency.value > 0)
-            and (not self.parameters.pid_only_mode.value)
-            else 0,
+            fast_a_demod_delay=(
+                phase_to_delay(self.parameters.demodulation_phase_a.value)
+                if (self.parameters.modulation_frequency.value > 0)
+                and (not self.parameters.pid_only_mode.value)
+                else 0
+            ),
             fast_a_demod_multiplier=self.parameters.demodulation_multiplier_a.value,
             fast_a_dx_sel=csrmap.signals.index("zero"),
             fast_a_y_tap=2,
             fast_a_dy_sel=csrmap.signals.index("zero"),
             fast_a_invert=int(self.parameters.invert_a.value),
             # channel B
-            fast_b_demod_delay=phase_to_delay(
-                self.parameters.demodulation_phase_b.value
-            )
-            if (self.parameters.modulation_frequency.value > 0)
-            and (not self.parameters.pid_only_mode.value)
-            else 0,
+            fast_b_demod_delay=(
+                phase_to_delay(self.parameters.demodulation_phase_b.value)
+                if (self.parameters.modulation_frequency.value > 0)
+                and (not self.parameters.pid_only_mode.value)
+                else 0
+            ),
             fast_b_demod_multiplier=self.parameters.demodulation_multiplier_b.value,
             fast_b_dx_sel=csrmap.signals.index("zero"),
             fast_b_y_tap=1,
             fast_b_dy_sel=csrmap.signals.index("zero"),
             fast_b_invert=int(self.parameters.invert_b.value),
             # trigger on sweep
             scopegen_external_trigger=1,
@@ -169,16 +176,16 @@
             gpio_n_do1_en=csrmap.signals.index("zero"),
             logic_slow_decimation=16,
         )
 
         for instruction_idx, [wait_for, peak_height] in enumerate(
             self.parameters.autolock_instructions.value
         ):
-            new["logic_autolock_robust_peak_height_%d" % instruction_idx] = peak_height
-            new["logic_autolock_robust_wait_for_%d" % instruction_idx] = wait_for
+            new[f"logic_autolock_robust_peak_height_{instruction_idx}"] = peak_height
+            new["logic_autolock_robust_wait_for_{instruction_idx}"] = wait_for
 
         if self.parameters.lock.value:
             # display combined error signal and control signal
             new.update(
                 {
                     "scopegen_adc_a_sel": csrmap.signals.index(
                         "logic_combined_error_signal"
@@ -285,23 +292,21 @@
             1
             if channel_polarity(slow_control_channel)
             == channel_polarity(control_channel)
             else -1
         )
 
         for chain in ("a", "b"):
-            automatic = getattr(self.parameters, "filter_automatic_%s" % chain).value
+            automatic = getattr(self.parameters, f"filter_automatic_{chain}").value
             # iir_idx means iir_c or iir_d
             for iir_idx in range(2):
                 # iir_sub_idx means in-phase signal or quadrature signal
                 for iir_sub_idx in range(2):
-                    iir_name = "fast_%s_iir_%s_%d" % (
-                        chain,
-                        ("c", "d")[iir_idx],
-                        iir_sub_idx + 1,
+                    iir_name = (
+                        f"fast_{chain}_iir_{('c', 'd')[iir_idx]}_{iir_sub_idx + 1}"
                     )
 
                     if automatic:
                         filter_enabled = True
                         filter_type = FilterType.LOW_PASS
                         filter_frequency = (
                             self.parameters.modulation_frequency.value / MHz * 1e6 / 2
@@ -312,23 +317,21 @@
                         # also helpful if the raw (not demodulated) signal should be
                         # displayed which can be achieved by setting modulation
                         # frequency to 0.
                         if filter_frequency < 10:
                             filter_enabled = False
                     else:
                         filter_enabled = getattr(
-                            self.parameters,
-                            "filter_%d_enabled_%s" % (iir_idx + 1, chain),
+                            self.parameters, f"filter_{iir_idx + 1}_enabled_{chain}"
                         ).value
                         filter_type = getattr(
-                            self.parameters, "filter_%d_type_%s" % (iir_idx + 1, chain)
+                            self.parameters, f"filter_{iir_idx + 1}_type_{chain}"
                         ).value
                         filter_frequency = getattr(
-                            self.parameters,
-                            "filter_%d_frequency_%s" % (iir_idx + 1, chain),
+                            self.parameters, f"filter_{iir_idx + 1}_frequency_{chain}"
                         ).value
 
                     if not filter_enabled:
                         self.set_iir(iir_name, *make_filter("P", k=1))
                     else:
                         if filter_type == FilterType.LOW_PASS:
                             self.set_iir(
@@ -342,15 +345,15 @@
                                 iir_name,
                                 *make_filter(
                                     "HP", f=filter_frequency / fpga_base_freq, k=1
                                 ),
                             )
                         else:
                             raise Exception(
-                                "unknown filter %s for %s" % (filter_type, iir_name)
+                                f"Unknown filter {filter_type} for {iir_name}"
                             )
 
         if lock_changed:
             if self.parameters.lock.value:
                 # set PI parameters
                 self.set_pid(kp, ki, kd, slope, reset=0, request_lock=1)
                 self.set_slow_pid(slow_strength, slow_slope, reset=0)
@@ -381,21 +384,21 @@
 
         if reset is not None:
             self.set("slow_chain_pid_reset", reset)
 
     def set(self, key, value):
         self.acquisition.exposed_set_csr(key, value)
 
-    def set_iir(self, iir_name, *args):
-        if self._iir_cache.get(iir_name) != args:
+    def set_iir(self, iir_name: str, b: list[float], a: list[float]) -> None:
+        if self._iir_cache.get(iir_name) != (b, a):
             # as setting iir parameters takes some time, take care that we don't  do it
             # too often
-            self.acquisition.exposed_set_iir_csr(iir_name, *args)
-            self._iir_cache[iir_name] = args
+            self.acquisition.exposed_set_iir_csr(iir_name, b, a)
+            self._iir_cache[iir_name] = (b, a)
 
 
-def twos_complement(num, N_bits):
+def twos_complement(num: int, N_bits: int) -> int:
     max_ = 1 << (N_bits - 1)
     full = 2 * max_
     if num < 0:
         num += full
     return num
```

### Comparing `linien-server-1.0.2rc1/linien_server/server.py` & `linien-server-2.0.0rc1/linien_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,37 +18,38 @@
 
 import _thread
 import atexit
 import logging
 import pickle
 from copy import copy
 from random import randint, random
+from socket import socket
 from threading import Event, Thread
 from time import sleep
-from typing import List, Optional, Tuple
+from typing import Any, Callable
 
-import click
 import numpy as np
 import rpyc
 from linien_common.common import N_POINTS, check_plot_data, update_signal_history
 from linien_common.communication import (
-    no_authenticator,
+    LinienControlService,
+    ParameterValues,
     pack,
     unpack,
-    username_and_password_authenticator,
 )
-from linien_common.config import DEFAULT_SERVER_PORT
+from linien_common.config import SERVER_PORT
 from linien_common.influxdb import InfluxDBCredentials, restore_credentials
 from linien_server import __version__
 from linien_server.autolock.autolock import Autolock
 from linien_server.influxdb import InfluxDBLogger
 from linien_server.noise_analysis import PIDOptimization, PSDAcquisition
 from linien_server.optimization.optimization import OptimizeSpectroscopy
 from linien_server.parameters import Parameters, restore_parameters, save_parameters
 from linien_server.registers import Registers
+from rpyc.core.protocol import Connection
 from rpyc.utils.server import ThreadedServer
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class BaseService(rpyc.Service):
@@ -57,99 +58,103 @@
     on the client.
     """
 
     def __init__(self) -> None:
         self.parameters = Parameters()
         self.parameters = restore_parameters(self.parameters)
         atexit.register(save_parameters, self.parameters)
-        self._uuid_mapping = {}  # type: ignore[var-annotated]
+        self._uuid_mapping: dict[Connection, str] = {}
 
         influxdb_credentials = restore_credentials()
         self.influxdb_logger = InfluxDBLogger(influxdb_credentials, self.parameters)
 
         self.stop_event = Event()
         self.stop_log_event = Event()
 
-    def on_connect(self, client) -> None:
-        self._uuid_mapping[client] = client.root.uuid
+    def on_connect(self, conn: Connection) -> None:
+        self._uuid_mapping[conn] = conn.root.uuid
 
-    def on_disconnect(self, client) -> None:
-        uuid = self._uuid_mapping[client]
+    def on_disconnect(self, conn: Connection) -> None:
+        uuid = self._uuid_mapping[conn]
         self.parameters.unregister_remote_listeners(uuid)
 
     def exposed_get_server_version(self) -> str:
         return __version__
 
-    def exposed_get_param(self, param_name: str) -> bytes:
+    def exposed_get_param(self, param_name: str) -> bytes | ParameterValues:
         return pack(getattr(self.parameters, param_name).value)
 
-    def exposed_set_param(self, param_name: str, value: bytes) -> None:
+    def exposed_set_param(
+        self, param_name: str, value: bytes | ParameterValues
+    ) -> None:
         getattr(self.parameters, param_name).value = unpack(value)
 
     def exposed_reset_param(self, param_name: str) -> None:
         getattr(self.parameters, param_name).reset()
 
-    def exposed_init_parameter_sync(self, uuid: str) -> bytes:
-        return pack(list(self.parameters.init_parameter_sync(uuid)))
+    def exposed_init_parameter_sync(
+        self, uuid: str
+    ) -> list[tuple[str, Any, bool, bool, bool, bool]]:
+        return list(self.parameters.init_parameter_sync(uuid))
 
     def exposed_register_remote_listener(self, uuid: str, param_name: str) -> None:
         self.parameters.register_remote_listener(uuid, param_name)
 
     def exposed_register_remote_listeners(
-        self, uuid: str, param_names: List[str]
+        self, uuid: str, param_names: list[str]
     ) -> None:
         for param_name in param_names:
             self.exposed_register_remote_listener(uuid, param_name)
 
-    def exposed_get_changed_parameters_queue(self, uuid: str) -> bytes:
-        return pack(self.parameters.get_changed_parameters_queue(uuid))
+    def exposed_get_changed_parameters_queue(self, uuid: str) -> list[tuple[str, Any]]:
+        return self.parameters.get_changed_parameters_queue(uuid)
 
     def exposed_set_parameter_log(self, param_name: str, value: bool) -> None:
         if getattr(self.parameters, param_name).log != value:
-            logger.debug("Setting log for %s to %s" % (param_name, value))
+            logger.debug(f"Setting log for {param_name} to {value}")
             getattr(self.parameters, param_name).log = value
 
     def exposed_get_parameter_log(self, param_name: str) -> bool:
         return getattr(self.parameters, param_name).log
 
     def exposed_update_influxdb_credentials(
         self, credentials: InfluxDBCredentials
-    ) -> Tuple[bool, int, str]:
+    ) -> tuple[bool, int, str]:
         credentials = copy(credentials)
         (
             connection_succesful,
             status_code,
             message,
         ) = self.influxdb_logger.test_connection(credentials)
         if connection_succesful:
             self.influxdb_logger.credentials = credentials
             logger.info("InfluxDB credentials updated successfully")
         else:
             logger.info(
-                "InfluxDB credentials update failed. Error message: %s (Status Code %s)"
-                % (message, status_code)
+                "InfluxDB credentials update failed. Error message: "
+                f" {message} (Status Code {status_code})"
             )
         return connection_succesful, status_code, message
 
-    def exposed_get_influxdb_credentials(self) -> bytes:
-        return pack(self.influxdb_logger.credentials)
+    def exposed_get_influxdb_credentials(self) -> InfluxDBCredentials:
+        return self.influxdb_logger.credentials
 
     def exposed_start_logging(self, interval: float) -> None:
         logger.info("Starting logging")
         self.influxdb_logger.start_logging(interval)
 
     def exposed_stop_logging(self) -> None:
         logger.info("Stopping logging")
         self.influxdb_logger.stop_logging()
 
     def exposed_get_logging_status(self) -> bool:
         return not self.influxdb_logger.stop_event.is_set()
 
 
-class RedPitayaControlService(BaseService):
+class RedPitayaControlService(BaseService, LinienControlService):
     """Control server that runs on the RP that provides high-level methods."""
 
     def __init__(self, host=None):
         self._cached_data = {}
         self.exposed_is_locked = None
 
         super(RedPitayaControlService, self).__init__()
@@ -179,17 +184,17 @@
         self.exposed_write_registers()
 
     def _send_ping_loop(self, stop_event: Event):
         MAX_PING = 3
         while not stop_event.is_set():
             self.parameters.ping.value += 1
             if self.parameters.ping.value <= MAX_PING:
-                logger.debug("ping  %s" % self.parameters.ping.value)
+                logger.debug(f"Ping  {self.parameters.ping.value}")
                 if self.parameters.ping.value == MAX_PING:
-                    logger.debug("further pings will be suppressed")
+                    logger.debug("Further pings will be suppressed")
             sleep(1)
 
     def _push_acquired_data_to_parameters(self, stop_event: Event):
         last_hash = None
         while not stop_event.is_set():
             (
                 new_data_returned,
@@ -219,18 +224,18 @@
                         continue
 
                     self.parameters.to_plot.value = new_data
 
                     # generate signal stats
                     stats = {}
                     for signal_name, signal in data_loaded.items():
-                        stats["%s_mean" % signal_name] = np.mean(signal)
-                        stats["%s_std" % signal_name] = np.std(signal)
-                        stats["%s_max" % signal_name] = np.max(signal)
-                        stats["%s_min" % signal_name] = np.min(signal)
+                        stats[f"{signal_name}_mean"] = np.mean(signal)
+                        stats[f"{signal_name}_std"] = np.std(signal)
+                        stats[f"{signal_name}_max"] = np.max(signal)
+                        stats[f"{signal_name}_min"] = np.min(signal)
                     self.parameters.signal_stats.value = stats
                     # update signal history (if in locked state)
                     (
                         self.parameters.control_signal_history.value,
                         self.parameters.monitor_signal_history.value,
                     ) = update_signal_history(
                         self.parameters.control_signal_history.value,
@@ -266,17 +271,19 @@
             self.parameters.task.value = autolock
             autolock.run(
                 x0,
                 x1,
                 spectrum,
                 should_watch_lock=start_watching,
                 auto_offset=auto_offset,
-                additional_spectra=pickle.loads(additional_spectra)
-                if additional_spectra is not None
-                else None,
+                additional_spectra=(
+                    pickle.loads(additional_spectra)
+                    if additional_spectra is not None
+                    else None
+                ),
             )
 
     def exposed_start_optimization(self, x0, x1, spectrum):
         if not self._task_running():
             optim = OptimizeSpectroscopy(self, self.parameters)
             self.parameters.task.value = optim
             optim.run(x0, x1, spectrum)
@@ -337,99 +344,73 @@
         """
         Directly sets a CSR register. This method is intended for debugging. Normally,
         the FPGA should be controlled via manipulation of parameters.
         """
         self.registers.set(key, value)
 
 
-class FakeRedPitayaControlService(BaseService):
+class FakeRedPitayaControlService(BaseService, LinienControlService):
     def __init__(self):
         super().__init__()
         self.exposed_is_locked = None
 
         self.random_data_thread = Thread(
             target=self._write_random_data_to_parameters_loop,
             args=(self.stop_event,),
             daemon=True,
         )
         self.random_data_thread.start()
 
     def _write_random_data_to_parameters_loop(self, stop_event: Event):
         while not stop_event.is_set():
             max_ = randint(0, 8191)
-            gen = lambda: np.array([randint(-max_, max_) for _ in range(N_POINTS)])
+
+            def gen():
+                return np.array([randint(-max_, max_) for _ in range(N_POINTS)])
+
             self.parameters.to_plot.value = pickle.dumps(
                 {
                     "error_signal_1": gen(),
                     "error_signal_1_quadrature": gen(),
                     "error_signal_2": gen(),
                     "error_signal_2_quadrature": gen(),
                 }
             )
             sleep(0.1)
 
     def exposed_write_registers(self):
         pass
 
     def exposed_start_autolock(self, x0, x1, spectrum):
-        logger.debug("start autolock %s %s" % (x0, x1))
+        logger.info(f"Start autolock {x0} {x1}")
 
     def exposed_start_optimization(self, x0, x1, spectrum):
-        logger.debug("start optimization")
+        logger.info("Start optimization")
         self.parameters.optimization_running.value = True
 
     def exposed_shutdown(self):
         raise SystemExit()
 
     def exposed_pause_acquisition(self):
         pass
 
     def exposed_continue_acquisition(self):
         pass
 
 
-# ignore type, otherwise "Argument 1 has incompatible type "Callable[[int, bool, str |
-# None, bool], Any]"; expected <nothing>" is raised for click 8.1.4.
-@click.command("linien-server")  # type: ignore[arg-type]
-@click.version_option(__version__)
-@click.argument("port", default=DEFAULT_SERVER_PORT, type=int, required=False)
-@click.option(
-    "--fake", is_flag=True, help="Runs a fake server that just returns random data"
-)
-@click.option(
-    "--host",
-    help=(
-        "Allows to run the server locally for development and connects to a RedPitaya. "
-        "Specify the RP's host as follows: --host=rp-f0xxxx.local"
-    ),
-)
-@click.option("--no-auth", is_flag=True, help="Disable authentication")
-def run_server(
-    port: int = DEFAULT_SERVER_PORT,
-    fake: bool = False,
-    host: Optional[str] = None,
-    no_auth: bool = False,
-):
-    logger.info("Start server on port %s" % port)
-
-    if fake:
-        logger.info("starting fake server")
-        control = FakeRedPitayaControlService()
+def run_threaded_server(
+    control: BaseService,
+    authenticator: Callable[[socket], tuple[socket, None]],
+) -> None:
+    """Run a (Fake)RedPitayaControlService in a threaded server."""
+    if isinstance(control, FakeRedPitayaControlService):
+        logger.info("Starting fake server")
     else:
-        control = RedPitayaControlService(host=host)
-
-    if no_auth or fake:
-        authenticator = no_authenticator
-    else:
-        authenticator = username_and_password_authenticator
+        logger.info("Starting server.")
 
     thread = ThreadedServer(
         control,
-        port=port,
+        port=SERVER_PORT,
         authenticator=authenticator,
-        protocol_config={"allow_pickle": True},
+        protocol_config={"allow_pickle": True, "allow_public_attrs": True},
     )
     thread.start()
-
-
-if __name__ == "__main__":
-    run_server()
```

### Comparing `linien-server-1.0.2rc1/linien_server.egg-info/SOURCES.txt` & `linien-server-2.0.0rc1/linien_server.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-setup.py
+pyproject.toml
 linien_server/__init__.py
 linien_server/acquisition.py
+linien_server/cli.py
 linien_server/csr.py
 linien_server/csrmap.py
-linien_server/gateware.bin
 linien_server/iir_coeffs.py
 linien_server/influxdb.py
-linien_server/linien_install_requirements.sh
-linien_server/linien_start_server.sh
-linien_server/linien_stop_server.sh
+linien_server/mdio_tool.py
 linien_server/noise_analysis.py
 linien_server/parameters.py
 linien_server/registers.py
 linien_server/server.py
 linien_server.egg-info/PKG-INFO
 linien_server.egg-info/SOURCES.txt
 linien_server.egg-info/dependency_links.txt
```

