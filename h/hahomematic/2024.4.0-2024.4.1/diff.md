# Comparing `tmp/hahomematic-2024.4.0.tar.gz` & `tmp/hahomematic-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.0.tar", last modified: Tue Apr  2 11:59:55 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.1.tar", last modified: Fri Apr  5 15:41:05 2024, max compression
```

## Comparing `hahomematic-2024.4.0.tar` & `hahomematic-2024.4.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.678846 hahomematic-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-02 11:59:55.678846 hahomematic-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.662846 hahomematic-2024.4.0/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.666846 hahomematic-2024.4.0/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27481 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.666846 hahomematic-2024.4.0/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.666846 hahomematic-2024.4.0/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.666846 hahomematic-2024.4.0/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.670846 hahomematic-2024.4.0/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33114 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    29499 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.670846 hahomematic-2024.4.0/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.674846 hahomematic-2024.4.0/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.674846 hahomematic-2024.4.0/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.678846 hahomematic-2024.4.0/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 11:59:55.000000 hahomematic-2024.4.0/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.674846 hahomematic-2024.4.0/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 11:59:55.678846 hahomematic-2024.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:59:55.678846 hahomematic-2024.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26200 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31933 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-02 11:59:28.000000 hahomematic-2024.4.0/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.044359 hahomematic-2024.4.1/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27481 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    56972 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.048359 hahomematic-2024.4.1/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33118 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.052359 hahomematic-2024.4.1/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:41:04.000000 hahomematic-2024.4.1/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 15:41:05.000000 hahomematic-2024.4.1/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 15:41:05.060360 hahomematic-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:41:05.056359 hahomematic-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26290 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31933 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-05 15:40:42.000000 hahomematic-2024.4.1/tests/test_text.py
```

### Comparing `hahomematic-2024.4.0/LICENSE` & `hahomematic-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/PKG-INFO` & `hahomematic-2024.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.0/README.md` & `hahomematic-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/__init__.py` & `hahomematic-2024.4.1/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.1/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/caches/persistent.py` & `hahomematic-2024.4.1/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/caches/visibility.py` & `hahomematic-2024.4.1/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/central/__init__.py` & `hahomematic-2024.4.1/hahomematic/central/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,30 +257,30 @@
         """Add new program button."""
         if (ccu_var_name := sysvar_entity.ccu_var_name) is not None:
             self._sysvar_entities[ccu_var_name] = sysvar_entity
 
     def remove_sysvar_entity(self, name: str) -> None:
         """Remove a sysvar entity."""
         if (sysvar_entity := self.get_sysvar_entity(name=name)) is not None:
-            sysvar_entity.fire_remove_entity_callback()
+            sysvar_entity.fire_entity_removed_callback()
             del self._sysvar_entities[name]
 
     @property
     def program_buttons(self) -> tuple[HmProgramButton, ...]:
         """Return the program entities."""
         return tuple(self._program_buttons.values())
 
     def add_program_button(self, program_button: HmProgramButton) -> None:
         """Add new program button."""
         self._program_buttons[program_button.pid] = program_button
 
     def remove_program_button(self, pid: str) -> None:
         """Remove a program button."""
         if (program_button := self.get_program_button(pid=pid)) is not None:
-            program_button.fire_remove_entity_callback()
+            program_button.fire_entity_removed_callback()
             del self._program_buttons[pid]
 
     @property
     def version(self) -> str | None:
         """Return the version of the backend."""
         if self._version is None:
             versions = [client.version for client in self._clients.values() if client.version]
