# Comparing `tmp/ping3-4.0.6.tar.gz` & `tmp/ping3-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping3-4.0.6.tar", last modified: Wed Apr  3 14:13:53 2024, max compression
+gzip compressed data, was "ping3-4.0.7.tar", last modified: Fri Apr  5 13:01:54 2024, max compression
```

## Comparing `ping3-4.0.6.tar` & `ping3-4.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.161885 ping3-4.0.6/
--rw-rw-rw-   0        0        0     1092 2021-02-26 10:16:53.000000 ping3-4.0.6/LICENSE
--rw-rw-rw-   0        0        0    13111 2024-04-03 14:13:53.160885 ping3-4.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    10819 2022-12-15 11:51:14.000000 ping3-4.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.128230 ping3-4.0.6/ping3/
--rw-rw-rw-   0        0        0    18128 2024-04-03 14:04:55.000000 ping3-4.0.6/ping3/__init__.py
--rw-rw-rw-   0        0        0       83 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/__main__.py
--rw-rw-rw-   0        0        0     2592 2024-04-03 14:06:02.000000 ping3-4.0.6/ping3/command_line.py
--rw-rw-rw-   0        0        0     1342 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/enums.py
--rw-rw-rw-   0        0        0     1786 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.158889 ping3-4.0.6/ping3.egg-info/
--rw-rw-rw-   0        0        0    13111 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1357 2024-04-03 13:46:03.000000 ping3-4.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 14:13:53.161885 ping3-4.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.157886 ping3-4.0.6/tests/
--rw-rw-rw-   0        0        0      721 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_benchmark.py
--rw-rw-rw-   0        0        0     4537 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_command_line.py
--rw-rw-rw-   0        0        0      819 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_multi.py
--rw-rw-rw-   0        0        0     8253 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_ping3.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.582811 ping3-4.0.7/
+-rw-rw-rw-   0        0        0     1092 2021-02-26 10:16:53.000000 ping3-4.0.7/LICENSE
+-rw-rw-rw-   0        0        0    13111 2024-04-05 13:01:54.581804 ping3-4.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10819 2022-12-15 11:51:14.000000 ping3-4.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.528111 ping3-4.0.7/ping3/
+-rw-rw-rw-   0        0        0    18068 2024-04-05 12:54:31.000000 ping3-4.0.7/ping3/__init__.py
+-rw-rw-rw-   0        0        0       83 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/__main__.py
+-rw-rw-rw-   0        0        0     2587 2024-04-05 12:54:52.000000 ping3-4.0.7/ping3/command_line.py
+-rw-rw-rw-   0        0        0     1342 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/enums.py
+-rw-rw-rw-   0        0        0     1786 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.579741 ping3-4.0.7/ping3.egg-info/
+-rw-rw-rw-   0        0        0    13111 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2024-04-03 13:46:03.000000 ping3-4.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:01:54.582811 ping3-4.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.578740 ping3-4.0.7/tests/
+-rw-rw-rw-   0        0        0      721 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     4537 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_command_line.py
+-rw-rw-rw-   0        0        0      819 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_multi.py
+-rw-rw-rw-   0        0        0     8253 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_ping3.py
```

### Comparing `ping3-4.0.6/LICENSE` & `ping3-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/PKG-INFO` & `ping3-4.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ping3
-Version: 4.0.6
+Version: 4.0.7
 Summary: A pure python3 version of ICMP ping implementation using raw socket.
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ping3-4.0.6/README.md` & `ping3-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/ping3/__init__.py` & `ping3-4.0.7/ping3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import functools
 import errno
 
 from . import errors
 from .enums import ICMP_DEFAULT_CODE, IcmpType, IcmpTimeExceededCode, IcmpDestinationUnreachableCode
 
-__version__ = "4.0.6"
+__version__ = "4.0.7"
 DEBUG = False  # DEBUG: Show debug info for developers. (default False)
 EXCEPTIONS = False  # EXCEPTIONS: Raise exception when delay is not available.
 LOGGER = None  # LOGGER: Record logs into console or file. Logger object should have .debug() method.
 
 IP_HEADER_FORMAT = "!BBHHHBBHII"
 ICMP_HEADER_FORMAT = "!BBHHH"  # According to netinet/ip_icmp.h. !=network byte order(big-endian), B=unsigned char, H=unsigned short
 ICMP_TIME_FORMAT = "!d"  # d=double
