# Comparing `tmp/zha-0.0.6.tar.gz` & `tmp/zha-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-0.0.6.tar", last modified: Wed Apr  3 14:47:29 2024, max compression
+gzip compressed data, was "zha-0.0.7.tar", last modified: Fri Apr  5 00:17:11 2024, max compression
```

## Comparing `zha-0.0.6.tar` & `zha-0.0.7.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.170809 zha-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 14:47:24.000000 zha-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 14:47:29.170809 zha-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 14:47:24.000000 zha-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-03 14:47:24.000000 zha-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:47:29.170809 zha-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 14:47:24.000000 zha-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.154809 zha-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_alarm_control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24049 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50974 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_cluster_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_debouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_fan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.158809 zha-0.0.6/zha/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 14:47:24.000000 zha-0.0.6/zha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.158809 zha-0.0.6/zha/application/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    26423 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/alarm_control_panel/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/alarm_control_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/alarm_control_panel/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/binary_sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/binary_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/binary_sensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/button/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/button/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/button/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/climate/
--rw-r--r--   0 runner    (1001) docker     (127)    31558 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/climate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/climate/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/cover/
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/cover/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/device_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/fan/
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/light/
--rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/lock/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/lock/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/number/
--rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/number/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/application/platforms/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/sensor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-03 14:47:24.000000 zha-0.0.6/zha/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-03 14:47:24.000000 zha-0.0.6/zha/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-03 14:47:24.000000 zha-0.0.6/zha/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-03 14:47:24.000000 zha-0.0.6/zha/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-03 14:47:24.000000 zha-0.0.6/zha/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 14:47:24.000000 zha-0.0.6/zha/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-03 14:47:24.000000 zha-0.0.6/zha/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-03 14:47:24.000000 zha-0.0.6/zha/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/zigbee/cluster_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24760 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/hvac.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/manufacturerspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37758 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 00:17:07.000000 zha-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 00:17:11.682067 zha-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:17:07.000000 zha-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-05 00:17:07.000000 zha-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:17:11.682067 zha-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 00:17:07.000000 zha-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.670066 zha-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_alarm_control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24049 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50974 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_cluster_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_debouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_fan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.670066 zha-0.0.7/zha/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:17:07.000000 zha-0.0.7/zha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26423 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/alarm_control_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/alarm_control_panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/alarm_control_panel/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/binary_sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/binary_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/binary_sensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/button/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/button/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)    31558 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/climate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/climate/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/cover/
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/cover/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/device_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/fan/
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/light/
+-rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/lock/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/number/
+-rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/number/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/sensor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-05 00:17:07.000000 zha-0.0.7/zha/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 00:17:07.000000 zha-0.0.7/zha/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-05 00:17:07.000000 zha-0.0.7/zha/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-05 00:17:07.000000 zha-0.0.7/zha/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-05 00:17:07.000000 zha-0.0.7/zha/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 00:17:07.000000 zha-0.0.7/zha/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 00:17:07.000000 zha-0.0.7/zha/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-05 00:17:07.000000 zha-0.0.7/zha/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/zha/zigbee/cluster_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    25212 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24605 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/manufacturerspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37573 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/zha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/top_level.txt
```

### Comparing `zha-0.0.6/LICENSE` & `zha-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/PKG-INFO` & `zha-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.6/pyproject.toml` & `zha-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_alarm_control_panel.py` & `zha-0.0.7/tests/test_alarm_control_panel.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_async_.py` & `zha-0.0.7/tests/test_async_.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_binary_sensor.py` & `zha-0.0.7/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_button.py` & `zha-0.0.7/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_climate.py` & `zha-0.0.7/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_cluster_handlers.py` & `zha-0.0.7/tests/test_cluster_handlers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_color.py` & `zha-0.0.7/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_cover.py` & `zha-0.0.7/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_debouncer.py` & `zha-0.0.7/tests/test_debouncer.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_device.py` & `zha-0.0.7/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_device_tracker.py` & `zha-0.0.7/tests/test_device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_discover.py` & `zha-0.0.7/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_event.py` & `zha-0.0.7/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_executor.py` & `zha-0.0.7/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_fan.py` & `zha-0.0.7/tests/test_fan.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_gateway.py` & `zha-0.0.7/tests/test_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
     assert isinstance(entity, GroupEntity)
     assert entity is not None
 
     info = entity.info_object
     assert info.class_name == "LightGroup"
     assert info.platform == Platform.LIGHT
