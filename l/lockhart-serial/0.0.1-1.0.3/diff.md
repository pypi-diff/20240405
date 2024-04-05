# Comparing `tmp/lockhart-serial-0.0.1.tar.gz` & `tmp/lockhart_serial-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart-serial-0.0.1.tar", last modified: Wed Feb 28 22:02:40 2024, max compression
+gzip compressed data, was "lockhart_serial-1.0.3.tar", last modified: Fri Apr  5 02:10:13 2024, max compression
```

## Comparing `lockhart-serial-0.0.1.tar` & `lockhart_serial-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.373039 lockhart-serial-0.0.1/
--rw-rw-rw-   0        0        0      510 2024-02-28 22:02:40.372066 lockhart-serial-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-28 21:58:53.000000 lockhart-serial-0.0.1/README.md
--rw-rw-rw-   0        0        0      611 2024-02-28 22:02:34.000000 lockhart-serial-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 22:02:40.373039 lockhart-serial-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.356036 lockhart-serial-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.359036 lockhart-serial-0.0.1/src/lockhart-serial/
--rw-rw-rw-   0        0        0        0 2024-02-28 21:55:36.000000 lockhart-serial-0.0.1/src/lockhart-serial/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 21:56:01.000000 lockhart-serial-0.0.1/src/lockhart-serial/lockhart_serial.py
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.371039 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/
--rw-rw-rw-   0        0        0      510 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/lockhart-serial/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/lockhart-serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/lockhart-serial/lockhart_serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/lockhart_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:10:13.000000 lockhart_serial-1.0.3/lockhart_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:10:08.000000 lockhart_serial-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:10:13.154410 lockhart_serial-1.0.3/setup.cfg
```