@@ -173,15 +173,15 @@
     _debug("Sent ICMP header:", read_icmp_header(icmp_header))
     _debug("Sent ICMP payload:", icmp_payload)
     packet = icmp_header + icmp_payload
     sock.sendto(packet, (dest_addr, 0))  # addr = (ip, port). Port is 0 respectively the OS default behavior will be used.
 
 
 @_func_logger
-def receive_one_ping(sock: socket.socket, icmp_id: int, seq: int, timeout: int) -> float | None:
+def receive_one_ping(sock: socket.socket, icmp_id: int, seq: int, timeout: int):
     """Receives the ping from the socket.
 
     IP Header (bits): version (8), type of service (8), length (16), id (16), flags (16), time to live (8), protocol (8), checksum (16), source ip (32), destination ip (32).
     ICMP Packet (bytes): IP Header (20), ICMP Header (8), ICMP Payload (*).
     Ping Wikipedia: https://en.wikipedia.org/wiki/Ping_(networking_utility)
     ToS (Type of Service) in IP header for ICMP is 0. Protocol in IP header for ICMP is 1.
 
@@ -253,15 +253,15 @@
                 time_sent = struct.unpack(ICMP_TIME_FORMAT, icmp_payload_raw[0:struct.calcsize(ICMP_TIME_FORMAT)])[0]
                 _debug("Received sent time: {} ({})".format(time.ctime(time_sent), time_sent))
                 return time_recv - time_sent
         _debug("Uncatched ICMP packet:", icmp_header)
 
 
 @_func_logger
-def ping(dest_addr: str, timeout: int = 4, unit: str = "s", src_addr: str = "", ttl: int | None = None, seq: int = 0, size: int = 56, interface: str = "") -> float | None | bool:
+def ping(dest_addr: str, timeout: int = 4, unit: str = "s", src_addr: str = "", ttl= None, seq: int = 0, size: int = 56, interface: str = ""):
     """
     Send one ping to destination address with the given timeout.
 
     Args:
         dest_addr (str): The destination address, can be an IP address or a domain name. Ex. "192.168.1.1"/"example.com"
         timeout (int): Time to wait for a response, in seconds. Default is 4s, same as Windows CMD. (default 4)
         unit (str): The unit of returned value. "s" for seconds, "ms" for milliseconds. (default "s")
@@ -321,15 +321,15 @@
             return None
         if unit == "ms":
             delay *= 1000  # in milliseconds
         return delay
 
 
 @_func_logger
-def verbose_ping(dest_addr: str, count: int = 4, interval: float = 0, *args, **kwargs) -> None:
+def verbose_ping(dest_addr: str, count: int = 4, interval: float = 0, *args, **kwargs):
     """
     Send pings to destination address with the given timeout and display the result.
 
     Args:
         dest_addr (str): The destination address. Ex. "192.168.1.1"/"example.com"
         count (int): How many pings should be sent. 0 means infinite loops until manually stopped. Default is 4, same as Windows CMD. (default 4)
         interval (float): How many seconds between two packets. Default is 0, which means send the next packet as soon as the previous one responsed. (default 0)
```

### Comparing `ping3-4.0.6/ping3/command_line.py` & `ping3-4.0.7/ping3/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 
 import ping3
 
 
-def main(assigned_args: list[str] = []) -> None:
+def main(assigned_args: list = []) -> None:
     """
     Parse and execute the call from command-line.
 
     Args:
         assigned_args (list[str]): List of strings to parse. The default is taken from sys.argv.
 
     Returns:
```

### Comparing `ping3-4.0.6/ping3/enums.py` & `ping3-4.0.7/ping3/enums.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/ping3/errors.py` & `ping3-4.0.7/ping3/errors.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/ping3.egg-info/PKG-INFO` & `ping3-4.0.7/ping3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ping3
-Version: 4.0.6
+Version: 4.0.7
 Summary: A pure python3 version of ICMP ping implementation using raw socket.
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ping3-4.0.6/pyproject.toml` & `ping3-4.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/tests/test_benchmark.py` & `ping3-4.0.7/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/tests/test_command_line.py` & `ping3-4.0.7/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/tests/test_multi.py` & `ping3-4.0.7/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.6/tests/test_ping3.py` & `ping3-4.0.7/tests/test_ping3.py`

 * *Files identical despite different names*