-    assert info.unique_id == "light.0x0002"
+    assert info.unique_id == "light_zha_group_0x0002"
     assert info.name == "Test Group_0x0002"
     assert info.group_id == zha_group.group_id
     assert info.supported_features == LightEntityFeature.TRANSITION
     assert info.min_mireds == 153
     assert info.max_mireds == 500
     assert info.effect_list is None
```

### Comparing `zha-0.0.6/tests/test_light.py` & `zha-0.0.7/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_lock.py` & `zha-0.0.7/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_number.py` & `zha-0.0.7/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_registries.py` & `zha-0.0.7/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_select.py` & `zha-0.0.7/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_sensor.py` & `zha-0.0.7/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_siren.py` & `zha-0.0.7/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_switch.py` & `zha-0.0.7/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_thread.py` & `zha-0.0.7/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_units.py` & `zha-0.0.7/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/tests/test_update.py` & `zha-0.0.7/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/__init__.py` & `zha-0.0.7/zha/application/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/const.py` & `zha-0.0.7/zha/application/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/discovery.py` & `zha-0.0.7/zha/application/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         """Discover entities for a ZHA device."""
         _LOGGER.debug(
             "Discovering entities for device: %s-%s",
             str(device.ieee),
             device.name,
         )
 
-        if device.is_coordinator:
+        if device.is_active_coordinator:
             self.discover_coordinator_device_entities(device)
             return
 
         self.discover_quirks_v2_entities(device)
         PLATFORM_ENTITIES.clean_up()
 
     def discover_quirks_v2_entities(self, device: Device) -> None:
```

### Comparing `zha-0.0.6/zha/application/gateway.py` & `zha-0.0.7/zha/application/gateway.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/helpers.py` & `zha-0.0.7/zha/application/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/__init__.py` & `zha-0.0.7/zha/application/platforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     """A base class for group entities."""
 
     def __init__(
         self,
         group: Group,
     ) -> None:
         """Initialize a group."""
-        super().__init__(f"{self.PLATFORM}.{group.group_id}")
+        super().__init__(f"{self.PLATFORM}_zha_group_0x{group.group_id:04x}")
         self._name: str = f"{group.name}_0x{group.group_id:04x}"
         self._group: Group = group
         self._group.register_group_entity(self)
 
     @cached_property
     def identifiers(self) -> GroupEntityIdentifiers:
         """Return a dict with the information necessary to identify this entity."""
```

### Comparing `zha-0.0.6/zha/application/platforms/alarm_control_panel/__init__.py` & `zha-0.0.7/zha/application/platforms/alarm_control_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/alarm_control_panel/const.py` & `zha-0.0.7/zha/application/platforms/alarm_control_panel/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/binary_sensor/__init__.py` & `zha-0.0.7/zha/application/platforms/binary_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/binary_sensor/const.py` & `zha-0.0.7/zha/application/platforms/binary_sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/button/__init__.py` & `zha-0.0.7/zha/application/platforms/button/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/climate/__init__.py` & `zha-0.0.7/zha/application/platforms/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/climate/const.py` & `zha-0.0.7/zha/application/platforms/climate/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/cover/__init__.py` & `zha-0.0.7/zha/application/platforms/cover/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/cover/const.py` & `zha-0.0.7/zha/application/platforms/cover/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/device_tracker.py` & `zha-0.0.7/zha/application/platforms/device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/fan/__init__.py` & `zha-0.0.7/zha/application/platforms/fan/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/fan/const.py` & `zha-0.0.7/zha/application/platforms/fan/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/fan/helpers.py` & `zha-0.0.7/zha/application/platforms/fan/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/helpers.py` & `zha-0.0.7/zha/application/platforms/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/light/__init__.py` & `zha-0.0.7/zha/application/platforms/light/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/light/const.py` & `zha-0.0.7/zha/application/platforms/light/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/light/helpers.py` & `zha-0.0.7/zha/application/platforms/light/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/lock/__init__.py` & `zha-0.0.7/zha/application/platforms/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/number/__init__.py` & `zha-0.0.7/zha/application/platforms/number/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/number/const.py` & `zha-0.0.7/zha/application/platforms/number/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/select.py` & `zha-0.0.7/zha/application/platforms/select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/sensor/__init__.py` & `zha-0.0.7/zha/application/platforms/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/sensor/const.py` & `zha-0.0.7/zha/application/platforms/sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/siren.py` & `zha-0.0.7/zha/application/platforms/siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/switch.py` & `zha-0.0.7/zha/application/platforms/switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/platforms/update.py` & `zha-0.0.7/zha/application/platforms/update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/application/registries.py` & `zha-0.0.7/zha/application/registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/async_.py` & `zha-0.0.7/zha/async_.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/debounce.py` & `zha-0.0.7/zha/debounce.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/decorators.py` & `zha-0.0.7/zha/decorators.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/event.py` & `zha-0.0.7/zha/event.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/mixins.py` & `zha-0.0.7/zha/mixins.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/units.py` & `zha-0.0.7/zha/units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/__init__.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,18 +265,14 @@
         """Return the status of the cluster handler."""
         return self._status
 
     def __hash__(self) -> int:
         """Make this a hashable."""
         return hash(self._unique_id)
 
