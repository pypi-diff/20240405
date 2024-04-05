# Comparing `tmp/FlaskFloodgate-1.0.tar.gz` & `tmp/FlaskFloodgate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlaskFloodgate-1.0.tar", last modified: Tue Mar 19 12:12:25 2024, max compression
+gzip compressed data, was "FlaskFloodgate-1.0.1.tar", last modified: Tue Mar 19 18:20:49 2024, max compression
```

## Comparing `FlaskFloodgate-1.0.tar` & `FlaskFloodgate-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:12:25.778927 FlaskFloodgate-1.0/
-drwxrwxrwx   0        0        0        0 2024-03-19 12:12:25.716045 FlaskFloodgate-1.0/FlaskFloodgate/
--rw-rw-rw-   0        0        0     3743 2024-03-19 11:49:02.000000 FlaskFloodgate-1.0/FlaskFloodgate/__init__.py
--rw-rw-rw-   0        0        0       92 2024-03-15 12:41:40.000000 FlaskFloodgate-1.0/FlaskFloodgate/exceptions.py
--rw-rw-rw-   0        0        0    24868 2024-03-19 11:53:56.000000 FlaskFloodgate-1.0/FlaskFloodgate/handlers.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:12:25.772895 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/
--rw-rw-rw-   0        0        0       59 2024-03-19 12:12:25.000000 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-03-19 12:12:25.000000 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:12:25.000000 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-19 12:12:25.000000 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-19 12:12:25.000000 FlaskFloodgate-1.0/FlaskFloodgate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       59 2024-03-19 12:12:25.775885 FlaskFloodgate-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-19 11:50:54.000000 FlaskFloodgate-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 12:12:25.780005 FlaskFloodgate-1.0/setup.cfg
--rw-rw-rw-   0        0        0      137 2024-03-19 12:12:10.000000 FlaskFloodgate-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 18:20:49.935311 FlaskFloodgate-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2024-03-19 12:26:36.000000 FlaskFloodgate-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4159 2024-03-19 18:20:49.932319 FlaskFloodgate-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3602 2024-03-19 13:21:33.000000 FlaskFloodgate-1.0.1/README.md
+-rw-rw-rw-   0        0        0      541 2024-03-19 18:20:26.000000 FlaskFloodgate-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-19 18:20:49.936308 FlaskFloodgate-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      137 2024-03-19 14:20:47.000000 FlaskFloodgate-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 18:20:49.875471 FlaskFloodgate-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-03-19 18:20:49.897414 FlaskFloodgate-1.0.1/src/FlaskFloodgate/
+-rw-rw-rw-   0        0        0     2189 2024-03-19 17:03:31.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-03-19 15:16:28.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate/exceptions.py
+-rw-rw-rw-   0        0        0    29104 2024-03-19 17:07:56.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate/handlers.py
+drwxrwxrwx   0        0        0        0 2024-03-19 18:20:49.929328 FlaskFloodgate-1.0.1/src/FlaskFloodgate.egg-info/
+-rw-rw-rw-   0        0        0     4159 2024-03-19 18:20:49.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-03-19 18:20:49.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 18:20:49.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-03-19 18:20:49.000000 FlaskFloodgate-1.0.1/src/FlaskFloodgate.egg-info/top_level.txt
```

### Comparing `FlaskFloodgate-1.0/FlaskFloodgate/handlers.py` & `FlaskFloodgate-1.0.1/src/FlaskFloodgate/handlers.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,133 +3,111 @@
 import json
 import sqlite3
 import logging
 
 from .exceptions import *
 
 from flask import Request
