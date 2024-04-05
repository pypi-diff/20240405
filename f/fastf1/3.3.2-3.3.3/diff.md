# Comparing `tmp/fastf1-3.3.2.tar.gz` & `tmp/fastf1-3.3.3.tar.gz`

## Comparing `fastf1-3.3.2.tar` & `fastf1-3.3.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/README.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/example_fastf1_signalrclient.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_annotate_corners.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_annotate_speed_trace.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_driver_laptimes.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_gear_shifts_on_track.py
--rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_laptimes_distribution.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_position_changes.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_qualifying_results.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_results_tracker.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_speed_on_track.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_speed_traces.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_strategy.py
--rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_team_pace_ranking.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.2/examples/plot_who_can_still_win_wdc.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/__init__.py
--rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/_api.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/_version.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/api.py
--rw-r--r--   0        0        0   153144 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/core.py
--rw-r--r--   0        0        0    38660 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/events.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/legacy.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/logger.py
--rw-r--r--   0        0        0    16303 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/plotting.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/req.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/utils.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/ergast/__init__.py
--rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/ergast/interface.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/ergast/legacy.py
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/ergast/sphinx.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/ergast/structure.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/internals/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/internals/pandas_base.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/internals/pandas_extensions.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/livetiming/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/livetiming/__main__.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/livetiming/client.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/livetiming/data.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/mvapi/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/mvapi/api.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/mvapi/data.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/mvapi/internals.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/_connection.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/events/_events.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/hubs/_hub.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.2/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastf1-3.3.2/requirements/dev.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.2/requirements/minver.txt
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.2/LICENSE
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.2/README.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/README.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/example_fastf1_signalrclient.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_annotate_corners.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_annotate_speed_trace.py
+-rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_driver_laptimes.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_gear_shifts_on_track.py
+-rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_laptimes_distribution.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_position_changes.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_qualifying_results.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_results_tracker.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_speed_on_track.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_speed_traces.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_strategy.py
+-rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_team_pace_ranking.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.3/examples/plot_who_can_still_win_wdc.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/__init__.py
+-rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/_api.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/_version.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/api.py
+-rw-r--r--   0        0        0   153144 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/core.py
+-rw-r--r--   0        0        0    38660 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/events.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/legacy.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/logger.py
+-rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/plotting.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/req.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/utils.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/__init__.py
+-rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/interface.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/legacy.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/sphinx.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/ergast/structure.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/pandas_base.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/internals/pandas_extensions.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/__main__.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/client.py
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/livetiming/data.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/api.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/data.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/mvapi/internals.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/events/_events.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/hubs/_hub.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.3/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastf1-3.3.3/requirements/dev.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.3/requirements/minver.txt
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.3/LICENSE
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.3/README.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.3/PKG-INFO
```

### Comparing `fastf1-3.3.2/examples/plot_annotate_corners.py` & `fastf1-3.3.3/examples/plot_annotate_corners.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_annotate_speed_trace.py` & `fastf1-3.3.3/examples/plot_annotate_speed_trace.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_driver_laptimes.py` & `fastf1-3.3.3/examples/plot_driver_laptimes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_gear_shifts_on_track.py` & `fastf1-3.3.3/examples/plot_gear_shifts_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_laptimes_distribution.py` & `fastf1-3.3.3/examples/plot_laptimes_distribution.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_position_changes.py` & `fastf1-3.3.3/examples/plot_position_changes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_qualifying_results.py` & `fastf1-3.3.3/examples/plot_qualifying_results.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_results_tracker.py` & `fastf1-3.3.3/examples/plot_results_tracker.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_speed_on_track.py` & `fastf1-3.3.3/examples/plot_speed_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_speed_traces.py` & `fastf1-3.3.3/examples/plot_speed_traces.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_strategy.py` & `fastf1-3.3.3/examples/plot_strategy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_team_pace_ranking.py` & `fastf1-3.3.3/examples/plot_team_pace_ranking.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/examples/plot_who_can_still_win_wdc.py` & `fastf1-3.3.3/examples/plot_who_can_still_win_wdc.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/__init__.py` & `fastf1-3.3.3/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/_api.py` & `fastf1-3.3.3/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/api.py` & `fastf1-3.3.3/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/core.py` & `fastf1-3.3.3/fastf1/core.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/events.py` & `fastf1-3.3.3/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/legacy.py` & `fastf1-3.3.3/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/logger.py` & `fastf1-3.3.3/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/plotting.py` & `fastf1-3.3.3/fastf1/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     "theo pourchaire": "#004601",
 
     "nyck de vries": "#1e3d61",
     "yuki tsunoda": "#356cac",
     "daniel ricciardo": "#2b4562",
     "liam lawson": "#2b4562",
     "isack hadjar": "#1e6176",