-    def emit_propagated_event(self, signal: str, *args: Any) -> None:
-        """Send a signal through dispatcher."""
-        self._endpoint.emit_propagated_event(signal, *args)
-
     async def bind(self) -> None:
         """Bind a zigbee cluster.
 
         This also swallows ZigbeeException exceptions that are thrown when
         devices are unreachable.
         """
         try:
```

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/closures.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/closures.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/const.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,9 +102,8 @@
 PARAMS: Final[str] = "params"
 
 SIGNAL_ATTR_UPDATED: Final[str] = "attribute_updated"
 SIGNAL_MOVE_LEVEL: Final[str] = "move_level"
 SIGNAL_REMOVE: Final[str] = "remove"
 SIGNAL_SET_LEVEL: Final[str] = "set_level"
 SIGNAL_STATE_ATTR: Final[str] = "update_state_attribute"
-SIGNAL_UPDATE_DEVICE: Final[str] = "{}_zha_update_device"
 UNKNOWN: Final[str] = "unknown"
```

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/general.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     REPORT_CONFIG_BATTERY_SAVE,
     REPORT_CONFIG_DEFAULT,
     REPORT_CONFIG_IMMEDIATE,
     REPORT_CONFIG_MAX_INT,
     REPORT_CONFIG_MIN_INT,
     SIGNAL_MOVE_LEVEL,
     SIGNAL_SET_LEVEL,
-    SIGNAL_UPDATE_DEVICE,
 )
 from zha.zigbee.cluster_handlers.helpers import is_hue_motion_sensor
 
 if TYPE_CHECKING:
     from zha.zigbee.endpoint import Endpoint
 
 
@@ -297,15 +296,15 @@
     BIND: bool = False
 
     def cluster_command(self, tsn, command_id, args):
         """Handle commands received to this cluster."""
         cmd = parse_and_log_command(self, tsn, command_id, args)
 
         if cmd == Identify.ServerCommandDefs.trigger_effect.name:
-            self.emit_propagated_event(f"{self.unique_id}_{cmd}", args[0])
+            self.emit_zha_event(f"{self.unique_id}_{cmd}", args[0])
 
 
 @registries.CLIENT_CLUSTER_HANDLER_REGISTRY.register(LevelControl.cluster_id)
 class LevelControlClientClusterHandler(ClientClusterHandler):
     """LevelControl client cluster."""
 
 
@@ -586,27 +585,24 @@
     def cluster_command(
         self, tsn: int, command_id: int, args: list[Any] | None
     ) -> None:
         """Handle OTA commands."""
         if command_id not in self.cluster.server_commands:
             return
 
-        signal_id = self._endpoint.unique_id.split("-")[0]
         cmd_name = self.cluster.server_commands[command_id].name
 
         if cmd_name == Ota.ServerCommandDefs.query_next_image.name:
             assert args
 
             current_file_version = args[3]
             self.cluster.update_attribute(
                 Ota.AttributeDefs.current_file_version.id, current_file_version
             )
-            self.emit_propagated_event(
-                SIGNAL_UPDATE_DEVICE.format(signal_id), current_file_version
-            )
+            self._endpoint.device.sw_version = current_file_version
 
 
 @registries.CLUSTER_HANDLER_REGISTRY.register(Partition.cluster_id)
 class PartitionClusterHandler(ClusterHandler):
     """Partition cluster handler."""
```

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/helpers.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/homeautomation.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/hvac.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/hvac.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/lighting.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/lighting.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/lightlink.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/lightlink.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/manufacturerspecific.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/manufacturerspecific.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/measurement.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/measurement.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/protocol.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/protocol.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/security.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,17 @@
 
         zigbee_reply = self.arm_map[mode](code)
         self._endpoint.device.gateway.async_create_task(zigbee_reply)
 
         if self.invalid_tries >= self.max_invalid_tries:
             self.alarm_status = AceCluster.AlarmStatus.Emergency
             self.armed_state = AceCluster.PanelStatus.In_Alarm
-            self.emit_propagated_event(f"{self.unique_id}_{SIGNAL_ALARM_TRIGGERED}")
+            self.emit_zha_event(f"{self.unique_id}_{SIGNAL_ALARM_TRIGGERED}", [])
         else:
-            self.emit_propagated_event(f"{self.unique_id}_{SIGNAL_ARMED_STATE_CHANGED}")
+            self.emit_zha_event(f"{self.unique_id}_{SIGNAL_ARMED_STATE_CHANGED}", [])
         self._emit_panel_status_changed()
 
     def _disarm(self, code: str):
         """Test the code and disarm the panel if the code is correct."""
         if (
             code != self.panel_code
             and self.armed_state != AceCluster.PanelStatus.Panel_Disarmed
```