```

### Comparing `hahomematic-2024.4.0/hahomematic/central/decorators.py` & `hahomematic-2024.4.1/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.1/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/client/__init__.py` & `hahomematic-2024.4.1/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.1/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.1/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/config.py` & `hahomematic-2024.4.1/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/const.py` & `hahomematic-2024.4.1/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/exceptions.py` & `hahomematic-2024.4.1/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/hmcli.py` & `hahomematic-2024.4.1/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/performance.py` & `hahomematic-2024.4.1/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.1/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             return EntityUsage.CE_SECONDARY
         return EntityUsage.CE_PRIMARY
 
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity values."""
         for entity in self._readable_entities:
             await entity.load_entity_value(call_source=call_source, direct_call=direct_call)
-        self.fire_update_entity_callback()
+        self.fire_entity_updated_callback()
 
     def is_state_change(self, **kwargs: Any) -> bool:
         """
         Check if the state changes due to kwargs.
 
         If the state is uncertain, the state should also marked as changed.
         """
@@ -225,23 +225,29 @@
             return
         self.device.add_sub_device_channel(
             channel_no=self._channel_no, base_channel_no=self._base_channel_no
         )
         if is_visible:
             entity.set_usage(EntityUsage.CE_VISIBLE)
 
-        entity.register_internal_update_callback(update_callback=self.fire_update_entity_callback)
+        entity.register_internal_entity_updated_callback(
+            entity_updated_callback=self.fire_entity_updated_callback
+        )
         self._data_entities[field] = entity
 
-    def unregister_update_callback(self, update_callback: Callable, custom_id: str) -> None:
+    def unregister_entity_updated_callback(
+        self, entity_updated_callback: Callable, custom_id: str
+    ) -> None:
         """Unregister update callback."""
         for entity in self._data_entities.values():
-            entity.unregister_internal_update_callback(update_callback=update_callback)
+            entity.unregister_internal_update_callback(update_callback=entity_updated_callback)
 
-        super().unregister_update_callback(update_callback=update_callback, custom_id=custom_id)
+        super().unregister_entity_updated_callback(
+            entity_updated_callback=entity_updated_callback, custom_id=custom_id
+        )
 
     def _mark_entities(self, entity_def: Mapping[int | tuple[int, ...], tuple[str, ...]]) -> None:
         """Mark entities to be created in HA."""
         if not entity_def:
             return
         for channel_nos, parameters in entity_def.items():
             if isinstance(channel_nos, int):
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.1/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.1/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/device.py` & `hahomematic-2024.4.1/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,32 +346,32 @@
 
     def add_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
         if isinstance(entity, BaseEntity):
             self.central.add_event_subscription(entity=entity)
         if isinstance(entity, GenericEntity):
             self._generic_entities[(entity.channel_address, entity.parameter)] = entity
-            self.register_update_callback(update_callback=entity.fire_update_entity_callback)
+            self.register_update_callback(update_callback=entity.fire_entity_updated_callback)
         if isinstance(entity, hmce.CustomEntity):
             self._custom_entities[entity.channel_no] = entity
         if isinstance(entity, GenericEvent):
             self._generic_events[(entity.channel_address, entity.parameter)] = entity
 
     def remove_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
         if isinstance(entity, BaseEntity):
             self.central.remove_event_subscription(entity=entity)
         if isinstance(entity, GenericEntity):
             del self._generic_entities[(entity.channel_address, entity.parameter)]
-            self.unregister_update_callback(update_callback=entity.fire_update_entity_callback)
+            self.unregister_update_callback(update_callback=entity.fire_entity_updated_callback)
         if isinstance(entity, hmce.CustomEntity):
             del self._custom_entities[entity.channel_no]
         if isinstance(entity, GenericEvent):
             del self._generic_events[(entity.channel_address, entity.parameter)]
-        entity.fire_remove_entity_callback()
+        entity.fire_entity_removed_callback()
 
     def clear_collections(self) -> None:
         """Remove entities from collections and central."""
         for event in self.generic_events:
             self.remove_entity(event)
         self._generic_events.clear()
 
@@ -492,15 +492,15 @@
         )
 
     def set_forced_availability(self, forced_availability: ForcedDeviceAvailability) -> None:
         """Set the availability of the device."""
         if self._forced_availability != forced_availability:
             self._forced_availability = forced_availability
             for entity in self.generic_entities:
-                entity.fire_update_entity_callback()
+                entity.fire_entity_updated_callback()
 
     async def export_device_definition(self) -> None:
         """Export the device definition for current device."""
         device_exporter = _DefinitionExporter(device=self)
         await device_exporter.export_data()
 
     def refresh_firmware_data(self) -> None:
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/entity.py` & `hahomematic-2024.4.1/hahomematic/platforms/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,17 +103,17 @@
 
     _platform: HmPlatform
 
     def __init__(self, central: hmcu.CentralUnit, unique_id: str) -> None:
         """Init the callback entity."""
         self._central: Final = central
         self._unique_id: Final = unique_id
-        self._update_callbacks: dict[Callable, str] = {}
-        self._refresh_callbacks: dict[Callable, str] = {}
-        self._remove_callbacks: list[Callable] = []
+        self._entity_updated_callbacks: dict[Callable, str] = {}
+        self._entity_refreshed_callbacks: dict[Callable, str] = {}
+        self._entity_removed_callbacks: list[Callable] = []
         self._custom_id: str | None = None
 
     @property
     @abstractmethod
     def available(self) -> bool:
         """Return the availability of the device."""
 
@@ -167,93 +167,108 @@
         )
 
     @property
     def is_registered(self) -> bool:
         """Return if entity is registered externally."""
         return self._custom_id is not None
 
-    def register_internal_update_callback(self, update_callback: Callable) -> None:
-        """Register internal update callback."""
-        self.register_update_callback(update_callback=update_callback, custom_id=DEFAULT_CUSTOM_ID)
-
-    def register_update_callback(self, update_callback: Callable, custom_id: str) -> None:
-        """Register update callback."""
-        if callable(update_callback):
-            self._update_callbacks[update_callback] = custom_id
+    def register_internal_entity_updated_callback(self, entity_updated_callback: Callable) -> None:
+        """Register internal entity updated callback."""
+        self.register_entity_updated_callback(
+            entity_updated_callback=entity_updated_callback, custom_id=DEFAULT_CUSTOM_ID
+        )
+
+    def register_entity_updated_callback(
+        self, entity_updated_callback: Callable, custom_id: str
+    ) -> None:
+        """Register entity updated callback."""
+        if callable(entity_updated_callback):
+            self._entity_updated_callbacks[entity_updated_callback] = custom_id
         if custom_id != DEFAULT_CUSTOM_ID:
-            if self._custom_id is not None:
+            if self._custom_id is not None and self._custom_id != custom_id:
                 raise HaHomematicException(
-                    f"REGISTER_UPDATE_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
+                    f"REGISTER_ENTITY_UPDATED_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
     def unregister_internal_update_callback(self, update_callback: Callable) -> None:
-        """Unregister update callback."""
-        self.unregister_update_callback(
-            update_callback=update_callback, custom_id=DEFAULT_CUSTOM_ID
+        """Unregister entity updated callback."""
+        self.unregister_entity_updated_callback(
+            entity_updated_callback=update_callback, custom_id=DEFAULT_CUSTOM_ID
         )
 
-    def unregister_update_callback(self, update_callback: Callable, custom_id: str) -> None:
-        """Unregister update callback."""
-        if update_callback in self._update_callbacks:
-            del self._update_callbacks[update_callback]
+    def unregister_entity_updated_callback(
+        self, entity_updated_callback: Callable, custom_id: str
+    ) -> None:
+        """Unregister entity updated callback."""
+        if entity_updated_callback in self._entity_updated_callbacks:
+            del self._entity_updated_callbacks[entity_updated_callback]
         if self.custom_id == custom_id:
             self._custom_id = None
 
-    def register_refresh_callback(self, refresh_callback: Callable, custom_id: str) -> None:
-        """Register update callback."""
-        if callable(refresh_callback):
-            self._refresh_callbacks[refresh_callback] = custom_id
+    def register_entity_refreshed_callback(
+        self, entity_refreshed_callback: Callable, custom_id: str
+    ) -> None:
+        """Register entity updated callback."""
+        if callable(entity_refreshed_callback):
+            self._entity_refreshed_callbacks[entity_refreshed_callback] = custom_id
         if custom_id != DEFAULT_CUSTOM_ID:
-            if self._custom_id is not None:
+            if self._custom_id is not None and self._custom_id != custom_id:
                 raise HaHomematicException(
-                    f"REGISTER_REFRESH_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
+                    f"REGISTER_ENTITY_REFRESHED_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
-    def unregister_refresh_callback(self, refresh_callback: Callable, custom_id: str) -> None:
-        """Unregister update callback."""
-        if refresh_callback in self._refresh_callbacks:
-            del self._refresh_callbacks[refresh_callback]
+    def unregister_entity_refreshed_callback(
+        self, entity_refreshed_callback: Callable, custom_id: str
+    ) -> None:
+        """Unregister entity updated callback."""
+        if entity_refreshed_callback in self._entity_refreshed_callbacks:
+            del self._entity_refreshed_callbacks[entity_refreshed_callback]
         if self.custom_id == custom_id:
             self._custom_id = None
 
-    def register_remove_callback(self, remove_callback: Callable) -> None:
-        """Register the remove callback."""
-        if callable(remove_callback) and remove_callback not in self._remove_callbacks:
-            self._remove_callbacks.append(remove_callback)
-
-    def unregister_remove_callback(self, remove_callback: Callable) -> None:
-        """Unregister the remove callback."""
-        if remove_callback in self._remove_callbacks:
-            self._remove_callbacks.remove(remove_callback)
+    def register_entity_removed_callback(self, entity_removed_callback: Callable) -> None:
+        """Register the entity removed callback."""
+        if (
+            callable(entity_removed_callback)
+            and entity_removed_callback not in self._entity_removed_callbacks
+        ):
+            self._entity_removed_callbacks.append(entity_removed_callback)
+
+    def unregister_entity_removed_callback(self, entity_removed_callback: Callable) -> None:
+        """Unregister the entity removed callback."""
+        if entity_removed_callback in self._entity_removed_callbacks:
+            self._entity_removed_callbacks.remove(entity_removed_callback)
 
-    def fire_update_entity_callback(self, *args: Any, **kwargs: Any) -> None:
+    def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated."""
-        for _callback in self._update_callbacks:
+        for _callback in self._entity_updated_callbacks:
             try:
                 _callback(*args, **kwargs)
             except Exception as ex:
