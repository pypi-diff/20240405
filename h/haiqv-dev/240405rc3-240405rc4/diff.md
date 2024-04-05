# Comparing `tmp/haiqv_dev-240405rc3-py3-none-any.whl.zip` & `tmp/haiqv_dev-240405rc4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 16085 bytes, number of entries: 31
+Zip file size: 16106 bytes, number of entries: 31
 -rw-rw-rw-  2.0 fat      110 b- defN 23-Oct-30 11:46 haiqv/.env
 -rw-rw-rw-  2.0 fat      865 b- defN 24-Apr-05 01:34 haiqv/__init__.py
--rw-rw-rw-  2.0 fat     8807 b- defN 24-Apr-05 14:30 haiqv/api.py
+-rw-rw-rw-  2.0 fat     8924 b- defN 24-Apr-05 14:37 haiqv/api.py
 -rw-rw-rw-  2.0 fat    11704 b- defN 24-Apr-05 02:37 haiqv/client.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Sep-11 06:53 haiqv/binding/__init__.py
 -rw-rw-rw-  2.0 fat     1152 b- defN 23-Sep-08 15:30 haiqv/binding/args_bind.py
 -rw-rw-rw-  2.0 fat     3107 b- defN 23-Sep-18 05:53 haiqv/binding/std_bind.py
 -rw-rw-rw-  2.0 fat      774 b- defN 23-Sep-08 15:40 haiqv/binding/yaml_bind.py
 -rw-rw-rw-  2.0 fat       34 b- defN 24-Feb-22 23:13 haiqv/common/__init__.py
 -rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-04 15:00 haiqv/common/keepalive.py
@@ -22,12 +22,12 @@
 -rw-rw-rw-  2.0 fat      208 b- defN 24-Apr-05 01:30 haiqv/store/log.py
 -rw-rw-rw-  2.0 fat     1661 b- defN 24-Feb-22 23:13 haiqv/store/notebook.py
 -rw-rw-rw-  2.0 fat     1078 b- defN 23-Oct-06 09:38 haiqv/store/run.py
 -rw-rw-rw-  2.0 fat      299 b- defN 24-Feb-22 23:13 haiqv/utils/__init__.py
 -rw-rw-rw-  2.0 fat      455 b- defN 23-Oct-06 14:32 haiqv/utils/common.py
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Oct-06 15:46 haiqv/utils/files.py
 -rw-rw-rw-  2.0 fat     1356 b- defN 24-Apr-05 01:30 haiqv/utils/log_config.py
--rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-05 14:31 haiqv_dev-240405rc3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 14:31 haiqv_dev-240405rc3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 14:31 haiqv_dev-240405rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2435 b- defN 24-Apr-05 14:31 haiqv_dev-240405rc3.dist-info/RECORD
-31 files, 40950 bytes uncompressed, 12209 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat      463 b- defN 24-Apr-05 14:39 haiqv_dev-240405rc4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 14:39 haiqv_dev-240405rc4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 14:39 haiqv_dev-240405rc4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2435 b- defN 24-Apr-05 14:39 haiqv_dev-240405rc4.dist-info/RECORD
+31 files, 41067 bytes uncompressed, 12230 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: haiqv/utils/files.py
 Comment: 
 
 Filename: haiqv/utils/log_config.py
 Comment: 
 
-Filename: haiqv_dev-240405rc3.dist-info/METADATA
+Filename: haiqv_dev-240405rc4.dist-info/METADATA
 Comment: 
 
-Filename: haiqv_dev-240405rc3.dist-info/WHEEL
+Filename: haiqv_dev-240405rc4.dist-info/WHEEL
 Comment: 
 
-Filename: haiqv_dev-240405rc3.dist-info/top_level.txt
+Filename: haiqv_dev-240405rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: haiqv_dev-240405rc3.dist-info/RECORD
+Filename: haiqv_dev-240405rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## haiqv/api.py

```diff
@@ -1,12 +1,13 @@
 import os
 import pkg_resources
 from importlib_metadata import distributions
 import __main__
 import signal
+import threading
 
 from typing import Any, Dict, Optional
 from datetime import datetime
 
 from .binding.args_bind import ArgBind
 from .binding.yaml_bind import YamlBind
 from .entities.run import Run
@@ -39,21 +40,27 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         status = 'Finished' if exc_type is None else 'Failed'
         finalize(status)
 
 
 def signal_handler(signum, frame):
-    if signum == signal.SIGINT:
-        finalize("Killed")
-        exit(1)
-
-    if signum == signal.SIGTERM:
-        finalize("Finished")
-        exit(0)
+    current_thread = threading.current_thread()
+    if current_thread is threading.main_thread():
+        if signum == signal.SIGINT:
+            finalize("Killed")
+            exit(1)
+
+        if signum == signal.SIGTERM:
+            finalize("Finished")
+            exit(0)
+
+
+signal.signal(signal.SIGTERM, signal_handler)
+signal.signal(signal.SIGINT, signal_handler)
 
 
 def _get_current_active_run() -> Optional[Run]:
     if RunStore.id() is None:
         return None
     return RunStore()
 
@@ -153,18 +160,14 @@
     global __active_run
     __active_run = run
 
     ka = KeepAliveTask()
     ka.set_fn(keepalive)
     ka.start(run_info.interval)
 
-    # main thread
-    signal.signal(signal.SIGTERM, signal_handler)
-    signal.signal(signal.SIGINT, signal_handler)
-
     return run
 
 
 def finalize(status: str = "Finished") -> None:
     bg = BackGroundTask()
     if bg is not None:
         bg.end_std_log()
```

