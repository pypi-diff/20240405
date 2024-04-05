# Comparing `tmp/pyais-2.6.2.tar.gz` & `tmp/pyais-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyais-2.6.2.tar", last modified: Sat Mar 16 10:35:25 2024, max compression
+gzip compressed data, was "pyais-2.6.3.tar", last modified: Fri Apr  5 12:49:34 2024, max compression
```

## Comparing `pyais-2.6.2.tar` & `pyais-2.6.3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:35:25.752614 pyais-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-16 10:35:21.000000 pyais-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-03-16 10:35:25.752614 pyais-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-03-16 10:35:21.000000 pyais-2.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:35:25.748614 pyais-2.6.2/pyais/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-03-16 10:35:21.000000 pyais-2.6.2/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:35:25.752614 pyais-2.6.2/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-16 10:35:25.000000 pyais-2.6.2/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-16 10:35:21.000000 pyais-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 10:35:25.752614 pyais-2.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:35:25.752614 pyais-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-16 10:35:21.000000 pyais-2.6.2/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.083509 pyais-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 12:49:27.000000 pyais-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-04-05 12:49:34.083509 pyais-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-04-05 12:49:27.000000 pyais-2.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.075509 pyais-2.6.3/pyais/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-04-05 12:49:27.000000 pyais-2.6.3/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.083509 pyais-2.6.3/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 12:49:34.000000 pyais-2.6.3/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-05 12:49:27.000000 pyais-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:49:34.083509 pyais-2.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:49:34.079509 pyais-2.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-05 12:49:27.000000 pyais-2.6.3/tests/test_udp_stream.py
```

### Comparing `pyais-2.6.2/LICENSE` & `pyais-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/PKG-INFO` & `pyais-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.2
+Version: 2.6.3
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
```

### Comparing `pyais-2.6.2/README.md` & `pyais-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/__init__.py` & `pyais-2.6.3/pyais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyais.messages import NMEAMessage, ANY_MESSAGE, AISSentence
 from pyais.stream import TCPConnection, FileReaderStream, IterMessages
 from pyais.encode import encode_dict, encode_msg, ais_to_nmea_0183
 from pyais.decode import decode
 from pyais.tracker import AISTracker, AISTrack
 
 __license__ = 'MIT'
-__version__ = '2.6.2'
+__version__ = '2.6.3'
 __author__ = 'Leon Morten Richter'
 
 __all__ = (
     'encode_dict',
     'encode_msg',
     'ais_to_nmea_0183',
     'NMEAMessage',
```

### Comparing `pyais-2.6.2/pyais/ais_types.py` & `pyais-2.6.3/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/decode.py` & `pyais-2.6.3/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/encode.py` & `pyais-2.6.3/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/exceptions.py` & `pyais-2.6.3/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/filter.py` & `pyais-2.6.3/pyais/filter.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/main.py` & `pyais-2.6.3/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/messages.py` & `pyais-2.6.3/pyais/messages.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/stream.py` & `pyais-2.6.3/pyais/stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/tracker.py` & `pyais-2.6.3/pyais/tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/pyais/util.py` & `pyais-2.6.3/pyais/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import base64
+import math
 import typing
 from collections import OrderedDict
 from functools import partial, reduce
 from operator import xor
 from typing import Any, Generator, Hashable, TYPE_CHECKING, Union, Dict
 
 from bitarray import bitarray
 
-from pyais.constants import SyncState
+from pyais.constants import COUNTRY_MAPPING, SyncState
 from pyais.exceptions import NonPrintableCharacterException
 
 if TYPE_CHECKING:
     BaseDict = OrderedDict[Hashable, Any]
 else:
     BaseDict = OrderedDict
 
@@ -414,7 +415,18 @@
     return {
         'keep_flag': keep_flag,
         'sync_state': sync_state,
         'slot_increment': slot_increment,
         'num_slots': num_slots,
         'keep_flag': keep_flag,
     }
+
+
+def get_first_three_digits(num: int) -> int:
+    if num < 1000:
+        return num
+    digits = int(math.log10(num)) + 1
+    return int(num // (10**(digits - 3)))
+
+
+def get_country(mmsi: int) -> typing.Tuple[str, str]:
+    return COUNTRY_MAPPING.get(get_first_three_digits(mmsi), ('NA', 'Unknown'))
```

### Comparing `pyais-2.6.2/pyais.egg-info/PKG-INFO` & `pyais-2.6.3/pyais.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.6.2
+Version: 2.6.3
 Summary: AIS message decoding
 Author-email: Leon Morten Richter <misc@leonmortenrichter.de>
 Maintainer-email: Leon Morten Richter <misc@leonmortenrichter.de>
 License: MIT License
         
         Copyright (c) 2019 M0r13n
```

### Comparing `pyais-2.6.2/pyais.egg-info/SOURCES.txt` & `pyais-2.6.3/pyais.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 tests/test_constants.py
 tests/test_decode.py
 tests/test_decode_raw.py
 tests/test_encode.py
 tests/test_examples.py
 tests/test_file_stream.py
 tests/test_filters.py
+tests/test_flags.py
 tests/test_generic_stream.py
 tests/test_main.py
 tests/test_nmea.py
 tests/test_socket.py
 tests/test_tag_block.py
 tests/test_talker_ids.py
 tests/test_tcp_stream.py
```

### Comparing `pyais-2.6.2/pyproject.toml` & `pyais-2.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_constants.py` & `pyais-2.6.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_decode.py` & `pyais-2.6.3/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_decode_raw.py` & `pyais-2.6.3/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_encode.py` & `pyais-2.6.3/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_examples.py` & `pyais-2.6.3/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 assert subprocess.check_call(f'{exe} {file}'.split(), env=env, shell=False) == 0
 
         # Delete the file that was created by one of the tests
         csv_file = pathlib.Path("decoded_message.csv")
         if csv_file.exists():
             csv_file.unlink()
 
-        assert i == 18
+        assert i == 19
```

### Comparing `pyais-2.6.2/tests/test_file_stream.py` & `pyais-2.6.3/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_filters.py` & `pyais-2.6.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_generic_stream.py` & `pyais-2.6.3/tests/test_generic_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_main.py` & `pyais-2.6.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_nmea.py` & `pyais-2.6.3/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_socket.py` & `pyais-2.6.3/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_tag_block.py` & `pyais-2.6.3/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_talker_ids.py` & `pyais-2.6.3/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_tcp_stream.py` & `pyais-2.6.3/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_tracker.py` & `pyais-2.6.3/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.6.2/tests/test_udp_stream.py` & `pyais-2.6.3/tests/test_udp_stream.py`

 * *Files identical despite different names*