-                _LOGGER.warning("FIRE_UPDATE_ENTITY_EVENT failed: %s", reduce_args(args=ex.args))
+                _LOGGER.warning("FIRE_ENTITY_UPDATED_EVENT failed: %s", reduce_args(args=ex.args))
 
-    def fire_refresh_entity_callback(self, *args: Any, **kwargs: Any) -> None:
+    def fire_entity_refreshed_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been refreshed."""
-        for _callback in self._refresh_callbacks:
+        for _callback in self._entity_refreshed_callbacks:
             try:
                 _callback(*args, **kwargs)
             except Exception as ex:
-                _LOGGER.warning("FIRE_REFRESH_ENTITY_EVENT failed: %s", reduce_args(args=ex.args))
+                _LOGGER.warning(
+                    "FIRE_ENTITY_REFRESHED_EVENT failed: %s", reduce_args(args=ex.args)
+                )
 
-    def fire_remove_entity_callback(self, *args: Any) -> None:
+    def fire_entity_removed_callback(self, *args: Any) -> None:
         """Do what is needed when the entity has been removed."""
-        for _callback in self._remove_callbacks:
+        for _callback in self._entity_removed_callbacks:
             try:
                 _callback(*args)
             except Exception as ex:
-                _LOGGER.warning("FIRE_REMOVE_ENTITY_EVENT failed: %s", reduce_args(args=ex.args))
+                _LOGGER.warning("FIRE_ENTITY_REMOVED_EVENT failed: %s", reduce_args(args=ex.args))
 
 
 class BaseEntity(CallbackEntity, PayloadMixin):
     """Base class for regular entities."""
 
     def __init__(
         self,
@@ -365,17 +380,17 @@
         """Return the entity usage."""
         return self._usage
 
     def set_usage(self, usage: EntityUsage) -> None:
         """Set the entity usage."""
         self._usage = usage
 
-    def fire_update_entity_callback(self, *args: Any, **kwargs: Any) -> None:
+    def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated."""
-        super().fire_update_entity_callback(*args, **kwargs)
+        super().fire_entity_updated_callback(*args, **kwargs)
         self._central.fire_entity_data_event_callback(
             interface_id=self._device.interface_id, entity=self
         )
 
     @abstractmethod
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity data."""
@@ -675,28 +690,28 @@
 
     def write_value(self, value: Any) -> tuple[ParameterT | None, ParameterT | None]:
         """Update value of the entity."""
         old_value = self._value
         if value == NO_CACHE_ENTRY:
             if self.last_refreshed != INIT_DATETIME:
                 self._state_uncertain = True
-                self.fire_update_entity_callback()
+                self.fire_entity_updated_callback()
             return (old_value, None)
 
         new_value = self._convert_value(value)
         if old_value == new_value:
             self._set_last_refreshed()
-            self.fire_refresh_entity_callback()
+            self.fire_entity_refreshed_callback()
             return (old_value, new_value)
 
         self._old_value = old_value
         self._value = new_value
         self._state_uncertain = False
         self._set_last_updated()
-        self.fire_update_entity_callback()
+        self.fire_entity_updated_callback()
         return (old_value, new_value)
 
     def update_parameter_data(self) -> None:
         """Update parameter data."""
         self._assign_parameter_data(
             parameter_data=self._central.paramset_descriptions.get_parameter_data(
                 interface_id=self._device.interface_id,
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/event.py` & `hahomematic-2024.4.1/hahomematic/platforms/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def event_type(self) -> EventType:
         """Return the event_type of the event."""
         return self._event_type
 
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
         if self.event_type in ENTITY_EVENTS:
-            self.fire_update_entity_callback(parameter=self.parameter.lower())
+            self.fire_entity_updated_callback(parameter=self.parameter.lower())
         self.fire_event(value)
 
     def fire_event(self, value: Any) -> None:
         """Do what is needed to fire an event."""
         self._central.fire_ha_event_callback(
             event_type=self.event_type, event_data=self.get_event_data(value=value)
         )
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.1/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/button.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,12 +55,12 @@
         if self.is_internal != data.is_internal:
             self.is_internal = data.is_internal
             do_update = True
         if self.last_execute_time != data.last_execute_time:
             self.last_execute_time = data.last_execute_time
             do_update = True
         if do_update:
-            self.fire_update_entity_callback()
+            self.fire_entity_updated_callback()
 
     async def press(self) -> None:
         """Handle the button press."""
         await self.central.execute_program(pid=self.pid)
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             value = str(value)
         elif isinstance(old_value, float):
             value = float(value)
 
         if old_value != value:
             self._old_value = old_value
             self._value = value
-            self.fire_update_entity_callback()
+            self.fire_entity_updated_callback()
 
     async def send_variable(self, value: Any) -> None:
         """Set variable value on CCU/Homegear."""
         if client := self.central.primary_client:
             await client.set_system_variable(
                 name=self.ccu_var_name, value=parse_sys_var(self.data_type, value)
             )
```

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.1/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/support.py` & `hahomematic-2024.4.1/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/platforms/update.py` & `hahomematic-2024.4.1/hahomematic/platforms/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,27 +67,31 @@
         return self._device.available_firmware
 
     @value_property
     def firmware_update_state(self) -> str | None:
         """Latest version available for install."""
         return self._device.firmware_update_state
 
-    def register_update_callback(self, update_callback: Callable, custom_id: str) -> None:
+    def register_entity_updated_callback(
+        self, entity_updated_callback: Callable, custom_id: str
+    ) -> None:
         """Register update callback."""
-        self._device.register_firmware_update_callback(update_callback)
+        self._device.register_firmware_update_callback(entity_updated_callback)
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None:
                 raise HaHomematicException(
                     f"REGISTER_UPDATE_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
-    def unregister_update_callback(self, update_callback: Callable, custom_id: str) -> None:
+    def unregister_entity_updated_callback(
+        self, entity_updated_callback: Callable, custom_id: str
+    ) -> None:
         """Unregister update callback."""
-        self._device.unregister_firmware_update_callback(update_callback)
+        self._device.unregister_firmware_update_callback(entity_updated_callback)
         if custom_id is not None:
             self._custom_id = None
 
     async def update_firmware(self, refresh_after_update_intervals: tuple[int, ...]) -> bool:
         """Turn the update on."""
         return await self._device.update_firmware(
             refresh_after_update_intervals=refresh_after_update_intervals
```

### Comparing `hahomematic-2024.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.1/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.1/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic/support.py` & `hahomematic-2024.4.1/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.1/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.0/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.1/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/hahomematic_support/client_local.py` & `hahomematic-2024.4.1/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/pyproject.toml` & `hahomematic-2024.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.0"
+version     = "2024.4.1"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.0/tests/test_action.py` & `hahomematic-2024.4.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_binary_sensor.py` & `hahomematic-2024.4.1/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_button.py` & `hahomematic-2024.4.1/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_central.py` & `hahomematic-2024.4.1/tests/test_central.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,15 +375,17 @@
     ebp_sensor = central.get_entities(platform=HmPlatform.SENSOR)
     assert ebp_sensor
     assert len(ebp_sensor) == 12
 
     def _device_changed(self, *args: Any, **kwargs: Any) -> None:
         """Handle device state changes."""
 
-    ebp_sensor[0].register_update_callback(update_callback=_device_changed, custom_id="some_id")
+    ebp_sensor[0].register_entity_updated_callback(
+        entity_updated_callback=_device_changed, custom_id="some_id"
+    )
     ebp_sensor2 = central.get_entities(platform=HmPlatform.SENSOR, registered=False)
     assert ebp_sensor2
     assert len(ebp_sensor2) == 11
 
 
 @pytest.mark.asyncio()
 async def test_hub_entities_by_platform(factory: helper.Factory) -> None:
@@ -392,26 +394,30 @@
     ebp_sensor = central.get_hub_entities(platform=HmPlatform.HUB_SENSOR)
     assert ebp_sensor
     assert len(ebp_sensor) == 4
 
     def _device_changed(self, *args: Any, **kwargs: Any) -> None:
         """Handle device state changes."""
 
-    ebp_sensor[0].register_update_callback(update_callback=_device_changed, custom_id="some_id")
+    ebp_sensor[0].register_entity_updated_callback(
+        entity_updated_callback=_device_changed, custom_id="some_id"
+    )
     ebp_sensor2 = central.get_hub_entities(
         platform=HmPlatform.HUB_SENSOR,
         registered=False,
     )
     assert ebp_sensor2
     assert len(ebp_sensor2) == 3
 
     ebp_sensor3 = central.get_hub_entities(platform=HmPlatform.HUB_BUTTON)
     assert ebp_sensor3
     assert len(ebp_sensor3) == 2
-    ebp_sensor3[0].register_update_callback(update_callback=_device_changed, custom_id="some_id")
+    ebp_sensor3[0].register_entity_updated_callback(
+        entity_updated_callback=_device_changed, custom_id="some_id"
+    )
     ebp_sensor4 = central.get_hub_entities(platform=HmPlatform.HUB_BUTTON, registered=False)
     assert ebp_sensor4
     assert len(ebp_sensor4) == 1
 
 
 @pytest.mark.asyncio()
 async def test_add_device(factory: helper.Factory) -> None:
```

### Comparing `hahomematic-2024.4.0/tests/test_central_pydevccu.py` & `hahomematic-2024.4.1/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_climate.py` & `hahomematic-2024.4.1/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_cover.py` & `hahomematic-2024.4.1/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_decorator.py` & `hahomematic-2024.4.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_device.py` & `hahomematic-2024.4.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_entity.py` & `hahomematic-2024.4.1/tests/test_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,18 @@
     central, _ = await factory.get_default_central(TEST_DEVICES)
     switch: CeSwitch = cast(CeSwitch, helper.get_prepared_custom_entity(central, "VCU2128127", 4))
     assert switch.usage == EntityUsage.CE_PRIMARY
 
     device_updated_mock = MagicMock()
     device_removed_mock = MagicMock()
 
-    switch.register_update_callback(update_callback=device_updated_mock, custom_id="some_id")
-    switch.register_remove_callback(remove_callback=device_removed_mock)
+    switch.register_entity_updated_callback(
+        entity_updated_callback=device_updated_mock, custom_id="some_id"
+    )
+    switch.register_entity_removed_callback(entity_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127"
     )
     central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
     assert factory.entity_event_mock.call_args_list[-1] == call(
@@ -61,16 +63,18 @@
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
     assert factory.system_event_mock.call_args_list[-1] == call(
         "deleteDevices", interface_id="CentralTest-BidCos-RF", addresses=["VCU2128127"]
     )
-    switch.unregister_update_callback(update_callback=device_updated_mock, custom_id="some_id")
-    switch.unregister_remove_callback(remove_callback=device_removed_mock)
+    switch.unregister_entity_updated_callback(
+        entity_updated_callback=device_updated_mock, custom_id="some_id"
+    )
+    switch.unregister_entity_removed_callback(entity_removed_callback=device_removed_mock)
 
     device_updated_mock.assert_called_with()
     device_removed_mock.assert_called_with()
 
 
 @pytest.mark.asyncio()
 async def test_generic_entity_callback(factory: helper.Factory) -> None:
@@ -78,16 +82,18 @@
     central, _ = await factory.get_default_central(TEST_DEVICES)
     switch: HmSwitch = cast(HmSwitch, central.get_generic_entity("VCU2128127:4", "STATE"))
     assert switch.usage == EntityUsage.NO_CREATE
 
     device_updated_mock = MagicMock()
     device_removed_mock = MagicMock()
 
-    switch.register_update_callback(update_callback=device_updated_mock, custom_id="some_id")
-    switch.register_remove_callback(remove_callback=device_removed_mock)
+    switch.register_entity_updated_callback(
+        entity_updated_callback=device_updated_mock, custom_id="some_id"
+    )
+    switch.register_entity_removed_callback(entity_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4_state/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127 State ch4"
     )
     central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
     assert factory.entity_event_mock.call_args_list[-1] == call(
@@ -101,16 +107,18 @@
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
     assert factory.system_event_mock.call_args_list[-1] == call(
         "deleteDevices", interface_id="CentralTest-BidCos-RF", addresses=["VCU2128127"]
     )
-    switch.unregister_update_callback(update_callback=device_updated_mock, custom_id="some_id")
-    switch.unregister_remove_callback(remove_callback=device_removed_mock)
+    switch.unregister_entity_updated_callback(
+        entity_updated_callback=device_updated_mock, custom_id="some_id"
+    )
+    switch.unregister_entity_removed_callback(entity_removed_callback=device_removed_mock)
 
     device_updated_mock.assert_called_with()
     device_removed_mock.assert_called_with()
 
 
 @pytest.mark.asyncio()
 async def test_load_custom_entity(factory: helper.Factory) -> None:
```

### Comparing `hahomematic-2024.4.0/tests/test_event.py` & `hahomematic-2024.4.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_json_rpc.py` & `hahomematic-2024.4.1/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_light.py` & `hahomematic-2024.4.1/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_lock.py` & `hahomematic-2024.4.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_number.py` & `hahomematic-2024.4.1/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_select.py` & `hahomematic-2024.4.1/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_sensor.py` & `hahomematic-2024.4.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_siren.py` & `hahomematic-2024.4.1/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_support.py` & `hahomematic-2024.4.1/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_switch.py` & `hahomematic-2024.4.1/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.0/tests/test_text.py` & `hahomematic-2024.4.1/tests/test_text.py`

 * *Files identical despite different names*