+    "ayumu iwasa": "#1e6176",
 
     "pierre gasly": "#fe86bc",
     "esteban ocon": "#ff117c",
     "jack doohan": "#894667",
 
     "fernando alonso": "#006f62",
     "lance stroll": "#00413b",
@@ -156,15 +157,15 @@
     'OWA': 'pato oward',
     'GAS': 'pierre gasly', 'OCO': 'esteban ocon',
     'DOO': 'jack doohan',
     'BOT': 'valtteri bottas', 'ZHO': 'zhou guanyu',
     'POU': 'theo pourchaire',
     'DEV': 'nyck de vries', 'TSU': 'yuki tsunoda',
     'RIC': 'daniel ricciardo', 'LAW': 'liam lawson',
-    'HAD': 'isack hadjar',
+    'HAD': 'isack hadjar', 'IWA': 'ayumu iwasa',
     'MAG': 'kevin magnussen', 'HUL': 'nico hulkenberg',
     'BEA': 'oliver bearman',
     'ALO': 'fernando alonso', 'STR': 'lance stroll',
     'DRU': 'felipe drugovich',
     'HAM': 'lewis hamilton', 'RUS': 'george russell',
     'VES': 'frederik vesti',
     'ALB': 'alexander albon', 'SAR': 'logan sargeant',
```

### Comparing `fastf1-3.3.2/fastf1/req.py` & `fastf1-3.3.3/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/utils.py` & `fastf1-3.3.3/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/ergast/interface.py` & `fastf1-3.3.3/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/ergast/legacy.py` & `fastf1-3.3.3/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/ergast/sphinx.py` & `fastf1-3.3.3/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/ergast/structure.py` & `fastf1-3.3.3/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/internals/pandas_base.py` & `fastf1-3.3.3/fastf1/internals/pandas_base.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/internals/pandas_extensions.py` & `fastf1-3.3.3/fastf1/internals/pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/livetiming/__init__.py` & `fastf1-3.3.3/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/livetiming/__main__.py` & `fastf1-3.3.3/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/livetiming/client.py` & `fastf1-3.3.3/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/livetiming/data.py` & `fastf1-3.3.3/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/mvapi/api.py` & `fastf1-3.3.3/fastf1/mvapi/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/mvapi/data.py` & `fastf1-3.3.3/fastf1/mvapi/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/signalr_aio/LICENSE` & `fastf1-3.3.3/fastf1/signalr_aio/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/signalr_aio/_connection.py` & `fastf1-3.3.3/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.3.3/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.3.3/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.3.3/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/.gitignore` & `fastf1-3.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/LICENSE` & `fastf1-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/README.md` & `fastf1-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/pyproject.toml` & `fastf1-3.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.2/PKG-INFO` & `fastf1-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastf1
-Version: 3.3.2
+Version: 3.3.3
 Summary: Python package for accessing and analyzing Formula 1 results, schedules, timing data and telemetry.
 Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev
 Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: fastf1 Version: 3.3.2 Summary: Python package for
+Metadata-Version: 2.3 Name: fastf1 Version: 3.3.3 Summary: Python package for
 accessing and analyzing Formula 1 results, schedules, timing data and
 telemetry. Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org License: MIT License Copyright (c) 2024
 Philipp SchÃ¤fer Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
```

