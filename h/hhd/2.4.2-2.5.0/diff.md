# Comparing `tmp/hhd-2.4.2.tar.gz` & `tmp/hhd-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.4.2.tar", last modified: Sun Mar 31 20:09:45 2024, max compression
+gzip compressed data, was "hhd-2.5.0.tar", last modified: Fri Apr  5 20:38:42 2024, max compression
```

## Comparing `hhd-2.4.2.tar` & `hhd-2.5.0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-31 20:09:40.000000 hhd-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-31 20:09:40.000000 hhd-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-03-31 20:09:45.724476 hhd-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-31 20:09:40.000000 hhd-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    21608 2024-03-31 20:09:40.000000 hhd-2.4.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 20:09:45.724476 hhd-2.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.712476 hhd-2.4.2/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25480 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.712476 hhd-2.4.2/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.712476 hhd-2.4.2/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35205 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19142 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.716476 hhd-2.4.2/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/http/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.720476 hhd-2.4.2/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-03-31 20:09:40.000000 hhd-2.4.2/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-31 20:09:45.000000 hhd-2.4.2/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.708476 hhd-2.4.2/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:09:45.724476 hhd-2.4.2/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-31 20:09:40.000000 hhd-2.4.2/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.873491 hhd-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 20:38:34.000000 hhd-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 20:38:34.000000 hhd-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-05 20:38:42.869491 hhd-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 20:38:34.000000 hhd-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-04-05 20:38:34.000000 hhd-2.5.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:38:42.873491 hhd-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/uinput/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.4.2/LICENSE` & `hhd-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/PKG-INFO` & `hhd-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.4.2
+Version: 2.5.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -91,15 +91,15 @@
   - Air Standard/Plus/Pro
   - 1S/1S Limited
   - 2/2S 
   - GEEK, GEEK 1S 
   - NEXT Lite/Pro/Advance
   - SLIDE
 - Ayn
-  - Loki Max
+  - Loki Zero/Max
 - AOKZOE
   - A1
   - A1 Pro 
 - Onexplayer
   - Mini Pro
 
 In addition, Handheld Daemon will attempt to work on Ayaneo, Ayn, Onexplayer, and
```

### Comparing `hhd-2.4.2/pyproject.toml` & `hhd-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.4.2"
+version = "2.5.0"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hhd-2.4.2/readme.md` & `hhd-2.5.0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   - Air Standard/Plus/Pro
   - 1S/1S Limited
   - 2/2S 
   - GEEK, GEEK 1S 
   - NEXT Lite/Pro/Advance
   - SLIDE
 - Ayn
-  - Loki Max
+  - Loki Zero/Max
 - AOKZOE
   - A1
   - A1 Pro 
 - Onexplayer
   - Mini Pro
 
 In addition, Handheld Daemon will attempt to work on Ayaneo, Ayn, Onexplayer, and
```

### Comparing `hhd-2.4.2/src/hhd/__main__.py` & `hhd-2.5.0/src/hhd/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
 ERROR_DELAY = 5
 INIT_DELAY = 0.4
 POLL_DELAY = 2
 
 
 class EmitHolder(Emitter):
-    def __init__(self, condition: Condition) -> None:
+    def __init__(self, condition: Condition, ctx) -> None:
         self._events = []
         self._condition = condition
-        super().__init__()
+        super().__init__(ctx=ctx)
 
     def __call__(self, event: Event | Sequence[Event]) -> None:
         with self._condition:
             if isinstance(event, Sequence):
                 self._events.extend(event)
             else:
                 self._events.append(event)
@@ -222,15 +222,15 @@
         if not sorted_plugins:
             logger.error(f"No plugins started, exiting...")
             return
 
         # Open plugins
         lock = RLock()
         cond = Condition(lock)
-        emit = EmitHolder(cond)
+        emit = EmitHolder(cond, ctx)
         for p in sorted_plugins:
             set_log_plugin(getattr(p, "log") if hasattr(p, "log") else "ukwn")
             p.open(emit, ctx)
             update_log_plugins()
         set_log_plugin("main")
 
         # Compile initial configuration
```

### Comparing `hhd-2.4.2/src/hhd/contrib/dev.py` & `hhd-2.5.0/src/hhd/contrib/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     endcap = False
     start = perf_counter()
     for ev in d.read_loop():
         curr = perf_counter() - start
         if ev.code == 0 and ev.type == 0 and ev.value == 0:
             print(
-                f"└ SYN ─ {curr:7.3}s ────────────────────────────────────────────────────────┘"
+                f"└ SYN ─ {curr:7.3f}s ────────────────────────────────────────────────────────┘"
             )
             endcap = True
         else:
             if endcap:
                 print(
                     "\n┌────────────────────────────────────────────────────────────────────────┐"
                 )
```

### Comparing `hhd-2.4.2/src/hhd/contrib/i18n.py` & `hhd-2.5.0/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/contrib/main.py` & `hhd-2.5.0/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/__init__.py` & `hhd-2.5.0/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/base.py` & `hhd-2.5.0/src/hhd/controller/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
+import os
 import select
 import time
-from io import BytesIO
-from queue import Queue
-from threading import Condition, RLock
-from typing import Any, Callable, Literal, NamedTuple, Protocol, Sequence, TypedDict
+from threading import RLock
+from typing import Any, Callable, Literal, Mapping, NamedTuple, Sequence, TypedDict
 
 from .const import Axis, Button, Configuration
 
 logger = logging.getLogger(__name__)
 
 
 class SpecialEvent(TypedDict):
@@ -85,18 +84,33 @@
 GRAB_TIMEOUT = 5
 
 QueueEvent = tuple[Any, Sequence[Event]]
 
 
 class ControllerEmitter:
 
-    def __init__(self) -> None:
+    def __init__(self, ctx=None) -> None:
         self.intercept_lock = RLock()
         self._intercept = None
         self._controller_cb = None
+        self._qam_cb = None
+        self.ctx = ctx
+        self.use_legacy_qam = bool(os.environ.get("HHD_QAM_LEGACY", None))
+
+    def send_qam(self):
+        with self.intercept_lock:
+            if self.use_legacy_qam:
+                return False
+            if self._qam_cb:
+                return self._qam_cb()
+            return False
+
+    def register_qam(self, cb: Callable[[], bool]):
+        with self.intercept_lock:
+            self._qam_cb = cb
 
     def grab(self, enable: bool):
         with self.intercept_lock:
             if enable:
                 self._intercept = time.perf_counter()
             else:
                 self._intercept = None
