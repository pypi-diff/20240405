# Comparing `tmp/lockhart-serial-0.0.1.tar.gz` & `tmp/lockhart_serial-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart-serial-0.0.1.tar", last modified: Wed Feb 28 22:02:40 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lockhart-serial-0.0.1.tar` & `lockhart_serial-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,10 @@
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
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/.gitattributes
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/pyvenv.cfg
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/lockhart_serial/__init__.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/lockhart_serial/lockhart_serial.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 lockhart_serial-1.0.8/PKG-INFO
```