-from typing import Literal, Callable
+from typing import Literal, Callable, Union
 from threading import Thread
 from datetime import timedelta
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 
 __all__ = ["DBHandler", "MemoryHandler", "Sqlite3Handler"]
 
 class DBHandler(ABC):   
     """
     The storage handler for the rate-limit handler. You can create your own custom subclass and use it accordingly.
 
-    ### Default Handlers provided:
-        `RAMHandler`
+    Default Handlers provided
+    *************************
+        :clasS:`MemoryHandler`\n
+        :clasS:`Sqlite3Handler`
 
-    :TODO: Add support for `Sqlite3`.
+    :TODO: Add support for `JSON`.
     """
     @classmethod
     @abstractmethod
     def update_ip(self, ip: str):
         """
         Used to save / update data regarding an `IP`.
 
-        ## Parameters
-            ip: `str`
-                The IP to store / update data about.
-
-        ## Returns
-            `None`
-
-        ## Raises
-            `IPRateLimitExceeded`
-                Indicates that the IP has exceeded the specified rate limit.
+        :param ip: The IP to store / update data about.
+        :type ip: str
 
-            `IPBlackListed`
-                Indicates that the IP has been blacklisted for exceeding the specified block limit.
-
-            `NotImplementedError`
-                Indicates that the custom subclass has not implemented this method.
+        :raises IPRateLimitExceeded: Indicates that the IP has exceeded the specified rate limit.
+        :raises IPBlackListed: Indicates that the IP has been blacklisted for exceeding the specified block limit.
+        :raises NotImplementedError: Indicates that the custom subclass has not implemented this method.                
         """
         raise NotImplementedError("Custom subclass must implement `update_ip`.")
     
     @classmethod
     @abstractmethod
     def blacklist_ip(self, ip: str):
         """
         Used to blacklist an `IP`.
 
-        ## Parameters
-            ip: `str`
-                The IP to blacklist.
-
-        ## Returns
-            `None`
-
-        ## Raises
-            `NotImplementedError`
-                Indicates that the custom subclass has not implemented this method.
+        :param ip: The IP to blacklist.
+        :type ip: str
+
+        :raises NotImplementedError: Indicates that the custom subclass has not implemented this method.
         """
         raise NotImplementedError("Custom subclass must implement `blacklist_ip`.")
     
 class MemoryHandler(DBHandler):
     def __init__(
             self,
             amount: int,
             time_window: timedelta,
             block_limit: int = 5,
-            block_exceed_duration: timedelta | Literal["FOREVER"] = timedelta(days=1),
+            block_exceed_duration: Union[timedelta, Literal["FOREVER"]] = timedelta(days=1),
             relative_block: bool = True,
             block_exceed_reset: bool = True,
-            max_window_duration: timedelta = timedelta(days=1),
+            max_window_duration: Union[timedelta, Literal["FOREVER"]] = timedelta(days=1),
             accumulate_requests: bool = False,
             request_data_check: Callable[[Request], bool] = None,
             logger: logging.Logger = None,
-            export_dir: str | None = os.getcwd()
+            export_dir: Union[str, None] = 0
         ) -> None:
         """
         A custom subclass of `DBHandler`. Represents a `RAM / Memory` Handler for IP-related data.
 
-        ## Parameters
-            amount: `int`
-                The maximum amount of requests allowed for an IP in `time_window` time.
+        :param amount: The maximum amount of requests allowed for an IP in `time_window` time.
+        :type amount: int
 
-            time_window: `timedelta`
-                The time window in which the `amount` requests is allowed.
+        :param time_window: The time window in which the `amount` requests is allowed.
+        :type amount: :class:`datetime.timedelta`
 
-            block_limit: `int` = `5`
-                The number of times 
+        :param block_limit: The maximum number of times an IP can be blocked, defaults to `5`.
+        :type block_limit: int, optional
 
-            block_exceed_duration: `timedelta | Literal['FOREVER']` = `timedelta(days=1)`
-                The time duration for which the IP is blocked when it exceeds the specified `block_limit`.
-                If set to 'FOREVER', as the name implies, it will be blacklisted forever until specifically removed from the blacklist.
+        :param block_exceed_duration: The time duration for which the IP is blocked when it exceeds the specified `block_limit`. If set to 'FOREVER', as the name implies, it will be blacklisted forever until specifically removed from the blacklist, defaults to :class:`datetime.timedelta(days=1)`.
+        :type block_exceed_duration: Union[:class:`datetime.timedelta`, Literal['FOREVER']], optional
 
-            relative_block: `bool` = `True`
-                If set to `True`, the `block_exceed_duration` timer (if set to a `timedelta` object) will reset and start again everytime the IP sends a request during the ongoing `block_exceed_duration` timer.
-                If set to `False`, the `block_exceed_duration` timer (if set to a `timedelta` object) will not reset and start from the first ever blocked request for the window.
+        :param relative_block: If set to `True`, the `block_exceed_duration` timer (if set to a `timedelta` object) will reset and start again everytime the IP sends a request during the ongoing `block_exceed_duration` timer. If set to `False`, the `block_exceed_duration` timer (if set to a `timedelta` object) will not reset and start from the first ever blocked request for the window, defaults to `True`.
+        :type relative_block: bool, optional
 
-            block_exceed_reset: `bool` = `True`
-                If an IP exceeds the specified `block limit` and the `block_exceed_duration` is set to a `timedelta` object, then the IP will be blocked by `block_exceed_duration` everytime it exceeds the specified `amount` per specified `time_window`.
+        :param block_exceed_reset: If an IP exceeds the specified `block limit` and the `block_exceed_duration` is set to a `timedelta` object, then the IP will be blocked by `block_exceed_duration` everytime it exceeds the specified `amount` per specified `time_window`, defaults to `True`.
+        :type block_exceed_reset: bool, optional
 
-            max_window_duration: `timedelta` = `timedelta(days=1)`
-                The time duration in which a request window data is removed from the DB.
-                Does not include the Blacklist DB (if `block_exceed_duration` specified to 'FOREVER').
+        :param max_window_duration: The time duration in which a request window data is removed from the DB. (Does not include the Blacklist DB.) Defaults to :class:`datetime.timedelta(days=1)`.
+        :type max_window_duration: Union[:class:`datetime.timedelta`, Literal['FOREVER']], optional
 
-            accumulate_requests: `bool` = `False`
-                If set to `True`, it allows an IP to use the left-over amount of requests from the previous time-window along with the new one.
+        :param accumulate_requests: If set to `True`, it allows an IP to use the left-over amount of requests from the previous time-window along with the new one, defaults to `True`.
+        :type accumulate_requests: bool, optional
 
-            request_data_check: `Callable[[Request], bool]` = `None`
-                A function that takes in the `Flask request` as a positional argument and returns a `bool` indicating whether the IP is free from rate-limit checks.
-                If it returns `True`, the IP is excluded from rate-limit checks.
+        :param request_data_check: A function that takes in the `Flask request` as a positional argument and returns a `bool` indicating whether the IP is free from rate-limit checks. If it returns `True`, the IP is excluded from rate-limit checks, defaults to `None`.
+        :type request_data_check: Union[function, Callable[[Flask.Request], bool]], optional
 
-            logger: `logging.Loger` = `None`
-                The logger to use.
+        :param logger: The logger to use, defaults to `None`.
+        :type logger: :class:`logging.Logger`, optional
 
-            export_dir: `str | None` = `os.getcwd()`
-                The directory where the parameters will be exported to prevent data-loss in case of a server failure. If set to `None`, the parameters are not exported. 
-
-        ## Returns
-            `None`
+        :param export_dir: The directory where the parameters will be exported to prevent data-loss in case of a server failure. If set to `None`, the parameters are not exported, defaults to `0`.
+        :type export_dir: Union[str, None], optional
         """
         super().__init__()
         self._cache = {}
 
         self.amount = amount
         self.window = time_window.total_seconds()
         self.block_limit = block_limit