## Comparing `haiqv_dev-240405rc3.dist-info/RECORD` & `haiqv_dev-240405rc4.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 haiqv/.env,sha256=bBm0oc8lfX2xFpIT9DwnsA0yWn9J2qcdZkuMTsx8o6Q,110
 haiqv/__init__.py,sha256=12wRk0tZxD85Sj4zWAAfUm4oHLs7MD5sxOi4FmxsoM8,865
-haiqv/api.py,sha256=vwBimHdp6jcH2DpG1knEI4Gzh8h2dpMPLO3WQAuBV_s,8807
+haiqv/api.py,sha256=py5kfAVuzq9grXYaZirjUy7D1ydRi7IUUFnV8G9K4DA,8924
 haiqv/client.py,sha256=cIX0_hFLtNy3TVSHQklIC1TYDF0G5_S5qIxikGqVv0k,11704
 haiqv/binding/__init__.py,sha256=WMCLDB06c6N2n9d23lYw0D9yvHgo4pZrXoluK8-KPiY,96
 haiqv/binding/args_bind.py,sha256=zJsSN7k9qZKCdYG14l6uqbjoVrIvSn2c72wWRZvG06Q,1152
 haiqv/binding/std_bind.py,sha256=jQd_AnKBiC2CmT8OQnZaQygodIkWKu91vmi620Di5wc,3107
 haiqv/binding/yaml_bind.py,sha256=384asQbh3Ij1eZTmmsxYVDpUAMO2RUJxVGj3GdLJpbk,774
 haiqv/common/__init__.py,sha256=sF9I5DcPYIHYPqRCyPdKCZedbbgUaHm8Bz50HY2hOi4,34
 haiqv/common/keepalive.py,sha256=53Pzi4J3Z7Z9eOukYGHAJDb8uQwqyb1M0iVCkJOvp0k,1123
@@ -21,11 +21,11 @@
 haiqv/store/log.py,sha256=rHSRA4DVwkmgLLT29n7QVYQOHYIp9jIkzqVzKiVkAGI,208
 haiqv/store/notebook.py,sha256=F-7worOcqfVK7tWfc401Abi7e88uQzy6gBipmRjk-yM,1661
 haiqv/store/run.py,sha256=j6WDspjJ9kN8l1iwXJ7oiSeU_7YWCmmn1JGFhoMbxLY,1078
 haiqv/utils/__init__.py,sha256=rjY9t2z9cSkEkDEsdAJh_B7MfSJ15UwhRTZgNAaBjK8,299
 haiqv/utils/common.py,sha256=Kb3Hg7LE1Gzkx7izxukThWUW39DN3ZVNN1p7yAAs8Jo,455
 haiqv/utils/files.py,sha256=lTjgWgQjPBn5tEYa8VZSPjgRnchSDycyX1M56euBwsM,1570
 haiqv/utils/log_config.py,sha256=iHX6PB3jQK7bkDJSbCSZbtOMJ0qyFV0VM7HDkuntYXw,1356
-haiqv_dev-240405rc3.dist-info/METADATA,sha256=pPL2oBAfCVuEufRFvKlkJoJX5OPL4XxDsaH2KqRJ7mk,463
-haiqv_dev-240405rc3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-haiqv_dev-240405rc3.dist-info/top_level.txt,sha256=52YfvrdtWlmTWTttjb58LZWM39jxBZivosJGgv7BqXg,6
-haiqv_dev-240405rc3.dist-info/RECORD,,
+haiqv_dev-240405rc4.dist-info/METADATA,sha256=dXW36sS5rFuWXU1LvnAZ48mDhD_sOjWoSsskcw9TmiI,463
+haiqv_dev-240405rc4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+haiqv_dev-240405rc4.dist-info/top_level.txt,sha256=52YfvrdtWlmTWTttjb58LZWM39jxBZivosJGgv7BqXg,6
+haiqv_dev-240405rc4.dist-info/RECORD,,
```