### Comparing `zha-0.0.6/zha/zigbee/cluster_handlers/smartenergy.py` & `zha-0.0.7/zha/zigbee/cluster_handlers/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha/zigbee/device.py` & `zha-0.0.7/zha/zigbee/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 from zha.zigbee.cluster_handlers import ClusterHandler, ZDOClusterHandler
 from zha.zigbee.endpoint import Endpoint
 
 if TYPE_CHECKING:
     from zha.application.gateway import Gateway
 
 _LOGGER = logging.getLogger(__name__)
-_UPDATE_ALIVE_INTERVAL = (60, 90)
 _CHECKIN_GRACE_PERIODS = 2
 
 
 def get_device_automation_triggers(
     device: zigpy.device.Device,
 ) -> dict[tuple[str, str], dict[str, str]]:
     """Get the supported device automation triggers for a zigpy device."""
@@ -239,15 +238,15 @@
                 CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY,
             )
         self._available: bool = self.is_active_coordinator or (
             self.last_seen is not None
             and time.time() - self.last_seen < self.consider_unavailable_time
         )
         self._checkins_missed_count: int = 0
-        self._on_network: bool = False
+        self._on_network: bool = True
 
         self._platform_entities: dict[str, PlatformEntity] = {}
         self.semaphore: asyncio.Semaphore = asyncio.Semaphore(3)
         self._tracked_tasks: list[asyncio.Task] = []
         self._zdo_handler: ZDOClusterHandler = ZDOClusterHandler(self)
         self.status: DeviceStatus = DeviceStatus.CREATED
 
@@ -479,14 +478,19 @@
         }
 
     @property
     def sw_version(self) -> str | None:
         """Return the software version for this device."""
         return self._sw_build_id
 
+    @sw_version.setter
+    def sw_version(self, sw_build_id) -> None:
+        """Set the software version for this device."""
+        self._sw_build_id = sw_build_id
+
     @property
     def platform_entities(self) -> dict[str, PlatformEntity]:
         """Return the platform entities for this device."""
         return self._platform_entities
 
     def get_platform_entity(self, unique_id: str) -> PlatformEntity:
         """Get a platform entity by unique id."""
@@ -499,24 +503,14 @@
     def new(
         cls,
         zigpy_dev: zigpy.device.Device,
         gateway: Gateway,
     ) -> Self:
         """Create new device."""
         zha_dev = cls(zigpy_dev, gateway)
-        # pylint: disable=pointless-string-statement
-        """TODO verify
-        zha_dev.unsubs.append(
-            async_dispatcher_connect(
-                hass,
-                SIGNAL_UPDATE_DEVICE.format(str(zha_dev.ieee)),
-                zha_dev.async_update_sw_build_id,
-            )
-        )
-        """
         discovery.DEVICE_PROBE.discover_device_entities(zha_dev)
         return zha_dev
 
     def async_update_sw_build_id(self, sw_version: int) -> None:
         """Update device sw version."""
         self._sw_build_id = sw_version
```

### Comparing `zha-0.0.6/zha/zigbee/endpoint.py` & `zha-0.0.7/zha/zigbee/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,18 +230,14 @@
             (
                 entity_class,
                 (unique_id, cluster_handlers, self, self.device),
                 kwargs or {},
             )
         )
 
-    def emit_propagated_event(self, signal: str, *args: Any) -> None:
-        """Send a signal through hass dispatcher."""
-        self.device.emit(signal, *args)
-
     def emit_zha_event(self, event_data: dict[str, Any]) -> None:
         """Broadcast an event from this endpoint."""
         self.device.emit_zha_event(
             {
                 const.ATTR_UNIQUE_ID: self.unique_id,
                 const.ATTR_ENDPOINT_ID: self.id,
                 **event_data,
```

### Comparing `zha-0.0.6/zha/zigbee/group.py` & `zha-0.0.7/zha/zigbee/group.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.6/zha.egg-info/PKG-INFO` & `zha-0.0.7/zha.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.6/zha.egg-info/SOURCES.txt` & `zha-0.0.7/zha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