@@ -143,14 +121,17 @@
         self.blacklist = []
 
         if max_window_duration:
             self.mwd = round(max_window_duration.total_seconds())
             self.cleanup_thread = Thread(target=self.cleanup)
             self.cleanup_thread.start()
 
+        if export_dir == 0:
+            export_dir = os.getcwd()
+
         if not export_dir is None:
             expfp = os.path.join(export_dir, "Rate-Limit-Params.json")
             with open(expfp, "w") as f:
                 json.dump(
                     obj={
                         "amount": self.amount,
                         "window": self.window,
@@ -167,33 +148,26 @@
 
             print(f"The Rate-Limit Parameters have been exported to the following file:\n{expfp}\nTo load the parameters, use the `load_params` method. (The logger is not exported. You'll need to specify it again when loading the parameters.)")
 
     def load_params(export_fp: str = None, request_data_check: Callable[[Request], bool] = None, logger = None):
         """
         Used to load the previously exported parameters.
 
-        ## Parameters
-            export_fp: `str` = `None`
-                The path of the JSON file where the exported data was stored. If not specified, looks for `Rate-Limit-Params.json` in the current working dir.
-
-            request_data_check: `Callable[[Request], bool]` = `None`
-                The function to check validity of request. It needs to specified while loading the parameters it is not exported.
+        :param export_fp: The path of the JSON file where the exported data was stored. If not specified, looks for `Rate-Limit-Params.json` in the current working dir.
+        :type export_fp: str
                 
-            logger: `logging.Logger` = `None`
-                The logger to use needs to specified while loading the parameters as the logger is not exported.
-
-        ## Raises
-            `ValueError`
-                Indicates that there is something wrong with the `export_fp`.
+        :param request_data_check: The function to check validity of request. It needs to specified (if used earlier) while loading the parameters as it is not exported, defaults to `None`.
+        :type request_data_check: Union[function, Callable[[Flask.Request], bool]], optional
 
-            `json.JSONDecodeError`
-                Indicates that the file does not contain valid JSON data.
+        :param logger: The logger to use needs to specified (if used earlier) while loading the parameters as the logger is not exported, defaults to `None`.
+        :type logger: logging.Logger
 
-            `KeyError`
-                Indicates that the data stored in the file was invalid.
+        :raises ValueError: Indicates that there is something wrong with the `export_fp`.
+        :raises json.JSONDecodeError: Indicates that the `export_fp` does not contain valid JSON data.
+        :raises KeyError: Indicates that the data stored in the file was invalid.
         """
         if not export_fp:
             export_fp = os.path.join(os.getcwd(), "Rate-Limit-Params.json")
             if not os.path.exists(export_fp):
                 raise ValueError("`export_fp` parameter was not defined and the current working directory does not contain `Rate-Limit-Params.json`.")
             
         if not os.path.exists(export_fp):
@@ -213,29 +187,50 @@
             max_window_duration=data["mwd"],
             request_data_check=request_data_check,
             logger=logger,
             export_dir=None
         )
 
     def log_info(self, msg: str):
+        """
+        Used to log `INFO` level messages using the logger.
+        Helps prevent excess lines of checking if the logger is set or not.
+
+        :param msg: The message to log.
+        :type msg: str
+        """
         if self.logger:
             self.logger.info(msg)
 
     def cleanup(self):
+        """
+        The cleanup function that is run in a thread and cleans up `expired` request windows if the following inequality is true:\n
+        `request_window_init_time + max_window_duration < current_time`\n
+        Is only run if `max_window_duration != 'FOREVER'`.        
+        """
         while True:
             time.sleep(self.mwd)
             self.log_info(f"Cleaning up request windows.")
             crtime = time.time()
             ol = len(self._cache)
             self._cache = {
                 ip: data for ip, data in self._cache.items() if (data["last-window-request-limit"] + self.mwd) > crtime
             }
             self.log_info(f"({ol - len(self._cache)}) Request windows cleaned.")
 
     def update_ip(self, ip: str):
+        """
+        Used to save / update data regarding an `IP`.
+
+        :param ip: The IP to store / update data about.
+        :type ip: str
+
+        :raises IPRateLimitExceeded: Indicates that the IP has exceeded the specified rate limit.
+        :raises IPBlackListed: Indicates that the IP has been blacklisted for exceeding the specified block limit. 
+        """
         crtime = time.time()
 
         if ip in self.blacklist:
             self.log_info(f"IP - '{ip}' sent a request when it is already blacklisted.")
             raise IPBlackListed(f"IP - '{ip}' is already blacklisted for exceeding the `block_limit`.")
 
         if not ip in self._cache or self._cache[ip]["last-window-request-limit"] <= crtime:
@@ -276,83 +271,81 @@
             self._cache[ip] = ip_data
             self.log_info(f"IP - '{ip}' has been rate-limited.")
             raise IPRateLimitExceeded(f"IP - '{ip}' has been rate-limited. Please wait {round(ip_data['last-window-request-limit'] - crtime)}s.")
 
         self._cache[ip] = ip_data
 
     def blacklist_ip(self, ip: str):
+        """
+        Used to blacklist an `IP`.
+
+        :param ip: The IP to blacklist.
+        :type ip: str
+        """
         self._cache.pop(ip, None)
         self.blacklist.append(ip)
 
 class Sqlite3Handler(DBHandler):
     def __init__(
             self,
             fp: str,
             table_name: str,
             amount: int,
             time_window: timedelta,
             block_limit: int = 5,
-            block_exceed_duration: timedelta | Literal["FOREVER"] = timedelta(days=1),
+            block_exceed_duration: Union[timedelta, Literal["FOREVER"]] = timedelta(days=1),
             relative_block: bool = True,
             block_exceed_reset: bool = True,
-            max_window_duration: timedelta | Literal["FOREVER"] = timedelta(days=7),
+            max_window_duration: Union[timedelta, Literal["FOREVER"]] = timedelta(days=7),
             accumulate_requests: bool = False,
             request_data_check: Callable[[Request], bool] = None,
             logger: logging.Logger = None,
-            export_dir: str | None = os.getcwd()
+            export_dir: Union[str, None] = 0
         ) -> None:
         """
         A custom subclass of `DBHandler`. Represents an `Sqlite3` Handler for IP-related data.
 
-        ## Parameters
-            fp: `str`
-                The file-path of the Sqlite3 file.
+        :param fp: The file-path of the `.db` file.
+        :type fp: str
 
-            table_name: `str`
-                The name of the table.
+        :param table_name: The name of the table.
+        :type table_name: str
 
-            amount: `int`
-                The maximum amount of requests allowed for an IP in `time_window` time.
+        :param amount: The maximum amount of requests allowed for an IP in `time_window` time.
+        :type amount: int
 
-            time_window: `timedelta`
-                The time window in which the `amount` requests is allowed.
+        :param time_window: The time window in which the `amount` requests is allowed.
+        :type amount: :class:`datetime.timedelta`
 
-            block_limit: `int` = `5`
-                The number of times 
+        :param block_limit: The maximum number of times an IP can be blocked, defaults to `5`.
+        :type block_limit: int, optional
 
-            block_exceed_duration: `timedelta | Literal['FOREVER']` = `timedelta(days=1)`
-                The time duration for which the IP is blocked when it exceeds the specified `block_limit`.
-                If set to 'FOREVER', as the name implies, it will be blacklisted forever until specifically removed from the blacklist.
+        :param block_exceed_duration: The time duration for which the IP is blocked when it exceeds the specified `block_limit`. If set to 'FOREVER', as the name implies, it will be blacklisted forever until specifically removed from the blacklist, defaults to :class:`datetime.timedelta(days=1)`.
+        :type block_exceed_duration: Union[:class:`datetime.timedelta`, Literal['FOREVER']], optional
 
-            relative_block: `bool` = `True`
-                If set to `True`, the `block_exceed_duration` timer (if set to a `timedelta` object) will reset and start again everytime the IP sends a request during the ongoing `block_exceed_duration` timer.
-                If set to `False`, the `block_exceed_duration` timer (if set to a `timedelta` object) will not reset and start from the first ever blocked request for the window.
+        :param relative_block: If set to `True`, the `block_exceed_duration` timer (if set to a `timedelta` object) will reset and start again everytime the IP sends a request during the ongoing `block_exceed_duration` timer. If set to `False`, the `block_exceed_duration` timer (if set to a `timedelta` object) will not reset and start from the first ever blocked request for the window, defaults to `True`.
+        :type relative_block: bool, optional
 
-            block_exceed_reset: `bool` = `True`
-                If an IP exceeds the specified `block limit` and the `block_exceed_duration` is set to a `timedelta` object, then the IP will be blocked by `block_exceed_duration` everytime it exceeds the specified `amount` per specified `time_window`.
+        :param block_exceed_reset: If an IP exceeds the specified `block limit` and the `block_exceed_duration` is set to a `timedelta` object, then the IP will be blocked by `block_exceed_duration` everytime it exceeds the specified `amount` per specified `time_window`, defaults to `True`.
+        :type block_exceed_reset: bool, optional
 
-            max_window_duration: `timedelta | Literal['FOREVER']` = `timedelta(days=7)`
-                The time duration in which a request window data is removed from the DB. If set to 'FOREVER', the request windows will never be erased from the DB.
-                Does not include the Blacklist DB.
+        :param max_window_duration: The time duration in which a request window data is removed from the DB. (Does not include the Blacklist DB.) Defaults to :class:`datetime.timedelta(days=1)`.
+        :type max_window_duration: Union[:class:`datetime.timedelta`, Literal['FOREVER']], optional
 
-            accumulate_requests: `bool` = `False`
-                If set to `True`, it allows an IP to use the left-over amount of requests from the previous time-window along with the new one. 
-                
-            request_data_check: `Callable[[Request], bool]` = `None`
-                A function that takes in the `Flask request` as a positional argument and returns a `bool` indicating whether the IP is free from rate-limit checks.
-                If it returns `True`, the IP is excluded from rate-limit checks.
+        :param accumulate_requests: If set to `True`, it allows an IP to use the left-over amount of requests from the previous time-window along with the new one, defaults to `True`.
+        :type accumulate_requests: bool, optional
 
-            logger: `logging.logger` = `None`
-                The logger to use.
+        :param request_data_check: A function that takes in the `Flask request` as a positional argument and returns a `bool` indicating whether the IP is free from rate-limit checks. If it returns `True`, the IP is excluded from rate-limit checks, defaults to `None`.
+        :type request_data_check: Union[function, Callable[[Flask.Request], bool]], optional
 
-            export_dir: `str | None` = `os.getcwd()`
-                The directory where the parameters will be exported to prevent data-loss in case of a server failure. If set to `None`, the parameters are not exported. 
-            
-        ## Returns
-            `None`
+        :param logger: The logger to use, defaults to `None`.
+        :type logger: :class:`logging.Logger`, optional
+
+        :param export_dir: The directory where the parameters will be exported to prevent data-loss in case of a server failure. If set to `None`, the parameters are not exported, defaults to `0`.
+        :type export_dir: Union[str, None], optional
         """
         self._fp = fp
         self.table = table_name
 
         with self._connect() as (conn, cursor):
             cursor.execute(f"""
                 CREATE TABLE IF NOT EXISTS {self.table} (
@@ -383,14 +376,17 @@
             self.mwd = round(max_window_duration.total_seconds())
             self.cleanup_thread = Thread(target=self.cleanup)
             self.cleanup_thread.start()
 
         if not os.path.exists(export_dir):
             os.mkdir(export_dir)
 
+        if export_dir == 0:
+            export_dir = os.getcwd()
+
         if not export_dir is None:
             expfp = os.path.join(export_dir, "Rate-Limit-Params.json")
             with open(expfp, "w") as f:
                 json.dump(
                     obj={
                         "fp": self._fp,
                         "table": self.table,
@@ -409,33 +405,26 @@
 
             print(f"The Rate-Limit Parameters have been exported to the following file:\n{expfp}\nTo load the parameters, use the `load_params` method. (The logger is not exported. You'll need to specify it again when loading the parameters.)")
 
     def load_params(export_fp: str = None, request_data_check: Callable[[Request], bool] = None, logger = None):
         """
         Used to load the previously exported parameters.
 
-        ## Parameters
-            export_fp: `str` = `None`
-                The path of the JSON file where the exported data was stored. If not specified, looks for `Rate-Limit-Params.json` in the current working dir.
-
-            request_data_check: `Callable[[Request], bool]` = `None`
-                The function to check validity of request. It needs to specified while loading the parameters it is not exported.
-
-            logger: `logging.Logger` = `None`
-                The logger to use needs to specified while loading the parameters as the logger is not exported.
-
-        ## Raises
-            `ValueError`
-                Indicates that there is something wrong with the `export_fp`.
+        :param export_fp: The path of the JSON file where the exported data was stored. If not specified, looks for `Rate-Limit-Params.json` in the current working dir.
+        :type export_fp: str
+                
+        :param request_data_check: The function to check validity of request. It needs to specified (if used earlier) while loading the parameters as it is not exported, defaults to `None`.
+        :type request_data_check: Union[function, Callable[[Flask.Request], bool]], optional
 
-            `json.JSONDecodeError`
-                Indicates that the file does not contain valid JSON data.
+        :param logger: The logger to use needs to specified (if used earlier) while loading the parameters as the logger is not exported, defaults to `None`.
+        :type logger: logging.Logger
 
-            `KeyError`
-                Indicates that the data stored in the file was invalid.
+        :raises ValueError: Indicates that there is something wrong with the `export_fp`.
+        :raises json.JSONDecodeError: Indicates that the `export_fp` does not contain valid JSON data.
+        :raises KeyError: Indicates that the data stored in the file was invalid.
         """
         if not export_fp:
             export_fp = os.path.join(os.getcwd(), "Rate-Limit-Params.json")
             if not os.path.exists(export_fp):
                 raise ValueError("`export_fp` parameter was not defined and the current working directory does not contain `Rate-Limit-Params.json`.")
             
         if not os.path.exists(export_fp):
@@ -457,27 +446,48 @@
             max_window_duration=data["mwd"],
             request_data_check=request_data_check,
             logger=logger,
             export_dir=None
         )
 
     def log_info(self, msg: str):
+        """
+        Used to log `INFO` level messages using the logger.
+        Helps prevent excess lines of checking if the logger is set or not.
+
+        :param msg: The message to log.
+        :type msg: str
+        """
         if self.logger:
             self.logger.info(msg)
 
     def cleanup(self):
+        """
+        The cleanup function that is run in a thread and cleans up `expired` request windows if the following inequality is true:\n
+        `request_window_init_time + max_window_duration < current_time`\n
+        Is only run if `max_window_duration != 'FOREVER'`.
+        """
         while True:
             time.sleep(self.mwd)
             with self._connect() as (conn, cursor):
                 self.log_info(f"Cleaning up request windows.")
                 cursor.execute(f"DELETE FROM {self.table} WHERE last_window_request_limit <= ?", (round(time.time()) - self.mwd,))
                 conn.commit()
                 self.log_info(f"(?) Request windows cleaned.")
 
     def update_ip(self, ip: str):
+        """
+        Used to save / update data regarding an `IP`.
+
+        :param ip: The IP to store / update data about.
+        :type ip: str
+
+        :raises IPRateLimitExceeded: Indicates that the IP has exceeded the specified rate limit.
+        :raises IPBlackListed: Indicates that the IP has been blacklisted for exceeding the specified block limit. 
+        """
         crtime = time.time()
 
         with self._connect() as (conn, cursor):
             cursor.execute(f"SELECT * FROM {self.table}Blacklist WHERE ip = ?", (ip,))
             if cursor.fetchone():
                 self.log_info(f"IP - '{ip}' sent a request when it is already blacklisted.")
                 raise IPBlackListed(f"IP - '{ip}' is already blacklisted for exceeding the `block_limit`.")
@@ -526,41 +536,84 @@
                 
                 self.update_result(result, conn, cursor)
                 self.log_info(f"IP - '{ip}' has been rate-limited.")
                 raise IPRateLimitExceeded(f"IP - '{ip}' has been rate-limited. Please wait {round(result[2] - crtime)}s.")
 
             self.update_result(result, conn, cursor)
 
-    def update_result(self, data, conn, cursor):
+    def update_result(self, data: Union[list, tuple], conn: sqlite3.Connection, cursor: sqlite3.Cursor):
+        """
+        Used to `UPDATE` a result in the DB.
+        Helps prevent excess lines of code.
+
+        :param data: The data to insert by updating.
+        :type data: Union[list, tuple]
+
+        :param conn: The Sqlite3 Database connection.
+        :type conn: sqlite3.Connection
+
+        :param cursor: The Sqlite3 Database connection cursor.
+        :type cursor: sqlite3.Cursor
+        """
         cursor.execute(
             f"UPDATE {self.table} SET ip = ?, amount = ?, last_window_request_limit = ?, blocked = ?",
             (data[0], data[1], data[2], data[3])
         )
         conn.commit()
 
     def delete_ip(self, ip: str, conn: sqlite3.Connection = None, cursor: sqlite3.Cursor = None):
+        """
+        Used to remove an IP from the DB.
+
+        :param ip: The IP to remove.
+        :type ip: str
+
+        :param conn: The Sqlite3 Database connection, defaults to `None`.
+        :type conn: sqlite3.Connection, optional
+
+        :param cursor: The Sqlite3 Database connection cursor, defaults to `None`.
+        :type cursor: sqlite3.Cursor, optional
+        """
         if conn and cursor:
             cursor.execute(f"DELETE FROM {self.table} WHERE ip = ?", (ip,))
             conn.commit()
         else:
             with self._connect() as (conn, cursor):
                 cursor.execute(f"DELETE FROM {self.table} WHERE ip = ?", (ip,))
                 conn.commit()
 
     def blacklist_ip(self, ip: str, conn: sqlite3.Connection = None, cursor: sqlite3.Cursor = None):
+        """
+        Used to blacklist an `IP`.
+
+        :param ip: The IP to blacklist.
+        :type ip: str
+
+        :param conn: The Sqlite3 Database connection, defaults to `None`.
+        :type conn: sqlite3.Connection, optional
+
+        :param cursor: The Sqlite3 Database connection cursor, defaults to `None`.
+        :type cursor: sqlite3.Cursor, optional
+        """
         if conn and cursor:
             cursor.execute(f"INSERT INTO {self.table}Blacklist (ip) VALUES (?)", (ip,))
             conn.commit()
         else:
             with self._connect() as (conn, cursor):
                 cursor.execute(f"INSERT INTO {self.table}Blacklist (ip) VALUES (?)", (ip,))
                 conn.commit()
 
     @contextmanager
     def _connect(self):
+        """
+        A context manager for Sqlite3 Database Connections.
+
+        :return: A tuple object consisting of an Sqlite3 connection (at 0th index) and Sqlite3 connection cursor (at 1st index).
+        :rtype: tuple[sqlite3.Connection, sqlite3.Cursor]
+        """
         conn = sqlite3.connect(self._fp)
         cursor = conn.cursor()
         try:
             yield (conn, cursor)
         finally:
             cursor.close()
             conn.close()
```