@@ -309,19 +323,21 @@
         """Opens and returns a list of file descriptors that should be listened to."""
         raise NotImplementedError()
 
     def close(self, exit: bool) -> bool:
         """Called to close the device.
 
         If `exit` is true, the program is about to
-        close. If it is false, the controller is entering power save mode because
-        it is unused. In this case, if this service is required, you may forgo
-        closing and return false. If true, it is assumed this producer is closed.
-
-        `open()` will be called again once the consumers are ready."""
+        close. If it is false, the controller may be performing a configuration
+        change.
+        
+        In the first versions of Handheld Daemon, this API was meant to be used
+        for the controller to enter power saving mode. However, it turns out
+        that steam and the kernel do not let the controller disconnect,
+        so it was repurposed to skip controller hiding."""
         return False
 
     def produce(self, fds: Sequence[int]) -> Sequence[Event]:
         """Called with the file descriptors that are ready to read."""
         return []
 
 
@@ -340,21 +356,22 @@
 
 
 TouchpadAction = Literal["disabled", "left_click", "right_click"]
 
 
 class Multiplexer:
     QAM_HOLD_TIME = 0.5
-    QAM_MULTI_PRESS_DELAY = 0.225
+    QAM_MULTI_PRESS_DELAY = 0.2
     QAM_DELAY = 0.125
     REBOOT_HOLD = 4
     REBOOT_VIBRATION_STRENGTH = 0.6
     REBOOT_VIBRATION_ON = 0.3
     REBOOT_VIBRATION_OFF = 0.8
     REBOOT_VIBRATION_NUM = 3
+    STEAM_CHECK_INTERVAL = 3
 
     def __init__(
         self,
         swap_guide: (
             None | Literal["guide_is_start", "guide_is_select", "select_is_guide"]
         ) = None,
         trigger: None | Literal["analog_to_discrete", "discrete_to_analogue"] = None,
@@ -371,14 +388,16 @@
         touchpad_hold: TouchpadAction = "disabled",
         r3_to_share: bool = False,
         select_reboots: bool = False,
         nintendo_mode: bool = False,
         qam_button: str | None = None,
         emit: ControllerEmitter | None = None,
         imu: None | Literal["left_to_main", "right_to_main", "main_to_sides"] = None,
+        params: Mapping[str, Any] = {},
+        qam_multi_tap: bool = True,
     ) -> None:
         self.swap_guide = swap_guide
         self.trigger = trigger
         self.dpad = dpad
         self.led = led
         self.touchpad = touchpad
         self.status = status
@@ -403,39 +422,61 @@
         if share_to_qam:
             self.qam_button = "share"
 
         self.qam_pressed = None
         self.qam_pre_sent = False
         self.qam_released = None
         self.qam_times = 0
+        self.qam_multi_tap = qam_multi_tap and not os.environ.get(
+            "HHD_QAM_MULTI_DISABLE", None
+        )
         self.guide_pressed = False
+        self.steam_check = params.get("steam_check", None)
+        self.steam_check_last = time.perf_counter()
+        self.steam_check_fn = params.get("steam_check_fn", None)
 
         self.unique = str(time.perf_counter_ns())
         assert touchpad is None, "touchpad rewiring not supported yet"
 
     def process(self, events: Sequence[Event]):
         out: list[Event] = []
         status_events = set()
         touched = False
 
         curr = time.perf_counter()
+
+        # Send old events
         while len(self.queue) and self.queue[0][1] < curr:
             ev = self.queue.pop(0)[0]
             if ev == "reboot":
                 if self.select_is_held:
                     try:
                         import os
 
                         os.system("systemctl reboot")
                         logger.info("rebooting")
                     except Exception as e:
                         logger.error(f"Rebooting failed with error:\n{type(e)}:{e}")
             elif self.select_is_held or not ev.get("from_reboot", False):
                 out.append(ev)
 
+        # Check for steam for touchpad emulation
+        if (
+            self.steam_check_fn
+            and self.steam_check is not None
+            and self.steam_check_last + Multiplexer.STEAM_CHECK_INTERVAL < curr
+        ):
+            self.steam_check_last = curr
+            if self.steam_check:
+                msg = "Gamepadui launched. Restarting controller to enable touchpad emulation."
+            else:
+                msg = "Gamepadui closed. Restarting controller to disable touchpad emulation."
+
+            assert self.steam_check_fn() == self.steam_check, msg
+
         if self.select_pressed and self.select_pressed + self.REBOOT_HOLD < curr:
             self.select_pressed = None
             for i in range(self.REBOOT_VIBRATION_NUM):
                 self.queue.append(
                     (
                         {
                             "type": "rumble",
@@ -766,15 +807,18 @@
             )
 
         # Handle QAM button
         qam_apply = False
         was_held = True
         if self.qam_pressed and curr - self.qam_pressed > self.QAM_HOLD_TIME:
             qam_apply = True
-        if self.qam_released and curr - self.qam_released > self.QAM_MULTI_PRESS_DELAY:
+        if self.qam_released and (
+            curr - self.qam_released > self.QAM_MULTI_PRESS_DELAY
+            or not self.qam_multi_tap
+        ):
             qam_apply = True
         if (
             self.qam_pressed
             and self.qam_times == 2
             and not self.qam_pre_sent
             and self.emit
         ):
@@ -856,51 +900,54 @@
             return [
                 o
                 for o in events
                 if o["type"] not in ("button", "axis") or "ts" in o.get("code", "")
             ]
         elif send_steam_qam:
             # Send steam qam only if not intercepting
-            out.append(
-                {
-                    "type": "button",
-                    "code": "mode",
-                    "value": True,
-                },
-            )
-            self.queue.append(
-                (
+            if not self.emit or not self.emit.send_qam():
+                # Have a fallback if gamescope is not working
+                out.append(
                     {
                         "type": "button",
-                        "code": "a",
+                        "code": "mode",
                         "value": True,
                     },
-                    curr + self.QAM_DELAY,
                 )
-            )
-            self.queue.append(
-                (
-                    {
-                        "type": "button",
-                        "code": "a",
-                        "value": False,
-                    },
-                    curr + 2 * self.QAM_DELAY,
-                ),
-            )
-            self.queue.append(
-                (
-                    {
-                        "type": "button",
-                        "code": "mode",
-                        "value": False,
-                    },
-                    curr + 2 * self.QAM_DELAY,
-                ),
-            )
+                self.queue.append(
+                    (
+                        {
+                            "type": "button",
+                            "code": "a",
+                            "value": True,
+                        },
+                        curr + self.QAM_DELAY,
+                    )
+                )
+                self.queue.append(
+                    (
+                        {
+                            "type": "button",
+                            "code": "a",
+                            "value": False,
+                        },
+                        curr + 2 * self.QAM_DELAY,
+                    ),
+                )
+                self.queue.append(
+                    (
+                        {
+                            "type": "button",
+                            "code": "mode",
+                            "value": False,
+                        },
+                        curr + 2 * self.QAM_DELAY,
+                    ),
+                )
+
         return out
 
 
 class KeyboardWrapper(Producer, Consumer):
     def __init__(
         self, parent: Producer, button_map: Sequence[tuple[set[Button], Button]]
     ) -> None:
```

### Comparing `hhd-2.4.2/src/hhd/controller/const.py` & `hhd-2.5.0/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/lib/common.py` & `hhd-2.5.0/src/hhd/controller/lib/common.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/lib/hid.py` & `hhd-2.5.0/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/lib/hide.py` & `hhd-2.5.0/src/hhd/controller/lib/hide.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,26 +52,31 @@
 
 def hide_gamepad(devpath: str, vid: int, pid: int) -> str | None:
     input_dev = get_gamepad_name(devpath)
     parent = get_parent_sysfs(devpath)
     if not input_dev or not parent:
         return None
 
+    out_fn = f"/run/udev/rules.d/95-hhd-devhide-{input_dev}.rules"
+    if os.path.exists(out_fn):
+        # Skip hiding controller on reloads
+        return input_dev
+
     rule = f"""\
 # Hides device gamepad devices stemming from {input_dev}
 # Managed by HHD, this file will be autoremoved during configuration changes.
 SUBSYSTEMS=="input", KERNELS=="{input_dev}", ATTRS{{id/vendor}}=="{vid:04x}", ATTRS{{id/product}}=="{pid:04x}", GOTO="hhd_valid"
 GOTO="hhd_end"
 LABEL="hhd_valid"
 KERNEL=="js[0-9]*|event[0-9]*", SUBSYSTEM=="input", MODE="000", GROUP="root", TAG-="uaccess", RUN+="/bin/chmod 000 /dev/input/%k"
 LABEL="hhd_end"
 """  # , RUN+="/bin/chmod 000 /sys/%p"
     try:
         os.makedirs("/run/udev/rules.d/", exist_ok=True)
-        with open(f"/run/udev/rules.d/95-hhd-devhide-{input_dev}.rules", "w") as f:
+        with open(out_fn, "w") as f:
             f.write(rule)
         reload_children(parent)
         return input_dev
     except Exception:
         return None
```

### Comparing `hhd-2.4.2/src/hhd/controller/lib/ioctl.py` & `hhd-2.5.0/src/hhd/controller/lib/ioctl.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/lib/uhid.py` & `hhd-2.5.0/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/physical/evdev.py` & `hhd-2.5.0/src/hhd/controller/physical/evdev.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import glob
 import logging
 import os
 import re
+import stat
 import subprocess
 import time
 from typing import Collection, Mapping, Sequence, TypeVar, cast
 
 import evdev
 from evdev import ecodes, ff
 
 from hhd.controller import Axis, Button, Consumer, Event, Producer, can_read
 from hhd.controller.base import Event
 from hhd.controller.const import AbsAxis, GamepadButton, KeyboardButton
 from hhd.controller.lib.common import hexify, matches_patterns
-from hhd.controller.lib.hide import hide_gamepad, unhide_all, unhide_gamepad
+from hhd.controller.lib.hide import hide_gamepad, unhide_gamepad
 
 logger = logging.getLogger(__name__)
 
 
 def B(b: str):
     return cast(int, getattr(evdev.ecodes, b))
 
@@ -145,14 +146,69 @@
 def find_joystick(ev: str):
     path = get_path(ev)
     for other in list_joysticks():
         if path == get_path(other):
             return other
 
 
+def is_device(fn):
+    """Check if ``fn`` is a readable and writable character device."""
+
+    if not os.path.exists(fn):
+        return False
+
+    m = os.stat(fn)[stat.ST_MODE]
+    if not stat.S_ISCHR(m):
+        return False
+
+    if not os.access(fn, os.R_OK | os.W_OK):
+        return False
+
+    return True
+
+
+def list_evs(filter_valid: bool = False):
+    with open("/proc/bus/input/devices", "r") as f:
+        data = f.read()
+
+        devs = {}
+        for d in data.split("\n\n"):
+            out = {}
+            for line in d.split("\n"):
+                if not line:
+                    continue
+                match line[0]:
+                    case "I":
+                        for attr in line[3:-1].split(" "):
+                            name, val = attr.split("=")
+                            out[name.lower()] = int(val, 16)
+                    case "N":
+                        out["name"] = line[len('N: Name="') : -1]
+                    case "H":
+                        for handler in line[len("H: Handlers=") : -1].split(" "):
+                            if "event" in handler:
+                                pth = "/dev/input/" + handler
+                                if not filter_valid or is_device(pth):
+                                    devs[pth] = out
+
+        return devs
+
+
+def enumerate_evs(
+    vid: int | None = None, pid: int | None = None, filter_valid: bool = False
+):
+    evs = list_evs(filter_valid)
+    return {
+        k: v
+        for k, v in evs.items()
+        if (vid is None or vid == v.get("vendor", None))
+        and (pid is None or pid == v.get("product", None))
+    }
+
+
 class GenericGamepadEvdev(Producer, Consumer):
 
     def __init__(
         self,
         vid: Sequence[int],
         pid: Sequence[int],
         name: Sequence[str | re.Pattern] = "",
@@ -184,22 +240,22 @@
         self.hide = hide
         self.grab = grab
         self.hidden = None
         self.queue = []
         self.postprocess = postprocess
 
     def open(self) -> Sequence[int]:
-        for d in evdev.list_devices():
-            dev = evdev.InputDevice(d)
-            if not matches_patterns(dev.info.vendor, self.vid):
+        for d, info in list_evs(filter_valid=True).items():
+            if not matches_patterns(info.get("vendor", ""), self.vid):
                 continue
-            if not matches_patterns(dev.info.product, self.pid):
+            if not matches_patterns(info.get("product", ""), self.pid):
                 continue
-            if not matches_patterns(dev.name, self.name):
+            if not matches_patterns(info.get("name", ""), self.name):
                 continue
+            dev = evdev.InputDevice(d)
             if self.capabilities:
                 matches = True
                 dev_cap = cast(dict[int, Sequence[int]], dev.capabilities())
                 for cap_id, caps in self.capabilities.items():
                     if cap_id not in dev_cap:
                         matches = False
                         break
@@ -249,15 +305,15 @@
         logger.error(err)
         if self.required:
             raise RuntimeError()
         return []
 
     def close(self, exit: bool) -> bool:
         if self.dev:
-            if self.hidden:
+            if self.hidden and exit:
                 unhide_gamepad(self.dev.path, self.hidden)
             self.dev.close()
             self.dev = None
             self.fd = 0
         return True
 
     def consume(self, events: Sequence[Event]):
```

### Comparing `hhd-2.4.2/src/hhd/controller/physical/hidraw.py` & `hhd-2.5.0/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/physical/imu.py` & `hhd-2.5.0/src/hhd/controller/physical/imu.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/physical/rgb.py` & `hhd-2.5.0/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.5.0/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,14 @@
 
         logger.info(
             f"Starting '{(DS5_EDGE_NAME if self.edge_mode else DS5_NAME).decode()}'."
         )
         return [self.fd]
 
     def close(self, exit: bool) -> bool:
-        if not exit:
-            """This is a consumer, so we would deadlock if it was disabled."""
-            return False
-
         if self.dev:
             self.dev.send_destroy()
             self.dev.close()
             self.dev = None
             self.fd = None
 
         return True
```

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.5.0/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.5.0/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/sd/const.py` & `hhd-2.5.0/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.5.0/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.5.0/src/hhd/controller/virtual/uinput/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/generic/__init__.py` & `hhd-2.5.0/src/hhd/device/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/generic/base.py` & `hhd-2.5.0/src/hhd/device/generic/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 import time
 from threading import Event as TEvent
 
 import evdev
 
 from hhd.controller import Multiplexer
 from hhd.controller.physical.evdev import B as EC
-from hhd.controller.physical.evdev import GenericGamepadEvdev
+from hhd.controller.physical.evdev import GenericGamepadEvdev, enumerate_evs
 from hhd.controller.physical.imu import CombinedImu, HrtimerTrigger
 from hhd.controller.physical.rgb import LedDevice
 from hhd.controller.virtual.uinput import UInputDevice
-from hhd.plugins import Config, Context, Emitter, get_outputs, get_gyro_state
+from hhd.plugins import Config, Context, Emitter, get_gyro_state, get_outputs
 
-from .const import (
-    BTN_MAPPINGS,
-    DEFAULT_MAPPINGS,
-)
+from .const import BTN_MAPPINGS, DEFAULT_MAPPINGS
 
-ERROR_DELAY = 1
-SELECT_TIMEOUT = 1
+FIND_DELAY = 0.1
+ERROR_DELAY = 0.3
+LONGER_ERROR_DELAY = 3
+LONGER_ERROR_MARGIN = 1.3
 
 logger = logging.getLogger(__name__)
 
 
 GAMEPAD_VID = 0x045E
 GAMEPAD_PID = 0x028E
 
@@ -39,34 +38,31 @@
     emit: Emitter,
     context: Context,
     should_exit: TEvent,
     updated: TEvent,
     dconf: dict,
 ):
     first = True
+    init = time.perf_counter()
     while not should_exit.is_set():
         if conf["controller_mode.mode"].to(str) == "disabled":
             time.sleep(ERROR_DELAY)
             continue
 
-        found_gamepad = False
         try:
-            for d in evdev.list_devices():
-                dev = evdev.InputDevice(d)
-                if dev.info.vendor == GAMEPAD_VID and dev.info.product == GAMEPAD_PID:
-                    found_gamepad = True
-                    break
+            found_device = bool(enumerate_evs(vid=GAMEPAD_VID))
         except Exception:
             logger.warning("Failed finding device, skipping check.")
-            found_gamepad = True
+            time.sleep(LONGER_ERROR_DELAY)
+            found_device = True
 
-        if not found_gamepad:
+        if not found_device:
             if first:
                 logger.info("Controller not found. Waiting...")
-            time.sleep(ERROR_DELAY)
+            time.sleep(FIND_DELAY)
             first = False
             continue
 
         # Use the oxp-platform driver if available
         if os.path.exists("/sys/devices/platform/oxp-platform/tt_toggle"):
             try:
                 with open("/sys/devices/platform/oxp-platform/tt_toggle", "w") as f:
@@ -76,37 +72,42 @@
                 logger.warn(
                     f"Turbo takeover failed. Ensure you have the latest oxp-sensors driver installed."
                 )
 
         try:
             logger.info("Launching emulated controller.")
             updated.clear()
+            init = time.perf_counter()
             controller_loop(conf.copy(), should_exit, updated, dconf, emit)
+            repeated_fail = False
         except Exception as e:
+            failed_fast = init + LONGER_ERROR_MARGIN > time.perf_counter()
+            sleep_time = (
+                LONGER_ERROR_DELAY if repeated_fail and failed_fast else ERROR_DELAY
+            )
+            repeated_fail = failed_fast
             logger.error(f"Received the following error:\n{type(e)}: {e}")
             logger.error(
-                f"Assuming controllers disconnected, restarting after {ERROR_DELAY}s."
+                f"Assuming controllers disconnected, restarting after {sleep_time}s."
             )
             first = True
             # Raise exception
             if conf.get("debug", False):
                 raise e
-            time.sleep(ERROR_DELAY)
+            time.sleep(sleep_time)
 
 
 def controller_loop(
     conf: Config, should_exit: TEvent, updated: TEvent, dconf: dict, emit: Emitter
 ):
     debug = conf.get("debug", False)
 
     # Output
     d_producers, d_outs, d_params = get_outputs(
-        conf["controller_mode"],
-        None,
-        conf["imu"].to(bool),
+        conf["controller_mode"], None, conf["imu"].to(bool), emit=emit
     )
 
     # Imu
     d_imu = CombinedImu(
         conf["imu_hz"].to(int),
         get_gyro_state(conf["imu_axis"], dconf.get("mapping", DEFAULT_MAPPINGS)),
     )
@@ -132,14 +133,15 @@
 
     multiplexer = Multiplexer(
         trigger="analog_to_discrete",
         dpad="analog_to_discrete",
         share_to_qam=conf["share_to_qam"].to(bool),
         nintendo_mode=conf["nintendo_mode"].to(bool),
         emit=emit,
+        params=d_params,
     )
 
     d_volume_btn = UInputDevice(
         name="Handheld Daemon Volume Keyboard",
         phys="phys-hhd-vbtn",
         capabilities={EC("EV_KEY"): [EC("KEY_VOLUMEUP"), EC("KEY_VOLUMEDOWN")]},
         btn_map={
@@ -229,21 +231,21 @@
             elapsed = t - start
             if elapsed < REPORT_DELAY_MIN:
                 time.sleep(REPORT_DELAY_MIN - elapsed)
 
     except KeyboardInterrupt:
         raise
     finally:
-        # d_vend.close(True)
+        # d_vend.close(not updated.is_set())
         try:
             d_timer.close()
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         for d in reversed(devs):
             try:
-                d.close(True)
+                d.close(not updated.is_set())
             except Exception as e:
                 logger.error(f"Error while closing device '{d}' with exception:\n{e}")
                 if debug:
                     raise e
```

### Comparing `hhd-2.4.2/src/hhd/device/generic/const.py` & `hhd-2.5.0/src/hhd/device/generic/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,19 +85,29 @@
 CONFS = {
     # Aokzoe
     "AOKZOE A1 AR07": {"name": "AOKZOE A1", "hrtimer": True},
     "AOKZOE A1 Pro": {"name": "AOKZOE A1 Pro", "hrtimer": True},
     # Onexplayer
     "ONEXPLAYER Mini Pro": {"name": "ONEXPLAYER Mini Pro", "hrtimer": True},
     # Ayn
+    "Loki MiniPro": {
+        "name": "Loki MiniPro",
+        "hrtimer": True,
+        "mapping": gen_gyro_state("x", False, "z", False, "y", True),
+    },
     "Loki Max": {
         "name": "Loki Max",
         "hrtimer": True,
         "mapping": gen_gyro_state("x", False, "z", False, "y", True),
     },
+    "Loki Zero": {
+        "name": "Loki Zero",
+        "hrtimer": True,
+        "mapping": gen_gyro_state("x", False, "z", False, "y", True),
+    },
     # Ayaneo
     "AIR Plus": {
         "name": "AYANEO AIR Plus",
         **AYA_DEFAULT_CONF,
         "mapping": AYANEO_AIR_PLUS_MAPPINGS,
     },
     "AIR 1S": {"name": "AIR 1S", **AYA_DEFAULT_CONF},
```

### Comparing `hhd-2.4.2/src/hhd/device/generic/controllers.yml` & `hhd-2.5.0/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/gpd/win/__init__.py` & `hhd-2.5.0/src/hhd/device/gpd/win/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/gpd/win/base.py` & `hhd-2.5.0/src/hhd/device/gpd/win/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 
 from .const import (
     GPD_TOUCHPAD_AXIS_MAP,
     GPD_TOUCHPAD_BUTTON_MAP,
     GPD_WIN_DEFAULT_MAPPINGS,
 )
 
-ERROR_DELAY = 1
+ERROR_DELAY = 0.3
 SELECT_TIMEOUT = 1
+ERROR_DELAY = 0.3
+LONGER_ERROR_DELAY = 3
+LONGER_ERROR_MARGIN = 1.3
 
 logger = logging.getLogger(__name__)
 
 GPD_WIN_4_VID = 0x2F24
 GPD_WIN_4_PID = 0x0135
 GAMEPAD_VID = 0x045E
 GAMEPAD_PID = 0x028E
@@ -149,14 +152,16 @@
     emit: Emitter,
     context: Context,
     should_exit: TEvent,
     updated: TEvent,
     dconf: dict,
 ):
     first = True
+    init = time.perf_counter()
+    repeated_fail = False
     while not should_exit.is_set():
         if conf["controller_mode.mode"].to(str) == "disabled":
             time.sleep(ERROR_DELAY)
             continue
 
         found_gamepad = False
         try:
@@ -175,38 +180,45 @@
             time.sleep(ERROR_DELAY)
             first = False
             continue
 
         try:
             logger.info("Launching emulated controller.")
             updated.clear()
+            init = time.perf_counter()
             controller_loop(conf.copy(), should_exit, updated, dconf, emit)
+            repeated_fail = False
         except Exception as e:
+            failed_fast = init + LONGER_ERROR_MARGIN > time.perf_counter()
+            sleep_time = (
+                LONGER_ERROR_DELAY if repeated_fail and failed_fast else ERROR_DELAY
+            )
+            repeated_fail = failed_fast
             logger.error(f"Received the following error:\n{type(e)}: {e}")
             logger.error(
-                f"Assuming controllers disconnected, restarting after {ERROR_DELAY}s."
+                f"Assuming controllers disconnected, restarting after {sleep_time}s."
             )
-            first = True
             # Raise exception
             if conf.get("debug", False):
                 raise e
-            time.sleep(ERROR_DELAY)
+            time.sleep(sleep_time)
 
 
 def controller_loop(
     conf: Config, should_exit: TEvent, updated: TEvent, dconf: dict, emit: Emitter
 ):
     debug = conf.get("debug", False)
     has_touchpad = dconf.get("touchpad", False)
 
     # Output
     d_producers, d_outs, d_params = get_outputs(
         conf["controller_mode"],
         conf["touchpad"] if has_touchpad else None,
         conf["imu"].to(bool),
+        emit=emit,
     )
 
     # Imu
     d_imu = CombinedImu(
         conf["imu_hz"].to(int),
         get_gyro_state(
             conf["imu_axis"], dconf.get("mapping", GPD_WIN_DEFAULT_MAPPINGS)
@@ -275,22 +287,26 @@
             trigger="analog_to_discrete",
             dpad="analog_to_discrete",
             touchpad_short=touch_actions["short"].to(TouchpadAction),
             touchpad_hold=touch_actions["hold"].to(TouchpadAction),
             nintendo_mode=conf["nintendo_mode"].to(bool),
             qam_button=qam_button,
             emit=emit,
+            params=d_params,
+            qam_multi_tap=False,
         )
     else:
         multiplexer = Multiplexer(
             trigger="analog_to_discrete",
             dpad="analog_to_discrete",
             nintendo_mode=conf["nintendo_mode"].to(bool),
             qam_button=qam_button,
             emit=emit,
+            params=d_params,
+            qam_multi_tap=False,
         )
 
     REPORT_FREQ_MIN = 25
     REPORT_FREQ_MAX = 400
 
     if conf["imu"].to(bool):
         REPORT_FREQ_MAX = max(REPORT_FREQ_MAX, conf["imu_hz"].to(float))
@@ -365,25 +381,25 @@
             if elapsed < REPORT_DELAY_MIN:
                 time.sleep(REPORT_DELAY_MIN - elapsed)
 
     except KeyboardInterrupt:
         raise
     finally:
         try:
-            d_vend.close(True)
+            d_vend.close(not updated.is_set())
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         try:
             d_timer.close()
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         for d in reversed(devs):
             try:
-                d.close(True)
+                d.close(not updated.is_set())
             except Exception as e:
                 logger.error(f"Error while closing device '{d}' with exception:\n{e}")
                 if debug:
                     raise e
```

### Comparing `hhd-2.4.2/src/hhd/device/gpd/win/const.py` & `hhd-2.5.0/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.5.0/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/__init__.py` & `hhd-2.5.0/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/base.py` & `hhd-2.5.0/src/hhd/device/legion_go/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from threading import Event as TEvent
 from typing import Sequence
 
 from hhd.controller import Axis, Button, Consumer, Event, Producer
 from hhd.controller.base import Multiplexer, TouchpadAction
 from hhd.controller.lib.hid import enumerate_unique
 from hhd.controller.physical.evdev import B as EC
-from hhd.controller.physical.evdev import GenericGamepadEvdev
+from hhd.controller.physical.evdev import GenericGamepadEvdev, enumerate_evs
 from hhd.controller.physical.imu import AccelImu, GyroImu
 from hhd.controller.virtual.uinput import (
     HHD_PID_MOTION,
     HHD_PID_VENDOR,
     MOTION_CAPABILITIES,
     MOTION_INPUT_PROPS,
     MOTION_LEFT_AXIS_MAP,
@@ -29,15 +29,18 @@
     LGO_RAW_INTERFACE_CONFIG_MAP,
     LGO_TOUCHPAD_AXIS_MAP,
     LGO_TOUCHPAD_BUTTON_MAP,
 )
 from .gyro_fix import GyroFixer
 from .hid import LegionHidraw, RgbCallback
 
-ERROR_DELAY = 1
+FIND_DELAY = 0.1
+ERROR_DELAY = 0.3
+LONGER_ERROR_DELAY = 3
+LONGER_ERROR_MARGIN = 1.3
 SELECT_TIMEOUT = 1
 
 logger = logging.getLogger(__name__)
 
 LEN_VID = 0x17EF
 LEN_PIDS = {
     0x6182: "xinput",
@@ -53,86 +56,97 @@
     context: Context,
     should_exit: TEvent,
     updated: TEvent,
     others: dict,
 ):
     reset = others.get("reset", False)
     gyro_fixer = None
+    init = time.perf_counter()
+    repeated_fail = False
 
     while not should_exit.is_set():
         if (
             conf["imu.mode"].to(str) == "display"
             and (gyro_fix := conf.get("imu.display.gyro_fix", False))
             and conf["imu.display.gyro"].to(bool)
         ):
             gyro_fixer = GyroFixer(int(gyro_fix) if int(gyro_fix) > 10 else 100)
         else:
             gyro_fixer = None
 
         try:
             controller_mode = None
             pid = None
+            first = True
             while not controller_mode:
-                devs = enumerate_unique(LEN_VID)
+                devs = enumerate_evs(vid=LEN_VID)
                 if not devs:
-                    logger.error(
-                        f"Legion go controllers not found, waiting {ERROR_DELAY}s."
-                    )
-                    time.sleep(ERROR_DELAY)
+                    if first:
+                        first = False
+                        logger.warning(f"Legion go controllers not found, waiting...")
+                    time.sleep(FIND_DELAY)
                     continue
 
-                for d in devs:
-                    if d["product_id"] in LEN_PIDS:
-                        pid = d["product_id"]
+                for d in devs.values():
+                    if d.get("product", None) in LEN_PIDS:
+                        pid = d["product"]
                         controller_mode = LEN_PIDS[pid]
                         break
                 else:
                     logger.error(
                         f"Legion go controllers not found, waiting {ERROR_DELAY}s."
                     )
-                    time.sleep(ERROR_DELAY)
+                    time.sleep(FIND_DELAY)
                     continue
 
             conf_copy = conf.copy()
             updated.clear()
             if (
                 controller_mode == "xinput"
                 and conf["xinput.mode"].to(str) != "disabled"
             ):
                 logger.info("Launching emulated controller.")
                 if gyro_fixer:
                     gyro_fixer.open()
+                init = time.perf_counter()
                 controller_loop_xinput(conf_copy, should_exit, updated, emit, reset)
             else:
                 if controller_mode != "xinput":
                     logger.info(
                         f"Controllers in non-supported (yet) mode: {controller_mode}."
                     )
                 else:
                     logger.info(
                         f"Controllers in xinput mode but emulation is disabled."
                     )
+                init = time.perf_counter()
                 controller_loop_rest(
                     controller_mode,
                     pid if pid else 2,
                     conf_copy,
                     should_exit,
                     updated,
                     emit,
                     reset,
                 )
+            repeated_fail = False
         except Exception as e:
+            failed_fast = init + LONGER_ERROR_MARGIN > time.perf_counter()
+            sleep_time = (
+                LONGER_ERROR_DELAY if repeated_fail and failed_fast else ERROR_DELAY
+            )
+            repeated_fail = failed_fast
             logger.error(f"Received the following error:\n{type(e)}: {e}")
             logger.error(
-                f"Assuming controllers disconnected, restarting after {ERROR_DELAY}s."
+                f"Assuming controllers disconnected, restarting after {sleep_time}s."
             )
             # Raise exception
             if conf.get("debug", False):
                 raise e
-            time.sleep(ERROR_DELAY)
+            time.sleep(sleep_time)
         finally:
             if gyro_fixer:
                 gyro_fixer.close()
         reset = False
 
 
 def controller_loop_rest(
@@ -234,15 +248,15 @@
         and conf["touchpad.mode"].to(TouchpadAction) == "controller"
     )
     motion = dimu != "disabled" or (
         dimu == "display"
         and (conf["imu.display.accel"].to(bool) or conf["imu.display.gyro"].to(bool))
     )
     d_producers, d_outs, d_params = get_outputs(
-        conf["xinput"], conf["touchpad"], motion, controller_id=cidx
+        conf["xinput"], conf["touchpad"], motion, controller_id=cidx, emit=emit
     )
 
     # Imu
     d_accel = AccelImu()
     # Legion go has a bit lower sensitivity than it should
     GYRO_MAPPINGS: dict[str, tuple[Axis, str | None, float, float | None]] = {
         "anglvel_x": (
@@ -336,14 +350,15 @@
         touchpad_short=touch_actions["short"].to(TouchpadAction),
         touchpad_right=touch_actions["hold"].to(TouchpadAction),
         select_reboots=conf["select_reboots"].to(bool),
         r3_to_share=conf["m2_to_mute"].to(bool),
         nintendo_mode=conf["nintendo_mode"].to(bool),
         emit=emit,
         imu=simu,
+        params=d_params,
     )
 
     d_right = UInputDevice(
         name="Handheld Daemon Controller Right Motion Sensors",
         phys="phys-hhd-main",
         capabilities=MOTION_CAPABILITIES,
         pid=HHD_PID_MOTION,
@@ -468,15 +483,15 @@
                 time.sleep(REPORT_DELAY_MIN - elapsed)
 
     except KeyboardInterrupt:
         raise
     finally:
         for d in reversed(devs):
             try:
-                d.close(True)
+                d.close(not updated.is_set())
             except Exception as e:
                 logger.error(f"Error while closing device '{d}' with exception:\n{e}")
                 if debug:
                     raise e
 
 
 class SelectivePassthrough(Producer, Consumer):
```

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/const.py` & `hhd-2.5.0/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/controllers.yml` & `hhd-2.5.0/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.5.0/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/legion_go/hid.py` & `hhd-2.5.0/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/orange_pi/__init__.py` & `hhd-2.5.0/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/orange_pi/base.py` & `hhd-2.5.0/src/hhd/device/orange_pi/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     debug = conf.get("debug", False)
 
     # Output
     d_producers, d_outs, d_params = get_outputs(
         conf["controller_mode"],
         None,
         conf["imu"].to(bool),
+        emit=emit,
     )
 
     # Imu
     d_imu = CombinedImu(
         conf["imu_hz"].to(int),
         get_gyro_state(conf["imu_axis"], dconf.get("mapping", DEFAULT_MAPPINGS)),
     )
@@ -128,14 +129,15 @@
 
     multiplexer = Multiplexer(
         trigger="analog_to_discrete",
         dpad="analog_to_discrete",
         share_to_qam=conf["share_to_qam"].to(bool),
         nintendo_mode=conf["nintendo_mode"].to(bool),
         emit=emit,
+        params=d_params,
     )
 
     # d_volume_btn = UInputDevice(
     #     name="Handheld Daemon Volume Keyboard",
     #     phys="phys-hhd-vbtn",
     #     capabilities={EC("EV_KEY"): [EC("KEY_VOLUMEUP"), EC("KEY_VOLUMEDOWN")]},
     #     btn_map={
@@ -225,21 +227,21 @@
             elapsed = t - start
             if elapsed < REPORT_DELAY_MIN:
                 time.sleep(REPORT_DELAY_MIN - elapsed)
 
     except KeyboardInterrupt:
         raise
     finally:
-        # d_vend.close(True)
+        # d_vend.close(not updated.is_set())
         try:
             d_timer.close()
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         for d in reversed(devs):
             try:
-                d.close(True)
+                d.close(not updated.is_set())
             except Exception as e:
                 logger.error(f"Error while closing device '{d}' with exception:\n{e}")
                 if debug:
                     raise e
```

### Comparing `hhd-2.4.2/src/hhd/device/orange_pi/const.py` & `hhd-2.5.0/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.5.0/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/rog_ally/__init__.py` & `hhd-2.5.0/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/rog_ally/base.py` & `hhd-2.5.0/src/hhd/device/rog_ally/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import logging
 import select
 import time
 from threading import Event as TEvent
 from typing import Literal, Sequence
 
 from hhd.controller import Axis, Event, Multiplexer, can_read
-from hhd.controller.base import Event
-from hhd.controller.lib.common import AM, BM, CM
-from hhd.controller.lib.hid import MAX_REPORT_SIZE
 from hhd.controller.physical.evdev import B as EC
-from hhd.controller.physical.evdev import GenericGamepadEvdev
-from hhd.controller.physical.hidraw import EventCallback, GenericGamepadHidraw
+from hhd.controller.physical.evdev import GenericGamepadEvdev, enumerate_evs
+from hhd.controller.physical.hidraw import GenericGamepadHidraw
 from hhd.controller.physical.imu import CombinedImu, HrtimerTrigger
 from hhd.plugins import Config, Context, Emitter, get_outputs
 
-from .hid import RgbCallback, switch_mode, Brightness
+from .hid import Brightness, RgbCallback, switch_mode
 
-ERROR_DELAY = 1
 SELECT_TIMEOUT = 1
 
 logger = logging.getLogger(__name__)
 
 ASUS_VID = 0x0B05
 ASUS_KBD_PID = 0x1ABE
 GAMEPAD_VID = 0x045E
@@ -47,14 +43,19 @@
 VIBRATION_OFF: Event = {
     "type": "rumble",
     "code": "main",
     "strong_magnitude": 0,
     "weak_magnitude": 0,
 }
 
+FIND_DELAY = 0.1
+ERROR_DELAY = 0.3
+LONGER_ERROR_DELAY = 3
+LONGER_ERROR_MARGIN = 1.3
+
 
 class AllyHidraw(GenericGamepadHidraw):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def open(self) -> Sequence[int]:
         self.queue: list[tuple[Event, float]] = []
@@ -129,36 +130,56 @@
 
         return out
 
 
 def plugin_run(
     conf: Config, emit: Emitter, context: Context, should_exit: TEvent, updated: TEvent
 ):
+    init = time.perf_counter()
+    repeated_fail = False
     while not should_exit.is_set():
         try:
+            first = True
+            while True:
+                gamepad_devs = enumerate_evs(vid=GAMEPAD_VID)
+                asus_devs = enumerate_evs(vid=ASUS_VID)
+                if not gamepad_devs or not asus_devs:
+                    if first:
+                        first = False
+                        logger.warning(f"Ally controller not found, waiting...")
+                    time.sleep(FIND_DELAY)
+                else:
+                    break
             logger.info("Launching emulated controller.")
             updated.clear()
+            init = time.perf_counter()
             controller_loop(conf.copy(), should_exit, updated, emit)
+            repeated_fail = False
         except Exception as e:
+            failed_fast = init + LONGER_ERROR_MARGIN > time.perf_counter()
+            sleep_time = (
+                LONGER_ERROR_DELAY if repeated_fail and failed_fast else ERROR_DELAY
+            )
+            repeated_fail = failed_fast
             logger.error(f"Received the following error:\n{type(e)}: {e}")
             logger.error(
-                f"Assuming controllers disconnected, restarting after {ERROR_DELAY}s."
+                f"Assuming controllers disconnected, restarting after {sleep_time}s."
             )
             # Raise exception
             if conf.get("debug", False):
                 raise e
-            time.sleep(ERROR_DELAY)
+            time.sleep(sleep_time)
 
 
 def controller_loop(conf: Config, should_exit: TEvent, updated: TEvent, emit: Emitter):
     debug = conf.get("debug", False)
 
     # Output
     d_producers, d_outs, d_params = get_outputs(
-        conf["controller_mode"], None, conf["imu"].to(bool)
+        conf["controller_mode"], None, conf["imu"].to(bool), emit=emit
     )
 
     # Imu
     d_imu = CombinedImu(conf["imu_hz"].to(int), ALLY_MAPPINGS, gyro_scale="0.000266")
     d_timer = HrtimerTrigger(conf["imu_hz"].to(int), [HrtimerTrigger.IMU_NAMES])
 
     # Inputs
@@ -195,14 +216,15 @@
         trigger="analog_to_discrete",
         dpad="analog_to_discrete",
         share_to_qam=conf["share_to_qam"].to(bool),
         select_reboots=conf["select_reboots"].to(bool),
         nintendo_mode=conf["nintendo_mode"].to(bool),
         emit=emit,
         swap_guide="select_is_guide" if conf["swap_armory"].to(bool) else None,
+        params=d_params,
     )
 
     REPORT_FREQ_MIN = 25
     REPORT_FREQ_MAX = 400
 
     if conf["imu"].to(bool):
         REPORT_FREQ_MAX = max(REPORT_FREQ_MAX, conf["imu_hz"].to(float))
@@ -272,25 +294,25 @@
             if elapsed < REPORT_DELAY_MIN:
                 time.sleep(REPORT_DELAY_MIN - elapsed)
 
     except KeyboardInterrupt:
         raise
     finally:
         try:
-            d_vend.close(True)
+            d_vend.close(not updated.is_set())
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         try:
             d_timer.close()
         except Exception as e:
             logger.error(f"Error while closing device '{d}' with exception:\n{e}")
             if debug:
                 raise e
         for d in reversed(devs):
             try:
-                d.close(True)
+                d.close(not updated.is_set())
             except Exception as e:
                 logger.error(f"Error while closing device '{d}' with exception:\n{e}")
                 if debug:
                     raise e
```

### Comparing `hhd-2.4.2/src/hhd/device/rog_ally/const.py` & `hhd-2.5.0/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.5.0/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/device/rog_ally/hid.py` & `hhd-2.5.0/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/http/api.py` & `hhd-2.5.0/src/hhd/http/api.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/http/index.html` & `hhd-2.5.0/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/http/static/index.js` & `hhd-2.5.0/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/logging.py` & `hhd-2.5.0/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/__init__.py` & `hhd-2.5.0/src/hhd/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/conf.py` & `hhd-2.5.0/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/display/__init__.py` & `hhd-2.5.0/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/gyro.yml` & `hhd-2.5.0/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/inputs.py` & `hhd-2.5.0/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/outputs.py` & `hhd-2.5.0/src/hhd/plugins/outputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Any, Mapping, Sequence
 
 from ..controller.base import Consumer, Producer
 from ..controller.virtual.dualsense import Dualsense, TouchpadCorrectionType
 from ..controller.virtual.uinput import (
     HHD_PID_MOTION,
     HHD_PID_TOUCHPAD,
@@ -9,36 +10,52 @@
     MOTION_CAPABILITIES,
     MOTION_INPUT_PROPS,
     TOUCHPAD_AXIS_MAP,
     TOUCHPAD_BUTTON_MAP,
     TOUCHPAD_CAPABILITIES,
     UInputDevice,
 )
+from .plugin import is_steam_gamepad_running
 from .utils import load_relative_yaml
 
+logger = logging.getLogger(__name__)
+
 
 def get_outputs(
-    conf, touch_conf, motion: bool = False, *, controller_id: int = 0
+    conf, touch_conf, motion: bool = False, *, controller_id: int = 0, emit=None
 ) -> tuple[Sequence[Producer], Sequence[Consumer], Mapping[str, Any]]:
     producers = []
     consumers = []
 
     controller = conf["mode"].to(str)
+    desktop_disable = False
     if touch_conf is not None:
         touchpad = touch_conf["mode"].to(str)
         correction = touch_conf["controller.correction"].to(TouchpadCorrectionType)
+        if touchpad in ("emulation", "controller"):
+            desktop_disable = touch_conf[touchpad]["desktop_disable"].to(bool)
     else:
         touchpad = "controller"
         correction = "stretch"
 
+    # Run steam check for touchpad
+    steam_check = (
+        is_steam_gamepad_running(emit.ctx) if emit and desktop_disable else None
+    )
+    match steam_check:
+        case True:
+            logger.info("Gamepadui active. Launching touchpad emulation.")
+        case False:
+            logger.info("Gamepadui closed. Activating touchpad emulation.")
+
     uses_touch = False
     uses_leds = False
     match controller:
         case "dualsense_edge":
-            uses_touch = touchpad == "controller"
+            uses_touch = touchpad == "controller" and steam_check is not False
             uses_leds = conf.get("dualsense_edge.led_support", False)
             d = Dualsense(
                 touchpad_method=correction,
                 edge_mode=True,
                 use_bluetooth=conf["dualsense_edge.bluetooth_mode"].to(bool),
                 enable_touchpad=uses_touch,
                 enable_rgb=uses_leds,
@@ -47,15 +64,15 @@
                 paddles_to_clicks=False,
                 flip_z=conf["dualsense_edge.flip_z"].to(bool),
                 controller_id=controller_id,
             )
             producers.append(d)
             consumers.append(d)
         case "dualsense":
-            uses_touch = touchpad == "controller"
+            uses_touch = touchpad == "controller" and steam_check is not False
             uses_leds = conf.get("dualsense.led_support", False)
             d = Dualsense(
                 touchpad_method=correction,
                 edge_mode=False,
                 use_bluetooth=conf["dualsense.bluetooth_mode"].to(bool),
                 enable_touchpad=uses_touch,
                 enable_rgb=uses_leds,
@@ -77,22 +94,22 @@
                     phys="phys-hhd-main",
                     capabilities=MOTION_CAPABILITIES,
                     pid=HHD_PID_MOTION,
                     btn_map={},
                     axis_map=MOTION_AXIS_MAP,
                     output_imu_timestamps=True,
                     input_props=MOTION_INPUT_PROPS,
-                    ignore_cmds=True
+                    ignore_cmds=True,
                 )
                 producers.append(d)
                 consumers.append(d)
         case _:
             raise RuntimeError(f"Invalid controller type: '{controller}'.")
 
-    if touchpad == "emulation":
+    if touchpad == "emulation" and steam_check is not False:
         d = UInputDevice(
             name="Handheld Daemon Touchpad",
             phys="phys-hhd-main",
             capabilities=TOUCHPAD_CAPABILITIES,
             pid=HHD_PID_TOUCHPAD,
             btn_map=TOUCHPAD_BUTTON_MAP,
             axis_map=TOUCHPAD_AXIS_MAP,
@@ -102,15 +119,21 @@
         producers.append(d)
         consumers.append(d)
         uses_touch = True
 
     return (
         producers,
         consumers,
-        {"uses_touch": uses_touch, "uses_leds": uses_leds, "is_dual": False},
+        {
+            "uses_touch": uses_touch,
+            "uses_leds": uses_leds,
+            "is_dual": False,
+            "steam_check": steam_check,
+            "steam_check_fn": lambda: emit and is_steam_gamepad_running(emit.ctx),
+        },
     )
 
 
 def get_outputs_config(
     can_disable: bool = False,
     has_leds: bool = True,
     start_disabled: bool = False,
```

### Comparing `hhd-2.4.2/src/hhd/plugins/outputs.yml` & `hhd-2.5.0/src/hhd/plugins/outputs.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/overlay/__init__.py` & `hhd-2.5.0/src/hhd/plugins/overlay/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,19 @@
     def open(
         self,
         emit,
         context: Context,
     ):
         try:
             from .base import OverlayService
+            from .x11 import QamHandler
 
             self.ovf = OverlayService(context, emit)
+            self.qam_handler = QamHandler(context)
+            emit.register_qam(self.qam_handler)
         except Exception as e:
             logger.warning(
                 f"Could not init overlay service, is python-xlib installed? Error:\n{e}"
             )
             self.ovf = None
 
     def settings(self):
@@ -77,14 +80,16 @@
                 if init:
                     logger.info(f"Executing overlay command: '{cmd}'")
                 self.ovf.update(cmd, init)
 
     def close(self):
         if self.ovf:
             self.ovf.close()
+        if self.qam_handler:
+            self.qam_handler.close()
 
 
 def autodetect(existing: Sequence[HHDPlugin]) -> Sequence[HHDPlugin]:
     if len(existing):
         return existing
 
     return [OverlayPlugin()]
```

### Comparing `hhd-2.4.2/src/hhd/plugins/overlay/base.py` & `hhd-2.5.0/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/overlay/controllers.py` & `hhd-2.5.0/src/hhd/plugins/overlay/controllers.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/overlay/overlay.py` & `hhd-2.5.0/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/overlay/x11.py` & `hhd-2.5.0/src/hhd/plugins/overlay/x11.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,96 @@
 import subprocess
 import time
 from select import select
 from threading import Event as TEvent
 from typing import Any, NamedTuple, Sequence
 
 import Xlib
-from Xlib import X, Xatom, display, error
+from Xlib import XK, X, Xatom, display, error
+from Xlib.ext.xtest import fake_input
 
-from hhd.utils import switch_priviledge, restore_priviledge
 from hhd.plugins import Emitter
+from hhd.utils import restore_priviledge, switch_priviledge
 
 logger = logging.getLogger(__name__)
 
 X11_DIR = b"/tmp/.X11-unix/"
 
 
 class CachedValues(NamedTuple):
     overlay: bool
     focus: bool
     notify: bool
     touch: int | None
 
 
+class QamHandler:
+
+    def __init__(self, ctx=None) -> None:
+        self.disp = None
+        self.ctx = ctx
+
+    def _register_display(self):
+        self.close()
+        try:
+            res = get_overlay_display(get_gamescope_displays(), self.ctx)
+            if not res:
+                logger.info(
+                    f"Could not find gamescope display, sending compatibility QAM."
+                )
+                return False
+            self.disp, name = res
+            logger.info(f"Registering display {name} to send QAM events to.")
+            return True
+        except Exception as e:
+            logger.info(f"Error while registering Gamescope display for QAM:\n{e}.")
+            return False
+
+    def _send_qam(self, expanded=False):
+        try:
+            disp = self.disp
+            if not disp:
+                return False
+            get_key = lambda k: disp.keysym_to_keycode(XK.string_to_keysym(k))
+            KCTRL = get_key("Control_L")
+            KEY = get_key("1" if expanded else "2")
+
+            steam = find_steam(disp)
+            if not steam:
+                logger.info(f"Could not find Steam (?). Sending compatibility QAM.")
+                return False
+
+            fake_input(disp, X.KeyPress, KCTRL, root=steam)
+            fake_input(disp, X.KeyPress, KEY, root=steam)
+            disp.sync()
+            fake_input(disp, X.KeyRelease, KCTRL, root=steam)
+            fake_input(disp, X.KeyRelease, KEY, root=steam)
+            disp.sync()
+            logger.info(f"Sent QAM event directly to gamescope.")
+            return True
+        except Exception as e:
+            logger.warning(
+                f"Could not send QAM to Gamescope with error:\n{e}\nSending compatibility QAM."
+            )
+            return False
+
+    def __call__(self, expanded=False) -> Any:
+        if self._send_qam(expanded):
+            return True
+        return self._register_display() and self._send_qam(expanded)
+
+    def close(self):
+        if self.disp:
+            try:
+                self.disp.close()
+                self.disp = None
+            except Exception:
+                pass
+
+
 def get_gamescope_displays():
     """Returns X11 UNIX sockets from gamescope opened under /tmp"""
     files = subprocess.run(["lsof", "-c", "gamescope-wl", "-Fn"], capture_output=True)
     out = []
     for ln in files.stdout.splitlines():
         if len(ln) < 1:
             continue
@@ -231,21 +296,20 @@
 
     hhd.change_property(stat_focus, Xatom.CARDINAL, 32, [1])
     hhd.change_property(stat_overlay, Xatom.CARDINAL, 32, [1])
     steam.change_property(stat_focus, Xatom.CARDINAL, 32, [0])
     steam.change_property(stat_overlay, Xatom.CARDINAL, 32, [0])
     steam.change_property(stat_notify, Xatom.CARDINAL, 32, [0])
 
-    # Give it a bit of time before setting the touch target to avoid steam
-    # messing with it
-    display.flush()
-    display.sync()
-    time.sleep(0.1)
-
     if touch_was_set:
+        # Give it a bit of time before setting the touch target to avoid steam
+        # messing with it
+        display.flush()
+        display.sync()
+        time.sleep(0.2)
         r.change_property(stat_click, Xatom.CARDINAL, 32, [TARGET_TOUCH])
 
     display.flush()
     display.sync()
 
 
 def hide_hhd(display, hhd, steam, old: CachedValues | None):
```

### Comparing `hhd-2.4.2/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.5.0/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/powerbutton/base.py` & `hhd-2.5.0/src/hhd/plugins/powerbutton/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,53 +3,30 @@
 import select
 import subprocess
 from threading import Event
 from time import perf_counter, sleep
 from typing import cast
 
 import evdev
-from evdev import ecodes as e
 
-from hhd.utils import Context, expanduser
+from hhd.utils import Context, expanduser, is_steam_gamepad_running
 
 from .const import PowerButtonConfig
 
 logger = logging.getLogger(__name__)
 
-STEAM_PID = "~/.steam/steam.pid"
 STEAM_EXE = "~/.steam/root/ubuntu12_32/steam"
 STEAM_WAIT_DELAY = 0.5
 LONG_PRESS_DELAY = 2.0
 
 
 def B(b: str):
     return cast(int, getattr(evdev.ecodes, b))
 
 
-def is_steam_gamescope_running(ctx: Context):
-    pid = None
-    try:
-        with open(expanduser(STEAM_PID, ctx)) as f:
-            pid = f.read().strip()
-
-        steam_cmd_path = f"/proc/{pid}/cmdline"
-        if not os.path.exists(steam_cmd_path):
-            return False
-
-        # Use this and line to determine if Steam is running in DeckUI mode.
-        with open(steam_cmd_path, "rb") as f:
-            steam_cmd = f.read()
-        is_deck_ui = b"-gamepadui" in steam_cmd
-        if not is_deck_ui:
-            return False
-    except Exception as e:
-        return False
-    return True
-
-
 def run_steam_command(command: str, ctx: Context):
     global home_path
     try:
         if ctx.euid != ctx.uid:
             result = subprocess.run(
                 [
                     "su",
@@ -136,28 +113,28 @@
 def power_button_isa(cfg: PowerButtonConfig, perms: Context, should_exit: Event):
     press_dev = None
     press_devs = []
     hold_dev = None
     try:
         while not should_exit.is_set():
             # Initial check for steam
-            if not is_steam_gamescope_running(perms):
+            if not is_steam_gamepad_running(perms):
                 # Close devices
                 if press_devs:
                     for d in press_devs:
                         d.close()
                     press_devs = []
                 if press_dev:
                     press_dev.close()
                     press_dev = None
                 if hold_dev:
                     hold_dev.close()
                     hold_dev = None
                 logger.info(f"Waiting for steam to launch.")
-                while not is_steam_gamescope_running(perms):
+                while not is_steam_gamepad_running(perms):
                     if should_exit.is_set():
                         return
                     sleep(STEAM_WAIT_DELAY)
 
             if not press_dev or not hold_dev:
                 logger.info(f"Steam is running, hooking power button.")
                 press_devs = register_power_buttons(cfg)
@@ -206,25 +183,25 @@
 def power_button_timer(cfg: PowerButtonConfig, perms: Context, should_exit: Event):
     dev = None
     devs = []
     try:
         pressed_time = None
         while not should_exit.is_set():
             # Initial check for steam
-            if not is_steam_gamescope_running(perms):
+            if not is_steam_gamepad_running(perms):
                 # Close devices
                 if devs:
                     for d in devs:
                         d.close()
                         devs = []
                     if dev:
                         dev.close()
                         dev = None
                 logger.info(f"Waiting for steam to launch.")
-                while not is_steam_gamescope_running(perms):
+                while not is_steam_gamepad_running(perms):
                     if should_exit.is_set():
                         return
                     sleep(STEAM_WAIT_DELAY)
 
             if not dev:
                 logger.info(f"Steam is running, hooking power button.")
                 devs = register_power_buttons(cfg)
```

### Comparing `hhd-2.4.2/src/hhd/plugins/powerbutton/const.py` & `hhd-2.5.0/src/hhd/plugins/powerbutton/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/settings.py` & `hhd-2.5.0/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/plugins/touchpad.yml` & `hhd-2.5.0/src/hhd/plugins/touchpad.yml`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,29 @@
   # Virtual emulation
   #
   emulation:
     type: container
     title: Virtual
     tags: [non-essential]
     hint: >-
-      Adds an emulated touchpad. This touchpad is meant to be for desktop
-      use and has left, right click support by default, within gamescope and
-      outside of it, regardless of the "Tap to Click" setting.
+      Adds an emulated touchpad. This touchpad is meant for use in gamescope
+      and has left, right click support by default.
+      However, it causes issues in desktop mode, and it doesnt allow dragging
+      files. Therefore, it will autodisable in desktop.
+      
     children:
+      desktop_disable:
+        type: bool
+        title: Disable on Desktop
+        hint: >-
+          Touchpad emulation will automatically be disabled when not in gamemode.
+          Specifically, steam will be periodically be checked to be running in
+          gamepad mode and if not, touchpad emulation will be disabled.
+        default: True
+
       short:
         type: multiple
         title: Short Action
         tags: [advanced]
         hint: >-
           Maps short touches (less than 0.2s) to a virtual touchpad button.
         options:
@@ -60,14 +71,23 @@
     tags: [non-essential]
     hint: >-
       Uses the touchpad of the emulated controller (if it exists).
       Otherwise, the touchpad remains unmapped (will still show up in the system).
       Meant to be used as steam input, so short press is unassigned by
       default and long press simulates trackpad click.
     children:
+      desktop_disable:
+        type: bool
+        title: Disable on Desktop
+        hint: >-
+          Touchpad emulation will automatically be disabled when not in gamemode.
+          Specifically, steam will be periodically be checked to be running in
+          gamepad mode and if not, touchpad emulation will be disabled.
+        default: True
+
       correction:
         type: multiple
         title: Location
         hint: >-
           Controls the placement of the real touchpad to the virtual one, using
           what steam expects. In Steam, the "Left" touchpad maps to the left
           half, the "Right" touchpad maps to the right half, and "Center" maps
```

### Comparing `hhd-2.4.2/src/hhd/plugins/utils.py` & `hhd-2.5.0/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd/settings.yml` & `hhd-2.5.0/src/hhd/settings.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/src/hhd.egg-info/PKG-INFO` & `hhd-2.5.0/src/hhd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.4.2
+Version: 2.5.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -91,15 +91,15 @@
   - Air Standard/Plus/Pro
   - 1S/1S Limited
   - 2/2S 
   - GEEK, GEEK 1S 
   - NEXT Lite/Pro/Advance
   - SLIDE
 - Ayn
-  - Loki Max
+  - Loki Zero/Max
 - AOKZOE
   - A1
   - A1 Pro 
 - Onexplayer
   - Mini Pro
 
 In addition, Handheld Daemon will attempt to work on Ayaneo, Ayn, Onexplayer, and
```

### Comparing `hhd-2.4.2/src/hhd.egg-info/SOURCES.txt` & `hhd-2.5.0/src/hhd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.5.0/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.5.0/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.4.2/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.5.0/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

