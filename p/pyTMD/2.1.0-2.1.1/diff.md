# Comparing `tmp/pyTMD-2.1.0.tar.gz` & `tmp/pyTMD-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTMD-2.1.0.tar", last modified: Sat Jan 13 22:25:51 2024, max compression
+gzip compressed data, was "pyTMD-2.1.1.tar", last modified: Thu Apr  4 23:36:01 2024, max compression
```

## Comparing `pyTMD-2.1.0.tar` & `pyTMD-2.1.1.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.624826 pyTMD-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-13 22:25:40.000000 pyTMD-2.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-13 22:25:40.000000 pyTMD-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-01-13 22:25:40.000000 pyTMD-2.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-13 22:25:40.000000 pyTMD-2.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-13 22:25:40.000000 pyTMD-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-13 22:25:40.000000 pyTMD-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-01-13 22:25:51.624826 pyTMD-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-01-13 22:25:40.000000 pyTMD-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-13 22:25:40.000000 pyTMD-2.1.0/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.612826 pyTMD-2.1.0/pyTMD/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37955 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    44771 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/astro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/calc_astrol_longitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/check_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    42787 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/compute_tide_corrections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13435 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/convert_crs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/convert_ll_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.620826 pyTMD-2.1.0/pyTMD/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12369 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (127)  3580648 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/finals.all
--rwxr-xr-x   0 runner    (1001) docker     (127)    30345 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (127)   130160 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (127)    10666 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    79072 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/mean-pole.tab
--rwxr-xr-x   0 runner    (1001) docker     (127)   159160 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (127)  6325011 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/opoleloadcoefcmcor.txt.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    33782 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/tab5.2e.txt
--rw-r--r--   0 runner    (1001) docker     (127)   145678 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/tab5.3a.txt
--rw-r--r--   0 runner    (1001) docker     (127)   113660 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/data/tab5.3b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/eop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.620826 pyTMD-2.1.0/pyTMD/io/
--rw-r--r--   0 runner    (1001) docker     (127)    44336 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/ATLAS.py
--rw-r--r--   0 runner    (1001) docker     (127)    32150 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/FES.py
--rw-r--r--   0 runner    (1001) docker     (127)    28478 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/GOT.py
--rw-r--r--   0 runner    (1001) docker     (127)    71125 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/OTIS.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/constituents.py
--rw-r--r--   0 runner    (1001) docker     (127)    72649 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/io/ocean_pole_tide.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/load_constituent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4828 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/load_nodal_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    42530 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    63070 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    60726 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    50621 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-01-13 22:25:40.000000 pyTMD-2.1.0/pyTMD/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.624826 pyTMD-2.1.0/pyTMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-01-13 22:25:51.000000 pyTMD-2.1.0/pyTMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-01-13 22:25:51.000000 pyTMD-2.1.0/pyTMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 22:25:51.000000 pyTMD-2.1.0/pyTMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-13 22:25:51.000000 pyTMD-2.1.0/pyTMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-13 22:25:51.000000 pyTMD-2.1.0/pyTMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-13 22:25:40.000000 pyTMD-2.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-13 22:25:40.000000 pyTMD-2.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:25:51.624826 pyTMD-2.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/arcticdata_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/aviso_fes_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_LPET_elevations.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_LPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_OPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_SET_displacements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24400 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_tidal_currents.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24605 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/compute_tidal_elevations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/reduce_OTIS_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/usap_cats_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-01-13 22:25:40.000000 pyTMD-2.1.0/scripts/verify_box_tpxo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 22:25:51.624826 pyTMD-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-13 22:25:40.000000 pyTMD-2.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-13 22:25:40.000000 pyTMD-2.1.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.400890 pyTMD-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-04 23:35:48.000000 pyTMD-2.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 23:35:48.000000 pyTMD-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-04 23:35:48.000000 pyTMD-2.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 23:35:48.000000 pyTMD-2.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 23:35:48.000000 pyTMD-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 23:35:48.000000 pyTMD-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-04 23:36:01.396890 pyTMD-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-04 23:35:48.000000 pyTMD-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 23:35:48.000000 pyTMD-2.1.1/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.384890 pyTMD-2.1.1/pyTMD/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43682 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47697 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/astro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/calc_astrol_longitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/check_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52596 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/compute_tide_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/convert_crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/convert_ll_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25710 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.392890 pyTMD-2.1.1/pyTMD/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12369 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)  3597756 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30345 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)   130160 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10666 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79520 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (127)   160700 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)  6325011 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/opoleloadcoefcmcor.txt.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34052 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/tab5.2e.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   145678 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/tab5.3a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   113660 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/data/tab5.3b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17526 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/eop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15241 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.396890 pyTMD-2.1.1/pyTMD/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    44418 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/ATLAS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/FES.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/GOT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72523 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/OTIS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/constituents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73614 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/io/ocean_pole_tide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/load_constituent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4828 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/load_nodal_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38904 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.396890 pyTMD-2.1.1/pyTMD/solve/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/solve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64055 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60382 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50621 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 23:35:48.000000 pyTMD-2.1.1/pyTMD/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.396890 pyTMD-2.1.1/pyTMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-04 23:36:01.000000 pyTMD-2.1.1/pyTMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-04 23:36:01.000000 pyTMD-2.1.1/pyTMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:36:01.000000 pyTMD-2.1.1/pyTMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 23:36:01.000000 pyTMD-2.1.1/pyTMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 23:36:01.000000 pyTMD-2.1.1/pyTMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 23:35:48.000000 pyTMD-2.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 23:35:48.000000 pyTMD-2.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:36:01.396890 pyTMD-2.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/arcticdata_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/aviso_fes_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_LPET_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_LPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22325 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_OPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20388 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_SET_displacements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25305 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_tidal_currents.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25442 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/compute_tidal_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/reduce_OTIS_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/usap_cats_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-04 23:35:48.000000 pyTMD-2.1.1/scripts/verify_box_tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:36:01.400890 pyTMD-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-04 23:35:48.000000 pyTMD-2.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 23:35:48.000000 pyTMD-2.1.1/version.txt
```

### Comparing `pyTMD-2.1.0/.gitignore` & `pyTMD-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/CODE_OF_CONDUCT.rst` & `pyTMD-2.1.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/CONTRIBUTORS.rst` & `pyTMD-2.1.1/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/LICENSE` & `pyTMD-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/PKG-INFO` & `pyTMD-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyTMD-2.1.0/README.rst` & `pyTMD-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/__init__.py` & `pyTMD-2.1.1/pyTMD/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,42 @@
 combined with data storage in netCDF4 and HDF5 and mapping using
 matplotlib and cartopy
 
 Documentation is available at https://pytmd.readthedocs.io
 """
 import pyTMD.arguments
 import pyTMD.astro
+import pyTMD.compute
+import pyTMD.ellipse
 import pyTMD.eop
 import pyTMD.interpolate
 import pyTMD.predict
-import pyTMD.solve
 import pyTMD.spatial
 import pyTMD.time
 import pyTMD.tools
 import pyTMD.utilities
 import pyTMD.version
 from pyTMD import io
+from pyTMD import solve
 from pyTMD.check_points import check_points
 from pyTMD.compute_tide_corrections import (
     compute_corrections,
     compute_tide_corrections,
     compute_LPET_corrections,
     compute_LPT_corrections,
     compute_OPT_corrections,
     compute_SET_corrections,
 )
-from pyTMD.constants import (
-    constants,
+from pyTMD.crs import (
+    crs,
+    datum,
     _ellipsoids
 )
-from pyTMD.convert_crs import convert_crs
-from pyTMD.crs import crs
-from pyTMD.ellipse import ellipse
 
 # Deprecated functions
 from pyTMD.calc_astrol_longitudes import calc_astrol_longitudes
+from pyTMD.convert_crs import convert_crs
 from pyTMD.convert_ll_xy import convert_ll_xy
 from pyTMD.load_nodal_corrections import load_nodal_corrections
 
 # get semantic version from setuptools-scm
 __version__ = pyTMD.version.version
```

### Comparing `pyTMD-2.1.0/pyTMD/arguments.py` & `pyTMD-2.1.1/pyTMD/arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,17 @@
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 UPDATE HISTORY:
     Updated 01/2024: add function to create arguments coefficients table
         add function to calculate the arguments for minor constituents
         include multiples of 90 degrees as variable following Ray 2017
         add function to calculate the Doodson numbers for constituents
+        add option to return None and not raise error for Doodson numbers
+        moved constituent parameters function from predict to arguments
+        added more constituent parameters for OTIS/ATLAS predictions
     Updated 12/2023: made keyword argument for selecting M1 coefficients
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 04/2023: using renamed astro mean_longitudes function
         function renamed from original load_nodal_corrections
     Updated 03/2023: add basic variable typing to function inputs
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 05/2022: added ESR netCDF4 formats to list of model types
@@ -91,17 +94,17 @@
 
                 - ``'Doodson'``
                 - ``'Ray'``
 
     Returns
     -------
     pu: np.ndarray
-        nodal correction for the constituent amplitude
+        nodal angle correction
     pf: np.ndarray
-        nodal correction for the constituent phase
+        nodal factor correction
     G: np.ndarray
         phase correction in degrees
 
     References
     ----------
     .. [1] A. T. Doodson and H. D. Warburg, "Admiralty Manual of Tides",
         HMSO, London, (1941).
@@ -156,20 +159,21 @@
     sinn = np.sin(n*dtr)
     cosn = np.cos(n*dtr)
     sin2n = np.sin(2.0*n*dtr)
     cos2n = np.cos(2.0*n*dtr)
     sin3n = np.sin(3.0*n*dtr)
 
     # set nodal corrections
-    # scale factor correction
+    # nodal factor correction
     f = np.zeros((nt, 60))
-    # phase correction
+    # nodal angle correction
     u = np.zeros((nt, 60))
     # determine nodal corrections f and u for each model type
     if kwargs['corrections'] in ('OTIS', 'ATLAS', 'TMD3', 'netcdf'):
+        # nodal factors
         f[:,0] = 1.0 # Sa
         f[:,1] = 1.0 # Ssa
         f[:,2] = 1.0 - 0.130*cosn # Mm
         f[:,3] = 1.0 # MSf
         f[:,4] = 1.043 + 0.414*cosn # Mf
         temp1 = (1.0 + 0.203*cosn + 0.040*cos2n)**2
         temp2 = (0.203*sinn + 0.040*sin2n)**2
@@ -249,14 +253,15 @@
         f[:,55] = f[:,4] # msqm
         f[:,56] = f[:,4] # mtm
         f[:,57] = f[:,29]**2 # n4
         f[:,58] = f[:,29] # eps2
         # mean sea level
         f[:,59] = 1.0 # Z0
 
+        # nodal angles
         u[:,0] = 0.0 # Sa
         u[:,1] = 0.0 # Ssa
         u[:,2] = 0.0 # Mm
         u[:,3] = 0.0 # MSf
         u[:,4] = -23.7*sinn + 2.7*sin2n - 0.4*sin3n # Mf
         temp1 = -(0.203*sinn + 0.040*sin2n)
         temp2 = (1.0 + 0.203*cosn + 0.040*cos2n)
@@ -335,14 +340,15 @@
         P_prime = np.sin(2.0*II)*np.sin(nu)
         Q_prime = np.sin(2.0*II)*np.cos(nu) + 0.3347
         nu_prime = np.arctan(P_prime/Q_prime)
         P_sec = (np.sin(II)**2)*np.sin(2.0*nu)
         Q_sec = (np.sin(II)**2)*np.cos(2.0*nu) + 0.0727
         nu_sec = 0.5*np.arctan(P_sec/Q_sec)
 
+        # nodal factors
         f[:,0] = 1.0 # Sa
         f[:,1] = 1.0 # Ssa
         f[:,2] = (2.0/3.0 - np.power(np.sin(II),2.0))/0.5021 # Mm
         f[:,3] = 1.0 # MSf
         f[:,4] = np.power(np.sin(II),2.0)/0.1578  # Mf
         f[:,7] = np.sin(II)*(np.cos(II/2.0)**2)/0.38 # 2Q1
         f[:,8] = f[:,7] # sigma1
@@ -407,14 +413,15 @@
         f[:,55] = f[:,4] # msqm
         f[:,56] = f[:,4] # mtm
         f[:,57] = f[:,29]**2 # n4
         f[:,58] = f[:,29] # eps2
         # mean sea level
         f[:,59] = 1.0 # Z0
 
+        # nodal angles
         u[:,0] = 0.0 # Sa
         u[:,1] = 0.0 # Ssa
         u[:,2] = 0.0 # Mm
         u[:,3] = (2.0*xi - 2.0*nu)/dtr # MSf
         u[:,4] = -2.0*xi/dtr # Mf
         u[:,7] = (2.0*xi - nu)/dtr # 2Q1
         u[:,8] = u[:,7] # sigma1
@@ -466,43 +473,45 @@
         u[:,56] = u[:,4] # mtm
         u[:,57] = (4.0*xi - 4.0*nu)/dtr # n4
         u[:,58] = u[:,29] # eps2
         # mean sea level
         u[:,59] = 0.0 # Z0
 
     elif kwargs['corrections'] in ('GOT',):
+        # nodal factors
         f[:,9] = 1.009 + 0.187*cosn - 0.015*cos2n# Q1
         f[:,11] = f[:,9]# O1
         f[:,16] = 1.0 # P1
         f[:,17] = 1.0 # S1
         f[:,18] = 1.006 + 0.115*cosn - 0.009*cos2n# K1
         f[:,26] = 1.000 - 0.037*cosn# N2
         f[:,29] = f[:,26]# M2
         f[:,34] = 1.0 # S2
         f[:,36] = 1.024 + 0.286*cosn + 0.008*cos2n# K2
         f[:,44] = f[:,29]**2# M4
 
+        # nodal angles
         u[:,9] = 10.8*sinn - 1.3*sin2n# Q1
         u[:,11] = u[:,9]# O1
         u[:,16] = 0.0 # P1
         u[:,17] = 0.0 # S1
         u[:,18] = -8.9*sinn + 0.7*sin2n# K1
         u[:,26] = -2.1*sinn# N2
         u[:,29] = u[:,26]# M2
         u[:,34] = 0.0 # S2
         u[:,36] = -17.7*sinn + 0.7*sin2n# K2
         u[:,44] = -4.2*sinn# M4
 
-    # take pu,pf,G for the set of given constituents
+    # number of constituents of interest
     nc = len(constituents)
-    # scale factor correction
+    # nodal factor corrections for given constituents
     pu = np.zeros((nt,nc))
-    # phase correction
+    # nodal angle corrections for given constituents
     pf = np.zeros((nt,nc))
-    # equilibrium arguments
+    # equilibrium arguments for given constituents
     G = np.zeros((nt,nc))
     for i,c in enumerate(constituents):
         # map between given constituents and supported in tidal program
         assert c.lower() in cindex, f'Unsupported constituent {c.lower()}'
         j, = [j for j,val in enumerate(cindex) if (val == c.lower())]
         pu[:,i] = u[:,j]*dtr
         pf[:,i] = f[:,j]
@@ -527,17 +536,17 @@
         time correction for converting to Ephemeris Time (days)
     corrections: str, default 'OTIS'
         use nodal corrections from OTIS/ATLAS or GOT models
 
     Returns
     -------
     pu: np.ndarray
-        nodal correction for the constituent amplitude
+        nodal angle correction
     pf: np.ndarray
-        nodal correction for the constituent phase
+        nodal factor correction
     G: np.ndarray
         phase correction in degrees
 
     References
     ----------
     .. [1] A. T. Doodson and H. D. Warburg, "Admiralty Manual of Tides",
         HMSO, London, (1941).
@@ -581,15 +590,15 @@
 
     # determine nodal corrections f and u
     sinn = np.sin(n*dtr)
     cosn = np.cos(n*dtr)
     sin2n = np.sin(2.0*n*dtr)
     cos2n = np.cos(2.0*n*dtr)
 
-    # scale factor corrections for minor constituents
+    # nodal factor corrections for minor constituents
     f = np.ones((nt, 20))
     f[:,0] = np.sqrt((1.0 + 0.189*cosn - 0.0058*cos2n)**2 +
         (0.189*sinn - 0.0058*sin2n)**2)# 2Q1
     f[:,1] = f[:,0]# sigma1
     f[:,2] = f[:,0]# rho1
     f[:,3] = np.sqrt((1.0 + 0.185*cosn)**2 + (0.185*sinn)**2)# M12
     f[:,4] = np.sqrt((1.0 + 0.201*cosn)**2 + (0.201*sinn)**2)# M11
@@ -599,15 +608,15 @@
         (0.640*sinn + 0.134*sin2n)**2)# OO1
     f[:,11] = np.sqrt((1.0 - 0.0373*cosn)**2 + (0.0373*sinn)**2)# 2N2
     f[:,12] = f[:,11]# mu2
     f[:,13] = f[:,11]# nu2
     f[:,15] = f[:,11]# L2
     f[:,16] = np.sqrt((1.0 + 0.441*cosn)**2 + (0.441*sinn)**2)# L2
 
-    # phase corrections for minor constituents
+    # nodal angle corrections for minor constituents
     u = np.zeros((nt, 20))
     u[:,0] = np.arctan2(0.189*sinn - 0.0058*sin2n,
         1.0 + 0.189*cosn - 0.0058*sin2n)/dtr# 2Q1
     u[:,1] = u[:,0]# sigma1
     u[:,2] = u[:,0]# rho1
     u[:,3] = np.arctan2( 0.185*sinn, 1.0 + 0.185*cosn)/dtr# M12
     u[:,4] = np.arctan2(-0.201*sinn, 1.0 + 0.201*cosn)/dtr# M11
@@ -631,15 +640,15 @@
         nu = at1 - at2
         I2 = np.tan(II/2.0)
         Ra1 = np.sqrt(1.0 - 12.0*(I2**2)*np.cos(2.0*(p - xi)) + 36.0*(I2**4))
         P2 = np.sin(2.0*(p - xi))
         Q2 = 1.0/(6.0*(I2**2)) - np.cos(2.0*(p - xi))
         R = np.arctan(P2/Q2)
 
-        # scale factor corrections for minor constituents
+        # nodal factor corrections for minor constituents
         f[:,0] = np.sin(II)*(np.cos(II/2.0)**2)/0.38 # 2Q1
         f[:,1] = f[:,0] # sigma1
         f[:,2] = f[:,0] # rho1
         f[:,3] = f[:,0] # M12
         f[:,4] = np.sin(2.0*II)/0.7214 # M11
         f[:,5] = f[:,4] # chi1
         f[:,9] = f[:,5] # J1
@@ -648,15 +657,15 @@
         f[:,12] = f[:,11] # mu2
         f[:,13] = f[:,11] # nu2
         f[:,14] = f[:,11] # lambda2
         f[:,15] = f[:,11]*Ra1 # L2
         f[:,18] = f[:,11] # eps2
         f[:,19] = np.power(np.sin(II),2.0)/0.1565 # eta2
 
-        # phase corrections for minor constituents
+        # nodal angle corrections for minor constituents
         u[:,0] = (2.0*xi - nu)/dtr # 2Q1
         u[:,1] = u[:,0] # sigma1
         u[:,2] = u[:,0] # rho1
         u[:,3] = u[:,0] # M12
         u[:,4] = -nu/dtr # M11
         u[:,5] = u[:,4] # chi1
         u[:,9] = u[:,4] # J1
@@ -687,14 +696,16 @@
     corrections: str, default 'OTIS'
         use arguments from OTIS/ATLAS or GOT models
     formalism: str, default 'Doodson'
         constituent identifier formalism
 
             - ``'Cartwright'``
             - ``'Doodson'``
+    raise_error: bool, default True
+        Raise exception if constituent is unsupported
 
     Returns
     -------
     numbers: float, np.ndarray or dict
         Doodson or Cartwright number for each constituent
 
     References
@@ -704,54 +715,63 @@
         of London. Series A, Containing Papers of a Mathematical and
         Physical Character*, 100(704), 305--329, (1921).
         `doi: 10.1098/rspa.1921.0088 <https://doi.org/10.1098/rspa.1921.0088>`_
     """
     # set default keyword arguments
     kwargs.setdefault('corrections', 'OTIS')
     kwargs.setdefault('formalism', 'Doodson')
+    kwargs.setdefault('raise_error', True)
     # validate inputs
     assert kwargs['formalism'].title() in ('Cartwright', 'Doodson'), \
         f'Unknown formalism {kwargs["formalism"]}'
 
     # constituents array (not all are included in tidal program)
     cindex = ['sa', 'ssa', 'mm', 'msf', 'mf', 'mt', 'alpha1', '2q1', 'sigma1',
         'q1', 'rho1', 'o1', 'tau1', 'm1', 'chi1', 'pi1', 'p1', 's1', 'k1',
         'psi1', 'phi1', 'theta1', 'j1', 'oo1', '2n2', 'mu2', 'n2', 'nu2', 'm2a',
         'm2', 'm2b', 'lambda2', 'l2', 't2', 's2', 'r2', 'k2', 'eta2', 'mns2',
         '2sm2', 'm3', 'mk3', 's3', 'mn4', 'm4', 'ms4', 'mk4', 's4', 's5', 'm6',
         's6', 's7', 's8', 'm8', 'mks2', 'msqm', 'mtm', 'n4', 'eps2', 'z0']
     # get the table of coefficients
     coefficients = _arguments_table(**kwargs)
     if isinstance(constituents, str):
+        # check that given constituents is supported in tidal program
+        if (constituents.lower() not in cindex) and kwargs['raise_error']:
+            raise ValueError(f'Unsupported constituent {constituents}')
+        elif (constituents.lower() not in cindex):
+            return None
         # map between given constituents and supported in tidal program
-        assert constituents.lower() in cindex, \
-            f'Unsupported constituent {constituents}'
         j, = [j for j,val in enumerate(cindex) if (val == constituents.lower())]
         # extract identifier in formalism
         if (kwargs['formalism'] == 'Cartwright'):
             # extract Cartwright number
             numbers = np.array(coefficients[:6,j])
         elif (kwargs['formalism'] == 'Doodson'):
             # convert from coefficients to Doodson number
-            numbers = _to_doodson_number(coefficients[:,j])
+            numbers = _to_doodson_number(coefficients[:,j], **kwargs)
     else:
         # output dictionary with Doodson numbers
         numbers = {}
         # for each input constituent
         for i,c in enumerate(constituents):
+            # check that given constituents is supported in tidal program
+            if (c.lower() not in cindex) and kwargs['raise_error']:
+                raise ValueError(f'Unsupported constituent {c}')
+            elif (c.lower() not in cindex):
+                numbers[c] = None
+                continue
             # map between given constituents and supported in tidal program
-            assert c.lower() in cindex, f'Unsupported constituent {c}'
             j, = [j for j,val in enumerate(cindex) if (val == c.lower())]
             # convert from coefficients to Doodson number
             if (kwargs['formalism'] == 'Cartwright'):
                 # extract Cartwright number
                 numbers[c] = np.array(coefficients[:6,j])
             elif (kwargs['formalism'] == 'Doodson'):
                 # convert from coefficients to Doodson number
-                numbers[c] = _to_doodson_number(coefficients[:,j])
+                numbers[c] = _to_doodson_number(coefficients[:,j], **kwargs)
     # return the Doodson or Cartwright number
     return numbers
 
 def _arguments_table(**kwargs):
     """
     Arguments table for tidal constituents [1]_ [2]_
 
@@ -904,35 +924,140 @@
     coef[:,16] = [2.0, 1.0, 0.0, 1.0, 0.0, 0.0, 0.0] # l2
     coef[:,17] = [2.0, 2.0, -3.0, 0.0, 0.0, 1.0, 0.0] # t2
     coef[:,18] = [2.0, -3.0, 2.0, 1.0, 0.0, 0.0, 0.0] # eps2
     coef[:,19] = [2.0, 3.0, 0.0, 0.0, 0.0, -1.0, 0.0] # eta2
     # return the coefficient table
     return coef
 
-def _to_doodson_number(coef: list | np.ndarray):
+def _constituent_parameters(c: str, **kwargs):
+    """
+    Loads parameters for a given tidal constituent
+
+    Parameters
+    ----------
+    c: str
+        tidal constituent ID
+    raise_error: bool, default False
+        Raise exception if constituent is unsupported
+
+    Returns
+    -------
+    amplitude: float
+        amplitude of equilibrium tide for tidal constituent (meters)
+    phase: float
+        phase of tidal constituent (radians)
+    omega: float
+        angular frequency of constituent (radians)
+    alpha: float
+        load love number of tidal constituent
+    species: float
+        spherical harmonic dependence of quadrupole potential
+
+    References
+    ----------
+    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
+        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
+        Technology*, 19(2), 183--204, (2002).
+        `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
+
+    .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
+    """
+    # default keyword arguments
+    kwargs.setdefault('raise_error', False)
+    # constituents array that are included in tidal program
+    cindex = ['m2', 's2', 'k1', 'o1', 'n2', 'p1', 'k2', 'q1', '2n2', 'mu2',
+        'nu2', 'l2', 't2', 'j1', 'm1', 'oo1', 'rho1', 'mf', 'mm', 'ssa',
+        'm4', 'ms4', 'mn4', 'm6', 'm8', 'mk3', 's6', '2sm2', '2mk3',
+        'msf', 'sa', 'mt', '2q1']
+    # species type (spherical harmonic dependence of quadrupole potential)
+    _species = np.array([2, 2, 1, 1, 2, 1, 2, 1, 2, 2, 2, 2, 2, 1, 1,
+        1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])
+    # Load Love numbers
+    # alpha = correction factor for first order load tides
+    _alpha = np.array([0.693, 0.693, 0.736, 0.695, 0.693, 0.706, 0.693,
+        0.695, 0.693, 0.693, 0.693, 0.693, 0.693, 0.695, 0.695, 0.695, 0.695,
+        0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693,
+        0.693, 0.693, 0.693, 0.693, 0.693, 0.693])
+    # omega: angular frequency of constituent, in radians
+    _omega = np.array([1.405189e-04, 1.454441e-04, 7.292117e-05, 6.759774e-05,
+        1.378797e-04, 7.252295e-05, 1.458423e-04, 6.495854e-05, 1.352405e-04,
+        1.355937e-04, 1.382329e-04, 1.431581e-04, 1.452450e-04, 7.556036e-05,
+        7.028195e-05, 7.824458e-05, 6.531174e-05, 0.053234e-04, 0.026392e-04,
+        0.003982e-04, 2.810377e-04, 2.859630e-04, 2.783984e-04, 4.215566e-04,
+        5.620755e-04, 2.134402e-04, 4.363323e-04, 1.503693e-04, 2.081166e-04,
+        4.925200e-06, 1.990970e-07, 7.962619e-06, 6.231934e-05])
+    # Astronomical arguments (relative to t0 = 1 Jan 0:00 1992)
+    # phases for each constituent are referred to the time when the phase of
+    # the forcing for that constituent is zero on the Greenwich meridian
+    _phase = np.array([1.731557546, 0.000000000, 0.173003674, 1.558553872,
+        6.050721243, 6.110181633, 3.487600001, 5.877717569, 4.086699633,
+        3.463115091, 5.427136701, 0.553986502, 0.052841931, 2.137025284,
+        2.436575100, 1.929046130, 5.254133027, 1.756042456, 1.964021610,
+        3.487600001, 3.463115091, 1.731557546, 1.499093481, 5.194672637,
+        6.926230184, 1.904561220, 0.000000000, 4.551627762, 3.809122439,
+        4.551627762, 6.232786837, 3.720064066, 3.91369596])
+    # amplitudes of equilibrium tide in meters
+    # _amplitude = np.array([0.242334,0.112743,0.141565,0.100661,0.046397,
+    _amplitude = np.array([0.2441, 0.112743, 0.141565, 0.100661, 0.046397,
+        0.046848, 0.030684, 0.019273, 0.006141, 0.007408, 0.008811, 0.006931,
+        0.006608, 0.007915, 0.007915, 0.004338, 0.003661, 0.042041, 0.022191,
+        0.019567, 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.003681, 0.003104,
+        0.008044, 0.002565])
+
+    # map between input constituent and cindex
+    j = [j for j,val in enumerate(cindex) if (val == c.lower())]
+    # set the values for the constituent
+    if j:
+        amplitude, = _amplitude[j]
+        phase, = _phase[j]
+        omega, = _omega[j]
+        alpha, = _alpha[j]
+        species, = _species[j]
+    elif kwargs['raise_error']:
+        raise ValueError(f'Unsupported constituent {c}')
+    else:
+        amplitude = 0.0
+        phase = 0.0
+        omega = 0.0
+        alpha = 0.0
+        species = 0
+    # return the values for the constituent
+    return (amplitude, phase, omega, alpha, species)
+
+def _to_doodson_number(coef: list | np.ndarray, **kwargs):
     """
     Converts Cartwright numbers into a Doodson number
 
     Parameters
     ----------
     coef: list or np.ndarray
         Doodson coefficients (Cartwright numbers) for constituent
+    raise_error: bool, default True
+        Raise exception if constituent is unsupported
 
     Returns
     -------
     DO: float
         Doodson number for constituent
     """
+    # default keyword arguments
+    kwargs.setdefault('raise_error', True)
     # assert length and verify array
     coef = np.array(coef[:6])
     # add 5 to values following Doodson convention (prevent negatives)
     coef[1:] += 5
-    # convert to single number and round off floating point errors
-    DO = np.sum([v*10**(2-o) for o,v in enumerate(coef)])
-    return np.round(DO, decimals=3)
+    # check for unsupported constituents
+    if (np.any(coef < 0) or np.any(coef > 10)) and kwargs['raise_error']:
+        raise ValueError('Unsupported constituent')
+    elif (np.any(coef < 0) or np.any(coef > 10)):
+        return None
+    else:
+        # convert to single number and round off floating point errors
+        DO = np.sum([v*10**(2-o) for o,v in enumerate(coef)])
+        return np.round(DO, decimals=3)
 
 def _from_doodson_number(DO: float | np.ndarray):
     """
     Converts Doodson numbers into Cartwright numbers
 
     Parameters
     ----------
```

### Comparing `pyTMD-2.1.0/pyTMD/astro.py` & `pyTMD-2.1.1/pyTMD/astro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 u"""
 astro.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (01/2024)
 Astronomical and nutation routines
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     PyEphem: Astronomical Ephemeris for Python
         https://rhodesmill.org/pyephem/
 
 REFERENCES:
     Jean Meeus, Astronomical Algorithms, 2nd edition, 1998.
     Oliver Montenbruck, Practical Ephemeris Calculations, 1989.
 
 UPDATE HISTORY:
+    Updated 01/2024: refactored lunisolar ephemerides functions
     Updated 12/2023: refactored phase_angles function to doodson_arguments
         added option to compute mean lunar time using equinox method
     Updated 05/2023: add wrapper function for nutation angles
         download JPL kernel file if not currently existing
     Updated 04/2023: added low resolution solar and lunar positions
         added function with more phase angles of the sun and moon
         functions to calculate solar and lunar positions with ephemerides
@@ -426,15 +427,55 @@
     T = (MJD - 51544.5)/36525.0
     # mean obliquity of the ecliptic (arcseconds)
     epsilon0 = np.array([84381.406, -46.836769, -1.831e-4,
         2.00340e-4, -5.76e-07, -4.34e-08])
     return atr*polynomial_sum(epsilon0, T)
 
 # PURPOSE: compute coordinates of the sun in an ECEF frame
-def solar_ecef(MJD: np.ndarray):
+def solar_ecef(MJD: np.ndarray, **kwargs):
+    """
+    Wrapper function for calculating the positional coordinates
+    of the sun in an Earth-centric, Earth-Fixed (ECEF) frame
+    [1]_ [2]_ [3]_
+
+    Parameters
+    ----------
+    MJD: np.ndarray
+        Modified Julian Day (MJD) of input date
+    ephemerides: str, default 'approximate'
+        Method for calculating solar ephemerides
+
+            - ``'approximate'``: low-resolution ephemerides
+            - ``'JPL'``: computed ephemerides from JPL kernels
+    kwargs: dict
+        Keyword options for ephemeris calculation
+
+    Returns
+    -------
+    X, Y, Z: np.ndarray
+        ECEF coordinates of the sun (meters)
+
+    References
+    ----------
+    .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
+    .. [2] O. Montenbruck, *Practical Ephemeris Calculations*,
+        146 pp., (1989).
+    .. [3] R. S. Park, W. M. Folkner, and J. G. Williams, and D. H. Boggs,
+        "The JPL Planetary and Lunar Ephemerides DE440 and DE441",
+        *The Astronomical Journal*, 161(3), 105, (2021).
+        `doi: 10.3847/1538-3881/abd414
+        <https://doi.org/10.3847/1538-3881/abd414>`_
+    """
+    kwargs.setdefault('ephemerides', 'approximate')
+    if (kwargs['ephemerides'].lower() == 'approximate'):
+        return solar_approximate(MJD, **kwargs)
+    elif (kwargs['ephemerides'].upper() == 'JPL'):
+        return solar_ephemerides(MJD, **kwargs)
+
+def solar_approximate(MJD, **kwargs):
     """
     Computes approximate positional coordinates of the sun in an
     Earth-centric, Earth-Fixed (ECEF) frame [1]_ [2]_
 
     Parameters
     ----------
     MJD: np.ndarray
@@ -533,15 +574,55 @@
     X = rot_z[0,0,:]*x + rot_z[0,1,:]*y + rot_z[0,2,:]*z
     Y = rot_z[1,0,:]*x + rot_z[1,1,:]*y + rot_z[1,2,:]*z
     Z = rot_z[2,0,:]*x + rot_z[2,1,:]*y + rot_z[2,2,:]*z
     # return the ECEF coordinates
     return (X, Y, Z)
 
 # PURPOSE: compute coordinates of the moon in an ECEF frame
-def lunar_ecef(MJD: np.ndarray):
+def lunar_ecef(MJD: np.ndarray, **kwargs):
+    """
+    Wrapper function for calculating the positional coordinates
+    of the moon in an Earth-centric, Earth-Fixed (ECEF) frame
+    [1]_ [2]_ [3]_
+
+    Parameters
+    ----------
+    MJD: np.ndarray
+        Modified Julian Day (MJD) of input date
+    ephemerides: str, default 'approximate'
+        Method for calculating lunar ephemerides
+
+            - ``'approximate'``: low-resolution ephemerides
+            - ``'JPL'``: computed ephemerides from JPL kernels
+    kwargs: dict
+        Keyword options for ephemeris calculation
+
+    Returns
+    -------
+    X, Y, Z: np.ndarray
+        ECEF coordinates of the moon (meters)
+
+    References
+    ----------
+    .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
+    .. [2] O. Montenbruck, *Practical Ephemeris Calculations*,
+        146 pp., (1989).
+    .. [3] R. S. Park, W. M. Folkner, and J. G. Williams, and D. H. Boggs,
+        "The JPL Planetary and Lunar Ephemerides DE440 and DE441",
+        *The Astronomical Journal*, 161(3), 105, (2021).
+        `doi: 10.3847/1538-3881/abd414
+        <https://doi.org/10.3847/1538-3881/abd414>`_
+    """
+    kwargs.setdefault('ephemerides', 'approximate')
+    if (kwargs['ephemerides'].lower() == 'approximate'):
+        return lunar_approximate(MJD, **kwargs)
+    elif (kwargs['ephemerides'].upper() == 'JPL'):
+        return lunar_ephemerides(MJD, **kwargs)
+
+def lunar_approximate(MJD, **kwargs):
     """
     Computes approximate positional coordinates of the moon in an
     Earth-centric, Earth-Fixed (ECEF) frame [1]_ [2]_
 
     Parameters
     ----------
     MJD: np.ndarray
```

### Comparing `pyTMD-2.1.0/pyTMD/calc_astrol_longitudes.py` & `pyTMD-2.1.1/pyTMD/calc_astrol_longitudes.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/check_points.py` & `pyTMD-2.1.1/pyTMD/check_points.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/compute_tide_corrections.py` & `pyTMD-2.1.1/pyTMD/compute.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 u"""
-compute_tide_corrections.py
-Written by Tyler Sutterley (12/2023)
+compute.py
+Written by Tyler Sutterley (02/2024)
 Calculates tidal elevations for correcting elevation or imagery data
+Calculates tidal currents at locations and times
 
 Ocean and Load Tides
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -55,14 +56,18 @@
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/GOT.py: extract tidal harmonic constants from GSFC GOT models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
+    Updated 01/2024: made the inferrence of minor constituents an option
+        refactored lunisolar ephemerides functions
+        renamed module to compute and added tidal currents function
     Updated 12/2023: use new crs class for coordinate reprojection
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 05/2023: use timescale class for time conversion operations
         use defaults from eop module for pole tide and EOP files
         add option for using higher resolution ephemerides from JPL
     Updated 04/2023: added function for radial solid earth tides
         using pathlib to define and expand paths
@@ -102,15 +107,14 @@
 """
 from __future__ import print_function, annotations
 
 import logging
 import pathlib
 import numpy as np
 import scipy.interpolate
-import pyTMD.constants
 import pyTMD.crs
 import pyTMD.eop
 import pyTMD.io
 import pyTMD.time
 import pyTMD.io.model
 import pyTMD.predict
 import pyTMD.spatial
@@ -118,16 +122,16 @@
 
 # attempt imports
 try:
     import pyproj
 except (AttributeError, ImportError, ModuleNotFoundError) as exc:
     logging.critical("pyproj not available")
 
-# PURPOSE: wrapper function for computing corrections
-def compute_corrections(
+# PURPOSE: wrapper function for computing values
+def corrections(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         CORRECTION: str = 'ocean',
         **kwargs
     ):
     """
     Wrapper function to compute tide corrections at points and times
 
@@ -149,45 +153,46 @@
             - ``'OPT'``: ocean pole tide
             - ``'SET'``: solid earth tide
     **kwargs: dict
         keyword arguments for correction functions
 
     Returns
     -------
-    correction: np.ndarray
+    values: np.ndarray
         tidal correction at coordinates and time in meters
     """
     if CORRECTION.lower() in ('ocean', 'load'):
-        return compute_tide_corrections(x, y, delta_time, **kwargs)
+        return tide_elevations(x, y, delta_time, **kwargs)
     elif (CORRECTION.upper() == 'LPET'):
-        return compute_LPET_corrections(x, y, delta_time, **kwargs)
+        return LPET_elevations(x, y, delta_time, **kwargs)
     elif (CORRECTION.upper() == 'LPT'):
-        return compute_LPT_corrections(x, y, delta_time, **kwargs)
+        return LPT_displacements(x, y, delta_time, **kwargs)
     elif (CORRECTION.upper() == 'OPT'):
-        return compute_OPT_corrections(x, y, delta_time, **kwargs)
+        return OPT_displacements(x, y, delta_time, **kwargs)
     elif (CORRECTION.upper() == 'SET'):
-        return compute_SET_corrections(x, y, delta_time, **kwargs)
+        return SET_displacements(x, y, delta_time, **kwargs)
     else:
         raise ValueError(f'Unrecognized correction type: {CORRECTION}')
 
 # PURPOSE: compute tides at points and times using tide model algorithms
-def compute_tide_corrections(
+def tide_elevations(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         DIRECTORY: str | pathlib.Path | None = None,
         MODEL: str | None = None,
         ATLAS_FORMAT: str = 'netcdf',
         GZIP: bool = False,
         DEFINITION_FILE: str | pathlib.Path | None = None,
         EPSG: str | int = 3031,
         EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
+        TYPE: str | None = 'drift',
         TIME: str = 'UTC',
         METHOD: str = 'spline',
         EXTRAPOLATE: bool = False,
         CUTOFF: int | float=10.0,
+        INFER_MINOR: bool = True,
         APPLY_FLEXURE: bool = False,
         FILL_VALUE: float = np.nan,
         **kwargs
     ):
     """
     Compute ocean or load tides at points and times from
     model constituents
@@ -241,16 +246,18 @@
 
     EXTRAPOLATE: bool, default False
         Extrapolate with nearest-neighbors
     CUTOFF: int or float, default 10.0
         Extrapolation cutoff in kilometers
 
         Set to ``np.inf`` to extrapolate for all points
+    INFER_MINOR: bool, default True
+        Infer the height values for minor tidal constituents
     APPLY_FLEXURE: bool, default False
-        Apply ice flexure scaling factor to height constituents
+        Apply ice flexure scaling factor to height values
 
         Only valid for models containing flexure fields
     FILL_VALUE: float, default np.nan
         Output invalid value
 
     Returns
     -------
@@ -340,58 +347,291 @@
         deltat = timescale.tt_ut1
 
     # calculate complex phase in radians for Euler's
     cph = -1j*ph*np.pi/180.0
     # calculate constituent oscillation
     hc = amp*np.exp(cph)
 
-    # predict tidal elevations at time and infer minor corrections
+    # predict tidal elevations at time
     if (TYPE.lower() == 'grid'):
         ny,nx = np.shape(x)
         tide = np.ma.zeros((ny,nx,nt),fill_value=FILL_VALUE)
         tide.mask = np.zeros((ny,nx,nt),dtype=bool)
         for i in range(nt):
             TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
                 deltat=deltat[i], corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
-                deltat=deltat[i], corrections=model.format)
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
+                    deltat=deltat[i], corrections=model.format)
+            else:
+                MINOR = np.ma.zeros_like(TIDE)
             # add major and minor components and reform grid
             tide[:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
             tide.mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask), (ny,nx))
     elif (TYPE.lower() == 'drift'):
         tide = np.ma.zeros((nt), fill_value=FILL_VALUE)
         tide.mask = np.any(hc.mask,axis=1)
         tide.data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
             deltat=deltat, corrections=model.format)
-        minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
-            deltat=deltat, corrections=model.format)
-        tide.data[:] += minor.data[:]
+        # calculate values for minor constituents by inferrence
+        if INFER_MINOR:
+            minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
+                deltat=deltat, corrections=model.format)
+            tide.data[:] += minor.data[:]
     elif (TYPE.lower() == 'time series'):
         nstation = len(x)
         tide = np.ma.zeros((nstation,nt), fill_value=FILL_VALUE)
         tide.mask = np.zeros((nstation,nt),dtype=bool)
         for s in range(nstation):
-            TIDE = pyTMD.predict.time_series(timescale.tide, hc[s,None,:], c,
-                deltat=deltat, corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(timescale.tide, hc[s,None,:], c,
+            HC = hc[s,None,:]
+            TIDE = pyTMD.predict.time_series(timescale.tide, HC, c,
                 deltat=deltat, corrections=model.format)
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                MINOR = pyTMD.predict.infer_minor(timescale.tide, HC, c,
+                    deltat=deltat, corrections=model.format)
+            else:
+                MINOR = np.ma.zeros_like(TIDE)
+            # add major and minor components
             tide.data[s,:] = TIDE.data[:] + MINOR.data[:]
             tide.mask[s,:] = (TIDE.mask | MINOR.mask)
     # replace invalid values with fill value
     tide.data[tide.mask] = tide.fill_value
 
     # return the ocean or load tide correction
     return tide
 
+# PURPOSE: compute tides at points and times using tide model algorithms
+def tide_currents(
+        x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
+        DIRECTORY: str | pathlib.Path | None = None,
+        MODEL: str | None = None,
+        ATLAS_FORMAT: str = 'netcdf',
+        GZIP: bool = False,
+        DEFINITION_FILE: str | pathlib.Path | None = None,
+        EPSG: str | int = 3031,
+        EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
+        TYPE: str | None = 'drift',
+        TIME: str = 'UTC',
+        METHOD: str = 'spline',
+        EXTRAPOLATE: bool = False,
+        CUTOFF: int | float=10.0,
+        INFER_MINOR: bool = True,
+        FILL_VALUE: float = np.nan,
+        **kwargs
+    ):
+    """
+    Compute ocean tide currents at points and times from
+    model constituents
+
+    Parameters
+    ----------
+    x: np.ndarray
+        x-coordinates in projection EPSG
+    y: np.ndarray
+        y-coordinates in projection EPSG
+    delta_time: np.ndarray
+        seconds since EPOCH or datetime array
+    DIRECTORY: str or NoneType, default None
+        working data directory for tide models
+    MODEL: str or NoneType, default None
+        Tide model to use in correction
+    ATLAS_FORMAT: str, default 'netcdf'
+        ATLAS tide model format
+
+            - ``'OTIS'``
+            - ``'netcdf'``
+    GZIP: bool, default False
+        Tide model files are gzip compressed
+    DEFINITION_FILE: str or NoneType, default None
+        Tide model definition file for use
+    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
+        Input coordinate system
+    EPOCH: tuple, default (2000,1,1,0,0,0)
+        Time period for calculating delta times
+    TYPE: str or NoneType, default 'drift'
+        Input data type
+
+            - ``None``: determined from input variable dimensions
+            - ``'drift'``: drift buoys or satellite/airborne altimetry
+            - ``'grid'``: spatial grids or images
+            - ``'time series'``: time series at a single point
+    TIME: str, default 'UTC'
+        Time type if need to compute leap seconds to convert to UTC
+
+            - ``'GPS'``: leap seconds needed
+            - ``'LORAN'``: leap seconds needed (LORAN = GPS + 9 seconds)
+            - ``'TAI'``: leap seconds needed (TAI = GPS + 19 seconds)
+            - ``'UTC'``: no leap seconds needed
+            - ``'datetime'``: numpy datatime array in UTC
+    METHOD: str
+        Interpolation method
+
+            - ```bilinear```: quick bilinear interpolation
+            - ```spline```: scipy bivariate spline interpolation
+            - ```linear```, ```nearest```: scipy regular grid interpolations
+
+    EXTRAPOLATE: bool, default False
+        Extrapolate with nearest-neighbors
+    CUTOFF: int or float, default 10.0
+        Extrapolation cutoff in kilometers
+
+        Set to ``np.inf`` to extrapolate for all points
+    INFER_MINOR: bool, default True
+        Infer the height values for minor tidal constituents
+    FILL_VALUE: float, default np.nan
+        Output invalid value
+
+    Returns
+    -------
+    tide: dict
+        tidal currents at coordinates and times
+    """
+
+    # check that tide directory is accessible
+    if DIRECTORY is not None:
+        DIRECTORY = pathlib.Path(DIRECTORY).expanduser()
+        if not DIRECTORY.exists():
+            raise FileNotFoundError("Invalid tide directory")
+
+    # validate input arguments
+    assert TIME in ('GPS', 'LORAN', 'TAI', 'UTC', 'datetime')
+    assert METHOD in ('bilinear', 'spline', 'linear', 'nearest')
+
+    # get parameters for tide model
+    if DEFINITION_FILE is not None:
+        model = pyTMD.io.model(DIRECTORY).from_file(
+            pathlib.Path(DEFINITION_FILE).expanduser())
+    else:
+        model = pyTMD.io.model(DIRECTORY, format=ATLAS_FORMAT,
+            compressed=GZIP).current(MODEL)
+
+    # determine input data type based on variable dimensions
+    if not TYPE:
+        TYPE = pyTMD.spatial.data_type(x, y, delta_time)
+    # reform coordinate dimensions for input grids
+    # or verify coordinate dimension shapes
+    if (TYPE.lower() == 'grid') and (np.size(x) != np.size(y)):
+        x,y = np.meshgrid(np.copy(x),np.copy(y))
+    elif (TYPE.lower() == 'grid'):
+        x = np.atleast_2d(x)
+        y = np.atleast_2d(y)
+    elif TYPE.lower() in ('time series', 'drift'):
+        x = np.atleast_1d(x)
+        y = np.atleast_1d(y)
+
+    # converting x,y from EPSG to latitude/longitude
+    crs1 = pyTMD.crs().from_input(EPSG)
+    crs2 = pyproj.CRS.from_epsg(4326)
+    transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
+    lon, lat = transformer.transform(x.flatten(), y.flatten())
+
+    # assert delta time is an array
+    delta_time = np.atleast_1d(delta_time)
+    # convert delta times or datetimes objects to timescale
+    if (TIME.lower() == 'datetime'):
+        timescale = pyTMD.time.timescale().from_datetime(
+            delta_time.flatten())
+    else:
+        timescale = pyTMD.time.timescale().from_deltatime(delta_time,
+            epoch=EPOCH, standard=TIME)
+    # number of time points
+    nt = len(timescale)
+
+    # python dictionary with tide model data
+    tide = {}
+    # iterate over u and v currents
+    for t in model.type:
+        # read tidal constants and interpolate to grid points
+        if model.format in ('OTIS', 'ATLAS', 'TMD3'):
+            amp,ph,D,c = pyTMD.io.OTIS.extract_constants(lon, lat, model.grid_file,
+                model.model_file['u'], model.projection, type=t,
+                method=METHOD, extrapolate=EXTRAPOLATE, cutoff=CUTOFF,
+                grid=model.format)
+            # use delta time at 2000.0 to match TMD outputs
+            deltat = np.zeros((nt), dtype=np.float64)
+        elif (model.format == 'netcdf'):
+            amp,ph,D,c = pyTMD.io.ATLAS.extract_constants(lon, lat, model.grid_file,
+                model.model_file[t], type=t, method=METHOD,
+                extrapolate=EXTRAPOLATE, cutoff=CUTOFF, scale=model.scale,
+                compressed=model.compressed)
+            # use delta time at 2000.0 to match TMD outputs
+            deltat = np.zeros((nt), dtype=np.float64)
+        elif (model.format == 'FES'):
+            amp,ph = pyTMD.io.FES.extract_constants(lon, lat, model.model_file[t],
+                type=t, version=model.version, method=METHOD,
+                extrapolate=EXTRAPOLATE, cutoff=CUTOFF, scale=model.scale,
+                compressed=model.compressed)
+            # available model constituents
+            c = model.constituents
+            # delta time (TT - UT1)
+            deltat = timescale.tt_ut1
+
+        # calculate complex phase in radians for Euler's
+        cph = -1j*ph*np.pi/180.0
+        # calculate constituent oscillation
+        hc = amp*np.exp(cph)
+
+        # predict tidal currents at time
+        if (TYPE.lower() == 'grid'):
+            ny,nx = np.shape(x)
+            tide[t] = np.ma.zeros((ny,nx,nt),fill_value=FILL_VALUE)
+            tide[t].mask = np.zeros((ny,nx,nt),dtype=bool)
+            for i in range(nt):
+                TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
+                    deltat=deltat[i], corrections=model.format)
+                # calculate values for minor constituents by inferrence
+                if INFER_MINOR:
+                    MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
+                        deltat=deltat[i], corrections=model.format)
+                else:
+                    MINOR = np.ma.zeros_like(TIDE)
+                # add major and minor components and reform grid
+                tide[t][:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
+                tide[t].mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask), (ny,nx))
+        elif (TYPE.lower() == 'drift'):
+            tide[t] = np.ma.zeros((nt), fill_value=FILL_VALUE)
+            tide[t].mask = np.any(hc.mask,axis=1)
+            tide[t].data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
+                deltat=deltat, corrections=model.format)
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
+                    deltat=deltat, corrections=model.format)
+                tide[t].data[:] += minor.data[:]
+        elif (TYPE.lower() == 'time series'):
+            nstation = len(x)
+            tide[t] = np.ma.zeros((nstation,nt), fill_value=FILL_VALUE)
+            tide[t].mask = np.zeros((nstation,nt),dtype=bool)
+            for s in range(nstation):
+                HC = hc[s,None,:]
+                TIDE = pyTMD.predict.time_series(timescale.tide, HC, c,
+                    deltat=deltat, corrections=model.format)
+                # calculate values for minor constituents by inferrence
+                if INFER_MINOR:
+                    MINOR = pyTMD.predict.infer_minor(timescale.tide, HC, c,
+                        deltat=deltat, corrections=model.format)
+                else:
+                    MINOR = np.ma.zeros_like(TIDE)
+                # add major and minor components
+                tide[t].data[s,:] = TIDE.data[:] + MINOR.data[:]
+                tide[t].mask[s,:] = (TIDE.mask | MINOR.mask)
+        # replace invalid values with fill value
+        tide[t].data[tide[t].mask] = tide[t].fill_value
+
+    # return the ocean tide currents
+    return tide
+
 # PURPOSE: compute long-period equilibrium tidal elevations
-def compute_LPET_corrections(
+def LPET_elevations(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         EPSG: str | int = 3031,
         EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
+        TYPE: str | None = 'drift',
         TIME: str = 'UTC',
         **kwargs
     ):
     """
     Compute long-period equilibrium tidal elevations at points and times
 
     Parameters
@@ -478,25 +718,25 @@
     elif (TYPE == 'time series'):
         nstation = len(x)
         tide_lpe = np.zeros((nstation,nt))
         for s in range(nstation):
             lpet = pyTMD.predict.equilibrium_tide(tide_time, lat[s])
             tide_lpe[s,:] = np.copy(lpet)
 
-    # return the long-period equilibrium tide corrections
+    # return the long-period equilibrium tide elevations
     return tide_lpe
 
 # PURPOSE: compute radial load pole tide displacements
 # following IERS Convention (2010) guidelines
-def compute_LPT_corrections(
+def LPT_displacements(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         h: float | np.ndarray = 0.0,
         EPSG: str | int = 3031,
         EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
+        TYPE: str | None = 'drift',
         TIME: str = 'UTC',
         ELLIPSOID: str = 'WGS84',
         CONVENTION: str = '2018',
         FILL_VALUE: float = np.nan,
         **kwargs
     ):
     """
@@ -594,15 +834,15 @@
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
     # tidal love number appropriate for the load tide
     hb2 = 0.6207
 
     # flatten heights
     h = np.array(h).flatten() if np.ndim(h) else h
     # convert from geodetic latitude to geocentric latitude
     # calculate X, Y and Z from geodetic latitude and longitude
@@ -649,25 +889,25 @@
         for s in range(nstation):
             SRAD = dfactor[s]*np.sin(2.0*theta[s])*(mx*np.cos(phi[s])+my*np.sin(phi[s]))
             Srad.data[s,:] = np.copy(SRAD)
             Srad.mask[s,:] = np.isnan(Srad.data[s,:])
     # replace invalid data with fill values
     Srad.data[Srad.mask] = Srad.fill_value
 
-    # return the solid earth pole tide corrections
+    # return the solid earth pole tide displacements
     return Srad
 
 # PURPOSE: compute radial load pole tide displacements
 # following IERS Convention (2010) guidelines
-def compute_OPT_corrections(
+def OPT_displacements(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         h: float | np.ndarray = 0.0,
         EPSG: str | int = 3031,
         EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
+        TYPE: str | None = 'drift',
         TIME: str = 'UTC',
         ELLIPSOID: str = 'WGS84',
         CONVENTION: str = '2018',
         METHOD: str = 'spline',
         FILL_VALUE: float = np.nan,
         **kwargs
     ):
@@ -773,15 +1013,15 @@
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
     # mean equatorial gravitational acceleration [m/s^2]
     ge = 9.7803278
     # density of sea water [kg/m^3]
     rho_w = 1025.0
     # tidal love number differential (1 + kl - hl) for pole tide frequencies
     gamma = 0.6870 + 0.0036j
 
@@ -850,24 +1090,24 @@
             URAD = K*atr*np.real((mx*gamma.real + my*gamma.imag)*UR.real[s] +
                 (my*gamma.real - mx*gamma.imag)*UR.imag[s])
             Urad.data[s,:] = np.copy(URAD)
             Urad.mask[s,:] = np.isnan(Urad.data[s,:])
     # replace invalid data with fill values
     Urad.data[Urad.mask] = Urad.fill_value
 
-    # return the ocean pole tide corrections
+    # return the ocean pole tide displacements
     return Urad
 
 # PURPOSE: compute solid earth tidal elevations
-def compute_SET_corrections(
+def SET_displacements(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         h: float | np.ndarray = 0.0,
         EPSG: str | int = 3031,
         EPOCH: list | tuple = (2000, 1, 1, 0, 0, 0),
-        TYPE: str or None = 'drift',
+        TYPE: str | None = 'drift',
         TIME: str = 'UTC',
         ELLIPSOID: str = 'WGS84',
         TIDE_SYSTEM='tide_free',
         EPHEMERIDES='approximate',
         **kwargs
     ):
     """
@@ -957,28 +1197,22 @@
             epoch=EPOCH, standard=TIME)
     # convert tide times to dynamical time
     tide_time = timescale.tide + timescale.tt_ut1
     # number of time points
     nt = len(timescale)
 
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
 
     # convert input coordinates to cartesian
     X, Y, Z = pyTMD.spatial.to_cartesian(lon, lat, h=h,
         a_axis=units.a_axis, flat=units.flat)
     # compute ephemerides for lunisolar coordinates
-    if (EPHEMERIDES.lower() == 'approximate'):
-        # get low-resolution solar and lunar ephemerides
-        SX, SY, SZ = pyTMD.astro.solar_ecef(timescale.MJD)
-        LX, LY, LZ = pyTMD.astro.lunar_ecef(timescale.MJD)
-    elif (EPHEMERIDES.upper() == 'JPL'):
-        # compute solar and lunar ephemerides from JPL kernel
-        SX, SY, SZ = pyTMD.astro.solar_ephemerides(timescale.MJD)
-        LX, LY, LZ = pyTMD.astro.lunar_ephemerides(timescale.MJD)
+    SX, SY, SZ = pyTMD.astro.solar_ecef(timescale.MJD, ephemerides=EPHEMERIDES)
+    LX, LY, LZ = pyTMD.astro.lunar_ecef(timescale.MJD, ephemerides=EPHEMERIDES)
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         ny,nx = np.shape(x)
         tide_se = np.zeros((ny,nx,nt))
         # convert coordinates to column arrays
         XYZ = np.c_[X, Y, Z]
@@ -1032,9 +1266,9 @@
             dln,dlt,drad = pyTMD.spatial.to_geodetic(
                 X + dxi[:,0], Y + dxi[:,1], Z + dxi[:,2],
                 a_axis=units.a_axis, flat=units.flat)
             # remove effects of original topography
             # (if added when computing cartesian coordinates)
             tide_se[s,:] = drad - h
 
-    # return the solid earth tide corrections
+    # return the solid earth tide displacements
     return tide_se
```

### Comparing `pyTMD-2.1.0/pyTMD/convert_crs.py` & `pyTMD-2.1.1/pyTMD/convert_crs.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/convert_ll_xy.py` & `pyTMD-2.1.1/pyTMD/convert_ll_xy.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/deltat.data` & `pyTMD-2.1.1/pyTMD/data/deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/finals.all` & `pyTMD-2.1.1/pyTMD/data/finals.all`

 * *Files 0% similar despite different names*

```diff
@@ -18232,815 +18232,906 @@
 2212 2 59915.00 I  0.141113 0.000016  0.189933 0.000013  I-0.0200318 0.0000048  0.4364 0.0034  I  -111.699    0.715    -6.072    0.117  0.141086  0.190030 -0.0200182  -111.557    -6.103  
 2212 3 59916.00 I  0.138517 0.000016  0.189627 0.000014  I-0.0204331 0.0000048  0.4026 0.0030  I  -111.641    0.715    -5.914    0.117  0.138520  0.189588 -0.0204483  -111.593    -5.954  
 2212 4 59917.00 I  0.135682 0.000016  0.189544 0.000015  I-0.0208201 0.0000036  0.3183 0.0031  I  -111.694    0.824    -5.748    0.127  0.135739  0.189603 -0.0208072  -111.696    -5.787  
 2212 5 59918.00 I  0.132708 0.000016  0.189107 0.000015  I-0.0210300 0.0000038  0.1150 0.0024  I  -111.745    0.824    -5.584    0.127  0.132595  0.189132 -0.0210271  -111.763    -5.625  
 2212 6 59919.00 I  0.130254 0.000011  0.188745 0.000014  I-0.0210506 0.0000032 -0.0870 0.0027  I  -111.676    0.994    -5.482    0.138  0.130234  0.188807 -0.0210546  -111.664    -5.528  
 2212 7 59920.00 I  0.127861 0.000014  0.188861 0.000015  I-0.0208548 0.0000038 -0.2928 0.0024  I  -111.515    0.845    -5.532    0.108  0.127804  0.188914 -0.0208636  -111.530    -5.568  
 2212 8 59921.00 I  0.125549 0.000013  0.188702 0.000014  I-0.0204831 0.0000037 -0.4445 0.0028  I  -111.400    0.845    -5.745    0.108  0.125550  0.188683 -0.0204842  -111.431    -5.765  
-2212 9 59922.00 I  0.123017 0.000012  0.188887 0.000013  I-0.0199769 0.0000040 -0.5630 0.0032  I  -111.406    0.845    -6.000    0.108  0.123051  0.188943 -0.0199575  -111.450    -5.997  
-221210 59923.00 I  0.120050 0.000012  0.189249 0.000009  I-0.0193674 0.0000053 -0.6506 0.0032  I  -111.440    0.685    -6.144    0.066  0.120023  0.189212 -0.0193465  -111.433    -6.148  
-221211 59924.00 I  0.117117 0.000018  0.189436 0.000010  I-0.0187029 0.0000051 -0.6567 0.0036  I  -111.367    0.693    -6.151    0.154  0.117059  0.189519 -0.0187186  -111.306    -6.171  
-221212 59925.00 I  0.114548 0.000018  0.189329 0.000011  I-0.0180986 0.0000050 -0.5289 0.0033  I  -111.144    0.693    -6.131    0.154  0.114474  0.189311 -0.0181257  -111.063    -6.164  
-221213 59926.00 I  0.112247 0.000017  0.189360 0.000011  I-0.0176422 0.0000042 -0.4098 0.0032  I  -110.805    0.815    -6.164    0.189  0.112235  0.189380 -0.0176371  -110.733    -6.213  
-221214 59927.00 I  0.110095 0.000017  0.189785 0.000011  I-0.0172863 0.0000041 -0.2687 0.0029  I  -110.369    0.815    -6.181    0.189  0.110057  0.189733 -0.0172887  -110.324    -6.215  
-221215 59928.00 I  0.107810 0.000017  0.190596 0.000011  I-0.0171108 0.0000039 -0.1095 0.0028  I  -109.904    0.815    -6.067    0.189  0.107848  0.190644 -0.0170929  -109.882    -6.084  
-221216 59929.00 I  0.105279 0.000016  0.191595 0.000011  I-0.0170862 0.0000038  0.1066 0.0027  I  -109.630    0.815    -5.836    0.189  0.105276  0.191662 -0.0170407  -109.642    -5.845  
-221217 59930.00 I  0.102631 0.000011  0.192132 0.000010  I-0.0173035 0.0000037  0.2613 0.0030  I  -109.773    0.904    -5.635    0.172  0.102588  0.192217 -0.0171383  -109.796    -5.644  
-221218 59931.00 I  0.100234 0.000026  0.192467 0.000018  I-0.0175525 0.0000047  0.2471 0.0039  I  -110.286    0.797    -5.548    0.132  0.100160  0.192490 -0.0173664  -110.291    -5.561  
-221219 59932.00 I  0.098305 0.000026  0.192746 0.000017  I-0.0177921 0.0000069  0.2159 0.0033  I  -110.856    0.688    -5.478    0.074  0.098210  0.192803 -0.0177187  -110.824    -5.496  
-221220 59933.00 I  0.096748 0.000029  0.193154 0.000026  I-0.0179712 0.0000046  0.1452 0.0042  I  -111.299    0.633    -5.321    0.073  0.096711  0.193084 -0.0179634  -111.212    -5.340  
+2212 9 59922.00 I  0.123017 0.000012  0.188887 0.000013  I-0.0199769 0.0000040 -0.5630 0.0032  I  -111.484    0.685    -5.968    0.066  0.123051  0.188943 -0.0199575  -111.450    -5.997  
+221210 59923.00 I  0.120050 0.000012  0.189249 0.000009  I-0.0193674 0.0000053 -0.6506 0.0032  I  -111.456    0.685    -6.135    0.066  0.120023  0.189212 -0.0193465  -111.433    -6.148  
+221211 59924.00 I  0.117117 0.000018  0.189436 0.000010  I-0.0187029 0.0000051 -0.6567 0.0036  I  -111.352    0.693    -6.154    0.154  0.117059  0.189519 -0.0187186  -111.306    -6.171  
+221212 59925.00 I  0.114548 0.000018  0.189329 0.000011  I-0.0180986 0.0000050 -0.5289 0.0033  I  -111.123    0.693    -6.138    0.154  0.114474  0.189311 -0.0181257  -111.063    -6.164  
+221213 59926.00 I  0.112247 0.000017  0.189360 0.000011  I-0.0176422 0.0000042 -0.4098 0.0032  I  -110.790    0.815    -6.171    0.189  0.112235  0.189380 -0.0176371  -110.733    -6.213  
+221214 59927.00 I  0.110095 0.000017  0.189785 0.000011  I-0.0172863 0.0000041 -0.2687 0.0029  I  -110.361    0.815    -6.186    0.189  0.110057  0.189733 -0.0172887  -110.324    -6.215  
+221215 59928.00 I  0.107810 0.000017  0.190596 0.000011  I-0.0171108 0.0000039 -0.1095 0.0028  I  -109.903    0.815    -6.070    0.189  0.107848  0.190644 -0.0170929  -109.882    -6.084  
+221216 59929.00 I  0.105279 0.000016  0.191595 0.000011  I-0.0170862 0.0000038  0.1066 0.0027  I  -109.632    0.815    -5.837    0.189  0.105276  0.191662 -0.0170407  -109.642    -5.845  
+221217 59930.00 I  0.102631 0.000011  0.192132 0.000010  I-0.0173035 0.0000037  0.2613 0.0030  I  -109.777    0.904    -5.635    0.172  0.102588  0.192217 -0.0171383  -109.796    -5.644  
+221218 59931.00 I  0.100234 0.000026  0.192467 0.000018  I-0.0175525 0.0000047  0.2471 0.0039  I  -110.289    0.797    -5.548    0.132  0.100160  0.192490 -0.0173664  -110.291    -5.561  
+221219 59932.00 I  0.098305 0.000026  0.192746 0.000017  I-0.0177921 0.0000069  0.2159 0.0033  I  -110.859    0.688    -5.478    0.074  0.098210  0.192803 -0.0177187  -110.824    -5.496  
+221220 59933.00 I  0.096748 0.000029  0.193154 0.000026  I-0.0179712 0.0000046  0.1452 0.0042  I  -111.300    0.633    -5.321    0.073  0.096711  0.193084 -0.0179634  -111.212    -5.340  
 221221 59934.00 I  0.095802 0.000029  0.193336 0.000026  I-0.0180841 0.0000048  0.0793 0.0033  I  -111.707    0.633    -5.196    0.073  0.095777  0.193348 -0.0181234  -111.654    -5.239  
-221222 59935.00 I  0.094819 0.000029  0.194003 0.000026  I-0.0180991 0.0000048 -0.0786 0.0034  I  -112.095    0.633    -5.329    0.073  0.094877  0.193950 -0.0181060  -112.105    -5.394  
-221223 59936.00 I  0.093422 0.000029  0.194945 0.000027  I-0.0179138 0.0000048 -0.2757 0.0031  I  -112.193    0.633    -5.683    0.073  0.093472  0.194922 -0.0178955  -112.150    -5.759  
-221224 59937.00 I  0.091312 0.000015  0.196096 0.000022  I-0.0176092 0.0000040 -0.2882 0.0032  I  -111.831    0.569    -5.931    0.073  0.091397  0.196126 -0.0175841  -111.706    -6.007  
-221225 59938.00 I  0.088380 0.000015  0.197001 0.000021  I-0.0173692 0.0000041 -0.2052 0.0034  I  -111.281    0.569    -5.869    0.073  0.088402  0.197099 -0.0173115  -111.094    -5.943  
-221226 59939.00 I  0.085224 0.000038  0.197366 0.000018  I-0.0172531 0.0000056  0.0407 0.0033  I  -110.944    0.610    -5.672    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
-221227 59940.00 I  0.082026 0.000038  0.197766 0.000018  I-0.0174768 0.0000052  0.3651 0.0037  I  -110.890    0.610    -5.593    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
-221228 59941.00 I  0.078215 0.000039  0.198405 0.000023  I-0.0179214 0.0000047  0.5037 0.0035  I  -110.935    0.673    -5.605    0.150  0.078253  0.198379 -0.0179243  -110.647    -5.673  
-221229 59942.00 I  0.074759 0.000039  0.198575 0.000023  I-0.0184549 0.0000048  0.5544 0.0033  I  -110.980    0.673    -5.519    0.150  0.074744  0.198584 -0.0184719  -110.694    -5.570  
-221230 59943.00 I  0.071219 0.000039  0.199149 0.000022  I-0.0190022 0.0000046  0.5210 0.0034  I  -111.076    0.673    -5.305    0.150  0.071281  0.199199 -0.0190102  -110.793    -5.341  
-221231 59944.00 I  0.067043 0.000039  0.200110 0.000023  I-0.0194890 0.0000048  0.4640 0.0039  I  -111.246    0.673    -5.118    0.150  0.067074  0.200103 -0.0194855  -110.973    -5.182  
-23 1 1 59945.00 I  0.062781 0.000011  0.200905 0.000017  I-0.0198682 0.0000063  0.2210 0.0036  I  -111.429    0.721    -5.054    0.134  0.062699  0.200944 -0.0197967  -111.162    -5.163  
-23 1 2 59946.00 I  0.059066 0.000032  0.201758 0.000019  I-0.0199331 0.0000054 -0.0158 0.0047  I  -111.537    0.585    -5.058    0.098  0.059003  0.201796 -0.0199243  -111.443    -5.114  
-23 1 3 59947.00 I  0.055736 0.000039  0.202461 0.000015  I-0.0198530 0.0000070 -0.2034 0.0045  I  -111.478    0.620    -5.070    0.135  0.055638  0.202514 -0.0198250  -111.467    -5.128  
-23 1 4 59948.00 I  0.052991 0.000039  0.203017 0.000016  I-0.0195098 0.0000073 -0.4406 0.0054  I  -111.210    0.620    -5.150    0.135  0.052933  0.202990 -0.0195007  -111.313    -5.194  
-23 1 5 59949.00 I  0.050823 0.000039  0.203824 0.000016  I-0.0190319 0.0000083 -0.4975 0.0055  I  -110.822    0.620    -5.373    0.135  0.050795  0.203830 -0.0190232  -110.822    -5.531  
-23 1 6 59950.00 I  0.048802 0.000039  0.205099 0.000015  I-0.0185223 0.0000082 -0.5317 0.0058  I  -110.501    0.620    -5.661    0.135  0.048795  0.205101 -0.0184663  -110.510    -5.834  
-23 1 7 59951.00 I  0.046882 0.000039  0.206230 0.000014  I-0.0179803 0.0000081 -0.5303 0.0060  I  -110.327    0.620    -5.837    0.135  0.046853  0.206221 -0.0179143  -110.392    -5.984  
-23 1 8 59952.00 I  0.045147 0.000028  0.207580 0.000013  I-0.0174926 0.0000087 -0.4362 0.0058  I  -110.217    0.872    -5.821    0.172  0.045146  0.207590 -0.0174487  -110.316    -5.948  
-23 1 9 59953.00 I  0.043372 0.000014  0.209048 0.000010  I-0.0171337 0.0000084 -0.2646 0.0058  I  -110.056    0.885    -5.710    0.141  0.043370  0.209111 -0.0171274  -110.159    -5.821  
-23 110 59954.00 I  0.041306 0.000013  0.210264 0.000010  I-0.0169644 0.0000078 -0.0899 0.0053  I  -109.811    0.885    -5.635    0.141  0.041325  0.210288 -0.0169671  -109.874    -5.733  
-23 111 59955.00 I  0.038971 0.000045  0.211091 0.000021  I-0.0169515 0.0000064  0.0778 0.0048  I  -109.516    0.812    -5.595    0.121  0.038979  0.211134 -0.0169747  -109.583    -5.665  
-23 112 59956.00 I  0.036558 0.000045  0.211946 0.000021  I-0.0170843 0.0000055  0.1385 0.0044  I  -109.232    0.812    -5.493    0.121  0.036547  0.211915 -0.0170559  -109.296    -5.533  
-23 113 59957.00 I  0.034217 0.000045  0.213007 0.000021  I-0.0172130 0.0000059  0.1527 0.0051  I  -109.088    0.812    -5.334    0.121  0.034173  0.213022 -0.0172046  -109.147    -5.343  
-23 114 59958.00 I  0.031793 0.000044  0.214433 0.000021  I-0.0173916 0.0000087  0.1726 0.0049  I  -109.224    0.683    -5.264    0.087  0.031810  0.214393 -0.0173877  -109.253    -5.273  
-23 115 59959.00 I  0.029354 0.000047  0.216069 0.000021  I-0.0175501 0.0000078  0.1681 0.0059  I  -109.609    0.630    -5.376    0.089  0.029351  0.216047 -0.0175710  -109.621    -5.396  
-23 116 59960.00 I  0.026875 0.000047  0.217955 0.000021  I-0.0177148 0.0000079  0.1246 0.0064  I  -110.025    0.630    -5.533    0.089  0.026882  0.217923 -0.0177110  -110.037    -5.563  
-23 117 59961.00 I  0.024350 0.000020  0.220229 0.000008  I-0.0177504 0.0000102 -0.0655 0.0059  I  -110.377    0.598    -5.524    0.090  0.024343  0.220214 -0.0177400  -110.403    -5.564  
-23 118 59962.00 I  0.021692 0.000036  0.222435 0.000013  I-0.0175612 0.0000088 -0.3232 0.0067  I  -110.849    0.664    -5.406    0.115  0.021681  0.222504 -0.0175873  -110.857    -5.445  
-23 119 59963.00 I  0.019109 0.000037  0.224226 0.000013  I-0.0171654 0.0000087 -0.3966 0.0061  I  -111.495    0.664    -5.479    0.115  0.019078  0.224261 -0.0172362  -111.474    -5.516  
-23 120 59964.00 I  0.016699 0.000037  0.225586 0.000014  I-0.0167619 0.0000085 -0.4885 0.0069  I  -111.910    0.664    -5.849    0.115  0.016715  0.225678 -0.0167521  -111.849    -5.887  
-23 121 59965.00 I  0.013985 0.000033  0.226869 0.000012  I-0.0161788 0.0000108 -0.6094 0.0056  I  -111.671    0.850    -6.200    0.149  0.014033  0.226892 -0.0161896  -111.635    -6.235  
-23 122 59966.00 I  0.010883 0.000041  0.227736 0.000033  I-0.0156323 0.0000073 -0.4628 0.0065  I  -110.955    0.571    -6.201    0.104  0.010879  0.227740 -0.0156593  -110.964    -6.230  
-23 123 59967.00 I  0.007809 0.000041  0.228873 0.000033  I-0.0152820 0.0000073 -0.2299 0.0053  I  -110.339    0.571    -5.952    0.104  0.007728  0.228830 -0.0153087  -110.393    -5.970  
-23 124 59968.00 I  0.005421 0.000028  0.230152 0.000032  I-0.0151989 0.0000076  0.0823 0.0051  I  -110.117    0.406    -5.789    0.065  0.005300  0.230244 -0.0152158  -110.223    -5.787  
-23 125 59969.00 I  0.003915 0.000028  0.231469 0.000047  I-0.0154136 0.0000070  0.2957 0.0052  I  -110.158    0.582    -5.792    0.151  0.003852  0.231401 -0.0153642  -110.193    -5.799  
-23 126 59970.00 I  0.002908 0.000028  0.233340 0.000048  I-0.0157015 0.0000070  0.2428 0.0049  I  -110.310    0.582    -5.753    0.151  0.002927  0.233231 -0.0156349  -110.268    -5.775  
-23 127 59971.00 I  0.001586 0.000027  0.235764 0.000048  I-0.0158884 0.0000069  0.1575 0.0050  I  -110.541    0.582    -5.590    0.151  0.001593  0.235918 -0.0158886  -110.468    -5.635  
-23 128 59972.00 I  0.000371 0.000010  0.238164 0.000037  I-0.0159939 0.0000072  0.0044 0.0049  I  -110.763    0.710    -5.488    0.199  0.000279  0.238107 -0.0159862  -110.687    -5.537  
-23 129 59973.00 I -0.000255 0.000028  0.240365 0.000038  I-0.0158894 0.0000069 -0.1722 0.0049  I  -110.849    0.898    -5.603    0.192 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
-23 130 59974.00 I -0.000873 0.000028  0.242676 0.000038  I-0.0156600 0.0000067 -0.3172 0.0048  I  -110.786    0.898    -5.839    0.192 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
-23 131 59975.00 I -0.001354 0.000029  0.244953 0.000016  I-0.0152326 0.0000068 -0.5294 0.0041  I  -110.640    1.298    -6.009    0.181 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
-23 2 1 59976.00 I -0.002314 0.000028  0.247836 0.000035  I-0.0146250 0.0000046 -0.6703 0.0042  I  -110.429    1.129    -6.088    0.183 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
-23 2 2 59977.00 I -0.003560 0.000028  0.250320 0.000035  I-0.0139085 0.0000050 -0.7616 0.0034  I  -110.152    1.129    -6.192    0.183 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
-23 2 3 59978.00 I -0.004897 0.000028  0.252424 0.000035  I-0.0131244 0.0000050 -0.7850 0.0034  I  -109.903    1.129    -6.364    0.183 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
-23 2 4 59979.00 I -0.006464 0.000011  0.254307 0.000034  I-0.0123983 0.0000046 -0.6291 0.0032  I  -109.801    0.955    -6.482    0.185 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
-23 2 5 59980.00 I -0.008211 0.000016  0.255926 0.000034  I-0.0118783 0.0000039 -0.4370 0.0030  I  -109.827    0.740    -6.420    0.153 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
-23 2 6 59981.00 I -0.009950 0.000015  0.257728 0.000034  I-0.0115055 0.0000040 -0.3014 0.0031  I  -109.825    0.740    -6.220    0.153 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
-23 2 7 59982.00 I -0.011920 0.000015  0.259682 0.000009  I-0.0112789 0.0000047 -0.1555 0.0028  I  -109.676    0.552    -6.038    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
-23 2 8 59983.00 I -0.014087 0.000029  0.261629 0.000024  I-0.0111899 0.0000038 -0.0235 0.0030  I  -109.407    0.750    -5.958    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
-23 2 9 59984.00 I -0.015736 0.000029  0.263465 0.000024  I-0.0112392 0.0000038  0.1303 0.0027  I  -109.150    0.750    -5.933    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
-23 210 59985.00 I -0.016689 0.000029  0.265519 0.000024  I-0.0114562 0.0000038  0.3010 0.0029  I  -109.025    0.750    -5.913    0.086 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
-23 211 59986.00 I -0.017890 0.000026  0.268029 0.000023  I-0.0118011 0.0000045  0.3513 0.0027  I  -109.094    0.923    -5.954    0.043 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
-23 212 59987.00 I -0.019627 0.000028  0.270430 0.000042  I-0.0121328 0.0000039  0.3235 0.0030  I  -109.312    0.780    -6.123    0.122 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
-23 213 59988.00 I -0.021935 0.000029  0.273058 0.000043  I-0.0124079 0.0000041  0.1749 0.0029  I  -109.540    0.780    -6.351    0.122 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
-23 214 59989.00 I -0.024500 0.000014  0.275809 0.000037  I-0.0124595 0.0000044 -0.0431 0.0029  I  -109.719    0.685    -6.477    0.160 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
-23 215 59990.00 I -0.026954 0.000018  0.278124 0.000037  I-0.0123401 0.0000042 -0.2057 0.0030  I  -109.976    0.660    -6.478    0.147 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
-23 216 59991.00 I -0.029366 0.000018  0.280707 0.000037  I-0.0120569 0.0000042 -0.3417 0.0030  I  -110.411    0.660    -6.554    0.147 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
-23 217 59992.00 I -0.031750 0.000018  0.282878 0.000038  I-0.0116866 0.0000042 -0.3880 0.0035  I  -110.784    0.660    -6.843    0.147 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
-23 218 59993.00 I -0.033987 0.000012  0.284848 0.000013  I-0.0113566 0.0000057 -0.2071 0.0033  I  -110.707    0.407    -7.158    0.088 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
-23 219 59994.00 I -0.035820 0.000015  0.286840 0.000022  I-0.0113184 0.0000050  0.1120 0.0037  I  -110.159    0.723    -7.206    0.176 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
-23 220 59995.00 I -0.037233 0.000015  0.288971 0.000022  I-0.0115754 0.0000048  0.4155 0.0035  I  -109.531    0.723    -6.992    0.176 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
-23 221 59996.00 I -0.038251 0.000010  0.291447 0.000021  I-0.0121525 0.0000048  0.7283 0.0037  I  -109.158    0.768    -6.795    0.198 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
-23 222 59997.00 I -0.038771 0.000044  0.294628 0.000021  I-0.0129541 0.0000057  0.8073 0.0038  I  -109.067    0.743    -6.758    0.155 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
-23 223 59998.00 I -0.038964 0.000044  0.298246 0.000020  I-0.0137297 0.0000058  0.7742 0.0041  I  -109.193    0.743    -6.751    0.155 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
-23 224 59999.00 I -0.039135 0.000044  0.301877 0.000020  I-0.0144999 0.0000059  0.7332 0.0048  I  -109.500    0.743    -6.677    0.155 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
-23 225 60000.00 I -0.039672 0.000043  0.305085 0.000007  I-0.0151484 0.0000076  0.5491 0.0045  I  -109.861    0.669    -6.668    0.064 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
-23 226 60001.00 I -0.040922 0.000043  0.308166 0.000040  I-0.0155605 0.0000067  0.2521 0.0051  I  -110.078    0.756    -6.870    0.057 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
-23 227 60002.00 I -0.042717 0.000043  0.310757 0.000040  I-0.0156517 0.0000067 -0.0476 0.0047  I  -110.087    0.756    -7.189    0.057 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
-23 228 60003.00 I -0.044026 0.000008  0.313156 0.000040  I-0.0155087 0.0000066 -0.2170 0.0043  I  -109.969    0.921    -7.398    0.034 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
-23 3 1 60004.00 I -0.045083 0.000009  0.316365 0.000040  I-0.0152845 0.0000055 -0.1861 0.0043  I  -109.746    0.899    -7.418    0.111 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
-23 3 2 60005.00 I -0.046060 0.000008  0.318717 0.000040  I-0.0151161 0.0000056 -0.2165 0.0038  I  -109.374    0.899    -7.380    0.111 -0.046065  0.318766 -0.0150624  -109.433    -7.347  
-23 3 3 60006.00 I -0.046658 0.000008  0.321124 0.000040  I-0.0148533 0.0000051 -0.2416 0.0040  I  -108.922    0.899    -7.419    0.111 -0.046677  0.321138 -0.0148245  -108.998    -7.328  
-23 3 4 60007.00 I -0.046916 0.000007  0.323791 0.000007  I-0.0146878 0.0000056 -0.1022 0.0043  I  -108.584    0.833    -7.496    0.222 -0.046882  0.323792 -0.0146819  -108.638    -7.416  
-23 3 5 60008.00 I -0.046598 0.000012  0.326588 0.000008  I-0.0146747 0.0000069  0.1144 0.0044  I  -108.469    0.921    -7.469    0.102 -0.046540  0.326621 -0.0146823  -108.483    -7.439  
-23 3 6 60009.00 I -0.045643 0.000013  0.329770 0.000008  I-0.0149259 0.0000068  0.3588 0.0051  I  -108.479    0.921    -7.292    0.102 -0.045657  0.329817 -0.0149129  -108.456    -7.322  
-23 3 7 60010.00 I -0.044603 0.000012  0.333311 0.000006  I-0.0153730 0.0000076  0.5451 0.0048  I  -108.457    0.938    -7.090    0.047 -0.044599  0.333296 -0.0153659  -108.413    -7.174  
-23 3 8 60011.00 I -0.043505 0.000027  0.336624 0.000018  I-0.0160098 0.0000068  0.7124 0.0050  I  -108.385    0.816    -7.008    0.040 -0.043530  0.336616 -0.0160051  -108.388    -7.094  
-23 3 9 60012.00 I -0.042357 0.000027  0.339825 0.000018  I-0.0167790 0.0000066  0.8231 0.0047  I  -108.359    0.816    -7.074    0.040 -0.042352  0.339803 -0.0167760  -108.432    -7.140  
-23 310 60013.00 I -0.041274 0.000027  0.343018 0.000018  I-0.0176211 0.0000064  0.8290 0.0040  I  -108.432    0.816    -7.209    0.040 -0.041322  0.343084 -0.0176027  -108.573    -7.251  
-23 311 60014.00 I -0.040745 0.000025  0.346439 0.000018  I-0.0184071 0.0000046  0.7452 0.0039  I  -108.558    0.724    -7.343    0.036 -0.040776  0.346390 -0.0184047  -108.718    -7.379  
-23 312 60015.00 I -0.040536 0.000025  0.349512 0.000019  I-0.0190959 0.0000043  0.6145 0.0032  I  -108.674    0.766    -7.475    0.055 -0.040519  0.349496 -0.0190910  -108.819    -7.513  
-23 313 60016.00 I -0.040083 0.000025  0.352549 0.000019  I-0.0196034 0.0000044  0.3857 0.0027  I  -108.744    0.766    -7.617    0.055 -0.040097  0.352572 -0.0196023  -108.854    -7.660  
-23 314 60017.00 I -0.039697 0.000008  0.355967 0.000010  I-0.0199051 0.0000032  0.2704 0.0027  I  -108.740    0.836    -7.752    0.075 -0.039717  0.355976 -0.0199116  -108.796    -7.801  
-23 315 60018.00 I -0.039668 0.000008  0.359423 0.000011  I-0.0201198 0.0000033  0.0821 0.0029  I  -108.653    0.836    -7.872    0.075 -0.039696  0.359397 -0.0200604  -108.636    -7.924  
-23 316 60019.00 I -0.039798 0.000006  0.362274 0.000010  I-0.0200760 0.0000048 -0.0861 0.0031  I  -108.517    0.836    -8.016    0.075 -0.039824  0.362249 -0.0200712  -108.426    -8.068  
-23 317 60020.00 I -0.039667 0.000007  0.364611 0.000010  I-0.0200343 0.0000052  0.0058 0.0045  I  -108.355    0.836    -8.203    0.075 -0.039666  0.364628 -0.0200376  -108.244    -8.259  
-23 318 60021.00 I -0.039049 0.000020  0.366839 0.000007  I-0.0201241 0.0000075  0.2073 0.0032  I  -108.156    0.322    -8.343    0.160 -0.039047  0.366850 -0.0201299  -108.073    -8.402  
-23 319 60022.00 I -0.038092 0.000017  0.368978 0.000007  I-0.0204892 0.0000039  0.5296 0.0043  I  -107.941    0.629    -8.308    0.080 -0.038102  0.368994 -0.0204875  -107.908    -8.371  
-23 320 60023.00 I -0.036906 0.000017  0.371254 0.000007  I-0.0211559 0.0000042  0.7696 0.0028  I  -107.783    0.629    -8.119    0.080 -0.036907  0.371284 -0.0211416  -107.809    -8.185  
-23 321 60024.00 I -0.035491 0.000017  0.373910 0.000006  I-0.0220021 0.0000041  0.9307 0.0037  I  -107.717    0.629    -7.949    0.080 -0.035480  0.373974 -0.0220007  -107.798    -8.018  
-23 322 60025.00 I -0.033909 0.000025  0.377081 0.000011  I-0.0229758 0.0000061  0.9672 0.0037  I  -107.722    0.713    -7.913    0.052 -0.033918  0.377072 -0.0229616  -107.800    -7.977  
-23 323 60026.00 I -0.032491 0.000025  0.380204 0.000014  I-0.0238897 0.0000062  0.8633 0.0045  I  -107.813    0.713    -7.949    0.052 -0.032503  0.380245 -0.0238876  -107.871    -8.006  
-23 324 60027.00 I -0.031166 0.000025  0.383326 0.000015  I-0.0246807 0.0000065  0.6945 0.0050  I  -108.036    0.713    -7.980    0.052 -0.031173  0.383274 -0.0246908  -108.068    -8.026  
-23 325 60028.00 I -0.029860 0.000018  0.386379 0.000014  I-0.0252313 0.0000079  0.3836 0.0046  I  -108.330    0.764    -8.053    0.021 -0.029863  0.386430 -0.0252241  -108.334    -8.069  
-23 326 60029.00 I -0.028393 0.000026  0.389491 0.000017  I-0.0254411 0.0000066  0.0524 0.0052  I  -108.535    0.823    -8.244    0.110 -0.028402  0.389466 -0.0254315  -108.511    -8.224  
-23 327 60030.00 I -0.026606 0.000026  0.392592 0.000017  I-0.0253855 0.0000069 -0.1306 0.0046  I  -108.563    0.823    -8.495    0.110 -0.026589  0.392633 -0.0253926  -108.515    -8.443  
-23 328 60031.00 I -0.024693 0.000020  0.395478 0.000014  I-0.0251941 0.0000065 -0.2710 0.0044  I  -108.449    0.885    -8.654    0.155 -0.024718  0.395445 -0.0251809  -108.385    -8.580  
-23 329 60032.00 I -0.023036 0.000028  0.397846 0.000027  I-0.0248755 0.0000054 -0.3156 0.0041  I  -108.220    0.774    -8.668    0.110 -0.023029  0.397858 -0.0248761  -108.184    -8.619  
-23 330 60033.00 I -0.021722 0.000030  0.400000 0.000027  I-0.0246029 0.0000050 -0.2404 0.0036  I  -107.836    0.774    -8.649    0.110 -0.021735  0.400017 -0.0245819  -107.840    -8.642  
-23 331 60034.00 I -0.020382 0.000030  0.402290 0.000027  I-0.0244064 0.0000049 -0.1301 0.0039  I  -107.337    0.774    -8.724    0.110 -0.020397  0.402194 -0.0243867  -107.382    -8.762  
-23 4 1 60035.00 I -0.018849 0.000023  0.404542 0.000026  I-0.0243562 0.0000060  0.0206 0.0036  I  -106.916    0.692    -8.870    0.022 -0.018832  0.404562 -0.0243447  -106.941    -8.931  
-23 4 2 60036.00 I -0.017326 0.000029  0.407391 0.000026  I-0.0244586 0.0000052  0.2044 0.0040  I  -106.764    0.762    -8.931    0.066 -0.017339  0.407431 -0.0244585  -106.744    -9.003  
-23 4 3 60037.00 I -0.015627 0.000029  0.409969 0.000026  I-0.0247644 0.0000054  0.3864 0.0037  I  -106.871    0.762    -8.807    0.066 -0.015648  0.409984 -0.0247405  -106.816    -8.883  
-23 4 4 60038.00 I -0.013796 0.000043  0.412653 0.000019  I-0.0252246 0.0000053  0.5481 0.0038  I  -107.072    0.781    -8.569    0.091 -0.013789  0.412618 -0.0252154  -107.008    -8.648  
-23 4 5 60039.00 I -0.012263 0.000042  0.415420 0.000019  I-0.0258463 0.0000053  0.6670 0.0037  I  -107.241    0.781    -8.388    0.091 -0.012263  0.415517 -0.0258359  -107.244    -8.468  
-23 4 6 60040.00 I -0.010721 0.000042  0.418378 0.000019  I-0.0265279 0.0000052  0.6940 0.0037  I  -107.373    0.781    -8.373    0.091 -0.010755  0.418256 -0.0265377  -107.466    -8.452  
-23 4 7 60041.00 I -0.009115 0.000042  0.421137 0.000019  I-0.0272224 0.0000052  0.6854 0.0038  I  -107.505    0.781    -8.494    0.091 -0.009065  0.421259 -0.0272490  -107.657    -8.560  
-23 4 8 60042.00 I -0.007830 0.000038  0.423808 0.000018  I-0.0278760 0.0000055  0.6087 0.0038  I  -107.640    0.652    -8.650    0.078 -0.007878  0.423780 -0.0279197  -107.816    -8.694  
-23 4 9 60043.00 I -0.006561 0.000038  0.426287 0.000018  I-0.0284238 0.0000056  0.4841 0.0049  I  -107.755    0.652    -8.772    0.078 -0.006541  0.426318 -0.0284814  -107.930    -8.792  
-23 410 60044.00 I -0.005305 0.000029  0.428798 0.000029  I-0.0288276 0.0000080  0.3097 0.0053  I  -107.827    0.801    -8.868    0.054 -0.005307  0.428835 -0.0288476  -107.977    -8.867  
-23 411 60045.00 I -0.004028 0.000029  0.431385 0.000029  I-0.0290273 0.0000089  0.0875 0.0057  I  -107.805    0.801    -8.980    0.054 -0.004073  0.431351 -0.0290184  -107.906    -8.967  
-23 412 60046.00 I -0.002968 0.000031  0.434138 0.000050  I-0.0290338 0.0000080 -0.0410 0.0060  I  -107.600    0.785    -9.128    0.034 -0.002903  0.434183 -0.0290346  -107.627    -9.117  
-23 413 60047.00 I -0.002348 0.000031  0.436686 0.000050  I-0.0289872 0.0000080 -0.0436 0.0056  I  -107.178    0.785    -9.287    0.034 -0.002436  0.436715 -0.0289857  -107.084    -9.311  
-23 414 60048.00 I -0.001840 0.000031  0.439392 0.000050  I-0.0290013 0.0000079  0.1180 0.0055  I  -106.653    0.785    -9.399    0.034 -0.001750  0.439264 -0.0290056  -106.448    -9.462  
-23 415 60049.00 I -0.001125 0.000031  0.441608 0.000050  I-0.0292515 0.0000076  0.3646 0.0056  I  -106.246    0.785    -9.410    0.034 -0.001196  0.441724 -0.0292618  -106.033    -9.492  
-23 416 60050.00 I  0.000182 0.000014  0.443579 0.000041  I-0.0297608 0.0000078  0.7020 0.0054  I  -106.123    0.685    -9.304    0.024  0.000214  0.443555 -0.0298215  -105.983    -9.387  
-23 417 60051.00 I  0.001680 0.000014  0.445279 0.000041  I-0.0306277 0.0000076  0.9558 0.0053  I  -106.274    0.685    -9.133    0.024  0.001716  0.445308 -0.0306441  -106.240    -9.208  
-23 418 60052.00 I  0.002961 0.000010  0.446948 0.000008  I-0.0316004 0.0000073  0.9934 0.0049  I  -106.537    0.645    -8.986    0.027  0.002942  0.446930 -0.0316096  -106.615    -9.044  
-23 419 60053.00 I  0.004301 0.000010  0.448610 0.000016  I-0.0325682 0.0000062  0.8921 0.0049  I  -106.749    0.656    -8.915    0.028  0.004306  0.448627 -0.0325371  -106.853    -8.950  
-23 420 60054.00 I  0.005751 0.000009  0.450435 0.000016  I-0.0333564 0.0000065  0.7064 0.0045  I  -106.869    0.656    -8.912    0.028  0.005723  0.450456 -0.0333578  -106.967    -8.923  
-23 421 60055.00 I  0.007436 0.000009  0.452646 0.000017  I-0.0339589 0.0000066  0.4546 0.0044  I  -106.962    0.656    -8.964    0.028  0.007430  0.452633 -0.0339749  -107.047    -8.949  
-23 422 60056.00 I  0.009113 0.000005  0.455108 0.000015  I-0.0342653 0.0000058  0.2020 0.0041  I  -107.078    0.708    -9.082    0.032  0.009155  0.455143 -0.0342997  -107.160    -9.039  
-23 423 60057.00 I  0.010722 0.000032  0.457864 0.000027  I-0.0343793 0.0000048 -0.0013 0.0037  I  -107.186    0.889    -9.265    0.103  0.010695  0.457843 -0.0343744  -107.269    -9.198  
-23 424 60058.00 I  0.012620 0.000032  0.460580 0.000027  I-0.0342716 0.0000047 -0.1778 0.0036  I  -107.223    0.889    -9.449    0.103  0.012615  0.460612 -0.0342760  -107.304    -9.366  
-23 425 60059.00 I  0.014991 0.000032  0.462937 0.000024  I-0.0340645 0.0000054 -0.2318 0.0033  I  -107.149    0.914    -9.554    0.112  0.014950  0.462927 -0.0340746  -107.224    -9.466  
-23 426 60060.00 I  0.017320 0.000034  0.465023 0.000040  I-0.0338276 0.0000046 -0.2271 0.0036  I  -106.946    0.956    -9.588    0.147  0.017333  0.465001 -0.0338446  -106.721    -9.586  
-23 427 60061.00 I  0.019414 0.000034  0.467084 0.000039  I-0.0336238 0.0000047 -0.1820 0.0033  I  -106.600    0.956    -9.648    0.147  0.019395  0.467135 -0.0336272  -106.199    -9.723  
-23 428 60062.00 I  0.021469 0.000034  0.469203 0.000039  I-0.0334926 0.0000048 -0.0500 0.0036  I  -106.145    0.956    -9.809    0.147  0.021422  0.469079 -0.0335007  -105.977    -9.882  
-23 429 60063.00 I  0.023805 0.000012  0.470595 0.000032  I-0.0335470 0.0000055  0.1515 0.0036  I  -105.721    1.100   -10.009    0.217  0.023823  0.470667 -0.0335561  -106.132    -9.986  
-23 430 60064.00 I  0.026001 0.000011  0.472110 0.000032  I-0.0337977 0.0000055  0.3592 0.0037  I  -105.525    1.100   -10.095    0.217  0.025987  0.472089 -0.0338124  -105.944   -10.067  
-23 5 1 60065.00 I  0.027599 0.000016  0.473432 0.000033  I-0.0342600 0.0000049  0.5509 0.0041  I  -105.663    1.087    -9.971    0.185  0.027605  0.473468 -0.0342084  -106.095    -9.946  
-23 5 2 60066.00 I  0.028833 0.000012  0.474628 0.000010  I-0.0348518 0.0000062  0.5997 0.0033  I  -106.054    1.082    -9.692    0.168  0.028796  0.474630 -0.0347850  -105.942    -9.706  
-23 5 3 60067.00 I  0.030246 0.000032  0.475672 0.000011  I-0.0354574 0.0000044  0.6426 0.0040  I  -106.495    0.999    -9.413    0.131  0.030234  0.475690 -0.0354724  -106.395    -9.387  
-23 5 4 60068.00 I  0.031946 0.000032  0.476548 0.000012  I-0.0361452 0.0000050  0.7103 0.0034  I  -106.824    0.999    -9.262    0.131  0.031924  0.476551 -0.0361704  -106.827    -9.225  
-23 5 5 60069.00 I  0.033832 0.000032  0.477617 0.000014  I-0.0368150 0.0000051  0.5891 0.0037  I  -107.028    0.999    -9.271    0.131  0.033840  0.477643 -0.0368208  -107.154    -9.237  
-23 5 6 60070.00 I  0.035731 0.000032  0.478662 0.000014  I-0.0373353 0.0000055  0.5038 0.0043  I  -107.195    0.999    -9.407    0.131  0.035678  0.478685 -0.0373656  -107.390    -9.396  
-23 5 7 60071.00 I  0.037835 0.000038  0.479801 0.000033  I-0.0377853 0.0000068  0.3067 0.0048  I  -107.376    0.943    -9.611    0.159  0.037872  0.479777 -0.0377721  -107.589    -9.635  
-23 5 8 60072.00 I  0.039835 0.000038  0.481253 0.000033  I-0.0379541 0.0000078  0.1259 0.0062  I  -107.496    0.943    -9.826    0.159  0.039787  0.481291 -0.0379959  -107.700    -9.885  
-23 5 9 60073.00 I  0.041721 0.000025  0.482657 0.000033  I-0.0380837 0.0000104  0.0849 0.0057  I  -107.431    1.016   -10.005    0.224  0.041742  0.482696 -0.0381001  -107.603   -10.090  
-23 510 60074.00 I  0.043549 0.000025  0.484306 0.000033  I-0.0381445 0.0000084  0.1057 0.0066  I  -107.132    1.018   -10.120    0.189  0.043548  0.484305 -0.0381955  -107.267   -10.183  
-23 511 60075.00 I  0.045317 0.000025  0.485513 0.000032  I-0.0383695 0.0000081  0.3496 0.0059  I  -106.677    1.018   -10.168    0.189  0.045281  0.485514 -0.0383861  -106.770   -10.195  
-23 512 60076.00 I  0.047287 0.000025  0.486627 0.000033  I-0.0388384 0.0000083  0.5774 0.0057  I  -106.221    1.018   -10.157    0.189  0.047344  0.486618 -0.0388214  -106.269   -10.150  
-23 513 60077.00 I  0.049462 0.000007  0.487745 0.000011  I-0.0395345 0.0000081  0.8357 0.0050  I  -105.906    1.021   -10.091    0.134  0.049455  0.487750 -0.0395385  -105.913   -10.091  
-23 514 60078.00 I  0.052351 0.000021  0.489079 0.000015  I-0.0405267 0.0000055  1.1447 0.0049  I  -105.814    1.098    -9.976    0.174  0.052341  0.489096 -0.0405378  -105.788   -10.004  
-23 515 60079.00 I  0.055850 0.000021  0.490657 0.000016  I-0.0417799 0.0000054  1.3217 0.0039  I  -105.949    1.098    -9.820    0.174  0.055853  0.490619 -0.0417757  -105.905    -9.881  
-23 516 60080.00 I  0.059214 0.000021  0.492183 0.000017  I-0.0431017 0.0000055  1.2935 0.0045  I  -106.246    1.158    -9.639    0.195  0.059171  0.492264 -0.0430984  -106.202    -9.725  
-23 517 60081.00 I  0.062101 0.000027  0.493474 0.000035  I-0.0443110 0.0000071  1.0976 0.0044  I  -106.590    1.083    -9.456    0.182  0.062111  0.493466 -0.0442928  -106.606    -9.528  
-23 518 60082.00 I  0.064534 0.000027  0.494600 0.000036  I-0.0452743 0.0000068  0.8337 0.0049  I  -106.858    1.083    -9.326    0.182  0.064515  0.494600 -0.0452544  -106.953    -9.369  
-23 519 60083.00 I  0.066927 0.000027  0.495695 0.000035  I-0.0459526 0.0000068  0.4923 0.0064  I  -106.992    1.083    -9.319    0.182  0.066867  0.495722 -0.0459063  -107.164    -9.334  
-23 520 60084.00 I  0.069370 0.000019  0.496665 0.000034  I-0.0462786 0.0000109  0.2101 0.0062  I  -107.042    0.667    -9.464    0.128  0.069368  0.496634 -0.0462641  -107.252    -9.474  
-23 521 60085.00 I  0.071647 0.000024  0.497526 0.000039  I-0.0463878 0.0000103 -0.0270 0.0075  I  -107.106    0.718    -9.696    0.098  0.071680  0.497569 -0.0463853  -107.324    -9.715  
-23 522 60086.00 I  0.073702 0.000024  0.498180 0.000039  I-0.0462355 0.0000103 -0.2312 0.0069  I  -107.220    0.718    -9.884    0.098  0.073653  0.498156 -0.0462514  -107.428    -9.915  
-23 523 60087.00 I  0.076165 0.000017  0.498914 0.000022  I-0.0459752 0.0000093 -0.2859 0.0061  I  -107.332    0.775    -9.945    0.041  0.076168  0.498968 -0.0459896  -107.516    -9.986  
-23 524 60088.00 I  0.079184 0.000042  0.499989 0.000038  I-0.0456707 0.0000064 -0.3195 0.0057  I  -107.371    0.991    -9.924    0.030  0.079160  0.500036 -0.0456668  -107.507    -9.957  
-23 525 60089.00 I  0.082209 0.000042  0.501053 0.000038  I-0.0453531 0.0000066 -0.3023 0.0046  I  -107.298    0.991    -9.944    0.030  0.082179  0.501016 -0.0453568  -107.375    -9.963  
-23 526 60090.00 I  0.084839 0.000042  0.502378 0.000038  I-0.0450874 0.0000065 -0.2212 0.0044  I  -107.098    0.991   -10.059    0.030  0.084872  0.502481 -0.0450984  -107.114   -10.061  
-23 527 60091.00 I  0.086777 0.000039  0.503682 0.000033  I-0.0449418 0.0000057 -0.0469 0.0043  I  -106.798    1.028   -10.181    0.025  0.086698  0.503700 -0.0449506  -106.780   -10.181  
-23 528 60092.00 I  0.088636 0.000039  0.504444 0.000033  I-0.0449941 0.0000057  0.1288 0.0038  I  -106.539    1.028   -10.168    0.025  0.088656  0.504426 -0.0449906  -106.507   -10.177  
-23 529 60093.00 I  0.090322 0.000043  0.505224 0.000034  I-0.0451723 0.0000051  0.2233 0.0039  I  -106.560    1.089    -9.977    0.075  0.090327  0.505272 -0.0452128  -106.520    -9.999  
-23 530 60094.00 I  0.091895 0.000020  0.506027 0.000023  I-0.0454411 0.0000054  0.3192 0.0040  I  -106.992    1.090    -9.702    0.116  0.091878  0.506018 -0.0454994  -106.948    -9.740  
-23 531 60095.00 I  0.093787 0.000020  0.506965 0.000024  I-0.0457732 0.0000062  0.3028 0.0044  I  -107.682    1.090    -9.464    0.116  0.093791  0.507001 -0.0457819  -107.635    -9.519  
-23 6 1 60096.00 I  0.096362 0.000020  0.507753 0.000024  I-0.0460239 0.0000070  0.2180 0.0046  I  -108.312    1.090    -9.313    0.116  0.096355  0.507784 -0.0460391  -108.261    -9.384  
-23 6 2 60097.00 I  0.099267 0.000020  0.508661 0.000024  I-0.0461937 0.0000068  0.0865 0.0050  I  -108.720    1.090    -9.251    0.116  0.099280  0.508684 -0.0462257  -108.791    -9.317  
-23 6 3 60098.00 I  0.102229 0.000020  0.509360 0.000024  I-0.0461713 0.0000072 -0.1219 0.0051  I  -109.011    1.090    -9.315    0.116  0.102195  0.509333 -0.0462142  -109.187    -9.367  
-23 6 4 60099.00 I  0.105157 0.000012  0.510004 0.000028  I-0.0459320 0.0000075 -0.3840 0.0057  I  -109.291    0.813    -9.540    0.129  0.105220  0.510064 -0.0459633  -109.506    -9.580  
-23 6 5 60100.00 I  0.108076 0.000011  0.510397 0.000019  I-0.0454372 0.0000089 -0.5444 0.0058  I  -109.451    0.669    -9.850    0.140  0.108006  0.510376 -0.0454993  -109.649    -9.884  
-23 6 6 60101.00 I  0.111210 0.000011  0.510768 0.000020  I-0.0449083 0.0000088 -0.5094 0.0062  I  -109.318    0.669   -10.073    0.140  0.111217  0.510811 -0.0449675  -109.453   -10.109  
-23 6 7 60102.00 I  0.114156 0.000020  0.511307 0.000041  I-0.0444265 0.0000085 -0.4501 0.0060  I  -108.947    0.669   -10.097    0.140  0.114187  0.511330 -0.0444769  -108.948   -10.159  
-23 6 8 60103.00 I  0.116579 0.000020  0.511551 0.000041  I-0.0440547 0.0000083 -0.2510 0.0060  I  -108.608    0.669    -9.979    0.140  0.116506  0.511524 -0.0441244  -108.464   -10.073  
-23 6 9 60104.00 I  0.119132 0.000020  0.511751 0.000041  I-0.0439352 0.0000085 -0.0199 0.0070  I  -108.502    0.669    -9.846    0.140  0.119171  0.511814 -0.0439844  -108.237    -9.970  
-23 610 60105.00 I  0.121691 0.000017  0.512167 0.000038  I-0.0440158 0.0000112  0.2137 0.0069  I  -108.589    0.322    -9.758    0.160  0.121697  0.512135 -0.0440725  -108.326    -9.905  
-23 611 60106.00 I  0.123859 0.000049  0.512546 0.000039  I-0.0443161 0.0000109  0.3078 0.0077  I  -108.703    0.883    -9.689    0.263  0.123832  0.512556 -0.0443300  -108.523    -9.845  
-23 612 60107.00 I  0.126117 0.000049  0.512878 0.000038  I-0.0445775 0.0000105  0.2402 0.0072  I  -108.772    0.883    -9.590    0.263  0.126093  0.512902 -0.0446157  -108.701    -9.737  
-23 613 60108.00 I  0.128688 0.000049  0.513085 0.000032  I-0.0447853 0.0000095  0.1390 0.0071  I  -108.870    0.902    -9.441    0.227  0.128655  0.513023 -0.0448327  -108.912    -9.554  
-23 614 60109.00 I  0.131247 0.000049  0.513138 0.000032  I-0.0448216 0.0000096 -0.0639 0.0066  I  -109.082    0.902    -9.257    0.227  0.131265  0.513186 -0.0448926  -109.174    -9.285  
-23 615 60110.00 I  0.133777 0.000049  0.513026 0.000032  I-0.0446568 0.0000093 -0.2690 0.0066  I  -109.349    0.902    -9.116    0.227  0.133765  0.513018 -0.0447062  -109.492    -9.052  
-23 616 60111.00 I  0.136504 0.000049  0.512874 0.000032  I-0.0442576 0.0000091 -0.5523 0.0053  I  -109.517    0.902    -9.134    0.227  0.136473  0.512884 -0.0442808  -109.770    -9.013  
-23 617 60112.00 I  0.139487 0.000017  0.512884 0.000031  I-0.0435763 0.0000052 -0.7634 0.0051  I  -109.522    0.956    -9.375    0.089  0.139533  0.512907 -0.0436680  -109.901    -9.229  
-23 618 60113.00 I  0.142516 0.000017  0.512720 0.000058  I-0.0427858 0.0000046 -0.8094 0.0042  I  -109.462    1.266    -9.754    0.190  0.142445  0.512759 -0.0429057  -109.870    -9.622  
-23 619 60114.00 I  0.145636 0.000020  0.512553 0.000050  I-0.0419677 0.0000066 -0.8249 0.0054  I  -109.475    1.319   -10.064    0.212  0.145679  0.512473 -0.0420518  -109.834    -9.972  
-23 620 60115.00 I  0.148707 0.000020  0.512111 0.000050  I-0.0411443 0.0000097 -0.8157 0.0058  I  -109.600    1.319   -10.143    0.212  0.148651  0.512369 -0.0411848  -109.895   -10.094  
-23 621 60116.00 I  0.152070 0.000019  0.512046 0.000051  I-0.0403426 0.0000096 -0.7877 0.0068  I  -109.794    1.270   -10.022    0.204  0.151998  0.511955 -0.0403854  -110.135    -9.968  
-23 622 60117.00 I  0.155441 0.000019  0.511504 0.000051  I-0.0395953 0.0000096 -0.6806 0.0069  I  -109.986    1.270    -9.876    0.204  0.155498  0.511551 -0.0396589  -110.417    -9.796  
-23 623 60118.00 I  0.158405 0.000019  0.511226 0.000051  I-0.0389782 0.0000099 -0.5830 0.0087  I  -110.093    1.270    -9.818    0.204  0.158323  0.511208 -0.0390256  -110.606    -9.712  
-23 624 60119.00 I  0.161363 0.000019  0.510808 0.000010  I-0.0384429 0.0000145 -0.4444 0.0074  I  -110.025    0.861    -9.788    0.172  0.161368  0.510809 -0.0384982  -110.515    -9.706  
-23 625 60120.00 I  0.164250 0.000020  0.510675 0.000011  I-0.0380781 0.0000109 -0.3396 0.0089  I  -109.834    1.079    -9.657    0.230  0.164234  0.510724 -0.0380713  -110.238    -9.623  
-23 626 60121.00 I  0.167176 0.000020  0.510316 0.000012  I-0.0377435 0.0000102 -0.2953 0.0076  I  -109.805    1.079    -9.425    0.230  0.167176  0.510340 -0.0377554  -110.105    -9.436  
-23 627 60122.00 I  0.170463 0.000009  0.509975 0.000009  I-0.0374955 0.0000105 -0.2271 0.0064  I  -110.250    1.184    -9.238    0.266  0.170433  0.509962 -0.0375206  -110.449    -9.278  
-23 628 60123.00 I  0.173912 0.000013  0.509926 0.000010  I-0.0372672 0.0000077 -0.2251 0.0065  I  -111.134    1.184    -9.202    0.266  0.173953  0.509955 -0.0373143  -111.285    -9.197  
-23 629 60124.00 I  0.177046 0.000013  0.509646 0.000010  I-0.0370212 0.0000075 -0.2954 0.0050  I  -112.044    1.184    -9.253    0.266  0.176991  0.509637 -0.0370420  -112.173    -9.179  
-23 630 60125.00 I  0.180252 0.000013  0.509107 0.000010  I-0.0366539 0.0000064 -0.4332 0.0062  I  -112.629    1.184    -9.273    0.266  0.180263  0.509120 -0.0366739  -112.749    -9.132  
-23 7 1 60126.00 I  0.183656 0.000011  0.508459 0.000009  I-0.0361420 0.0000098 -0.6093 0.0071  I  -112.911    0.322    -9.291    0.160  0.183626  0.508483 -0.0361336  -113.043    -9.133  
-23 7 2 60127.00 I  0.187232 0.000023  0.507864 0.000007  I-0.0354088 0.0000127 -0.8649 0.0090  I  -113.047    1.020    -9.440    0.262  0.187226  0.507848 -0.0353981  -113.199    -9.303  
-23 7 3 60128.00 I  0.190487 0.000023  0.507547 0.000007  I-0.0344549 0.0000150 -0.9924 0.0117  I  -112.999    1.020    -9.704    0.262  0.190492  0.507593 -0.0344896  -113.166    -9.608  
-23 7 4 60129.00 I  0.193222 0.000021  0.507380 0.000006  I-0.0334906 0.0000196 -0.9201 0.0115  I  -112.683    1.020    -9.857    0.262  0.193198  0.507334 -0.0335318  -112.851    -9.818  
-23 7 5 60130.00 I  0.195880 0.000037  0.507029 0.000036  I-0.0326180 0.0000174 -0.8377 0.0132  I  -112.288    0.922    -9.752    0.305  0.195908  0.507073 -0.0326419  -112.408    -9.794  
-23 7 6 60131.00 I  0.198446 0.000037  0.506393 0.000036  I-0.0318640 0.0000178 -0.6088 0.0126  I  -112.164    0.922    -9.517    0.305  0.198426  0.506374 -0.0319144  -112.214    -9.638  
-23 7 7 60132.00 I  0.201252 0.000037  0.505461 0.000036  I-0.0314177 0.0000183 -0.3281 0.0132  I  -112.430    0.922    -9.366    0.305  0.201220  0.505514 -0.0314343  -112.403    -9.552  
-23 7 8 60133.00 I  0.204175 0.000031  0.504523 0.000036  I-0.0311585 0.0000195 -0.1952 0.0119  I  -112.884    0.887    -9.327    0.318  0.204156  0.504535 -0.0311542  -112.760    -9.535  
-23 7 9 60134.00 I  0.206988 0.000033  0.503203 0.000038  I-0.0309690 0.0000152 -0.2371 0.0122  I  -113.259    0.964    -9.275    0.192  0.207001  0.503185 -0.0309623  -113.071    -9.471  
-23 710 60135.00 I  0.209578 0.000033  0.501982 0.000038  I-0.0306718 0.0000146 -0.3165 0.0106  I  -113.459    0.964    -9.156    0.192  0.209533  0.502013 -0.0306936  -113.323    -9.301  
-23 711 60136.00 I  0.212145 0.000011  0.500933 0.000014  I-0.0303096 0.0000149 -0.4752 0.0093  I  -113.573    0.979    -9.034    0.113  0.212151  0.500923 -0.0302988  -113.566    -9.109  
-23 712 60137.00 I  0.214603 0.000013  0.499872 0.000017  I-0.0297125 0.0000115 -0.6604 0.0091  I  -113.758    0.914    -8.970    0.140  0.214585  0.499885 -0.0297092  -113.875    -9.024  
-23 713 60138.00 I  0.216946 0.000013  0.498770 0.000017  I-0.0289484 0.0000104 -0.9666 0.0077  I  -114.077    0.914    -8.972    0.140  0.216926  0.498812 -0.0288524  -114.299    -9.039  
-23 714 60139.00 I  0.219383 0.000013  0.497577 0.000017  I-0.0278009 0.0000103 -1.2081 0.0069  I  -114.420    0.914    -9.068    0.140  0.219379  0.497583 -0.0277983  -114.717    -9.160  
-23 715 60140.00 I  0.221885 0.000008  0.496507 0.000013  I-0.0266107 0.0000092 -1.2142 0.0059  I  -114.616    0.738    -9.315    0.175  0.221871  0.496538 -0.0265972  -114.866    -9.393  
-23 716 60141.00 I  0.224428 0.000009  0.495455 0.000014  I-0.0253389 0.0000058 -1.3213 0.0057  I  -114.633    1.042    -9.686    0.151  0.224374  0.495464 -0.0253009  -114.764    -9.731  
-23 717 60142.00 I  0.226908 0.000009  0.494539 0.000014  I-0.0240248 0.0000068 -1.2585 0.0049  I  -114.584    1.042    -9.996    0.151  0.226953  0.494546 -0.0240270  -114.584   -10.007  
-23 718 60143.00 I  0.228994 0.000007  0.493795 0.000010  I-0.0228508 0.0000078 -1.1091 0.0044  I  -114.589    1.220   -10.031    0.129  0.228983  0.493824 -0.0228538  -114.472   -10.018  
-23 719 60144.00 I  0.231014 0.000013  0.493053 0.000041  I-0.0218066 0.0000057 -0.9597 0.0049  I  -114.684    1.108    -9.771    0.190  0.230996  0.493045 -0.0218364  -114.568    -9.765  
-23 720 60145.00 I  0.233355 0.000013  0.492245 0.000041  I-0.0209746 0.0000059 -0.6808 0.0041  I  -114.832    1.108    -9.416    0.190  0.233340  0.492282 -0.0210160  -114.761    -9.434  
-23 721 60146.00 I  0.235890 0.000012  0.491053 0.000041  I-0.0204262 0.0000059 -0.4583 0.0046  I  -114.949    1.108    -9.171    0.190  0.235893  0.491075 -0.0204242  -114.934    -9.222  
-23 722 60147.00 I  0.238222 0.000011  0.489957 0.000041  I-0.0200288 0.0000070 -0.3233 0.0036  I  -114.933    1.058    -9.045    0.223  0.238218  0.489978 -0.0200295  -114.946    -9.121  
-23 723 60148.00 I  0.240419 0.000016  0.488605 0.000059  I-0.0197761 0.0000040 -0.1989 0.0041  I  -114.779    0.993    -8.917    0.208  0.240409  0.488602 -0.0197499  -114.802    -9.012  
-23 724 60149.00 I  0.242681 0.000016  0.487118 0.000059  I-0.0195908 0.0000042 -0.1953 0.0032  I  -114.706    0.993    -8.765    0.208  0.242675  0.487119 -0.0195468  -114.739    -8.873  
-23 725 60150.00 I  0.244999 0.000013  0.485395 0.000044  I-0.0193684 0.0000051 -0.2431 0.0037  I  -115.043    0.926    -8.727    0.193  0.244998  0.485494 -0.0193720  -115.090    -8.835  
-23 726 60151.00 I  0.247381 0.000032  0.483992 0.000054  I-0.0191007 0.0000061 -0.3026 0.0040  I  -115.853    0.909    -8.917    0.172  0.247369  0.483986 -0.0191211  -115.939    -9.007  
-23 727 60152.00 I  0.249856 0.000032  0.482338 0.000054  I-0.0187258 0.0000061 -0.4742 0.0043  I  -116.766    0.909    -9.225    0.172  0.249864  0.482311 -0.0187234  -116.894    -9.285  
-23 728 60153.00 I  0.252315 0.000032  0.480751 0.000054  I-0.0181420 0.0000061 -0.6765 0.0055  I  -117.331    0.909    -9.431    0.172  0.252271  0.480832 -0.0181468  -117.493    -9.459  
-23 729 60154.00 I  0.254524 0.000030  0.479133 0.000033  I-0.0173864 0.0000092 -0.8380 0.0048  I  -117.450    0.853    -9.484    0.112  0.254520  0.479116 -0.0174005  -117.597    -9.513  
-23 730 60155.00 I  0.256291 0.000043  0.477290 0.000034  I-0.0164859 0.0000074 -0.9399 0.0059  I  -117.288    0.949    -9.533    0.242  0.256321  0.477330 -0.0165264  -117.387    -9.585  
-23 731 60156.00 I  0.257761 0.000043  0.475300 0.000034  I-0.0155659 0.0000074 -0.8641 0.0052  I  -116.942    0.949    -9.639    0.242  0.257717  0.475332 -0.0156145  -116.980    -9.717  
-23 8 1 60157.00 I  0.259498 0.000031  0.473330 0.000010  I-0.0147896 0.0000072 -0.6928 0.0052  I  -116.494    0.994    -9.634    0.296  0.259552  0.473316 -0.0148009  -116.465    -9.735  
-23 8 2 60158.00 I  0.261544 0.000036  0.471664 0.000020  I-0.0142003 0.0000072 -0.4616 0.0053  I  -116.218    1.031    -9.413    0.248  0.261538  0.471686 -0.0141968  -116.134    -9.492  
-23 8 3 60159.00 I  0.263450 0.000036  0.470052 0.000020  I-0.0138929 0.0000077 -0.1509 0.0054  I  -116.383    1.031    -9.185    0.248  0.263444  0.470105 -0.0138930  -116.254    -9.229  
-23 8 4 60160.00 I  0.265539 0.000036  0.468284 0.000020  I-0.0138751 0.0000080  0.0898 0.0063  I  -116.893    1.031    -9.206    0.248  0.265536  0.468247 -0.0138656  -116.730    -9.216  
-23 8 5 60161.00 I  0.267938 0.000019  0.466358 0.000019  I-0.0140318 0.0000099  0.2086 0.0055  I  -117.421    1.099    -9.400    0.143  0.267930  0.466413 -0.0140118  -117.309    -9.399  
-23 8 6 60162.00 I  0.270505 0.000039  0.464869 0.000020  I-0.0142153 0.0000075  0.0966 0.0062  I  -117.808    0.766    -9.472    0.146  0.270493  0.464868 -0.0141542  -117.788    -9.473  
-23 8 7 60163.00 I  0.272840 0.000039  0.463552 0.000020  I-0.0141761 0.0000074 -0.1619 0.0055  I  -118.108    0.766    -9.336    0.146  0.272864  0.463581 -0.0141484  -118.179    -9.345  
-23 8 8 60164.00 I  0.274695 0.000034  0.462185 0.000009  I-0.0139122 0.0000080 -0.3582 0.0049  I  -118.350    0.454    -9.201    0.147  0.274685  0.462231 -0.0139140  -118.493    -9.221  
-23 8 9 60165.00 I  0.276338 0.000043  0.460643 0.000044  I-0.0134468 0.0000064 -0.5930 0.0049  I  -118.507    0.689    -9.242    0.146  0.276337  0.460613 -0.0134271  -118.588    -9.279  
-23 810 60166.00 I  0.277800 0.000043  0.458740 0.000044  I-0.0127105 0.0000058 -0.8748 0.0042  I  -118.635    0.689    -9.397    0.146  0.277790  0.458807 -0.0127031  -118.608    -9.447  
-23 811 60167.00 I  0.279014 0.000043  0.456470 0.000044  I-0.0117167 0.0000054 -1.0981 0.0049  I  -118.788    0.689    -9.530    0.146  0.278994  0.456494 -0.0117351  -118.653    -9.582  
-23 812 60168.00 I  0.279961 0.000027  0.454691 0.000043  I-0.0105583 0.0000079 -1.1895 0.0045  I  -118.897    0.890    -9.634    0.144  0.279970  0.454733 -0.0106076  -118.715    -9.638  
-23 813 60169.00 I  0.280815 0.000030  0.452608 0.000043  I-0.0093774 0.0000071 -1.1620 0.0058  I  -118.849    0.890    -9.775    0.144  0.280771  0.452604 -0.0094177  -118.658    -9.705  
-23 814 60170.00 I  0.281797 0.000030  0.450668 0.000043  I-0.0082372 0.0000084 -1.1260 0.0075  I  -118.662    0.890    -9.901    0.144  0.281823  0.450679 -0.0082485  -118.477    -9.763  
-23 815 60171.00 I  0.282776 0.000014  0.448851 0.000008  I-0.0071514 0.0000131 -1.0120 0.0060  I  -118.461    0.322    -9.839    0.160  0.282744  0.448904 -0.0071781  -118.294    -9.656  
-23 816 60172.00 I  0.283528 0.000015  0.447043 0.000011  I-0.0062492 0.0000086 -0.7901 0.0080  I  -118.336    0.988    -9.510    0.130  0.283572  0.447025 -0.0062732  -118.177    -9.364  
-23 817 60173.00 I  0.284165 0.000015  0.445125 0.000011  I-0.0055512 0.0000091 -0.6283 0.0063  I  -118.283    0.988    -9.070    0.130  0.284154  0.445183 -0.0055690  -118.140    -8.999  
-23 818 60174.00 I  0.285204 0.000015  0.442935 0.000011  I-0.0049913 0.0000091 -0.4702 0.0066  I  -118.248    0.988    -8.774    0.130  0.285203  0.442912 -0.0050148  -118.142    -8.791  
-23 819 60175.00 I  0.286554 0.000005  0.440625 0.000008  I-0.0046028 0.0000095 -0.3359 0.0063  I  -118.185    0.988    -8.720    0.130  0.286566  0.440690 -0.0045717  -118.160    -8.828  
-23 820 60176.00 I  0.287722 0.000006  0.438142 0.000008  I-0.0042598 0.0000086 -0.3806 0.0066  I  -118.086    0.988    -8.795    0.130  0.287747  0.438093 -0.0041923  -118.159    -8.978  
-23 821 60177.00 I  0.288642 0.000034  0.435411 0.000010  I-0.0038322 0.0000091 -0.4533 0.0072  I  -118.042    0.779    -8.880    0.189  0.288671  0.435493 -0.0038044  -118.243    -9.084  
-23 822 60178.00 I  0.289781 0.000034  0.432402 0.000007  I-0.0033617 0.0000115 -0.5004 0.0069  I  -118.232    0.633    -9.000    0.218  0.289769  0.432356 -0.0033527  -118.537    -9.172  
-23 823 60179.00 I  0.291331 0.000037  0.429785 0.000009  I-0.0028134 0.0000105 -0.6016 0.0076  I  -118.741    0.633    -9.239    0.218  0.291358  0.429819 -0.0027933  -119.045    -9.335  
-23 824 60180.00 I  0.292553 0.000037  0.427254 0.000009  I-0.0021328 0.0000098 -0.7800 0.0072  I  -119.370    0.633    -9.548    0.218  0.292539  0.427299 -0.0020899  -119.401    -9.502  
-23 825 60181.00 I  0.294079 0.000037  0.424788 0.000010  I-0.0012525 0.0000099 -0.9613 0.0070  I  -119.769    0.633    -9.752    0.218  0.294147  0.424781 -0.0012425  -119.430    -9.558  
-23 826 60182.00 I  0.296071 0.000037  0.422621 0.000010  I-0.0002478 0.0000099 -1.0300 0.0058  I  -119.760    0.633    -9.759    0.218  0.296042  0.422672 -0.0002644  -119.256    -9.553  
-23 827 60183.00 I  0.298285 0.000017  0.420632 0.000040  I 0.0007720 0.0000062 -0.9922 0.0057  I  -119.427    0.993    -9.656    0.251  0.298312  0.420663  0.0007542  -118.937    -9.547  
-23 828 60184.00 I  0.300342 0.000017  0.418964 0.000040  I 0.0017079 0.0000058 -0.8685 0.0044  I  -118.942    0.993    -9.519    0.251  0.300336  0.418954  0.0017213  -118.543    -9.548  
-23 829 60185.00 I  0.302083 0.000010  0.417491 0.000040  I 0.0024623 0.0000063 -0.6049 0.0047  I  -118.517    0.993    -9.273    0.251  0.302082  0.417627  0.0024765  -118.239    -9.441  
-23 830 60186.00 I  0.303511 0.000011  0.416416 0.000043  I 0.0028563 0.0000074 -0.1571 0.0048  I  -118.429    0.985    -8.902    0.246  0.303509  0.416370  0.0028590  -118.177    -9.106  
-23 831 60187.00 I  0.304427 0.000011  0.414916 0.000043  I 0.0028237 0.0000072  0.1492 0.0052  I  -118.782    0.985    -8.655    0.246  0.304481  0.414958  0.0028596  -118.523    -8.848  
-23 9 1 60188.00 I  0.304732 0.000011  0.413285 0.000043  I 0.0025928 0.0000072  0.3508 0.0061  I  -119.276    0.985    -8.786    0.246  0.304685  0.413225  0.0025855  -119.010    -8.951  
-23 9 2 60189.00 I  0.304823 0.000009  0.411156 0.000017  I 0.0021720 0.0000098  0.4028 0.0059  I  -119.530    0.903    -9.157    0.177  0.304825  0.411174  0.0022047  -119.329    -9.293  
-23 9 3 60190.00 I  0.304678 0.000009  0.409255 0.000017  I 0.0018676 0.0000094  0.2137 0.0066  I  -119.571    0.903    -9.352    0.177  0.304727  0.409265  0.0019255  -119.472    -9.461  
-23 9 4 60191.00 I  0.304312 0.000028  0.407154 0.000038  I 0.0017751 0.0000088 -0.0669 0.0065  I  -119.713    0.666    -9.218    0.072  0.304257  0.407156  0.0018953  -119.709    -9.301  
-23 9 5 60192.00 I  0.304214 0.000028  0.404867 0.000035  I 0.0020446 0.0000089 -0.4771 0.0057  I  -120.030    0.643    -9.030    0.052  0.304229  0.404886  0.0021594  -120.091    -9.090  
-23 9 6 60193.00 I  0.304249 0.000030  0.402291 0.000050  I 0.0026777 0.0000074 -0.7324 0.0059  I  -120.278    0.813    -9.080    0.069  0.304276  0.402304  0.0027036  -120.353    -9.124  
-23 9 7 60194.00 I  0.304268 0.000029  0.399235 0.000050  I 0.0034656 0.0000077 -0.8561 0.0055  I  -120.302    0.813    -9.314    0.069  0.304265  0.399324  0.0034693  -120.231    -9.351  
-23 9 8 60195.00 I  0.305009 0.000029  0.395835 0.000050  I 0.0043858 0.0000081 -0.9673 0.0057  I  -120.203    0.813    -9.477    0.069  0.305032  0.395644  0.0043809  -119.988    -9.520  
-23 9 9 60196.00 I  0.306212 0.000029  0.392387 0.000050  I 0.0053634 0.0000083 -0.9680 0.0060  I  -120.070    0.813    -9.465    0.069  0.306254  0.392502  0.0053793  -119.832    -9.558  
-23 910 60197.00 I  0.307414 0.000036  0.389478 0.000037  I 0.0063268 0.0000089 -0.9837 0.0063  I  -119.851    0.988    -9.393    0.089  0.307408  0.389458  0.0063492  -119.671    -9.536  
-23 911 60198.00 I  0.308549 0.000035  0.386753 0.000037  I 0.0072722 0.0000094 -0.8238 0.0072  I  -119.521    0.988    -9.356    0.089  0.308542  0.386795  0.0072245  -119.423    -9.464  
-23 912 60199.00 I  0.309303 0.000034  0.384486 0.000013  I 0.0079686 0.0000113 -0.6466 0.0068  I  -119.184    0.953    -9.281    0.088  0.309341  0.384450  0.0079652  -119.169    -9.303  
-23 913 60200.00 I  0.309641 0.000034  0.382304 0.000015  I 0.0085612 0.0000099 -0.4569 0.0076  I  -118.939    0.963    -9.048    0.147  0.309615  0.382316  0.0085199  -118.964    -9.046  
-23 914 60201.00 I  0.309654 0.000034  0.380127 0.000016  I 0.0088801 0.0000102 -0.2605 0.0070  I  -118.776    0.963    -8.698    0.147  0.309657  0.380143  0.0088938  -118.809    -8.719  
-23 915 60202.00 I  0.309698 0.000034  0.377600 0.000018  I 0.0091239 0.0000098 -0.1892 0.0076  I  -118.641    0.963    -8.438    0.147  0.309721  0.377614  0.0091238  -118.667    -8.501  
-23 916 60203.00 I  0.309780 0.000009  0.374699 0.000018  I 0.0092421 0.0000113 -0.0685 0.0066  I  -118.536    0.989    -8.420    0.219  0.309751  0.374744  0.0092593  -118.529    -8.503  
-23 917 60204.00 I  0.309662 0.000023  0.371808 0.000019  I 0.0093008 0.0000089 -0.0673 0.0070  I  -118.489    1.047    -8.594    0.154  0.309757  0.371760  0.0093601  -118.451    -8.682  
-23 918 60205.00 I  0.308973 0.000024  0.369030 0.000020  I 0.0094187 0.0000082 -0.1921 0.0058  I  -118.502    1.047    -8.796    0.154  0.308886  0.369108  0.0095049  -118.457    -8.880  
-23 919 60206.00 I  0.308191 0.000024  0.366279 0.000035  I 0.0096948 0.0000074 -0.3463 0.0055  I  -118.573    0.962    -8.933    0.088  0.308208  0.366181  0.0097240  -118.563    -9.000  
-23 920 60207.00 I  0.307449 0.000024  0.363548 0.000035  I 0.0100811 0.0000072 -0.4098 0.0052  I  -118.734    0.962    -9.034    0.088  0.307457  0.363678  0.0100660  -118.869    -9.060  
-23 921 60208.00 I  0.306792 0.000024  0.360712 0.000034  I 0.0105407 0.0000072 -0.5521 0.0052  I  -118.971    0.962    -9.142    0.088  0.306721  0.360579  0.0105661  -119.283    -9.118  
-23 922 60209.00 I  0.306356 0.000024  0.357776 0.000034  I 0.0111897 0.0000074 -0.7074 0.0051  I  -119.149    0.962    -9.235    0.088  0.306436  0.357851  0.0112184  -119.529    -9.192  
-23 923 60210.00 I  0.305729 0.000011  0.354968 0.000033  I 0.0119276 0.0000071 -0.7788 0.0060  I  -119.095    0.673    -9.260    0.042  0.305659  0.354987  0.0119856  -119.445    -9.228  
-23 924 60211.00 I  0.305040 0.000010  0.351923 0.000033  I 0.0127089 0.0000094 -0.7350 0.0073  I  -118.757    0.673    -9.207    0.042  0.305106  0.351922  0.0127431  -119.033    -9.199  
-23 925 60212.00 I  0.304196 0.000019  0.348963 0.000049  I 0.0133433 0.0000127 -0.5283 0.0078  I  -118.270    0.749    -9.062    0.131  0.304158  0.349002  0.0133969  -118.449    -9.085  
-23 926 60213.00 I  0.303376 0.000019  0.346195 0.000049  I 0.0137617 0.0000124 -0.3104 0.0087  I  -117.901    0.749    -8.772    0.131  0.303399  0.346155  0.0138149  -117.987    -8.827  
-23 927 60214.00 I  0.302828 0.000020  0.343401 0.000049  I 0.0139035 0.0000118  0.0891 0.0085  I  -117.908    0.698    -8.368    0.099  0.302795  0.343537  0.0138975  -117.925    -8.449  
-23 928 60215.00 I  0.302617 0.000020  0.340971 0.000049  I 0.0135930 0.0000117  0.4601 0.0083  I  -118.278    0.698    -8.079    0.099  0.302657  0.340917  0.0135997  -118.314    -8.163  
-23 929 60216.00 I  0.302176 0.000020  0.338726 0.000049  I 0.0130375 0.0000117  0.6686 0.0080  I  -118.651    0.698    -8.142    0.099  0.302155  0.338760  0.0130375  -118.728    -8.223  
-23 930 60217.00 I  0.301754 0.000020  0.336452 0.000049  I 0.0123116 0.0000109  0.7097 0.0076  I  -118.680    0.698    -8.473    0.099  0.301747  0.336425  0.0123503  -118.801    -8.546  
-2310 1 60218.00 I  0.301359 0.000010  0.334278 0.000015  I 0.0117044 0.0000096  0.4920 0.0070  I  -118.476    0.632    -8.712    0.074  0.301385  0.334305  0.0117122  -118.634    -8.774  
-2310 2 60219.00 I  0.300724 0.000010  0.332011 0.000015  I 0.0113497 0.0000089  0.2079 0.0063  I  -118.449    0.632    -8.661    0.074  0.300711  0.331993  0.0113503  -118.635    -8.711  
-2310 3 60220.00 I  0.299820 0.000008  0.329492 0.000014  I 0.0113050 0.0000083 -0.1255 0.0053  I  -118.738    0.586    -8.503    0.069  0.299884  0.329534  0.0113093  -118.934    -8.547  
-2310 4 60221.00 I  0.298799 0.000012  0.326812 0.000016  I 0.0115851 0.0000058 -0.4121 0.0049  I  -119.039    0.744    -8.515    0.072  0.298717  0.326782  0.0115775  -119.190    -8.569  
-2310 5 60222.00 I  0.298187 0.000012  0.324029 0.000016  I 0.0120882 0.0000053 -0.5757 0.0042  I  -119.046    0.744    -8.693    0.072  0.298232  0.324037  0.0120742  -119.132    -8.761  
-2310 6 60223.00 I  0.297917 0.000013  0.321483 0.000017  I 0.0127152 0.0000061 -0.6753 0.0050  I  -118.775    0.744    -8.803    0.072  0.297920  0.321485  0.0127240  -118.796    -8.884  
-2310 7 60224.00 I  0.297528 0.000013  0.319100 0.000017  I 0.0133915 0.0000085 -0.6331 0.0051  I  -118.399    0.915    -8.717    0.074  0.297532  0.319119  0.0133996  -118.390    -8.787  
-2310 8 60225.00 I  0.296859 0.000013  0.316814 0.000018  I 0.0139419 0.0000082 -0.4723 0.0058  I  -117.994    0.910    -8.539    0.046  0.296876  0.316797  0.0139877  -117.978    -8.588  
-2310 9 60226.00 I  0.295926 0.000012  0.314602 0.000019  I 0.0143494 0.0000080 -0.3514 0.0065  I  -117.586    0.910    -8.425    0.046  0.295928  0.314663  0.0144054  -117.574    -8.450  
-231010 60227.00 I  0.294937 0.000010  0.312309 0.000017  I 0.0146306 0.0000100 -0.1881 0.0054  I  -117.260    0.907    -8.368    0.010  0.294921  0.312271  0.0146356  -117.258    -8.374  
-231011 60228.00 I  0.293751 0.000010  0.309885 0.000019  I 0.0146839 0.0000073  0.1003 0.0061  I  -117.098    0.801    -8.237    0.070  0.293786  0.309909  0.0146710  -117.114    -8.254  
-231012 60229.00 I  0.292362 0.000010  0.307301 0.000019  I 0.0144884 0.0000071  0.2135 0.0050  I  -117.071    0.801    -7.976    0.070  0.292342  0.307369  0.0145299  -117.105    -8.014  
-231013 60230.00 I  0.291451 0.000011  0.304797 0.000018  I 0.0142796 0.0000068  0.2585 0.0046  I  -117.090    0.801    -7.711    0.070  0.291417  0.304741  0.0142940  -117.141    -7.774  
-231014 60231.00 I  0.290930 0.000011  0.302891 0.000016  I 0.0139537 0.0000059  0.3564 0.0043  I  -117.133    0.739    -7.622    0.089  0.290959  0.302931  0.0139979  -117.183    -7.692  
-231015 60232.00 I  0.290251 0.000011  0.301036 0.000015  I 0.0136227 0.0000053  0.2865 0.0036  I  -117.230    0.739    -7.756    0.089  0.290206  0.301059  0.0136690  -117.269    -7.821  
-231016 60233.00 I  0.289563 0.000014  0.298937 0.000016  I 0.0133971 0.0000040  0.1676 0.0034  I  -117.345    0.652    -7.990    0.063  0.289556  0.298935  0.0134187  -117.374    -8.045  
-231017 60234.00 I  0.288900 0.000013  0.296734 0.000014  I 0.0132934 0.0000041  0.0312 0.0033  I  -117.377    0.599    -8.162    0.035  0.288888  0.296768  0.0133241  -117.400    -8.202  
-231018 60235.00 I  0.288074 0.000015  0.294663 0.000014  I 0.0133560 0.0000053 -0.1692 0.0031  I  -117.283    0.588    -8.211    0.038  0.288061  0.294608  0.0133850  -117.311    -8.232  
-231019 60236.00 I  0.286787 0.000015  0.292871 0.000014  I 0.0136095 0.0000047 -0.3028 0.0035  I  -117.130    0.588    -8.193    0.038  0.286823  0.292913  0.0136196  -117.185    -8.186  
-231020 60237.00 I  0.285225 0.000015  0.291132 0.000015  I 0.0139197 0.0000047 -0.3107 0.0034  I  -116.962    0.588    -8.189    0.038  0.285166  0.291121  0.0139436  -117.049    -8.158  
-231021 60238.00 I  0.283861 0.000016  0.289337 0.000015  I 0.0142165 0.0000050 -0.2755 0.0041  I  -116.700    0.588    -8.229    0.038  0.283894  0.289336  0.0142475  -116.787    -8.196  
-231022 60239.00 I  0.282750 0.000014  0.287380 0.000016  I 0.0144456 0.0000066 -0.1650 0.0040  I  -116.249    0.702    -8.269    0.061  0.282734  0.287395  0.0144590  -116.313    -8.253  
-231023 60240.00 I  0.281940 0.000015  0.284979 0.000015  I 0.0145045 0.0000063  0.0716 0.0044  I  -115.678    0.702    -8.218    0.061  0.281945  0.284996  0.0144889  -115.709    -8.227  
-231024 60241.00 I  0.281311 0.000013  0.282384 0.000015  I 0.0142729 0.0000059  0.3967 0.0039  I  -115.236    0.743    -8.008    0.063  0.281319  0.282356  0.0142581  -115.235    -8.043  
-231025 60242.00 I  0.280643 0.000014  0.279904 0.000018  I 0.0137408 0.0000047  0.6327 0.0038  I  -115.157    0.723    -7.667    0.083  0.280625  0.279902  0.0137506  -115.163    -7.716  
-231026 60243.00 I  0.280187 0.000014  0.277738 0.000017  I 0.0130350 0.0000047  0.7863 0.0033  I  -115.415    0.723    -7.358    0.083  0.280203  0.277777  0.0130086  -115.441    -7.417  
-231027 60244.00 I  0.280032 0.000013  0.275710 0.000016  I 0.0122055 0.0000046  0.8279 0.0033  I  -115.708    0.723    -7.258    0.083  0.280001  0.275702  0.0121805  -115.756    -7.323  
-231028 60245.00 I  0.280040 0.000012  0.274099 0.000014  I 0.0114610 0.0000045  0.6242 0.0030  I  -115.752    0.696    -7.366    0.105  0.280015  0.274097  0.0114735  -115.828    -7.433  
-231029 60246.00 I  0.279553 0.000019  0.272844 0.000018  I 0.0110035 0.0000039  0.2814 0.0027  I  -115.593    0.669    -7.505    0.085  0.279560  0.272859  0.0110296  -115.697    -7.571  
-231030 60247.00 I  0.278176 0.000019  0.271662 0.000018  I 0.0108838 0.0000031 -0.0183 0.0029  I  -115.523    0.669    -7.534    0.085  0.278140  0.271640  0.0108288  -115.650    -7.597  
-231031 60248.00 I  0.276358 0.000017  0.270311 0.000015  I 0.0110115 0.0000043 -0.2321 0.0025  I  -115.687    0.639    -7.506    0.055  0.276348  0.270303  0.0109909  -115.831    -7.561  
-2311 1 60249.00 I  0.274620 0.000020  0.268283 0.000018  I 0.0113202 0.0000039 -0.3626 0.0029  I  -115.899    0.728    -7.547    0.041  0.274569  0.268315  0.0113342  -116.023    -7.580  
-2311 2 60250.00 I  0.273173 0.000020  0.266200 0.000018  I 0.0117332 0.0000040 -0.4828 0.0029  I  -115.878    0.728    -7.654    0.041                                                     
-2311 3 60251.00 I  0.271880 0.000020  0.264336 0.000020  I 0.0122554 0.0000043 -0.5118 0.0039  I  -115.553    0.728    -7.704    0.041                                                     
-2311 4 60252.00 I  0.270960 0.000013  0.262659 0.000016  I 0.0127070 0.0000068 -0.3913 0.0041  I  -115.058    0.818    -7.627    0.021                                                     
-2311 5 60253.00 I  0.270122 0.000014  0.261236 0.000017  I 0.0130144 0.0000069 -0.2000 0.0050  I  -114.549    0.870    -7.500    0.131                                                     
-2311 6 60254.00 I  0.269206 0.000015  0.259834 0.000017  I 0.0131092 0.0000072 -0.0153 0.0060  I  -114.119    0.870    -7.430    0.131                                                     
-2311 7 60255.00 I  0.268234 0.000011  0.258527 0.000015  I 0.0130391 0.0000098  0.1870 0.0058  I  -113.836    0.922    -7.403    0.188                                                     
-2311 8 60256.00 I  0.266811 0.000013  0.257164 0.000016  I 0.0127598 0.0000090  0.3154 0.0070  I  -113.751    0.887    -7.293    0.186                                                     
-2311 9 60257.00 I  0.265197 0.000013  0.255659 0.000015  I 0.0124248 0.0000100  0.3942 0.0066  I  -113.845    0.887    -7.028    0.186                                                     
-231110 60258.00 I  0.263482 0.000012  0.254388 0.000014  I 0.0119499 0.0000097  0.5375 0.0075  I  -114.034    0.887    -6.697    0.186                                                     
-231111 60259.00 I  0.261648 0.000011  0.252856 0.000013  I 0.0113960 0.0000112  0.5421 0.0069  I  -114.241    0.714    -6.480    0.177                                                     
-231112 60260.00 I  0.259929 0.000013  0.251266 0.000015  I 0.0109204 0.0000098  0.3824 0.0074  I  -114.426    0.981    -6.489    0.088                                                     
-231113 60261.00 I  0.258270 0.000012  0.249709 0.000015  I 0.0106139 0.0000097  0.2745 0.0077  I  -114.548    0.981    -6.677    0.088                                                     
-231114 60262.00 I  0.256528 0.000010  0.248151 0.000013  I 0.0103990 0.0000118  0.0837 0.0067  I  -114.547    1.078    -6.891    0.018                                                     
-231115 60263.00 I  0.254567 0.000010  0.246730 0.000012  I 0.0104590 0.0000092 -0.1448 0.0073  I  -114.397    0.937    -7.011    0.064                                                     
-231116 60264.00 I  0.252443 0.000010  0.245077 0.000012  I 0.0106306 0.0000087 -0.1995 0.0063  I  -114.142    0.937    -7.020    0.064                                                     
-231117 60265.00 I  0.250375 0.000010  0.242944 0.000012  I 0.0108548 0.0000086 -0.2446 0.0061  I  -113.840    0.937    -6.986    0.064                                                     
-231118 60266.00 I  0.248426 0.000006  0.240394 0.000007  I 0.0111057 0.0000085 -0.2475 0.0057  I  -113.496    0.872    -6.981    0.084                                                     
-231119 60267.00 I  0.246658 0.000011  0.238111 0.000011  I 0.0113002 0.0000076 -0.1017 0.0057  I  -113.091    0.863    -7.010    0.088                                                     
-231120 60268.00 I  0.245309 0.000011  0.236090 0.000012  I 0.0112875 0.0000075  0.1090 0.0054  I  -112.671    0.863    -7.009    0.088                                                     
-231121 60269.00 I  0.244544 0.000011  0.234519 0.000013  I 0.0110953 0.0000076  0.2806 0.0053  I  -112.373    0.850    -6.910    0.093                                                     
-231122 60270.00 I  0.243514 0.000014  0.233440 0.000020  I 0.0107424 0.0000074  0.4040 0.0052  I  -112.324    0.883    -6.703    0.130                                                     
-231123 60271.00 I  0.242040 0.000013  0.232223 0.000019  I 0.0103236 0.0000072  0.4184 0.0053  I  -112.517    0.883    -6.454    0.130                                                     
-231124 60272.00 I  0.240930 0.000013  0.231317 0.000019  I 0.0099105 0.0000077  0.4183 0.0063  I  -112.790    0.883    -6.252    0.130                                                     
-231125 60273.00 I  0.239752 0.000010  0.230762 0.000017  I 0.0095249 0.0000104  0.3047 0.0060  I  -112.951    1.000    -6.146    0.207                                                     
-231126 60274.00 I  0.238314 0.000011  0.230139 0.000024  I 0.0093608 0.0000093  0.0119 0.0068  I  -112.934    0.806    -6.130    0.145                                                     
-231127 60275.00 I  0.236335 0.000011  0.229437 0.000023  I 0.0094871 0.0000089 -0.2390 0.0072  I  -112.833    0.806    -6.184    0.145                                                     
-231128 60276.00 I  0.233892 0.000007  0.228517 0.000018  I 0.0098250 0.0000109 -0.4484 0.0063  I  -112.773    0.569    -6.297    0.045                                                     
-231129 60277.00 I  0.231441 0.000011  0.227255 0.000023  I 0.0103674 0.0000089 -0.6084 0.0071  I  -112.763    1.037    -6.441    0.035                                                     
-231130 60278.00 I  0.229064 0.000010  0.225877 0.000023  I 0.0109929 0.0000090 -0.6218 0.0063  I  -112.686    1.037    -6.544    0.035                                                     
-2312 1 60279.00 I  0.226764 0.000011  0.224812 0.000024  I 0.0115679 0.0000088 -0.5059 0.0068  I  -112.437    1.037    -6.542    0.035                                                     
-2312 2 60280.00 I  0.224380 0.000010  0.223864 0.000017  I 0.0119987 0.0000101 -0.3720 0.0062  I  -112.031    1.110    -6.448    0.031                                                     
-2312 3 60281.00 I  0.222059 0.000010  0.222492 0.000023  I 0.0122998 0.0000086 -0.2019 0.0066  I  -111.594    1.094    -6.346    0.056                                                     
-2312 4 60282.00 I  0.219836 0.000010  0.220816 0.000023  I 0.0124140 0.0000085 -0.0663 0.0063  I  -111.247    1.094    -6.290    0.056                                                     
-2312 5 60283.00 I  0.217389 0.000007  0.219194 0.000019  I 0.0124342 0.0000091  0.0639 0.0056  I  -111.053    1.081    -6.234    0.069                                                     
-2312 6 60284.00 I  0.214669 0.000010  0.217471 0.000019  I 0.0122721 0.0000073  0.2363 0.0057  I  -111.045    1.043    -6.087    0.063                                                     
-2312 7 60285.00 I  0.211889 0.000009  0.215809 0.000018  I 0.0119910 0.0000070  0.3203 0.0050  I  -111.248    1.043    -5.830    0.063                                                     
-2312 8 60286.00 I  0.208805 0.000011  0.214045 0.000020  I 0.0116589 0.0000068  0.3219 0.0050  I  -111.643    1.043    -5.565    0.063                                                     
-2312 9 60287.00 I  0.205726 0.000012  0.212089 0.000011  I 0.0113838 0.0000071  0.2137 0.0044  P  -112.144    0.278    -5.436    0.145                                                     
-231210 60288.00 I  0.202964 0.000013  0.210509 0.000013  I 0.0112439 0.0000055  0.0682 0.0047  P  -112.579    0.288    -5.503    0.148                                                     
-231211 60289.00 I  0.200016 0.000091  0.209379 0.000091  I 0.0112422 0.0000063 -0.0617 0.0054  P  -112.841    0.297    -5.721    0.151                                                     
-231212 60290.00 I  0.196861 0.000091  0.208354 0.000091  I 0.0113753 0.0000092 -0.2155 0.0052  P  -112.936    0.304    -5.995    0.154                                                     
-231213 60291.00 I  0.193382 0.000091  0.207682 0.000091  I 0.0116635 0.0000084 -0.3402 0.0065  P  -112.900    0.309    -6.227    0.155                                                     
-231214 60292.00 I  0.189627 0.000091  0.206818 0.000091  I 0.0120386 0.0000091 -0.4135 0.0068  P  -112.734    0.313    -6.335    0.157                                                     
-231215 60293.00 I  0.185838 0.000091  0.205780 0.000091  I 0.0124496 0.0000106 -0.3642 0.0071  P  -112.452    0.316    -6.290    0.158                                                     
-231216 60294.00 I  0.182003 0.000091  0.204694 0.000090  I 0.0126955 0.0000110 -0.1004 0.0085  P  -112.135    0.318    -6.156    0.158                                                     
-231217 60295.00 I  0.178173 0.000091  0.203460 0.000091  I 0.0126371 0.0000134  0.2032 0.0087  P  -111.898    0.319    -6.043    0.159                                                     
-231218 60296.00 I  0.174401 0.000091  0.202306 0.000091  I 0.0123044 0.0000136  0.4608 0.0098  P  -111.799    0.320    -6.005    0.159                                                     
-231219 60297.00 I  0.170707 0.000091  0.201277 0.000091  I 0.0117270 0.0000143  0.6837 0.0102  P  -111.827    0.321    -5.999    0.160                                                     
-231220 60298.00 I  0.167494 0.000091  0.200649 0.000091  I 0.0109682 0.0000151  0.8130 0.0112  P  -111.948    0.321    -5.947    0.160                                                     
-231221 60299.00 I  0.164909 0.000091  0.200449 0.000091  I 0.0101391 0.0000172  0.8282 0.0125  P  -112.135    0.321    -5.821    0.160                                                     
-231222 60300.00 I  0.162550 0.000091  0.200471 0.000091  I 0.0093549 0.0000200  0.7143 0.0122  P  -112.359    0.321    -5.650    0.160                                                     
-231223 60301.00 I  0.160084 0.000091  0.200814 0.000091  I 0.0087393 0.0000173  0.5141 0.0139  P  -112.539    0.322    -5.492    0.160                                                     
-231224 60302.00 I  0.157627 0.000091  0.201258 0.000091  I 0.0083744 0.0000192  0.1709 0.0115  P  -112.564    0.322    -5.411    0.160                                                     
-231225 60303.00 I  0.155018 0.000091  0.201565 0.000091  I 0.0083678 0.0000151 -0.0833 0.0120  P  -112.382    0.322    -5.468    0.160                                                     
-231226 60304.00 I  0.151984 0.000090  0.201780 0.000091  I 0.0084600 0.0000145 -0.0946 0.0094  P  -112.091    0.322    -5.665    0.160                                                     
-231227 60305.00 I  0.148902 0.000091  0.201604 0.000091  I 0.0085339 0.0000111 -0.0365 0.0075  P  -111.860    0.322    -5.913    0.160                                                     
-231228 60306.00 I  0.146109 0.000091  0.201436 0.000091  I 0.0086018 0.0000039                 P  -111.746    0.322    -6.072    0.160                                                     
-231229 60307.00 P  0.143431 0.000601  0.201326 0.000413  P 0.0087926 0.0001080                 P  -111.647    0.322    -6.058    0.160                                                     
-231230 60308.00 P  0.140872 0.000892  0.201406 0.000681  P 0.0089246 0.0002041                 P  -111.444    0.322    -5.922    0.160                                                     
-231231 60309.00 P  0.138402 0.001124  0.201593 0.000911  P 0.0089262 0.0003028                 P  -111.153    0.322    -5.788    0.160                                                     
-24 1 1 60310.00 P  0.135961 0.001324  0.201902 0.001121  P 0.0087932 0.0004021                 P  -110.875    0.322    -5.715    0.160                                                     
-24 1 2 60311.00 P  0.133515 0.001503  0.202297 0.001317  P 0.0085259 0.0005017                 P  -110.685    0.322    -5.645    0.160                                                     
-24 1 3 60312.00 P  0.131068 0.001668  0.202753 0.001501  P 0.0081568 0.0006014                 P  -110.621    0.322    -5.506    0.160                                                     
-24 1 4 60313.00 P  0.128620 0.001821  0.203257 0.001677  P 0.0077535 0.0007012                 P  -110.761    0.322    -5.341    0.160                                                     
-24 1 5 60314.00 P  0.126174 0.001965  0.203798 0.001847  P 0.0073732 0.0007500                 P  -111.160    0.322    -5.285    0.160                                                     
-24 1 6 60315.00 P  0.123737 0.002102  0.204369 0.002010  P 0.0070690 0.0005500                 P  -111.703    0.322    -5.407    0.160                                                     
-24 1 7 60316.00 P  0.121315 0.002232  0.204971 0.002169  P 0.0068884 0.0007548                 P  -112.136    0.322    -5.624    0.160                                                     
-24 1 8 60317.00 P  0.118911 0.002356  0.205605 0.002323  P 0.0068725 0.0009344                 P  -112.332    0.322    -5.818    0.160                                                     
-24 1 9 60318.00 P  0.116526 0.002476  0.206273 0.002473  P 0.0070081 0.0010994                 P  -112.404    0.322    -5.985    0.160                                                     
-24 110 60319.00 P  0.114160 0.002592  0.206978 0.002619  P 0.0071964 0.0012543                 P  -112.454    0.322    -6.186    0.160                                                     
-24 111 60320.00 P  0.111812 0.002704  0.207719 0.002763  P 0.0074010 0.0014016                 P  -112.371    0.322    -6.365    0.160                                                     
-24 112 60321.00 P  0.109483 0.002812  0.208497 0.002904  P 0.0074992 0.0015429                 P  -112.044    0.322    -6.358    0.160                                                     
-24 113 60322.00 P  0.107170 0.002917  0.209312 0.003042  P 0.0073713 0.0016792                 P  -111.637    0.322    -6.123    0.160                                                     
-24 114 60323.00 P  0.104876 0.003020  0.210163 0.003178  P 0.0069690 0.0018113                 P  -111.450    0.322    -5.855    0.160                                                     
-24 115 60324.00 P  0.102599 0.003120  0.211050 0.003311  P 0.0063093 0.0019399                 P  -111.574    0.322    -5.765    0.160                                                     
-24 116 60325.00 P  0.100341 0.003218  0.211972 0.003442  P 0.0054939 0.0020652                 P  -111.856    0.322    -5.840    0.160                                                     
-24 117 60326.00 P  0.098102 0.003313  0.212928 0.003572  P 0.0046649 0.0021877                 P  -112.126    0.322    -5.911    0.160                                                     
-24 118 60327.00 P  0.095883 0.003407  0.213919 0.003700  P 0.0039727 0.0023077                 P  -112.344    0.322    -5.887    0.160                                                     
-24 119 60328.00 P  0.093684 0.003498  0.214944 0.003826  P 0.0035325 0.0024255                 P  -112.529    0.322    -5.812    0.160                                                     
-24 120 60329.00 P  0.091506 0.003588  0.216002 0.003950  P 0.0033869 0.0025411                 P  -112.661    0.322    -5.753    0.160                                                     
-24 121 60330.00 P  0.089350 0.003676  0.217094 0.004073  P 0.0035287 0.0026548                 P  -112.653    0.322    -5.742    0.160                                                     
-24 122 60331.00 P  0.087215 0.003762  0.218219 0.004195  P 0.0039000 0.0027668                 P  -112.428    0.322    -5.808    0.160                                                     
-24 123 60332.00 P  0.085104 0.003848  0.219377 0.004315  P 0.0044178 0.0028772                 P  -112.034    0.322    -5.983    0.160                                                     
-24 124 60333.00 P  0.083016 0.003931  0.220568 0.004434  P 0.0049971 0.0029860                 P  -111.660    0.322    -6.226    0.160                                                     
-24 125 60334.00 P  0.080951 0.004014  0.221790 0.004551  P 0.0055513 0.0030934                 P  -111.462    0.322    -6.395    0.160                                                     
-24 126 60335.00 P  0.078911 0.004095  0.223044 0.004668  P 0.0060126 0.0031995                 P  -111.405    0.322    -6.364    0.160                                                     
-24 127 60336.00 P  0.076896 0.004175  0.224329 0.004783  P 0.0063428 0.0033043                 P  -111.332    0.322    -6.155    0.160                                                     
-24 128 60337.00 P  0.074906 0.004253  0.225646 0.004897  P 0.0065185 0.0034080                 P  -111.158    0.322    -5.931    0.160                                                     
-24 129 60338.00 P  0.072942 0.004331  0.226992 0.005010  P 0.0065372 0.0035105                 P  -110.935    0.322    -5.815    0.160                                                     
-24 130 60339.00 P  0.071004 0.004408  0.228369 0.005123  P 0.0064247 0.0036120                 P  -110.747    0.322    -5.778    0.160                                                     
-24 131 60340.00 P  0.069092 0.004483  0.229776 0.005234  P 0.0062344 0.0037124                 P  -110.653    0.322    -5.738    0.160                                                     
-24 2 1 60341.00 P  0.067208 0.004558  0.231211 0.005344  P 0.0060331 0.0038119                 P  -110.728    0.322    -5.730    0.160                                                     
-24 2 2 60342.00 P  0.065352 0.004632  0.232676 0.005454  P 0.0058882 0.0039105                 P  -111.036    0.322    -5.892    0.160                                                     
-24 2 3 60343.00 P  0.063524 0.004705  0.234168 0.005563  P 0.0058599 0.0040082                 P  -111.472    0.322    -6.256    0.160                                                     
-24 2 4 60344.00 P  0.061725 0.004777  0.235689 0.005670  P 0.0059904 0.0041051                 P  -111.776    0.322    -6.631    0.160                                                     
-24 2 5 60345.00 P  0.059955 0.004848  0.237237 0.005777  P 0.0062960 0.0042012                 P  -111.854    0.322    -6.794    0.160                                                     
-24 2 6 60346.00 P  0.058214 0.004918  0.238812 0.005884  P 0.0067530 0.0042965                 P  -111.935    0.322    -6.786    0.160                                                     
-24 2 7 60347.00 P  0.056504 0.004988  0.240413 0.005989  P 0.0072791 0.0043911                 P  -112.189    0.322    -6.862    0.160                                                     
-24 2 8 60348.00 P  0.054823 0.005057  0.242040 0.006094  P 0.0077489 0.0044849                 P  -112.354    0.322    -7.105    0.160                                                     
-24 2 9 60349.00 P  0.053174 0.005125  0.243693 0.006198  P 0.0080160 0.0045781                 P  -112.074    0.322    -7.256    0.160                                                     
-24 210 60350.00 P  0.051556 0.005193  0.245371 0.006302  P 0.0079636 0.0046706                 P  -111.488    0.322    -7.077    0.160                                                     
-24 211 60351.00 P  0.049969 0.005260  0.247073 0.006404  P 0.0075607 0.0047625                 P  -111.112    0.322    -6.725    0.160                                                     
-24 212 60352.00 P  0.048414 0.005326  0.248800 0.006507  P 0.0068799 0.0048537                 P  -111.194    0.322    -6.551    0.160                                                     
-24 213 60353.00 P  0.046892 0.005392  0.250549 0.006608  P 0.0060742 0.0049444                 P  -111.534    0.322    -6.637    0.160                                                     
-24 214 60354.00 P  0.045402 0.005457  0.252322 0.006709  P 0.0053288 0.0050344                 P  -111.874    0.322    -6.772    0.160                                                     
-24 215 60355.00 P  0.043946 0.005522  0.254117 0.006809  P 0.0047948 0.0051240                 P  -112.151    0.322    -6.823    0.160                                                     
-24 216 60356.00 P  0.042523 0.005585  0.255934 0.006909  P 0.0045527 0.0052129                 P  -112.360    0.322    -6.882    0.160                                                     
-24 217 60357.00 P  0.041133 0.005649  0.257773 0.007008  P 0.0046061 0.0053014                 P  -112.445    0.322    -7.046    0.160                                                     
-24 218 60358.00 P  0.039778 0.005712  0.259632 0.007107  P 0.0048982 0.0053893                 P  -112.372    0.322    -7.249    0.160                                                     
-24 219 60359.00 P  0.038457 0.005774  0.261512 0.007205  P 0.0053414 0.0054768                 P  -112.154    0.322    -7.389    0.160                                                     
-24 220 60360.00 P  0.037171 0.005836  0.263411 0.007303  P 0.0058399 0.0055637                 P  -111.821    0.322    -7.482    0.160                                                     
-24 221 60361.00 P  0.035920 0.005897  0.265330 0.007400  P 0.0063030 0.0056502                 P  -111.449    0.322    -7.587    0.160                                                     
-24 222 60362.00 P  0.034704 0.005958  0.267267 0.007497  P 0.0066557 0.0057362                 P  -111.162    0.322    -7.662    0.160                                                     
-24 223 60363.00 P  0.033524 0.006019  0.269222 0.007593  P 0.0068482 0.0058218                 P  -111.017    0.322    -7.574    0.160                                                     
-24 224 60364.00 P  0.032379 0.006079  0.271195 0.007688  P 0.0068613 0.0059070                 P  -110.941    0.322    -7.296    0.160                                                     
-24 225 60365.00 P  0.031271 0.006138  0.273184 0.007784  P 0.0067057 0.0059917                 P  -110.827    0.322    -6.982    0.160                                                     
-24 226 60366.00 P  0.030199 0.006197  0.275190 0.007878  P 0.0064118 0.0060760                 P  -110.657    0.322    -6.828    0.160                                                     
-24 227 60367.00 P  0.029163 0.006256  0.277212 0.007973  P 0.0060327 0.0061599                 P  -110.500    0.322    -6.866    0.160                                                     
-24 228 60368.00 P  0.028164 0.006314  0.279249 0.008067  P 0.0056352 0.0062434                 P  -110.421    0.322    -6.989    0.160                                                     
-24 229 60369.00 P  0.027203 0.006372  0.281301 0.008160  P 0.0052906 0.0063266                 P  -110.454    0.322    -7.144    0.160                                                     
-24 3 1 60370.00 P  0.026278 0.006429  0.283367 0.008253  P 0.0050561 0.0064093                 P  -110.605    0.322    -7.405    0.160                                                     
-24 3 2 60371.00 P  0.025391 0.006486  0.285446 0.008346  P 0.0049737 0.0064917                 P  -110.789    0.322    -7.809    0.160                                                     
-24 3 3 60372.00 P  0.024541 0.006543  0.287538 0.008438  P 0.0050609 0.0065737                 P  -110.820    0.322    -8.195    0.160                                                     
-24 3 4 60373.00 P  0.023730 0.006600  0.289643 0.008530  P 0.0053022 0.0066554                 P  -110.653    0.322    -8.332    0.160                                                     
-24 3 5 60374.00 P  0.022956 0.006655  0.291759 0.008621  P 0.0056357 0.0067368                 P  -110.547    0.322    -8.234    0.160                                                     
-24 3 6 60375.00 P  0.022220 0.006711  0.293886 0.008712  P 0.0059545 0.0068177                 P  -110.751    0.322    -8.207    0.160                                                     
-24 3 7 60376.00 P  0.021522 0.006766  0.296023 0.008803  P 0.0061185 0.0068984                 P  -111.037    0.322    -8.444    0.160                                                     
-24 3 8 60377.00 P  0.020863 0.006821  0.298171 0.008894  P 0.0059905 0.0069788                                                                                                             
-24 3 9 60378.00 P  0.020242 0.006876  0.300327 0.008984  P 0.0054923 0.0070588                                                                                                             
-24 310 60379.00 P  0.019659 0.006930  0.302493 0.009073  P 0.0046437 0.0071385                                                                                                             
-24 311 60380.00 P  0.019115 0.006984  0.304666 0.009163  P 0.0035674 0.0072179                                                                                                             
-24 312 60381.00 P  0.018610 0.007038  0.306847 0.009252  P 0.0024522 0.0072970                                                                                                             
-24 313 60382.00 P  0.018144 0.007091  0.309035 0.009340  P 0.0014885 0.0073758                                                                                                             
-24 314 60383.00 P  0.017716 0.007144  0.311229 0.009429  P 0.0008091 0.0074544                                                                                                             
-24 315 60384.00 P  0.017328 0.007197  0.313428 0.009517  P 0.0004549 0.0075326                                                                                                             
-24 316 60385.00 P  0.016978 0.007249  0.315633 0.009604  P 0.0003851 0.0076106                                                                                                             
-24 317 60386.00 P  0.016668 0.007301  0.317842 0.009692  P 0.0005081 0.0076883                                                                                                             
-24 318 60387.00 P  0.016396 0.007353  0.320054 0.009779  P 0.0007158 0.0077657                                                                                                             
-24 319 60388.00 P  0.016163 0.007405  0.322270 0.009865  P 0.0009083 0.0078428                                                                                                             
-24 320 60389.00 P  0.015970 0.007456  0.324489 0.009952  P 0.0010053 0.0079197                                                                                                             
-24 321 60390.00 P  0.015815 0.007507  0.326709 0.010038  P 0.0009531 0.0079964                                                                                                             
-24 322 60391.00 P  0.015699 0.007558  0.328931 0.010124  P 0.0007218 0.0080728                                                                                                             
-24 323 60392.00 P  0.015622 0.007609  0.331153 0.010210  P 0.0003086 0.0081489                                                                                                             
-24 324 60393.00 P  0.015584 0.007659  0.333376 0.010295  P-0.0002626 0.0082248                                                                                                             
-24 325 60394.00 P  0.015585 0.007709  0.335598 0.010380  P-0.0009423 0.0083005                                                                                                             
-24 326 60395.00 P  0.015625 0.007759  0.337819 0.010465  P-0.0016634 0.0083759                                                                                                             
-24 327 60396.00 P  0.015703 0.007808  0.340038 0.010549  P-0.0023529 0.0084511                                                                                                             
-24 328 60397.00 P  0.015820 0.007858  0.342254 0.010634  P-0.0029441 0.0085261                                                                                                             
-24 329 60398.00 P  0.015975 0.007907  0.344468 0.010718  P-0.0033874 0.0086008                                                                                                             
-24 330 60399.00 P  0.016169 0.007956  0.346679 0.010801  P-0.0036580 0.0086754                                                                                                             
-24 331 60400.00 P  0.016401 0.008004  0.348885 0.010885  P-0.0037616 0.0087497                                                                                                             
-24 4 1 60401.00 P  0.016671 0.008053  0.351087 0.010968  P-0.0037435 0.0088237                                                                                                             
-24 4 2 60402.00 P  0.016979 0.008101  0.353283 0.011051  P-0.0036898 0.0088976                                                                                                             
-24 4 3 60403.00 P  0.017325 0.008149  0.355473 0.011134  P-0.0037207 0.0089713                                                                                                             
-24 4 4 60404.00 P  0.017708 0.008197  0.357657 0.011216  P-0.0039658 0.0090448                                                                                                             
-24 4 5 60405.00 P  0.018129 0.008244  0.359833 0.011299  P-0.0045277 0.0091180                                                                                                             
-24 4 6 60406.00 P  0.018588 0.008292  0.362002 0.011381  P-0.0054405 0.0091911                                                                                                             
-24 4 7 60407.00 P  0.019083 0.008339  0.364163 0.011463  P-0.0066426 0.0092639                                                                                                             
-24 4 8 60408.00 P  0.019615 0.008386  0.366314 0.011544  P-0.0079845 0.0093366                                                                                                             
-24 4 9 60409.00 P  0.020184 0.008433  0.368455 0.011626  P-0.0092730 0.0094091                                                                                                             
-24 410 60410.00 P  0.020789 0.008479  0.370587 0.011707  P-0.0103327 0.0094814                                                                                                             
-24 411 60411.00 P  0.021430 0.008526  0.372708 0.011788  P-0.0110625 0.0095535                                                                                                             
-24 412 60412.00 P  0.022108 0.008572  0.374818 0.011868  P-0.0114581 0.0096254                                                                                                             
-24 413 60413.00 P  0.022821 0.008618  0.376916 0.011949  P-0.0115936 0.0096971                                                                                                             
-24 414 60414.00 P  0.023569 0.008664  0.379002 0.012029  P-0.0115830 0.0097686                                                                                                             
-24 415 60415.00 P  0.024353 0.008709  0.381075 0.012109  P-0.0114830 0.0098400                                                                                                             
-24 416 60416.00 P  0.025172 0.008755  0.383135 0.012189  P-0.0114373 0.0099112                                                                                                             
-24 417 60417.00 P  0.026025 0.008800  0.385181 0.012269  P-0.0115077 0.0099822                                                                                                             
-24 418 60418.00 P  0.026913 0.008845  0.387212 0.012348  P-0.0117283 0.0100531                                                                                                             
-24 419 60419.00 P  0.027835 0.008890  0.389229 0.012428  P-0.0121063 0.0101238                                                                                                             
-24 420 60420.00 P  0.028790 0.008935  0.391230 0.012507  P-0.0126234 0.0101943                                                                                                             
-24 421 60421.00 P  0.029779 0.008979  0.393215 0.012586  P-0.0132384 0.0102646                                                                                                             
-24 422 60422.00 P  0.030801 0.009024  0.395184 0.012664  P-0.0138909 0.0103348                                                                                                             
-24 423 60423.00 P  0.031855 0.009068  0.397135 0.012743  P-0.0145102 0.0104048                                                                                                             
-24 424 60424.00 P  0.032942 0.009112  0.399070 0.012821  P-0.0150244 0.0104747                                                                                                             
-24 425 60425.00 P  0.034061 0.009156  0.400986 0.012899  P-0.0153751 0.0105444                                                                                                             
-24 426 60426.00 P  0.035211 0.009200  0.402883 0.012977  P-0.0155290 0.0106139                                                                                                             
-24 427 60427.00 P  0.036393 0.009243  0.404762 0.013055  P-0.0154872 0.0106833                                                                                                             
-24 428 60428.00 P  0.037606 0.009287  0.406621 0.013133  P-0.0152894 0.0107526                                                                                                             
-24 429 60429.00 P  0.038849 0.009330  0.408461 0.013210  P-0.0150144 0.0108216                                                                                                             
-24 430 60430.00 P  0.040122 0.009373  0.410279 0.013287  P-0.0147704 0.0108906                                                                                                             
-24 5 1 60431.00 P  0.041425 0.009416  0.412077 0.013364  P-0.0146760 0.0109594                                                                                                             
-24 5 2 60432.00 P  0.042757 0.009459  0.413854 0.013441  P-0.0148330 0.0110280                                                                                                             
-24 5 3 60433.00 P  0.044117 0.009502  0.415609 0.013518  P-0.0152947 0.0110965                                                                                                             
-24 5 4 60434.00 P  0.045506 0.009545  0.417342 0.013594  P-0.0160408 0.0111649                                                                                                             
-24 5 5 60435.00 P  0.046924 0.009587  0.419052 0.013671  P-0.0169692 0.0112331                                                                                                             
-24 5 6 60436.00 P  0.048368 0.009629  0.420739 0.013747  P-0.0179186 0.0113012                                                                                                             
-24 5 7 60437.00 P  0.049840 0.009671  0.422402 0.013823  P-0.0187142 0.0113691                                                                                                             
-24 5 8 60438.00 P  0.051338 0.009713  0.424042 0.013899  P-0.0192215 0.0114369                                                                                                             
-24 5 9 60439.00 P  0.052862 0.009755  0.425657 0.013975  P-0.0193873 0.0115046                                                                                                             
-24 510 60440.00 P  0.054412 0.009797  0.427248 0.014050  P-0.0192458 0.0115721                                                                                                             
-24 511 60441.00 P  0.055987 0.009839  0.428813 0.014126  P-0.0188944 0.0116395                                                                                                             
-24 512 60442.00 P  0.057587 0.009880  0.430353 0.014201  P-0.0184533 0.0117067                                                                                                             
-24 513 60443.00 P  0.059211 0.009922  0.431867 0.014276  P-0.0180303 0.0117739                                                                                                             
-24 514 60444.00 P  0.060858 0.009963  0.433355 0.014351  P-0.0177026 0.0118409                                                                                                             
-24 515 60445.00 P  0.062529 0.010004  0.434816 0.014426  P-0.0175128 0.0119077                                                                                                             
-24 516 60446.00 P  0.064222 0.010045  0.436251 0.014500  P-0.0174734 0.0119745                                                                                                             
-24 517 60447.00 P  0.065938 0.010086  0.437658 0.014575  P-0.0175712 0.0120411                                                                                                             
-24 518 60448.00 P  0.067675 0.010126  0.439037 0.014649  P-0.0177707 0.0121076                                                                                                             
-24 519 60449.00 P  0.069433 0.010167  0.440389 0.014724  P-0.0180184 0.0121740                                                                                                             
-24 520 60450.00 P  0.071212 0.010207  0.441712 0.014798  P-0.0182487 0.0122402                                                                                                             
-24 521 60451.00 P  0.073011 0.010248  0.443007 0.014871  P-0.0183923 0.0123063                                                                                                             
-24 522 60452.00 P  0.074829 0.010288  0.444273 0.014945  P-0.0183872 0.0123723                                                                                                             
-24 523 60453.00 P  0.076666 0.010328  0.445510 0.015019  P-0.0181902 0.0124382                                                                                                             
-24 524 60454.00 P  0.078522 0.010368  0.446717 0.015092  P-0.0177890 0.0125040                                                                                                             
-24 525 60455.00 P  0.080395 0.010408  0.447895 0.015166  P-0.0172129 0.0125696                                                                                                             
-24 526 60456.00 P  0.082286 0.010448  0.449043 0.015239  P-0.0165343 0.0126352                                                                                                             
-24 527 60457.00 P  0.084194 0.010487  0.450160 0.015312  P-0.0158580 0.0127006                                                                                                             
-24 528 60458.00 P  0.086117 0.010527  0.451248 0.015385  P-0.0153008 0.0127659                                                                                                             
-24 529 60459.00 P  0.088056 0.010566  0.452304 0.015458  P-0.0149609 0.0128311                                                                                                             
-24 530 60460.00 P  0.090011 0.010606  0.453329 0.015530  P-0.0148919 0.0128962                                                                                                             
-24 531 60461.00 P  0.091979 0.010645  0.454324 0.015603  P-0.0150845 0.0129612                                                                                                             
-24 6 1 60462.00 P  0.093962 0.010684  0.455287 0.015675  P-0.0154621 0.0130260                                                                                                             
-24 6 2 60463.00 P  0.095958 0.010723  0.456218 0.015748  P-0.0158954 0.0130908                                                                                                             
-24 6 3 60464.00 P  0.097966 0.010762  0.457118 0.015820  P-0.0162314 0.0131554                                                                                                             
-24 6 4 60465.00 P  0.099987 0.010801  0.457986 0.015892  P-0.0163354 0.0132199                                                                                                             
-24 6 5 60466.00 P  0.102019 0.010839  0.458821 0.015964  P-0.0161294 0.0132844                                                                                                             
-24 6 6 60467.00 P  0.104062 0.010878  0.459625 0.016036  P-0.0156114 0.0133487                                                                                                             
-24 6 7 60468.00 P  0.106115 0.010916  0.460396 0.016107  P-0.0148490 0.0134129                                                                                                             
-24 6 8 60469.00 P  0.108178 0.010955  0.461134 0.016179  P-0.0139520 0.0134770                                                                                                             
-24 6 9 60470.00 P  0.110250 0.010993  0.461840 0.016250  P-0.0130354 0.0135410                                                                                                             
-24 610 60471.00 P  0.112331 0.011031  0.462513 0.016321  P-0.0121911 0.0136050                                                                                                             
-24 611 60472.00 P  0.114420 0.011069  0.463153 0.016393  P-0.0114758 0.0136688                                                                                                             
-24 612 60473.00 P  0.116516 0.011107  0.463760 0.016464  P-0.0109098 0.0137325                                                                                                             
-24 613 60474.00 P  0.118619 0.011145  0.464334 0.016535  P-0.0104830 0.0137961                                                                                                             
-24 614 60475.00 P  0.120728 0.011183  0.464874 0.016605  P-0.0101624 0.0138596                                                                                                             
-24 615 60476.00 P  0.122842 0.011220  0.465382 0.016676  P-0.0098976 0.0139230                                                                                                             
-24 616 60477.00 P  0.124961 0.011258  0.465856 0.016747  P-0.0096268 0.0139863                                                                                                             
-24 617 60478.00 P  0.127085 0.011295  0.466296 0.016817  P-0.0092849 0.0140495                                                                                                             
-24 618 60479.00 P  0.129212 0.011333  0.466703 0.016887  P-0.0088100 0.0141127                                                                                                             
-24 619 60480.00 P  0.131343 0.011370  0.467077 0.016958  P-0.0081539 0.0141757                                                                                                             
-24 620 60481.00 P  0.133476 0.011407  0.467417 0.017028  P-0.0072933 0.0142386                                                                                                             
-24 621 60482.00 P  0.135611 0.011444  0.467723 0.017098  P-0.0062422 0.0143014                                                                                                             
-24 622 60483.00 P  0.137747 0.011481  0.467996 0.017168  P-0.0050592 0.0143642                                                                                                             
-24 623 60484.00 P  0.139884 0.011518  0.468236 0.017237  P-0.0038447 0.0144268                                                                                                             
-24 624 60485.00 P  0.142021 0.011555  0.468442 0.017307  P-0.0027198 0.0144894                                                                                                             
-24 625 60486.00 P  0.144157 0.011592  0.468614 0.017377  P-0.0017935 0.0145519                                                                                                             
-24 626 60487.00 P  0.146293 0.011629  0.468753 0.017446  P-0.0011282 0.0146142                                                                                                             
-24 627 60488.00 P  0.148426 0.011665  0.468858 0.017515  P-0.0007171 0.0146765                                                                                                             
-24 628 60489.00 P  0.150558 0.011702  0.468930 0.017585  P-0.0004842 0.0147387                                                                                                             
-24 629 60490.00 P  0.152686 0.011738  0.468968 0.017654  P-0.0003038 0.0148008                                                                                                             
-24 630 60491.00 P  0.154811 0.011774  0.468973 0.017723  P-0.0000338 0.0148629                                                                                                             
-24 7 1 60492.00 P  0.156932 0.011811  0.468945 0.017792  P 0.0004484 0.0149248                                                                                                             
-24 7 2 60493.00 P  0.159048 0.011847  0.468884 0.017861  P 0.0012157 0.0149867                                                                                                             
-24 7 3 60494.00 P  0.161159 0.011883  0.468790 0.017929  P 0.0022743 0.0150484                                                                                                             
-24 7 4 60495.00 P  0.163265 0.011919  0.468663 0.017998  P 0.0035644 0.0151101                                                                                                             
-24 7 5 60496.00 P  0.165363 0.011955  0.468503 0.018066  P 0.0049784 0.0151717                                                                                                             
-24 7 6 60497.00 P  0.167455 0.011991  0.468310 0.018135  P 0.0063910 0.0152332                                                                                                             
-24 7 7 60498.00 P  0.169539 0.012026  0.468085 0.018203  P 0.0076908 0.0152946                                                                                                             
-24 7 8 60499.00 P  0.171615 0.012062  0.467827 0.018271  P 0.0088040 0.0153560                                                                                                             
-24 7 9 60500.00 P  0.173683 0.012097  0.467537 0.018339  P 0.0097018 0.0154172                                                                                                             
-24 710 60501.00 P  0.175741 0.012133  0.467215 0.018407  P 0.0103971 0.0154784                                                                                                             
-24 711 60502.00 P  0.177789 0.012168  0.466861 0.018475  P 0.0109340 0.0155395                                                                                                             
-24 712 60503.00 P  0.179827 0.012204  0.466475 0.018543  P 0.0113768 0.0156005                                                                                                             
-24 713 60504.00 P  0.181854 0.012239  0.466057 0.018611  P 0.0117987 0.0156614                                                                                                             
-24 714 60505.00 P  0.183870 0.012274  0.465608 0.018679  P 0.0122709 0.0157223                                                                                                             
-24 715 60506.00 P  0.185873 0.012309  0.465128 0.018746  P 0.0128528 0.0157831                                                                                                             
-24 716 60507.00 P  0.187864 0.012344  0.464617 0.018814  P 0.0135853 0.0158438                                                                                                             
-24 717 60508.00 P  0.189842 0.012379  0.464075 0.018881  P 0.0144863 0.0159044                                                                                                             
-24 718 60509.00 P  0.191806 0.012414  0.463503 0.018948  P 0.0155456 0.0159649                                                                                                             
-24 719 60510.00 P  0.193756 0.012449  0.462900 0.019015  P 0.0167178 0.0160254                                                                                                             
-24 720 60511.00 P  0.195691 0.012484  0.462267 0.019082  P 0.0179182 0.0160858                                                                                                             
-24 721 60512.00 P  0.197611 0.012519  0.461604 0.019149  P 0.0190291 0.0161461                                                                                                             
-24 722 60513.00 P  0.199516 0.012553  0.460912 0.019216  P 0.0199248 0.0162063                                                                                                             
-24 723 60514.00 P  0.201404 0.012588  0.460191 0.019283  P 0.0205120 0.0162665                                                                                                             
-24 724 60515.00 P  0.203276 0.012622  0.459440 0.019350  P 0.0207710 0.0163265                                                                                                             
-24 725 60516.00 P  0.205130 0.012656  0.458661 0.019416  P 0.0207745 0.0163866                                                                                                             
-24 726 60517.00 P  0.206967 0.012691  0.457853 0.019483  P 0.0206713 0.0164465                                                                                                             
-24 727 60518.00 P  0.208785 0.012725  0.457017 0.019549  P 0.0206367 0.0165063                                                                                                             
-24 728 60519.00 P  0.210585 0.012759  0.456153 0.019616  P 0.0208156 0.0165661                                                                                                             
-24 729 60520.00 P  0.212366 0.012793  0.455262 0.019682  P 0.0212843 0.0166258                                                                                                             
-24 730 60521.00 P  0.214127 0.012827  0.454344 0.019748  P 0.0220444 0.0166855                                                                                                             
-24 731 60522.00 P  0.215868 0.012861  0.453398 0.019814  P 0.0230334 0.0167451                                                                                                             
-24 8 1 60523.00 P  0.217589 0.012895  0.452426 0.019880  P 0.0241475 0.0168046                                                                                                             
-24 8 2 60524.00 P  0.219289 0.012929  0.451428 0.019946  P 0.0252809 0.0168640                                                                                                             
-24 8 3 60525.00 P  0.220968 0.012963  0.450404 0.020012  P 0.0263466 0.0169233                                                                                                             
-24 8 4 60526.00 P  0.222624 0.012997  0.449355 0.020078  P 0.0272712 0.0169826                                                                                                             
-24 8 5 60527.00 P  0.224259 0.013030  0.448280 0.020143  P 0.0280065 0.0170419                                                                                                             
-24 8 6 60528.00 P  0.225871 0.013064  0.447181 0.020209  P 0.0285702 0.0171010                                                                                                             
-24 8 7 60529.00 P  0.227460 0.013097  0.446057 0.020274  P 0.0290206 0.0171601                                                                                                             
-24 8 8 60530.00 P  0.229025 0.013131  0.444910 0.020340  P 0.0293346 0.0172191                                                                                                             
-24 8 9 60531.00 P  0.230567 0.013164  0.443738 0.020405  P 0.0296098 0.0172780                                                                                                             
-24 810 60532.00 P  0.232085 0.013197  0.442544 0.020470  P 0.0299144 0.0173369                                                                                                             
-24 811 60533.00 P  0.233578 0.013231  0.441326 0.020536  P 0.0303424 0.0173957                                                                                                             
-24 812 60534.00 P  0.235046 0.013264  0.440086 0.020601  P 0.0308515 0.0174545                                                                                                             
-24 813 60535.00 P  0.236489 0.013297  0.438825 0.020666  P 0.0315318 0.0175131                                                                                                             
-24 814 60536.00 P  0.237906 0.013330  0.437541 0.020731  P 0.0323526 0.0175718                                                                                                             
-24 815 60537.00 P  0.239298 0.013363  0.436237 0.020796  P 0.0332826 0.0176303                                                                                                             
-24 816 60538.00 P  0.240663 0.013396  0.434911 0.020860  P 0.0343115 0.0176888                                                                                                             
-24 817 60539.00 P  0.242001 0.013429  0.433566 0.020925  P 0.0352635 0.0177472                                                                                                             
-24 818 60540.00 P  0.243312 0.013462  0.432200 0.020990  P 0.0359728 0.0178055                                                                                                             
-24 819 60541.00 P  0.244596 0.013495  0.430815 0.021054  P 0.0363117 0.0178638                                                                                                             
-24 820 60542.00 P  0.245853 0.013527  0.429411 0.021119  P 0.0362615 0.0179220                                                                                                             
-24 821 60543.00 P  0.247082 0.013560  0.427989 0.021183  P 0.0358726 0.0179802                                                                                                             
-24 822 60544.00 P  0.248282 0.013592  0.426548 0.021247  P 0.0351969 0.0180383                                                                                                             
-24 823 60545.00 P  0.249455 0.013625  0.425090 0.021312  P 0.0345240 0.0180963                                                                                                             
-24 824 60546.00 P  0.250598 0.013657  0.423615 0.021376  P 0.0339254 0.0181543                                                                                                             
-24 825 60547.00 P  0.251713 0.013690  0.422123 0.021440  P 0.0335690 0.0182122                                                                                                             
-24 826 60548.00 P  0.252798 0.013722  0.420614 0.021504  P 0.0334563 0.0182700                                                                                                             
-24 827 60549.00 P  0.253854 0.013754  0.419090 0.021568  P 0.0335632 0.0183278                                                                                                             
-24 828 60550.00 P  0.254881 0.013787  0.417551 0.021632  P 0.0338474 0.0183855                                                                                                             
-24 829 60551.00 P  0.255877 0.013819  0.415997 0.021695  P 0.0342777 0.0184432                                                                                                             
-24 830 60552.00 P  0.256843 0.013851  0.414429 0.021759  P 0.0347214 0.0185008                                                                                                             
-24 831 60553.00 P  0.257780 0.013883  0.412847 0.021823  P 0.0350294 0.0185583                                                                                                             
-24 9 1 60554.00 P  0.258685 0.013915  0.411251 0.021886  P 0.0352336 0.0186158                                                                                                             
-24 9 2 60555.00 P  0.259560 0.013947  0.409643 0.021950  P 0.0353490 0.0186732                                                                                                             
-24 9 3 60556.00 P  0.260404 0.013979  0.408023 0.022013  P 0.0352851 0.0187306                                                                                                             
-24 9 4 60557.00 P  0.261218 0.014011  0.406390 0.022077  P 0.0352201 0.0187879                                                                                                             
-24 9 5 60558.00 P  0.262000 0.014043  0.404747 0.022140  P 0.0350295 0.0188451                                                                                                             
-24 9 6 60559.00 P  0.262750 0.014074  0.403092 0.022203  P 0.0349876 0.0189023                                                                                                             
-24 9 7 60560.00 P  0.263470 0.014106  0.401428 0.022266  P 0.0350218 0.0189594                                                                                                             
-24 9 8 60561.00 P  0.264157 0.014138  0.399753 0.022329  P 0.0352267 0.0190165                                                                                                             
-24 9 9 60562.00 P  0.264813 0.014169  0.398069 0.022392  P 0.0356412 0.0190735                                                                                                             
-24 910 60563.00 P  0.265438 0.014201  0.396377 0.022455  P 0.0361274 0.0191305                                                                                                             
-24 911 60564.00 P  0.266030 0.014232  0.394676 0.022518  P 0.0367291 0.0191874                                                                                                             
-24 912 60565.00 P  0.266591 0.014264  0.392968 0.022581  P 0.0374522 0.0192442                                                                                                             
-24 913 60566.00 P  0.267119 0.014295  0.391252 0.022644  P 0.0381969 0.0193010                                                                                                             
-24 914 60567.00 P  0.267615 0.014326  0.389529 0.022707  P 0.0388628 0.0193577                                                                                                             
-24 915 60568.00 P  0.268079 0.014358  0.387801 0.022769  P 0.0392608 0.0194144                                                                                                             
-24 916 60569.00 P  0.268511 0.014389  0.386067 0.022832  P 0.0393235 0.0194710                                                                                                             
-24 917 60570.00 P  0.268911 0.014420  0.384327 0.022894  P 0.0390454 0.0195276                                                                                                             
-24 918 60571.00 P  0.269278 0.014451  0.382583 0.022957  P 0.0385175 0.0195841                                                                                                             
-24 919 60572.00 P  0.269613 0.014482  0.380835 0.023019  P 0.0378572 0.0196405                                                                                                             
-24 920 60573.00 P  0.269915 0.014513  0.379083 0.023081  P 0.0373449 0.0196969                                                                                                             
-24 921 60574.00 P  0.270186 0.014544  0.377329 0.023143  P 0.0370525 0.0197532                                                                                                             
-24 922 60575.00 P  0.270423 0.014575  0.375571 0.023206  P 0.0371226 0.0198095                                                                                                             
-24 923 60576.00 P  0.270629 0.014606  0.373812 0.023268  P 0.0374371 0.0198658                                                                                                             
-24 924 60577.00 P  0.270802 0.014637  0.372051 0.023330  P 0.0379364 0.0199219                                                                                                             
-24 925 60578.00 P  0.270943 0.014667  0.370289 0.023392  P 0.0384709 0.0199781                                                                                                             
-24 926 60579.00 P  0.271052 0.014698  0.368527 0.023453  P 0.0390857 0.0200341                                                                                                             
-24 927 60580.00 P  0.271129 0.014729  0.366765 0.023515  P 0.0395780 0.0200902                                                                                                             
-24 928 60581.00 P  0.271173 0.014759  0.365003 0.023577  P 0.0399290 0.0201461                                                                                                             
-24 929 60582.00 P  0.271186 0.014790  0.363243 0.023639  P 0.0400517 0.0202021                                                                                                             
-24 930 60583.00 P  0.271167 0.014820  0.361484 0.023700  P 0.0399670 0.0202579                                                                                                             
-2410 1 60584.00 P  0.271115 0.014851  0.359727 0.023762  P 0.0396790 0.0203137                                                                                                             
-2410 2 60585.00 P  0.271032 0.014881  0.357973 0.023823  P 0.0393000 0.0203695                                                                                                             
-2410 3 60586.00 P  0.270918 0.014912  0.356221 0.023885  P 0.0389718 0.0204252                                                                                                             
-2410 4 60587.00 P  0.270772 0.014942  0.354474 0.023946  P 0.0387645 0.0204809                                                                                                             
-2410 5 60588.00 P  0.270594 0.014972  0.352731 0.024008  P 0.0387272 0.0205365                                                                                                             
-2410 6 60589.00 P  0.270386 0.015003  0.350992 0.024069  P 0.0388625 0.0205920                                                                                                             
-2410 7 60590.00 P  0.270146 0.015033  0.349258 0.024130  P 0.0391451 0.0206475                                                                                                             
-2410 8 60591.00 P  0.269875 0.015063  0.347530 0.024191  P 0.0395964 0.0207030                                                                                                             
-2410 9 60592.00 P  0.269573 0.015093  0.345809 0.024252  P 0.0401276 0.0207584                                                                                                             
-241010 60593.00 P  0.269241 0.015123  0.344093 0.024313  P 0.0407064 0.0208138                                                                                                             
-241011 60594.00 P  0.268879 0.015153  0.342385 0.024374  P 0.0412022 0.0208691                                                                                                             
-241012 60595.00 P  0.268486 0.015183  0.340685 0.024435  P 0.0415381 0.0209243                                                                                                             
-241013 60596.00 P  0.268063 0.015213  0.338992 0.024496  P 0.0416013 0.0209795                                                                                                             
-241014 60597.00 P  0.267610 0.015243  0.337309 0.024557  P 0.0413772 0.0210347                                                                                                             
-241015 60598.00 P  0.267128 0.015273  0.335634 0.024618  P 0.0407936 0.0210898                                                                                                             
-241016 60599.00 P  0.266616 0.015303  0.333968 0.024678  P 0.0400333 0.0211449                                                                                                             
-241017 60600.00 P  0.266076 0.015332  0.332313 0.024739  P 0.0392129 0.0211999                                                                                                             
-241018 60601.00 P  0.265506 0.015362  0.330668 0.024799  P 0.0384832 0.0212548                                                                                                             
-241019 60602.00 P  0.264907 0.015392  0.329034 0.024860  P 0.0380655 0.0213098                                                                                                             
-241020 60603.00 P  0.264281 0.015421  0.327411 0.024920  P 0.0380376 0.0213646                                                                                                             
-241021 60604.00 P  0.263626 0.015451  0.325800 0.024981  P 0.0382693 0.0214195                                                                                                             
-241022 60605.00 P  0.262943 0.015480  0.324202 0.025041  P 0.0386708 0.0214742                                                                                                             
-241023 60606.00 P  0.262233 0.015510  0.322615 0.025101  P 0.0390329 0.0215290                                                                                                             
-241024 60607.00 P  0.261495 0.015539  0.321043 0.025162  P 0.0393147 0.0215837                                                                                                             
-241025 60608.00 P  0.260730 0.015569  0.319483 0.025222  P 0.0394575 0.0216383                                                                                                             
-241026 60609.00 P  0.259939 0.015598  0.317938 0.025282  P 0.0393967 0.0216929                                                                                                             
-241027 60610.00 P  0.259121 0.015627  0.316407 0.025342  P 0.0391438 0.0217474                                                                                                             
-241028 60611.00 P  0.258277 0.015657  0.314890 0.025402  P 0.0385889 0.0218019                                                                                                             
-241029 60612.00 P  0.257408 0.015686  0.313389 0.025462  P 0.0380298 0.0218564                                                                                                             
-241030 60613.00 P  0.256513 0.015715  0.311904 0.025522  P 0.0374333 0.0219108                                                                                                             
-241031 60614.00 P  0.255593 0.015744  0.310435 0.025582  P 0.0368659 0.0219652                                                                                                             
-2411 1 60615.00 P  0.254648 0.015773  0.308982 0.025641  P 0.0364138 0.0220195                                                                                                             
-2411 2 60616.00 P  0.253679 0.015802  0.307545 0.025701  P 0.0360853 0.0220738                                                                                                             
-2411 3 60617.00 P  0.252686 0.015831  0.306127 0.025761  P 0.0359500 0.0221280                                                                                                             
-2411 4 60618.00 P  0.251669 0.015860  0.304725 0.025820  P 0.0359903 0.0221822                                                                                                             
-2411 5 60619.00 P  0.250629 0.015889  0.303342 0.025880  P 0.0361773 0.0222363                                                                                                             
-2411 6 60620.00 P  0.249567 0.015918  0.301976 0.025939  P 0.0364305 0.0222904                                                                                                             
-2411 7 60621.00 P  0.248481 0.015947  0.300630 0.025999  P 0.0367380 0.0223444                                                                                                             
-2411 8 60622.00 P  0.247374 0.015976  0.299302 0.026058  P 0.0369218 0.0223985                                                                                                             
-2411 9 60623.00 P  0.246244 0.016005  0.297994 0.026118  P 0.0368870 0.0224524                                                                                                             
-241110 60624.00 P  0.245094 0.016034  0.296706 0.026177  P 0.0364448 0.0225063                                                                                                             
-241111 60625.00 P  0.243923 0.016062  0.295437 0.026236  P 0.0358103 0.0225602                                                                                                             
-241112 60626.00 P  0.242731 0.016091  0.294189 0.026295  P 0.0349851 0.0226140                                                                                                             
-241113 60627.00 P  0.241519 0.016120  0.292962 0.026354  P 0.0340177 0.0226678                                                                                                             
-241114 60628.00 P  0.240287 0.016148  0.291755 0.026413  P 0.0330429 0.0227216                                                                                                             
-241115 60629.00 P  0.239036 0.016177  0.290570 0.026473  P 0.0323154 0.0227753                                                                                                             
-241116 60630.00 P  0.237767 0.016205  0.289407 0.026532  P 0.0319982 0.0228290                                                                                                             
-241117 60631.00 P  0.236479 0.016234  0.288265 0.026590  P 0.0320998 0.0228826                                                                                                             
-241118 60632.00 P  0.235173 0.016262  0.287145 0.026649  P 0.0323631 0.0229362                                                                                                             
-241119 60633.00 P  0.233849 0.016291  0.286048 0.026708  P 0.0327560 0.0229897                                                                                                             
-241120 60634.00 P  0.232509 0.016319  0.284974 0.026767  P 0.0331466 0.0230432                                                                                                             
-241121 60635.00 P  0.231152 0.016347  0.283922 0.026826  P 0.0334092 0.0230966                                                                                                             
-241122 60636.00 P  0.229779 0.016376  0.282894 0.026884  P 0.0335791 0.0231500                                                                                                             
-241123 60637.00 P  0.228391 0.016404  0.281889 0.026943  P 0.0335416 0.0232034                                                                                                             
-241124 60638.00 P  0.226987 0.016432  0.280908 0.027002  P 0.0333379 0.0232567                                                                                                             
-241125 60639.00 P  0.225569 0.016460  0.279951 0.027060  P 0.0330361 0.0233100                                                                                                             
-241126 60640.00 P  0.224136 0.016489  0.279018 0.027119  P 0.0327222 0.0233633                                                                                                             
-241127 60641.00 P  0.222690 0.016517  0.278109 0.027177  P 0.0323859 0.0234165                                                                                                             
-241128 60642.00 P  0.221230 0.016545  0.277225 0.027235  P 0.0321964 0.0234697                                                                                                             
-241129 60643.00 P  0.219758 0.016573  0.276366 0.027294  P 0.0321724 0.0235228                                                                                                             
-241130 60644.00 P  0.218274 0.016601  0.275532 0.027352  P 0.0324093 0.0235759                                                                                                             
-2412 1 60645.00 P  0.216777 0.016629  0.274723 0.027410  P 0.0328833 0.0236289                                                                                                             
-2412 2 60646.00 P  0.215270 0.016657  0.273939 0.027468  P 0.0334867 0.0236819                                                                                                             
-2412 3 60647.00 P  0.213751 0.016685  0.273180 0.027527  P 0.0341309 0.0237349                                                                                                             
-2412 4 60648.00 P  0.212223 0.016713  0.272448 0.027585  P 0.0347378 0.0237878                                                                                                             
-2412 5 60649.00 P  0.210684 0.016740  0.271741 0.027643  P 0.0352362 0.0238407                                                                                                             
-2412 6 60650.00 P  0.209136 0.016768  0.271060 0.027701  P 0.0356428 0.0238935                                                                                                             
-2412 7 60651.00 P  0.207580 0.016796  0.270405 0.027759  P 0.0358122 0.0239463                                                                                                             
-2412 8 60652.00 P  0.206015 0.016824  0.269776 0.027817  P 0.0356762 0.0239991                                                                                                             
-2412 9 60653.00 P  0.204442 0.016851  0.269174 0.027874  P 0.0353098 0.0240518                                                                                                             
-241210 60654.00 P  0.202863 0.016879  0.268598 0.027932  P 0.0348071 0.0241045                                                                                                             
-241211 60655.00 P  0.201276 0.016907  0.268049 0.027990  P 0.0343388 0.0241572                                                                                                             
-241212 60656.00 P  0.199683 0.016934  0.267526 0.028048  P 0.0341443 0.0242098                                                                                                             
-241213 60657.00 P  0.198085 0.016962  0.267030 0.028105  P 0.0342267 0.0242624                                                                                                             
-241214 60658.00 P  0.196481 0.016989  0.266561 0.028163  P 0.0346803 0.0243149                                                                                                             
-241215 60659.00 P  0.194872 0.017017  0.266119 0.028221  P 0.0353212 0.0243674                                                                                                             
-241216 60660.00 P  0.193260 0.017044  0.265703 0.028278  P 0.0360731 0.0244199                                                                                                             
-241217 60661.00 P  0.191643 0.017072  0.265315 0.028336  P 0.0369084 0.0244723                                                                                                             
-241218 60662.00 P  0.190024 0.017099  0.264954 0.028393  P 0.0376304 0.0245247                                                                                                             
-241219 60663.00 P  0.188402 0.017127  0.264619 0.028451  P 0.0381392 0.0245770                                                                                                             
-241220 60664.00 P  0.186777 0.017154  0.264312 0.028508  P 0.0383757 0.0246293                                                                                                             
-241221 60665.00 P  0.185151 0.017181  0.264032 0.028565  P 0.0382966 0.0246816                                                                                                             
-241222 60666.00 P  0.183524 0.017208  0.263779 0.028622  P 0.0382473 0.0247338                                                                                                             
-241223 60667.00 P  0.181897 0.017236  0.263553 0.028680  P 0.0381505 0.0247860                                                                                                             
-241224 60668.00 P  0.180269 0.017263  0.263354 0.028737  P 0.0380417 0.0248382                                                                                                             
-241225 60669.00 P  0.178642 0.017290  0.263183 0.028794  P 0.0380150 0.0248903                                                                                                             
-241226 60670.00 P  0.177016 0.017317  0.263038 0.028851  P 0.0381722 0.0249424                                                                                                             
-241227 60671.00 P  0.175391 0.017344  0.262921 0.028908  P 0.0384390 0.0249945                                                                                                             
-241228 60672.00 P  0.173768 0.017371  0.262830 0.028965  P 0.0388291 0.0250465                                                                                                             
-241229 60673.00 P  0.172147 0.017398  0.262766 0.029022  P 0.0392223 0.0250985                                                                                                             
-241230 60674.00 P  0.170530 0.017425  0.262730 0.029079  P 0.0396904 0.0251504                                                                                                             
-241231 60675.00 P  0.168916 0.017452  0.262720 0.029136  P 0.0401578 0.0252023                                                                                                             
-25 1 1 60676.00 P  0.167305 0.017479  0.262737 0.029193  P 0.0405763 0.0252542                                                                                                             
-25 1 2 60677.00 P  0.165700 0.017506  0.262781 0.029250  P 0.0408286 0.0253060                                                                                                             
-25 1 3 60678.00 P  0.164099 0.017533  0.262851 0.029306  P 0.0408307 0.0253578                                                                                                             
-25 1 4 60679.00 P  0.162504 0.017560  0.262947 0.029363  P 0.0405490 0.0254096                                                                                                             
-25 1 5 60680.00                                                                                                                                                                            
-25 1 6 60681.00                                                                                                                                                                            
-25 1 7 60682.00                                                                                                                                                                            
-25 1 8 60683.00                                                                                                                                                                            
-25 1 9 60684.00                                                                                                                                                                            
-25 110 60685.00                                                                                                                                                                            
-25 111 60686.00                                                                                                                                                                            
-25 112 60687.00                                                                                                                                                                            
-25 113 60688.00                                                                                                                                                                            
-25 114 60689.00                                                                                                                                                                            
-25 115 60690.00                                                                                                                                                                            
-25 116 60691.00                                                                                                                                                                            
-25 117 60692.00                                                                                                                                                                            
-25 118 60693.00                                                                                                                                                                            
-25 119 60694.00                                                                                                                                                                            
-25 120 60695.00                                                                                                                                                                            
-25 121 60696.00                                                                                                                                                                            
-25 122 60697.00                                                                                                                                                                            
-25 123 60698.00                                                                                                                                                                            
-25 124 60699.00                                                                                                                                                                            
-25 125 60700.00                                                                                                                                                                            
-25 126 60701.00                                                                                                                                                                            
-25 127 60702.00                                                                                                                                                                            
-25 128 60703.00                                                                                                                                                                            
-25 129 60704.00                                                                                                                                                                            
-25 130 60705.00                                                                                                                                                                            
-25 131 60706.00                                                                                                                                                                            
-25 2 1 60707.00                                                                                                                                                                            
-25 2 2 60708.00                                                                                                                                                                            
-25 2 3 60709.00                                                                                                                                                                            
-25 2 4 60710.00                                                                                                                                                                            
-25 2 5 60711.00                                                                                                                                                                            
-25 2 6 60712.00                                                                                                                                                                            
-25 2 7 60713.00                                                                                                                                                                            
-25 2 8 60714.00                                                                                                                                                                            
-25 2 9 60715.00                                                                                                                                                                            
-25 210 60716.00                                                                                                                                                                            
-25 211 60717.00                                                                                                                                                                            
-25 212 60718.00                                                                                                                                                                            
-25 213 60719.00                                                                                                                                                                            
-25 214 60720.00                                                                                                                                                                            
-25 215 60721.00                                                                                                                                                                            
-25 216 60722.00                                                                                                                                                                            
-25 217 60723.00                                                                                                                                                                            
-25 218 60724.00                                                                                                                                                                            
-25 219 60725.00                                                                                                                                                                            
-25 220 60726.00                                                                                                                                                                            
-25 221 60727.00                                                                                                                                                                            
-25 222 60728.00                                                                                                                                                                            
-25 223 60729.00                                                                                                                                                                            
+221222 59935.00 I  0.094819 0.000029  0.194003 0.000026  I-0.0180991 0.0000048 -0.0786 0.0034  I  -112.094    0.633    -5.329    0.073  0.094877  0.193950 -0.0181060  -112.105    -5.394  
+221223 59936.00 I  0.093422 0.000029  0.194945 0.000027  I-0.0179138 0.0000048 -0.2757 0.0031  I  -112.181    0.322    -5.886    0.160  0.093472  0.194922 -0.0178955  -112.150    -5.759  
+221224 59937.00 I  0.091312 0.000015  0.196096 0.000022  I-0.0176092 0.0000040 -0.2882 0.0032  I  -111.866    0.322    -6.083    0.160  0.091397  0.196126 -0.0175841  -111.706    -6.007  
+221225 59938.00 I  0.088380 0.000015  0.197001 0.000021  I-0.0173692 0.0000041 -0.2052 0.0034  I  -111.332    0.322    -5.977    0.160  0.088402  0.197099 -0.0173115  -111.094    -5.943  
+221226 59939.00 I  0.085224 0.000038  0.197366 0.000018  I-0.0172531 0.0000056  0.0407 0.0033  I  -110.989    0.610    -5.744    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
+221227 59940.00 I  0.082026 0.000038  0.197766 0.000018  I-0.0174768 0.0000052  0.3651 0.0037  I  -110.918    0.610    -5.635    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
+221228 59941.00 I  0.078215 0.000039  0.198405 0.000023  I-0.0179214 0.0000047  0.5037 0.0035  I  -110.944    0.673    -5.626    0.150  0.078253  0.198379 -0.0179243  -110.647    -5.673  
+221229 59942.00 I  0.074759 0.000039  0.198575 0.000023  I-0.0184549 0.0000048  0.5544 0.0033  I  -110.979    0.673    -5.525    0.150  0.074744  0.198584 -0.0184719  -110.694    -5.570  
+221230 59943.00 I  0.071219 0.000039  0.199149 0.000022  I-0.0190022 0.0000046  0.5210 0.0034  I  -111.070    0.673    -5.303    0.150  0.071281  0.199199 -0.0190102  -110.793    -5.341  
+221231 59944.00 I  0.067043 0.000039  0.200110 0.000023  I-0.0194890 0.0000048  0.4640 0.0039  I  -111.238    0.673    -5.112    0.150  0.067074  0.200103 -0.0194855  -110.973    -5.182  
+23 1 1 59945.00 I  0.062781 0.000011  0.200905 0.000017  I-0.0198682 0.0000063  0.2210 0.0036  I  -111.422    0.721    -5.047    0.134  0.062699  0.200944 -0.0197967  -111.162    -5.163  
+23 1 2 59946.00 I  0.059066 0.000032  0.201758 0.000019  I-0.0199331 0.0000054 -0.0158 0.0047  I  -111.530    0.585    -5.051    0.098  0.059003  0.201796 -0.0199243  -111.443    -5.114  
+23 1 3 59947.00 I  0.055736 0.000039  0.202461 0.000015  I-0.0198530 0.0000070 -0.2034 0.0045  I  -111.614    0.620    -4.987    0.135  0.055638  0.202514 -0.0198250  -111.467    -5.128  
+23 1 4 59948.00 I  0.052991 0.000039  0.203017 0.000016  I-0.0195102 0.0000072 -0.4391 0.0054  I  -111.255    0.620    -5.114    0.135  0.052933  0.202990 -0.0195007  -111.313    -5.194  
+23 1 5 59949.00 I  0.050823 0.000039  0.203823 0.000016  I-0.0190344 0.0000081 -0.4959 0.0054  I  -110.809    0.620    -5.372    0.135  0.050795  0.203830 -0.0190232  -110.822    -5.531  
+23 1 6 59950.00 I  0.048802 0.000039  0.205099 0.000015  I-0.0185256 0.0000081 -0.5312 0.0057  I  -110.462    0.620    -5.678    0.135  0.048795  0.205101 -0.0184663  -110.510    -5.834  
+23 1 7 59951.00 I  0.046882 0.000039  0.206230 0.000014  I-0.0179842 0.0000080 -0.5300 0.0059  I  -110.282    0.620    -5.861    0.135  0.046853  0.206221 -0.0179143  -110.392    -5.984  
+23 1 8 59952.00 I  0.045147 0.000028  0.207580 0.000013  I-0.0174954 0.0000086 -0.4393 0.0057  I  -110.180    0.872    -5.845    0.172  0.045146  0.207590 -0.0174487  -110.316    -5.948  
+23 1 9 59953.00 I  0.043371 0.000014  0.209048 0.000010  I-0.0171331 0.0000082 -0.2661 0.0058  I  -110.034    0.885    -5.729    0.141  0.043370  0.209111 -0.0171274  -110.159    -5.821  
+23 110 59954.00 I  0.041306 0.000013  0.210264 0.000010  I-0.0169645 0.0000077 -0.0889 0.0052  I  -109.802    0.885    -5.647    0.141  0.041325  0.210288 -0.0169671  -109.874    -5.733  
+23 111 59955.00 I  0.038971 0.000045  0.211091 0.000021  I-0.0169516 0.0000063  0.0772 0.0047  I  -109.513    0.812    -5.601    0.121  0.038979  0.211134 -0.0169747  -109.583    -5.665  
+23 112 59956.00 I  0.036561 0.000045  0.211946 0.000021  I-0.0170839 0.0000054  0.1384 0.0043  I  -109.230    0.812    -5.496    0.121  0.036547  0.211915 -0.0170559  -109.296    -5.533  
+23 113 59957.00 I  0.034209 0.000045  0.213007 0.000021  I-0.0172129 0.0000059  0.1531 0.0051  I  -109.084    0.812    -5.334    0.121  0.034173  0.213022 -0.0172046  -109.147    -5.343  
+23 114 59958.00 I  0.031797 0.000044  0.214433 0.000020  I-0.0173915 0.0000087  0.1720 0.0049  I  -109.218    0.683    -5.263    0.087  0.031810  0.214393 -0.0173877  -109.253    -5.273  
+23 115 59959.00 I  0.029352 0.000047  0.216069 0.000021  I-0.0175491 0.0000078  0.1674 0.0058  I  -109.604    0.630    -5.375    0.089  0.029351  0.216047 -0.0175710  -109.621    -5.396  
+23 116 59960.00 I  0.026876 0.000048  0.217955 0.000021  I-0.0177137 0.0000078  0.1251 0.0064  I  -110.022    0.630    -5.531    0.089  0.026882  0.217923 -0.0177110  -110.037    -5.563  
+23 117 59961.00 I  0.024346 0.000021  0.220229 0.000008  I-0.0177502 0.0000101 -0.0644 0.0060  I  -110.366    0.598    -5.521    0.090  0.024343  0.220214 -0.0177400  -110.403    -5.564  
+23 118 59962.00 I  0.021693 0.000037  0.222435 0.000013  I-0.0175661 0.0000090 -0.3104 0.0067  I  -110.845    0.664    -5.405    0.115  0.021681  0.222504 -0.0175873  -110.857    -5.445  
+23 119 59963.00 I  0.019111 0.000037  0.224227 0.000013  I-0.0171811 0.0000088 -0.4012 0.0062  I  -111.500    0.664    -5.479    0.115  0.019078  0.224261 -0.0172362  -111.474    -5.516  
+23 120 59964.00 I  0.016694 0.000037  0.225584 0.000013  I-0.0167614 0.0000086 -0.4990 0.0071  I  -111.920    0.664    -5.850    0.115  0.016715  0.225678 -0.0167521  -111.849    -5.887  
+23 121 59965.00 I  0.013986 0.000033  0.226870 0.000012  I-0.0161801 0.0000111 -0.6060 0.0057  I  -111.682    0.850    -6.204    0.149  0.014033  0.226892 -0.0161896  -111.635    -6.235  
+23 122 59966.00 I  0.010882 0.000041  0.227735 0.000033  I-0.0156326 0.0000074 -0.4636 0.0066  I  -110.964    0.571    -6.209    0.104  0.010879  0.227740 -0.0156593  -110.964    -6.230  
+23 123 59967.00 I  0.007810 0.000041  0.228874 0.000033  I-0.0152837 0.0000073 -0.2287 0.0053  I  -110.343    0.571    -5.962    0.104  0.007728  0.228830 -0.0153087  -110.393    -5.970  
+23 124 59968.00 I  0.005419 0.000028  0.230151 0.000032  I-0.0152003 0.0000076  0.0817 0.0051  I  -110.162    0.406    -5.765    0.065  0.005300  0.230244 -0.0152158  -110.223    -5.787  
+23 125 59969.00 I  0.003918 0.000028  0.231469 0.000047  I-0.0154144 0.0000071  0.2940 0.0052  I  -110.161    0.582    -5.782    0.151  0.003852  0.231401 -0.0153642  -110.193    -5.799  
+23 126 59970.00 I  0.002905 0.000028  0.233341 0.000048  I-0.0157010 0.0000072  0.2443 0.0050  I  -110.293    0.582    -5.746    0.151  0.002927  0.233231 -0.0156349  -110.268    -5.775  
+23 127 59971.00 I  0.001585 0.000028  0.235760 0.000048  I-0.0158913 0.0000071  0.1595 0.0052  I  -110.520    0.582    -5.584    0.151  0.001593  0.235918 -0.0158886  -110.468    -5.635  
+23 128 59972.00 I  0.000374 0.000012  0.238166 0.000037  I-0.0159956 0.0000075  0.0013 0.0050  I  -110.750    0.710    -5.486    0.199  0.000279  0.238107 -0.0159862  -110.687    -5.537  
+23 129 59973.00 I -0.000258 0.000029  0.240364 0.000038  I-0.0158886 0.0000071 -0.1730 0.0051  I  -110.852    0.898    -5.610    0.192 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
+23 130 59974.00 I -0.000868 0.000030  0.242677 0.000038  I-0.0156599 0.0000069 -0.3164 0.0050  I  -110.805    0.898    -5.854    0.192 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
+23 131 59975.00 I -0.001367 0.000029  0.244951 0.000016  I-0.0152327 0.0000069 -0.5291 0.0041  I  -110.669    1.298    -6.028    0.181 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
+23 2 1 59976.00 I -0.002309 0.000029  0.247837 0.000035  I-0.0146257 0.0000045 -0.6700 0.0042  I  -110.460    1.129    -6.104    0.183 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
+23 2 2 59977.00 I -0.003560 0.000029  0.250320 0.000035  I-0.0139102 0.0000049 -0.7586 0.0033  I  -110.176    1.129    -6.200    0.183 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
+23 2 3 59978.00 I -0.004897 0.000029  0.252423 0.000035  I-0.0131284 0.0000049 -0.7875 0.0033  I  -109.914    1.129    -6.362    0.183 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
+23 2 4 59979.00 I -0.006465 0.000011  0.254309 0.000034  I-0.0123974 0.0000045 -0.6298 0.0031  I  -109.800    0.955    -6.474    0.185 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
+23 2 5 59980.00 I -0.008210 0.000016  0.255926 0.000034  I-0.0118811 0.0000039 -0.4354 0.0030  I  -109.815    0.740    -6.410    0.153 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
+23 2 6 59981.00 I -0.009952 0.000016  0.257728 0.000034  I-0.0115057 0.0000039 -0.3039 0.0031  I  -109.806    0.740    -6.211    0.153 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
+23 2 7 59982.00 I -0.011914 0.000016  0.259683 0.000009  I-0.0112791 0.0000047 -0.1550 0.0027  I  -109.751    0.552    -6.022    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
+23 2 8 59983.00 I -0.014081 0.000029  0.261627 0.000024  I-0.0111890 0.0000038 -0.0261 0.0030  I  -109.430    0.750    -5.953    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
+23 2 9 59984.00 I -0.015741 0.000029  0.263467 0.000024  I-0.0112366 0.0000038  0.1320 0.0027  I  -109.159    0.750    -5.940    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
+23 210 59985.00 I -0.016680 0.000028  0.265511 0.000024  I-0.0114572 0.0000039  0.3025 0.0030  I  -108.913    0.923    -5.888    0.043 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
+23 211 59986.00 I -0.017894 0.000025  0.268034 0.000023  I-0.0118011 0.0000047  0.3513 0.0028  I  -109.047    0.923    -5.947    0.043 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
+23 212 59987.00 I -0.019627 0.000028  0.270430 0.000041  I-0.0121337 0.0000040  0.3219 0.0032  I  -109.300    0.780    -6.124    0.122 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
+23 213 59988.00 I -0.021932 0.000028  0.273053 0.000042  I-0.0124063 0.0000042  0.1769 0.0030  I  -109.543    0.780    -6.353    0.122 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
+23 214 59989.00 I -0.024511 0.000014  0.275828 0.000036  I-0.0124630 0.0000046 -0.0415 0.0030  I  -109.722    0.685    -6.477    0.160 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
+23 215 59990.00 I -0.026950 0.000017  0.278113 0.000036  I-0.0123404 0.0000042 -0.2086 0.0031  I  -109.971    0.660    -6.478    0.147 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
+23 216 59991.00 I -0.029366 0.000017  0.280710 0.000036  I-0.0120575 0.0000043 -0.3406 0.0030  I  -110.396    0.660    -6.556    0.147 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
+23 217 59992.00 I -0.031752 0.000017  0.282876 0.000037  I-0.0116874 0.0000042 -0.3879 0.0036  I  -110.938    0.386    -6.841    0.092 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
+23 218 59993.00 I -0.033986 0.000012  0.284849 0.000013  I-0.0113574 0.0000058 -0.2081 0.0033  I  -110.809    0.386    -7.151    0.092 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
+23 219 59994.00 I -0.035821 0.000014  0.286840 0.000022  I-0.0113179 0.0000050  0.1116 0.0038  I  -110.223    0.693    -7.193    0.185 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
+23 220 59995.00 I -0.037231 0.000014  0.288972 0.000022  I-0.0115756 0.0000049  0.4161 0.0035  I  -109.571    0.693    -6.974    0.185 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
+23 221 59996.00 I -0.038258 0.000009  0.291443 0.000021  I-0.0121528 0.0000049  0.7286 0.0038  I  -109.179    0.736    -6.776    0.208 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
+23 222 59997.00 I -0.038767 0.000043  0.294621 0.000051  I-0.0129547 0.0000057  0.8069 0.0038  I  -109.074    0.712    -6.744    0.164 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
+23 223 59998.00 I -0.038968 0.000043  0.298280 0.000050  I-0.0137296 0.0000057  0.7742 0.0041  I  -109.189    0.712    -6.747    0.164 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
+23 224 59999.00 I -0.039125 0.000043  0.301745 0.000050  I-0.0145001 0.0000059  0.7324 0.0047  I  -109.491    0.712    -6.684    0.164 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
+23 225 60000.00 I -0.039677 0.000043  0.305150 0.000047  I-0.0151470 0.0000075  0.5482 0.0044  I  -109.853    0.644    -6.686    0.073 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
+23 226 60001.00 I -0.040919 0.000043  0.308147 0.000061  I-0.0155598 0.0000066  0.2539 0.0050  I  -110.075    0.735    -6.897    0.065 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
+23 227 60002.00 I -0.042719 0.000043  0.310770 0.000061  I-0.0156520 0.0000067 -0.0487 0.0046  I  -110.093    0.735    -7.225    0.065 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
+23 228 60003.00 I -0.044027 0.000007  0.313126 0.000039  I-0.0155073 0.0000064 -0.2165 0.0044  I  -109.884    0.906    -7.369    0.036 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
+23 3 1 60004.00 I -0.045082 0.000009  0.316381 0.000039  I-0.0152853 0.0000056 -0.1852 0.0043  I  -109.692    0.879    -7.414    0.104 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
+23 3 2 60005.00 I -0.046060 0.000008  0.318711 0.000039  I-0.0151155 0.0000057 -0.2180 0.0038  I  -109.346    0.879    -7.396    0.104 -0.046065  0.318766 -0.0150624  -109.433    -7.347  
+23 3 3 60006.00 I -0.046661 0.000008  0.321129 0.000039  I-0.0148525 0.0000052 -0.2411 0.0040  I  -108.915    0.879    -7.449    0.104 -0.046677  0.321138 -0.0148245  -108.998    -7.328  
+23 3 4 60007.00 I -0.046914 0.000006  0.323789 0.000007  I-0.0146877 0.0000056 -0.1010 0.0043  I  -108.593    0.791    -7.533    0.205 -0.046882  0.323792 -0.0146819  -108.638    -7.416  
+23 3 5 60008.00 I -0.046600 0.000012  0.326589 0.000008  I-0.0146756 0.0000069  0.1143 0.0044  I  -108.490    0.899    -7.504    0.098 -0.046540  0.326621 -0.0146823  -108.483    -7.439  
+23 3 6 60009.00 I -0.045640 0.000013  0.329769 0.000007  I-0.0149259 0.0000069  0.3582 0.0051  I  -108.508    0.899    -7.322    0.098 -0.045657  0.329817 -0.0149129  -108.456    -7.322  
+23 3 7 60010.00 I -0.044609 0.000012  0.333314 0.000006  I-0.0153731 0.0000076  0.5454 0.0048  I  -108.450    0.919    -7.142    0.052 -0.044599  0.333296 -0.0153659  -108.413    -7.174  
+23 3 8 60011.00 I -0.043502 0.000026  0.336621 0.000017  I-0.0160102 0.0000068  0.7132 0.0050  I  -108.389    0.793    -7.047    0.047 -0.043530  0.336616 -0.0160051  -108.388    -7.094  
+23 3 9 60012.00 I -0.042359 0.000026  0.339829 0.000017  I-0.0167801 0.0000066  0.8227 0.0047  I  -108.368    0.793    -7.101    0.047 -0.042352  0.339803 -0.0167760  -108.432    -7.140  
+23 310 60013.00 I -0.041267 0.000027  0.343005 0.000018  I-0.0176210 0.0000064  0.8282 0.0040  I  -108.444    0.793    -7.226    0.047 -0.041322  0.343084 -0.0176027  -108.573    -7.251  
+23 311 60014.00 I -0.040748 0.000025  0.346447 0.000017  I-0.0184072 0.0000046  0.7458 0.0039  I  -108.575    0.697    -7.352    0.044 -0.040776  0.346390 -0.0184047  -108.718    -7.379  
+23 312 60015.00 I -0.040536 0.000025  0.349510 0.000018  I-0.0190960 0.0000044  0.6137 0.0032  I  -108.695    0.744    -7.476    0.062 -0.040519  0.349496 -0.0190910  -108.819    -7.513  
+23 313 60016.00 I -0.040082 0.000025  0.352548 0.000019  I-0.0196027 0.0000045  0.3858 0.0027  I  -108.769    0.744    -7.612    0.062 -0.040097  0.352572 -0.0196023  -108.854    -7.660  
+23 314 60017.00 I -0.039698 0.000007  0.355970 0.000010  I-0.0199052 0.0000033  0.2707 0.0028  I  -108.766    0.819    -7.742    0.083 -0.039717  0.355976 -0.0199116  -108.796    -7.801  
+23 315 60018.00 I -0.039666 0.000008  0.359420 0.000012  I-0.0201196 0.0000034  0.0821 0.0029  I  -108.677    0.819    -7.857    0.083 -0.039696  0.359397 -0.0200604  -108.636    -7.924  
+23 316 60019.00 I -0.039798 0.000006  0.362272 0.000011  I-0.0200763 0.0000048 -0.0859 0.0031  I  -108.535    0.819    -7.996    0.083 -0.039824  0.362249 -0.0200712  -108.426    -8.068  
+23 317 60020.00 I -0.039667 0.000007  0.364605 0.000011  I-0.0200343 0.0000053  0.0054 0.0045  I  -108.365    0.819    -8.180    0.083 -0.039666  0.364628 -0.0200376  -108.244    -8.259  
+23 318 60021.00 I -0.039049 0.000020  0.366835 0.000007  I-0.0201240 0.0000075  0.2073 0.0033  I  -108.158    0.322    -8.317    0.160 -0.039047  0.366850 -0.0201299  -108.073    -8.402  
+23 319 60022.00 I -0.038092 0.000017  0.368973 0.000009  I-0.0204889 0.0000039  0.5293 0.0043  I  -107.937    0.599    -8.282    0.090 -0.038102  0.368994 -0.0204875  -107.908    -8.371  
+23 320 60023.00 I -0.036905 0.000017  0.371253 0.000009  I-0.0211554 0.0000042  0.7696 0.0028  I  -107.775    0.599    -8.094    0.090 -0.036907  0.371284 -0.0211416  -107.809    -8.185  
+23 321 60024.00 I -0.035496 0.000017  0.373893 0.000008  I-0.0220019 0.0000041  0.9314 0.0037  I  -107.710    0.599    -7.930    0.090 -0.035480  0.373974 -0.0220007  -107.798    -8.018  
+23 322 60025.00 I -0.033905 0.000025  0.377083 0.000010  I-0.0229764 0.0000061  0.9677 0.0037  I  -107.721    0.684    -7.901    0.056 -0.033918  0.377072 -0.0229616  -107.800    -7.977  
+23 323 60026.00 I -0.032493 0.000024  0.380196 0.000014  I-0.0238902 0.0000062  0.8625 0.0045  I  -107.822    0.684    -7.948    0.056 -0.032503  0.380245 -0.0238876  -107.871    -8.006  
+23 324 60027.00 I -0.031162 0.000024  0.383326 0.000014  I-0.0246804 0.0000065  0.6941 0.0050  I  -108.056    0.684    -7.990    0.056 -0.031173  0.383274 -0.0246908  -108.068    -8.026  
+23 325 60028.00 I -0.029861 0.000018  0.386372 0.000013  I-0.0252312 0.0000079  0.3841 0.0046  I  -108.360    0.735    -8.072    0.009 -0.029863  0.386430 -0.0252241  -108.334    -8.069  
+23 326 60029.00 I -0.028392 0.000026  0.389487 0.000015  I-0.0254402 0.0000065  0.0489 0.0052  I  -108.572    0.797    -8.271    0.102 -0.028402  0.389466 -0.0254315  -108.511    -8.224  
+23 327 60030.00 I -0.026606 0.000026  0.392587 0.000015  I-0.0253812 0.0000069 -0.1298 0.0046  I  -108.602    0.797    -8.526    0.102 -0.026589  0.392633 -0.0253926  -108.515    -8.443  
+23 328 60031.00 I -0.024692 0.000020  0.395475 0.000013  I-0.0251942 0.0000065 -0.2676 0.0044  I  -108.485    0.861    -8.684    0.144 -0.024718  0.395445 -0.0251809  -108.385    -8.580  
+23 329 60032.00 I -0.023036 0.000029  0.397843 0.000026  I-0.0248756 0.0000054 -0.3165 0.0041  I  -108.245    0.745    -8.693    0.104 -0.023029  0.397858 -0.0248761  -108.184    -8.619  
+23 330 60033.00 I -0.021722 0.000030  0.399991 0.000026  I-0.0246029 0.0000050 -0.2402 0.0036  I  -107.847    0.745    -8.664    0.104 -0.021735  0.400017 -0.0245819  -107.840    -8.642  
+23 331 60034.00 I -0.020382 0.000031  0.402301 0.000026  I-0.0244064 0.0000049 -0.1301 0.0039  I  -107.338    0.745    -8.730    0.104 -0.020397  0.402194 -0.0243867  -107.382    -8.762  
+23 4 1 60035.00 I -0.018848 0.000024  0.404529 0.000025  I-0.0243562 0.0000060  0.0206 0.0036  I  -106.916    0.659    -8.865    0.029 -0.018832  0.404562 -0.0243447  -106.941    -8.931  
+23 4 2 60036.00 I -0.017325 0.000029  0.407389 0.000026  I-0.0244586 0.0000052  0.2045 0.0040  I  -106.771    0.730    -8.919    0.073 -0.017339  0.407431 -0.0244585  -106.744    -9.003  
+23 4 3 60037.00 I -0.015631 0.000029  0.409965 0.000026  I-0.0247645 0.0000054  0.3864 0.0037  I  -106.888    0.730    -8.791    0.073 -0.015648  0.409984 -0.0247405  -106.816    -8.883  
+23 4 4 60038.00 I -0.013784 0.000042  0.412645 0.000018  I-0.0252246 0.0000053  0.5480 0.0038  I  -107.097    0.753    -8.552    0.102 -0.013789  0.412618 -0.0252154  -107.008    -8.648  
+23 4 5 60039.00 I -0.012264 0.000041  0.415415 0.000017  I-0.0258463 0.0000053  0.6670 0.0037  I  -107.266    0.753    -8.375    0.102 -0.012263  0.415517 -0.0258359  -107.244    -8.468  
+23 4 6 60040.00 I -0.010735 0.000041  0.418382 0.000017  I-0.0265279 0.0000052  0.6940 0.0037  I  -107.393    0.753    -8.366    0.102 -0.010755  0.418256 -0.0265377  -107.466    -8.452  
+23 4 7 60041.00 I -0.009106 0.000041  0.421127 0.000017  I-0.0272224 0.0000052  0.6855 0.0037  I  -107.524    0.753    -8.494    0.102 -0.009065  0.421259 -0.0272490  -107.657    -8.560  
+23 4 8 60042.00 I -0.007833 0.000037  0.423806 0.000016  I-0.0278761 0.0000054  0.6087 0.0038  I  -107.660    0.624    -8.657    0.090 -0.007878  0.423780 -0.0279197  -107.816    -8.694  
+23 4 9 60043.00 I -0.006560 0.000037  0.426282 0.000016  I-0.0284239 0.0000055  0.4840 0.0048  I  -107.779    0.624    -8.785    0.090 -0.006541  0.426318 -0.0284814  -107.930    -8.792  
+23 410 60044.00 I -0.005306 0.000029  0.428793 0.000031  I-0.0288276 0.0000080  0.3096 0.0052  I  -107.855    0.779    -8.886    0.045 -0.005307  0.428835 -0.0288476  -107.977    -8.867  
+23 411 60045.00 I -0.004025 0.000029  0.431383 0.000031  I-0.0290272 0.0000089  0.0876 0.0057  I  -107.836    0.779    -9.002    0.045 -0.004073  0.431351 -0.0290184  -107.906    -8.967  
+23 412 60046.00 I -0.002976 0.000030  0.434126 0.000051  I-0.0290339 0.0000080 -0.0409 0.0060  I  -107.633    0.766    -9.151    0.031 -0.002903  0.434183 -0.0290346  -107.627    -9.117  
+23 413 60047.00 I -0.002341 0.000030  0.436681 0.000051  I-0.0289873 0.0000080 -0.0437 0.0056  I  -107.208    0.766    -9.309    0.031 -0.002436  0.436715 -0.0289857  -107.084    -9.311  
+23 414 60048.00 I -0.001850 0.000030  0.439402 0.000051  I-0.0290013 0.0000079  0.1179 0.0055  I  -106.677    0.766    -9.419    0.031 -0.001750  0.439264 -0.0290056  -106.448    -9.462  
+23 415 60049.00 I -0.001120 0.000030  0.441595 0.000051  I-0.0292514 0.0000076  0.3645 0.0056  I  -106.261    0.766    -9.425    0.031 -0.001196  0.441724 -0.0292618  -106.033    -9.492  
+23 416 60050.00 I  0.000181 0.000013  0.443576 0.000041  I-0.0297607 0.0000078  0.7022 0.0054  I  -106.127    0.661    -9.315    0.035  0.000214  0.443555 -0.0298215  -105.983    -9.387  
+23 417 60051.00 I  0.001683 0.000013  0.445277 0.000041  I-0.0306278 0.0000076  0.9559 0.0053  I  -106.268    0.661    -9.142    0.035  0.001716  0.445308 -0.0306441  -106.240    -9.208  
+23 418 60052.00 I  0.002957 0.000010  0.446935 0.000020  I-0.0316004 0.0000073  0.9932 0.0049  I  -106.524    0.617    -8.994    0.039  0.002942  0.446930 -0.0316096  -106.615    -9.044  
+23 419 60053.00 I  0.004303 0.000009  0.448609 0.000012  I-0.0325682 0.0000062  0.8925 0.0049  I  -106.731    0.633    -8.924    0.038  0.004306  0.448627 -0.0325371  -106.853    -8.950  
+23 420 60054.00 I  0.005750 0.000009  0.450431 0.000012  I-0.0333569 0.0000065  0.7063 0.0045  I  -106.852    0.633    -8.926    0.038  0.005723  0.450456 -0.0333578  -106.967    -8.923  
+23 421 60055.00 I  0.007438 0.000009  0.452639 0.000012  I-0.0339589 0.0000066  0.4543 0.0044  I  -106.948    0.633    -8.980    0.038  0.007430  0.452633 -0.0339749  -107.047    -8.949  
+23 422 60056.00 I  0.009113 0.000020  0.455105 0.000012  I-0.0342654 0.0000058  0.2021 0.0041  I  -107.071    0.708    -9.100    0.032  0.009155  0.455143 -0.0342997  -107.160    -9.039  
+23 423 60057.00 I  0.010724 0.000032  0.457859 0.000023  I-0.0343794 0.0000048 -0.0013 0.0038  I  -107.189    0.867    -9.283    0.098  0.010695  0.457843 -0.0343744  -107.269    -9.198  
+23 424 60058.00 I  0.012614 0.000032  0.460577 0.000023  I-0.0342718 0.0000048 -0.1779 0.0036  I  -107.237    0.867    -9.464    0.098  0.012615  0.460612 -0.0342760  -107.304    -9.366  
+23 425 60059.00 I  0.015009 0.000032  0.462926 0.000020  I-0.0340645 0.0000054 -0.2320 0.0033  I  -107.173    0.890    -9.563    0.107  0.014950  0.462927 -0.0340746  -107.224    -9.466  
+23 426 60060.00 I  0.017312 0.000033  0.465023 0.000034  I-0.0338275 0.0000046 -0.2271 0.0036  I  -106.980    0.933    -9.587    0.147  0.017333  0.465001 -0.0338446  -106.721    -9.586  
+23 427 60061.00 I  0.019416 0.000033  0.467073 0.000034  I-0.0336237 0.0000047 -0.1820 0.0033  I  -106.641    0.933    -9.638    0.147  0.019395  0.467135 -0.0336272  -106.199    -9.723  
+23 428 60062.00 I  0.021468 0.000033  0.469219 0.000034  I-0.0334925 0.0000048 -0.0499 0.0036  I  -106.189    0.933    -9.790    0.147  0.021422  0.469079 -0.0335007  -105.977    -9.882  
+23 429 60063.00 I  0.023805 0.000011  0.470578 0.000028  I-0.0335470 0.0000055  0.1516 0.0036  I  -105.765    1.082    -9.985    0.227  0.023823  0.470667 -0.0335561  -106.132    -9.986  
+23 430 60064.00 I  0.026003 0.000011  0.472109 0.000028  I-0.0337976 0.0000055  0.3590 0.0037  I  -105.564    1.082   -10.071    0.227  0.025987  0.472089 -0.0338124  -105.944   -10.067  
+23 5 1 60065.00 I  0.027600 0.000015  0.473426 0.000028  I-0.0342597 0.0000049  0.5507 0.0041  I  -105.694    1.064    -9.951    0.192  0.027605  0.473468 -0.0342084  -106.095    -9.946  
+23 5 2 60066.00 I  0.028831 0.000012  0.474625 0.000007  I-0.0348515 0.0000062  0.5999 0.0033  I  -106.075    1.057    -9.680    0.172  0.028796  0.474630 -0.0347850  -105.942    -9.706  
+23 5 3 60067.00 I  0.030251 0.000031  0.475662 0.000008  I-0.0354574 0.0000044  0.6427 0.0040  I  -106.506    0.975    -9.411    0.136  0.030234  0.475690 -0.0354724  -106.395    -9.387  
+23 5 4 60068.00 I  0.031941 0.000031  0.476548 0.000007  I-0.0361452 0.0000050  0.7103 0.0034  I  -106.826    0.975    -9.271    0.136  0.031924  0.476551 -0.0361704  -106.827    -9.225  
+23 5 5 60069.00 I  0.033845 0.000031  0.477603 0.000009  I-0.0368151 0.0000051  0.5890 0.0037  I  -107.022    0.975    -9.290    0.136  0.033840  0.477643 -0.0368208  -107.154    -9.237  
+23 5 6 60070.00 I  0.035724 0.000031  0.478662 0.000009  I-0.0373353 0.0000055  0.5038 0.0043  I  -107.188    0.975    -9.428    0.136  0.035678  0.478685 -0.0373656  -107.390    -9.396  
+23 5 7 60071.00 I  0.037836 0.000038  0.479793 0.000030  I-0.0377855 0.0000068  0.3069 0.0048  I  -107.373    0.920    -9.628    0.167  0.037872  0.479777 -0.0377721  -107.589    -9.635  
+23 5 8 60072.00 I  0.039839 0.000038  0.481255 0.000030  I-0.0379544 0.0000078  0.1257 0.0062  I  -107.500    0.920    -9.836    0.167  0.039787  0.481291 -0.0379959  -107.700    -9.885  
+23 5 9 60073.00 I  0.041704 0.000025  0.482630 0.000030  I-0.0380837 0.0000104  0.0848 0.0058  I  -107.443    0.994   -10.008    0.234  0.041742  0.482696 -0.0381001  -107.603   -10.090  
+23 510 60074.00 I  0.043557 0.000025  0.484312 0.000030  I-0.0381446 0.0000085  0.1058 0.0066  I  -107.149    1.000   -10.119    0.197  0.043548  0.484305 -0.0381955  -107.267   -10.183  
+23 511 60075.00 I  0.045314 0.000025  0.485508 0.000030  I-0.0383696 0.0000081  0.3496 0.0059  I  -106.699    1.000   -10.165    0.197  0.045281  0.485514 -0.0383861  -106.770   -10.195  
+23 512 60076.00 I  0.047290 0.000025  0.486616 0.000030  I-0.0388384 0.0000083  0.5773 0.0057  I  -106.246    1.000   -10.153    0.197  0.047344  0.486618 -0.0388214  -106.269   -10.150  
+23 513 60077.00 I  0.049460 0.000005  0.487744 0.000008  I-0.0395345 0.0000081  0.8358 0.0050  I  -105.936    1.005   -10.087    0.139  0.049455  0.487750 -0.0395385  -105.913   -10.091  
+23 514 60078.00 I  0.052351 0.000021  0.489073 0.000012  I-0.0405268 0.0000055  1.1446 0.0049  I  -105.846    1.079    -9.969    0.182  0.052341  0.489096 -0.0405378  -105.788   -10.004  
+23 515 60079.00 I  0.055852 0.000021  0.490657 0.000013  I-0.0417798 0.0000054  1.3216 0.0039  I  -105.980    1.079    -9.813    0.182  0.055853  0.490619 -0.0417757  -105.905    -9.881  
+23 516 60080.00 I  0.059212 0.000021  0.492163 0.000013  I-0.0431017 0.0000055  1.2936 0.0045  I  -106.272    1.136    -9.632    0.204  0.059171  0.492264 -0.0430984  -106.202    -9.725  
+23 517 60081.00 I  0.062104 0.000026  0.493475 0.000034  I-0.0443111 0.0000071  1.0980 0.0044  I  -106.604    1.064    -9.451    0.191  0.062111  0.493466 -0.0442928  -106.606    -9.528  
+23 518 60082.00 I  0.064531 0.000027  0.494597 0.000034  I-0.0452747 0.0000068  0.8336 0.0049  I  -106.856    1.064    -9.325    0.191  0.064515  0.494600 -0.0452544  -106.953    -9.369  
+23 519 60083.00 I  0.066937 0.000026  0.495682 0.000034  I-0.0459525 0.0000068  0.4920 0.0064  I  -106.975    1.064    -9.323    0.191  0.066867  0.495722 -0.0459063  -107.164    -9.334  
+23 520 60084.00 I  0.069365 0.000017  0.496663 0.000033  I-0.0462786 0.0000109  0.2102 0.0062  I  -107.015    0.667    -9.474    0.128  0.069368  0.496634 -0.0462641  -107.252    -9.474  
+23 521 60085.00 I  0.071648 0.000023  0.497520 0.000038  I-0.0463878 0.0000103 -0.0268 0.0075  I  -107.074    0.700    -9.712    0.101  0.071680  0.497569 -0.0463853  -107.324    -9.715  
+23 522 60086.00 I  0.073705 0.000023  0.498181 0.000038  I-0.0462358 0.0000103 -0.2312 0.0069  I  -107.188    0.700    -9.906    0.101  0.073653  0.498156 -0.0462514  -107.428    -9.915  
+23 523 60087.00 I  0.076150 0.000016  0.498891 0.000021  I-0.0459752 0.0000093 -0.2861 0.0061  I  -107.307    0.737    -9.971    0.056  0.076168  0.498968 -0.0459896  -107.516    -9.986  
+23 524 60088.00 I  0.079193 0.000041  0.499992 0.000037  I-0.0456708 0.0000064 -0.3194 0.0057  I  -107.358    0.969    -9.954    0.034  0.079160  0.500036 -0.0456668  -107.507    -9.957  
+23 525 60089.00 I  0.082204 0.000041  0.501052 0.000037  I-0.0453531 0.0000066 -0.3025 0.0046  I  -107.302    0.969    -9.975    0.034  0.082179  0.501016 -0.0453568  -107.375    -9.963  
+23 526 60090.00 I  0.084853 0.000041  0.502354 0.000037  I-0.0450873 0.0000065 -0.2211 0.0044  I  -107.120    0.969   -10.090    0.034  0.084872  0.502481 -0.0450984  -107.114   -10.061  
+23 527 60091.00 I  0.086769 0.000038  0.503688 0.000032  I-0.0449419 0.0000057 -0.0468 0.0043  I  -106.837    1.008   -10.209    0.021  0.086698  0.503700 -0.0449506  -106.780   -10.181  
+23 528 60092.00 I  0.088639 0.000039  0.504437 0.000032  I-0.0449941 0.0000057  0.1286 0.0038  I  -106.593    1.008   -10.191    0.021  0.088656  0.504426 -0.0449906  -106.507   -10.177  
+23 529 60093.00 I  0.090321 0.000043  0.505220 0.000032  I-0.0451722 0.0000051  0.2235 0.0039  I  -106.625    1.075    -9.995    0.074  0.090327  0.505272 -0.0452128  -106.520    -9.999  
+23 530 60094.00 I  0.091899 0.000020  0.506023 0.000020  I-0.0454413 0.0000054  0.3192 0.0040  I  -107.063    1.078    -9.714    0.121  0.091878  0.506018 -0.0454994  -106.948    -9.740  
+23 531 60095.00 I  0.093774 0.000020  0.506956 0.000020  I-0.0457732 0.0000062  0.3027 0.0044  I  -107.752    1.078    -9.472    0.121  0.093791  0.507001 -0.0457819  -107.635    -9.519  
+23 6 1 60096.00 I  0.096370 0.000020  0.507734 0.000020  I-0.0460240 0.0000070  0.2182 0.0046  I  -108.375    1.078    -9.317    0.121  0.096355  0.507784 -0.0460391  -108.261    -9.384  
+23 6 2 60097.00 I  0.099265 0.000020  0.508665 0.000020  I-0.0461938 0.0000068  0.0864 0.0050  I  -108.771    1.078    -9.254    0.121  0.099280  0.508684 -0.0462257  -108.791    -9.317  
+23 6 3 60098.00 I  0.102230 0.000020  0.509354 0.000020  I-0.0461713 0.0000072 -0.1219 0.0051  I  -109.044    1.078    -9.317    0.121  0.102195  0.509333 -0.0462142  -109.187    -9.367  
+23 6 4 60099.00 I  0.105157 0.000012  0.509999 0.000025  I-0.0459322 0.0000075 -0.3837 0.0057  I  -109.305    0.792    -9.541    0.138  0.105220  0.510064 -0.0459633  -109.506    -9.580  
+23 6 5 60100.00 I  0.108078 0.000011  0.510397 0.000016  I-0.0454376 0.0000089 -0.5446 0.0058  I  -109.445    0.644    -9.851    0.150  0.108006  0.510376 -0.0454993  -109.649    -9.884  
+23 6 6 60101.00 I  0.111198 0.000011  0.510745 0.000017  I-0.0449083 0.0000088 -0.5097 0.0062  I  -109.295    0.644   -10.074    0.150  0.111217  0.510811 -0.0449675  -109.453   -10.109  
+23 6 7 60102.00 I  0.114163 0.000020  0.511310 0.000040  I-0.0444264 0.0000085 -0.4501 0.0060  I  -108.909    0.644   -10.097    0.150  0.114187  0.511330 -0.0444769  -108.948   -10.159  
+23 6 8 60103.00 I  0.116581 0.000020  0.511550 0.000040  I-0.0440545 0.0000083 -0.2511 0.0060  I  -108.560    0.644    -9.977    0.150  0.116506  0.511524 -0.0441244  -108.464   -10.073  
+23 6 9 60104.00 I  0.119116 0.000020  0.511727 0.000040  I-0.0439350 0.0000085 -0.0196 0.0070  I  -108.448    0.644    -9.842    0.150  0.119171  0.511814 -0.0439844  -108.237    -9.970  
+23 610 60105.00 I  0.121701 0.000017  0.512173 0.000037  I-0.0440159 0.0000112  0.2138 0.0069  I  -108.532    0.322    -9.753    0.160  0.121697  0.512135 -0.0440725  -108.326    -9.905  
+23 611 60106.00 I  0.123858 0.000049  0.512538 0.000038  I-0.0443160 0.0000109  0.3075 0.0077  I  -108.648    0.864    -9.684    0.271  0.123832  0.512556 -0.0443300  -108.523    -9.845  
+23 612 60107.00 I  0.126114 0.000049  0.512876 0.000038  I-0.0445773 0.0000105  0.2403 0.0072  I  -108.723    0.864    -9.586    0.271  0.126093  0.512902 -0.0446157  -108.701    -9.737  
+23 613 60108.00 I  0.128699 0.000049  0.513073 0.000028  I-0.0447853 0.0000095  0.1391 0.0071  I  -108.831    0.888    -9.439    0.233  0.128655  0.513023 -0.0448327  -108.912    -9.554  
+23 614 60109.00 I  0.131242 0.000049  0.513140 0.000028  I-0.0448216 0.0000096 -0.0639 0.0066  I  -109.056    0.888    -9.260    0.233  0.131265  0.513186 -0.0448926  -109.174    -9.285  
+23 615 60110.00 I  0.133780 0.000049  0.513009 0.000028  I-0.0446568 0.0000093 -0.2690 0.0066  I  -109.339    0.888    -9.124    0.233  0.133765  0.513018 -0.0447062  -109.492    -9.052  
+23 616 60111.00 I  0.136503 0.000049  0.512875 0.000028  I-0.0442575 0.0000091 -0.5523 0.0053  I  -109.526    0.888    -9.145    0.233  0.136473  0.512884 -0.0442808  -109.770    -9.013  
+23 617 60112.00 I  0.139488 0.000017  0.512879 0.000027  I-0.0435763 0.0000052 -0.7632 0.0051  I  -109.550    0.956    -9.385    0.089  0.139533  0.512907 -0.0436680  -109.901    -9.229  
+23 618 60113.00 I  0.142516 0.000017  0.512712 0.000054  I-0.0427860 0.0000046 -0.8093 0.0042  I  -109.507    1.247    -9.763    0.196  0.142445  0.512759 -0.0429057  -109.870    -9.622  
+23 619 60114.00 I  0.145637 0.000020  0.512563 0.000047  I-0.0419678 0.0000066 -0.8251 0.0054  I  -109.529    1.297   -10.071    0.219  0.145679  0.512473 -0.0420518  -109.834    -9.972  
+23 620 60115.00 I  0.148706 0.000020  0.512055 0.000047  I-0.0411442 0.0000097 -0.8157 0.0058  I  -109.655    1.297   -10.150    0.219  0.148651  0.512369 -0.0411848  -109.895   -10.094  
+23 621 60116.00 I  0.152070 0.000019  0.512066 0.000048  I-0.0403426 0.0000096 -0.7876 0.0068  I  -109.837    1.250   -10.029    0.210  0.151998  0.511955 -0.0403854  -110.135    -9.968  
+23 622 60117.00 I  0.155443 0.000019  0.511494 0.000048  I-0.0395953 0.0000096 -0.6806 0.0069  I  -110.009    1.250    -9.883    0.210  0.155498  0.511551 -0.0396589  -110.417    -9.796  
+23 623 60118.00 I  0.158403 0.000019  0.511221 0.000048  I-0.0389783 0.0000099 -0.5830 0.0087  I  -110.094    1.250    -9.826    0.210  0.158323  0.511208 -0.0390256  -110.606    -9.712  
+23 624 60119.00 I  0.161365 0.000019  0.510804 0.000008  I-0.0384428 0.0000145 -0.4450 0.0074  I  -110.007    0.861    -9.794    0.172  0.161368  0.510809 -0.0384982  -110.515    -9.706  
+23 625 60120.00 I  0.164249 0.000021  0.510670 0.000008  I-0.0380774 0.0000110 -0.3397 0.0089  I  -109.803    1.079    -9.660    0.230  0.164234  0.510724 -0.0380713  -110.238    -9.623  
+23 626 60121.00 I  0.167178 0.000021  0.510316 0.000009  I-0.0377433 0.0000102 -0.2947 0.0076  I  -109.764    1.079    -9.423    0.230  0.167176  0.510340 -0.0377554  -110.105    -9.436  
+23 627 60122.00 I  0.170453 0.000008  0.509954 0.000006  I-0.0374955 0.0000106 -0.2271 0.0064  I  -110.204    1.184    -9.229    0.266  0.170433  0.509962 -0.0375206  -110.449    -9.278  
+23 628 60123.00 I  0.173919 0.000012  0.509928 0.000009  I-0.0372671 0.0000077 -0.2256 0.0065  I  -111.085    1.184    -9.186    0.266  0.173953  0.509955 -0.0373143  -111.285    -9.197  
+23 629 60124.00 I  0.177044 0.000012  0.509642 0.000009  I-0.0370206 0.0000075 -0.2952 0.0050  I  -111.994    1.184    -9.230    0.266  0.176991  0.509637 -0.0370420  -112.173    -9.179  
+23 630 60125.00 I  0.180255 0.000012  0.509092 0.000008  I-0.0366540 0.0000064 -0.4328 0.0062  I  -112.579    1.184    -9.242    0.266  0.180263  0.509120 -0.0366739  -112.749    -9.132  
+23 7 1 60126.00 I  0.183654 0.000009  0.508460 0.000008  I-0.0361420 0.0000098 -0.6093 0.0071  I  -112.863    0.322    -9.254    0.160  0.183626  0.508483 -0.0361336  -113.043    -9.133  
+23 7 2 60127.00 I  0.187232 0.000022  0.507857 0.000007  I-0.0354092 0.0000127 -0.8644 0.0090  I  -113.003    1.020    -9.398    0.262  0.187226  0.507848 -0.0353981  -113.199    -9.303  
+23 7 3 60128.00 I  0.190493 0.000022  0.507547 0.000007  I-0.0344555 0.0000150 -0.9927 0.0117  I  -112.960    1.020    -9.659    0.262  0.190492  0.507593 -0.0344896  -113.166    -9.608  
+23 7 4 60129.00 I  0.193205 0.000021  0.507362 0.000020  I-0.0334907 0.0000196 -0.9204 0.0115  I  -112.649    1.020    -9.812    0.262  0.193198  0.507334 -0.0335318  -112.851    -9.818  
+23 7 5 60130.00 I  0.195889 0.000037  0.507029 0.000034  I-0.0326182 0.0000174 -0.8376 0.0132  I  -112.259    0.910    -9.709    0.310  0.195908  0.507073 -0.0326419  -112.408    -9.794  
+23 7 6 60131.00 I  0.198442 0.000037  0.506393 0.000034  I-0.0318642 0.0000178 -0.6088 0.0126  I  -112.141    0.910    -9.480    0.310  0.198426  0.506374 -0.0319144  -112.214    -9.638  
+23 7 7 60132.00 I  0.201259 0.000037  0.505435 0.000034  I-0.0314178 0.0000183 -0.3283 0.0132  I  -112.414    0.910    -9.340    0.310  0.201220  0.505514 -0.0314343  -112.403    -9.552  
+23 7 8 60133.00 I  0.204172 0.000031  0.504531 0.000034  I-0.0311585 0.0000195 -0.1951 0.0119  I  -112.874    0.870    -9.316    0.325  0.204156  0.504535 -0.0311542  -112.760    -9.535  
+23 7 9 60134.00 I  0.206990 0.000033  0.503195 0.000035  I-0.0309693 0.0000152 -0.2367 0.0122  I  -113.256    0.942    -9.283    0.198  0.207001  0.503185 -0.0309623  -113.071    -9.471  
+23 710 60135.00 I  0.209579 0.000033  0.501981 0.000035  I-0.0306723 0.0000146 -0.3168 0.0106  I  -113.461    0.942    -9.180    0.198  0.209533  0.502013 -0.0306936  -113.323    -9.301  
+23 711 60136.00 I  0.212142 0.000012  0.500918 0.000009  I-0.0303095 0.0000149 -0.4757 0.0093  I  -113.575    0.957    -9.068    0.120  0.212151  0.500923 -0.0302988  -113.566    -9.109  
+23 712 60137.00 I  0.214605 0.000013  0.499871 0.000011  I-0.0297120 0.0000115 -0.6615 0.0091  I  -113.757    0.893    -9.004    0.147  0.214585  0.499885 -0.0297092  -113.875    -9.024  
+23 713 60138.00 I  0.216947 0.000013  0.498769 0.000010  I-0.0289469 0.0000105 -0.9661 0.0077  I  -114.072    0.893    -8.999    0.147  0.216926  0.498812 -0.0288524  -114.299    -9.039  
+23 714 60139.00 I  0.219377 0.000013  0.497558 0.000010  I-0.0278010 0.0000103 -1.2070 0.0070  I  -114.413    0.893    -9.084    0.147  0.219379  0.497583 -0.0277983  -114.717    -9.160  
+23 715 60140.00 I  0.221889 0.000006  0.496510 0.000006  I-0.0266107 0.0000092 -1.2144 0.0059  I  -114.616    0.722    -9.321    0.182  0.221871  0.496538 -0.0265972  -114.866    -9.393  
+23 716 60141.00 I  0.224427 0.000007  0.495448 0.000007  I-0.0253391 0.0000059 -1.3209 0.0057  I  -114.645    1.024    -9.685    0.158  0.224374  0.495464 -0.0253009  -114.764    -9.731  
+23 717 60142.00 I  0.226909 0.000007  0.494539 0.000007  I-0.0240251 0.0000068 -1.2587 0.0049  I  -114.609    1.024    -9.988    0.158  0.226953  0.494546 -0.0240270  -114.584   -10.007  
+23 718 60143.00 I  0.228994 0.000020  0.493777 0.000020  I-0.0228508 0.0000078 -1.1093 0.0044  I  -114.624    1.201   -10.018    0.136  0.228983  0.493824 -0.0228538  -114.472   -10.018  
+23 719 60144.00 I  0.231013 0.000012  0.493052 0.000039  I-0.0218066 0.0000057 -0.9596 0.0049  I  -114.722    1.082    -9.751    0.199  0.230996  0.493045 -0.0218364  -114.568    -9.765  
+23 720 60145.00 I  0.233355 0.000012  0.492246 0.000039  I-0.0209746 0.0000059 -0.6808 0.0041  I  -114.866    1.082    -9.391    0.199  0.233340  0.492282 -0.0210160  -114.761    -9.434  
+23 721 60146.00 I  0.235890 0.000012  0.491027 0.000039  I-0.0204262 0.0000059 -0.4584 0.0046  I  -114.974    1.082    -9.147    0.199  0.235893  0.491075 -0.0204242  -114.934    -9.222  
+23 722 60147.00 I  0.238222 0.000011  0.489964 0.000039  I-0.0200288 0.0000070 -0.3231 0.0036  I  -114.949    1.029    -9.032    0.232  0.238218  0.489978 -0.0200295  -114.946    -9.121  
+23 723 60148.00 I  0.240419 0.000016  0.488596 0.000057  I-0.0197763 0.0000040 -0.1991 0.0041  I  -114.785    0.967    -8.923    0.216  0.240409  0.488602 -0.0197499  -114.802    -9.012  
+23 724 60149.00 I  0.242681 0.000017  0.487124 0.000057  I-0.0195905 0.0000042 -0.1954 0.0032  I  -114.703    0.967    -8.789    0.216  0.242675  0.487119 -0.0195468  -114.739    -8.873  
+23 725 60150.00 I  0.245000 0.000013  0.485359 0.000042  I-0.0193684 0.0000051 -0.2428 0.0037  I  -115.034    0.902    -8.766    0.201  0.244998  0.485494 -0.0193720  -115.090    -8.835  
+23 726 60151.00 I  0.247381 0.000031  0.484001 0.000051  I-0.0191007 0.0000061 -0.3027 0.0040  I  -115.842    0.886    -8.960    0.179  0.247369  0.483986 -0.0191211  -115.939    -9.007  
+23 727 60152.00 I  0.249854 0.000031  0.482335 0.000051  I-0.0187258 0.0000061 -0.4742 0.0043  I  -116.755    0.886    -9.264    0.179  0.249864  0.482311 -0.0187234  -116.894    -9.285  
+23 728 60153.00 I  0.252323 0.000031  0.480728 0.000051  I-0.0181421 0.0000061 -0.6764 0.0055  I  -117.325    0.886    -9.458    0.179  0.252271  0.480832 -0.0181468  -117.493    -9.459  
+23 729 60154.00 I  0.254520 0.000029  0.479139 0.000030  I-0.0173864 0.0000092 -0.8384 0.0048  I  -117.454    0.837    -9.494    0.119  0.254520  0.479116 -0.0174005  -117.597    -9.513  
+23 730 60155.00 I  0.256292 0.000042  0.477282 0.000031  I-0.0164854 0.0000074 -0.9401 0.0059  I  -117.305    0.927    -9.527    0.250  0.256321  0.477330 -0.0165264  -117.387    -9.585  
+23 731 60156.00 I  0.257766 0.000042  0.475300 0.000031  I-0.0155656 0.0000074 -0.8637 0.0052  I  -116.972    0.927    -9.619    0.250  0.257717  0.475332 -0.0156145  -116.980    -9.717  
+23 8 1 60157.00 I  0.259476 0.000031  0.473311 0.000008  I-0.0147895 0.0000072 -0.6927 0.0052  I  -116.535    0.969    -9.606    0.306  0.259552  0.473316 -0.0148009  -116.465    -9.735  
+23 8 2 60158.00 I  0.261556 0.000036  0.471666 0.000015  I-0.0142002 0.0000072 -0.4615 0.0053  I  -116.267    1.008    -9.387    0.257  0.261538  0.471686 -0.0141968  -116.134    -9.492  
+23 8 3 60159.00 I  0.263447 0.000036  0.470046 0.000015  I-0.0138929 0.0000077 -0.1509 0.0054  I  -116.433    1.008    -9.167    0.257  0.263444  0.470105 -0.0138930  -116.254    -9.229  
+23 8 4 60160.00 I  0.265540 0.000036  0.468278 0.000015  I-0.0138750 0.0000080  0.0897 0.0063  I  -116.934    1.008    -9.199    0.257  0.265536  0.468247 -0.0138656  -116.730    -9.216  
+23 8 5 60161.00 I  0.267937 0.000019  0.466354 0.000014  I-0.0140318 0.0000099  0.2087 0.0055  I  -117.441    1.080    -9.402    0.152  0.267930  0.466413 -0.0140118  -117.309    -9.399  
+23 8 6 60162.00 I  0.270506 0.000039  0.464863 0.000015  I-0.0142155 0.0000075  0.0968 0.0062  I  -117.800    0.747    -9.480    0.155  0.270493  0.464868 -0.0141542  -117.788    -9.473  
+23 8 7 60163.00 I  0.272844 0.000039  0.463553 0.000014  I-0.0141764 0.0000075 -0.1621 0.0055  I  -118.075    0.747    -9.347    0.155  0.272864  0.463581 -0.0141484  -118.179    -9.345  
+23 8 8 60164.00 I  0.274687 0.000034  0.462161 0.000006  I-0.0139122 0.0000081 -0.3584 0.0049  I  -118.305    0.429    -9.214    0.156  0.274685  0.462231 -0.0139140  -118.493    -9.221  
+23 8 9 60165.00 I  0.276342 0.000043  0.460645 0.000041  I-0.0134468 0.0000064 -0.5932 0.0050  I  -118.472    0.665    -9.257    0.155  0.276337  0.460613 -0.0134271  -118.588    -9.279  
+23 810 60166.00 I  0.277799 0.000043  0.458742 0.000041  I-0.0127102 0.0000058 -0.8748 0.0042  I  -118.624    0.665    -9.412    0.155  0.277790  0.458807 -0.0127031  -118.608    -9.447  
+23 811 60167.00 I  0.279016 0.000043  0.456435 0.000042  I-0.0117167 0.0000055 -1.0978 0.0049  I  -118.809    0.665    -9.545    0.155  0.278994  0.456494 -0.0117351  -118.653    -9.582  
+23 812 60168.00 I  0.279961 0.000027  0.454704 0.000042  I-0.0105583 0.0000080 -1.1896 0.0045  I  -118.945    0.867    -9.650    0.154  0.279970  0.454733 -0.0106076  -118.715    -9.638  
+23 813 60169.00 I  0.280816 0.000030  0.452597 0.000042  I-0.0093773 0.0000071 -1.1619 0.0058  I  -118.917    0.867    -9.791    0.154  0.280771  0.452604 -0.0094177  -118.658    -9.705  
+23 814 60170.00 I  0.281796 0.000030  0.450670 0.000042  I-0.0082372 0.0000084 -1.1260 0.0075  I  -118.742    0.867    -9.916    0.154  0.281823  0.450679 -0.0082485  -118.477    -9.763  
+23 815 60171.00 I  0.282782 0.000014  0.448827 0.000010  I-0.0071513 0.0000131 -1.0121 0.0067  I  -118.548    0.322    -9.854    0.160  0.282744  0.448904 -0.0071781  -118.294    -9.656  
+23 816 60172.00 I  0.283523 0.000047  0.447048 0.000013  I-0.0062492 0.0000105 -0.7897 0.0085  I  -118.424    0.967    -9.523    0.141  0.283572  0.447025 -0.0062732  -118.177    -9.364  
+23 817 60173.00 I  0.284180 0.000047  0.445115 0.000012  I-0.0055513 0.0000109 -0.6292 0.0076  I  -118.366    0.967    -9.080    0.141  0.284154  0.445183 -0.0055690  -118.140    -8.999  
+23 818 60174.00 I  0.285144 0.000047  0.442948 0.000012  I-0.0049903 0.0000109 -0.4702 0.0079  I  -118.322    0.967    -8.780    0.141  0.285203  0.442912 -0.0050148  -118.142    -8.791  
+23 819 60175.00 I  0.286579 0.000045  0.440612 0.000011  I-0.0046030 0.0000114 -0.3351 0.0076  I  -118.245    0.967    -8.720    0.141  0.286566  0.440690 -0.0045717  -118.160    -8.828  
+23 820 60176.00 I  0.287716 0.000045  0.438143 0.000011  I-0.0042600 0.0000106 -0.3805 0.0077  I  -118.130    0.967    -8.790    0.141  0.287747  0.438093 -0.0041923  -118.159    -8.978  
+23 821 60177.00 I  0.288646 0.000056  0.435394 0.000048  I-0.0038329 0.0000104 -0.4533 0.0078  I  -118.069    0.763    -8.868    0.196  0.288671  0.435493 -0.0038044  -118.243    -9.084  
+23 822 60178.00 I  0.289772 0.000033  0.432444 0.000047  I-0.0033618 0.0000115 -0.5008 0.0074  I  -118.245    0.620    -8.982    0.225  0.289769  0.432356 -0.0033527  -118.537    -9.172  
+23 823 60179.00 I  0.291360 0.000036  0.429611 0.000048  I-0.0028135 0.0000105 -0.6016 0.0076  I  -118.744    0.620    -9.218    0.225  0.291358  0.429819 -0.0027933  -119.045    -9.335  
+23 824 60180.00 I  0.292543 0.000036  0.427326 0.000048  I-0.0021328 0.0000098 -0.7799 0.0072  I  -119.369    0.620    -9.528    0.225  0.292539  0.427299 -0.0020899  -119.401    -9.502  
+23 825 60181.00 I  0.294072 0.000036  0.424751 0.000048  I-0.0012525 0.0000099 -0.9618 0.0070  I  -119.770    0.620    -9.734    0.225  0.294147  0.424781 -0.0012425  -119.430    -9.558  
+23 826 60182.00 I  0.296076 0.000036  0.422629 0.000048  I-0.0002470 0.0000099 -1.0304 0.0058  I  -119.768    0.620    -9.745    0.225  0.296042  0.422672 -0.0002644  -119.256    -9.553  
+23 827 60183.00 I  0.298285 0.000016  0.420622 0.000039  I 0.0007728 0.0000062 -0.9926 0.0057  I  -119.442    0.971    -9.646    0.262  0.298312  0.420663  0.0007542  -118.937    -9.547  
+23 828 60184.00 I  0.300343 0.000016  0.418969 0.000039  I 0.0017092 0.0000058 -0.8680 0.0044  I  -118.964    0.971    -9.514    0.262  0.300336  0.418954  0.0017213  -118.543    -9.548  
+23 829 60185.00 I  0.302084 0.000008  0.417455 0.000038  I 0.0024624 0.0000062 -0.6042 0.0047  I  -118.543    0.971    -9.271    0.262  0.302082  0.417627  0.0024765  -118.239    -9.441  
+23 830 60186.00 I  0.303510 0.000009  0.416426 0.000040  I 0.0028567 0.0000074 -0.1576 0.0047  I  -118.455    0.965    -8.903    0.256  0.303509  0.416370  0.0028590  -118.177    -9.106  
+23 831 60187.00 I  0.304430 0.000009  0.414907 0.000040  I 0.0028241 0.0000071  0.1495 0.0051  I  -118.803    0.965    -8.656    0.256  0.304481  0.414958  0.0028596  -118.523    -8.848  
+23 9 1 60188.00 I  0.304726 0.000009  0.413283 0.000040  I 0.0025930 0.0000071  0.3509 0.0060  I  -119.288    0.965    -8.788    0.256  0.304685  0.413225  0.0025855  -119.010    -8.951  
+23 9 2 60189.00 I  0.304826 0.000007  0.411150 0.000015  I 0.0021722 0.0000097  0.4028 0.0059  I  -119.531    0.903    -9.161    0.177  0.304825  0.411174  0.0022047  -119.329    -9.293  
+23 9 3 60190.00 I  0.304679 0.000007  0.409252 0.000015  I 0.0018679 0.0000093  0.2134 0.0065  I  -119.560    0.903    -9.360    0.177  0.304727  0.409265  0.0019255  -119.472    -9.461  
+23 9 4 60191.00 I  0.304310 0.000014  0.407148 0.000035  I 0.0017757 0.0000088 -0.0668 0.0064  I  -119.692    0.643    -9.229    0.080  0.304257  0.407156  0.0018953  -119.709    -9.301  
+23 9 5 60192.00 I  0.304218 0.000013  0.404869 0.000032  I 0.0020447 0.0000089 -0.4768 0.0058  I  -120.005    0.617    -9.043    0.063  0.304229  0.404886  0.0021594  -120.091    -9.090  
+23 9 6 60193.00 I  0.304237 0.000017  0.402264 0.000047  I 0.0026778 0.0000075 -0.7325 0.0059  I  -120.257    0.790    -9.095    0.079  0.304276  0.402304  0.0027036  -120.353    -9.124  
+23 9 7 60194.00 I  0.304271 0.000017  0.399238 0.000047  I 0.0034656 0.0000078 -0.8561 0.0055  I  -120.295    0.790    -9.329    0.079  0.304265  0.399324  0.0034693  -120.231    -9.351  
+23 9 8 60195.00 I  0.305004 0.000017  0.395838 0.000047  I 0.0043858 0.0000081 -0.9673 0.0057  I  -120.213    0.790    -9.489    0.079  0.305032  0.395644  0.0043809  -119.988    -9.520  
+23 9 9 60196.00 I  0.306216 0.000017  0.392377 0.000047  I 0.0053633 0.0000084 -0.9680 0.0061  I  -120.091    0.790    -9.475    0.079  0.306254  0.392502  0.0053793  -119.832    -9.558  
+23 910 60197.00 I  0.307411 0.000035  0.389475 0.000034  I 0.0063267 0.0000090 -0.9834 0.0063  I  -119.876    0.964    -9.399    0.097  0.307408  0.389458  0.0063492  -119.671    -9.536  
+23 911 60198.00 I  0.308557 0.000035  0.386752 0.000034  I 0.0072718 0.0000095 -0.8239 0.0073  I  -119.545    0.964    -9.359    0.097  0.308542  0.386795  0.0072245  -119.423    -9.464  
+23 912 60199.00 I  0.309278 0.000033  0.384468 0.000020  I 0.0079686 0.0000114 -0.6468 0.0069  I  -119.205    0.928    -9.279    0.096  0.309341  0.384450  0.0079652  -119.169    -9.303  
+23 913 60200.00 I  0.309653 0.000034  0.382306 0.000009  I 0.0085610 0.0000100 -0.4567 0.0077  I  -118.959    0.940    -9.037    0.153  0.309615  0.382316  0.0085199  -118.964    -9.046  
+23 914 60201.00 I  0.309655 0.000034  0.380119 0.000010  I 0.0088800 0.0000103 -0.2607 0.0070  I  -118.797    0.940    -8.680    0.153  0.309657  0.380143  0.0088938  -118.809    -8.719  
+23 915 60202.00 I  0.309683 0.000034  0.377605 0.000012  I 0.0091239 0.0000099 -0.1892 0.0076  I  -118.666    0.940    -8.415    0.153  0.309721  0.377614  0.0091238  -118.667    -8.501  
+23 916 60203.00 I  0.309786 0.000009  0.374690 0.000012  I 0.0092421 0.0000113 -0.0687 0.0067  I  -118.566    0.970    -8.397    0.225  0.309751  0.374744  0.0092593  -118.529    -8.503  
+23 917 60204.00 I  0.309662 0.000023  0.371804 0.000012  I 0.0093010 0.0000089 -0.0673 0.0070  I  -118.524    1.025    -8.577    0.161  0.309757  0.371760  0.0093601  -118.451    -8.682  
+23 918 60205.00 I  0.308974 0.000023  0.369031 0.000013  I 0.0094187 0.0000082 -0.1920 0.0058  I  -118.539    1.025    -8.789    0.161  0.308886  0.369108  0.0095049  -118.457    -8.880  
+23 919 60206.00 I  0.308186 0.000023  0.366256 0.000033  I 0.0096949 0.0000074 -0.3465 0.0055  I  -118.606    0.943    -8.939    0.094  0.308208  0.366181  0.0097240  -118.563    -9.000  
+23 920 60207.00 I  0.307454 0.000023  0.363552 0.000033  I 0.0100813 0.0000072 -0.4097 0.0052  I  -118.755    0.943    -9.053    0.094  0.307457  0.363678  0.0100660  -118.869    -9.060  
+23 921 60208.00 I  0.306783 0.000023  0.360704 0.000032  I 0.0105408 0.0000072 -0.5523 0.0052  I  -118.978    0.943    -9.171    0.094  0.306721  0.360579  0.0105661  -119.283    -9.118  
+23 922 60209.00 I  0.306362 0.000023  0.357772 0.000032  I 0.0111902 0.0000074 -0.7079 0.0050  I  -119.144    0.943    -9.268    0.094  0.306436  0.357851  0.0112184  -119.529    -9.192  
+23 923 60210.00 I  0.305728 0.000009  0.354964 0.000032  I 0.0119279 0.0000069 -0.7774 0.0059  I  -119.083    0.660    -9.291    0.037  0.305659  0.354987  0.0119856  -119.445    -9.228  
+23 924 60211.00 I  0.305041 0.000008  0.351920 0.000032  I 0.0127088 0.0000091 -0.7383 0.0070  I  -118.743    0.660    -9.233    0.037  0.305106  0.351922  0.0127431  -119.033    -9.199  
+23 925 60212.00 I  0.304195 0.000016  0.348957 0.000044  I 0.0133497 0.0000122 -0.5348 0.0075  I  -118.256    0.730    -9.080    0.139  0.304158  0.349002  0.0133969  -118.449    -9.085  
+23 926 60213.00 I  0.303380 0.000016  0.346199 0.000044  I 0.0137696 0.0000120 -0.3049 0.0085  I  -117.889    0.730    -8.782    0.139  0.303399  0.346155  0.0138149  -117.987    -8.827  
+23 927 60214.00 I  0.302813 0.000018  0.343366 0.000044  I 0.0139037 0.0000117  0.0922 0.0084  I  -117.896    0.680    -8.371    0.107  0.302795  0.343537  0.0138975  -117.925    -8.449  
+23 928 60215.00 I  0.302627 0.000018  0.340983 0.000044  I 0.0135953 0.0000117  0.4589 0.0083  I  -118.266    0.680    -8.079    0.107  0.302657  0.340917  0.0135997  -118.314    -8.163  
+23 929 60216.00 I  0.302167 0.000018  0.338707 0.000044  I 0.0130379 0.0000118  0.6697 0.0080  I  -118.639    0.680    -8.141    0.107  0.302155  0.338760  0.0130375  -118.728    -8.223  
+23 930 60217.00 I  0.301757 0.000018  0.336457 0.000044  I 0.0123128 0.0000109  0.7098 0.0077  I  -118.667    0.680    -8.473    0.107  0.301747  0.336425  0.0123503  -118.801    -8.546  
+2310 1 60218.00 I  0.301359 0.000017  0.334261 0.000038  I 0.0117054 0.0000098  0.4884 0.0071  I  -118.462    0.615    -8.713    0.082  0.301385  0.334305  0.0117122  -118.634    -8.774  
+2310 2 60219.00 I  0.300722 0.000017  0.332050 0.000038  I 0.0113550 0.0000091  0.2099 0.0065  I  -118.438    0.615    -8.662    0.082  0.300711  0.331993  0.0113503  -118.635    -8.711  
+2310 3 60220.00 I  0.299834 0.000015  0.329334 0.000038  I 0.0113049 0.0000086 -0.1264 0.0054  I  -118.732    0.571    -8.507    0.076  0.299884  0.329534  0.0113093  -118.934    -8.547  
+2310 4 60221.00 I  0.298794 0.000016  0.326874 0.000038  I 0.0115917 0.0000057 -0.4145 0.0049  I  -119.043    0.733    -8.522    0.078  0.298717  0.326782  0.0115775  -119.190    -8.569  
+2310 5 60222.00 I  0.298188 0.000016  0.324013 0.000038  I 0.0120899 0.0000048 -0.5707 0.0040  I  -119.063    0.733    -8.702    0.078  0.298232  0.324037  0.0120742  -119.132    -8.761  
+2310 6 60223.00 I  0.297920 0.000016  0.321461 0.000038  I 0.0127161 0.0000055 -0.6760 0.0045  I  -118.806    0.733    -8.815    0.078  0.297920  0.321485  0.0127240  -118.796    -8.884  
+2310 7 60224.00 I  0.297527 0.000009  0.319108 0.000009  I 0.0133921 0.0000077 -0.6320 0.0047  I  -118.440    0.906    -8.732    0.079  0.297532  0.319119  0.0133996  -118.390    -8.787  
+2310 8 60225.00 I  0.296857 0.000039  0.316795 0.000046  I 0.0139428 0.0000076 -0.4762 0.0053  I  -118.044    0.897    -8.557    0.049  0.296876  0.316797  0.0139877  -117.978    -8.588  
+2310 9 60226.00 I  0.295941 0.000039  0.314644 0.000046  I 0.0143547 0.0000074 -0.3511 0.0060  I  -117.640    0.897    -8.444    0.049  0.295928  0.314663  0.0144054  -117.574    -8.450  
+231010 60227.00 I  0.294876 0.000038  0.312138 0.000046  I 0.0146314 0.0000092 -0.1852 0.0050  I  -117.313    0.892    -8.385    0.009  0.294921  0.312271  0.0146356  -117.258    -8.374  
+231011 60228.00 I  0.293776 0.000038  0.309952 0.000046  I 0.0146880 0.0000068  0.0920 0.0057  I  -117.146    0.782    -8.248    0.076  0.293786  0.309909  0.0146710  -117.114    -8.254  
+231012 60229.00 I  0.292356 0.000038  0.307283 0.000046  I 0.0144982 0.0000067  0.2169 0.0047  I  -117.110    0.782    -7.979    0.076  0.292342  0.307369  0.0145299  -117.105    -8.014  
+231013 60230.00 I  0.291449 0.000038  0.304779 0.000046  I 0.0142799 0.0000066  0.2649 0.0044  I  -117.118    0.782    -7.707    0.076  0.291417  0.304741  0.0142940  -117.141    -7.774  
+231014 60231.00 I  0.290932 0.000007  0.302894 0.000007  I 0.0139544 0.0000057  0.3549 0.0042  I  -117.151    0.717    -7.616    0.098  0.290959  0.302931  0.0139979  -117.183    -7.692  
+231015 60232.00 I  0.290251 0.000007  0.301030 0.000005  I 0.0136232 0.0000053  0.2855 0.0039  I  -117.238    0.717    -7.750    0.098  0.290206  0.301059  0.0136690  -117.269    -7.821  
+231016 60233.00 I  0.289562 0.000012  0.298932 0.000005  I 0.0133997 0.0000054  0.1673 0.0041  I  -117.345    0.629    -7.987    0.069  0.289556  0.298935  0.0134187  -117.374    -8.045  
+231017 60234.00 I  0.288902 0.000012  0.296734 0.000005  I 0.0132940 0.0000062  0.0328 0.0044  I  -117.371    0.575    -8.164    0.039  0.288888  0.296768  0.0133241  -117.400    -8.202  
+231018 60235.00 I  0.288068 0.000020  0.294644 0.000011  I 0.0133569 0.0000069 -0.1700 0.0045  I  -117.275    0.564    -8.219    0.040  0.288061  0.294608  0.0133850  -117.311    -8.232  
+231019 60236.00 I  0.286785 0.000020  0.292872 0.000011  I 0.0136105 0.0000065 -0.3022 0.0047  I  -117.121    0.564    -8.205    0.040  0.286823  0.292913  0.0136196  -117.185    -8.186  
+231020 60237.00 I  0.285245 0.000020  0.291131 0.000011  I 0.0139200 0.0000065 -0.3105 0.0047  I  -116.955    0.564    -8.204    0.040  0.285166  0.291121  0.0139436  -117.049    -8.158  
+231021 60238.00 I  0.283853 0.000021  0.289333 0.000012  I 0.0142170 0.0000068 -0.2752 0.0046  I  -116.701    0.564    -8.244    0.040  0.283894  0.289336  0.0142475  -116.787    -8.196  
+231022 60239.00 I  0.282751 0.000021  0.287369 0.000030  I 0.0144459 0.0000066 -0.1663 0.0047  I  -116.261    0.679    -8.281    0.068  0.282734  0.287395  0.0144590  -116.313    -8.253  
+231023 60240.00 I  0.281943 0.000021  0.285004 0.000030  I 0.0145065 0.0000064  0.0719 0.0045  I  -115.700    0.679    -8.227    0.068  0.281945  0.284996  0.0144889  -115.709    -8.227  
+231024 60241.00 I  0.281299 0.000013  0.282272 0.000028  I 0.0142728 0.0000061  0.3982 0.0040  I  -115.264    0.720    -8.011    0.072  0.281319  0.282356  0.0142581  -115.235    -8.043  
+231025 60242.00 I  0.280646 0.000025  0.279941 0.000035  I 0.0137411 0.0000049  0.6317 0.0039  I  -115.186    0.701    -7.664    0.092  0.280625  0.279902  0.0137506  -115.163    -7.716  
+231026 60243.00 I  0.280193 0.000025  0.277744 0.000035  I 0.0130356 0.0000048  0.7866 0.0034  I  -115.439    0.701    -7.352    0.092  0.280203  0.277777  0.0130086  -115.441    -7.417  
+231027 60244.00 I  0.280006 0.000025  0.275624 0.000035  I 0.0122057 0.0000046  0.8283 0.0034  I  -115.724    0.701    -7.250    0.092  0.280001  0.275702  0.0121805  -115.756    -7.323  
+231028 60245.00 I  0.280050 0.000022  0.274137 0.000021  I 0.0114611 0.0000047  0.6239 0.0037  I  -115.759    0.675    -7.360    0.114  0.280015  0.274097  0.0114735  -115.828    -7.433  
+231029 60246.00 I  0.279551 0.000031  0.272817 0.000051  I 0.0110036 0.0000057  0.2824 0.0035  I  -115.592    0.648    -7.503    0.094  0.279560  0.272859  0.0110296  -115.697    -7.571  
+231030 60247.00 I  0.278182 0.000031  0.271706 0.000051  I 0.0108832 0.0000052 -0.0197 0.0047  I  -115.515    0.648    -7.541    0.094  0.278140  0.271640  0.0108288  -115.650    -7.597  
+231031 60248.00 I  0.276334 0.000022  0.270137 0.000047  I 0.0110132 0.0000074 -0.2323 0.0039  I  -115.677    0.617    -7.521    0.065  0.276348  0.270303  0.0109909  -115.831    -7.561  
+2311 1 60249.00 I  0.274628 0.000024  0.268350 0.000047  I 0.0113198 0.0000059 -0.3607 0.0048  I  -115.891    0.708    -7.569    0.046  0.274569  0.268315  0.0113342  -116.023    -7.580  
+2311 2 60250.00 I  0.273174 0.000024  0.266183 0.000047  I 0.0117328 0.0000060 -0.4836 0.0043  I  -115.877    0.708    -7.681    0.046  0.273198  0.266114  0.0117789  -115.971    -7.663  
+2311 3 60251.00 I  0.271872 0.000024  0.264311 0.000048  I 0.0122554 0.0000062 -0.5119 0.0046  I  -115.560    0.708    -7.730    0.046  0.271821  0.264434  0.0122712  -115.614    -7.690  
+2311 4 60252.00 I  0.270964 0.000011  0.262667 0.000010  I 0.0127069 0.0000070 -0.3913 0.0048  I  -115.072    0.799    -7.645    0.011  0.270924  0.262558  0.0127260  -115.116    -7.627  
+2311 5 60253.00 I  0.270121 0.000012  0.261227 0.000011  I 0.0130143 0.0000072 -0.1996 0.0051  I  -114.569    0.852    -7.504    0.136  0.270153  0.261321  0.0130385  -114.618    -7.532  
+2311 6 60254.00 I  0.269207 0.000013  0.259837 0.000011  I 0.0131086 0.0000075 -0.0154 0.0063  I  -114.143    0.852    -7.419    0.136  0.269116  0.259779  0.0131375  -114.197    -7.493  
+2311 7 60255.00 I  0.268229 0.000008  0.258500 0.000008  I 0.0130391 0.0000103  0.1866 0.0060  I  -113.863    0.904    -7.379    0.196  0.268298  0.258530  0.0130292  -113.915    -7.488  
+2311 8 60256.00 I  0.266813 0.000010  0.257169 0.000009  I 0.0127596 0.0000093  0.3159 0.0072  I  -113.777    0.871    -7.264    0.192  0.266724  0.257199  0.0127909  -113.812    -7.341  
+2311 9 60257.00 I  0.265199 0.000010  0.255657 0.000007  I 0.0124244 0.0000102  0.3940 0.0068  I  -113.869    0.871    -7.000    0.192  0.265207  0.255588  0.0124412  -113.870    -7.028  
+231110 60258.00 I  0.263474 0.000010  0.254368 0.000007  I 0.0119498 0.0000098  0.5374 0.0076  I  -114.057    0.871    -6.675    0.192  0.263493  0.254443  0.0119535  -114.009    -6.661  
+231111 60259.00 I  0.261652 0.000009  0.252860 0.000006  I 0.0113957 0.0000112  0.5423 0.0069  I  -114.265    0.714    -6.469    0.177  0.261629  0.252836  0.0114045  -114.126    -6.454  
+231112 60260.00 I  0.259928 0.000013  0.251255 0.000013  I 0.0109198 0.0000097  0.3834 0.0073  I  -114.453    0.968    -6.491    0.089  0.259927  0.251292  0.0108944  -114.234    -6.490  
+231113 60261.00 I  0.258273 0.000013  0.249722 0.000013  I 0.0106125 0.0000095  0.2738 0.0076  I  -114.576    0.968    -6.690    0.089  0.258249  0.249725  0.0105445  -114.369    -6.684  
+231114 60262.00 I  0.256518 0.000010  0.248084 0.000012  I 0.0103990 0.0000116  0.0837 0.0066  I  -114.575    1.060    -6.913    0.025  0.256507  0.248149  0.0103854  -114.441    -6.893  
+231115 60263.00 I  0.254570 0.000018  0.246752 0.000013  I 0.0104575 0.0000091 -0.1438 0.0072  I  -114.421    0.918    -7.036    0.072  0.254570  0.246747  0.0104172  -114.353    -7.028  
+231116 60264.00 I  0.252448 0.000018  0.245071 0.000013  I 0.0106298 0.0000086 -0.2009 0.0062  I  -114.158    0.918    -7.043    0.072  0.252424  0.245071  0.0105996  -114.146    -7.065  
+231117 60265.00 I  0.250353 0.000018  0.242920 0.000013  I 0.0108549 0.0000085 -0.2448 0.0060  I  -113.848    0.918    -7.005    0.072  0.250380  0.242975  0.0108565  -113.885    -7.060  
+231118 60266.00 I  0.248435 0.000015  0.240400 0.000020  I 0.0111057 0.0000084 -0.2477 0.0055  I  -113.500    0.851    -6.994    0.093  0.248406  0.240354  0.0111168  -113.566    -7.059  
+231119 60267.00 I  0.246657 0.000017  0.238102 0.000006  I 0.0113003 0.0000071 -0.1005 0.0055  I  -113.093    0.844    -7.016    0.101  0.246682  0.238139  0.0113046  -113.174    -7.077  
+231120 60268.00 I  0.245306 0.000017  0.236094 0.000007  I 0.0112864 0.0000070  0.1075 0.0048  I  -112.673    0.844    -7.009    0.101  0.245271  0.236097  0.0113015  -112.760    -7.062  
+231121 60269.00 I  0.244552 0.000008  0.234484 0.000005  I 0.0110970 0.0000066  0.2802 0.0048  I  -112.373    0.835    -6.904    0.108  0.244498  0.234480  0.0111044  -112.462    -6.950  
+231122 60270.00 I  0.243514 0.000010  0.233448 0.000010  I 0.0107417 0.0000065  0.4058 0.0046  I  -112.322    0.866    -6.692    0.134  0.243598  0.233507  0.0107595  -112.403    -6.748  
+231123 60271.00 I  0.242037 0.000010  0.232220 0.000010  I 0.0103234 0.0000063  0.4175 0.0047  I  -112.510    0.866    -6.440    0.134  0.241883  0.232192  0.0103424  -112.588    -6.509  
+231124 60272.00 I  0.240934 0.000010  0.231295 0.000011  I 0.0099103 0.0000068  0.4185 0.0060  I  -112.777    0.866    -6.239    0.134  0.240989  0.231266  0.0099187  -112.864    -6.316  
+231125 60273.00 I  0.239750 0.000008  0.230767 0.000011  I 0.0095247 0.0000102  0.3046 0.0057  I  -112.932    1.000    -6.137    0.207  0.239692  0.230833  0.0095577  -113.106    -6.196  
+231126 60274.00 I  0.238315 0.000008  0.230131 0.000015  I 0.0093607 0.0000091  0.0117 0.0067  I  -112.910    0.800    -6.129    0.143  0.238294  0.230077  0.0094031  -113.204    -6.155  
+231127 60275.00 I  0.236336 0.000008  0.229439 0.000015  I 0.0094872 0.0000088 -0.2390 0.0070  I  -112.806    0.800    -6.193    0.143  0.236360  0.229500  0.0094752  -113.202    -6.183  
+231128 60276.00 I  0.233892 0.000005  0.228492 0.000013  I 0.0098250 0.0000107 -0.4485 0.0062  I  -112.749    0.553    -6.314    0.034  0.233806  0.228473  0.0098338  -113.200    -6.274  
+231129 60277.00 I  0.231441 0.000010  0.227259 0.000014  I 0.0103680 0.0000087 -0.6094 0.0069  I  -112.749    1.019    -6.463    0.025  0.231481  0.227298  0.0103599  -113.080    -6.419  
+231130 60278.00 I  0.229067 0.000010  0.225875 0.000013  I 0.0109942 0.0000087 -0.6213 0.0060  I  -112.687    1.019    -6.568    0.025  0.228990  0.225880  0.0110065  -112.835    -6.533  
+2312 1 60279.00 I  0.226755 0.000010  0.224791 0.000013  I 0.0115682 0.0000084 -0.5058 0.0064  I  -112.453    1.019    -6.565    0.025  0.226816  0.224745  0.0115719  -112.416    -6.544  
+2312 2 60280.00 I  0.224384 0.000009  0.223868 0.000007  I 0.0119997 0.0000095 -0.3720 0.0058  I  -112.060    1.091    -6.466    0.022  0.224305  0.223935  0.0120098  -112.137    -6.481  
+2312 3 60281.00 I  0.222057 0.000010  0.222485 0.000011  I 0.0123010 0.0000081 -0.2048 0.0062  I  -111.631    1.074    -6.357    0.060  0.222071  0.222430  0.0123212  -111.909    -6.410  
+2312 4 60282.00 I  0.219838 0.000010  0.220816 0.000011  I 0.0124187 0.0000080 -0.0660 0.0058  I  -111.288    1.074    -6.294    0.060  0.219794  0.220875  0.0124645  -111.526    -6.362  
+2312 5 60283.00 I  0.217384 0.000005  0.219174 0.000010  I 0.0124352 0.0000084  0.0662 0.0052  I  -111.093    1.060    -6.234    0.077  0.217420  0.219115  0.0124535  -111.142    -6.298  
+2312 6 60284.00 I  0.214673 0.000026  0.217467 0.000037  I 0.0122756 0.0000068  0.2306 0.0053  I  -111.078    0.988    -6.085    0.070  0.214571  0.217536  0.0122758  -111.087    -6.142  
+2312 7 60285.00 I  0.211879 0.000026  0.215829 0.000037  I 0.0119980 0.0000066  0.3229 0.0047  I  -111.271    0.988    -5.830    0.070  0.211936  0.215746  0.0119773  -111.334    -5.879  
+2312 8 60286.00 I  0.208848 0.000026  0.213944 0.000037  I 0.0116591 0.0000065  0.3271 0.0047  I  -111.651    0.988    -5.570    0.070  0.208772  0.214113  0.0116481  -111.833    -5.608  
+2312 9 60287.00 I  0.205707 0.000026  0.212134 0.000036  I 0.0113841 0.0000068  0.2103 0.0044  I  -112.103    0.827    -5.437    0.049  0.205670  0.212065  0.0113851  -112.299    -5.455  
+231210 60288.00 I  0.202975 0.000027  0.210484 0.000037  I 0.0112452 0.0000060  0.0733 0.0046  I  -112.459    0.856    -5.492    0.057  0.203013  0.210473  0.0112396  -112.615    -5.487  
+231211 60289.00 I  0.200028 0.000027  0.209353 0.000037  I 0.0112395 0.0000063 -0.0696 0.0051  I  -112.627    0.856    -5.694    0.057  0.199952  0.209451  0.0112226  -112.730    -5.675  
+231212 60290.00 I  0.196871 0.000008  0.208329 0.000007  I 0.0113856 0.0000083 -0.2160 0.0044  I  -112.630    0.890    -5.954    0.063  0.196871  0.208244  0.0113677  -112.676    -5.935  
+231213 60291.00 I  0.193386 0.000026  0.207670 0.000012  I 0.0116610 0.0000061 -0.3309 0.0052  I  -112.513    0.945    -6.175    0.146  0.193357  0.207726  0.0116597  -112.524    -6.202  
+231214 60292.00 I  0.189615 0.000026  0.206796 0.000012  I 0.0120392 0.0000062 -0.4212 0.0046  I  -112.284    0.945    -6.276    0.146  0.189583  0.206787  0.0120425  -112.273    -6.363  
+231215 60293.00 I  0.185893 0.000026  0.205764 0.000012  I 0.0124533 0.0000070 -0.3613 0.0049  I  -111.956    0.945    -6.225    0.146  0.185845  0.205745  0.0124339  -111.930    -6.367  
+231216 60294.00 I  0.181989 0.000025  0.204684 0.000011  I 0.0126949 0.0000075 -0.1009 0.0048  I  -111.609    1.008    -6.084    0.197  0.181994  0.204722  0.0126576  -111.598    -6.234  
+231217 60295.00 I  0.178173 0.000052  0.203437 0.000034  I 0.0126386 0.0000066  0.2090 0.0051  I  -111.354    0.869    -5.965    0.136  0.178144  0.203403  0.0126038  -111.370    -6.091  
+231218 60296.00 I  0.174431 0.000052  0.202319 0.000034  I 0.0122995 0.0000069  0.4512 0.0047  I  -111.244    0.869    -5.924    0.136  0.174426  0.202336  0.0122851  -111.282    -6.014  
+231219 60297.00 I  0.170620 0.000046  0.201130 0.000033  I 0.0117396 0.0000067  0.6831 0.0048  I  -111.265    0.848    -5.917    0.090  0.170661  0.201214  0.0117121  -111.310    -5.968  
+231220 60298.00 I  0.167503 0.000046  0.200670 0.000033  I 0.0109643 0.0000067  0.8220 0.0050  I  -111.381    0.848    -5.867    0.090  0.167464  0.200619  0.0109464  -111.392    -5.892  
+231221 60299.00 I  0.164923 0.000046  0.200401 0.000033  I 0.0101424 0.0000074  0.8204 0.0052  I  -111.567    0.848    -5.746    0.090  0.164895  0.200433  0.0101277  -111.528    -5.749  
+231222 60300.00 I  0.162552 0.000046  0.200454 0.000033  I 0.0093549 0.0000080  0.7244 0.0063  I  -111.794    0.848    -5.582    0.090  0.162559  0.200456  0.0093539  -111.691    -5.567  
+231223 60301.00 I  0.160086 0.000010  0.200805 0.000008  I 0.0087336 0.0000101  0.5084 0.0064  I  -111.984    0.907    -5.432    0.059  0.160059  0.200780  0.0087321  -111.813    -5.402  
+231224 60302.00 I  0.157628 0.000010  0.201250 0.000008  I 0.0083684 0.0000101  0.2016 0.0120  I  -112.021    0.907    -5.362    0.059  0.157580  0.201308  0.0083399  -111.797    -5.323  
+231225 60303.00 I  0.155027 0.000020  0.201550 0.000020  I 0.0083214 0.0000218 -0.0782 0.0092  I  -111.856    0.322    -5.427    0.160  0.155062  0.201492  0.0081989  -111.605    -5.389  
+231226 60304.00 I  0.151982 0.000032  0.201768 0.000020  I 0.0084447 0.0000153 -0.1178 0.0122  I  -111.583    0.767    -5.632    0.134  0.151948  0.201842  0.0082629  -111.345    -5.604  
+231227 60305.00 I  0.148901 0.000033  0.201589 0.000008  I 0.0085308 0.0000111 -0.0787 0.0091  I  -111.371    0.627    -5.887    0.186  0.148900  0.201561  0.0084167  -111.199    -5.883  
+231228 60306.00 I  0.146037 0.000033  0.201377 0.000008  I 0.0086448 0.0000100 -0.1676 0.0072  I  -111.273    0.627    -6.049    0.186  0.146049  0.201377  0.0086182  -111.234    -6.083  
+231229 60307.00 I  0.143446 0.000033  0.201315 0.000008  I 0.0088481 0.0000092 -0.2027 0.0068  I  -111.186    0.627    -6.035    0.186  0.143421  0.201375  0.0088430  -111.373    -6.128  
+231230 60308.00 I  0.141083 0.000033  0.201555 0.000008  I 0.0089894 0.0000093 -0.0552 0.0064  I  -110.990    0.627    -5.894    0.186  0.141056  0.201504  0.0089829  -111.268    -6.021  
+231231 60309.00 I  0.138972 0.000032  0.201878 0.000008  I 0.0089482 0.0000089  0.1233 0.0055  I  -110.700    0.627    -5.752    0.186  0.138979  0.201930  0.0089356  -110.895    -5.878  
+24 1 1 60310.00 I  0.136911 0.000012  0.202189 0.000010  I 0.0087625 0.0000057  0.2426 0.0053  I  -110.420    0.815    -5.669    0.155  0.136894  0.202185  0.0087572  -110.452    -5.772  
+24 1 2 60311.00 I  0.134905 0.000009  0.202522 0.000007  I 0.0084758 0.0000059  0.3236 0.0040  I  -110.225    1.001    -5.586    0.074  0.134917  0.202555  0.0084757  -110.087    -5.652  
+24 1 3 60312.00 I  0.133126 0.000012  0.203114 0.000009  I 0.0081213 0.0000055  0.3867 0.0044  I  -110.157    0.863    -5.435    0.053  0.133109  0.203087  0.0081157  -109.914    -5.458  
+24 1 4 60313.00 I  0.131591 0.000013  0.203992 0.000009  I 0.0077041 0.0000066  0.4448 0.0047  I  -110.292    0.863    -5.259    0.053  0.131582  0.204005  0.0077008  -110.198    -5.245  
+24 1 5 60314.00 I  0.130041 0.000013  0.205136 0.000009  I 0.0072716 0.0000075  0.3831 0.0052  I  -110.688    0.863    -5.195    0.053  0.130046  0.205151  0.0072587  -110.796    -5.152  
+24 1 6 60315.00 I  0.127943 0.000013  0.206077 0.000010  I 0.0069620 0.0000080  0.2489 0.0063  I  -111.228    0.863    -5.310    0.053  0.127924  0.206114  0.0068909  -111.426    -5.273  
+24 1 7 60316.00 I  0.125603 0.000028  0.206386 0.000010  I 0.0067770 0.0000100  0.1049 0.0063  I  -111.657    0.690    -5.524    0.122  0.125599  0.206334  0.0066966  -111.850    -5.519  
+24 1 8 60317.00 I  0.123304 0.000028  0.206616 0.000010  I 0.0067867 0.0000097 -0.1426 0.0075  I  -111.848    0.690    -5.716    0.122  0.123296  0.206642  0.0067475  -111.991    -5.753  
+24 1 9 60318.00 I  0.121232 0.000027  0.206576 0.000008  I 0.0070484 0.0000113 -0.3487 0.0071  I  -111.917    0.690    -5.880    0.151  0.121192  0.206575  0.0070360  -111.988    -5.961  
+24 110 60319.00 I  0.119299 0.000031  0.206278 0.000037  I 0.0074356 0.0000104 -0.4095 0.0074  I  -111.962    0.690    -6.078    0.152  0.119280  0.206262  0.0074355  -112.002    -6.175  
+24 111 60320.00 I  0.117581 0.000031  0.206444 0.000037  I 0.0078418 0.0000097 -0.3937 0.0071  I  -111.875    0.690    -6.253    0.152  0.117602  0.206432  0.0078271  -111.898    -6.355  
+24 112 60321.00 I  0.115888 0.000031  0.206583 0.000037  I 0.0081784 0.0000096 -0.2441 0.0063  I  -111.543    0.690    -6.241    0.152  0.115879  0.206702  0.0081417  -111.556    -6.342  
+24 113 60322.00 I  0.114322 0.000017  0.207056 0.000036  I 0.0082924 0.0000081  0.0183 0.0055  I  -111.130    0.678    -6.001    0.160  0.114245  0.207034  0.0082712  -111.146    -6.094  
+24 114 60323.00 I  0.113343 0.000026  0.207803 0.000037  I 0.0081403 0.0000054  0.2851 0.0050  I  -110.933    0.578    -5.728    0.084  0.113378  0.207784  0.0081341  -110.961    -5.809  
+24 115 60324.00 I  0.112244 0.000026  0.208935 0.000037  I 0.0077484 0.0000057  0.4734 0.0043  I  -111.043    0.578    -5.634    0.084  0.112214  0.209001  0.0077530  -111.087    -5.702  
+24 116 60325.00 I  0.111007 0.000021  0.209775 0.000007  I 0.0072101 0.0000067  0.6121 0.0041  I  -111.305    0.569    -5.705    0.073  0.110998  0.209753  0.0072002  -111.363    -5.761  
+24 117 60326.00 I  0.109669 0.000031  0.210731 0.000038  I 0.0065683 0.0000060  0.6186 0.0052  I  -111.549    0.666    -5.775    0.059  0.109707  0.210704  0.0065513  -111.598    -5.826  
+24 118 60327.00 I  0.107701 0.000031  0.211863 0.000038  I 0.0060260 0.0000080  0.4659 0.0055  I  -111.735    0.666    -5.751    0.059  0.107654  0.211907  0.0059931  -111.772    -5.800  
+24 119 60328.00 I  0.105479 0.000031  0.212762 0.000038  I 0.0056641 0.0000093  0.2304 0.0068  I  -111.888    0.666    -5.678    0.059  0.105447  0.212778  0.0056646  -111.917    -5.725  
+24 120 60329.00 I  0.102653 0.000024  0.213958 0.000039  I 0.0055611 0.0000110  0.0073 0.0068  I  -111.990    0.706    -5.625    0.047  0.102668  0.213985  0.0055761  -112.052    -5.663  
+24 121 60330.00 I  0.099227 0.000034  0.214511 0.000040  I 0.0056538 0.0000099 -0.2286 0.0074  I  -111.956    0.707    -5.622    0.040  0.099188  0.214508  0.0056875  -112.070    -5.647  
+24 122 60331.00 I  0.095646 0.000034  0.214904 0.000040  I 0.0059644 0.0000099 -0.3028 0.0088  I  -111.707    0.707    -5.698    0.040  0.095614  0.214880  0.0059347  -111.865    -5.711  
+24 123 60332.00 I  0.092164 0.000024  0.215190 0.000014  I 0.0062340 0.0000145 -0.3009 0.0068  I  -111.289    0.709    -5.887    0.028  0.092142  0.215252  0.0062476  -111.472    -5.891  
+24 124 60333.00 I  0.088472 0.000035  0.215339 0.000017  I 0.0065570 0.0000093 -0.2715 0.0082  I  -110.892    0.914    -6.145    0.084  0.088475  0.215315  0.0065434  -111.012    -6.155  
+24 125 60334.00 I  0.085035 0.000035  0.215397 0.000016  I 0.0067471 0.0000077 -0.1523 0.0059  I  -110.673    0.914    -6.332    0.084  0.085015  0.215422  0.0067558  -110.704    -6.354  
+24 126 60335.00 I  0.082057 0.000035  0.215778 0.000014  I 0.0068565 0.0000074 -0.0176 0.0057  I  -110.602    0.914    -6.316    0.084  0.082036  0.215766  0.0068335  -110.548    -6.353  
+24 127 60336.00 I  0.079096 0.000026  0.216502 0.000011  I 0.0067730 0.0000085  0.1451 0.0056  I  -110.526    1.027    -6.122    0.114  0.079128  0.216515  0.0067647  -110.477    -6.174  
+24 128 60337.00 I  0.076254 0.000030  0.217099 0.000012  I 0.0065327 0.0000084  0.4087 0.0060  I  -110.359    0.969    -5.909    0.139  0.076203  0.217108  0.0065455  -110.366    -5.976  
+24 129 60338.00 I  0.073644 0.000030  0.217518 0.000011  I 0.0060052 0.0000086  0.5236 0.0079  I  -110.147    0.969    -5.802    0.139  0.073683  0.217508  0.0060957  -110.224    -5.878  
+24 130 60339.00 I  0.070970 0.000015  0.217913 0.000006  I 0.0055113 0.0000133  0.5611 0.0070  I  -109.970    0.786    -5.771    0.171  0.070956  0.217931  0.0055078  -110.114    -5.849  
+24 131 60340.00 I  0.068314 0.000035  0.218407 0.000013  I 0.0048657 0.0000110  0.6506 0.0087  I  -109.880    0.853    -5.735    0.178  0.068290  0.218391  0.0048845  -110.040    -5.788  
+24 2 1 60341.00 I  0.065615 0.000035  0.219270 0.000013  I 0.0042692 0.0000112  0.5629 0.0074  I  -109.952    0.853    -5.729    0.178  0.065607  0.219297  0.0042881  -110.106    -5.750  
+24 2 2 60342.00 I  0.062919 0.000035  0.220835 0.000013  I 0.0037404 0.0000099  0.4736 0.0075  I  -110.252    0.853    -5.890    0.178                                                     
+24 2 3 60343.00 I  0.060166 0.000031  0.222593 0.000012  I 0.0033494 0.0000101  0.3022 0.0063  I  -110.675    0.987    -6.252    0.197                                                     
+24 2 4 60344.00 I  0.057725 0.000042  0.224295 0.000026  I 0.0031592 0.0000077  0.0611 0.0065  I  -110.961    0.975    -6.623    0.171                                                     
+24 2 5 60345.00 I  0.055778 0.000042  0.226041 0.000026  I 0.0032006 0.0000082 -0.1002 0.0062  I  -111.017    0.975    -6.781    0.171                                                     
+24 2 6 60346.00 I  0.053749 0.000028  0.227776 0.000023  I 0.0033276 0.0000098 -0.1655 0.0053  I  -111.074    0.973    -6.767    0.165                                                     
+24 2 7 60347.00 I  0.052413 0.000029  0.229333 0.000027  I 0.0035072 0.0000067 -0.1578 0.0059  I  -111.301    1.011    -6.838    0.164                                                     
+24 2 8 60348.00 I  0.051232 0.000029  0.231102 0.000027  I 0.0036015 0.0000065 -0.0251 0.0046  I  -111.440    1.011    -7.076    0.164                                                     
+24 2 9 60349.00 I  0.049742 0.000029  0.233129 0.000027  I 0.0035262 0.0000064  0.2013 0.0048  I  -111.142    1.011    -7.222    0.164                                                     
+24 210 60350.00 I  0.048227 0.000010  0.235224 0.000015  I 0.0031547 0.0000072  0.5604 0.0044  I  -110.552    1.067    -7.039    0.163                                                     
+24 211 60351.00 I  0.047102 0.000012  0.237167 0.000017  I 0.0024081 0.0000061  0.9113 0.0046  I  -110.182    0.912    -6.685    0.165                                                     
+24 212 60352.00 I  0.046122 0.000012  0.238842 0.000017  I 0.0013833 0.0000057  1.1085 0.0047  I  -110.280    0.912    -6.510    0.165                                                     
+24 213 60353.00 I  0.044584 0.000008  0.240612 0.000011  I 0.0002500 0.0000071  1.1288 0.0046  I  -110.639    0.736    -6.597    0.166                                                     
+24 214 60354.00 I  0.042513 0.000009  0.242111 0.000026  I-0.0008322 0.0000071  1.0226 0.0050  I  -110.999    0.730    -6.733    0.138                                                     
+24 215 60355.00 I  0.040479 0.000009  0.243075 0.000025  I-0.0017534 0.0000069  0.7910 0.0049  I  -111.297    0.730    -6.786    0.138                                                     
+24 216 60356.00 I  0.038718 0.000009  0.244123 0.000025  I-0.0024075 0.0000068  0.5392 0.0057  I  -111.525    0.730    -6.850    0.138                                                     
+24 217 60357.00 I  0.036981 0.000006  0.245112 0.000024  I-0.0028197 0.0000090  0.2509 0.0050  I  -111.627    0.720    -7.021    0.044                                                     
+24 218 60358.00 I  0.034981 0.000029  0.246720 0.000034  I-0.0029098 0.0000073 -0.0361 0.0058  I  -111.570    0.700    -7.233    0.084                                                     
+24 219 60359.00 I  0.032902 0.000029  0.248184 0.000034  I-0.0027838 0.0000072 -0.2142 0.0043  I  -111.367    0.700    -7.384    0.084                                                     
+24 220 60360.00 I  0.030840 0.000029  0.249858 0.000024  I-0.0025158 0.0000044 -0.2891 0.0044  I  -111.050    0.693    -7.487    0.097                                                     
+24 221 60361.00 I  0.028795 0.000036  0.251461 0.000025  I-0.0022339 0.0000049 -0.2791 0.0035  I  -110.696    0.783    -7.602    0.105                                                     
+24 222 60362.00 I  0.026418 0.000036  0.253252 0.000025  I-0.0019652 0.0000055 -0.2464 0.0038  I  -110.429    0.783    -7.687    0.105                                                     
+24 223 60363.00 I  0.024106 0.000036  0.255324 0.000025  I-0.0017714 0.0000057 -0.1227 0.0046  I  -110.308    0.783    -7.610    0.105                                                     
+24 224 60364.00 I  0.021482 0.000022  0.257663 0.000007  I-0.0017348 0.0000074  0.0459 0.0046  I  -110.261    1.124    -7.341    0.120                                                     
+24 225 60365.00 I  0.018842 0.000026  0.259563 0.000022  I-0.0018617 0.0000072  0.2100 0.0052  I  -110.176    0.764    -7.038    0.196                                                     
+24 226 60366.00 I  0.016285 0.000026  0.261550 0.000022  I-0.0021319 0.0000073  0.3054 0.0053  I  -110.033    0.764    -6.893    0.196                                                     
+24 227 60367.00 I  0.013550 0.000015  0.263683 0.000021  I-0.0024598 0.0000077  0.3626 0.0050  I  -109.893    0.574    -6.938    0.227                                                     
+24 228 60368.00 I  0.010702 0.000034  0.265660 0.000036  I-0.0028389 0.0000068  0.3652 0.0052  I  -109.817    0.639    -7.065    0.192                                                     
+24 229 60369.00 I  0.007865 0.000034  0.267828 0.000036  I-0.0031534 0.0000069  0.2574 0.0048  I  -109.842    0.639    -7.223    0.192                                                     
+24 3 1 60370.00 I  0.005660 0.000034  0.269789 0.000036  I-0.0033589 0.0000069  0.1652 0.0048  I  -109.976    0.639    -7.486    0.192                                                     
+24 3 2 60371.00 I  0.004414 0.000031  0.272392 0.000030  I-0.0034879 0.0000068  0.0852 0.0049  I  -110.136    0.723    -7.893    0.141                                                     
+24 3 3 60372.00 I  0.003477 0.000034  0.275390 0.000030  I-0.0035060 0.0000070 -0.0649 0.0049  I  -110.140    0.775    -8.284    0.212                                                     
+24 3 4 60373.00 I  0.002173 0.000034  0.278172 0.000030  I-0.0033359 0.0000071 -0.2817 0.0053  I  -109.944    0.775    -8.425    0.212                                                     
+24 3 5 60374.00 I  0.000711 0.000015  0.280475 0.000006  I-0.0029814 0.0000080 -0.3822 0.0049  I  -109.813    0.835    -8.333    0.271                                                     
+24 3 6 60375.00 I -0.000735 0.000019  0.282421 0.000009  I-0.0026506 0.0000068 -0.2455 0.0053  I  -109.994    0.769    -8.309    0.246                                                     
+24 3 7 60376.00 I -0.001817 0.000019  0.284155 0.000009  I-0.0025228 0.0000069 -0.0115 0.0047  I  -110.262    0.769    -8.550    0.246                                                     
+24 3 8 60377.00 I -0.002724 0.000021  0.286089 0.000009  I-0.0026689 0.0000065  0.3463 0.0046  I  -110.141    0.769    -8.824    0.246                                                     
+24 3 9 60378.00 I -0.003626 0.000014  0.288368 0.000009  I-0.0032352 0.0000062  0.7635 0.0042  P  -109.665    0.278    -8.755    0.145                                                     
+24 310 60379.00 I -0.004657 0.000015  0.290857 0.000013  I-0.0041686 0.0000054  1.0989 0.0041  P  -109.332    0.288    -8.362    0.148                                                     
+24 311 60380.00 I -0.005980 0.000017  0.293388 0.000015  I-0.0053810 0.0000053  1.2784 0.0042  P  -109.498    0.297    -8.032    0.151                                                     
+24 312 60381.00 I -0.007156 0.000007  0.295684 0.000012  I-0.0066419 0.0000064  1.2074 0.0042  P  -110.003    0.304    -7.988    0.154                                                     
+24 313 60382.00 I -0.007950 0.000010  0.297891 0.000015  I-0.0077452 0.0000066  0.9846 0.0053  P  -110.533    0.309    -8.090    0.155                                                     
+24 314 60383.00 I -0.008484 0.000014  0.299997 0.000015  I-0.0085788 0.0000085  0.6648 0.0057  P  -110.953    0.313    -8.189    0.157                                                     
+24 315 60384.00 I -0.009107 0.000091  0.302243 0.000090  I-0.0090684 0.0000094  0.3260 0.0080  P  -111.193    0.316    -8.369    0.158                                                     
+24 316 60385.00 I -0.010137 0.000091  0.304786 0.000090  I-0.0092616 0.0000135  0.0798 0.0081  P  -111.165    0.318    -8.726    0.158                                                     
+24 317 60386.00 I -0.011336 0.000090  0.307132 0.000091  I-0.0092550 0.0000131 -0.0855 0.0096  P  -110.912    0.319    -9.119    0.159                                                     
+24 318 60387.00 I -0.012345 0.000091  0.309252 0.000091  I-0.0091400 0.0000136 -0.1026 0.0098  P  -110.616    0.320    -9.316    0.159                                                     
+24 319 60388.00 I -0.013089 0.000091  0.311328 0.000091  I-0.0090922 0.0000146  0.0076 0.0106  P  -110.361    0.321    -9.281    0.160                                                     
+24 320 60389.00 I -0.013354 0.000091  0.313096 0.000091  I-0.0091658 0.0000163  0.1495 0.0109  P  -110.092    0.321    -9.166    0.160                                                     
+24 321 60390.00 I -0.012864 0.000091  0.314734 0.000091  I-0.0093927 0.0000161  0.2960 0.0099  P  -109.797    0.321    -9.065    0.160                                                     
+24 322 60391.00 I -0.012034 0.000091  0.316464 0.000091  I-0.0097565 0.0000114  0.4386 0.0099  P  -109.574    0.321    -8.904    0.160                                                     
+24 323 60392.00 I -0.011308 0.000091  0.318724 0.000091  I-0.0102724 0.0000115  0.5885 0.0080  P  -109.485    0.322    -8.606    0.160                                                     
+24 324 60393.00 I -0.010831 0.000091  0.321718 0.000092  I-0.0109142 0.0000111  0.6804 0.0070  P  -109.464    0.322    -8.269    0.160                                                     
+24 325 60394.00 I -0.010719 0.000091  0.324745 0.000091  I-0.0116407 0.0000079  0.7950 0.0065  P  -109.429    0.322    -8.108    0.160                                                     
+24 326 60395.00 I -0.010996 0.000091  0.327463 0.000091  I-0.0124767 0.0000066  0.8273 0.0045  P  -109.385    0.322    -8.219    0.160                                                     
+24 327 60396.00 I -0.011486 0.000090  0.330132 0.000091  I-0.0132121 0.0000041  0.6102 0.0042  P  -109.382    0.322    -8.495    0.160                                                     
+24 328 60397.00 I -0.012189 0.000090  0.332952 0.000090  I-0.0137639 0.0000051                 P  -109.425    0.322    -8.777    0.160                                                     
+24 329 60398.00 P -0.012639 0.000628  0.335467 0.000449  P-0.0142069 0.0001080                 P  -109.465    0.322    -9.025    0.160                                                     
+24 330 60399.00 P -0.013059 0.000932  0.338046 0.000739  P-0.0144323 0.0002041                 P  -109.445    0.322    -9.283    0.160                                                     
+24 331 60400.00 P -0.013262 0.001174  0.340532 0.000990  P-0.0144308 0.0003028                 P  -109.311    0.322    -9.527    0.160                                                     
+24 4 1 60401.00 P -0.013263 0.001383  0.342981 0.001218  P-0.0142351 0.0004021                 P  -109.054    0.322    -9.650    0.160                                                     
+24 4 2 60402.00 P -0.013073 0.001571  0.345443 0.001430  P-0.0139170 0.0005017                 P  -108.800    0.322    -9.632    0.160                                                     
+24 4 3 60403.00 P -0.012753 0.001743  0.347922 0.001630  P-0.0136039 0.0006014                 P  -108.720    0.322    -9.636    0.160                                                     
+24 4 4 60404.00 P -0.012342 0.001903  0.350417 0.001822  P-0.0134621 0.0007012                 P  -108.784    0.322    -9.798    0.160                                                     
+24 4 5 60405.00 P -0.011869 0.002053  0.352934 0.002006  P-0.0136267 0.0007500                 P  -108.760    0.322    -9.984    0.160                                                     
+24 4 6 60406.00 P -0.011352 0.002196  0.355466 0.002183  P-0.0141432 0.0005500                 P  -108.578    0.322    -9.910    0.160                                                     
+24 4 7 60407.00 P -0.010801 0.002332  0.357999 0.002355  P-0.0149912 0.0007548                 P  -108.487    0.322    -9.536    0.160                                                     
+24 4 8 60408.00 P -0.010216 0.002462  0.360521 0.002522  P-0.0160648 0.0009344                 P  -108.716    0.322    -9.152    0.160                                                     
+24 4 9 60409.00 P -0.009597 0.002587  0.363026 0.002685  P-0.0171624 0.0010994                 P  -109.187    0.322    -9.009    0.160                                                     
+24 410 60410.00 P -0.008940 0.002708  0.365509 0.002845  P-0.0180723 0.0012543                 P  -109.677    0.322    -9.070    0.160                                                     
+24 411 60411.00 P -0.008240 0.002824  0.367971 0.003001  P-0.0186951 0.0014016                 P  -110.042    0.322    -9.211    0.160                                                     
+24 412 60412.00 P -0.007496 0.002938  0.370412 0.003153  P-0.0189999 0.0015429                 P  -110.164    0.322    -9.462    0.160                                                     
+24 413 60413.00 P -0.006706 0.003048  0.372834 0.003303  P-0.0190619 0.0016792                 P  -109.944    0.322    -9.874    0.160                                                     
+24 414 60414.00 P -0.005870 0.003155  0.375239 0.003451  P-0.0189890 0.0018113                 P  -109.483    0.322   -10.293    0.160                                                     
+24 415 60415.00 P -0.004991 0.003259  0.377630 0.003596  P-0.0188771 0.0019399                 P  -109.071    0.322   -10.469    0.160                                                     
+24 416 60416.00 P -0.004069 0.003362  0.380005 0.003739  P-0.0188181 0.0020652                 P  -108.865    0.322   -10.341    0.160                                                     
+24 417 60417.00 P -0.003106 0.003461  0.382366 0.003879  P-0.0188764 0.0021877                 P  -108.742    0.322   -10.087    0.160                                                     
+24 418 60418.00 P -0.002103 0.003559  0.384711 0.004018  P-0.0190842 0.0023077                 P  -108.554    0.322    -9.883    0.160                                                     
+24 419 60419.00 P -0.001062 0.003654  0.387041 0.004155  P-0.0194412 0.0024255                 P  -108.360    0.322    -9.716    0.160                                                     
+24 420 60420.00 P  0.000018 0.003748  0.389353 0.004290  P-0.0199221 0.0025411                 P  -108.309    0.322    -9.481    0.160                                                     
+24 421 60421.00 P  0.001135 0.003840  0.391648 0.004423  P-0.0204829 0.0026548                 P  -108.414    0.322    -9.199    0.160                                                     
+24 422 60422.00 P  0.002290 0.003931  0.393923 0.004555  P-0.0210727 0.0027668                 P  -108.566    0.322    -9.049    0.160                                                     
+24 423 60423.00 P  0.003482 0.004020  0.396180 0.004686  P-0.0216202 0.0028772                 P  -108.692    0.322    -9.173    0.160                                                     
+24 424 60424.00 P  0.004711 0.004107  0.398416 0.004815  P-0.0220491 0.0029860                 P  -108.804    0.322    -9.511    0.160                                                     
+24 425 60425.00 P  0.005977 0.004193  0.400632 0.004943  P-0.0223026 0.0030934                 P  -108.898    0.322    -9.863    0.160                                                     
+24 426 60426.00 P  0.007279 0.004278  0.402828 0.005069  P-0.0223497 0.0031995                 P  -108.920    0.322   -10.084    0.160                                                     
+24 427 60427.00 P  0.008618 0.004361  0.405002 0.005194  P-0.0221964 0.0033043                 P  -108.843    0.322   -10.184    0.160                                                     
+24 428 60428.00 P  0.009992 0.004443  0.407154 0.005318  P-0.0218966 0.0034080                 P  -108.710    0.322   -10.245    0.160                                                     
+24 429 60429.00 P  0.011401 0.004525  0.409284 0.005441  P-0.0215402 0.0035105                 P  -108.555    0.322   -10.318    0.160                                                     
+24 430 60430.00 P  0.012845 0.004605  0.411391 0.005563  P-0.0212422 0.0036120                 P  -108.357    0.322   -10.399    0.160                                                     
+24 5 1 60431.00 P  0.014323 0.004684  0.413475 0.005684  P-0.0211147 0.0037124                 P  -108.108    0.322   -10.483    0.160                                                     
+24 5 2 60432.00 P  0.015834 0.004762  0.415535 0.005804  P-0.0212536 0.0038119                 P  -107.874    0.322   -10.554    0.160                                                     
+24 5 3 60433.00 P  0.017379 0.004839  0.417571 0.005923  P-0.0217105 0.0039105                 P  -107.754    0.322   -10.539    0.160                                                     
+24 5 4 60434.00 P  0.018957 0.004915  0.419582 0.006041  P-0.0224643 0.0040082                 P  -107.831    0.322   -10.348    0.160                                                     
+24 5 5 60435.00 P  0.020567 0.004990  0.421567 0.006158  P-0.0234135 0.0041051                 P  -108.134    0.322   -10.007    0.160                                                     
+24 5 6 60436.00 P  0.022208 0.005065  0.423527 0.006274  P-0.0243924 0.0042012                 P  -108.599    0.322    -9.696    0.160                                                     
+24 5 7 60437.00 P  0.023881 0.005138  0.425461 0.006390  P-0.0252290 0.0042965                 P  -109.087    0.322    -9.570    0.160                                                     
+24 5 8 60438.00 P  0.025585 0.005211  0.427367 0.006504  P-0.0257912 0.0043911                 P  -109.491    0.322    -9.626    0.160                                                     
+24 5 9 60439.00 P  0.027319 0.005283  0.429247 0.006618  P-0.0260252 0.0044849                 P  -109.761    0.322    -9.786    0.160                                                     
+24 510 60440.00 P  0.029083 0.005355  0.431099 0.006731  P-0.0259641 0.0045781                 P  -109.819    0.322   -10.031    0.160                                                     
+24 511 60441.00 P  0.030875 0.005425  0.432922 0.006844  P-0.0257020 0.0046706                 P  -109.585    0.322   -10.352    0.160                                                     
+24 512 60442.00 P  0.032697 0.005495  0.434717 0.006955  P-0.0253559 0.0047625                 P  -109.154    0.322   -10.631    0.160                                                     
+24 513 60443.00 P  0.034546 0.005564  0.436483 0.007066  P-0.0250264 0.0048537                 P  -108.797    0.322   -10.702    0.160                                                     
+24 514 60444.00 P  0.036423 0.005633  0.438220 0.007177  P-0.0247857 0.0049444                 P  -108.690    0.322   -10.538    0.160                                                     
+24 515 60445.00 P  0.038327 0.005701  0.439927 0.007286  P-0.0246742 0.0050344                 P  -108.733    0.322   -10.291    0.160                                                     
+24 516 60446.00 P  0.040258 0.005768  0.441603 0.007395  P-0.0247019 0.0051240                 P  -108.729    0.322   -10.114    0.160                                                     
+24 517 60447.00 P  0.042214 0.005835  0.443249 0.007504  P-0.0248588 0.0052129                 P  -108.659    0.322   -10.002    0.160                                                     
+24 518 60448.00 P  0.044195 0.005901  0.444864 0.007611  P-0.0251127 0.0053014                 P  -108.674    0.322    -9.846    0.160                                                     
+24 519 60449.00 P  0.046201 0.005967  0.446447 0.007718  P-0.0254111 0.0053893                 P  -108.871    0.322    -9.619    0.160                                                     
+24 520 60450.00 P  0.048231 0.006032  0.447999 0.007825  P-0.0256903 0.0054768                 P  -109.186    0.322    -9.454    0.160                                                     
+24 521 60451.00 P  0.050285 0.006097  0.449518 0.007931  P-0.0258821 0.0055637                 P  -109.501    0.322    -9.508    0.160                                                     
+24 522 60452.00 P  0.052361 0.006161  0.451005 0.008037  P-0.0259244 0.0056502                 P  -109.755    0.322    -9.783    0.160                                                     
+24 523 60453.00 P  0.054460 0.006225  0.452460 0.008141  P-0.0257747 0.0057362                 P  -109.927    0.322   -10.114    0.160                                                     
+24 524 60454.00 P  0.056580 0.006288  0.453881 0.008246  P-0.0254232 0.0058218                 P  -109.996    0.322   -10.322    0.160                                                     
+24 525 60455.00 P  0.058721 0.006350  0.455268 0.008350  P-0.0249018 0.0059070                 P  -109.965    0.322   -10.356    0.160                                                     
+24 526 60456.00 P  0.060883 0.006413  0.456622 0.008453  P-0.0242859 0.0059917                 P  -109.891    0.322   -10.301    0.160                                                     
+24 527 60457.00 P  0.063064 0.006474  0.457942 0.008556  P-0.0236753 0.0060760                 P  -109.822    0.322   -10.268    0.160                                                     
+24 528 60458.00 P  0.065265 0.006536  0.459227 0.008659  P-0.0231863 0.0061599                 P  -109.732    0.322   -10.294    0.160                                                     
+24 529 60459.00 P  0.067484 0.006596  0.460478 0.008760  P-0.0229134 0.0062434                 P  -109.573    0.322   -10.336    0.160                                                     
+24 530 60460.00 P  0.069721 0.006657  0.461694 0.008862  P-0.0229074 0.0063266                 P  -109.387    0.322   -10.320    0.160                                                     
+24 531 60461.00 P  0.071974 0.006717  0.462874 0.008963  P-0.0231590 0.0064093                 P  -109.318    0.322   -10.200    0.160                                                     
+24 6 1 60462.00 P  0.074245 0.006777  0.464020 0.009064  P-0.0235905 0.0064917                 P  -109.489    0.322    -9.981    0.160                                                     
+24 6 2 60463.00 P  0.076531 0.006836  0.465129 0.009164  P-0.0240725 0.0065737                 P  -109.884    0.322    -9.725    0.160                                                     
+24 6 3 60464.00 P  0.078833 0.006895  0.466203 0.009264  P-0.0244495 0.0066554                 P  -110.358    0.322    -9.526    0.160                                                     
+24 6 4 60465.00 P  0.081149 0.006953  0.467241 0.009363  P-0.0245871 0.0067368                 P  -110.765    0.322    -9.454    0.160                                                     
+24 6 5 60466.00 P  0.083479 0.007011  0.468242 0.009462  P-0.0244077 0.0068177                 P  -111.047    0.322    -9.522    0.160                                                     
+24 6 6 60467.00 P  0.085823 0.007069  0.469206 0.009560  P-0.0239085 0.0068984                 P  -111.209    0.322    -9.704    0.160                                                     
+24 6 7 60468.00 P  0.088179 0.007126  0.470135 0.009659  P-0.0231583 0.0069788                                                                                                             
+24 6 8 60469.00 P  0.090546 0.007183  0.471026 0.009756  P-0.0222650 0.0070588                                                                                                             
+24 6 9 60470.00 P  0.092925 0.007240  0.471880 0.009854  P-0.0213421 0.0071385                                                                                                             
+24 610 60471.00 P  0.095315 0.007296  0.472697 0.009951  P-0.0204812 0.0072179                                                                                                             
+24 611 60472.00 P  0.097714 0.007352  0.473476 0.010047  P-0.0197379 0.0072970                                                                                                             
+24 612 60473.00 P  0.100123 0.007408  0.474218 0.010144  P-0.0191313 0.0073758                                                                                                             
+24 613 60474.00 P  0.102540 0.007464  0.474923 0.010240  P-0.0186569 0.0074544                                                                                                             
+24 614 60475.00 P  0.104965 0.007519  0.475589 0.010335  P-0.0182866 0.0075326                                                                                                             
+24 615 60476.00 P  0.107398 0.007573  0.476218 0.010430  P-0.0179739 0.0076106                                                                                                             
+24 616 60477.00 P  0.109836 0.007628  0.476809 0.010525  P-0.0176564 0.0076883                                                                                                             
+24 617 60478.00 P  0.112281 0.007682  0.477362 0.010620  P-0.0172677 0.0077657                                                                                                             
+24 618 60479.00 P  0.114731 0.007736  0.477877 0.010714  P-0.0167470 0.0078428                                                                                                             
+24 619 60480.00 P  0.117185 0.007790  0.478353 0.010808  P-0.0160452 0.0079197                                                                                                             
+24 620 60481.00 P  0.119643 0.007843  0.478792 0.010902  P-0.0151404 0.0079964                                                                                                             
+24 621 60482.00 P  0.122104 0.007896  0.479192 0.010995  P-0.0140455 0.0080728                                                                                                             
+24 622 60483.00 P  0.124567 0.007949  0.479554 0.011088  P-0.0128189 0.0081489                                                                                                             
+24 623 60484.00 P  0.127032 0.008002  0.479878 0.011180  P-0.0115615 0.0082248                                                                                                             
+24 624 60485.00 P  0.129498 0.008054  0.480163 0.011273  P-0.0103945 0.0083005                                                                                                             
+24 625 60486.00 P  0.131965 0.008106  0.480410 0.011365  P-0.0094319 0.0083759                                                                                                             
+24 626 60487.00 P  0.134431 0.008158  0.480619 0.011457  P-0.0087403 0.0084511                                                                                                             
+24 627 60488.00 P  0.136896 0.008209  0.480789 0.011548  P-0.0083167 0.0085261                                                                                                             
+24 628 60489.00 P  0.139359 0.008260  0.480922 0.011639  P-0.0080873 0.0086008                                                                                                             
+24 629 60490.00 P  0.141820 0.008312  0.481016 0.011730  P-0.0079261 0.0086754                                                                                                             
+24 630 60491.00 P  0.144278 0.008362  0.481072 0.011821  P-0.0076886 0.0087497                                                                                                             
+24 7 1 60492.00 P  0.146733 0.008413  0.481090 0.011912  P-0.0072492 0.0088237                                                                                                             
+24 7 2 60493.00 P  0.149183 0.008463  0.481070 0.012002  P-0.0065294 0.0088976                                                                                                             
+24 7 3 60494.00 P  0.151628 0.008513  0.481012 0.012092  P-0.0055155 0.0089713                                                                                                             
+24 7 4 60495.00 P  0.154067 0.008563  0.480916 0.012181  P-0.0042543 0.0090448                                                                                                             
+24 7 5 60496.00 P  0.156500 0.008613  0.480783 0.012271  P-0.0028393 0.0091180                                                                                                             
+24 7 6 60497.00 P  0.158926 0.008663  0.480612 0.012360  P-0.0013812 0.0091911                                                                                                             
+24 7 7 60498.00 P  0.161345 0.008712  0.480404 0.012449  P 0.0000182 0.0092639                                                                                                             
+24 7 8 60499.00 P  0.163756 0.008761  0.480156 0.012537  P 0.0012874 0.0093366                                                                                                             
+24 7 9 60500.00 P  0.166159 0.008810  0.479871 0.012626  P 0.0023939 0.0094091                                                                                                             
+24 710 60501.00 P  0.168553 0.008858  0.479549 0.012714  P 0.0033418 0.0094814                                                                                                             
+24 711 60502.00 P  0.170936 0.008907  0.479190 0.012802  P 0.0041611 0.0095535                                                                                                             
+24 712 60503.00 P  0.173308 0.008955  0.478795 0.012889  P 0.0048997 0.0096254                                                                                                             
+24 713 60504.00 P  0.175669 0.009003  0.478363 0.012977  P 0.0056177 0.0096971                                                                                                             
+24 714 60505.00 P  0.178017 0.009051  0.477895 0.013064  P 0.0063807 0.0097686                                                                                                             
+24 715 60506.00 P  0.180353 0.009099  0.477391 0.013151  P 0.0072004 0.0098400                                                                                                             
+24 716 60507.00 P  0.182676 0.009146  0.476851 0.013238  P 0.0081676 0.0099112                                                                                                             
+24 717 60508.00 P  0.184984 0.009193  0.476275 0.013324  P 0.0093100 0.0099822                                                                                                             
+24 718 60509.00 P  0.187278 0.009241  0.475664 0.013410  P 0.0106264 0.0100531                                                                                                             
+24 719 60510.00 P  0.189557 0.009288  0.475018 0.013497  P 0.0120748 0.0101238                                                                                                             
+24 720 60511.00 P  0.191820 0.009334  0.474337 0.013582  P 0.0135687 0.0101943                                                                                                             
+24 721 60512.00 P  0.194067 0.009381  0.473621 0.013668  P 0.0149853 0.0102646                                                                                                             
+24 722 60513.00 P  0.196296 0.009427  0.472871 0.013754  P 0.0161962 0.0103348                                                                                                             
+24 723 60514.00 P  0.198508 0.009474  0.472086 0.013839  P 0.0171083 0.0104048                                                                                                             
+24 724 60515.00 P  0.200702 0.009520  0.471268 0.013924  P 0.0177020 0.0104747                                                                                                             
+24 725 60516.00 P  0.202878 0.009565  0.470417 0.014009  P 0.0180446 0.0105444                                                                                                             
+24 726 60517.00 P  0.205034 0.009611  0.469532 0.014093  P 0.0182714 0.0106139                                                                                                             
+24 727 60518.00 P  0.207170 0.009657  0.468615 0.014178  P 0.0185434 0.0106833                                                                                                             
+24 728 60519.00 P  0.209286 0.009702  0.467665 0.014262  P 0.0190004 0.0107526                                                                                                             
+24 729 60520.00 P  0.211381 0.009747  0.466682 0.014346  P 0.0197271 0.0108216                                                                                                             
+24 730 60521.00 P  0.213455 0.009793  0.465668 0.014430  P 0.0207400 0.0108906                                                                                                             
+24 731 60522.00 P  0.215507 0.009837  0.464623 0.014514  P 0.0219940 0.0109594                                                                                                             
+24 8 1 60523.00 P  0.217536 0.009882  0.463546 0.014597  P 0.0234014 0.0110280                                                                                                             
+24 8 2 60524.00 P  0.219542 0.009927  0.462438 0.014681  P 0.0248556 0.0110965                                                                                                             
+24 8 3 60525.00 P  0.221525 0.009971  0.461300 0.014764  P 0.0262556 0.0111649                                                                                                             
+24 8 4 60526.00 P  0.223484 0.010016  0.460132 0.014847  P 0.0275236 0.0112331                                                                                                             
+24 8 5 60527.00 P  0.225418 0.010060  0.458934 0.014930  P 0.0286152 0.0113012                                                                                                             
+24 8 6 60528.00 P  0.227328 0.010104  0.457707 0.015012  P 0.0295215 0.0113691                                                                                                             
+24 8 7 60529.00 P  0.229212 0.010148  0.456452 0.015095  P 0.0302657 0.0114369                                                                                                             
+24 8 8 60530.00 P  0.231070 0.010192  0.455167 0.015177  P 0.0308946 0.0115046                                                                                                             
+24 8 9 60531.00 P  0.232902 0.010235  0.453855 0.015259  P 0.0314700 0.0115721                                                                                                             
+24 810 60532.00 P  0.234707 0.010279  0.452515 0.015341  P 0.0320587 0.0116395                                                                                                             
+24 811 60533.00 P  0.236484 0.010322  0.451148 0.015422  P 0.0327226 0.0117067                                                                                                             
+24 812 60534.00 P  0.238235 0.010365  0.449754 0.015504  P 0.0335105 0.0117739                                                                                                             
+24 813 60535.00 P  0.239957 0.010408  0.448334 0.015585  P 0.0344515 0.0118409                                                                                                             
+24 814 60536.00 P  0.241650 0.010451  0.446888 0.015667  P 0.0355505 0.0119077                                                                                                             
+24 815 60537.00 P  0.243315 0.010494  0.445417 0.015748  P 0.0367801 0.0119745                                                                                                             
+24 816 60538.00 P  0.244950 0.010537  0.443921 0.015829  P 0.0380726 0.0120411                                                                                                             
+24 817 60539.00 P  0.246556 0.010579  0.442400 0.015909  P 0.0393202 0.0121076                                                                                                             
+24 818 60540.00 P  0.248131 0.010622  0.440856 0.015990  P 0.0403905 0.0121740                                                                                                             
+24 819 60541.00 P  0.249676 0.010664  0.439288 0.016070  P 0.0411620 0.0122402                                                                                                             
+24 820 60542.00 P  0.251191 0.010706  0.437697 0.016151  P 0.0415718 0.0123063                                                                                                             
+24 821 60543.00 P  0.252674 0.010748  0.436083 0.016231  P 0.0416493 0.0123723                                                                                                             
+24 822 60544.00 P  0.254126 0.010790  0.434448 0.016311  P 0.0415171 0.0124382                                                                                                             
+24 823 60545.00 P  0.255545 0.010832  0.432791 0.016391  P 0.0413542 0.0125040                                                                                                             
+24 824 60546.00 P  0.256933 0.010873  0.431113 0.016470  P 0.0413380 0.0125696                                                                                                             
+24 825 60547.00 P  0.258288 0.010915  0.429414 0.016550  P 0.0415909 0.0126352                                                                                                             
+24 826 60548.00 P  0.259611 0.010956  0.427696 0.016629  P 0.0421510 0.0127006                                                                                                             
+24 827 60549.00 P  0.260900 0.010998  0.425958 0.016708  P 0.0429772 0.0127659                                                                                                             
+24 828 60550.00 P  0.262156 0.011039  0.424201 0.016787  P 0.0439768 0.0128311                                                                                                             
+24 829 60551.00 P  0.263379 0.011080  0.422426 0.016866  P 0.0450375 0.0128962                                                                                                             
+24 830 60552.00 P  0.264567 0.011121  0.420633 0.016945  P 0.0460538 0.0129612                                                                                                             
+24 831 60553.00 P  0.265722 0.011162  0.418823 0.017024  P 0.0469437 0.0130260                                                                                                             
+24 9 1 60554.00 P  0.266842 0.011202  0.416996 0.017102  P 0.0476562 0.0130908                                                                                                             
+24 9 2 60555.00 P  0.267927 0.011243  0.415153 0.017181  P 0.0481740 0.0131554                                                                                                             
+24 9 3 60556.00 P  0.268978 0.011283  0.413294 0.017259  P 0.0485108 0.0132199                                                                                                             
+24 9 4 60557.00 P  0.269994 0.011324  0.411420 0.017337  P 0.0487073 0.0132844                                                                                                             
+24 9 5 60558.00 P  0.270974 0.011364  0.409531 0.017415  P 0.0488234 0.0133487                                                                                                             
+24 9 6 60559.00 P  0.271919 0.011404  0.407628 0.017493  P 0.0489282 0.0134129                                                                                                             
+24 9 7 60560.00 P  0.272829 0.011444  0.405712 0.017570  P 0.0490888 0.0134770                                                                                                             
+24 9 8 60561.00 P  0.273702 0.011484  0.403784 0.017648  P 0.0493601 0.0135410                                                                                                             
+24 9 9 60562.00 P  0.274540 0.011524  0.401842 0.017725  P 0.0497764 0.0136050                                                                                                             
+24 910 60563.00 P  0.275342 0.011564  0.399889 0.017803  P 0.0503471 0.0136688                                                                                                             
+24 911 60564.00 P  0.276107 0.011604  0.397925 0.017880  P 0.0510532 0.0137325                                                                                                             
+24 912 60565.00 P  0.276836 0.011643  0.395951 0.017957  P 0.0518425 0.0137961                                                                                                             
+24 913 60566.00 P  0.277529 0.011683  0.393966 0.018034  P 0.0526269 0.0138596                                                                                                             
+24 914 60567.00 P  0.278185 0.011722  0.391972 0.018110  P 0.0532874 0.0139230                                                                                                             
+24 915 60568.00 P  0.278804 0.011761  0.389969 0.018187  P 0.0536965 0.0139863                                                                                                             
+24 916 60569.00 P  0.279387 0.011800  0.387958 0.018264  P 0.0537572 0.0140495                                                                                                             
+24 917 60570.00 P  0.279933 0.011839  0.385939 0.018340  P 0.0534464 0.0141127                                                                                                             
+24 918 60571.00 P  0.280442 0.011878  0.383912 0.018416  P 0.0528402 0.0141757                                                                                                             
+24 919 60572.00 P  0.280914 0.011917  0.381880 0.018492  P 0.0521031 0.0142386                                                                                                             
+24 920 60573.00 P  0.281349 0.011956  0.379841 0.018568  P 0.0514356 0.0143014                                                                                                             
+24 921 60574.00 P  0.281747 0.011995  0.377797 0.018644  P 0.0510117 0.0143642                                                                                                             
+24 922 60575.00 P  0.282108 0.012033  0.375748 0.018720  P 0.0509222 0.0144268                                                                                                             
+24 923 60576.00 P  0.282432 0.012072  0.373695 0.018796  P 0.0511605 0.0144894                                                                                                             
+24 924 60577.00 P  0.282718 0.012110  0.371639 0.018871  P 0.0516415 0.0145519                                                                                                             
+24 925 60578.00 P  0.282968 0.012148  0.369579 0.018947  P 0.0522440 0.0146142                                                                                                             
+24 926 60579.00 P  0.283181 0.012187  0.367517 0.019022  P 0.0528499 0.0146765                                                                                                             
+24 927 60580.00 P  0.283357 0.012225  0.365453 0.019097  P 0.0533700 0.0147387                                                                                                             
+24 928 60581.00 P  0.283496 0.012263  0.363388 0.019172  P 0.0537502 0.0148008                                                                                                             
+24 929 60582.00 P  0.283598 0.012301  0.361322 0.019247  P 0.0539722 0.0148629                                                                                                             
+24 930 60583.00 P  0.283663 0.012339  0.359256 0.019322  P 0.0540477 0.0149248                                                                                                             
+2410 1 60584.00 P  0.283692 0.012376  0.357190 0.019397  P 0.0540140 0.0149867                                                                                                             
+2410 2 60585.00 P  0.283684 0.012414  0.355125 0.019472  P 0.0539277 0.0150484                                                                                                             
+2410 3 60586.00 P  0.283639 0.012452  0.353062 0.019546  P 0.0538547 0.0151101                                                                                                             
+2410 4 60587.00 P  0.283558 0.012489  0.351001 0.019620  P 0.0538586 0.0151717                                                                                                             
+2410 5 60588.00 P  0.283440 0.012527  0.348943 0.019695  P 0.0539886 0.0152332                                                                                                             
+2410 6 60589.00 P  0.283286 0.012564  0.346888 0.019769  P 0.0542714 0.0152946                                                                                                             
+2410 7 60590.00 P  0.283097 0.012601  0.344837 0.019843  P 0.0547085 0.0153560                                                                                                             
+2410 8 60591.00 P  0.282871 0.012638  0.342790 0.019917  P 0.0552769 0.0154172                                                                                                             
+2410 9 60592.00 P  0.282609 0.012676  0.340749 0.019991  P 0.0559296 0.0154784                                                                                                             
+241010 60593.00 P  0.282312 0.012713  0.338713 0.020065  P 0.0565947 0.0155395                                                                                                             
+241011 60594.00 P  0.281980 0.012749  0.336683 0.020138  P 0.0571753 0.0156005                                                                                                             
+241012 60595.00 P  0.281612 0.012786  0.334660 0.020212  P 0.0575591 0.0156614                                                                                                             
+241013 60596.00 P  0.281209 0.012823  0.332644 0.020285  P 0.0576435 0.0157223                                                                                                             
+241014 60597.00 P  0.280771 0.012860  0.330635 0.020359  P 0.0573711 0.0157831                                                                                                             
+241015 60598.00 P  0.280299 0.012896  0.328635 0.020432  P 0.0567648 0.0158438                                                                                                             
+241016 60599.00 P  0.279792 0.012933  0.326644 0.020505  P 0.0559391 0.0159044                                                                                                             
+241017 60600.00 P  0.279251 0.012969  0.324663 0.020578  P 0.0550769 0.0159649                                                                                                             
+241018 60601.00 P  0.278676 0.013006  0.322691 0.020651  P 0.0543749 0.0160254                                                                                                             
+241019 60602.00 P  0.278067 0.013042  0.320729 0.020724  P 0.0539781 0.0160858                                                                                                             
+241020 60603.00 P  0.277425 0.013078  0.318779 0.020797  P 0.0539355 0.0161461                                                                                                             
+241021 60604.00 P  0.276750 0.013114  0.316840 0.020869  P 0.0541938 0.0162063                                                                                                             
+241022 60605.00 P  0.276042 0.013150  0.314913 0.020942  P 0.0546314 0.0162665                                                                                                             
+241023 60606.00 P  0.275301 0.013186  0.312999 0.021014  P 0.0551091 0.0163265                                                                                                             
+241024 60607.00 P  0.274528 0.013222  0.311098 0.021086  P 0.0555118 0.0163866                                                                                                             
+241025 60608.00 P  0.273723 0.013258  0.309210 0.021159  P 0.0557651 0.0164465                                                                                                             
+241026 60609.00 P  0.272887 0.013294  0.307336 0.021231  P 0.0558330 0.0165063                                                                                                             
+241027 60610.00 P  0.272019 0.013330  0.305477 0.021303  P 0.0557139 0.0165661                                                                                                             
+241028 60611.00 P  0.271120 0.013365  0.303633 0.021375  P 0.0554377 0.0166258                                                                                                             
+241029 60612.00 P  0.270190 0.013401  0.301804 0.021447  P 0.0550582 0.0166855                                                                                                             
+241030 60613.00 P  0.269230 0.013436  0.299991 0.021519  P 0.0546429 0.0167451                                                                                                             
+241031 60614.00 P  0.268240 0.013472  0.298195 0.021590  P 0.0542578 0.0168046                                                                                                             
+2411 1 60615.00 P  0.267220 0.013507  0.296416 0.021662  P 0.0539608 0.0168640                                                                                                             
+2411 2 60616.00 P  0.266171 0.013542  0.294654 0.021733  P 0.0538121 0.0169233                                                                                                             
+2411 3 60617.00 P  0.265094 0.013578  0.292909 0.021805  P 0.0538609 0.0169826                                                                                                             
+2411 4 60618.00 P  0.263987 0.013613  0.291183 0.021876  P 0.0541115 0.0170419                                                                                                             
+2411 5 60619.00 P  0.262853 0.013648  0.289476 0.021947  P 0.0544598 0.0171010                                                                                                             
+2411 6 60620.00 P  0.261691 0.013683  0.287788 0.022018  P 0.0548011 0.0171601                                                                                                             
+2411 7 60621.00 P  0.260502 0.013718  0.286119 0.022089  P 0.0550830 0.0172191                                                                                                             
+2411 8 60622.00 P  0.259286 0.013753  0.284471 0.022160  P 0.0551698 0.0172780                                                                                                             
+2411 9 60623.00 P  0.258043 0.013788  0.282842 0.022231  P 0.0550677 0.0173369                                                                                                             
+241110 60624.00 P  0.256775 0.013822  0.281235 0.022302  P 0.0545807 0.0173957                                                                                                             
+241111 60625.00 P  0.255481 0.013857  0.279648 0.022373  P 0.0538548 0.0174545                                                                                                             
+241112 60626.00 P  0.254161 0.013892  0.278084 0.022443  P 0.0529236 0.0175131                                                                                                             
+241113 60627.00 P  0.252818 0.013926  0.276541 0.022514  P 0.0518639 0.0175718                                                                                                             
+241114 60628.00 P  0.251449 0.013961  0.275020 0.022584  P 0.0508994 0.0176303                                                                                                             
+241115 60629.00 P  0.250058 0.013995  0.273523 0.022655  P 0.0502230 0.0176888                                                                                                             
+241116 60630.00 P  0.248642 0.014029  0.272048 0.022725  P 0.0498967 0.0177472                                                                                                             
+241117 60631.00 P  0.247204 0.014064  0.270597 0.022795  P 0.0498677 0.0178055                                                                                                             
+241118 60632.00 P  0.245744 0.014098  0.269170 0.022865  P 0.0500938 0.0178638                                                                                                             
+241119 60633.00 P  0.244262 0.014132  0.267766 0.022935  P 0.0504464 0.0179220                                                                                                             
+241120 60634.00 P  0.242758 0.014166  0.266387 0.023005  P 0.0507622 0.0179802                                                                                                             
+241121 60635.00 P  0.241234 0.014200  0.265033 0.023075  P 0.0508377 0.0180383                                                                                                             
+241122 60636.00 P  0.239689 0.014234  0.263705 0.023145  P 0.0506912 0.0180963                                                                                                             
+241123 60637.00 P  0.238124 0.014268  0.262401 0.023214  P 0.0503988 0.0181543                                                                                                             
+241124 60638.00 P  0.236540 0.014302  0.261123 0.023284  P 0.0499223 0.0182122                                                                                                             
+241125 60639.00 P  0.234937 0.014336  0.259871 0.023354  P 0.0493741 0.0182700                                                                                                             
+241126 60640.00 P  0.233315 0.014369  0.258646 0.023423  P 0.0488191 0.0183278                                                                                                             
+241127 60641.00 P  0.231676 0.014403  0.257447 0.023492  P 0.0482433 0.0183855                                                                                                             
+241128 60642.00 P  0.230020 0.014437  0.256275 0.023562  P 0.0477649 0.0184432                                                                                                             
+241129 60643.00 P  0.228347 0.014470  0.255130 0.023631  P 0.0474514 0.0185008                                                                                                             
+241130 60644.00 P  0.226657 0.014504  0.254012 0.023700  P 0.0472740 0.0185583                                                                                                             
+2412 1 60645.00 P  0.224952 0.014537  0.252922 0.023769  P 0.0472205 0.0186158                                                                                                             
+2412 2 60646.00 P  0.223232 0.014571  0.251860 0.023838  P 0.0473032 0.0186732                                                                                                             
+2412 3 60647.00 P  0.221497 0.014604  0.250825 0.023907  P 0.0475462 0.0187306                                                                                                             
+2412 4 60648.00 P  0.219748 0.014637  0.249819 0.023976  P 0.0477937 0.0187879                                                                                                             
+2412 5 60649.00 P  0.217986 0.014670  0.248842 0.024044  P 0.0478374 0.0188451                                                                                                             
+2412 6 60650.00 P  0.216210 0.014704  0.247893 0.024113  P 0.0476758 0.0189023                                                                                                             
+2412 7 60651.00 P  0.214422 0.014737  0.246973 0.024182  P 0.0472312 0.0189594                                                                                                             
+2412 8 60652.00 P  0.212623 0.014770  0.246082 0.024250  P 0.0464937 0.0190165                                                                                                             
+2412 9 60653.00 P  0.210812 0.014803  0.245221 0.024319  P 0.0454841 0.0190735                                                                                                             
+241210 60654.00 P  0.208990 0.014836  0.244388 0.024387  P 0.0442908 0.0191305                                                                                                             
+241211 60655.00 P  0.207158 0.014869  0.243585 0.024455  P 0.0431558 0.0191874                                                                                                             
+241212 60656.00 P  0.205317 0.014901  0.242812 0.024523  P 0.0422120 0.0192442                                                                                                             
+241213 60657.00 P  0.203467 0.014934  0.242069 0.024592  P 0.0415468 0.0193010                                                                                                             
+241214 60658.00 P  0.201608 0.014967  0.241356 0.024660  P 0.0412094 0.0193577                                                                                                             
+241215 60659.00 P  0.199741 0.015000  0.240672 0.024728  P 0.0410972 0.0194144                                                                                                             
+241216 60660.00 P  0.197867 0.015032  0.240019 0.024796  P 0.0411469 0.0194710                                                                                                             
+241217 60661.00 P  0.195986 0.015065  0.239396 0.024863  P 0.0412184 0.0195276                                                                                                             
+241218 60662.00 P  0.194099 0.015097  0.238804 0.024931  P 0.0411386 0.0195841                                                                                                             
+241219 60663.00 P  0.192206 0.015130  0.238242 0.024999  P 0.0408812 0.0196405                                                                                                             
+241220 60664.00 P  0.190309 0.015162  0.237710 0.025067  P 0.0404580 0.0196969                                                                                                             
+241221 60665.00 P  0.188407 0.015194  0.237209 0.025134  P 0.0398667 0.0197532                                                                                                             
+241222 60666.00 P  0.186501 0.015227  0.236739 0.025202  P 0.0392805 0.0198095                                                                                                             
+241223 60667.00 P  0.184591 0.015259  0.236300 0.025269  P 0.0387085 0.0198658                                                                                                             
+241224 60668.00 P  0.182679 0.015291  0.235891 0.025336  P 0.0381796 0.0199219                                                                                                             
+241225 60669.00 P  0.180765 0.015323  0.235513 0.025404  P 0.0378319 0.0199781                                                                                                             
+241226 60670.00 P  0.178850 0.015355  0.235165 0.025471  P 0.0376142 0.0200341                                                                                                             
+241227 60671.00 P  0.176933 0.015387  0.234849 0.025538  P 0.0376027 0.0200902                                                                                                             
+241228 60672.00 P  0.175016 0.015419  0.234563 0.025605  P 0.0379161 0.0201461                                                                                                             
+241229 60673.00 P  0.173098 0.015451  0.234308 0.025672  P 0.0382490 0.0202021                                                                                                             
+241230 60674.00 P  0.171182 0.015483  0.234084 0.025739  P 0.0387786 0.0202579                                                                                                             
+241231 60675.00 P  0.169267 0.015515  0.233890 0.025806  P 0.0393248 0.0203137                                                                                                             
+25 1 1 60676.00 P  0.167354 0.015547  0.233727 0.025873  P 0.0398723 0.0203695                                                                                                             
+25 1 2 60677.00 P  0.165443 0.015578  0.233595 0.025939  P 0.0401528 0.0204252                                                                                                             
+25 1 3 60678.00 P  0.163535 0.015610  0.233494 0.026006  P 0.0401294 0.0204809                                                                                                             
+25 1 4 60679.00 P  0.161630 0.015642  0.233423 0.026073  P 0.0397809 0.0205365                                                                                                             
+25 1 5 60680.00 P  0.159730 0.015673  0.233382 0.026139  P 0.0392198 0.0205920                                                                                                             
+25 1 6 60681.00 P  0.157834 0.015705  0.233372 0.026206  P 0.0383936 0.0206475                                                                                                             
+25 1 7 60682.00 P  0.155943 0.015736  0.233392 0.026272  P 0.0375241 0.0207030                                                                                                             
+25 1 8 60683.00 P  0.154058 0.015768  0.233442 0.026338  P 0.0367918 0.0207584                                                                                                             
+25 1 9 60684.00 P  0.152179 0.015799  0.233523 0.026405  P 0.0362191 0.0208138                                                                                                             
+25 110 60685.00 P  0.150308 0.015831  0.233633 0.026471  P 0.0359207 0.0208691                                                                                                             
+25 111 60686.00 P  0.148443 0.015862  0.233773 0.026537  P 0.0359466 0.0209243                                                                                                             
+25 112 60687.00 P  0.146586 0.015893  0.233943 0.026603  P 0.0361820 0.0209795                                                                                                             
+25 113 60688.00 P  0.144738 0.015924  0.234143 0.026669  P 0.0365292 0.0210347                                                                                                             
+25 114 60689.00 P  0.142899 0.015956  0.234372 0.026735  P 0.0368268 0.0210898                                                                                                             
+25 115 60690.00 P  0.141069 0.015987  0.234630 0.026801  P 0.0369877 0.0211449                                                                                                             
+25 116 60691.00 P  0.139249 0.016018  0.234918 0.026867  P 0.0368682 0.0211999                                                                                                             
+25 117 60692.00 P  0.137440 0.016049  0.235234 0.026933  P 0.0365847 0.0212548                                                                                                             
+25 118 60693.00 P  0.135641 0.016080  0.235579 0.026998  P 0.0360826 0.0213098                                                                                                             
+25 119 60694.00 P  0.133855 0.016111  0.235953 0.027064  P 0.0354889 0.0213646                                                                                                             
+25 120 60695.00 P  0.132080 0.016142  0.236355 0.027130  P 0.0348377 0.0214195                                                                                                             
+25 121 60696.00 P  0.130318 0.016173  0.236785 0.027195  P 0.0342260 0.0214742                                                                                                             
+25 122 60697.00 P  0.128568 0.016203  0.237244 0.027261  P 0.0337603 0.0215290                                                                                                             
+25 123 60698.00 P  0.126833 0.016234  0.237729 0.027326  P 0.0335397 0.0215837                                                                                                             
+25 124 60699.00 P  0.125111 0.016265  0.238243 0.027391  P 0.0335747 0.0216383                                                                                                             
+25 125 60700.00 P  0.123404 0.016296  0.238784 0.027457  P 0.0337341 0.0216929                                                                                                             
+25 126 60701.00 P  0.121711 0.016326  0.239351 0.027522  P 0.0340399 0.0217474                                                                                                             
+25 127 60702.00 P  0.120034 0.016357  0.239946 0.027587  P 0.0344215 0.0218019                                                                                                             
+25 128 60703.00 P  0.118373 0.016387  0.240567 0.027652  P 0.0347305 0.0218564                                                                                                             
+25 129 60704.00 P  0.116729 0.016418  0.241214 0.027717  P 0.0348607 0.0219108                                                                                                             
+25 130 60705.00 P  0.115101 0.016448  0.241888 0.027782  P 0.0346061 0.0219652                                                                                                             
+25 131 60706.00 P  0.113490 0.016479  0.242587 0.027847  P 0.0340722 0.0220195                                                                                                             
+25 2 1 60707.00 P  0.111897 0.016509  0.243311 0.027912  P 0.0332099 0.0220738                                                                                                             
+25 2 2 60708.00 P  0.110322 0.016539  0.244061 0.027977  P 0.0321843 0.0221280                                                                                                             
+25 2 3 60709.00 P  0.108766 0.016570  0.244835 0.028041  P 0.0310848 0.0221822                                                                                                             
+25 2 4 60710.00 P  0.107228 0.016600  0.245634 0.028106  P 0.0301319 0.0222363                                                                                                             
+25 2 5 60711.00 P  0.105710 0.016630  0.246457 0.028171  P 0.0294940 0.0222904                                                                                                             
+25 2 6 60712.00 P  0.104212 0.016660  0.247304 0.028235  P 0.0290967 0.0223444                                                                                                             
+25 2 7 60713.00 P  0.102734 0.016690  0.248174 0.028300  P 0.0289882 0.0223985                                                                                                             
+25 2 8 60714.00 P  0.101276 0.016721  0.249068 0.028364  P 0.0290782 0.0224524                                                                                                             
+25 2 9 60715.00 P  0.099839 0.016751  0.249985 0.028429  P 0.0292864 0.0225063                                                                                                             
+25 210 60716.00 P  0.098424 0.016781  0.250924 0.028493  P 0.0294029 0.0225602                                                                                                             
+25 211 60717.00 P  0.097030 0.016811  0.251885 0.028557  P 0.0293941 0.0226140                                                                                                             
+25 212 60718.00 P  0.095659 0.016840  0.252868 0.028621  P 0.0291722 0.0226678                                                                                                             
+25 213 60719.00 P  0.094309 0.016870  0.253873 0.028686  P 0.0287260 0.0227216                                                                                                             
+25 214 60720.00 P  0.092983 0.016900  0.254899 0.028750  P 0.0281458 0.0227753                                                                                                             
+25 215 60721.00 P  0.091679 0.016930  0.255945 0.028814  P 0.0274248 0.0228290                                                                                                             
+25 216 60722.00 P  0.090399 0.016960  0.257012 0.028878  P 0.0266025 0.0228826                                                                                                             
+25 217 60723.00 P  0.089143 0.016989  0.258099 0.028942  P 0.0257445 0.0229362                                                                                                             
+25 218 60724.00 P  0.087911 0.017019  0.259205 0.029006  P 0.0249582 0.0229897                                                                                                             
+25 219 60725.00 P  0.086703 0.017049  0.260331 0.029069  P 0.0243090 0.0230432                                                                                                             
+25 220 60726.00 P  0.085520 0.017078  0.261475 0.029133  P 0.0237492 0.0230966                                                                                                             
+25 221 60727.00 P  0.084362 0.017108  0.262638 0.029197  P 0.0233845 0.0231500                                                                                                             
+25 222 60728.00 P  0.083229 0.017138  0.263818 0.029261  P 0.0230773 0.0232034                                                                                                             
+25 223 60729.00 P  0.082122 0.017167  0.265017 0.029324  P 0.0228102 0.0232567                                                                                                             
+25 224 60730.00 P  0.081040 0.017196  0.266232 0.029388  P 0.0224558 0.0233100                                                                                                             
+25 225 60731.00 P  0.079984 0.017226  0.267464 0.029451  P 0.0219170 0.0233633                                                                                                             
+25 226 60732.00 P  0.078955 0.017255  0.268713 0.029515  P 0.0211303 0.0234165                                                                                                             
+25 227 60733.00 P  0.077953 0.017285  0.269977 0.029578  P 0.0200968 0.0234697                                                                                                             
+25 228 60734.00 P  0.076977 0.017314  0.271257 0.029641  P 0.0187798 0.0235228                                                                                                             
+25 3 1 60735.00 P  0.076028 0.017343  0.272551 0.029705  P 0.0171917 0.0235759                                                                                                             
+25 3 2 60736.00 P  0.075106 0.017372  0.273861 0.029768  P 0.0155689 0.0236289                                                                                                             
+25 3 3 60737.00 P  0.074212 0.017402  0.275184 0.029831  P 0.0141275 0.0236819                                                                                                             
+25 3 4 60738.00 P  0.073345 0.017431  0.276521 0.029894  P 0.0129183 0.0237349                                                                                                             
+25 3 5 60739.00 P  0.072507 0.017460  0.277872 0.029957  P 0.0121592 0.0237878                                                                                                             
+25 3 6 60740.00 P  0.071696 0.017489  0.279235 0.030021  P 0.0116587 0.0238407                                                                                                             
+25 3 7 60741.00 P  0.070913 0.017518  0.280610 0.030084  P 0.0115425 0.0238935                                                                                                             
+25 3 8 60742.00 P  0.070159 0.017547  0.281998 0.030146  P 0.0115512 0.0239463                                                                                                             
+25 3 9 60743.00 P  0.069433 0.017576  0.283397 0.030209  P 0.0116024 0.0239991                                                                                                             
+25 310 60744.00 P  0.068736 0.017605  0.284806 0.030272  P 0.0116011 0.0240518                                                                                                             
+25 311 60745.00 P  0.068068 0.017634  0.286227 0.030335  P 0.0113390 0.0241045                                                                                                             
+25 312 60746.00 P  0.067428 0.017663  0.287657 0.030398  P 0.0108597 0.0241572                                                                                                             
+25 313 60747.00 P  0.066818 0.017691  0.289097 0.030460  P 0.0102407 0.0242098                                                                                                             
+25 314 60748.00 P  0.066237 0.017720  0.290545 0.030523  P 0.0095205 0.0242624                                                                                                             
+25 315 60749.00 P  0.065684 0.017749  0.292003 0.030586  P 0.0087872 0.0243149                                                                                                             
+25 316 60750.00 P  0.065162 0.017778  0.293469 0.030648  P 0.0080552 0.0243674                                                                                                             
+25 317 60751.00 P  0.064668 0.017806  0.294942 0.030711  P 0.0074248 0.0244199                                                                                                             
+25 318 60752.00 P  0.064205 0.017835  0.296422 0.030773  P 0.0069686 0.0244723                                                                                                             
+25 319 60753.00 P  0.063770 0.017864  0.297910 0.030835  P 0.0067324 0.0245247                                                                                                             
+25 320 60754.00 P  0.063366 0.017892  0.299403 0.030898  P 0.0066748 0.0245770                                                                                                             
+25 321 60755.00 P  0.062991 0.017921  0.300902 0.030960  P 0.0068510 0.0246293                                                                                                             
+25 322 60756.00 P  0.062645 0.017949  0.302407 0.031022  P 0.0071099 0.0246816                                                                                                             
+25 323 60757.00 P  0.062330 0.017978  0.303916 0.031085  P 0.0074247 0.0247338                                                                                                             
+25 324 60758.00 P  0.062044 0.018006  0.305430 0.031147  P 0.0075868 0.0247860                                                                                                             
+25 325 60759.00 P  0.061787 0.018035  0.306948 0.031209  P 0.0075104 0.0248382                                                                                                             
+25 326 60760.00 P  0.061561 0.018063  0.308469 0.031271  P 0.0070686 0.0248903                                                                                                             
+25 327 60761.00 P  0.061364 0.018091  0.309992 0.031333  P 0.0063754 0.0249424                                                                                                             
+25 328 60762.00 P  0.061197 0.018120  0.311519 0.031395  P 0.0053494 0.0249945                                                                                                             
+25 329 60763.00 P  0.061060 0.018148  0.313047 0.031457  P 0.0041476 0.0250465                                                                                                             
+25 330 60764.00 P  0.060952 0.018176  0.314576 0.031519  P 0.0028886 0.0250985                                                                                                             
+25 331 60765.00 P  0.060874 0.018205  0.316107 0.031580  P 0.0017765 0.0251504                                                                                                             
+25 4 1 60766.00 P  0.060825 0.018233  0.317638 0.031642  P 0.0009167 0.0252023                                                                                                             
+25 4 2 60767.00 P  0.060806 0.018261  0.319169 0.031704  P 0.0004053 0.0252542                                                                                                             
+25 4 3 60768.00 P  0.060816 0.018289  0.320700 0.031766  P 0.0002585 0.0253060                                                                                                             
+25 4 4 60769.00 P  0.060856 0.018317  0.322230 0.031827  P 0.0003547 0.0253578                                                                                                             
+25 4 5 60770.00 P  0.060925 0.018345  0.323758 0.031889  P 0.0005453 0.0254096                                                                                                             
+25 4 6 60771.00                                                                                                                                                                            
+25 4 7 60772.00                                                                                                                                                                            
+25 4 8 60773.00                                                                                                                                                                            
+25 4 9 60774.00                                                                                                                                                                            
+25 410 60775.00                                                                                                                                                                            
+25 411 60776.00                                                                                                                                                                            
+25 412 60777.00                                                                                                                                                                            
+25 413 60778.00                                                                                                                                                                            
+25 414 60779.00                                                                                                                                                                            
+25 415 60780.00                                                                                                                                                                            
+25 416 60781.00                                                                                                                                                                            
+25 417 60782.00                                                                                                                                                                            
+25 418 60783.00                                                                                                                                                                            
+25 419 60784.00                                                                                                                                                                            
+25 420 60785.00                                                                                                                                                                            
+25 421 60786.00                                                                                                                                                                            
+25 422 60787.00                                                                                                                                                                            
+25 423 60788.00                                                                                                                                                                            
+25 424 60789.00                                                                                                                                                                            
+25 425 60790.00                                                                                                                                                                            
+25 426 60791.00                                                                                                                                                                            
+25 427 60792.00                                                                                                                                                                            
+25 428 60793.00                                                                                                                                                                            
+25 429 60794.00                                                                                                                                                                            
+25 430 60795.00                                                                                                                                                                            
+25 5 1 60796.00                                                                                                                                                                            
+25 5 2 60797.00                                                                                                                                                                            
+25 5 3 60798.00                                                                                                                                                                            
+25 5 4 60799.00                                                                                                                                                                            
+25 5 5 60800.00                                                                                                                                                                            
+25 5 6 60801.00                                                                                                                                                                            
+25 5 7 60802.00                                                                                                                                                                            
+25 5 8 60803.00                                                                                                                                                                            
+25 5 9 60804.00                                                                                                                                                                            
+25 510 60805.00                                                                                                                                                                            
+25 511 60806.00                                                                                                                                                                            
+25 512 60807.00                                                                                                                                                                            
+25 513 60808.00                                                                                                                                                                            
+25 514 60809.00                                                                                                                                                                            
+25 515 60810.00                                                                                                                                                                            
+25 516 60811.00                                                                                                                                                                            
+25 517 60812.00                                                                                                                                                                            
+25 518 60813.00                                                                                                                                                                            
+25 519 60814.00                                                                                                                                                                            
+25 520 60815.00                                                                                                                                                                            
+25 521 60816.00                                                                                                                                                                            
+25 522 60817.00                                                                                                                                                                            
+25 523 60818.00                                                                                                                                                                            
+25 524 60819.00                                                                                                                                                                            
+25 525 60820.00
```

### Comparing `pyTMD-2.1.0/pyTMD/data/historic_deltat.data` & `pyTMD-2.1.1/pyTMD/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/iers_deltat.data` & `pyTMD-2.1.1/pyTMD/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/leap-seconds.list` & `pyTMD-2.1.1/pyTMD/data/leap-seconds.list`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/mean-pole.tab` & `pyTMD-2.1.1/pyTMD/data/mean-pole.tab`

 * *Files 10% similar despite different names*

```diff
@@ -1,2471 +1,2485 @@
-1900.00  -0.0072168   0.0476686
-1900.05  -0.0072560   0.0478734
-1900.10  -0.0072961   0.0480786
-1900.15  -0.0073372   0.0482841
-1900.20  -0.0073793   0.0484898
-1900.25  -0.0074224   0.0486959
-1900.30  -0.0074664   0.0489023
-1900.35  -0.0075115   0.0491089
-1900.40  -0.0075576   0.0493158
-1900.45  -0.0076047   0.0495229
-1900.50  -0.0076528   0.0497303
-1900.55  -0.0077019   0.0499379
-1900.60  -0.0077521   0.0501457
-1900.65  -0.0078033   0.0503538
-1900.70  -0.0078556   0.0505620
-1900.75  -0.0079089   0.0507704
-1900.80  -0.0079632   0.0509790
-1900.85  -0.0080186   0.0511878
-1900.90  -0.0080751   0.0513967
-1900.95  -0.0081326   0.0516058
-1901.00  -0.0081912   0.0518150
-1901.05  -0.0082509   0.0520244
-1901.10  -0.0083116   0.0522338
-1901.15  -0.0083734   0.0524434
-1901.20  -0.0084363   0.0526531
-1901.25  -0.0085003   0.0528628
-1901.30  -0.0085653   0.0530727
-1901.35  -0.0086315   0.0532826
-1901.40  -0.0086987   0.0534925
-1901.45  -0.0087670   0.0537025
-1901.50  -0.0088364   0.0539126
-1901.55  -0.0089069   0.0541227
-1901.60  -0.0089785   0.0543328
-1901.65  -0.0090511   0.0545429
-1901.70  -0.0091249   0.0547531
-1901.75  -0.0091997   0.0549632
-1901.80  -0.0092756   0.0551733
-1901.85  -0.0093526   0.0553834
-1901.90  -0.0094307   0.0555935
-1901.95  -0.0095098   0.0558036
-1902.00  -0.0095900   0.0560136
-1902.05  -0.0096712   0.0562236
-1902.10  -0.0097535   0.0564336
-1902.15  -0.0098369   0.0566435
-1902.20  -0.0099213   0.0568533
-1902.25  -0.0100068   0.0570631
-1902.30  -0.0100932   0.0572728
-1902.35  -0.0101807   0.0574824
-1902.40  -0.0102693   0.0576920
-1902.45  -0.0103588   0.0579014
-1902.50  -0.0104493   0.0581108
-1902.55  -0.0105409   0.0583201
-1902.60  -0.0106334   0.0585293
-1902.65  -0.0107268   0.0587385
-1902.70  -0.0108213   0.0589475
-1902.75  -0.0109167   0.0591565
-1902.80  -0.0110130   0.0593653
-1902.85  -0.0111102   0.0595741
-1902.90  -0.0112083   0.0597827
-1902.95  -0.0113074   0.0599913
-1903.00  -0.0114073   0.0601998
-1903.05  -0.0115081   0.0604082
-1903.10  -0.0116097   0.0606165
-1903.15  -0.0117121   0.0608247
-1903.20  -0.0118154   0.0610328
-1903.25  -0.0119194   0.0612409
-1903.30  -0.0120243   0.0614489
-1903.35  -0.0121299   0.0616568
-1903.40  -0.0122362   0.0618647
-1903.45  -0.0123432   0.0620725
-1903.50  -0.0124510   0.0622802
-1903.55  -0.0125594   0.0624879
-1903.60  -0.0126685   0.0626956
-1903.65  -0.0127781   0.0629032
-1903.70  -0.0128884   0.0631108
-1903.75  -0.0129993   0.0633184
-1903.80  -0.0131108   0.0635260
-1903.85  -0.0132227   0.0637336
-1903.90  -0.0133352   0.0639412
-1903.95  -0.0134482   0.0641489
-1904.00  -0.0135616   0.0643566
-1904.05  -0.0136754   0.0645643
-1904.10  -0.0137896   0.0647721
-1904.15  -0.0139042   0.0649800
-1904.20  -0.0140192   0.0651880
-1904.25  -0.0141344   0.0653960
-1904.30  -0.0142500   0.0656042
-1904.35  -0.0143657   0.0658126
-1904.40  -0.0144817   0.0660210
-1904.45  -0.0145979   0.0662297
-1904.50  -0.0147142   0.0664385
-1904.55  -0.0148307   0.0666475
-1904.60  -0.0149472   0.0668568
-1904.65  -0.0150638   0.0670662
-1904.70  -0.0151804   0.0672759
-1904.75  -0.0152970   0.0674859
-1904.80  -0.0154135   0.0676962
-1904.85  -0.0155300   0.0679067
-1904.90  -0.0156463   0.0681176
-1904.95  -0.0157625   0.0683288
-1905.00  -0.0158784   0.0685404
-1905.05  -0.0159942   0.0687524
-1905.10  -0.0161097   0.0689647
-1905.15  -0.0162248   0.0691775
-1905.20  -0.0163397   0.0693907
-1905.25  -0.0164541   0.0696043
-1905.30  -0.0165682   0.0698185
-1905.35  -0.0166818   0.0700331
-1905.40  -0.0167949   0.0702482
-1905.45  -0.0169074   0.0704639
-1905.50  -0.0170194   0.0706801
-1905.55  -0.0171308   0.0708970
-1905.60  -0.0172416   0.0711143
-1905.65  -0.0173516   0.0713323
-1905.70  -0.0174610   0.0715510
-1905.75  -0.0175695   0.0717703
-1905.80  -0.0176773   0.0719902
-1905.85  -0.0177843   0.0722108
-1905.90  -0.0178903   0.0724322
-1905.95  -0.0179955   0.0726542
-1906.00  -0.0180997   0.0728770
-1906.05  -0.0182030   0.0731006
-1906.10  -0.0183052   0.0733249
-1906.15  -0.0184063   0.0735500
-1906.20  -0.0185063   0.0737759
-1906.25  -0.0186053   0.0740026
-1906.30  -0.0187030   0.0742301
-1906.35  -0.0187995   0.0744585
-1906.40  -0.0188948   0.0746877
-1906.45  -0.0189888   0.0749177
-1906.50  -0.0190816   0.0751487
-1906.55  -0.0191729   0.0753805
-1906.60  -0.0192629   0.0756132
-1906.65  -0.0193515   0.0758468
-1906.70  -0.0194386   0.0760814
-1906.75  -0.0195242   0.0763168
-1906.80  -0.0196084   0.0765531
-1906.85  -0.0196910   0.0767904
-1906.90  -0.0197720   0.0770285
-1906.95  -0.0198515   0.0772676
-1907.00  -0.0199293   0.0775076
-1907.05  -0.0200054   0.0777486
-1907.10  -0.0200799   0.0779904
-1907.15  -0.0201527   0.0782332
-1907.20  -0.0202237   0.0784769
-1907.25  -0.0202930   0.0787214
-1907.30  -0.0203604   0.0789669
-1907.35  -0.0204261   0.0792133
-1907.40  -0.0204899   0.0794605
-1907.45  -0.0205519   0.0797086
-1907.50  -0.0206120   0.0799576
-1907.55  -0.0206702   0.0802074
-1907.60  -0.0207265   0.0804580
-1907.65  -0.0207808   0.0807094
-1907.70  -0.0208332   0.0809616
-1907.75  -0.0208836   0.0812146
-1907.80  -0.0209321   0.0814684
-1907.85  -0.0209785   0.0817228
-1907.90  -0.0210229   0.0819780
-1907.95  -0.0210653   0.0822338
-1908.00  -0.0211056   0.0824903
-1908.05  -0.0211439   0.0827474
-1908.10  -0.0211801   0.0830051
-1908.15  -0.0212143   0.0832633
-1908.20  -0.0212463   0.0835221
-1908.25  -0.0212763   0.0837814
-1908.30  -0.0213042   0.0840411
-1908.35  -0.0213299   0.0843012
-1908.40  -0.0213536   0.0845617
-1908.45  -0.0213751   0.0848225
-1908.50  -0.0213945   0.0850837
-1908.55  -0.0214118   0.0853451
-1908.60  -0.0214269   0.0856066
-1908.65  -0.0214400   0.0858684
-1908.70  -0.0214509   0.0861303
-1908.75  -0.0214597   0.0863922
-1908.80  -0.0214664   0.0866541
-1908.85  -0.0214709   0.0869160
-1908.90  -0.0214733   0.0871779
-1908.95  -0.0214737   0.0874396
-1909.00  -0.0214719   0.0877010
-1909.05  -0.0214680   0.0879623
-1909.10  -0.0214620   0.0882232
-1909.15  -0.0214540   0.0884838
-1909.20  -0.0214438   0.0887440
-1909.25  -0.0214316   0.0890036
-1909.30  -0.0214174   0.0892628
-1909.35  -0.0214010   0.0895213
-1909.40  -0.0213827   0.0897792
-1909.45  -0.0213623   0.0900363
-1909.50  -0.0213399   0.0902927
-1909.55  -0.0213155   0.0905482
-1909.60  -0.0212892   0.0908028
-1909.65  -0.0212608   0.0910565
-1909.70  -0.0212305   0.0913091
-1909.75  -0.0211982   0.0915606
-1909.80  -0.0211641   0.0918109
-1909.85  -0.0211280   0.0920600
-1909.90  -0.0210900   0.0923077
-1909.95  -0.0210501   0.0925542
-1910.00  -0.0210084   0.0927991
-1910.05  -0.0209649   0.0930426
-1910.10  -0.0209195   0.0932846
-1910.15  -0.0208723   0.0935248
-1910.20  -0.0208233   0.0937634
-1910.25  -0.0207726   0.0940003
-1910.30  -0.0207201   0.0942353
-1910.35  -0.0206659   0.0944684
-1910.40  -0.0206100   0.0946996
-1910.45  -0.0205524   0.0949287
-1910.50  -0.0204932   0.0951558
-1910.55  -0.0204323   0.0953808
-1910.60  -0.0203697   0.0956035
-1910.65  -0.0203056   0.0958240
-1910.70  -0.0202399   0.0960422
-1910.75  -0.0201727   0.0962579
-1910.80  -0.0201039   0.0964713
-1910.85  -0.0200336   0.0966821
-1910.90  -0.0199618   0.0968904
-1910.95  -0.0198885   0.0970961
-1911.00  -0.0198138   0.0972992
-1911.05  -0.0197377   0.0974995
-1911.10  -0.0196601   0.0976971
-1911.15  -0.0195812   0.0978919
-1911.20  -0.0195009   0.0980838
-1911.25  -0.0194193   0.0982728
-1911.30  -0.0193363   0.0984588
-1911.35  -0.0192521   0.0986419
-1911.40  -0.0191665   0.0988219
-1911.45  -0.0190797   0.0989989
-1911.50  -0.0189917   0.0991728
-1911.55  -0.0189025   0.0993435
-1911.60  -0.0188120   0.0995110
-1911.65  -0.0187204   0.0996753
-1911.70  -0.0186276   0.0998364
-1911.75  -0.0185337   0.0999942
-1911.80  -0.0184387   0.1001487
-1911.85  -0.0183426   0.1002998
-1911.90  -0.0182454   0.1004477
-1911.95  -0.0181471   0.1005921
-1912.00  -0.0180478   0.1007332
-1912.05  -0.0179475   0.1008708
-1912.10  -0.0178461   0.1010050
-1912.15  -0.0177438   0.1011358
-1912.20  -0.0176405   0.1012632
-1912.25  -0.0175362   0.1013871
-1912.30  -0.0174310   0.1015075
-1912.35  -0.0173248   0.1016244
-1912.40  -0.0172178   0.1017379
-1912.45  -0.0171098   0.1018480
-1912.50  -0.0170010   0.1019545
-1912.55  -0.0168913   0.1020576
-1912.60  -0.0167807   0.1021572
-1912.65  -0.0166693   0.1022534
-1912.70  -0.0165571   0.1023462
-1912.75  -0.0164441   0.1024355
-1912.80  -0.0163302   0.1025214
-1912.85  -0.0162156   0.1026040
-1912.90  -0.0161002   0.1026831
-1912.95  -0.0159840   0.1027589
-1913.00  -0.0158670   0.1028314
-1913.05  -0.0157493   0.1029006
-1913.10  -0.0156309   0.1029665
-1913.15  -0.0155117   0.1030291
-1913.20  -0.0153918   0.1030886
-1913.25  -0.0152712   0.1031448
-1913.30  -0.0151499   0.1031979
-1913.35  -0.0150279   0.1032479
-1913.40  -0.0149052   0.1032948
-1913.45  -0.0147818   0.1033387
-1913.50  -0.0146577   0.1033796
-1913.55  -0.0145330   0.1034176
-1913.60  -0.0144076   0.1034527
-1913.65  -0.0142816   0.1034849
-1913.70  -0.0141549   0.1035143
-1913.75  -0.0140275   0.1035409
-1913.80  -0.0138995   0.1035649
-1913.85  -0.0137709   0.1035862
-1913.90  -0.0136416   0.1036049
-1913.95  -0.0135118   0.1036211
-1914.00  -0.0133812   0.1036348
-1914.05  -0.0132501   0.1036460
-1914.10  -0.0131184   0.1036549
-1914.15  -0.0129860   0.1036616
-1914.20  -0.0128530   0.1036659
-1914.25  -0.0127194   0.1036681
-1914.30  -0.0125852   0.1036682
-1914.35  -0.0124504   0.1036663
-1914.40  -0.0123150   0.1036623
-1914.45  -0.0121790   0.1036565
-1914.50  -0.0120424   0.1036488
-1914.55  -0.0119052   0.1036393
-1914.60  -0.0117674   0.1036281
-1914.65  -0.0116290   0.1036153
-1914.70  -0.0114900   0.1036009
-1914.75  -0.0113504   0.1035850
-1914.80  -0.0112102   0.1035676
-1914.85  -0.0110695   0.1035489
-1914.90  -0.0109281   0.1035289
-1914.95  -0.0107862   0.1035077
-1915.00  -0.0106437   0.1034854
-1915.05  -0.0105006   0.1034620
-1915.10  -0.0103569   0.1034375
-1915.15  -0.0102126   0.1034122
-1915.20  -0.0100677   0.1033860
-1915.25  -0.0099223   0.1033590
-1915.30  -0.0097763   0.1033313
-1915.35  -0.0096297   0.1033029
-1915.40  -0.0094826   0.1032739
-1915.45  -0.0093349   0.1032445
-1915.50  -0.0091866   0.1032146
-1915.55  -0.0090377   0.1031844
-1915.60  -0.0088883   0.1031539
-1915.65  -0.0087383   0.1031231
-1915.70  -0.0085878   0.1030922
-1915.75  -0.0084367   0.1030612
-1915.80  -0.0082851   0.1030302
-1915.85  -0.0081329   0.1029992
-1915.90  -0.0079802   0.1029683
-1915.95  -0.0078270   0.1029376
-1916.00  -0.0076733   0.1029072
-1916.05  -0.0075190   0.1028771
-1916.10  -0.0073642   0.1028473
-1916.15  -0.0072089   0.1028180
-1916.20  -0.0070531   0.1027891
-1916.25  -0.0068968   0.1027608
-1916.30  -0.0067400   0.1027331
-1916.35  -0.0065827   0.1027061
-1916.40  -0.0064250   0.1026799
-1916.45  -0.0062668   0.1026544
-1916.50  -0.0061082   0.1026297
-1916.55  -0.0059491   0.1026059
-1916.60  -0.0057896   0.1025831
-1916.65  -0.0056297   0.1025613
-1916.70  -0.0054694   0.1025406
-1916.75  -0.0053086   0.1025209
-1916.80  -0.0051476   0.1025024
-1916.85  -0.0049861   0.1024851
-1916.90  -0.0048243   0.1024691
-1916.95  -0.0046622   0.1024543
-1917.00  -0.0044998   0.1024409
-1917.05  -0.0043370   0.1024288
-1917.10  -0.0041740   0.1024182
-1917.15  -0.0040107   0.1024091
-1917.20  -0.0038472   0.1024014
-1917.25  -0.0036835   0.1023953
-1917.30  -0.0035195   0.1023908
-1917.35  -0.0033554   0.1023879
-1917.40  -0.0031911   0.1023867
-1917.45  -0.0030266   0.1023871
-1917.50  -0.0028621   0.1023893
-1917.55  -0.0026974   0.1023932
-1917.60  -0.0025327   0.1023989
-1917.65  -0.0023679   0.1024064
-1917.70  -0.0022031   0.1024158
-1917.75  -0.0020384   0.1024271
-1917.80  -0.0018736   0.1024402
-1917.85  -0.0017090   0.1024553
-1917.90  -0.0015444   0.1024723
-1917.95  -0.0013800   0.1024913
-1918.00  -0.0012157   0.1025123
-1918.05  -0.0010515   0.1025354
-1918.10  -0.0008877   0.1025604
-1918.15  -0.0007240   0.1025876
-1918.20  -0.0005607   0.1026168
-1918.25  -0.0003976   0.1026481
-1918.30  -0.0002349   0.1026816
-1918.35  -0.0000726   0.1027172
-1918.40   0.0000893   0.1027549
-1918.45   0.0002507   0.1027948
-1918.50   0.0004116   0.1028369
-1918.55   0.0005720   0.1028811
-1918.60   0.0007318   0.1029276
-1918.65   0.0008910   0.1029763
-1918.70   0.0010495   0.1030272
-1918.75   0.0012074   0.1030804
-1918.80   0.0013645   0.1031358
-1918.85   0.0015209   0.1031935
-1918.90   0.0016764   0.1032535
-1918.95   0.0018311   0.1033157
-1919.00   0.0019849   0.1033802
-1919.05   0.0021377   0.1034470
-1919.10   0.0022895   0.1035161
-1919.15   0.0024403   0.1035875
-1919.20   0.0025900   0.1036612
-1919.25   0.0027387   0.1037372
-1919.30   0.0028861   0.1038155
-1919.35   0.0030323   0.1038962
-1919.40   0.0031773   0.1039791
-1919.45   0.0033209   0.1040644
-1919.50   0.0034633   0.1041521
-1919.55   0.0036042   0.1042420
-1919.60   0.0037436   0.1043343
-1919.65   0.0038816   0.1044289
-1919.70   0.0040181   0.1045258
-1919.75   0.0041529   0.1046251
-1919.80   0.0042862   0.1047267
-1919.85   0.0044177   0.1048307
-1919.90   0.0045475   0.1049369
-1919.95   0.0046756   0.1050455
-1920.00   0.0048018   0.1051565
-1920.05   0.0049262   0.1052697
-1920.10   0.0050487   0.1053853
-1920.15   0.0051692   0.1055032
-1920.20   0.0052877   0.1056235
-1920.25   0.0054042   0.1057460
-1920.30   0.0055186   0.1058709
-1920.35   0.0056308   0.1059981
-1920.40   0.0057409   0.1061276
-1920.45   0.0058487   0.1062594
-1920.50   0.0059542   0.1063935
-1920.55   0.0060575   0.1065300
-1920.60   0.0061584   0.1066687
-1920.65   0.0062569   0.1068097
-1920.70   0.0063529   0.1069530
-1920.75   0.0064465   0.1070986
-1920.80   0.0065376   0.1072465
-1920.85   0.0066261   0.1073967
-1920.90   0.0067120   0.1075491
-1920.95   0.0067953   0.1077039
-1921.00   0.0068759   0.1078608
-1921.05   0.0069538   0.1080201
-1921.10   0.0070290   0.1081816
-1921.15   0.0071014   0.1083454
-1921.20   0.0071709   0.1085114
-1921.25   0.0072377   0.1086797
-1921.30   0.0073015   0.1088502
-1921.35   0.0073625   0.1090230
-1921.40   0.0074205   0.1091980
-1921.45   0.0074756   0.1093752
-1921.50   0.0075277   0.1095546
-1921.55   0.0075767   0.1097363
-1921.60   0.0076228   0.1099202
-1921.65   0.0076657   0.1101063
-1921.70   0.0077056   0.1102946
-1921.75   0.0077424   0.1104851
-1921.80   0.0077761   0.1106778
-1921.85   0.0078066   0.1108727
-1921.90   0.0078339   0.1110698
-1921.95   0.0078581   0.1112690
-1922.00   0.0078791   0.1114705
-1922.05   0.0078969   0.1116741
-1922.10   0.0079115   0.1118799
-1922.15   0.0079228   0.1120878
-1922.20   0.0079309   0.1122980
-1922.25   0.0079358   0.1125102
-1922.30   0.0079375   0.1127247
-1922.35   0.0079358   0.1129413
-1922.40   0.0079310   0.1131600
-1922.45   0.0079228   0.1133809
-1922.50   0.0079115   0.1136039
-1922.55   0.0078968   0.1138290
-1922.60   0.0078789   0.1140562
-1922.65   0.0078578   0.1142856
-1922.70   0.0078334   0.1145171
-1922.75   0.0078058   0.1147507
-1922.80   0.0077749   0.1149865
-1922.85   0.0077409   0.1152243
-1922.90   0.0077036   0.1154642
-1922.95   0.0076632   0.1157063
-1923.00   0.0076195   0.1159504
-1923.05   0.0075727   0.1161966
-1923.10   0.0075228   0.1164449
-1923.15   0.0074697   0.1166953
-1923.20   0.0074135   0.1169478
-1923.25   0.0073543   0.1172023
-1923.30   0.0072919   0.1174590
-1923.35   0.0072266   0.1177176
-1923.40   0.0071582   0.1179784
-1923.45   0.0070868   0.1182412
-1923.50   0.0070125   0.1185060
-1923.55   0.0069352   0.1187730
-1923.60   0.0068550   0.1190419
-1923.65   0.0067720   0.1193129
-1923.70   0.0066861   0.1195859
-1923.75   0.0065975   0.1198610
-1923.80   0.0065060   0.1201381
-1923.85   0.0064118   0.1204173
-1923.90   0.0063150   0.1206984
-1923.95   0.0062154   0.1209816
-1924.00   0.0061133   0.1212668
-1924.05   0.0060086   0.1215540
-1924.10   0.0059013   0.1218432
-1924.15   0.0057915   0.1221343
-1924.20   0.0056793   0.1224275
-1924.25   0.0055647   0.1227227
-1924.30   0.0054477   0.1230199
-1924.35   0.0053284   0.1233190
-1924.40   0.0052068   0.1236201
-1924.45   0.0050830   0.1239232
-1924.50   0.0049570   0.1242283
-1924.55   0.0048289   0.1245353
-1924.60   0.0046987   0.1248442
-1924.65   0.0045664   0.1251551
-1924.70   0.0044322   0.1254680
-1924.75   0.0042960   0.1257827
-1924.80   0.0041580   0.1260994
-1924.85   0.0040181   0.1264180
-1924.90   0.0038764   0.1267385
-1924.95   0.0037330   0.1270609
-1925.00   0.0035879   0.1273852
-1925.05   0.0034412   0.1277114
-1925.10   0.0032929   0.1280394
-1925.15   0.0031431   0.1283694
-1925.20   0.0029918   0.1287011
-1925.25   0.0028390   0.1290348
-1925.30   0.0026849   0.1293702
-1925.35   0.0025295   0.1297075
-1925.40   0.0023729   0.1300466
-1925.45   0.0022150   0.1303875
-1925.50   0.0020559   0.1307302
-1925.55   0.0018957   0.1310746
-1925.60   0.0017345   0.1314209
-1925.65   0.0015723   0.1317688
-1925.70   0.0014091   0.1321185
-1925.75   0.0012450   0.1324700
-1925.80   0.0010801   0.1328231
-1925.85   0.0009144   0.1331780
-1925.90   0.0007479   0.1335345
-1925.95   0.0005807   0.1338927
-1926.00   0.0004128   0.1342525
-1926.05   0.0002444   0.1346139
-1926.10   0.0000753   0.1349770
-1926.15  -0.0000942   0.1353416
-1926.20  -0.0002642   0.1357078
-1926.25  -0.0004346   0.1360756
-1926.30  -0.0006053   0.1364449
-1926.35  -0.0007764   0.1368157
-1926.40  -0.0009478   0.1371880
-1926.45  -0.0011194   0.1375618
-1926.50  -0.0012912   0.1379370
-1926.55  -0.0014632   0.1383137
-1926.60  -0.0016352   0.1386917
-1926.65  -0.0018073   0.1390711
-1926.70  -0.0019795   0.1394519
-1926.75  -0.0021516   0.1398340
-1926.80  -0.0023237   0.1402174
-1926.85  -0.0024957   0.1406020
-1926.90  -0.0026675   0.1409879
-1926.95  -0.0028392   0.1413750
-1927.00  -0.0030107   0.1417633
-1927.05  -0.0031819   0.1421528
-1927.10  -0.0033529   0.1425434
-1927.15  -0.0035235   0.1429351
-1927.20  -0.0036938   0.1433278
-1927.25  -0.0038638   0.1437216
-1927.30  -0.0040333   0.1441164
-1927.35  -0.0042024   0.1445122
-1927.40  -0.0043710   0.1449089
-1927.45  -0.0045391   0.1453065
-1927.50  -0.0047067   0.1457050
-1927.55  -0.0048738   0.1461043
-1927.60  -0.0050402   0.1465044
-1927.65  -0.0052061   0.1469053
-1927.70  -0.0053713   0.1473069
-1927.75  -0.0055359   0.1477092
-1927.80  -0.0056998   0.1481122
-1927.85  -0.0058630   0.1485158
-1927.90  -0.0060255   0.1489199
-1927.95  -0.0061872   0.1493246
-1928.00  -0.0063481   0.1497298
-1928.05  -0.0065083   0.1501354
-1928.10  -0.0066677   0.1505415
-1928.15  -0.0068262   0.1509480
-1928.20  -0.0069839   0.1513548
-1928.25  -0.0071407   0.1517619
-1928.30  -0.0072966   0.1521692
-1928.35  -0.0074517   0.1525768
-1928.40  -0.0076058   0.1529846
-1928.45  -0.0077590   0.1533925
-1928.50  -0.0079112   0.1538005
-1928.55  -0.0080625   0.1542085
-1928.60  -0.0082128   0.1546166
-1928.65  -0.0083622   0.1550246
-1928.70  -0.0085105   0.1554325
-1928.75  -0.0086578   0.1558404
-1928.80  -0.0088041   0.1562480
-1928.85  -0.0089493   0.1566555
-1928.90  -0.0090935   0.1570627
-1928.95  -0.0092366   0.1574696
-1929.00  -0.0093787   0.1578762
-1929.05  -0.0095196   0.1582825
-1929.10  -0.0096595   0.1586883
-1929.15  -0.0097982   0.1590936
-1929.20  -0.0099359   0.1594985
-1929.25  -0.0100724   0.1599028
-1929.30  -0.0102077   0.1603065
-1929.35  -0.0103419   0.1607096
-1929.40  -0.0104750   0.1611120
-1929.45  -0.0106069   0.1615138
-1929.50  -0.0107376   0.1619147
-1929.55  -0.0108671   0.1623149
-1929.60  -0.0109954   0.1627143
-1929.65  -0.0111225   0.1631128
-1929.70  -0.0112484   0.1635103
-1929.75  -0.0113731   0.1639070
-1929.80  -0.0114965   0.1643026
-1929.85  -0.0116187   0.1646972
-1929.90  -0.0117396   0.1650908
-1929.95  -0.0118592   0.1654832
-1930.00  -0.0119776   0.1658745
-1930.05  -0.0120946   0.1662647
-1930.10  -0.0122104   0.1666536
-1930.15  -0.0123248   0.1670413
-1930.20  -0.0124380   0.1674277
-1930.25  -0.0125497   0.1678128
-1930.30  -0.0126602   0.1681966
-1930.35  -0.0127692   0.1685789
-1930.40  -0.0128769   0.1689599
-1930.45  -0.0129832   0.1693395
-1930.50  -0.0130881   0.1697175
-1930.55  -0.0131916   0.1700941
-1930.60  -0.0132937   0.1704692
-1930.65  -0.0133943   0.1708427
-1930.70  -0.0134935   0.1712146
-1930.75  -0.0135912   0.1715849
-1930.80  -0.0136874   0.1719536
-1930.85  -0.0137821   0.1723206
-1930.90  -0.0138752   0.1726859
-1930.95  -0.0139669   0.1730496
-1931.00  -0.0140570   0.1734115
-1931.05  -0.0141455   0.1737717
-1931.10  -0.0142324   0.1741301
-1931.15  -0.0143178   0.1744867
-1931.20  -0.0144015   0.1748416
-1931.25  -0.0144835   0.1751946
-1931.30  -0.0145640   0.1755458
-1931.35  -0.0146427   0.1758951
-1931.40  -0.0147197   0.1762426
-1931.45  -0.0147950   0.1765882
-1931.50  -0.0148685   0.1769319
-1931.55  -0.0149403   0.1772737
-1931.60  -0.0150103   0.1776137
-1931.65  -0.0150785   0.1779517
-1931.70  -0.0151449   0.1782877
-1931.75  -0.0152094   0.1786219
-1931.80  -0.0152720   0.1789541
-1931.85  -0.0153328   0.1792844
-1931.90  -0.0153916   0.1796127
-1931.95  -0.0154485   0.1799391
-1932.00  -0.0155034   0.1802635
-1932.05  -0.0155563   0.1805860
-1932.10  -0.0156072   0.1809065
-1932.15  -0.0156560   0.1812251
-1932.20  -0.0157028   0.1815417
-1932.25  -0.0157475   0.1818564
-1932.30  -0.0157900   0.1821691
-1932.35  -0.0158304   0.1824799
-1932.40  -0.0158687   0.1827888
-1932.45  -0.0159047   0.1830958
-1932.50  -0.0159385   0.1834008
-1932.55  -0.0159701   0.1837039
-1932.60  -0.0159994   0.1840051
-1932.65  -0.0160264   0.1843045
-1932.70  -0.0160511   0.1846019
-1932.75  -0.0160734   0.1848975
-1932.80  -0.0160934   0.1851913
-1932.85  -0.0161109   0.1854832
-1932.90  -0.0161260   0.1857732
-1932.95  -0.0161387   0.1860615
-1933.00  -0.0161489   0.1863480
-1933.05  -0.0161565   0.1866327
-1933.10  -0.0161617   0.1869156
-1933.15  -0.0161643   0.1871968
-1933.20  -0.0161643   0.1874762
-1933.25  -0.0161617   0.1877540
-1933.30  -0.0161565   0.1880300
-1933.35  -0.0161487   0.1883044
-1933.40  -0.0161382   0.1885772
-1933.45  -0.0161249   0.1888483
-1933.50  -0.0161090   0.1891178
-1933.55  -0.0160903   0.1893858
-1933.60  -0.0160689   0.1896522
-1933.65  -0.0160447   0.1899170
-1933.70  -0.0160177   0.1901803
-1933.75  -0.0159879   0.1904422
-1933.80  -0.0159553   0.1907025
-1933.85  -0.0159198   0.1909615
-1933.90  -0.0158815   0.1912190
-1933.95  -0.0158403   0.1914751
-1934.00  -0.0157962   0.1917299
-1934.05  -0.0157491   0.1919833
-1934.10  -0.0156992   0.1922354
-1934.15  -0.0156463   0.1924862
-1934.20  -0.0155905   0.1927357
-1934.25  -0.0155317   0.1929840
-1934.30  -0.0154700   0.1932311
-1934.35  -0.0154053   0.1934770
-1934.40  -0.0153376   0.1937217
-1934.45  -0.0152669   0.1939653
-1934.50  -0.0151933   0.1942078
-1934.55  -0.0151166   0.1944491
-1934.60  -0.0150370   0.1946894
-1934.65  -0.0149543   0.1949287
-1934.70  -0.0148687   0.1951669
-1934.75  -0.0147800   0.1954042
-1934.80  -0.0146884   0.1956404
-1934.85  -0.0145938   0.1958758
-1934.90  -0.0144962   0.1961101
-1934.95  -0.0143956   0.1963436
-1935.00  -0.0142921   0.1965762
-1935.05  -0.0141855   0.1968080
-1935.10  -0.0140761   0.1970388
-1935.15  -0.0139637   0.1972689
-1935.20  -0.0138484   0.1974982
-1935.25  -0.0137301   0.1977266
-1935.30  -0.0136090   0.1979543
-1935.35  -0.0134850   0.1981813
-1935.40  -0.0133582   0.1984075
-1935.45  -0.0132285   0.1986330
-1935.50  -0.0130960   0.1988578
-1935.55  -0.0129607   0.1990819
-1935.60  -0.0128226   0.1993053
-1935.65  -0.0126818   0.1995281
-1935.70  -0.0125383   0.1997502
-1935.75  -0.0123921   0.1999717
-1935.80  -0.0122433   0.2001925
-1935.85  -0.0120918   0.2004128
-1935.90  -0.0119378   0.2006324
-1935.95  -0.0117812   0.2008514
-1936.00  -0.0116221   0.2010698
-1936.05  -0.0114605   0.2012876
-1936.10  -0.0112965   0.2015048
-1936.15  -0.0111301   0.2017215
-1936.20  -0.0109614   0.2019375
-1936.25  -0.0107903   0.2021530
-1936.30  -0.0106170   0.2023679
-1936.35  -0.0104415   0.2025822
-1936.40  -0.0102638   0.2027960
-1936.45  -0.0100840   0.2030091
-1936.50  -0.0099021   0.2032216
-1936.55  -0.0097182   0.2034336
-1936.60  -0.0095323   0.2036450
-1936.65  -0.0093445   0.2038557
-1936.70  -0.0091549   0.2040658
-1936.75  -0.0089635   0.2042754
-1936.80  -0.0087703   0.2044842
-1936.85  -0.0085754   0.2046925
-1936.90  -0.0083790   0.2049000
-1936.95  -0.0081809   0.2051069
-1937.00  -0.0079814   0.2053132
-1937.05  -0.0077804   0.2055187
-1937.10  -0.0075780   0.2057235
-1937.15  -0.0073744   0.2059276
-1937.20  -0.0071694   0.2061309
-1937.25  -0.0069633   0.2063335
-1937.30  -0.0067561   0.2065353
-1937.35  -0.0065478   0.2067362
-1937.40  -0.0063385   0.2069364
-1937.45  -0.0061283   0.2071357
-1937.50  -0.0059173   0.2073341
-1937.55  -0.0057054   0.2075316
-1937.60  -0.0054929   0.2077282
-1937.65  -0.0052797   0.2079239
-1937.70  -0.0050659   0.2081186
-1937.75  -0.0048516   0.2083123
-1937.80  -0.0046369   0.2085050
-1937.85  -0.0044218   0.2086966
-1937.90  -0.0042064   0.2088872
-1937.95  -0.0039907   0.2090766
-1938.00  -0.0037749   0.2092649
-1938.05  -0.0035590   0.2094521
-1938.10  -0.0033430   0.2096380
-1938.15  -0.0031271   0.2098228
-1938.20  -0.0029113   0.2100063
-1938.25  -0.0026956   0.2101885
-1938.30  -0.0024802   0.2103693
-1938.35  -0.0022651   0.2105489
-1938.40  -0.0020503   0.2107270
-1938.45  -0.0018360   0.2109038
-1938.50  -0.0016222   0.2110791
-1938.55  -0.0014089   0.2112530
-1938.60  -0.0011962   0.2114253
-1938.65  -0.0009843   0.2115962
-1938.70  -0.0007730   0.2117654
-1938.75  -0.0005625   0.2119331
-1938.80  -0.0003529   0.2120992
-1938.85  -0.0001442   0.2122636
-1938.90   0.0000635   0.2124263
-1938.95   0.0002702   0.2125873
-1939.00   0.0004759   0.2127466
-1939.05   0.0006805   0.2129041
-1939.10   0.0008838   0.2130599
-1939.15   0.0010860   0.2132138
-1939.20   0.0012869   0.2133659
-1939.25   0.0014865   0.2135161
-1939.30   0.0016848   0.2136644
-1939.35   0.0018817   0.2138108
-1939.40   0.0020772   0.2139552
-1939.45   0.0022711   0.2140977
-1939.50   0.0024636   0.2142382
-1939.55   0.0026546   0.2143767
-1939.60   0.0028440   0.2145132
-1939.65   0.0030318   0.2146476
-1939.70   0.0032180   0.2147800
-1939.75   0.0034025   0.2149102
-1939.80   0.0035854   0.2150384
-1939.85   0.0037666   0.2151645
-1939.90   0.0039461   0.2152885
-1939.95   0.0041238   0.2154104
-1940.00   0.0042998   0.2155301
-1940.05   0.0044740   0.2156477
-1940.10   0.0046465   0.2157631
-1940.15   0.0048172   0.2158763
-1940.20   0.0049861   0.2159874
-1940.25   0.0051532   0.2160964
-1940.30   0.0053185   0.2162031
-1940.35   0.0054820   0.2163077
-1940.40   0.0056437   0.2164102
-1940.45   0.0058036   0.2165104
-1940.50   0.0059618   0.2166085
-1940.55   0.0061181   0.2167045
-1940.60   0.0062727   0.2167983
-1940.65   0.0064255   0.2168900
-1940.70   0.0065766   0.2169795
-1940.75   0.0067260   0.2170669
-1940.80   0.0068737   0.2171523
-1940.85   0.0070196   0.2172355
-1940.90   0.0071639   0.2173167
-1940.95   0.0073066   0.2173959
-1941.00   0.0074476   0.2174730
-1941.05   0.0075871   0.2175481
-1941.10   0.0077250   0.2176212
-1941.15   0.0078613   0.2176924
-1941.20   0.0079962   0.2177616
-1941.25   0.0081296   0.2178290
-1941.30   0.0082615   0.2178944
-1941.35   0.0083921   0.2179581
-1941.40   0.0085213   0.2180199
-1941.45   0.0086492   0.2180799
-1941.50   0.0087758   0.2181382
-1941.55   0.0089012   0.2181948
-1941.60   0.0090254   0.2182498
-1941.65   0.0091485   0.2183031
-1941.70   0.0092705   0.2183548
-1941.75   0.0093915   0.2184050
-1941.80   0.0095114   0.2184536
-1941.85   0.0096304   0.2185009
-1941.90   0.0097485   0.2185467
-1941.95   0.0098658   0.2185911
-1942.00   0.0099823   0.2186342
-1942.05   0.0100980   0.2186761
-1942.10   0.0102130   0.2187167
-1942.15   0.0103274   0.2187562
-1942.20   0.0104413   0.2187946
-1942.25   0.0105546   0.2188319
-1942.30   0.0106674   0.2188681
-1942.35   0.0107799   0.2189035
-1942.40   0.0108919   0.2189379
-1942.45   0.0110037   0.2189715
-1942.50   0.0111152   0.2190042
-1942.55   0.0112266   0.2190363
-1942.60   0.0113377   0.2190676
-1942.65   0.0114489   0.2190984
-1942.70   0.0115599   0.2191285
-1942.75   0.0116710   0.2191582
-1942.80   0.0117822   0.2191874
-1942.85   0.0118935   0.2192162
-1942.90   0.0120050   0.2192446
-1942.95   0.0121168   0.2192728
-1943.00   0.0122288   0.2193008
-1943.05   0.0123411   0.2193286
-1943.10   0.0124539   0.2193563
-1943.15   0.0125670   0.2193839
-1943.20   0.0126807   0.2194115
-1943.25   0.0127949   0.2194393
-1943.30   0.0129096   0.2194671
-1943.35   0.0130250   0.2194951
-1943.40   0.0131410   0.2195233
-1943.45   0.0132577   0.2195518
-1943.50   0.0133752   0.2195807
-1943.55   0.0134934   0.2196100
-1943.60   0.0136124   0.2196397
-1943.65   0.0137323   0.2196699
-1943.70   0.0138531   0.2197006
-1943.75   0.0139747   0.2197320
-1943.80   0.0140973   0.2197640
-1943.85   0.0142209   0.2197967
-1943.90   0.0143455   0.2198301
-1943.95   0.0144711   0.2198643
-1944.00   0.0145977   0.2198994
-1944.05   0.0147254   0.2199354
-1944.10   0.0148541   0.2199723
-1944.15   0.0149840   0.2200101
-1944.20   0.0151149   0.2200490
-1944.25   0.0152470   0.2200889
-1944.30   0.0153802   0.2201299
-1944.35   0.0155146   0.2201720
-1944.40   0.0156501   0.2202153
-1944.45   0.0157868   0.2202598
-1944.50   0.0159246   0.2203055
-1944.55   0.0160635   0.2203525
-1944.60   0.0162036   0.2204008
-1944.65   0.0163449   0.2204504
-1944.70   0.0164873   0.2205013
-1944.75   0.0166308   0.2205537
-1944.80   0.0167755   0.2206074
-1944.85   0.0169213   0.2206625
-1944.90   0.0170681   0.2207191
-1944.95   0.0172161   0.2207772
-1945.00   0.0173651   0.2208368
-1945.05   0.0175151   0.2208978
-1945.10   0.0176662   0.2209604
-1945.15   0.0178182   0.2210245
-1945.20   0.0179712   0.2210902
-1945.25   0.0181252   0.2211574
-1945.30   0.0182801   0.2212262
-1945.35   0.0184358   0.2212966
-1945.40   0.0185924   0.2213686
-1945.45   0.0187498   0.2214422
-1945.50   0.0189080   0.2215174
-1945.55   0.0190669   0.2215942
-1945.60   0.0192264   0.2216726
-1945.65   0.0193867   0.2217527
-1945.70   0.0195475   0.2218343
-1945.75   0.0197090   0.2219176
-1945.80   0.0198709   0.2220025
-1945.85   0.0200333   0.2220890
-1945.90   0.0201961   0.2221771
-1945.95   0.0203593   0.2222669
-1946.00   0.0205228   0.2223582
-1946.05   0.0206866   0.2224512
-1946.10   0.0208506   0.2225457
-1946.15   0.0210147   0.2226418
-1946.20   0.0211790   0.2227395
-1946.25   0.0213433   0.2228388
-1946.30   0.0215076   0.2229397
-1946.35   0.0216719   0.2230420
-1946.40   0.0218360   0.2231460
-1946.45   0.0220000   0.2232514
-1946.50   0.0221637   0.2233584
-1946.55   0.0223271   0.2234669
-1946.60   0.0224902   0.2235769
-1946.65   0.0226528   0.2236883
-1946.70   0.0228150   0.2238013
-1946.75   0.0229767   0.2239157
-1946.80   0.0231377   0.2240315
-1946.85   0.0232981   0.2241488
-1946.90   0.0234578   0.2242675
-1946.95   0.0236167   0.2243876
-1947.00   0.0237748   0.2245090
-1947.05   0.0239320   0.2246319
-1947.10   0.0240883   0.2247561
-1947.15   0.0242435   0.2248817
-1947.20   0.0243977   0.2250087
-1947.25   0.0245507   0.2251369
-1947.30   0.0247026   0.2252665
-1947.35   0.0248532   0.2253974
-1947.40   0.0250026   0.2255296
-1947.45   0.0251506   0.2256631
-1947.50   0.0252972   0.2257978
-1947.55   0.0254423   0.2259339
-1947.60   0.0255859   0.2260712
-1947.65   0.0257280   0.2262097
-1947.70   0.0258685   0.2263495
-1947.75   0.0260073   0.2264905
-1947.80   0.0261445   0.2266327
-1947.85   0.0262799   0.2267762
-1947.90   0.0264134   0.2269209
-1947.95   0.0265452   0.2270668
-1948.00   0.0266751   0.2272139
-1948.05   0.0268030   0.2273622
-1948.10   0.0269290   0.2275117
-1948.15   0.0270530   0.2276625
-1948.20   0.0271750   0.2278144
-1948.25   0.0272949   0.2279676
-1948.30   0.0274127   0.2281219
-1948.35   0.0275283   0.2282775
-1948.40   0.0276418   0.2284343
-1948.45   0.0277531   0.2285923
-1948.50   0.0278622   0.2287515
-1948.55   0.0279690   0.2289119
-1948.60   0.0280735   0.2290736
-1948.65   0.0281758   0.2292365
-1948.70   0.0282757   0.2294007
-1948.75   0.0283733   0.2295662
-1948.80   0.0284685   0.2297329
-1948.85   0.0285614   0.2299008
-1948.90   0.0286518   0.2300701
-1948.95   0.0287399   0.2302407
-1949.00   0.0288256   0.2304126
-1949.05   0.0289088   0.2305858
-1949.10   0.0289896   0.2307604
-1949.15   0.0290680   0.2309363
-1949.20   0.0291439   0.2311136
-1949.25   0.0292174   0.2312923
-1949.30   0.0292884   0.2314724
-1949.35   0.0293570   0.2316539
-1949.40   0.0294232   0.2318368
-1949.45   0.0294869   0.2320213
-1949.50   0.0295482   0.2322071
-1949.55   0.0296070   0.2323945
-1949.60   0.0296634   0.2325834
-1949.65   0.0297174   0.2327738
-1949.70   0.0297690   0.2329658
-1949.75   0.0298182   0.2331593
-1949.80   0.0298650   0.2333544
-1949.85   0.0299095   0.2335511
-1949.90   0.0299516   0.2337495
-1949.95   0.0299913   0.2339495
-1950.00   0.0300288   0.2341511
-1950.05   0.0300639   0.2343544
-1950.10   0.0300967   0.2345595
-1950.15   0.0301273   0.2347662
-1950.20   0.0301557   0.2349747
-1950.25   0.0301818   0.2351849
-1950.30   0.0302058   0.2353969
-1950.35   0.0302275   0.2356107
-1950.40   0.0302472   0.2358262
-1950.45   0.0302647   0.2360436
-1950.50   0.0302801   0.2362628
-1950.55   0.0302934   0.2364839
-1950.60   0.0303048   0.2367068
-1950.65   0.0303141   0.2369315
-1950.70   0.0303214   0.2371581
-1950.75   0.0303268   0.2373867
-1950.80   0.0303303   0.2376171
-1950.85   0.0303319   0.2378494
-1950.90   0.0303316   0.2380835
-1950.95   0.0303295   0.2383196
-1951.00   0.0303256   0.2385577
-1951.05   0.0303200   0.2387976
-1951.10   0.0303126   0.2390394
-1951.15   0.0303035   0.2392831
-1951.20   0.0302928   0.2395288
-1951.25   0.0302804   0.2397763
-1951.30   0.0302665   0.2400258
-1951.35   0.0302509   0.2402771
-1951.40   0.0302339   0.2405303
-1951.45   0.0302153   0.2407854
-1951.50   0.0301953   0.2410423
-1951.55   0.0301738   0.2413011
-1951.60   0.0301509   0.2415616
-1951.65   0.0301266   0.2418240
-1951.70   0.0301010   0.2420882
-1951.75   0.0300741   0.2423541
-1951.80   0.0300459   0.2426217
-1951.85   0.0300164   0.2428911
-1951.90   0.0299858   0.2431621
-1951.95   0.0299539   0.2434348
-1952.00   0.0299208   0.2437091
-1952.05   0.0298866   0.2439849
-1952.10   0.0298513   0.2442623
-1952.15   0.0298150   0.2445412
-1952.20   0.0297775   0.2448215
-1952.25   0.0297390   0.2451033
-1952.30   0.0296995   0.2453864
-1952.35   0.0296591   0.2456708
-1952.40   0.0296176   0.2459565
-1952.45   0.0295753   0.2462434
-1952.50   0.0295320   0.2465314
-1952.55   0.0294878   0.2468205
-1952.60   0.0294427   0.2471106
-1952.65   0.0293968   0.2474018
-1952.70   0.0293500   0.2476938
-1952.75   0.0293024   0.2479866
-1952.80   0.0292541   0.2482802
-1952.85   0.0292049   0.2485745
-1952.90   0.0291549   0.2488694
-1952.95   0.0291042   0.2491649
-1953.00   0.0290528   0.2494608
-1953.05   0.0290006   0.2497571
-1953.10   0.0289477   0.2500537
-1953.15   0.0288941   0.2503504
-1953.20   0.0288397   0.2506474
-1953.25   0.0287847   0.2509443
-1953.30   0.0287290   0.2512412
-1953.35   0.0286726   0.2515379
-1953.40   0.0286156   0.2518344
-1953.45   0.0285579   0.2521305
-1953.50   0.0284995   0.2524262
-1953.55   0.0284405   0.2527214
-1953.60   0.0283808   0.2530159
-1953.65   0.0283205   0.2533096
-1953.70   0.0282595   0.2536025
-1953.75   0.0281978   0.2538944
-1953.80   0.0281355   0.2541853
-1953.85   0.0280725   0.2544749
-1953.90   0.0280089   0.2547633
-1953.95   0.0279446   0.2550502
-1954.00   0.0278797   0.2553357
-1954.05   0.0278141   0.2556194
-1954.10   0.0277478   0.2559014
-1954.15   0.0276808   0.2561816
-1954.20   0.0276131   0.2564597
-1954.25   0.0275447   0.2567357
-1954.30   0.0274757   0.2570095
-1954.35   0.0274059   0.2572809
-1954.40   0.0273354   0.2575499
-1954.45   0.0272641   0.2578162
-1954.50   0.0271921   0.2580798
-1954.55   0.0271193   0.2583406
-1954.60   0.0270458   0.2585983
-1954.65   0.0269714   0.2588530
-1954.70   0.0268963   0.2591045
-1954.75   0.0268204   0.2593525
-1954.80   0.0267436   0.2595972
-1954.85   0.0266660   0.2598382
-1954.90   0.0265875   0.2600754
-1954.95   0.0265082   0.2603089
-1955.00   0.0264279   0.2605383
-1955.05   0.0263468   0.2607637
-1955.10   0.0262647   0.2609848
-1955.15   0.0261817   0.2612015
-1955.20   0.0260977   0.2614138
-1955.25   0.0260128   0.2616216
-1955.30   0.0259269   0.2618245
-1955.35   0.0258399   0.2620227
-1955.40   0.0257519   0.2622159
-1955.45   0.0256629   0.2624040
-1955.50   0.0255728   0.2625870
-1955.55   0.0254816   0.2627646
-1955.60   0.0253893   0.2629369
-1955.65   0.0252959   0.2631036
-1955.70   0.0252014   0.2632646
-1955.75   0.0251056   0.2634199
-1955.80   0.0250088   0.2635694
-1955.85   0.0249107   0.2637129
-1955.90   0.0248113   0.2638503
-1955.95   0.0247108   0.2639816
-1956.00   0.0246090   0.2641065
-1956.05   0.0245059   0.2642252
-1956.10   0.0244015   0.2643373
-1956.15   0.0242959   0.2644429
-1956.20   0.0241889   0.2645419
-1956.25   0.0240805   0.2646341
-1956.30   0.0239708   0.2647195
-1956.35   0.0238597   0.2647979
-1956.40   0.0237473   0.2648694
-1956.45   0.0236334   0.2649339
-1956.50   0.0235181   0.2649912
-1956.55   0.0234013   0.2650413
-1956.60   0.0232831   0.2650841
-1956.65   0.0231634   0.2651195
-1956.70   0.0230423   0.2651476
-1956.75   0.0229196   0.2651682
-1956.80   0.0227955   0.2651812
-1956.85   0.0226698   0.2651867
-1956.90   0.0225426   0.2651845
-1956.95   0.0224138   0.2651747
-1957.00   0.0222835   0.2651571
-1957.05   0.0221516   0.2651318
-1957.10   0.0220182   0.2650987
-1957.15   0.0218831   0.2650577
-1957.20   0.0217465   0.2650089
-1957.25   0.0216083   0.2649522
-1957.30   0.0214684   0.2648876
-1957.35   0.0213270   0.2648150
-1957.40   0.0211840   0.2647345
-1957.45   0.0210393   0.2646460
-1957.50   0.0208930   0.2645496
-1957.55   0.0207451   0.2644452
-1957.60   0.0205955   0.2643329
-1957.65   0.0204444   0.2642125
-1957.70   0.0202916   0.2640842
-1957.75   0.0201371   0.2639480
-1957.80   0.0199811   0.2638038
-1957.85   0.0198234   0.2636518
-1957.90   0.0196641   0.2634918
-1957.95   0.0195032   0.2633239
-1958.00   0.0193407   0.2631483
-1958.05   0.0191765   0.2629648
-1958.10   0.0190108   0.2627736
-1958.15   0.0188435   0.2625746
-1958.20   0.0186746   0.2623680
-1958.25   0.0185041   0.2621537
-1958.30   0.0183320   0.2619319
-1958.35   0.0181584   0.2617025
-1958.40   0.0179833   0.2614657
-1958.45   0.0178067   0.2612215
-1958.50   0.0176285   0.2609699
-1958.55   0.0174488   0.2607112
-1958.60   0.0172677   0.2604452
-1958.65   0.0170851   0.2601721
-1958.70   0.0169010   0.2598920
-1958.75   0.0167155   0.2596050
-1958.80   0.0165286   0.2593111
-1958.85   0.0163404   0.2590105
-1958.90   0.0161507   0.2587032
-1958.95   0.0159598   0.2583893
-1959.00   0.0157675   0.2580690
-1959.05   0.0155739   0.2577423
-1959.10   0.0153791   0.2574093
-1959.15   0.0151830   0.2570702
-1959.20   0.0149857   0.2567251
-1959.25   0.0147872   0.2563741
-1959.30   0.0145876   0.2560173
-1959.35   0.0143868   0.2556547
-1959.40   0.0141850   0.2552867
-1959.45   0.0139821   0.2549132
-1959.50   0.0137781   0.2545344
-1959.55   0.0135732   0.2541505
-1959.60   0.0133673   0.2537615
-1959.65   0.0131605   0.2533676
-1959.70   0.0129528   0.2529689
-1959.75   0.0127443   0.2525657
-1959.80   0.0125349   0.2521579
-1959.85   0.0123248   0.2517458
-1959.90   0.0121139   0.2513295
-1959.95   0.0119023   0.2509092
-1960.00   0.0116901   0.2504849
-1960.05   0.0114773   0.2500569
-1960.10   0.0112639   0.2496253
-1960.15   0.0110500   0.2491902
-1960.20   0.0108356   0.2487519
-1960.25   0.0106207   0.2483104
-1960.30   0.0104055   0.2478659
-1960.35   0.0101899   0.2474186
-1960.40   0.0099740   0.2469685
-1960.45   0.0097579   0.2465160
-1960.50   0.0095415   0.2460611
-1960.55   0.0093250   0.2456040
-1960.60   0.0091084   0.2451449
-1960.65   0.0088917   0.2446838
-1960.70   0.0086750   0.2442210
-1960.75   0.0084583   0.2437567
-1960.80   0.0082417   0.2432909
-1960.85   0.0080252   0.2428239
-1960.90   0.0078090   0.2423558
-1960.95   0.0075929   0.2418867
-1961.00   0.0073771   0.2414169
-1961.05   0.0071617   0.2409464
-1961.10   0.0069466   0.2404755
-1961.15   0.0067320   0.2400042
-1961.20   0.0065179   0.2395328
-1961.25   0.0063043   0.2390614
-1961.30   0.0060913   0.2385902
-1961.35   0.0058789   0.2381192
-1961.40   0.0056672   0.2376487
-1961.45   0.0054563   0.2371788
-1961.50   0.0052461   0.2367097
-1961.55   0.0050368   0.2362414
-1961.60   0.0048284   0.2357742
-1961.65   0.0046210   0.2353082
-1961.70   0.0044145   0.2348435
-1961.75   0.0042091   0.2343803
-1961.80   0.0040048   0.2339188
-1961.85   0.0038016   0.2334589
-1961.90   0.0035997   0.2330010
-1961.95   0.0033989   0.2325451
-1962.00   0.0031995   0.2320913
-1962.05   0.0030014   0.2316398
-1962.10   0.0028048   0.2311908
-1962.15   0.0026095   0.2307442
-1962.20   0.0024157   0.2303004
-1962.25   0.0022235   0.2298593
-1962.30   0.0020329   0.2294211
-1962.35   0.0018438   0.2289860
-1962.40   0.0016565   0.2285540
-1962.45   0.0014709   0.2281252
-1962.50   0.0012870   0.2276998
-1962.55   0.0011049   0.2272778
-1962.60   0.0009246   0.2268595
-1962.65   0.0007463   0.2264448
-1962.70   0.0005699   0.2260339
-1962.75   0.0003954   0.2256268
-1962.80   0.0002229   0.2252237
-1962.85   0.0000525   0.2248247
-1962.90  -0.0001158   0.2244298
-1962.95  -0.0002821   0.2240392
-1963.00  -0.0004462   0.2236528
-1963.05  -0.0006081   0.2232709
-1963.10  -0.0007677   0.2228935
-1963.15  -0.0009252   0.2225206
-1963.20  -0.0010803   0.2221523
-1963.25  -0.0012331   0.2217888
-1963.30  -0.0013836   0.2214300
-1963.35  -0.0015317   0.2210760
-1963.40  -0.0016774   0.2207269
-1963.45  -0.0018207   0.2203828
-1963.50  -0.0019615   0.2200437
-1963.55  -0.0020999   0.2197097
-1963.60  -0.0022357   0.2193808
-1963.65  -0.0023691   0.2190570
-1963.70  -0.0024998   0.2187385
-1963.75  -0.0026280   0.2184252
-1963.80  -0.0027537   0.2181173
-1963.85  -0.0028767   0.2178146
-1963.90  -0.0029971   0.2175174
-1963.95  -0.0031148   0.2172255
-1964.00  -0.0032300   0.2169391
-1964.05  -0.0033424   0.2166582
-1964.10  -0.0034522   0.2163828
-1964.15  -0.0035592   0.2161129
-1964.20  -0.0036636   0.2158485
-1964.25  -0.0037652   0.2155897
-1964.30  -0.0038642   0.2153364
-1964.35  -0.0039604   0.2150888
-1964.40  -0.0040539   0.2148468
-1964.45  -0.0041446   0.2146103
-1964.50  -0.0042326   0.2143795
-1964.55  -0.0043178   0.2141544
-1964.60  -0.0044003   0.2139348
-1964.65  -0.0044800   0.2137209
-1964.70  -0.0045570   0.2135126
-1964.75  -0.0046312   0.2133100
-1964.80  -0.0047027   0.2131129
-1964.85  -0.0047714   0.2129215
-1964.90  -0.0048374   0.2127357
-1964.95  -0.0049006   0.2125555
-1965.00  -0.0049611   0.2123809
-1965.05  -0.0050189   0.2122119
-1965.10  -0.0050739   0.2120484
-1965.15  -0.0051263   0.2118905
-1965.20  -0.0051759   0.2117381
-1965.25  -0.0052228   0.2115912
-1965.30  -0.0052670   0.2114497
-1965.35  -0.0053086   0.2113138
-1965.40  -0.0053475   0.2111832
-1965.45  -0.0053837   0.2110581
-1965.50  -0.0054173   0.2109383
-1965.55  -0.0054482   0.2108239
-1965.60  -0.0054765   0.2107148
-1965.65  -0.0055023   0.2106110
-1965.70  -0.0055254   0.2105124
-1965.75  -0.0055460   0.2104191
-1965.80  -0.0055640   0.2103310
-1965.85  -0.0055794   0.2102480
-1965.90  -0.0055924   0.2101701
-1965.95  -0.0056028   0.2100973
-1966.00  -0.0056108   0.2100295
-1966.05  -0.0056163   0.2099667
-1966.10  -0.0056193   0.2099089
-1966.15  -0.0056199   0.2098560
-1966.20  -0.0056181   0.2098079
-1966.25  -0.0056139   0.2097647
-1966.30  -0.0056073   0.2097263
-1966.35  -0.0055983   0.2096926
-1966.40  -0.0055871   0.2096636
-1966.45  -0.0055735   0.2096393
-1966.50  -0.0055576   0.2096195
-1966.55  -0.0055394   0.2096044
-1966.60  -0.0055190   0.2095937
-1966.65  -0.0054964   0.2095875
-1966.70  -0.0054715   0.2095857
-1966.75  -0.0054445   0.2095882
-1966.80  -0.0054153   0.2095951
-1966.85  -0.0053839   0.2096062
-1966.90  -0.0053505   0.2096216
-1966.95  -0.0053149   0.2096411
-1967.00  -0.0052772   0.2096648
-1967.05  -0.0052375   0.2096925
-1967.10  -0.0051957   0.2097242
-1967.15  -0.0051519   0.2097600
-1967.20  -0.0051061   0.2097996
-1967.25  -0.0050584   0.2098431
-1967.30  -0.0050087   0.2098904
-1967.35  -0.0049570   0.2099415
-1967.40  -0.0049034   0.2099962
-1967.45  -0.0048480   0.2100547
-1967.50  -0.0047906   0.2101168
-1967.55  -0.0047314   0.2101824
-1967.60  -0.0046704   0.2102516
-1967.65  -0.0046076   0.2103242
-1967.70  -0.0045429   0.2104003
-1967.75  -0.0044765   0.2104797
-1967.80  -0.0044083   0.2105624
-1967.85  -0.0043384   0.2106484
-1967.90  -0.0042668   0.2107376
-1967.95  -0.0041935   0.2108300
-1968.00  -0.0041185   0.2109255
-1968.05  -0.0040418   0.2110241
-1968.10  -0.0039635   0.2111257
-1968.15  -0.0038836   0.2112303
-1968.20  -0.0038020   0.2113378
-1968.25  -0.0037189   0.2114483
-1968.30  -0.0036342   0.2115615
+1900.00  -0.0072169   0.0476688
+1900.05  -0.0072561   0.0478737
+1900.10  -0.0072962   0.0480788
+1900.15  -0.0073373   0.0482843
+1900.20  -0.0073794   0.0484901
+1900.25  -0.0074225   0.0486961
+1900.30  -0.0074665   0.0489025
+1900.35  -0.0075116   0.0491091
+1900.40  -0.0075577   0.0493160
+1900.45  -0.0076048   0.0495231
+1900.50  -0.0076529   0.0497305
+1900.55  -0.0077020   0.0499381
+1900.60  -0.0077522   0.0501460
+1900.65  -0.0078034   0.0503540
+1900.70  -0.0078557   0.0505622
+1900.75  -0.0079090   0.0507707
+1900.80  -0.0079633   0.0509793
+1900.85  -0.0080187   0.0511880
+1900.90  -0.0080752   0.0513970
+1900.95  -0.0081327   0.0516060
+1901.00  -0.0081913   0.0518152
+1901.05  -0.0082510   0.0520246
+1901.10  -0.0083117   0.0522340
+1901.15  -0.0083735   0.0524436
+1901.20  -0.0084364   0.0526533
+1901.25  -0.0085004   0.0528630
+1901.30  -0.0085655   0.0530729
+1901.35  -0.0086316   0.0532828
+1901.40  -0.0086988   0.0534927
+1901.45  -0.0087671   0.0537027
+1901.50  -0.0088365   0.0539128
+1901.55  -0.0089070   0.0541229
+1901.60  -0.0089786   0.0543330
+1901.65  -0.0090513   0.0545431
+1901.70  -0.0091250   0.0547532
+1901.75  -0.0091998   0.0549634
+1901.80  -0.0092757   0.0551735
+1901.85  -0.0093527   0.0553836
+1901.90  -0.0094308   0.0555937
+1901.95  -0.0095099   0.0558038
+1902.00  -0.0095901   0.0560138
+1902.05  -0.0096713   0.0562238
+1902.10  -0.0097537   0.0564337
+1902.15  -0.0098370   0.0566436
+1902.20  -0.0099214   0.0568535
+1902.25  -0.0100069   0.0570632
+1902.30  -0.0100934   0.0572729
+1902.35  -0.0101809   0.0574826
+1902.40  -0.0102694   0.0576921
+1902.45  -0.0103589   0.0579016
+1902.50  -0.0104495   0.0581110
+1902.55  -0.0105410   0.0583203
+1902.60  -0.0106335   0.0585295
+1902.65  -0.0107270   0.0587386
+1902.70  -0.0108214   0.0589477
+1902.75  -0.0109168   0.0591566
+1902.80  -0.0110131   0.0593655
+1902.85  -0.0111103   0.0595742
+1902.90  -0.0112085   0.0597829
+1902.95  -0.0113075   0.0599914
+1903.00  -0.0114074   0.0601999
+1903.05  -0.0115082   0.0604083
+1903.10  -0.0116098   0.0606166
+1903.15  -0.0117123   0.0608248
+1903.20  -0.0118155   0.0610330
+1903.25  -0.0119196   0.0612410
+1903.30  -0.0120244   0.0614490
+1903.35  -0.0121300   0.0616569
+1903.40  -0.0122363   0.0618648
+1903.45  -0.0123434   0.0620726
+1903.50  -0.0124511   0.0622803
+1903.55  -0.0125595   0.0624880
+1903.60  -0.0126686   0.0626957
+1903.65  -0.0127783   0.0629033
+1903.70  -0.0128886   0.0631109
+1903.75  -0.0129995   0.0633185
+1903.80  -0.0131109   0.0635261
+1903.85  -0.0132229   0.0637337
+1903.90  -0.0133354   0.0639413
+1903.95  -0.0134483   0.0641490
+1904.00  -0.0135617   0.0643567
+1904.05  -0.0136756   0.0645644
+1904.10  -0.0137898   0.0647722
+1904.15  -0.0139044   0.0649801
+1904.20  -0.0140193   0.0651881
+1904.25  -0.0141346   0.0653961
+1904.30  -0.0142501   0.0656043
+1904.35  -0.0143659   0.0658127
+1904.40  -0.0144819   0.0660211
+1904.45  -0.0145980   0.0662298
+1904.50  -0.0147144   0.0664386
+1904.55  -0.0148308   0.0666476
+1904.60  -0.0149474   0.0668569
+1904.65  -0.0150639   0.0670663
+1904.70  -0.0151805   0.0672760
+1904.75  -0.0152971   0.0674860
+1904.80  -0.0154137   0.0676963
+1904.85  -0.0155301   0.0679068
+1904.90  -0.0156464   0.0681177
+1904.95  -0.0157626   0.0683289
+1905.00  -0.0158786   0.0685405
+1905.05  -0.0159943   0.0687525
+1905.10  -0.0161098   0.0689648
+1905.15  -0.0162250   0.0691776
+1905.20  -0.0163398   0.0693908
+1905.25  -0.0164543   0.0696044
+1905.30  -0.0165683   0.0698186
+1905.35  -0.0166819   0.0700332
+1905.40  -0.0167950   0.0702483
+1905.45  -0.0169076   0.0704640
+1905.50  -0.0170196   0.0706802
+1905.55  -0.0171310   0.0708971
+1905.60  -0.0172417   0.0711144
+1905.65  -0.0173518   0.0713325
+1905.70  -0.0174611   0.0715511
+1905.75  -0.0175697   0.0717704
+1905.80  -0.0176775   0.0719903
+1905.85  -0.0177845   0.0722110
+1905.90  -0.0178905   0.0724323
+1905.95  -0.0179957   0.0726543
+1906.00  -0.0180999   0.0728771
+1906.05  -0.0182031   0.0731007
+1906.10  -0.0183053   0.0733250
+1906.15  -0.0184065   0.0735501
+1906.20  -0.0185065   0.0737760
+1906.25  -0.0186054   0.0740027
+1906.30  -0.0187032   0.0742302
+1906.35  -0.0187997   0.0744586
+1906.40  -0.0188950   0.0746878
+1906.45  -0.0189890   0.0749179
+1906.50  -0.0190817   0.0751488
+1906.55  -0.0191731   0.0753806
+1906.60  -0.0192631   0.0756134
+1906.65  -0.0193516   0.0758470
+1906.70  -0.0194388   0.0760815
+1906.75  -0.0195244   0.0763169
+1906.80  -0.0196086   0.0765532
+1906.85  -0.0196912   0.0767905
+1906.90  -0.0197722   0.0770287
+1906.95  -0.0198516   0.0772678
+1907.00  -0.0199295   0.0775078
+1907.05  -0.0200056   0.0777487
+1907.10  -0.0200801   0.0779906
+1907.15  -0.0201528   0.0782333
+1907.20  -0.0202239   0.0784770
+1907.25  -0.0202931   0.0787216
+1907.30  -0.0203606   0.0789670
+1907.35  -0.0204263   0.0792134
+1907.40  -0.0204901   0.0794607
+1907.45  -0.0205521   0.0797088
+1907.50  -0.0206122   0.0799577
+1907.55  -0.0206704   0.0802075
+1907.60  -0.0207267   0.0804582
+1907.65  -0.0207810   0.0807096
+1907.70  -0.0208334   0.0809618
+1907.75  -0.0208838   0.0812148
+1907.80  -0.0209322   0.0814685
+1907.85  -0.0209787   0.0817230
+1907.90  -0.0210231   0.0819782
+1907.95  -0.0210655   0.0822340
+1908.00  -0.0211058   0.0824905
+1908.05  -0.0211441   0.0827476
+1908.10  -0.0211803   0.0830053
+1908.15  -0.0212144   0.0832635
+1908.20  -0.0212465   0.0835223
+1908.25  -0.0212764   0.0837816
+1908.30  -0.0213043   0.0840413
+1908.35  -0.0213301   0.0843014
+1908.40  -0.0213537   0.0845619
+1908.45  -0.0213752   0.0848227
+1908.50  -0.0213946   0.0850839
+1908.55  -0.0214119   0.0853452
+1908.60  -0.0214271   0.0856068
+1908.65  -0.0214401   0.0858686
+1908.70  -0.0214510   0.0861305
+1908.75  -0.0214598   0.0863924
+1908.80  -0.0214665   0.0866543
+1908.85  -0.0214710   0.0869162
+1908.90  -0.0214735   0.0871781
+1908.95  -0.0214738   0.0874398
+1909.00  -0.0214720   0.0877013
+1909.05  -0.0214681   0.0879625
+1909.10  -0.0214622   0.0882234
+1909.15  -0.0214541   0.0884840
+1909.20  -0.0214439   0.0887442
+1909.25  -0.0214317   0.0890038
+1909.30  -0.0214175   0.0892630
+1909.35  -0.0214012   0.0895215
+1909.40  -0.0213828   0.0897794
+1909.45  -0.0213624   0.0900366
+1909.50  -0.0213400   0.0902929
+1909.55  -0.0213156   0.0905485
+1909.60  -0.0212893   0.0908031
+1909.65  -0.0212609   0.0910567
+1909.70  -0.0212306   0.0913093
+1909.75  -0.0211983   0.0915608
+1909.80  -0.0211642   0.0918111
+1909.85  -0.0211281   0.0920602
+1909.90  -0.0210901   0.0923080
+1909.95  -0.0210502   0.0925544
+1910.00  -0.0210085   0.0927994
+1910.05  -0.0209649   0.0930429
+1910.10  -0.0209196   0.0932848
+1910.15  -0.0208724   0.0935251
+1910.20  -0.0208234   0.0937637
+1910.25  -0.0207727   0.0940005
+1910.30  -0.0207202   0.0942355
+1910.35  -0.0206660   0.0944686
+1910.40  -0.0206101   0.0946998
+1910.45  -0.0205525   0.0949290
+1910.50  -0.0204932   0.0951560
+1910.55  -0.0204323   0.0953810
+1910.60  -0.0203698   0.0956037
+1910.65  -0.0203057   0.0958242
+1910.70  -0.0202400   0.0960424
+1910.75  -0.0201727   0.0962581
+1910.80  -0.0201039   0.0964715
+1910.85  -0.0200336   0.0966823
+1910.90  -0.0199618   0.0968906
+1910.95  -0.0198885   0.0970963
+1911.00  -0.0198138   0.0972994
+1911.05  -0.0197377   0.0974997
+1911.10  -0.0196601   0.0976973
+1911.15  -0.0195812   0.0978921
+1911.20  -0.0195009   0.0980840
+1911.25  -0.0194193   0.0982730
+1911.30  -0.0193363   0.0984590
+1911.35  -0.0192521   0.0986421
+1911.40  -0.0191665   0.0988221
+1911.45  -0.0190797   0.0989991
+1911.50  -0.0189917   0.0991729
+1911.55  -0.0189024   0.0993437
+1911.60  -0.0188120   0.0995112
+1911.65  -0.0187204   0.0996755
+1911.70  -0.0186276   0.0998366
+1911.75  -0.0185337   0.0999944
+1911.80  -0.0184387   0.1001488
+1911.85  -0.0183425   0.1003000
+1911.90  -0.0182453   0.1004478
+1911.95  -0.0181471   0.1005923
+1912.00  -0.0180478   0.1007333
+1912.05  -0.0179474   0.1008710
+1912.10  -0.0178461   0.1010052
+1912.15  -0.0177437   0.1011360
+1912.20  -0.0176404   0.1012633
+1912.25  -0.0175361   0.1013872
+1912.30  -0.0174309   0.1015076
+1912.35  -0.0173248   0.1016246
+1912.40  -0.0172177   0.1017381
+1912.45  -0.0171098   0.1018481
+1912.50  -0.0170009   0.1019546
+1912.55  -0.0168912   0.1020577
+1912.60  -0.0167806   0.1021574
+1912.65  -0.0166692   0.1022535
+1912.70  -0.0165570   0.1023463
+1912.75  -0.0164440   0.1024356
+1912.80  -0.0163301   0.1025215
+1912.85  -0.0162155   0.1026041
+1912.90  -0.0161000   0.1026832
+1912.95  -0.0159838   0.1027590
+1913.00  -0.0158669   0.1028315
+1913.05  -0.0157492   0.1029007
+1913.10  -0.0156307   0.1029666
+1913.15  -0.0155115   0.1030292
+1913.20  -0.0153916   0.1030886
+1913.25  -0.0152710   0.1031449
+1913.30  -0.0151497   0.1031980
+1913.35  -0.0150277   0.1032480
+1913.40  -0.0149050   0.1032949
+1913.45  -0.0147816   0.1033388
+1913.50  -0.0146575   0.1033797
+1913.55  -0.0145328   0.1034176
+1913.60  -0.0144074   0.1034527
+1913.65  -0.0142814   0.1034849
+1913.70  -0.0141547   0.1035143
+1913.75  -0.0140273   0.1035409
+1913.80  -0.0138993   0.1035649
+1913.85  -0.0137707   0.1035862
+1913.90  -0.0136414   0.1036049
+1913.95  -0.0135115   0.1036211
+1914.00  -0.0133810   0.1036347
+1914.05  -0.0132499   0.1036460
+1914.10  -0.0131181   0.1036549
+1914.15  -0.0129858   0.1036615
+1914.20  -0.0128528   0.1036659
+1914.25  -0.0127192   0.1036681
+1914.30  -0.0125850   0.1036682
+1914.35  -0.0124502   0.1036662
+1914.40  -0.0123148   0.1036623
+1914.45  -0.0121787   0.1036564
+1914.50  -0.0120421   0.1036487
+1914.55  -0.0119049   0.1036392
+1914.60  -0.0117671   0.1036280
+1914.65  -0.0116287   0.1036152
+1914.70  -0.0114897   0.1036008
+1914.75  -0.0113501   0.1035849
+1914.80  -0.0112099   0.1035675
+1914.85  -0.0110692   0.1035488
+1914.90  -0.0109278   0.1035288
+1914.95  -0.0107859   0.1035076
+1915.00  -0.0106433   0.1034853
+1915.05  -0.0105002   0.1034618
+1915.10  -0.0103565   0.1034374
+1915.15  -0.0102123   0.1034120
+1915.20  -0.0100674   0.1033858
+1915.25  -0.0099220   0.1033588
+1915.30  -0.0097760   0.1033311
+1915.35  -0.0096294   0.1033027
+1915.40  -0.0094822   0.1032738
+1915.45  -0.0093345   0.1032443
+1915.50  -0.0091862   0.1032144
+1915.55  -0.0090374   0.1031842
+1915.60  -0.0088879   0.1031537
+1915.65  -0.0087380   0.1031229
+1915.70  -0.0085874   0.1030920
+1915.75  -0.0084364   0.1030610
+1915.80  -0.0082847   0.1030300
+1915.85  -0.0081326   0.1029990
+1915.90  -0.0079799   0.1029681
+1915.95  -0.0078266   0.1029374
+1916.00  -0.0076729   0.1029070
+1916.05  -0.0075186   0.1028768
+1916.10  -0.0073638   0.1028470
+1916.15  -0.0072085   0.1028177
+1916.20  -0.0070527   0.1027888
+1916.25  -0.0068964   0.1027606
+1916.30  -0.0067396   0.1027329
+1916.35  -0.0065823   0.1027059
+1916.40  -0.0064246   0.1026796
+1916.45  -0.0062664   0.1026541
+1916.50  -0.0061077   0.1026294
+1916.55  -0.0059487   0.1026056
+1916.60  -0.0057892   0.1025828
+1916.65  -0.0056292   0.1025610
+1916.70  -0.0054689   0.1025402
+1916.75  -0.0053082   0.1025206
+1916.80  -0.0051471   0.1025021
+1916.85  -0.0049857   0.1024848
+1916.90  -0.0048239   0.1024687
+1916.95  -0.0046618   0.1024539
+1917.00  -0.0044993   0.1024405
+1917.05  -0.0043366   0.1024285
+1917.10  -0.0041736   0.1024178
+1917.15  -0.0040103   0.1024087
+1917.20  -0.0038468   0.1024010
+1917.25  -0.0036830   0.1023949
+1917.30  -0.0035190   0.1023904
+1917.35  -0.0033549   0.1023875
+1917.40  -0.0031906   0.1023862
+1917.45  -0.0030262   0.1023867
+1917.50  -0.0028616   0.1023888
+1917.55  -0.0026970   0.1023928
+1917.60  -0.0025322   0.1023985
+1917.65  -0.0023675   0.1024060
+1917.70  -0.0022027   0.1024153
+1917.75  -0.0020379   0.1024266
+1917.80  -0.0018732   0.1024397
+1917.85  -0.0017085   0.1024548
+1917.90  -0.0015439   0.1024718
+1917.95  -0.0013795   0.1024908
+1918.00  -0.0012152   0.1025118
+1918.05  -0.0010511   0.1025349
+1918.10  -0.0008872   0.1025599
+1918.15  -0.0007236   0.1025871
+1918.20  -0.0005602   0.1026163
+1918.25  -0.0003972   0.1026476
+1918.30  -0.0002345   0.1026810
+1918.35  -0.0000722   0.1027166
+1918.40   0.0000897   0.1027543
+1918.45   0.0002511   0.1027942
+1918.50   0.0004121   0.1028363
+1918.55   0.0005724   0.1028806
+1918.60   0.0007323   0.1029270
+1918.65   0.0008915   0.1029757
+1918.70   0.0010500   0.1030267
+1918.75   0.0012079   0.1030798
+1918.80   0.0013650   0.1031352
+1918.85   0.0015213   0.1031929
+1918.90   0.0016769   0.1032529
+1918.95   0.0018315   0.1033151
+1919.00   0.0019853   0.1033796
+1919.05   0.0021381   0.1034464
+1919.10   0.0022900   0.1035155
+1919.15   0.0024408   0.1035869
+1919.20   0.0025905   0.1036605
+1919.25   0.0027391   0.1037366
+1919.30   0.0028865   0.1038149
+1919.35   0.0030328   0.1038955
+1919.40   0.0031777   0.1039785
+1919.45   0.0033214   0.1040638
+1919.50   0.0034637   0.1041514
+1919.55   0.0036046   0.1042413
+1919.60   0.0037441   0.1043336
+1919.65   0.0038821   0.1044282
+1919.70   0.0040185   0.1045252
+1919.75   0.0041534   0.1046244
+1919.80   0.0042866   0.1047260
+1919.85   0.0044181   0.1048300
+1919.90   0.0045480   0.1049362
+1919.95   0.0046760   0.1050448
+1920.00   0.0048023   0.1051558
+1920.05   0.0049267   0.1052690
+1920.10   0.0050491   0.1053846
+1920.15   0.0051696   0.1055025
+1920.20   0.0052881   0.1056228
+1920.25   0.0054046   0.1057453
+1920.30   0.0055190   0.1058702
+1920.35   0.0056312   0.1059974
+1920.40   0.0057413   0.1061269
+1920.45   0.0058491   0.1062587
+1920.50   0.0059547   0.1063928
+1920.55   0.0060579   0.1065292
+1920.60   0.0061588   0.1066680
+1920.65   0.0062573   0.1068090
+1920.70   0.0063534   0.1069523
+1920.75   0.0064469   0.1070979
+1920.80   0.0065380   0.1072458
+1920.85   0.0066265   0.1073959
+1920.90   0.0067124   0.1075484
+1920.95   0.0067957   0.1077031
+1921.00   0.0068763   0.1078601
+1921.05   0.0069542   0.1080194
+1921.10   0.0070294   0.1081809
+1921.15   0.0071018   0.1083447
+1921.20   0.0071713   0.1085107
+1921.25   0.0072381   0.1086790
+1921.30   0.0073019   0.1088495
+1921.35   0.0073629   0.1090222
+1921.40   0.0074209   0.1091972
+1921.45   0.0074760   0.1093744
+1921.50   0.0075281   0.1095539
+1921.55   0.0075771   0.1097356
+1921.60   0.0076232   0.1099194
+1921.65   0.0076661   0.1101055
+1921.70   0.0077060   0.1102938
+1921.75   0.0077428   0.1104843
+1921.80   0.0077765   0.1106771
+1921.85   0.0078070   0.1108720
+1921.90   0.0078343   0.1110690
+1921.95   0.0078585   0.1112683
+1922.00   0.0078795   0.1114698
+1922.05   0.0078973   0.1116734
+1922.10   0.0079119   0.1118792
+1922.15   0.0079232   0.1120871
+1922.20   0.0079314   0.1122973
+1922.25   0.0079362   0.1125095
+1922.30   0.0079379   0.1127240
+1922.35   0.0079362   0.1129406
+1922.40   0.0079314   0.1131593
+1922.45   0.0079232   0.1133802
+1922.50   0.0079119   0.1136032
+1922.55   0.0078972   0.1138283
+1922.60   0.0078793   0.1140556
+1922.65   0.0078582   0.1142850
+1922.70   0.0078338   0.1145165
+1922.75   0.0078062   0.1147501
+1922.80   0.0077753   0.1149858
+1922.85   0.0077413   0.1152237
+1922.90   0.0077040   0.1154636
+1922.95   0.0076636   0.1157056
+1923.00   0.0076199   0.1159498
+1923.05   0.0075731   0.1161960
+1923.10   0.0075232   0.1164443
+1923.15   0.0074701   0.1166947
+1923.20   0.0074139   0.1169472
+1923.25   0.0073547   0.1172017
+1923.30   0.0072923   0.1174583
+1923.35   0.0072270   0.1177170
+1923.40   0.0071586   0.1179778
+1923.45   0.0070872   0.1182406
+1923.50   0.0070129   0.1185055
+1923.55   0.0069356   0.1187724
+1923.60   0.0068555   0.1190413
+1923.65   0.0067724   0.1193123
+1923.70   0.0066865   0.1195854
+1923.75   0.0065979   0.1198605
+1923.80   0.0065064   0.1201376
+1923.85   0.0064123   0.1204167
+1923.90   0.0063154   0.1206979
+1923.95   0.0062159   0.1209810
+1924.00   0.0061137   0.1212662
+1924.05   0.0060090   0.1215534
+1924.10   0.0059017   0.1218426
+1924.15   0.0057920   0.1221338
+1924.20   0.0056798   0.1224270
+1924.25   0.0055651   0.1227222
+1924.30   0.0054481   0.1230194
+1924.35   0.0053288   0.1233185
+1924.40   0.0052073   0.1236197
+1924.45   0.0050834   0.1239228
+1924.50   0.0049575   0.1242278
+1924.55   0.0048293   0.1245348
+1924.60   0.0046991   0.1248438
+1924.65   0.0045669   0.1251547
+1924.70   0.0044326   0.1254675
+1924.75   0.0042965   0.1257823
+1924.80   0.0041584   0.1260990
+1924.85   0.0040185   0.1264176
+1924.90   0.0038769   0.1267381
+1924.95   0.0037335   0.1270605
+1925.00   0.0035884   0.1273848
+1925.05   0.0034416   0.1277110
+1925.10   0.0032933   0.1280391
+1925.15   0.0031435   0.1283690
+1925.20   0.0029922   0.1287008
+1925.25   0.0028395   0.1290344
+1925.30   0.0026854   0.1293699
+1925.35   0.0025300   0.1297071
+1925.40   0.0023733   0.1300462
+1925.45   0.0022154   0.1303871
+1925.50   0.0020563   0.1307298
+1925.55   0.0018962   0.1310743
+1925.60   0.0017350   0.1314205
+1925.65   0.0015727   0.1317685
+1925.70   0.0014096   0.1321182
+1925.75   0.0012455   0.1324697
+1925.80   0.0010805   0.1328228
+1925.85   0.0009148   0.1331777
+1925.90   0.0007483   0.1335342
+1925.95   0.0005811   0.1338924
+1926.00   0.0004132   0.1342522
+1926.05   0.0002448   0.1346136
+1926.10   0.0000758   0.1349767
+1926.15  -0.0000938   0.1353414
+1926.20  -0.0002637   0.1357076
+1926.25  -0.0004341   0.1360754
+1926.30  -0.0006049   0.1364447
+1926.35  -0.0007760   0.1368155
+1926.40  -0.0009474   0.1371878
+1926.45  -0.0011190   0.1375616
+1926.50  -0.0012908   0.1379368
+1926.55  -0.0014628   0.1383134
+1926.60  -0.0016348   0.1386915
+1926.65  -0.0018069   0.1390709
+1926.70  -0.0019791   0.1394517
+1926.75  -0.0021512   0.1398337
+1926.80  -0.0023233   0.1402171
+1926.85  -0.0024953   0.1406018
+1926.90  -0.0026671   0.1409877
+1926.95  -0.0028388   0.1413748
+1927.00  -0.0030103   0.1417631
+1927.05  -0.0031815   0.1421526
+1927.10  -0.0033525   0.1425432
+1927.15  -0.0035231   0.1429349
+1927.20  -0.0036934   0.1433276
+1927.25  -0.0038634   0.1437214
+1927.30  -0.0040329   0.1441162
+1927.35  -0.0042020   0.1445120
+1927.40  -0.0043706   0.1449087
+1927.45  -0.0045387   0.1453063
+1927.50  -0.0047063   0.1457048
+1927.55  -0.0048734   0.1461041
+1927.60  -0.0050399   0.1465042
+1927.65  -0.0052057   0.1469051
+1927.70  -0.0053710   0.1473067
+1927.75  -0.0055356   0.1477090
+1927.80  -0.0056995   0.1481120
+1927.85  -0.0058627   0.1485156
+1927.90  -0.0060251   0.1489197
+1927.95  -0.0061869   0.1493244
+1928.00  -0.0063478   0.1497296
+1928.05  -0.0065080   0.1501353
+1928.10  -0.0066673   0.1505413
+1928.15  -0.0068259   0.1509478
+1928.20  -0.0069836   0.1513546
+1928.25  -0.0071404   0.1517617
+1928.30  -0.0072963   0.1521691
+1928.35  -0.0074514   0.1525767
+1928.40  -0.0076055   0.1529844
+1928.45  -0.0077587   0.1533923
+1928.50  -0.0079110   0.1538003
+1928.55  -0.0080622   0.1542083
+1928.60  -0.0082126   0.1546164
+1928.65  -0.0083619   0.1550244
+1928.70  -0.0085102   0.1554323
+1928.75  -0.0086575   0.1558402
+1928.80  -0.0088038   0.1562478
+1928.85  -0.0089491   0.1566553
+1928.90  -0.0090933   0.1570625
+1928.95  -0.0092364   0.1574694
+1929.00  -0.0093784   0.1578760
+1929.05  -0.0095194   0.1582823
+1929.10  -0.0096593   0.1586881
+1929.15  -0.0097980   0.1590934
+1929.20  -0.0099357   0.1594983
+1929.25  -0.0100722   0.1599026
+1929.30  -0.0102075   0.1603063
+1929.35  -0.0103418   0.1607094
+1929.40  -0.0104748   0.1611118
+1929.45  -0.0106067   0.1615135
+1929.50  -0.0107374   0.1619145
+1929.55  -0.0108669   0.1623147
+1929.60  -0.0109953   0.1627141
+1929.65  -0.0111224   0.1631125
+1929.70  -0.0112483   0.1635101
+1929.75  -0.0113729   0.1639067
+1929.80  -0.0114964   0.1643024
+1929.85  -0.0116185   0.1646970
+1929.90  -0.0117394   0.1650905
+1929.95  -0.0118591   0.1654830
+1930.00  -0.0119774   0.1658743
+1930.05  -0.0120945   0.1662644
+1930.10  -0.0122103   0.1666533
+1930.15  -0.0123247   0.1670410
+1930.20  -0.0124379   0.1674274
+1930.25  -0.0125496   0.1678125
+1930.30  -0.0126601   0.1681963
+1930.35  -0.0127691   0.1685787
+1930.40  -0.0128768   0.1689596
+1930.45  -0.0129832   0.1693392
+1930.50  -0.0130881   0.1697172
+1930.55  -0.0131916   0.1700938
+1930.60  -0.0132936   0.1704688
+1930.65  -0.0133943   0.1708423
+1930.70  -0.0134934   0.1712142
+1930.75  -0.0135911   0.1715846
+1930.80  -0.0136873   0.1719532
+1930.85  -0.0137820   0.1723202
+1930.90  -0.0138752   0.1726856
+1930.95  -0.0139669   0.1730492
+1931.00  -0.0140570   0.1734111
+1931.05  -0.0141455   0.1737713
+1931.10  -0.0142324   0.1741297
+1931.15  -0.0143178   0.1744864
+1931.20  -0.0144015   0.1748412
+1931.25  -0.0144835   0.1751942
+1931.30  -0.0145639   0.1755454
+1931.35  -0.0146427   0.1758947
+1931.40  -0.0147197   0.1762422
+1931.45  -0.0147950   0.1765878
+1931.50  -0.0148685   0.1769315
+1931.55  -0.0149403   0.1772733
+1931.60  -0.0150103   0.1776132
+1931.65  -0.0150785   0.1779512
+1931.70  -0.0151449   0.1782873
+1931.75  -0.0152094   0.1786215
+1931.80  -0.0152721   0.1789537
+1931.85  -0.0153328   0.1792839
+1931.90  -0.0153916   0.1796122
+1931.95  -0.0154485   0.1799386
+1932.00  -0.0155034   0.1802630
+1932.05  -0.0155563   0.1805855
+1932.10  -0.0156072   0.1809060
+1932.15  -0.0156560   0.1812246
+1932.20  -0.0157028   0.1815412
+1932.25  -0.0157475   0.1818559
+1932.30  -0.0157900   0.1821686
+1932.35  -0.0158304   0.1824794
+1932.40  -0.0158687   0.1827883
+1932.45  -0.0159047   0.1830952
+1932.50  -0.0159386   0.1834003
+1932.55  -0.0159701   0.1837034
+1932.60  -0.0159994   0.1840046
+1932.65  -0.0160264   0.1843039
+1932.70  -0.0160511   0.1846014
+1932.75  -0.0160734   0.1848970
+1932.80  -0.0160934   0.1851907
+1932.85  -0.0161109   0.1854826
+1932.90  -0.0161260   0.1857727
+1932.95  -0.0161387   0.1860609
+1933.00  -0.0161489   0.1863474
+1933.05  -0.0161566   0.1866321
+1933.10  -0.0161617   0.1869150
+1933.15  -0.0161643   0.1871962
+1933.20  -0.0161643   0.1874756
+1933.25  -0.0161617   0.1877534
+1933.30  -0.0161565   0.1880294
+1933.35  -0.0161487   0.1883038
+1933.40  -0.0161382   0.1885766
+1933.45  -0.0161249   0.1888477
+1933.50  -0.0161090   0.1891172
+1933.55  -0.0160903   0.1893851
+1933.60  -0.0160689   0.1896515
+1933.65  -0.0160447   0.1899164
+1933.70  -0.0160177   0.1901797
+1933.75  -0.0159879   0.1904415
+1933.80  -0.0159553   0.1907019
+1933.85  -0.0159198   0.1909608
+1933.90  -0.0158815   0.1912183
+1933.95  -0.0158402   0.1914745
+1934.00  -0.0157961   0.1917292
+1934.05  -0.0157491   0.1919826
+1934.10  -0.0156991   0.1922347
+1934.15  -0.0156463   0.1924855
+1934.20  -0.0155904   0.1927350
+1934.25  -0.0155317   0.1929833
+1934.30  -0.0154699   0.1932304
+1934.35  -0.0154052   0.1934763
+1934.40  -0.0153375   0.1937210
+1934.45  -0.0152668   0.1939646
+1934.50  -0.0151932   0.1942071
+1934.55  -0.0151165   0.1944484
+1934.60  -0.0150369   0.1946887
+1934.65  -0.0149542   0.1949280
+1934.70  -0.0148686   0.1951662
+1934.75  -0.0147799   0.1954034
+1934.80  -0.0146883   0.1956397
+1934.85  -0.0145937   0.1958750
+1934.90  -0.0144960   0.1961094
+1934.95  -0.0143955   0.1963429
+1935.00  -0.0142919   0.1965755
+1935.05  -0.0141854   0.1968072
+1935.10  -0.0140759   0.1970381
+1935.15  -0.0139635   0.1972681
+1935.20  -0.0138482   0.1974974
+1935.25  -0.0137300   0.1977259
+1935.30  -0.0136088   0.1979536
+1935.35  -0.0134848   0.1981805
+1935.40  -0.0133580   0.1984067
+1935.45  -0.0132283   0.1986322
+1935.50  -0.0130958   0.1988570
+1935.55  -0.0129605   0.1990811
+1935.60  -0.0128224   0.1993046
+1935.65  -0.0126816   0.1995273
+1935.70  -0.0125381   0.1997494
+1935.75  -0.0123919   0.1999709
+1935.80  -0.0122430   0.2001918
+1935.85  -0.0120916   0.2004120
+1935.90  -0.0119375   0.2006316
+1935.95  -0.0117809   0.2008506
+1936.00  -0.0116218   0.2010690
+1936.05  -0.0114602   0.2012868
+1936.10  -0.0112962   0.2015041
+1936.15  -0.0111298   0.2017207
+1936.20  -0.0109611   0.2019367
+1936.25  -0.0107900   0.2021522
+1936.30  -0.0106167   0.2023671
+1936.35  -0.0104411   0.2025814
+1936.40  -0.0102634   0.2027952
+1936.45  -0.0100836   0.2030083
+1936.50  -0.0099017   0.2032208
+1936.55  -0.0097178   0.2034328
+1936.60  -0.0095319   0.2036442
+1936.65  -0.0093441   0.2038549
+1936.70  -0.0091545   0.2040650
+1936.75  -0.0089631   0.2042746
+1936.80  -0.0087699   0.2044834
+1936.85  -0.0085750   0.2046917
+1936.90  -0.0083785   0.2048992
+1936.95  -0.0081805   0.2051062
+1937.00  -0.0079809   0.2053124
+1937.05  -0.0077799   0.2055179
+1937.10  -0.0075776   0.2057227
+1937.15  -0.0073739   0.2059268
+1937.20  -0.0071690   0.2061301
+1937.25  -0.0069628   0.2063327
+1937.30  -0.0067556   0.2065345
+1937.35  -0.0065473   0.2067355
+1937.40  -0.0063380   0.2069356
+1937.45  -0.0061278   0.2071349
+1937.50  -0.0059168   0.2073333
+1937.55  -0.0057049   0.2075309
+1937.60  -0.0054924   0.2077275
+1937.65  -0.0052792   0.2079231
+1937.70  -0.0050654   0.2081178
+1937.75  -0.0048511   0.2083115
+1937.80  -0.0046363   0.2085042
+1937.85  -0.0044212   0.2086959
+1937.90  -0.0042058   0.2088864
+1937.95  -0.0039901   0.2090759
+1938.00  -0.0037743   0.2092642
+1938.05  -0.0035584   0.2094513
+1938.10  -0.0033424   0.2096373
+1938.15  -0.0031265   0.2098220
+1938.20  -0.0029107   0.2100055
+1938.25  -0.0026950   0.2101877
+1938.30  -0.0024796   0.2103686
+1938.35  -0.0022645   0.2105481
+1938.40  -0.0020497   0.2107263
+1938.45  -0.0018354   0.2109031
+1938.50  -0.0016216   0.2110784
+1938.55  -0.0014083   0.2112523
+1938.60  -0.0011956   0.2114246
+1938.65  -0.0009836   0.2115955
+1938.70  -0.0007724   0.2117647
+1938.75  -0.0005619   0.2119324
+1938.80  -0.0003523   0.2120985
+1938.85  -0.0001436   0.2122629
+1938.90   0.0000642   0.2124256
+1938.95   0.0002709   0.2125867
+1939.00   0.0004766   0.2127459
+1939.05   0.0006811   0.2129035
+1939.10   0.0008845   0.2130592
+1939.15   0.0010867   0.2132131
+1939.20   0.0012876   0.2133652
+1939.25   0.0014872   0.2135154
+1939.30   0.0016855   0.2136637
+1939.35   0.0018824   0.2138101
+1939.40   0.0020778   0.2139546
+1939.45   0.0022718   0.2140970
+1939.50   0.0024643   0.2142375
+1939.55   0.0026553   0.2143760
+1939.60   0.0028447   0.2145125
+1939.65   0.0030325   0.2146470
+1939.70   0.0032187   0.2147793
+1939.75   0.0034032   0.2149096
+1939.80   0.0035861   0.2150378
+1939.85   0.0037673   0.2151639
+1939.90   0.0039467   0.2152879
+1939.95   0.0041245   0.2154098
+1940.00   0.0043004   0.2155295
+1940.05   0.0044747   0.2156471
+1940.10   0.0046471   0.2157625
+1940.15   0.0048178   0.2158758
+1940.20   0.0049867   0.2159869
+1940.25   0.0051538   0.2160958
+1940.30   0.0053191   0.2162026
+1940.35   0.0054826   0.2163072
+1940.40   0.0056443   0.2164096
+1940.45   0.0058043   0.2165099
+1940.50   0.0059624   0.2166080
+1940.55   0.0061188   0.2167039
+1940.60   0.0062733   0.2167977
+1940.65   0.0064262   0.2168894
+1940.70   0.0065773   0.2169790
+1940.75   0.0067266   0.2170664
+1940.80   0.0068743   0.2171517
+1940.85   0.0070202   0.2172350
+1940.90   0.0071645   0.2173162
+1940.95   0.0073072   0.2173953
+1941.00   0.0074482   0.2174725
+1941.05   0.0075877   0.2175476
+1941.10   0.0077256   0.2176207
+1941.15   0.0078619   0.2176919
+1941.20   0.0079967   0.2177611
+1941.25   0.0081301   0.2178285
+1941.30   0.0082621   0.2178939
+1941.35   0.0083927   0.2179576
+1941.40   0.0085219   0.2180194
+1941.45   0.0086498   0.2180794
+1941.50   0.0087764   0.2181377
+1941.55   0.0089018   0.2181943
+1941.60   0.0090260   0.2182493
+1941.65   0.0091491   0.2183026
+1941.70   0.0092710   0.2183543
+1941.75   0.0093920   0.2184045
+1941.80   0.0095119   0.2184531
+1941.85   0.0096309   0.2185004
+1941.90   0.0097490   0.2185462
+1941.95   0.0098663   0.2185906
+1942.00   0.0099828   0.2186338
+1942.05   0.0100985   0.2186756
+1942.10   0.0102135   0.2187163
+1942.15   0.0103279   0.2187557
+1942.20   0.0104418   0.2187941
+1942.25   0.0105551   0.2188314
+1942.30   0.0106679   0.2188677
+1942.35   0.0107803   0.2189030
+1942.40   0.0108924   0.2189374
+1942.45   0.0110041   0.2189710
+1942.50   0.0111157   0.2190038
+1942.55   0.0112270   0.2190358
+1942.60   0.0113382   0.2190672
+1942.65   0.0114493   0.2190979
+1942.70   0.0115603   0.2191281
+1942.75   0.0116714   0.2191577
+1942.80   0.0117826   0.2191869
+1942.85   0.0118939   0.2192157
+1942.90   0.0120054   0.2192442
+1942.95   0.0121171   0.2192724
+1943.00   0.0122291   0.2193003
+1943.05   0.0123415   0.2193281
+1943.10   0.0124542   0.2193558
+1943.15   0.0125674   0.2193834
+1943.20   0.0126810   0.2194111
+1943.25   0.0127952   0.2194388
+1943.30   0.0129099   0.2194666
+1943.35   0.0130253   0.2194946
+1943.40   0.0131413   0.2195229
+1943.45   0.0132580   0.2195514
+1943.50   0.0133754   0.2195802
+1943.55   0.0134936   0.2196095
+1943.60   0.0136127   0.2196392
+1943.65   0.0137325   0.2196694
+1943.70   0.0138533   0.2197001
+1943.75   0.0139749   0.2197315
+1943.80   0.0140975   0.2197635
+1943.85   0.0142211   0.2197962
+1943.90   0.0143457   0.2198296
+1943.95   0.0144712   0.2198639
+1944.00   0.0145978   0.2198989
+1944.05   0.0147255   0.2199349
+1944.10   0.0148543   0.2199718
+1944.15   0.0149841   0.2200097
+1944.20   0.0151151   0.2200485
+1944.25   0.0152471   0.2200884
+1944.30   0.0153804   0.2201294
+1944.35   0.0155147   0.2201716
+1944.40   0.0156502   0.2202149
+1944.45   0.0157868   0.2202594
+1944.50   0.0159247   0.2203051
+1944.55   0.0160636   0.2203521
+1944.60   0.0162037   0.2204003
+1944.65   0.0163450   0.2204499
+1944.70   0.0164874   0.2205009
+1944.75   0.0166309   0.2205532
+1944.80   0.0167755   0.2206069
+1944.85   0.0169213   0.2206621
+1944.90   0.0170681   0.2207187
+1944.95   0.0172161   0.2207767
+1945.00   0.0173651   0.2208363
+1945.05   0.0175151   0.2208973
+1945.10   0.0176661   0.2209599
+1945.15   0.0178182   0.2210240
+1945.20   0.0179712   0.2210897
+1945.25   0.0181252   0.2211569
+1945.30   0.0182800   0.2212257
+1945.35   0.0184357   0.2212961
+1945.40   0.0185923   0.2213681
+1945.45   0.0187497   0.2214417
+1945.50   0.0189079   0.2215169
+1945.55   0.0190668   0.2215937
+1945.60   0.0192263   0.2216721
+1945.65   0.0193866   0.2217522
+1945.70   0.0195474   0.2218338
+1945.75   0.0197088   0.2219171
+1945.80   0.0198707   0.2220020
+1945.85   0.0200331   0.2220885
+1945.90   0.0201959   0.2221767
+1945.95   0.0203591   0.2222664
+1946.00   0.0205226   0.2223578
+1946.05   0.0206864   0.2224507
+1946.10   0.0208504   0.2225452
+1946.15   0.0210145   0.2226414
+1946.20   0.0211788   0.2227391
+1946.25   0.0213431   0.2228383
+1946.30   0.0215074   0.2229392
+1946.35   0.0216716   0.2230416
+1946.40   0.0218358   0.2231455
+1946.45   0.0219997   0.2232510
+1946.50   0.0221634   0.2233579
+1946.55   0.0223268   0.2234664
+1946.60   0.0224899   0.2235764
+1946.65   0.0226526   0.2236879
+1946.70   0.0228147   0.2238008
+1946.75   0.0229764   0.2239152
+1946.80   0.0231374   0.2240310
+1946.85   0.0232978   0.2241483
+1946.90   0.0234575   0.2242670
+1946.95   0.0236164   0.2243871
+1947.00   0.0237745   0.2245086
+1947.05   0.0239317   0.2246314
+1947.10   0.0240879   0.2247557
+1947.15   0.0242431   0.2248813
+1947.20   0.0243973   0.2250082
+1947.25   0.0245504   0.2251365
+1947.30   0.0247022   0.2252661
+1947.35   0.0248528   0.2253970
+1947.40   0.0250022   0.2255292
+1947.45   0.0251502   0.2256626
+1947.50   0.0252968   0.2257974
+1947.55   0.0254419   0.2259334
+1947.60   0.0255855   0.2260707
+1947.65   0.0257276   0.2262092
+1947.70   0.0258681   0.2263490
+1947.75   0.0260069   0.2264900
+1947.80   0.0261440   0.2266323
+1947.85   0.0262794   0.2267757
+1947.90   0.0264130   0.2269204
+1947.95   0.0265447   0.2270663
+1948.00   0.0266746   0.2272135
+1948.05   0.0268026   0.2273618
+1948.10   0.0269285   0.2275113
+1948.15   0.0270525   0.2276620
+1948.20   0.0271745   0.2278140
+1948.25   0.0272944   0.2279671
+1948.30   0.0274122   0.2281215
+1948.35   0.0275278   0.2282771
+1948.40   0.0276413   0.2284339
+1948.45   0.0277526   0.2285919
+1948.50   0.0278616   0.2287511
+1948.55   0.0279684   0.2289115
+1948.60   0.0280730   0.2290732
+1948.65   0.0281752   0.2292361
+1948.70   0.0282751   0.2294003
+1948.75   0.0283727   0.2295658
+1948.80   0.0284680   0.2297325
+1948.85   0.0285608   0.2299005
+1948.90   0.0286513   0.2300697
+1948.95   0.0287393   0.2302403
+1949.00   0.0288250   0.2304122
+1949.05   0.0289082   0.2305855
+1949.10   0.0289890   0.2307600
+1949.15   0.0290674   0.2309360
+1949.20   0.0291433   0.2311133
+1949.25   0.0292168   0.2312919
+1949.30   0.0292879   0.2314720
+1949.35   0.0293565   0.2316536
+1949.40   0.0294226   0.2318365
+1949.45   0.0294863   0.2320209
+1949.50   0.0295476   0.2322068
+1949.55   0.0296064   0.2323942
+1949.60   0.0296628   0.2325831
+1949.65   0.0297168   0.2327735
+1949.70   0.0297684   0.2329655
+1949.75   0.0298176   0.2331590
+1949.80   0.0298644   0.2333541
+1949.85   0.0299089   0.2335508
+1949.90   0.0299510   0.2337492
+1949.95   0.0299907   0.2339492
+1950.00   0.0300282   0.2341508
+1950.05   0.0300633   0.2343542
+1950.10   0.0300962   0.2345592
+1950.15   0.0301267   0.2347659
+1950.20   0.0301551   0.2349744
+1950.25   0.0301812   0.2351847
+1950.30   0.0302052   0.2353966
+1950.35   0.0302269   0.2356104
+1950.40   0.0302466   0.2358260
+1950.45   0.0302641   0.2360434
+1950.50   0.0302795   0.2362626
+1950.55   0.0302929   0.2364836
+1950.60   0.0303042   0.2367065
+1950.65   0.0303135   0.2369313
+1950.70   0.0303208   0.2371579
+1950.75   0.0303262   0.2373865
+1950.80   0.0303297   0.2376169
+1950.85   0.0303313   0.2378492
+1950.90   0.0303310   0.2380834
+1950.95   0.0303289   0.2383195
+1951.00   0.0303251   0.2385575
+1951.05   0.0303194   0.2387974
+1951.10   0.0303120   0.2390392
+1951.15   0.0303030   0.2392830
+1951.20   0.0302922   0.2395286
+1951.25   0.0302799   0.2397762
+1951.30   0.0302659   0.2400256
+1951.35   0.0302504   0.2402770
+1951.40   0.0302333   0.2405302
+1951.45   0.0302148   0.2407853
+1951.50   0.0301947   0.2410422
+1951.55   0.0301732   0.2413009
+1951.60   0.0301504   0.2415615
+1951.65   0.0301261   0.2418239
+1951.70   0.0301005   0.2420881
+1951.75   0.0300736   0.2423540
+1951.80   0.0300454   0.2426217
+1951.85   0.0300159   0.2428910
+1951.90   0.0299852   0.2431620
+1951.95   0.0299534   0.2434347
+1952.00   0.0299203   0.2437090
+1952.05   0.0298861   0.2439849
+1952.10   0.0298509   0.2442623
+1952.15   0.0298145   0.2445412
+1952.20   0.0297770   0.2448215
+1952.25   0.0297386   0.2451033
+1952.30   0.0296991   0.2453864
+1952.35   0.0296586   0.2456708
+1952.40   0.0296172   0.2459565
+1952.45   0.0295748   0.2462433
+1952.50   0.0295315   0.2465314
+1952.55   0.0294873   0.2468205
+1952.60   0.0294423   0.2471107
+1952.65   0.0293964   0.2474018
+1952.70   0.0293496   0.2476938
+1952.75   0.0293020   0.2479866
+1952.80   0.0292536   0.2482803
+1952.85   0.0292045   0.2485746
+1952.90   0.0291545   0.2488695
+1952.95   0.0291038   0.2491649
+1953.00   0.0290524   0.2494608
+1953.05   0.0290002   0.2497571
+1953.10   0.0289473   0.2500537
+1953.15   0.0288937   0.2503505
+1953.20   0.0288394   0.2506474
+1953.25   0.0287844   0.2509444
+1953.30   0.0287287   0.2512413
+1953.35   0.0286723   0.2515380
+1953.40   0.0286153   0.2518345
+1953.45   0.0285576   0.2521307
+1953.50   0.0284992   0.2524264
+1953.55   0.0284402   0.2527215
+1953.60   0.0283805   0.2530160
+1953.65   0.0283201   0.2533098
+1953.70   0.0282592   0.2536027
+1953.75   0.0281975   0.2538946
+1953.80   0.0281352   0.2541854
+1953.85   0.0280723   0.2544751
+1953.90   0.0280086   0.2547634
+1953.95   0.0279444   0.2550504
+1954.00   0.0278794   0.2553358
+1954.05   0.0278138   0.2556196
+1954.10   0.0277475   0.2559016
+1954.15   0.0276806   0.2561818
+1954.20   0.0276129   0.2564599
+1954.25   0.0275445   0.2567359
+1954.30   0.0274755   0.2570097
+1954.35   0.0274057   0.2572811
+1954.40   0.0273351   0.2575501
+1954.45   0.0272639   0.2578164
+1954.50   0.0271919   0.2580800
+1954.55   0.0271191   0.2583408
+1954.60   0.0270456   0.2585986
+1954.65   0.0269713   0.2588532
+1954.70   0.0268961   0.2591047
+1954.75   0.0268202   0.2593528
+1954.80   0.0267434   0.2595974
+1954.85   0.0266658   0.2598384
+1954.90   0.0265874   0.2600757
+1954.95   0.0265080   0.2603091
+1955.00   0.0264278   0.2605386
+1955.05   0.0263467   0.2607639
+1955.10   0.0262646   0.2609851
+1955.15   0.0261816   0.2612018
+1955.20   0.0260976   0.2614141
+1955.25   0.0260127   0.2616218
+1955.30   0.0259268   0.2618248
+1955.35   0.0258398   0.2620230
+1955.40   0.0257519   0.2622162
+1955.45   0.0256628   0.2624043
+1955.50   0.0255727   0.2625873
+1955.55   0.0254816   0.2627650
+1955.60   0.0253893   0.2629372
+1955.65   0.0252959   0.2631039
+1955.70   0.0252013   0.2632649
+1955.75   0.0251056   0.2634203
+1955.80   0.0250087   0.2635697
+1955.85   0.0249106   0.2637132
+1955.90   0.0248113   0.2638506
+1955.95   0.0247108   0.2639819
+1956.00   0.0246090   0.2641069
+1956.05   0.0245059   0.2642255
+1956.10   0.0244016   0.2643377
+1956.15   0.0242959   0.2644433
+1956.20   0.0241889   0.2645422
+1956.25   0.0240806   0.2646344
+1956.30   0.0239709   0.2647198
+1956.35   0.0238598   0.2647983
+1956.40   0.0237473   0.2648698
+1956.45   0.0236334   0.2649343
+1956.50   0.0235181   0.2649916
+1956.55   0.0234014   0.2650417
+1956.60   0.0232832   0.2650845
+1956.65   0.0231635   0.2651199
+1956.70   0.0230424   0.2651480
+1956.75   0.0229197   0.2651686
+1956.80   0.0227956   0.2651816
+1956.85   0.0226699   0.2651871
+1956.90   0.0225427   0.2651849
+1956.95   0.0224139   0.2651751
+1957.00   0.0222836   0.2651575
+1957.05   0.0221517   0.2651322
+1957.10   0.0220183   0.2650991
+1957.15   0.0218832   0.2650581
+1957.20   0.0217466   0.2650093
+1957.25   0.0216084   0.2649526
+1957.30   0.0214686   0.2648880
+1957.35   0.0213271   0.2648154
+1957.40   0.0211841   0.2647349
+1957.45   0.0210394   0.2646465
+1957.50   0.0208931   0.2645500
+1957.55   0.0207452   0.2644456
+1957.60   0.0205957   0.2643333
+1957.65   0.0204445   0.2642129
+1957.70   0.0202917   0.2640847
+1957.75   0.0201373   0.2639484
+1957.80   0.0199813   0.2638043
+1957.85   0.0198236   0.2636522
+1957.90   0.0196643   0.2634922
+1957.95   0.0195034   0.2633244
+1958.00   0.0193409   0.2631487
+1958.05   0.0191767   0.2629652
+1958.10   0.0190110   0.2627740
+1958.15   0.0188437   0.2625750
+1958.20   0.0186748   0.2623684
+1958.25   0.0185043   0.2621541
+1958.30   0.0183323   0.2619323
+1958.35   0.0181587   0.2617029
+1958.40   0.0179835   0.2614661
+1958.45   0.0178069   0.2612219
+1958.50   0.0176287   0.2609704
+1958.55   0.0174490   0.2607116
+1958.60   0.0172679   0.2604456
+1958.65   0.0170853   0.2601725
+1958.70   0.0169012   0.2598924
+1958.75   0.0167158   0.2596054
+1958.80   0.0165289   0.2593115
+1958.85   0.0163406   0.2590109
+1958.90   0.0161510   0.2587036
+1958.95   0.0159600   0.2583897
+1959.00   0.0157677   0.2580694
+1959.05   0.0155742   0.2577427
+1959.10   0.0153793   0.2574097
+1959.15   0.0151832   0.2570706
+1959.20   0.0149859   0.2567255
+1959.25   0.0147875   0.2563745
+1959.30   0.0145878   0.2560177
+1959.35   0.0143871   0.2556551
+1959.40   0.0141852   0.2552871
+1959.45   0.0139823   0.2549136
+1959.50   0.0137784   0.2545348
+1959.55   0.0135735   0.2541509
+1959.60   0.0133676   0.2537619
+1959.65   0.0131608   0.2533680
+1959.70   0.0129531   0.2529693
+1959.75   0.0127445   0.2525660
+1959.80   0.0125352   0.2521583
+1959.85   0.0123251   0.2517462
+1959.90   0.0121142   0.2513299
+1959.95   0.0119026   0.2509095
+1960.00   0.0116904   0.2504853
+1960.05   0.0114776   0.2500573
+1960.10   0.0112642   0.2496257
+1960.15   0.0110503   0.2491906
+1960.20   0.0108359   0.2487522
+1960.25   0.0106210   0.2483107
+1960.30   0.0104058   0.2478662
+1960.35   0.0101902   0.2474189
+1960.40   0.0099743   0.2469689
+1960.45   0.0097582   0.2465164
+1960.50   0.0095418   0.2460615
+1960.55   0.0093253   0.2456043
+1960.60   0.0091087   0.2451452
+1960.65   0.0088920   0.2446841
+1960.70   0.0086753   0.2442214
+1960.75   0.0084586   0.2437570
+1960.80   0.0082420   0.2432912
+1960.85   0.0080256   0.2428242
+1960.90   0.0078093   0.2423561
+1960.95   0.0075932   0.2418870
+1961.00   0.0073774   0.2414172
+1961.05   0.0071620   0.2409467
+1961.10   0.0069469   0.2404758
+1961.15   0.0067323   0.2400045
+1961.20   0.0065182   0.2395331
+1961.25   0.0063046   0.2390617
+1961.30   0.0060916   0.2385905
+1961.35   0.0058792   0.2381195
+1961.40   0.0056675   0.2376490
+1961.45   0.0054566   0.2371791
+1961.50   0.0052464   0.2367099
+1961.55   0.0050371   0.2362417
+1961.60   0.0048287   0.2357745
+1961.65   0.0046213   0.2353085
+1961.70   0.0044148   0.2348438
+1961.75   0.0042094   0.2343806
+1961.80   0.0040051   0.2339190
+1961.85   0.0038019   0.2334592
+1961.90   0.0036000   0.2330012
+1961.95   0.0033993   0.2325453
+1962.00   0.0031998   0.2320915
+1962.05   0.0030017   0.2316401
+1962.10   0.0028051   0.2311910
+1962.15   0.0026098   0.2307445
+1962.20   0.0024160   0.2303006
+1962.25   0.0022238   0.2298595
+1962.30   0.0020332   0.2294213
+1962.35   0.0018441   0.2289862
+1962.40   0.0016568   0.2285542
+1962.45   0.0014711   0.2281254
+1962.50   0.0012873   0.2277000
+1962.55   0.0011052   0.2272780
+1962.60   0.0009249   0.2268597
+1962.65   0.0007466   0.2264450
+1962.70   0.0005701   0.2260340
+1962.75   0.0003957   0.2256270
+1962.80   0.0002232   0.2252239
+1962.85   0.0000528   0.2248249
+1962.90  -0.0001156   0.2244300
+1962.95  -0.0002818   0.2240393
+1963.00  -0.0004459   0.2236530
+1963.05  -0.0006078   0.2232711
+1963.10  -0.0007675   0.2228936
+1963.15  -0.0009249   0.2225207
+1963.20  -0.0010800   0.2221525
+1963.25  -0.0012329   0.2217889
+1963.30  -0.0013833   0.2214301
+1963.35  -0.0015315   0.2210761
+1963.40  -0.0016772   0.2207271
+1963.45  -0.0018205   0.2203830
+1963.50  -0.0019613   0.2200439
+1963.55  -0.0020996   0.2197098
+1963.60  -0.0022355   0.2193809
+1963.65  -0.0023688   0.2190572
+1963.70  -0.0024996   0.2187386
+1963.75  -0.0026278   0.2184254
+1963.80  -0.0027534   0.2181174
+1963.85  -0.0028764   0.2178148
+1963.90  -0.0029968   0.2175175
+1963.95  -0.0031146   0.2172256
+1964.00  -0.0032297   0.2169392
+1964.05  -0.0033422   0.2166583
+1964.10  -0.0034519   0.2163829
+1964.15  -0.0035590   0.2161130
+1964.20  -0.0036634   0.2158486
+1964.25  -0.0037650   0.2155898
+1964.30  -0.0038640   0.2153365
+1964.35  -0.0039602   0.2150889
+1964.40  -0.0040536   0.2148468
+1964.45  -0.0041444   0.2146104
+1964.50  -0.0042324   0.2143796
+1964.55  -0.0043176   0.2141544
+1964.60  -0.0044001   0.2139349
+1964.65  -0.0044798   0.2137210
+1964.70  -0.0045568   0.2135127
+1964.75  -0.0046310   0.2133100
+1964.80  -0.0047025   0.2131130
+1964.85  -0.0047712   0.2129216
+1964.90  -0.0048372   0.2127358
+1964.95  -0.0049004   0.2125556
+1965.00  -0.0049610   0.2123810
+1965.05  -0.0050187   0.2122120
+1965.10  -0.0050738   0.2120485
+1965.15  -0.0051261   0.2118905
+1965.20  -0.0051757   0.2117381
+1965.25  -0.0052226   0.2115912
+1965.30  -0.0052669   0.2114498
+1965.35  -0.0053084   0.2113138
+1965.40  -0.0053473   0.2111833
+1965.45  -0.0053835   0.2110581
+1965.50  -0.0054171   0.2109384
+1965.55  -0.0054480   0.2108239
+1965.60  -0.0054764   0.2107148
+1965.65  -0.0055021   0.2106110
+1965.70  -0.0055252   0.2105125
+1965.75  -0.0055458   0.2104192
+1965.80  -0.0055638   0.2103310
+1965.85  -0.0055793   0.2102480
+1965.90  -0.0055922   0.2101701
+1965.95  -0.0056027   0.2100973
+1966.00  -0.0056106   0.2100295
+1966.05  -0.0056161   0.2099668
+1966.10  -0.0056192   0.2099089
+1966.15  -0.0056198   0.2098560
+1966.20  -0.0056179   0.2098080
+1966.25  -0.0056137   0.2097648
+1966.30  -0.0056071   0.2097263
+1966.35  -0.0055982   0.2096926
+1966.40  -0.0055869   0.2096636
+1966.45  -0.0055733   0.2096393
+1966.50  -0.0055575   0.2096196
+1966.55  -0.0055393   0.2096044
+1966.60  -0.0055189   0.2095937
+1966.65  -0.0054963   0.2095875
+1966.70  -0.0054714   0.2095857
+1966.75  -0.0054444   0.2095882
+1966.80  -0.0054152   0.2095951
+1966.85  -0.0053838   0.2096063
+1966.90  -0.0053503   0.2096216
+1966.95  -0.0053148   0.2096412
+1967.00  -0.0052771   0.2096648
+1967.05  -0.0052374   0.2096925
+1967.10  -0.0051956   0.2097243
+1967.15  -0.0051518   0.2097600
+1967.20  -0.0051060   0.2097996
+1967.25  -0.0050583   0.2098431
+1967.30  -0.0050086   0.2098904
+1967.35  -0.0049569   0.2099415
+1967.40  -0.0049033   0.2099963
+1967.45  -0.0048479   0.2100547
+1967.50  -0.0047905   0.2101168
+1967.55  -0.0047313   0.2101824
+1967.60  -0.0046703   0.2102516
+1967.65  -0.0046075   0.2103242
+1967.70  -0.0045428   0.2104003
+1967.75  -0.0044764   0.2104797
+1967.80  -0.0044082   0.2105624
+1967.85  -0.0043383   0.2106484
+1967.90  -0.0042667   0.2107376
+1967.95  -0.0041934   0.2108300
+1968.00  -0.0041184   0.2109255
+1968.05  -0.0040417   0.2110241
+1968.10  -0.0039634   0.2111257
+1968.15  -0.0038835   0.2112303
+1968.20  -0.0038019   0.2113378
+1968.25  -0.0037188   0.2114483
+1968.30  -0.0036341   0.2115615
 1968.35  -0.0035479   0.2116776
 1968.40  -0.0034601   0.2117964
-1968.45  -0.0033708   0.2119179
-1968.50  -0.0032800   0.2120421
-1968.55  -0.0031877   0.2121689
+1968.45  -0.0033707   0.2119179
+1968.50  -0.0032799   0.2120421
+1968.55  -0.0031876   0.2121689
 1968.60  -0.0030939   0.2122983
-1968.65  -0.0029987   0.2124302
+1968.65  -0.0029986   0.2124302
 1968.70  -0.0029020   0.2125646
-1968.75  -0.0028040   0.2127015
-1968.80  -0.0027045   0.2128407
-1968.85  -0.0026036   0.2129824
-1968.90  -0.0025014   0.2131264
-1968.95  -0.0023978   0.2132726
+1968.75  -0.0028039   0.2127015
+1968.80  -0.0027044   0.2128407
+1968.85  -0.0026035   0.2129824
+1968.90  -0.0025013   0.2131264
+1968.95  -0.0023977   0.2132726
 1969.00  -0.0022928   0.2134211
-1969.05  -0.0021866   0.2135719
+1969.05  -0.0021865   0.2135719
 1969.10  -0.0020790   0.2137248
-1969.15  -0.0019702   0.2138798
+1969.15  -0.0019701   0.2138798
 1969.20  -0.0018600   0.2140370
 1969.25  -0.0017486   0.2141962
 1969.30  -0.0016360   0.2143575
 1969.35  -0.0015221   0.2145208
-1969.40  -0.0014071   0.2146860
+1969.40  -0.0014070   0.2146860
 1969.45  -0.0012908   0.2148532
-1969.50  -0.0011734   0.2150223
-1969.55  -0.0010548   0.2151933
+1969.50  -0.0011733   0.2150223
+1969.55  -0.0010547   0.2151933
 1969.60  -0.0009350   0.2153661
 1969.65  -0.0008141   0.2155407
 1969.70  -0.0006921   0.2157171
-1969.75  -0.0005690   0.2158953
+1969.75  -0.0005690   0.2158952
 1969.80  -0.0004448   0.2160751
 1969.85  -0.0003196   0.2162567
 1969.90  -0.0001933   0.2164400
-1969.95  -0.0000660   0.2166249
-1970.00   0.0000623   0.2168115
+1969.95  -0.0000659   0.2166249
+1970.00   0.0000624   0.2168115
 1970.05   0.0001917   0.2169996
 1970.10   0.0003220   0.2171893
 1970.15   0.0004533   0.2173806
 1970.20   0.0005855   0.2175734
 1970.25   0.0007186   0.2177678
-1970.30   0.0008526   0.2179636
+1970.30   0.0008527   0.2179636
 1970.35   0.0009876   0.2181609
 1970.40   0.0011234   0.2183596
-1970.45   0.0012600   0.2185598
+1970.45   0.0012601   0.2185598
 1970.50   0.0013975   0.2187614
 1970.55   0.0015358   0.2189644
 1970.60   0.0016749   0.2191688
-1970.65   0.0018147   0.2193745
+1970.65   0.0018148   0.2193745
 1970.70   0.0019554   0.2195816
 1970.75   0.0020967   0.2197901
 1970.80   0.0022388   0.2199998
 1970.85   0.0023815   0.2202109
 1970.90   0.0025249   0.2204233
 1970.95   0.0026690   0.2206369
 1971.00   0.0028137   0.2208518
 1971.05   0.0029590   0.2210680
 1971.10   0.0031048   0.2212854
 1971.15   0.0032513   0.2215041
 1971.20   0.0033982   0.2217240
 1971.25   0.0035457   0.2219451
 1971.30   0.0036937   0.2221675
 1971.35   0.0038422   0.2223910
-1971.40   0.0039911   0.2226157
+1971.40   0.0039911   0.2226158
 1971.45   0.0041404   0.2228417
 1971.50   0.0042901   0.2230688
 1971.55   0.0044402   0.2232971
-1971.60   0.0045907   0.2235265
+1971.60   0.0045907   0.2235266
 1971.65   0.0047415   0.2237572
-1971.70   0.0048926   0.2239889
-1971.75   0.0050440   0.2242219
+1971.70   0.0048926   0.2239890
+1971.75   0.0050439   0.2242219
 1971.80   0.0051956   0.2244560
-1971.85   0.0053475   0.2246912
+1971.85   0.0053474   0.2246913
 1971.90   0.0054995   0.2249276
-1971.95   0.0056518   0.2251651
+1971.95   0.0056517   0.2251652
 1972.00   0.0058042   0.2254038
-1972.05   0.0059568   0.2256436
-1972.10   0.0061094   0.2258845
-1972.15   0.0062622   0.2261266
-1972.20   0.0064150   0.2263697
-1972.25   0.0065678   0.2266140
-1972.30   0.0067207   0.2268594
-1972.35   0.0068735   0.2271060
-1972.40   0.0070263   0.2273536
-1972.45   0.0071790   0.2276024
-1972.50   0.0073317   0.2278523
-1972.55   0.0074842   0.2281033
-1972.60   0.0076367   0.2283554
-1972.65   0.0077889   0.2286086
-1972.70   0.0079410   0.2288629
-1972.75   0.0080929   0.2291183
-1972.80   0.0082445   0.2293748
-1972.85   0.0083959   0.2296324
-1972.90   0.0085470   0.2298911
-1972.95   0.0086979   0.2301509
-1973.00   0.0088484   0.2304118
-1973.05   0.0089985   0.2306738
-1973.10   0.0091484   0.2309369
-1973.15   0.0092978   0.2312010
-1973.20   0.0094468   0.2314663
-1973.25   0.0095954   0.2317326
-1973.30   0.0097436   0.2320000
-1973.35   0.0098913   0.2322685
-1973.40   0.0100385   0.2325381
-1973.45   0.0101853   0.2328087
-1973.50   0.0103315   0.2330804
-1973.55   0.0104772   0.2333531
-1973.60   0.0106223   0.2336269
-1973.65   0.0107669   0.2339018
-1973.70   0.0109109   0.2341776
-1973.75   0.0110542   0.2344546
-1973.80   0.0111970   0.2347325
-1973.85   0.0113391   0.2350115
-1973.90   0.0114806   0.2352915
-1973.95   0.0116215   0.2355725
-1974.00   0.0117617   0.2358546
-1974.05   0.0119012   0.2361376
-1974.10   0.0120400   0.2364216
-1974.15   0.0121781   0.2367066
-1974.20   0.0123155   0.2369925
-1974.25   0.0124522   0.2372795
-1974.30   0.0125881   0.2375673
-1974.35   0.0127233   0.2378562
-1974.40   0.0128578   0.2381459
-1974.45   0.0129915   0.2384366
-1974.50   0.0131245   0.2387282
-1974.55   0.0132566   0.2390206
-1974.60   0.0133881   0.2393140
-1974.65   0.0135187   0.2396082
-1974.70   0.0136486   0.2399033
-1974.75   0.0137777   0.2401993
-1974.80   0.0139060   0.2404961
-1974.85   0.0140336   0.2407936
-1974.90   0.0141603   0.2410920
-1974.95   0.0142863   0.2413912
-1975.00   0.0144115   0.2416912
-1975.05   0.0145359   0.2419919
-1975.10   0.0146596   0.2422933
-1975.15   0.0147825   0.2425955
-1975.20   0.0149046   0.2428983
-1975.25   0.0150259   0.2432019
-1975.30   0.0151465   0.2435061
-1975.35   0.0152663   0.2438109
-1975.40   0.0153854   0.2441164
-1975.45   0.0155037   0.2444225
-1975.50   0.0156213   0.2447292
-1975.55   0.0157382   0.2450364
-1975.60   0.0158543   0.2453442
-1975.65   0.0159698   0.2456525
-1975.70   0.0160845   0.2459613
-1975.75   0.0161986   0.2462706
-1975.80   0.0163120   0.2465804
-1975.85   0.0164247   0.2468906
-1975.90   0.0165368   0.2472011
-1975.95   0.0166482   0.2475121
-1976.00   0.0167590   0.2478235
-1976.05   0.0168692   0.2481351
-1976.10   0.0169788   0.2484471
-1976.15   0.0170878   0.2487594
-1976.20   0.0171962   0.2490719
-1976.25   0.0173041   0.2493847
-1976.30   0.0174114   0.2496977
-1976.35   0.0175182   0.2500108
-1976.40   0.0176245   0.2503242
-1976.45   0.0177303   0.2506376
-1976.50   0.0178357   0.2509512
-1976.55   0.0179406   0.2512648
-1976.60   0.0180450   0.2515785
-1976.65   0.0181491   0.2518922
-1976.70   0.0182527   0.2522059
-1976.75   0.0183560   0.2525195
-1976.80   0.0184589   0.2528331
-1976.85   0.0185614   0.2531466
-1976.90   0.0186636   0.2534599
-1976.95   0.0187656   0.2537732
-1977.00   0.0188672   0.2540862
-1977.05   0.0189686   0.2543990
-1977.10   0.0190697   0.2547116
-1977.15   0.0191706   0.2550239
-1977.20   0.0192713   0.2553359
-1977.25   0.0193718   0.2556476
-1977.30   0.0194722   0.2559589
-1977.35   0.0195724   0.2562699
-1977.40   0.0196725   0.2565804
-1977.45   0.0197725   0.2568905
-1977.50   0.0198723   0.2572001
-1977.55   0.0199722   0.2575092
-1977.60   0.0200719   0.2578177
-1977.65   0.0201717   0.2581257
-1977.70   0.0202714   0.2584331
-1977.75   0.0203712   0.2587399
-1977.80   0.0204710   0.2590460
-1977.85   0.0205708   0.2593514
-1977.90   0.0206707   0.2596561
-1977.95   0.0207707   0.2599600
-1978.00   0.0208708   0.2602632
-1978.05   0.0209710   0.2605656
-1978.10   0.0210714   0.2608671
-1978.15   0.0211719   0.2611678
-1978.20   0.0212726   0.2614676
-1978.25   0.0213735   0.2617665
-1978.30   0.0214746   0.2620644
-1978.35   0.0215759   0.2623614
-1978.40   0.0216775   0.2626573
-1978.45   0.0217793   0.2629523
-1978.50   0.0218814   0.2632461
-1978.55   0.0219838   0.2635389
-1978.60   0.0220865   0.2638306
-1978.65   0.0221894   0.2641211
-1978.70   0.0222927   0.2644105
-1978.75   0.0223964   0.2646987
-1978.80   0.0225004   0.2649857
-1978.85   0.0226048   0.2652714
-1978.90   0.0227095   0.2655559
-1978.95   0.0228146   0.2658390
-1979.00   0.0229201   0.2661209
-1979.05   0.0230260   0.2664015
-1979.10   0.0231324   0.2666806
-1979.15   0.0232391   0.2669584
-1979.20   0.0233463   0.2672348
-1979.25   0.0234539   0.2675098
-1979.30   0.0235619   0.2677833
-1979.35   0.0236705   0.2680554
-1979.40   0.0237794   0.2683260
-1979.45   0.0238888   0.2685951
-1979.50   0.0239987   0.2688626
-1979.55   0.0241091   0.2691286
-1979.60   0.0242199   0.2693931
-1979.65   0.0243312   0.2696560
-1979.70   0.0244430   0.2699173
-1979.75   0.0245553   0.2701770
-1979.80   0.0246680   0.2704351
-1979.85   0.0247812   0.2706915
-1979.90   0.0248949   0.2709463
-1979.95   0.0250091   0.2711994
-1980.00   0.0251238   0.2714508
-1980.05   0.0252389   0.2717006
-1980.10   0.0253545   0.2719487
-1980.15   0.0254706   0.2721950
-1980.20   0.0255871   0.2724397
-1980.25   0.0257042   0.2726826
-1980.30   0.0258216   0.2729238
-1980.35   0.0259396   0.2731632
-1980.40   0.0260579   0.2734009
-1980.45   0.0261768   0.2736369
-1980.50   0.0262960   0.2738711
-1980.55   0.0264157   0.2741035
-1980.60   0.0265358   0.2743342
-1980.65   0.0266563   0.2745631
-1980.70   0.0267772   0.2747902
-1980.75   0.0268985   0.2750156
-1980.80   0.0270202   0.2752391
-1980.85   0.0271422   0.2754610
-1980.90   0.0272646   0.2756810
-1980.95   0.0273874   0.2758993
-1981.00   0.0275105   0.2761159
-1981.05   0.0276339   0.2763307
-1981.10   0.0277576   0.2765437
-1981.15   0.0278816   0.2767550
-1981.20   0.0280059   0.2769646
-1981.25   0.0281305   0.2771724
-1981.30   0.0282553   0.2773786
-1981.35   0.0283804   0.2775830
-1981.40   0.0285056   0.2777857
-1981.45   0.0286311   0.2779867
-1981.50   0.0287568   0.2781861
-1981.55   0.0288827   0.2783838
-1981.60   0.0290087   0.2785798
-1981.65   0.0291349   0.2787742
-1981.70   0.0292611   0.2789670
-1981.75   0.0293875   0.2791583
-1981.80   0.0295140   0.2793479
-1981.85   0.0296405   0.2795359
-1981.90   0.0297671   0.2797224
-1981.95   0.0298937   0.2799074
-1982.00   0.0300204   0.2800909
-1982.05   0.0301470   0.2802729
-1982.10   0.0302736   0.2804535
-1982.15   0.0304002   0.2806326
-1982.20   0.0305267   0.2808103
-1982.25   0.0306531   0.2809866
-1982.30   0.0307794   0.2811615
-1982.35   0.0309056   0.2813351
-1982.40   0.0310316   0.2815074
-1982.45   0.0311575   0.2816784
-1982.50   0.0312831   0.2818482
-1982.55   0.0314086   0.2820167
-1982.60   0.0315339   0.2821841
-1982.65   0.0316588   0.2823503
-1982.70   0.0317836   0.2825153
-1982.75   0.0319080   0.2826792
-1982.80   0.0320321   0.2828421
-1982.85   0.0321559   0.2830039
-1982.90   0.0322794   0.2831647
-1982.95   0.0324025   0.2833246
-1983.00   0.0325252   0.2834835
-1983.05   0.0326474   0.2836414
-1983.10   0.0327693   0.2837986
-1983.15   0.0328907   0.2839549
-1983.20   0.0330116   0.2841103
-1983.25   0.0331320   0.2842651
-1983.30   0.0332519   0.2844191
-1983.35   0.0333713   0.2845724
-1983.40   0.0334901   0.2847250
-1983.45   0.0336083   0.2848770
-1983.50   0.0337260   0.2850285
-1983.55   0.0338430   0.2851794
-1983.60   0.0339595   0.2853298
-1983.65   0.0340752   0.2854798
-1983.70   0.0341903   0.2856293
-1983.75   0.0343047   0.2857784
-1983.80   0.0344185   0.2859272
-1983.85   0.0345315   0.2860756
-1983.90   0.0346437   0.2862238
-1983.95   0.0347552   0.2863718
-1984.00   0.0348660   0.2865195
-1984.05   0.0349759   0.2866671
-1984.10   0.0350850   0.2868146
-1984.15   0.0351934   0.2869620
-1984.20   0.0353009   0.2871093
-1984.25   0.0354075   0.2872567
-1984.30   0.0355133   0.2874041
-1984.35   0.0356181   0.2875515
-1984.40   0.0357221   0.2876991
-1984.45   0.0358252   0.2878468
-1984.50   0.0359274   0.2879946
-1984.55   0.0360286   0.2881427
-1984.60   0.0361288   0.2882911
-1984.65   0.0362281   0.2884397
-1984.70   0.0363265   0.2885887
-1984.75   0.0364238   0.2887380
-1984.80   0.0365201   0.2888877
-1984.85   0.0366155   0.2890379
-1984.90   0.0367098   0.2891885
-1984.95   0.0368030   0.2893396
-1985.00   0.0368953   0.2894912
-1985.05   0.0369865   0.2896434
-1985.10   0.0370766   0.2897962
-1985.15   0.0371656   0.2899496
-1985.20   0.0372536   0.2901037
-1985.25   0.0373405   0.2902584
-1985.30   0.0374262   0.2904139
-1985.35   0.0375109   0.2905701
-1985.40   0.0375945   0.2907271
-1985.45   0.0376769   0.2908848
-1985.50   0.0377582   0.2910434
-1985.55   0.0378384   0.2912029
-1985.60   0.0379175   0.2913632
-1985.65   0.0379954   0.2915244
-1985.70   0.0380722   0.2916865
-1985.75   0.0381478   0.2918496
-1985.80   0.0382222   0.2920136
-1985.85   0.0382955   0.2921786
-1985.90   0.0383677   0.2923446
-1985.95   0.0384386   0.2925117
-1986.00   0.0385084   0.2926797
-1986.05   0.0385770   0.2928489
-1986.10   0.0386445   0.2930191
-1986.15   0.0387107   0.2931904
-1986.20   0.0387758   0.2933628
-1986.25   0.0388397   0.2935363
-1986.30   0.0389025   0.2937110
-1986.35   0.0389640   0.2938868
-1986.40   0.0390243   0.2940638
-1986.45   0.0390835   0.2942419
-1986.50   0.0391415   0.2944212
-1986.55   0.0391983   0.2946017
-1986.60   0.0392539   0.2947834
-1986.65   0.0393084   0.2949663
-1986.70   0.0393617   0.2951504
-1986.75   0.0394137   0.2953356
-1986.80   0.0394646   0.2955221
-1986.85   0.0395144   0.2957099
-1986.90   0.0395629   0.2958988
-1986.95   0.0396103   0.2960889
-1987.00   0.0396566   0.2962803
-1987.05   0.0397016   0.2964729
-1987.10   0.0397455   0.2966667
-1987.15   0.0397883   0.2968617
-1987.20   0.0398298   0.2970579
-1987.25   0.0398703   0.2972553
-1987.30   0.0399096   0.2974539
-1987.35   0.0399477   0.2976538
-1987.40   0.0399847   0.2978547
-1987.45   0.0400206   0.2980569
-1987.50   0.0400554   0.2982603
-1987.55   0.0400890   0.2984648
-1987.60   0.0401215   0.2986704
-1987.65   0.0401529   0.2988772
-1987.70   0.0401832   0.2990851
-1987.75   0.0402124   0.2992941
-1987.80   0.0402405   0.2995042
-1987.85   0.0402675   0.2997154
-1987.90   0.0402934   0.2999277
-1987.95   0.0403183   0.3001410
-1988.00   0.0403421   0.3003554
-1988.05   0.0403648   0.3005707
-1988.10   0.0403864   0.3007871
-1988.15   0.0404070   0.3010045
-1988.20   0.0404266   0.3012228
-1988.25   0.0404451   0.3014420
-1988.30   0.0404626   0.3016622
-1988.35   0.0404791   0.3018833
-1988.40   0.0404946   0.3021053
-1988.45   0.0405091   0.3023281
-1988.50   0.0405225   0.3025517
-1988.55   0.0405350   0.3027762
-1988.60   0.0405465   0.3030014
-1988.65   0.0405571   0.3032274
-1988.70   0.0405666   0.3034541
-1988.75   0.0405753   0.3036816
-1988.80   0.0405829   0.3039097
-1988.85   0.0405896   0.3041385
-1988.90   0.0405954   0.3043679
-1988.95   0.0406003   0.3045979
-1989.00   0.0406043   0.3048284
-1989.05   0.0406074   0.3050596
-1989.10   0.0406095   0.3052912
-1989.15   0.0406108   0.3055233
-1989.20   0.0406113   0.3057559
-1989.25   0.0406108   0.3059889
-1989.30   0.0406095   0.3062223
-1989.35   0.0406074   0.3064561
-1989.40   0.0406044   0.3066902
-1989.45   0.0406006   0.3069246
-1989.50   0.0405960   0.3071593
-1989.55   0.0405906   0.3073943
-1989.60   0.0405845   0.3076294
-1989.65   0.0405775   0.3078648
-1989.70   0.0405698   0.3081003
-1989.75   0.0405613   0.3083359
-1989.80   0.0405520   0.3085716
-1989.85   0.0405421   0.3088073
-1989.90   0.0405314   0.3090431
-1989.95   0.0405200   0.3092789
-1990.00   0.0405079   0.3095146
-1990.05   0.0404951   0.3097503
-1990.10   0.0404816   0.3099858
-1990.15   0.0404675   0.3102212
-1990.20   0.0404527   0.3104565
-1990.25   0.0404373   0.3106915
-1990.30   0.0404213   0.3109264
-1990.35   0.0404046   0.3111609
-1990.40   0.0403874   0.3113952
-1990.45   0.0403696   0.3116291
-1990.50   0.0403512   0.3118627
-1990.55   0.0403322   0.3120958
-1990.60   0.0403127   0.3123286
-1990.65   0.0402927   0.3125609
-1990.70   0.0402722   0.3127927
-1990.75   0.0402512   0.3130240
-1990.80   0.0402296   0.3132548
-1990.85   0.0402077   0.3134850
-1990.90   0.0401852   0.3137146
-1990.95   0.0401623   0.3139435
-1991.00   0.0401390   0.3141718
-1991.05   0.0401153   0.3143994
-1991.10   0.0400912   0.3146263
-1991.15   0.0400667   0.3148524
-1991.20   0.0400419   0.3150777
-1991.25   0.0400167   0.3153023
-1991.30   0.0399911   0.3155260
-1991.35   0.0399653   0.3157488
-1991.40   0.0399391   0.3159708
-1991.45   0.0399127   0.3161918
-1991.50   0.0398860   0.3164119
-1991.55   0.0398591   0.3166310
-1991.60   0.0398319   0.3168492
-1991.65   0.0398046   0.3170663
-1991.70   0.0397770   0.3172824
-1991.75   0.0397492   0.3174974
-1991.80   0.0397213   0.3177113
-1991.85   0.0396933   0.3179241
-1991.90   0.0396651   0.3181358
-1991.95   0.0396368   0.3183463
-1992.00   0.0396084   0.3185557
-1992.05   0.0395800   0.3187638
-1992.10   0.0395515   0.3189708
-1992.15   0.0395229   0.3191764
-1992.20   0.0394944   0.3193809
-1992.25   0.0394658   0.3195840
-1992.30   0.0394373   0.3197858
-1992.35   0.0394088   0.3199864
-1992.40   0.0393804   0.3201856
-1992.45   0.0393521   0.3203834
-1992.50   0.0393238   0.3205799
-1992.55   0.0392957   0.3207750
-1992.60   0.0392677   0.3209687
-1992.65   0.0392398   0.3211609
-1992.70   0.0392121   0.3213518
-1992.75   0.0391846   0.3215412
-1992.80   0.0391573   0.3217292
-1992.85   0.0391303   0.3219156
-1992.90   0.0391035   0.3221007
-1992.95   0.0390769   0.3222842
-1993.00   0.0390507   0.3224662
-1993.05   0.0390247   0.3226467
-1993.10   0.0389991   0.3228257
-1993.15   0.0389738   0.3230031
-1993.20   0.0389489   0.3231791
-1993.25   0.0389243   0.3233534
-1993.30   0.0389002   0.3235263
-1993.35   0.0388764   0.3236975
-1993.40   0.0388531   0.3238672
-1993.45   0.0388303   0.3240353
-1993.50   0.0388079   0.3242019
-1993.55   0.0387860   0.3243669
-1993.60   0.0387646   0.3245303
-1993.65   0.0387438   0.3246921
-1993.70   0.0387234   0.3248523
-1993.75   0.0387037   0.3250110
-1993.80   0.0386845   0.3251680
-1993.85   0.0386659   0.3253235
-1993.90   0.0386479   0.3254773
-1993.95   0.0386305   0.3256296
-1994.00   0.0386138   0.3257803
-1994.05   0.0385978   0.3259294
-1994.10   0.0385824   0.3260770
-1994.15   0.0385677   0.3262229
-1994.20   0.0385537   0.3263673
-1994.25   0.0385405   0.3265102
-1994.30   0.0385280   0.3266514
-1994.35   0.0385162   0.3267911
-1994.40   0.0385052   0.3269293
-1994.45   0.0384950   0.3270659
-1994.50   0.0384856   0.3272009
-1994.55   0.0384770   0.3273345
-1994.60   0.0384692   0.3274665
-1994.65   0.0384623   0.3275970
-1994.70   0.0384562   0.3277260
-1994.75   0.0384510   0.3278535
-1994.80   0.0384467   0.3279796
-1994.85   0.0384432   0.3281041
-1994.90   0.0384407   0.3282273
-1994.95   0.0384390   0.3283489
-1995.00   0.0384383   0.3284692
-1995.05   0.0384386   0.3285880
-1995.10   0.0384397   0.3287054
-1995.15   0.0384419   0.3288214
-1995.20   0.0384450   0.3289361
-1995.25   0.0384490   0.3290494
-1995.30   0.0384541   0.3291613
-1995.35   0.0384601   0.3292720
-1995.40   0.0384672   0.3293813
-1995.45   0.0384753   0.3294893
-1995.50   0.0384844   0.3295961
-1995.55   0.0384945   0.3297015
-1995.60   0.0385056   0.3298058
-1995.65   0.0385178   0.3299088
-1995.70   0.0385311   0.3300107
-1995.75   0.0385454   0.3301113
-1995.80   0.0385607   0.3302108
-1995.85   0.0385772   0.3303091
-1995.90   0.0385947   0.3304063
-1995.95   0.0386132   0.3305024
-1996.00   0.0386329   0.3305975
-1996.05   0.0386536   0.3306914
-1996.10   0.0386755   0.3307844
-1996.15   0.0386984   0.3308763
-1996.20   0.0387224   0.3309672
-1996.25   0.0387475   0.3310572
-1996.30   0.0387737   0.3311462
-1996.35   0.0388010   0.3312343
-1996.40   0.0388295   0.3313214
-1996.45   0.0388590   0.3314077
-1996.50   0.0388896   0.3314932
-1996.55   0.0389213   0.3315778
-1996.60   0.0389542   0.3316615
-1996.65   0.0389881   0.3317446
-1996.70   0.0390232   0.3318268
-1996.75   0.0390593   0.3319083
-1996.80   0.0390966   0.3319891
-1996.85   0.0391350   0.3320692
-1996.90   0.0391744   0.3321486
-1996.95   0.0392150   0.3322274
-1997.00   0.0392567   0.3323056
-1997.05   0.0392994   0.3323831
-1997.10   0.0393433   0.3324601
-1997.15   0.0393882   0.3325366
-1997.20   0.0394342   0.3326125
-1997.25   0.0394813   0.3326879
-1997.30   0.0395295   0.3327629
-1997.35   0.0395788   0.3328374
-1997.40   0.0396291   0.3329115
-1997.45   0.0396804   0.3329852
-1997.50   0.0397329   0.3330585
-1997.55   0.0397864   0.3331314
-1997.60   0.0398409   0.3332040
-1997.65   0.0398965   0.3332763
-1997.70   0.0399531   0.3333483
-1997.75   0.0400107   0.3334201
-1997.80   0.0400694   0.3334916
-1997.85   0.0401291   0.3335629
-1997.90   0.0401897   0.3336340
-1997.95   0.0402514   0.3337049
-1998.00   0.0403141   0.3337756
-1998.05   0.0403778   0.3338463
-1998.10   0.0404424   0.3339168
-1998.15   0.0405080   0.3339872
-1998.20   0.0405746   0.3340575
-1998.25   0.0406421   0.3341278
-1998.30   0.0407106   0.3341981
-1998.35   0.0407801   0.3342684
-1998.40   0.0408504   0.3343386
-1998.45   0.0409217   0.3344089
-1998.50   0.0409939   0.3344793
-1998.55   0.0410670   0.3345497
-1998.60   0.0411410   0.3346202
-1998.65   0.0412159   0.3346907
-1998.70   0.0412917   0.3347614
-1998.75   0.0413683   0.3348323
-1998.80   0.0414458   0.3349032
-1998.85   0.0415242   0.3349743
-1998.90   0.0416034   0.3350456
-1998.95   0.0416834   0.3351171
-1999.00   0.0417643   0.3351888
-1999.05   0.0418460   0.3352607
-1999.10   0.0419285   0.3353329
-1999.15   0.0420118   0.3354053
-1999.20   0.0420959   0.3354779
-1999.25   0.0421808   0.3355508
-1999.30   0.0422664   0.3356240
-1999.35   0.0423529   0.3356975
-1999.40   0.0424401   0.3357712
-1999.45   0.0425280   0.3358453
-1999.50   0.0426167   0.3359197
-1999.55   0.0427062   0.3359944
-1999.60   0.0427963   0.3360694
-1999.65   0.0428872   0.3361447
-1999.70   0.0429788   0.3362204
-1999.75   0.0430711   0.3362965
-1999.80   0.0431641   0.3363729
-1999.85   0.0432578   0.3364496
-1999.90   0.0433522   0.3365268
-1999.95   0.0434473   0.3366042
-2000.00   0.0435431   0.3366821
-2000.05   0.0436395   0.3367603
-2000.10   0.0437366   0.3368389
-2000.15   0.0438344   0.3369178
-2000.20   0.0439328   0.3369972
-2000.25   0.0440318   0.3370769
-2000.30   0.0441315   0.3371569
-2000.35   0.0442319   0.3372373
-2000.40   0.0443329   0.3373181
-2000.45   0.0444345   0.3373993
-2000.50   0.0445368   0.3374808
-2000.55   0.0446396   0.3375627
-2000.60   0.0447431   0.3376449
-2000.65   0.0448473   0.3377274
-2000.70   0.0449520   0.3378103
-2000.75   0.0450574   0.3378936
-2000.80   0.0451634   0.3379771
-2000.85   0.0452700   0.3380610
-2000.90   0.0453772   0.3381452
-2000.95   0.0454850   0.3382296
-2001.00   0.0455935   0.3383144
-2001.05   0.0457025   0.3383995
-2001.10   0.0458122   0.3384848
-2001.15   0.0459225   0.3385703
-2001.20   0.0460334   0.3386562
-2001.25   0.0461450   0.3387422
-2001.30   0.0462572   0.3388285
-2001.35   0.0463699   0.3389150
-2001.40   0.0464834   0.3390017
-2001.45   0.0465974   0.3390885
-2001.50   0.0467121   0.3391756
-2001.55   0.0468275   0.3392627
-2001.60   0.0469434   0.3393501
-2001.65   0.0470601   0.3394375
-2001.70   0.0471774   0.3395250
-2001.75   0.0472953   0.3396127
-2001.80   0.0474139   0.3397004
-2001.85   0.0475332   0.3397881
-2001.90   0.0476532   0.3398759
-2001.95   0.0477739   0.3399637
-2002.00   0.0478952   0.3400515
-2002.05   0.0480173   0.3401392
-2002.10   0.0481401   0.3402269
-2002.15   0.0482635   0.3403146
-2002.20   0.0483878   0.3404022
-2002.25   0.0485127   0.3404896
-2002.30   0.0486384   0.3405770
-2002.35   0.0487649   0.3406642
-2002.40   0.0488921   0.3407512
-2002.45   0.0490201   0.3408381
-2002.50   0.0491489   0.3409247
-2002.55   0.0492784   0.3410111
-2002.60   0.0494088   0.3410972
-2002.65   0.0495400   0.3411831
-2002.70   0.0496721   0.3412687
-2002.75   0.0498050   0.3413539
-2002.80   0.0499387   0.3414388
-2002.85   0.0500733   0.3415234
-2002.90   0.0502088   0.3416075
-2002.95   0.0503451   0.3416913
-2003.00   0.0504824   0.3417746
-2003.05   0.0506206   0.3418574
-2003.10   0.0507597   0.3419398
-2003.15   0.0508997   0.3420217
-2003.20   0.0510407   0.3421030
-2003.25   0.0511827   0.3421838
-2003.30   0.0513257   0.3422641
-2003.35   0.0514696   0.3423437
-2003.40   0.0516145   0.3424228
-2003.45   0.0517605   0.3425011
-2003.50   0.0519075   0.3425789
-2003.55   0.0520555   0.3426559
-2003.60   0.0522046   0.3427323
-2003.65   0.0523548   0.3428079
-2003.70   0.0525060   0.3428828
-2003.75   0.0526584   0.3429570
-2003.80   0.0528118   0.3430303
-2003.85   0.0529664   0.3431029
-2003.90   0.0531221   0.3431746
-2003.95   0.0532789   0.3432455
-2004.00   0.0534369   0.3433155
-2004.05   0.0535961   0.3433846
-2004.10   0.0537564   0.3434529
-2004.15   0.0539180   0.3435202
-2004.20   0.0540807   0.3435866
-2004.25   0.0542447   0.3436521
-2004.30   0.0544098   0.3437166
-2004.35   0.0545763   0.3437801
-2004.40   0.0547439   0.3438426
-2004.45   0.0549128   0.3439041
-2004.50   0.0550830   0.3439646
-2004.55   0.0552544   0.3440240
-2004.60   0.0554271   0.3440824
-2004.65   0.0556011   0.3441397
-2004.70   0.0557764   0.3441960
-2004.75   0.0559530   0.3442512
-2004.80   0.0561309   0.3443052
-2004.85   0.0563101   0.3443582
-2004.90   0.0564907   0.3444100
-2004.95   0.0566725   0.3444608
-2005.00   0.0568557   0.3445104
-2005.05   0.0570402   0.3445588
-2005.10   0.0572261   0.3446061
-2005.15   0.0574133   0.3446523
-2005.20   0.0576019   0.3446973
-2005.25   0.0577918   0.3447411
-2005.30   0.0579830   0.3447838
-2005.35   0.0581756   0.3448253
-2005.40   0.0583695   0.3448657
-2005.45   0.0585648   0.3449049
-2005.50   0.0587615   0.3449429
-2005.55   0.0589595   0.3449797
-2005.60   0.0591588   0.3450154
-2005.65   0.0593595   0.3450499
-2005.70   0.0595615   0.3450833
-2005.75   0.0597648   0.3451155
-2005.80   0.0599695   0.3451465
-2005.85   0.0601755   0.3451764
-2005.90   0.0603828   0.3452051
-2005.95   0.0605915   0.3452327
-2006.00   0.0608014   0.3452592
-2006.05   0.0610127   0.3452846
-2006.10   0.0612252   0.3453089
-2006.15   0.0614390   0.3453320
-2006.20   0.0616541   0.3453541
-2006.25   0.0618705   0.3453751
-2006.30   0.0620881   0.3453950
-2006.35   0.0623070   0.3454139
-2006.40   0.0625271   0.3454317
-2006.45   0.0627484   0.3454486
-2006.50   0.0629709   0.3454644
-2006.55   0.0631946   0.3454792
-2006.60   0.0634194   0.3454931
-2006.65   0.0636455   0.3455060
-2006.70   0.0638727   0.3455179
-2006.75   0.0641010   0.3455290
-2006.80   0.0643304   0.3455391
-2006.85   0.0645609   0.3455484
-2006.90   0.0647925   0.3455569
-2006.95   0.0650252   0.3455645
-2007.00   0.0652589   0.3455713
-2007.05   0.0654936   0.3455773
-2007.10   0.0657294   0.3455825
-2007.15   0.0659661   0.3455870
-2007.20   0.0662038   0.3455909
-2007.25   0.0664424   0.3455940
-2007.30   0.0666820   0.3455964
-2007.35   0.0669224   0.3455983
-2007.40   0.0671637   0.3455995
-2007.45   0.0674059   0.3456002
-2007.50   0.0676489   0.3456003
-2007.55   0.0678928   0.3455999
-2007.60   0.0681374   0.3455990
-2007.65   0.0683828   0.3455977
-2007.70   0.0686289   0.3455959
-2007.75   0.0688757   0.3455938
-2007.80   0.0691232   0.3455913
-2007.85   0.0693714   0.3455884
-2007.90   0.0696203   0.3455852
-2007.95   0.0698697   0.3455818
-2008.00   0.0701197   0.3455782
-2008.05   0.0703703   0.3455743
-2008.10   0.0706215   0.3455703
-2008.15   0.0708731   0.3455661
-2008.20   0.0711253   0.3455618
-2008.25   0.0713779   0.3455575
-2008.30   0.0716310   0.3455531
-2008.35   0.0718844   0.3455487
-2008.40   0.0721383   0.3455444
-2008.45   0.0723925   0.3455401
-2008.50   0.0726470   0.3455359
-2008.55   0.0729019   0.3455318
-2008.60   0.0731570   0.3455279
-2008.65   0.0734124   0.3455242
-2008.70   0.0736680   0.3455208
-2008.75   0.0739239   0.3455176
-2008.80   0.0741799   0.3455147
-2008.85   0.0744361   0.3455121
-2008.90   0.0746924   0.3455099
-2008.95   0.0749488   0.3455081
-2009.00   0.0752053   0.3455067
-2009.05   0.0754619   0.3455057
-2009.10   0.0757185   0.3455053
-2009.15   0.0759751   0.3455054
-2009.20   0.0762318   0.3455060
-2009.25   0.0764884   0.3455072
-2009.30   0.0767449   0.3455091
-2009.35   0.0770014   0.3455115
-2009.40   0.0772577   0.3455147
-2009.45   0.0775140   0.3455185
-2009.50   0.0777701   0.3455231
-2009.55   0.0780261   0.3455284
-2009.60   0.0782818   0.3455345
-2009.65   0.0785374   0.3455415
-2009.70   0.0787928   0.3455492
-2009.75   0.0790479   0.3455578
-2009.80   0.0793028   0.3455673
-2009.85   0.0795574   0.3455777
-2009.90   0.0798117   0.3455891
-2009.95   0.0800657   0.3456014
-2010.00   0.0803194   0.3456146
-2010.05   0.0805728   0.3456289
-2010.10   0.0808258   0.3456442
-2010.15   0.0810784   0.3456605
-2010.20   0.0813307   0.3456778
-2010.25   0.0815826   0.3456963
-2010.30   0.0818340   0.3457158
-2010.35   0.0820851   0.3457364
-2010.40   0.0823357   0.3457581
-2010.45   0.0825859   0.3457810
-2010.50   0.0828356   0.3458050
-2010.55   0.0830849   0.3458302
-2010.60   0.0833337   0.3458565
-2010.65   0.0835820   0.3458840
-2010.70   0.0838298   0.3459127
-2010.75   0.0840771   0.3459426
-2010.80   0.0843239   0.3459737
-2010.85   0.0845702   0.3460060
-2010.90   0.0848160   0.3460395
-2010.95   0.0850612   0.3460742
-2011.00   0.0853060   0.3461101
-2011.05   0.0855502   0.3461473
-2011.10   0.0857938   0.3461857
-2011.15   0.0860369   0.3462253
-2011.20   0.0862795   0.3462662
-2011.25   0.0865215   0.3463083
-2011.30   0.0867630   0.3463516
-2011.35   0.0870039   0.3463961
-2011.40   0.0872442   0.3464418
-2011.45   0.0874841   0.3464888
-2011.50   0.0877233   0.3465369
-2011.55   0.0879620   0.3465862
-2011.60   0.0882001   0.3466368
-2011.65   0.0884377   0.3466885
-2011.70   0.0886747   0.3467413
-2011.75   0.0889112   0.3467953
-2011.80   0.0891471   0.3468505
-2011.85   0.0893825   0.3469068
-2011.90   0.0896174   0.3469642
-2011.95   0.0898516   0.3470227
-2012.00   0.0900854   0.3470823
-2012.05   0.0903186   0.3471430
-2012.10   0.0905513   0.3472047
-2012.15   0.0907835   0.3472675
-2012.20   0.0910151   0.3473312
-2012.25   0.0912463   0.3473960
-2012.30   0.0914769   0.3474617
-2012.35   0.0917070   0.3475284
-2012.40   0.0919366   0.3475960
-2012.45   0.0921657   0.3476646
-2012.50   0.0923943   0.3477340
-2012.55   0.0926225   0.3478043
-2012.60   0.0928501   0.3478754
-2012.65   0.0930773   0.3479473
-2012.70   0.0933040   0.3480201
-2012.75   0.0935303   0.3480935
-2012.80   0.0937561   0.3481677
-2012.85   0.0939815   0.3482427
-2012.90   0.0942064   0.3483183
-2012.95   0.0944309   0.3483945
-2013.00   0.0946550   0.3484714
-2013.05   0.0948786   0.3485488
-2013.10   0.0951019   0.3486268
-2013.15   0.0953247   0.3487054
-2013.20   0.0955471   0.3487844
-2013.25   0.0957692   0.3488639
-2013.30   0.0959908   0.3489439
-2013.35   0.0962121   0.3490242
-2013.40   0.0964330   0.3491050
-2013.45   0.0966535   0.3491860
-2013.50   0.0968736   0.3492674
-2013.55   0.0970934   0.3493491
-2013.60   0.0973129   0.3494310
-2013.65   0.0975320   0.3495132
-2013.70   0.0977507   0.3495955
-2013.75   0.0979691   0.3496780
-2013.80   0.0981872   0.3497606
-2013.85   0.0984050   0.3498433
-2013.90   0.0986224   0.3499260
-2013.95   0.0988395   0.3500088
-2014.00   0.0990563   0.3500915
-2014.05   0.0992728   0.3501743
-2014.10   0.0994890   0.3502569
-2014.15   0.0997048   0.3503395
-2014.20   0.0999204   0.3504219
-2014.25   0.1001356   0.3505041
-2014.30   0.1003506   0.3505862
-2014.35   0.1005653   0.3506680
-2014.40   0.1007796   0.3507496
-2014.45   0.1009937   0.3508309
-2014.50   0.1012074   0.3509119
-2014.55   0.1014209   0.3509926
-2014.60   0.1016341   0.3510728
-2014.65   0.1018469   0.3511527
-2014.70   0.1020595   0.3512322
-2014.75   0.1022718   0.3513112
-2014.80   0.1024838   0.3513897
-2014.85   0.1026954   0.3514677
-2014.90   0.1029068   0.3515452
-2014.95   0.1031178   0.3516221
-2015.00   0.1033286   0.3516985
-2015.05   0.1035390   0.3517742
-2015.10   0.1037491   0.3518493
-2015.15   0.1039589   0.3519238
-2015.20   0.1041683   0.3519976
-2015.25   0.1043775   0.3520707
-2015.30   0.1045863   0.3521431
-2015.35   0.1047947   0.3522148
-2015.40   0.1050028   0.3522857
-2015.45   0.1052105   0.3523558
-2015.50   0.1054179   0.3524251
-2015.55   0.1056249   0.3524937
-2015.60   0.1058315   0.3525614
-2015.65   0.1060377   0.3526283
-2015.70   0.1062436   0.3526943
-2015.75   0.1064490   0.3527595
-2015.80   0.1066540   0.3528237
-2015.85   0.1068586   0.3528871
-2015.90   0.1070628   0.3529496
-2015.95   0.1072665   0.3530111
-2016.00   0.1074698   0.3530718
-2016.05   0.1076726   0.3531314
-2016.10   0.1078749   0.3531902
-2016.15   0.1080768   0.3532479
-2016.20   0.1082782   0.3533047
-2016.25   0.1084790   0.3533606
-2016.30   0.1086794   0.3534154
-2016.35   0.1088792   0.3534693
-2016.40   0.1090785   0.3535222
-2016.45   0.1092772   0.3535740
-2016.50   0.1094753   0.3536249
-2016.55   0.1096729   0.3536748
-2016.60   0.1098699   0.3537237
-2016.65   0.1100663   0.3537715
-2016.70   0.1102620   0.3538184
-2016.75   0.1104572   0.3538642
-2016.80   0.1106516   0.3539090
-2016.85   0.1108455   0.3539529
-2016.90   0.1110386   0.3539957
-2016.95   0.1112311   0.3540375
-2017.00   0.1114228   0.3540783
-2017.05   0.1116139   0.3541181
-2017.10   0.1118042   0.3541569
-2017.15   0.1119938   0.3541947
-2017.20   0.1121826   0.3542316
-2017.25   0.1123707   0.3542674
-2017.30   0.1125579   0.3543023
-2017.35   0.1127444   0.3543362
-2017.40   0.1129300   0.3543691
-2017.45   0.1131149   0.3544011
-2017.50   0.1132988   0.3544322
-2017.55   0.1134820   0.3544623
-2017.60   0.1136642   0.3544914
-2017.65   0.1138456   0.3545197
-2017.70   0.1140260   0.3545470
-2017.75   0.1142056   0.3545734
-2017.80   0.1143842   0.3545989
-2017.85   0.1145619   0.3546236
-2017.90   0.1147386   0.3546473
-2017.95   0.1149144   0.3546702
-2018.00   0.1150892   0.3546923
-2018.05   0.1152630   0.3547135
-2018.10   0.1154357   0.3547339
-2018.15   0.1156075   0.3547534
-2018.20   0.1157782   0.3547722
-2018.25   0.1159479   0.3547901
-2018.30   0.1161165   0.3548073
-2018.35   0.1162841   0.3548237
-2018.40   0.1164506   0.3548394
-2018.45   0.1166160   0.3548543
-2018.50   0.1167802   0.3548685
-2018.55   0.1169434   0.3548819
-2018.60   0.1171054   0.3548947
-2018.65   0.1172663   0.3549068
-2018.70   0.1174260   0.3549182
-2018.75   0.1175846   0.3549289
-2018.80   0.1177420   0.3549390
-2018.85   0.1178982   0.3549484
-2018.90   0.1180533   0.3549573
-2018.95   0.1182071   0.3549655
-2019.00   0.1183597   0.3549731
-2019.05   0.1185111   0.3549802
-2019.10   0.1186613   0.3549867
-2019.15   0.1188103   0.3549926
-2019.20   0.1189580   0.3549980
-2019.25   0.1191044   0.3550029
-2019.30   0.1192496   0.3550072
-2019.35   0.1193935   0.3550111
-2019.40   0.1195362   0.3550145
-2019.45   0.1196775   0.3550174
-2019.50   0.1198176   0.3550198
-2019.55   0.1199564   0.3550218
-2019.60   0.1200939   0.3550234
-2019.65   0.1202301   0.3550246
-2019.70   0.1203649   0.3550253
-2019.75   0.1204985   0.3550257
-2019.80   0.1206308   0.3550257
-2019.85   0.1207617   0.3550253
-2019.90   0.1208913   0.3550246
-2019.95   0.1210195   0.3550235
-2020.00   0.1211464   0.3550221
-2020.05   0.1212720   0.3550204
-2020.10   0.1213963   0.3550184
-2020.15   0.1215192   0.3550161
-2020.20   0.1216407   0.3550135
-2020.25   0.1217609   0.3550106
-2020.30   0.1218797   0.3550075
-2020.35   0.1219972   0.3550041
-2020.40   0.1221134   0.3550005
-2020.45   0.1222282   0.3549967
-2020.50   0.1223416   0.3549926
-2020.55   0.1224537   0.3549884
-2020.60   0.1225644   0.3549839
-2020.65   0.1226737   0.3549793
-2020.70   0.1227817   0.3549745
-2020.75   0.1228883   0.3549695
-2020.80   0.1229936   0.3549644
-2020.85   0.1230975   0.3549591
-2020.90   0.1232001   0.3549537
-2020.95   0.1233013   0.3549482
-2021.00   0.1234012   0.3549425
-2021.05   0.1234997   0.3549368
-2021.10   0.1235969   0.3549309
-2021.15   0.1236927   0.3549249
-2021.20   0.1237871   0.3549189
-2021.25   0.1238803   0.3549128
-2021.30   0.1239720   0.3549066
-2021.35   0.1240625   0.3549004
-2021.40   0.1241516   0.3548941
-2021.45   0.1242394   0.3548877
-2021.50   0.1243259   0.3548814
-2021.55   0.1244110   0.3548750
-2021.60   0.1244948   0.3548685
-2021.65   0.1245773   0.3548621
-2021.70   0.1246585   0.3548556
-2021.75   0.1247384   0.3548492
-2021.80   0.1248170   0.3548427
-2021.85   0.1248943   0.3548362
-2021.90   0.1249703   0.3548298
-2021.95   0.1250450   0.3548234
-2022.00   0.1251185   0.3548170
-2022.05   0.1251906   0.3548106
-2022.10   0.1252615   0.3548043
-2022.15   0.1253311   0.3547980
-2022.20   0.1253995   0.3547918
-2022.25   0.1254666   0.3547856
-2022.30   0.1255324   0.3547795
-2022.35   0.1255970   0.3547735
-2022.40   0.1256604   0.3547675
-2022.45   0.1257226   0.3547616
-2022.50   0.1257835   0.3547557
-2022.55   0.1258432   0.3547500
-2022.60   0.1259017   0.3547443
-2022.65   0.1259590   0.3547387
-2022.70   0.1260151   0.3547332
-2022.75   0.1260699   0.3547278
-2022.80   0.1261237   0.3547226
-2022.85   0.1261762   0.3547174
-2022.90   0.1262275   0.3547123
-2022.95   0.1262777   0.3547073
-2023.00   0.1263268   0.3547025
-2023.05   0.1263747   0.3546978
-2023.10   0.1264214   0.3546932
-2023.15   0.1264670   0.3546887
-2023.20   0.1265115   0.3546844
-2023.25   0.1265549   0.3546802
-2023.30   0.1265971   0.3546761
-2023.35   0.1266382   0.3546722
-2023.40   0.1266783   0.3546684
-2023.45   0.1267172   0.3546647
-2023.50   0.1267551   0.3546612
+1972.05   0.0059567   0.2256436
+1972.10   0.0061093   0.2258845
+1972.15   0.0062621   0.2261266
+1972.20   0.0064149   0.2263698
+1972.25   0.0065677   0.2266141
+1972.30   0.0067206   0.2268595
+1972.35   0.0068734   0.2271060
+1972.40   0.0070262   0.2273537
+1972.45   0.0071789   0.2276024
+1972.50   0.0073316   0.2278523
+1972.55   0.0074841   0.2281033
+1972.60   0.0076365   0.2283554
+1972.65   0.0077888   0.2286086
+1972.70   0.0079408   0.2288629
+1972.75   0.0080927   0.2291183
+1972.80   0.0082443   0.2293749
+1972.85   0.0083957   0.2296325
+1972.90   0.0085468   0.2298912
+1972.95   0.0086976   0.2301510
+1973.00   0.0088481   0.2304119
+1973.05   0.0089983   0.2306739
+1973.10   0.0091481   0.2309370
+1973.15   0.0092975   0.2312012
+1973.20   0.0094465   0.2314664
+1973.25   0.0095951   0.2317328
+1973.30   0.0097433   0.2320002
+1973.35   0.0098910   0.2322687
+1973.40   0.0100382   0.2325382
+1973.45   0.0101849   0.2328089
+1973.50   0.0103311   0.2330806
+1973.55   0.0104768   0.2333533
+1973.60   0.0106219   0.2336271
+1973.65   0.0107664   0.2339020
+1973.70   0.0109104   0.2341779
+1973.75   0.0110538   0.2344548
+1973.80   0.0111965   0.2347328
+1973.85   0.0113386   0.2350118
+1973.90   0.0114801   0.2352918
+1973.95   0.0116209   0.2355728
+1974.00   0.0117611   0.2358549
+1974.05   0.0119005   0.2361379
+1974.10   0.0120393   0.2364219
+1974.15   0.0121774   0.2367069
+1974.20   0.0123147   0.2369929
+1974.25   0.0124514   0.2372798
+1974.30   0.0125873   0.2375677
+1974.35   0.0127225   0.2378566
+1974.40   0.0128569   0.2381463
+1974.45   0.0129906   0.2384370
+1974.50   0.0131235   0.2387286
+1974.55   0.0132556   0.2390211
+1974.60   0.0133870   0.2393145
+1974.65   0.0135176   0.2396088
+1974.70   0.0136475   0.2399039
+1974.75   0.0137765   0.2401999
+1974.80   0.0139048   0.2404967
+1974.85   0.0140323   0.2407943
+1974.90   0.0141590   0.2410927
+1974.95   0.0142849   0.2413919
+1975.00   0.0144100   0.2416919
+1975.05   0.0145344   0.2419927
+1975.10   0.0146580   0.2422941
+1975.15   0.0147808   0.2425963
+1975.20   0.0149028   0.2428992
+1975.25   0.0150241   0.2432028
+1975.30   0.0151446   0.2435071
+1975.35   0.0152643   0.2438120
+1975.40   0.0153833   0.2441175
+1975.45   0.0155016   0.2444236
+1975.50   0.0156191   0.2447304
+1975.55   0.0157359   0.2450377
+1975.60   0.0158519   0.2453455
+1975.65   0.0159673   0.2456539
+1975.70   0.0160820   0.2459627
+1975.75   0.0161959   0.2462721
+1975.80   0.0163092   0.2465819
+1975.85   0.0164218   0.2468922
+1975.90   0.0165338   0.2472028
+1975.95   0.0166451   0.2475139
+1976.00   0.0167558   0.2478253
+1976.05   0.0168658   0.2481370
+1976.10   0.0169753   0.2484491
+1976.15   0.0170842   0.2487614
+1976.20   0.0171924   0.2490741
+1976.25   0.0173002   0.2493869
+1976.30   0.0174074   0.2497000
+1976.35   0.0175141   0.2500133
+1976.40   0.0176202   0.2503267
+1976.45   0.0177259   0.2506402
+1976.50   0.0178311   0.2509539
+1976.55   0.0179358   0.2512676
+1976.60   0.0180401   0.2515814
+1976.65   0.0181440   0.2518952
+1976.70   0.0182474   0.2522090
+1976.75   0.0183505   0.2525228
+1976.80   0.0184532   0.2528365
+1976.85   0.0185556   0.2531501
+1976.90   0.0186576   0.2534636
+1976.95   0.0187593   0.2537770
+1977.00   0.0188608   0.2540902
+1977.05   0.0189619   0.2544031
+1977.10   0.0190629   0.2547159
+1977.15   0.0191635   0.2550284
+1977.20   0.0192640   0.2553405
+1977.25   0.0193643   0.2556524
+1977.30   0.0194644   0.2559639
+1977.35   0.0195644   0.2562750
+1977.40   0.0196642   0.2565857
+1977.45   0.0197639   0.2568960
+1977.50   0.0198635   0.2572058
+1977.55   0.0199631   0.2575151
+1977.60   0.0200626   0.2578239
+1977.65   0.0201620   0.2581321
+1977.70   0.0202615   0.2584397
+1977.75   0.0203609   0.2587467
+1977.80   0.0204604   0.2590530
+1977.85   0.0205600   0.2593587
+1977.90   0.0206595   0.2596636
+1977.95   0.0207592   0.2599678
+1978.00   0.0208590   0.2602713
+1978.05   0.0209589   0.2605739
+1978.10   0.0210589   0.2608758
+1978.15   0.0211590   0.2611767
+1978.20   0.0212594   0.2614768
+1978.25   0.0213599   0.2617760
+1978.30   0.0214606   0.2620743
+1978.35   0.0215616   0.2623715
+1978.40   0.0216627   0.2626678
+1978.45   0.0217642   0.2629631
+1978.50   0.0218658   0.2632573
+1978.55   0.0219678   0.2635504
+1978.60   0.0220701   0.2638425
+1978.65   0.0221726   0.2641334
+1978.70   0.0222755   0.2644231
+1978.75   0.0223787   0.2647117
+1978.80   0.0224822   0.2649991
+1978.85   0.0225861   0.2652852
+1978.90   0.0226904   0.2655701
+1978.95   0.0227950   0.2658537
+1979.00   0.0229001   0.2661360
+1979.05   0.0230055   0.2664170
+1979.10   0.0231113   0.2666966
+1979.15   0.0232176   0.2669749
+1979.20   0.0233242   0.2672518
+1979.25   0.0234313   0.2675273
+1979.30   0.0235388   0.2678013
+1979.35   0.0236468   0.2680739
+1979.40   0.0237552   0.2683450
+1979.45   0.0238641   0.2686146
+1979.50   0.0239734   0.2688827
+1979.55   0.0240832   0.2691493
+1979.60   0.0241934   0.2694143
+1979.65   0.0243042   0.2696778
+1979.70   0.0244154   0.2699397
+1979.75   0.0245270   0.2702000
+1979.80   0.0246391   0.2704586
+1979.85   0.0247518   0.2707157
+1979.90   0.0248648   0.2709711
+1979.95   0.0249784   0.2712249
+1980.00   0.0250924   0.2714770
+1980.05   0.0252069   0.2717274
+1980.10   0.0253219   0.2719762
+1980.15   0.0254373   0.2722233
+1980.20   0.0255532   0.2724686
+1980.25   0.0256695   0.2727123
+1980.30   0.0257863   0.2729542
+1980.35   0.0259036   0.2731944
+1980.40   0.0260212   0.2734328
+1980.45   0.0261394   0.2736695
+1980.50   0.0262579   0.2739045
+1980.55   0.0263769   0.2741378
+1980.60   0.0264963   0.2743692
+1980.65   0.0266160   0.2745990
+1980.70   0.0267362   0.2748269
+1980.75   0.0268568   0.2750531
+1980.80   0.0269777   0.2752776
+1980.85   0.0270990   0.2755003
+1980.90   0.0272207   0.2757212
+1980.95   0.0273427   0.2759404
+1981.00   0.0274650   0.2761579
+1981.05   0.0275877   0.2763736
+1981.10   0.0277107   0.2765876
+1981.15   0.0278339   0.2767998
+1981.20   0.0279574   0.2770104
+1981.25   0.0280812   0.2772192
+1981.30   0.0282053   0.2774263
+1981.35   0.0283296   0.2776317
+1981.40   0.0284541   0.2778354
+1981.45   0.0285788   0.2780375
+1981.50   0.0287037   0.2782378
+1981.55   0.0288287   0.2784366
+1981.60   0.0289540   0.2786337
+1981.65   0.0290793   0.2788292
+1981.70   0.0292048   0.2790230
+1981.75   0.0293304   0.2792153
+1981.80   0.0294561   0.2794060
+1981.85   0.0295818   0.2795952
+1981.90   0.0297076   0.2797828
+1981.95   0.0298334   0.2799689
+1982.00   0.0299593   0.2801535
+1982.05   0.0300851   0.2803367
+1982.10   0.0302109   0.2805184
+1982.15   0.0303367   0.2806987
+1982.20   0.0304624   0.2808775
+1982.25   0.0305880   0.2810550
+1982.30   0.0307135   0.2812311
+1982.35   0.0308389   0.2814059
+1982.40   0.0309641   0.2815794
+1982.45   0.0310892   0.2817516
+1982.50   0.0312141   0.2819226
+1982.55   0.0313388   0.2820924
+1982.60   0.0314632   0.2822609
+1982.65   0.0315875   0.2824283
+1982.70   0.0317114   0.2825946
+1982.75   0.0318351   0.2827598
+1982.80   0.0319584   0.2829239
+1982.85   0.0320815   0.2830869
+1982.90   0.0322042   0.2832490
+1982.95   0.0323265   0.2834101
+1983.00   0.0324484   0.2835703
+1983.05   0.0325699   0.2837295
+1983.10   0.0326910   0.2838879
+1983.15   0.0328117   0.2840455
+1983.20   0.0329319   0.2842022
+1983.25   0.0330516   0.2843582
+1983.30   0.0331708   0.2845135
+1983.35   0.0332894   0.2846681
+1983.40   0.0334075   0.2848220
+1983.45   0.0335251   0.2849753
+1983.50   0.0336421   0.2851280
+1983.55   0.0337584   0.2852802
+1983.60   0.0338742   0.2854319
+1983.65   0.0339893   0.2855831
+1983.70   0.0341037   0.2857339
+1983.75   0.0342175   0.2858843
+1983.80   0.0343305   0.2860343
+1983.85   0.0344429   0.2861840
+1983.90   0.0345545   0.2863335
+1983.95   0.0346654   0.2864827
+1984.00   0.0347755   0.2866317
+1984.05   0.0348849   0.2867805
+1984.10   0.0349934   0.2869292
+1984.15   0.0351012   0.2870779
+1984.20   0.0352081   0.2872264
+1984.25   0.0353141   0.2873750
+1984.30   0.0354193   0.2875236
+1984.35   0.0355237   0.2876722
+1984.40   0.0356271   0.2878210
+1984.45   0.0357297   0.2879699
+1984.50   0.0358313   0.2881189
+1984.55   0.0359320   0.2882682
+1984.60   0.0360318   0.2884177
+1984.65   0.0361306   0.2885675
+1984.70   0.0362284   0.2887176
+1984.75   0.0363253   0.2888680
+1984.80   0.0364212   0.2890188
+1984.85   0.0365160   0.2891701
+1984.90   0.0366099   0.2893218
+1984.95   0.0367027   0.2894740
+1985.00   0.0367946   0.2896267
+1985.05   0.0368853   0.2897799
+1985.10   0.0369750   0.2899337
+1985.15   0.0370637   0.2900882
+1985.20   0.0371513   0.2902432
+1985.25   0.0372378   0.2903990
+1985.30   0.0373232   0.2905554
+1985.35   0.0374075   0.2907125
+1985.40   0.0374908   0.2908705
+1985.45   0.0375729   0.2910291
+1985.50   0.0376539   0.2911886
+1985.55   0.0377338   0.2913490
+1985.60   0.0378125   0.2915101
+1985.65   0.0378902   0.2916722
+1985.70   0.0379667   0.2918351
+1985.75   0.0380420   0.2919990
+1985.80   0.0381162   0.2921638
+1985.85   0.0381893   0.2923296
+1985.90   0.0382612   0.2924964
+1985.95   0.0383319   0.2926642
+1986.00   0.0384015   0.2928330
+1986.05   0.0384699   0.2930028
+1986.10   0.0385371   0.2931737
+1986.15   0.0386032   0.2933456
+1986.20   0.0386681   0.2935187
+1986.25   0.0387319   0.2936928
+1986.30   0.0387944   0.2938681
+1986.35   0.0388558   0.2940445
+1986.40   0.0389160   0.2942220
+1986.45   0.0389751   0.2944006
+1986.50   0.0390330   0.2945804
+1986.55   0.0390897   0.2947614
+1986.60   0.0391452   0.2949435
+1986.65   0.0391995   0.2951268
+1986.70   0.0392527   0.2953113
+1986.75   0.0393047   0.2954970
+1986.80   0.0393556   0.2956839
+1986.85   0.0394052   0.2958719
+1986.90   0.0394537   0.2960612
+1986.95   0.0395011   0.2962516
+1987.00   0.0395473   0.2964433
+1987.05   0.0395923   0.2966361
+1987.10   0.0396362   0.2968301
+1987.15   0.0396789   0.2970253
+1987.20   0.0397205   0.2972217
+1987.25   0.0397610   0.2974193
+1987.30   0.0398003   0.2976180
+1987.35   0.0398384   0.2978180
+1987.40   0.0398755   0.2980190
+1987.45   0.0399114   0.2982213
+1987.50   0.0399462   0.2984246
+1987.55   0.0399798   0.2986292
+1987.60   0.0400124   0.2988348
+1987.65   0.0400439   0.2990415
+1987.70   0.0400742   0.2992494
+1987.75   0.0401035   0.2994583
+1987.80   0.0401317   0.2996684
+1987.85   0.0401587   0.2998794
+1987.90   0.0401848   0.3000916
+1987.95   0.0402097   0.3003047
+1988.00   0.0402336   0.3005189
+1988.05   0.0402564   0.3007340
+1988.10   0.0402782   0.3009502
+1988.15   0.0402989   0.3011673
+1988.20   0.0403186   0.3013853
+1988.25   0.0403373   0.3016043
+1988.30   0.0403549   0.3018241
+1988.35   0.0403715   0.3020449
+1988.40   0.0403871   0.3022665
+1988.45   0.0404018   0.3024889
+1988.50   0.0404154   0.3027121
+1988.55   0.0404280   0.3029362
+1988.60   0.0404397   0.3031610
+1988.65   0.0404504   0.3033865
+1988.70   0.0404601   0.3036128
+1988.75   0.0404689   0.3038397
+1988.80   0.0404768   0.3040673
+1988.85   0.0404837   0.3042955
+1988.90   0.0404897   0.3045244
+1988.95   0.0404948   0.3047538
+1989.00   0.0404989   0.3049838
+1989.05   0.0405022   0.3052143
+1989.10   0.0405046   0.3054453
+1989.15   0.0405061   0.3056768
+1989.20   0.0405067   0.3059088
+1989.25   0.0405065   0.3061411
+1989.30   0.0405054   0.3063738
+1989.35   0.0405035   0.3066069
+1989.40   0.0405008   0.3068403
+1989.45   0.0404972   0.3070740
+1989.50   0.0404929   0.3073079
+1989.55   0.0404877   0.3075421
+1989.60   0.0404818   0.3077765
+1989.65   0.0404750   0.3080110
+1989.70   0.0404676   0.3082457
+1989.75   0.0404593   0.3084805
+1989.80   0.0404503   0.3087154
+1989.85   0.0404406   0.3089503
+1989.90   0.0404302   0.3091853
+1989.95   0.0404191   0.3094202
+1990.00   0.0404073   0.3096550
+1990.05   0.0403947   0.3098898
+1990.10   0.0403816   0.3101245
+1990.15   0.0403677   0.3103590
+1990.20   0.0403532   0.3105933
+1990.25   0.0403381   0.3108274
+1990.30   0.0403224   0.3110613
+1990.35   0.0403060   0.3112949
+1990.40   0.0402891   0.3115283
+1990.45   0.0402716   0.3117612
+1990.50   0.0402535   0.3119938
+1990.55   0.0402349   0.3122261
+1990.60   0.0402157   0.3124578
+1990.65   0.0401960   0.3126892
+1990.70   0.0401758   0.3129200
+1990.75   0.0401551   0.3131503
+1990.80   0.0401339   0.3133801
+1990.85   0.0401123   0.3136093
+1990.90   0.0400902   0.3138379
+1990.95   0.0400676   0.3140658
+1991.00   0.0400447   0.3142931
+1991.05   0.0400213   0.3145196
+1991.10   0.0399975   0.3147455
+1991.15   0.0399734   0.3149706
+1991.20   0.0399489   0.3151949
+1991.25   0.0399241   0.3154184
+1991.30   0.0398989   0.3156411
+1991.35   0.0398734   0.3158629
+1991.40   0.0398477   0.3160838
+1991.45   0.0398216   0.3163038
+1991.50   0.0397953   0.3165229
+1991.55   0.0397688   0.3167410
+1991.60   0.0397420   0.3169581
+1991.65   0.0397150   0.3171742
+1991.70   0.0396878   0.3173892
+1991.75   0.0396605   0.3176032
+1991.80   0.0396330   0.3178161
+1991.85   0.0396053   0.3180278
+1991.90   0.0395776   0.3182385
+1991.95   0.0395497   0.3184480
+1992.00   0.0395217   0.3186563
+1992.05   0.0394937   0.3188634
+1992.10   0.0394656   0.3190693
+1992.15   0.0394375   0.3192740
+1992.20   0.0394094   0.3194774
+1992.25   0.0393813   0.3196795
+1992.30   0.0393532   0.3198803
+1992.35   0.0393252   0.3200798
+1992.40   0.0392972   0.3202780
+1992.45   0.0392693   0.3204748
+1992.50   0.0392415   0.3206703
+1992.55   0.0392138   0.3208644
+1992.60   0.0391862   0.3210571
+1992.65   0.0391588   0.3212484
+1992.70   0.0391316   0.3214383
+1992.75   0.0391046   0.3216267
+1992.80   0.0390778   0.3218137
+1992.85   0.0390512   0.3219992
+1992.90   0.0390249   0.3221832
+1992.95   0.0389988   0.3223658
+1993.00   0.0389730   0.3225469
+1993.05   0.0389476   0.3227264
+1993.10   0.0389224   0.3229045
+1993.15   0.0388976   0.3230810
+1993.20   0.0388732   0.3232560
+1993.25   0.0388491   0.3234294
+1993.30   0.0388255   0.3236013
+1993.35   0.0388022   0.3237717
+1993.40   0.0387794   0.3239405
+1993.45   0.0387571   0.3241077
+1993.50   0.0387352   0.3242734
+1993.55   0.0387138   0.3244375
+1993.60   0.0386929   0.3246000
+1993.65   0.0386726   0.3247609
+1993.70   0.0386528   0.3249203
+1993.75   0.0386335   0.3250781
+1993.80   0.0386149   0.3252343
+1993.85   0.0385968   0.3253889
+1993.90   0.0385793   0.3255419
+1993.95   0.0385625   0.3256934
+1994.00   0.0385463   0.3258433
+1994.05   0.0385308   0.3259916
+1994.10   0.0385159   0.3261383
+1994.15   0.0385017   0.3262835
+1994.20   0.0384883   0.3264271
+1994.25   0.0384756   0.3265691
+1994.30   0.0384636   0.3267096
+1994.35   0.0384523   0.3268485
+1994.40   0.0384419   0.3269859
+1994.45   0.0384322   0.3271218
+1994.50   0.0384233   0.3272561
+1994.55   0.0384152   0.3273889
+1994.60   0.0384080   0.3275202
+1994.65   0.0384016   0.3276500
+1994.70   0.0383960   0.3277783
+1994.75   0.0383913   0.3279051
+1994.80   0.0383875   0.3280305
+1994.85   0.0383846   0.3281543
+1994.90   0.0383826   0.3282768
+1994.95   0.0383814   0.3283978
+1995.00   0.0383812   0.3285173
+1995.05   0.0383820   0.3286355
+1995.10   0.0383837   0.3287523
+1995.15   0.0383863   0.3288677
+1995.20   0.0383899   0.3289817
+1995.25   0.0383945   0.3290943
+1995.30   0.0384001   0.3292057
+1995.35   0.0384067   0.3293157
+1995.40   0.0384142   0.3294244
+1995.45   0.0384228   0.3295318
+1995.50   0.0384324   0.3296380
+1995.55   0.0384430   0.3297429
+1995.60   0.0384547   0.3298466
+1995.65   0.0384674   0.3299490
+1995.70   0.0384811   0.3300503
+1995.75   0.0384959   0.3301504
+1995.80   0.0385117   0.3302493
+1995.85   0.0385287   0.3303471
+1995.90   0.0385466   0.3304438
+1995.95   0.0385657   0.3305394
+1996.00   0.0385858   0.3306339
+1996.05   0.0386070   0.3307273
+1996.10   0.0386293   0.3308198
+1996.15   0.0386527   0.3309112
+1996.20   0.0386772   0.3310016
+1996.25   0.0387028   0.3310911
+1996.30   0.0387295   0.3311796
+1996.35   0.0387572   0.3312672
+1996.40   0.0387861   0.3313539
+1996.45   0.0388161   0.3314398
+1996.50   0.0388472   0.3315247
+1996.55   0.0388793   0.3316089
+1996.60   0.0389126   0.3316923
+1996.65   0.0389470   0.3317748
+1996.70   0.0389825   0.3318566
+1996.75   0.0390191   0.3319377
+1996.80   0.0390568   0.3320181
+1996.85   0.0390956   0.3320978
+1996.90   0.0391354   0.3321768
+1996.95   0.0391764   0.3322552
+1997.00   0.0392185   0.3323330
+1997.05   0.0392617   0.3324102
+1997.10   0.0393059   0.3324868
+1997.15   0.0393513   0.3325629
+1997.20   0.0393977   0.3326384
+1997.25   0.0394452   0.3327135
+1997.30   0.0394937   0.3327881
+1997.35   0.0395434   0.3328622
+1997.40   0.0395941   0.3329360
+1997.45   0.0396458   0.3330093
+1997.50   0.0396986   0.3330823
+1997.55   0.0397525   0.3331549
+1997.60   0.0398074   0.3332272
+1997.65   0.0398633   0.3332992
+1997.70   0.0399203   0.3333709
+1997.75   0.0399783   0.3334423
+1997.80   0.0400373   0.3335135
+1997.85   0.0400973   0.3335845
+1997.90   0.0401583   0.3336553
+1997.95   0.0402204   0.3337259
+1998.00   0.0402834   0.3337964
+1998.05   0.0403474   0.3338667
+1998.10   0.0404123   0.3339370
+1998.15   0.0404783   0.3340071
+1998.20   0.0405452   0.3340772
+1998.25   0.0406130   0.3341472
+1998.30   0.0406818   0.3342173
+1998.35   0.0407516   0.3342873
+1998.40   0.0408222   0.3343573
+1998.45   0.0408938   0.3344273
+1998.50   0.0409663   0.3344974
+1998.55   0.0410397   0.3345676
+1998.60   0.0411140   0.3346378
+1998.65   0.0411892   0.3347082
+1998.70   0.0412653   0.3347787
+1998.75   0.0413422   0.3348493
+1998.80   0.0414200   0.3349200
+1998.85   0.0414986   0.3349909
+1998.90   0.0415781   0.3350620
+1998.95   0.0416584   0.3351333
+1999.00   0.0417395   0.3352048
+1999.05   0.0418215   0.3352765
+1999.10   0.0419043   0.3353484
+1999.15   0.0419878   0.3354206
+1999.20   0.0420722   0.3354931
+1999.25   0.0421573   0.3355658
+1999.30   0.0422433   0.3356388
+1999.35   0.0423299   0.3357121
+1999.40   0.0424174   0.3357857
+1999.45   0.0425056   0.3358596
+1999.50   0.0425945   0.3359338
+1999.55   0.0426842   0.3360083
+1999.60   0.0427746   0.3360832
+1999.65   0.0428657   0.3361584
+1999.70   0.0429576   0.3362339
+1999.75   0.0430501   0.3363098
+1999.80   0.0431434   0.3363861
+1999.85   0.0432373   0.3364627
+1999.90   0.0433319   0.3365396
+1999.95   0.0434272   0.3366170
+2000.00   0.0435232   0.3366947
+2000.05   0.0436199   0.3367728
+2000.10   0.0437172   0.3368512
+2000.15   0.0438151   0.3369300
+2000.20   0.0439138   0.3370092
+2000.25   0.0440130   0.3370888
+2000.30   0.0441129   0.3371687
+2000.35   0.0442135   0.3372490
+2000.40   0.0443147   0.3373297
+2000.45   0.0444165   0.3374107
+2000.50   0.0445190   0.3374921
+2000.55   0.0446220   0.3375739
+2000.60   0.0447257   0.3376560
+2000.65   0.0448301   0.3377384
+2000.70   0.0449350   0.3378212
+2000.75   0.0450406   0.3379043
+2000.80   0.0451468   0.3379878
+2000.85   0.0452535   0.3380715
+2000.90   0.0453609   0.3381556
+2000.95   0.0454690   0.3382400
+2001.00   0.0455776   0.3383247
+2001.05   0.0456869   0.3384096
+2001.10   0.0457967   0.3384948
+2001.15   0.0459072   0.3385803
+2001.20   0.0460183   0.3386661
+2001.25   0.0461300   0.3387520
+2001.30   0.0462424   0.3388382
+2001.35   0.0463554   0.3389246
+2001.40   0.0464690   0.3390112
+2001.45   0.0465832   0.3390980
+2001.50   0.0466981   0.3391849
+2001.55   0.0468136   0.3392721
+2001.60   0.0469297   0.3393593
+2001.65   0.0470465   0.3394466
+2001.70   0.0471640   0.3395341
+2001.75   0.0472821   0.3396217
+2001.80   0.0474009   0.3397093
+2001.85   0.0475204   0.3397970
+2001.90   0.0476405   0.3398847
+2001.95   0.0477613   0.3399724
+2002.00   0.0478828   0.3400601
+2002.05   0.0480051   0.3401478
+2002.10   0.0481280   0.3402354
+2002.15   0.0482516   0.3403230
+2002.20   0.0483760   0.3404105
+2002.25   0.0485011   0.3404979
+2002.30   0.0486270   0.3405852
+2002.35   0.0487536   0.3406724
+2002.40   0.0488810   0.3407593
+2002.45   0.0490091   0.3408461
+2002.50   0.0491381   0.3409327
+2002.55   0.0492678   0.3410190
+2002.60   0.0493983   0.3411051
+2002.65   0.0495297   0.3411909
+2002.70   0.0496619   0.3412764
+2002.75   0.0497949   0.3413616
+2002.80   0.0499288   0.3414465
+2002.85   0.0500635   0.3415310
+2002.90   0.0501991   0.3416151
+2002.95   0.0503357   0.3416988
+2003.00   0.0504731   0.3417820
+2003.05   0.0506114   0.3418648
+2003.10   0.0507506   0.3419471
+2003.15   0.0508908   0.3420290
+2003.20   0.0510320   0.3421103
+2003.25   0.0511741   0.3421910
+2003.30   0.0513172   0.3422712
+2003.35   0.0514613   0.3423508
+2003.40   0.0516063   0.3424298
+2003.45   0.0517524   0.3425081
+2003.50   0.0518996   0.3425858
+2003.55   0.0520477   0.3426628
+2003.60   0.0521970   0.3427391
+2003.65   0.0523473   0.3428147
+2003.70   0.0524986   0.3428895
+2003.75   0.0526511   0.3429636
+2003.80   0.0528047   0.3430369
+2003.85   0.0529594   0.3431094
+2003.90   0.0531152   0.3431811
+2003.95   0.0532722   0.3432519
+2004.00   0.0534303   0.3433219
+2004.05   0.0535896   0.3433910
+2004.10   0.0537501   0.3434592
+2004.15   0.0539117   0.3435265
+2004.20   0.0540746   0.3435928
+2004.25   0.0542387   0.3436582
+2004.30   0.0544040   0.3437227
+2004.35   0.0545705   0.3437861
+2004.40   0.0547383   0.3438486
+2004.45   0.0549073   0.3439100
+2004.50   0.0550776   0.3439705
+2004.55   0.0552491   0.3440298
+2004.60   0.0554220   0.3440882
+2004.65   0.0555961   0.3441455
+2004.70   0.0557715   0.3442017
+2004.75   0.0559482   0.3442568
+2004.80   0.0561262   0.3443108
+2004.85   0.0563056   0.3443637
+2004.90   0.0564862   0.3444155
+2004.95   0.0566682   0.3444662
+2005.00   0.0568515   0.3445157
+2005.05   0.0570361   0.3445641
+2005.10   0.0572221   0.3446114
+2005.15   0.0574094   0.3446575
+2005.20   0.0575981   0.3447024
+2005.25   0.0577881   0.3447462
+2005.30   0.0579795   0.3447888
+2005.35   0.0581722   0.3448303
+2005.40   0.0583662   0.3448706
+2005.45   0.0585616   0.3449097
+2005.50   0.0587584   0.3449477
+2005.55   0.0589565   0.3449845
+2005.60   0.0591559   0.3450201
+2005.65   0.0593567   0.3450545
+2005.70   0.0595588   0.3450878
+2005.75   0.0597622   0.3451200
+2005.80   0.0599670   0.3451510
+2005.85   0.0601731   0.3451808
+2005.90   0.0603806   0.3452095
+2005.95   0.0605893   0.3452370
+2006.00   0.0607994   0.3452635
+2006.05   0.0610107   0.3452888
+2006.10   0.0612234   0.3453130
+2006.15   0.0614373   0.3453361
+2006.20   0.0616525   0.3453581
+2006.25   0.0618690   0.3453790
+2006.30   0.0620867   0.3453989
+2006.35   0.0623057   0.3454177
+2006.40   0.0625258   0.3454355
+2006.45   0.0627473   0.3454522
+2006.50   0.0629699   0.3454680
+2006.55   0.0631937   0.3454827
+2006.60   0.0634187   0.3454965
+2006.65   0.0636448   0.3455094
+2006.70   0.0638721   0.3455213
+2006.75   0.0641005   0.3455323
+2006.80   0.0643300   0.3455424
+2006.85   0.0645607   0.3455516
+2006.90   0.0647924   0.3455599
+2006.95   0.0650251   0.3455675
+2007.00   0.0652590   0.3455742
+2007.05   0.0654938   0.3455801
+2007.10   0.0657296   0.3455853
+2007.15   0.0659665   0.3455898
+2007.20   0.0662043   0.3455935
+2007.25   0.0664430   0.3455966
+2007.30   0.0666827   0.3455990
+2007.35   0.0669232   0.3456007
+2007.40   0.0671647   0.3456019
+2007.45   0.0674070   0.3456025
+2007.50   0.0676501   0.3456025
+2007.55   0.0678940   0.3456021
+2007.60   0.0681388   0.3456011
+2007.65   0.0683843   0.3455997
+2007.70   0.0686305   0.3455979
+2007.75   0.0688775   0.3455956
+2007.80   0.0691251   0.3455930
+2007.85   0.0693734   0.3455901
+2007.90   0.0696224   0.3455869
+2007.95   0.0698719   0.3455834
+2008.00   0.0701221   0.3455796
+2008.05   0.0703728   0.3455757
+2008.10   0.0706241   0.3455716
+2008.15   0.0708759   0.3455673
+2008.20   0.0711282   0.3455630
+2008.25   0.0713809   0.3455586
+2008.30   0.0716341   0.3455541
+2008.35   0.0718877   0.3455496
+2008.40   0.0721417   0.3455452
+2008.45   0.0723960   0.3455408
+2008.50   0.0726507   0.3455365
+2008.55   0.0729057   0.3455324
+2008.60   0.0731610   0.3455284
+2008.65   0.0734165   0.3455246
+2008.70   0.0736723   0.3455211
+2008.75   0.0739283   0.3455178
+2008.80   0.0741845   0.3455148
+2008.85   0.0744409   0.3455121
+2008.90   0.0746973   0.3455098
+2008.95   0.0749539   0.3455079
+2009.00   0.0752106   0.3455064
+2009.05   0.0754674   0.3455054
+2009.10   0.0757242   0.3455049
+2009.15   0.0759810   0.3455049
+2009.20   0.0762378   0.3455054
+2009.25   0.0764946   0.3455065
+2009.30   0.0767513   0.3455083
+2009.35   0.0770080   0.3455106
+2009.40   0.0772646   0.3455137
+2009.45   0.0775210   0.3455174
+2009.50   0.0777774   0.3455219
+2009.55   0.0780336   0.3455271
+2009.60   0.0782896   0.3455331
+2009.65   0.0785454   0.3455400
+2009.70   0.0788010   0.3455476
+2009.75   0.0790564   0.3455561
+2009.80   0.0793115   0.3455655
+2009.85   0.0795664   0.3455758
+2009.90   0.0798210   0.3455870
+2009.95   0.0800753   0.3455992
+2010.00   0.0803293   0.3456124
+2010.05   0.0805830   0.3456265
+2010.10   0.0808363   0.3456417
+2010.15   0.0810892   0.3456579
+2010.20   0.0813418   0.3456751
+2010.25   0.0815941   0.3456934
+2010.30   0.0818459   0.3457128
+2010.35   0.0820973   0.3457333
+2010.40   0.0823483   0.3457549
+2010.45   0.0825988   0.3457776
+2010.50   0.0828490   0.3458015
+2010.55   0.0830986   0.3458265
+2010.60   0.0833478   0.3458527
+2010.65   0.0835966   0.3458801
+2010.70   0.0838449   0.3459087
+2010.75   0.0840926   0.3459384
+2010.80   0.0843400   0.3459694
+2010.85   0.0845868   0.3460015
+2010.90   0.0848331   0.3460349
+2010.95   0.0850789   0.3460694
+2011.00   0.0853242   0.3461052
+2011.05   0.0855689   0.3461423
+2011.10   0.0858132   0.3461805
+2011.15   0.0860569   0.3462199
+2011.20   0.0863001   0.3462606
+2011.25   0.0865428   0.3463025
+2011.30   0.0867850   0.3463456
+2011.35   0.0870266   0.3463900
+2011.40   0.0872677   0.3464355
+2011.45   0.0875083   0.3464822
+2011.50   0.0877483   0.3465302
+2011.55   0.0879879   0.3465793
+2011.60   0.0882269   0.3466296
+2011.65   0.0884653   0.3466811
+2011.70   0.0887033   0.3467337
+2011.75   0.0889407   0.3467875
+2011.80   0.0891776   0.3468424
+2011.85   0.0894141   0.3468985
+2011.90   0.0896500   0.3469556
+2011.95   0.0898854   0.3470139
+2012.00   0.0901203   0.3470732
+2012.05   0.0903547   0.3471335
+2012.10   0.0905886   0.3471950
+2012.15   0.0908221   0.3472574
+2012.20   0.0910551   0.3473209
+2012.25   0.0912876   0.3473853
+2012.30   0.0915197   0.3474507
+2012.35   0.0917513   0.3475170
+2012.40   0.0919824   0.3475843
+2012.45   0.0922131   0.3476524
+2012.50   0.0924434   0.3477214
+2012.55   0.0926733   0.3477913
+2012.60   0.0929027   0.3478620
+2012.65   0.0931318   0.3479334
+2012.70   0.0933604   0.3480057
+2012.75   0.0935887   0.3480786
+2012.80   0.0938166   0.3481523
+2012.85   0.0940441   0.3482267
+2012.90   0.0942712   0.3483017
+2012.95   0.0944980   0.3483774
+2013.00   0.0947245   0.3484536
+2013.05   0.0949506   0.3485305
+2013.10   0.0951764   0.3486078
+2013.15   0.0954019   0.3486857
+2013.20   0.0956270   0.3487640
+2013.25   0.0958519   0.3488427
+2013.30   0.0960765   0.3489219
+2013.35   0.0963008   0.3490015
+2013.40   0.0965249   0.3490813
+2013.45   0.0967487   0.3491615
+2013.50   0.0969722   0.3492420
+2013.55   0.0971955   0.3493227
+2013.60   0.0974185   0.3494036
+2013.65   0.0976414   0.3494847
+2013.70   0.0978640   0.3495659
+2013.75   0.0980864   0.3496473
+2013.80   0.0983086   0.3497287
+2013.85   0.0985307   0.3498101
+2013.90   0.0987525   0.3498916
+2013.95   0.0989742   0.3499730
+2014.00   0.0991957   0.3500543
+2014.05   0.0994171   0.3501356
+2014.10   0.0996383   0.3502167
+2014.15   0.0998593   0.3502977
+2014.20   0.1000802   0.3503784
+2014.25   0.1003010   0.3504589
+2014.30   0.1005217   0.3505392
+2014.35   0.1007422   0.3506192
+2014.40   0.1009627   0.3506988
+2014.45   0.1011830   0.3507781
+2014.50   0.1014032   0.3508569
+2014.55   0.1016234   0.3509354
+2014.60   0.1018434   0.3510134
+2014.65   0.1020634   0.3510909
+2014.70   0.1022832   0.3511679
+2014.75   0.1025030   0.3512443
+2014.80   0.1027227   0.3513201
+2014.85   0.1029424   0.3513954
+2014.90   0.1031619   0.3514700
+2014.95   0.1033814   0.3515439
+2015.00   0.1036008   0.3516172
+2015.05   0.1038202   0.3516897
+2015.10   0.1040395   0.3517615
+2015.15   0.1042588   0.3518325
+2015.20   0.1044779   0.3519027
+2015.25   0.1046971   0.3519720
+2015.30   0.1049161   0.3520406
+2015.35   0.1051351   0.3521082
+2015.40   0.1053540   0.3521750
+2015.45   0.1055729   0.3522408
+2015.50   0.1057917   0.3523057
+2015.55   0.1060104   0.3523696
+2015.60   0.1062291   0.3524325
+2015.65   0.1064477   0.3524945
+2015.70   0.1066662   0.3525554
+2015.75   0.1068847   0.3526152
+2015.80   0.1071031   0.3526740
+2015.85   0.1073213   0.3527318
+2015.90   0.1075395   0.3527884
+2015.95   0.1077576   0.3528439
+2016.00   0.1079756   0.3528983
+2016.05   0.1081935   0.3529515
+2016.10   0.1084113   0.3530036
+2016.15   0.1086290   0.3530545
+2016.20   0.1088466   0.3531042
+2016.25   0.1090640   0.3531527
+2016.30   0.1092813   0.3532000
+2016.35   0.1094985   0.3532461
+2016.40   0.1097155   0.3532910
+2016.45   0.1099324   0.3533346
+2016.50   0.1101491   0.3533770
+2016.55   0.1103656   0.3534181
+2016.60   0.1105820   0.3534579
+2016.65   0.1107982   0.3534965
+2016.70   0.1110142   0.3535338
+2016.75   0.1112299   0.3535698
+2016.80   0.1114455   0.3536045
+2016.85   0.1116609   0.3536379
+2016.90   0.1118760   0.3536700
+2016.95   0.1120908   0.3537008
+2017.00   0.1123055   0.3537303
+2017.05   0.1125198   0.3537585
+2017.10   0.1127340   0.3537854
+2017.15   0.1129478   0.3538110
+2017.20   0.1131613   0.3538353
+2017.25   0.1133745   0.3538582
+2017.30   0.1135875   0.3538798
+2017.35   0.1138000   0.3539002
+2017.40   0.1140123   0.3539192
+2017.45   0.1142242   0.3539369
+2017.50   0.1144358   0.3539533
+2017.55   0.1146470   0.3539684
+2017.60   0.1148578   0.3539822
+2017.65   0.1150682   0.3539947
+2017.70   0.1152783   0.3540059
+2017.75   0.1154879   0.3540158
+2017.80   0.1156971   0.3540244
+2017.85   0.1159058   0.3540317
+2017.90   0.1161141   0.3540378
+2017.95   0.1163220   0.3540426
+2018.00   0.1165294   0.3540462
+2018.05   0.1167363   0.3540484
+2018.10   0.1169427   0.3540495
+2018.15   0.1171486   0.3540493
+2018.20   0.1173540   0.3540478
+2018.25   0.1175588   0.3540451
+2018.30   0.1177632   0.3540412
+2018.35   0.1179669   0.3540361
+2018.40   0.1181701   0.3540298
+2018.45   0.1183728   0.3540223
+2018.50   0.1185748   0.3540136
+2018.55   0.1187763   0.3540037
+2018.60   0.1189771   0.3539927
+2018.65   0.1191773   0.3539805
+2018.70   0.1193769   0.3539671
+2018.75   0.1195759   0.3539526
+2018.80   0.1197742   0.3539370
+2018.85   0.1199719   0.3539202
+2018.90   0.1201688   0.3539024
+2018.95   0.1203651   0.3538834
+2019.00   0.1205607   0.3538633
+2019.05   0.1207556   0.3538422
+2019.10   0.1209498   0.3538200
+2019.15   0.1211433   0.3537967
+2019.20   0.1213360   0.3537724
+2019.25   0.1215280   0.3537470
+2019.30   0.1217193   0.3537206
+2019.35   0.1219098   0.3536932
+2019.40   0.1220995   0.3536648
+2019.45   0.1222884   0.3536353
+2019.50   0.1224766   0.3536049
+2019.55   0.1226639   0.3535735
+2019.60   0.1228505   0.3535411
+2019.65   0.1230362   0.3535078
+2019.70   0.1232212   0.3534736
+2019.75   0.1234053   0.3534383
+2019.80   0.1235885   0.3534022
+2019.85   0.1237710   0.3533652
+2019.90   0.1239526   0.3533272
+2019.95   0.1241333   0.3532884
+2020.00   0.1243131   0.3532486
+2020.05   0.1244921   0.3532080
+2020.10   0.1246703   0.3531665
+2020.15   0.1248475   0.3531242
+2020.20   0.1250238   0.3530810
+2020.25   0.1251993   0.3530370
+2020.30   0.1253738   0.3529922
+2020.35   0.1255475   0.3529465
+2020.40   0.1257202   0.3529001
+2020.45   0.1258921   0.3528528
+2020.50   0.1260630   0.3528048
+2020.55   0.1262329   0.3527560
+2020.60   0.1264020   0.3527064
+2020.65   0.1265701   0.3526561
+2020.70   0.1267373   0.3526050
+2020.75   0.1269035   0.3525531
+2020.80   0.1270688   0.3525006
+2020.85   0.1272332   0.3524473
+2020.90   0.1273966   0.3523933
+2020.95   0.1275590   0.3523386
+2021.00   0.1277205   0.3522832
+2021.05   0.1278810   0.3522272
+2021.10   0.1280406   0.3521704
+2021.15   0.1281992   0.3521130
+2021.20   0.1283568   0.3520549
+2021.25   0.1285135   0.3519962
+2021.30   0.1286692   0.3519368
+2021.35   0.1288239   0.3518768
+2021.40   0.1289776   0.3518161
+2021.45   0.1291304   0.3517549
+2021.50   0.1292822   0.3516930
+2021.55   0.1294330   0.3516305
+2021.60   0.1295828   0.3515674
+2021.65   0.1297317   0.3515038
+2021.70   0.1298796   0.3514395
+2021.75   0.1300265   0.3513747
+2021.80   0.1301724   0.3513093
+2021.85   0.1303173   0.3512434
+2021.90   0.1304613   0.3511769
+2021.95   0.1306042   0.3511098
+2022.00   0.1307462   0.3510422
+2022.05   0.1308873   0.3509741
+2022.10   0.1310273   0.3509054
+2022.15   0.1311664   0.3508363
+2022.20   0.1313045   0.3507666
+2022.25   0.1314416   0.3506964
+2022.30   0.1315777   0.3506257
+2022.35   0.1317129   0.3505546
+2022.40   0.1318471   0.3504829
+2022.45   0.1319803   0.3504108
+2022.50   0.1321126   0.3503382
+2022.55   0.1322439   0.3502651
+2022.60   0.1323742   0.3501916
+2022.65   0.1325036   0.3501176
+2022.70   0.1326320   0.3500431
+2022.75   0.1327594   0.3499682
+2022.80   0.1328859   0.3498929
+2022.85   0.1330115   0.3498172
+2022.90   0.1331361   0.3497410
+2022.95   0.1332597   0.3496644
+2023.00   0.1333824   0.3495874
+2023.05   0.1335042   0.3495100
+2023.10   0.1336250   0.3494321
+2023.15   0.1337449   0.3493539
+2023.20   0.1338639   0.3492753
+2023.25   0.1339819   0.3491963
+2023.30   0.1340990   0.3491169
+2023.35   0.1342152   0.3490372
+2023.40   0.1343304   0.3489570
+2023.45   0.1344448   0.3488765
+2023.50   0.1345582   0.3487957
+2023.55   0.1346707   0.3487145
+2023.60   0.1347824   0.3486329
+2023.65   0.1348931   0.3485510
+2023.70   0.1350029   0.3484687
+2023.75   0.1351118   0.3483861
+2023.80   0.1352199   0.3483032
+2023.85   0.1353270   0.3482200
+2023.90   0.1354333   0.3481364
+2023.95   0.1355387   0.3480525
+2024.00   0.1356432   0.3479683
+2024.05   0.1357468   0.3478838
+2024.10   0.1358496   0.3477990
+2024.15   0.1359515   0.3477139
+2024.20   0.1360526   0.3476284
```

### Comparing `pyTMD-2.1.0/pyTMD/data/merged_deltat.data` & `pyTMD-2.1.1/pyTMD/data/merged_deltat.data`

 * *Files 2% similar despite different names*

```diff
@@ -7952,7 +7952,84 @@
  2024  1  5 69.1767
  2024  1  6 69.1770
  2024  1  7 69.1772
  2024  1  8 69.1772
  2024  1  9 69.1769
  2024  1 10 69.1766
  2024  1 11 69.1762
+ 2024  1 12 69.1758
+ 2024  1 13 69.1757
+ 2024  1 14 69.1758
+ 2024  1 15 69.1762
+ 2024  1 16 69.1768
+ 2024  1 17 69.1774
+ 2024  1 18 69.1779
+ 2024  1 19 69.1783
+ 2024  1 20 69.1784
+ 2024  1 21 69.1784
+ 2024  1 22 69.1781
+ 2024  1 23 69.1778
+ 2024  1 24 69.1775
+ 2024  1 25 69.1773
+ 2024  1 26 69.1771
+ 2024  1 27 69.1772
+ 2024  1 28 69.1775
+ 2024  1 29 69.1779
+ 2024  1 30 69.1785
+ 2024  1 31 69.1791
+ 2024  2  1 69.1797
+ 2024  2  2 69.1803
+ 2024  2  3 69.1806
+ 2024  2  4 69.1808
+ 2024  2  5 69.1808
+ 2024  2  6 69.1807
+ 2024  2  7 69.1805
+ 2024  2  8 69.1804
+ 2024  2  9 69.1805
+ 2024  2 10 69.1808
+ 2024  2 11 69.1816
+ 2024  2 12 69.1826
+ 2024  2 13 69.1838
+ 2024  2 14 69.1848
+ 2024  2 15 69.1858
+ 2024  2 16 69.1864
+ 2024  2 17 69.1868
+ 2024  2 18 69.1869
+ 2024  2 19 69.1868
+ 2024  2 20 69.1865
+ 2024  2 21 69.1862
+ 2024  2 22 69.1860
+ 2024  2 23 69.1858
+ 2024  2 24 69.1857
+ 2024  2 25 69.1859
+ 2024  2 26 69.1861
+ 2024  2 27 69.1865
+ 2024  2 28 69.1868
+ 2024  2 29 69.1871
+ 2024  3  1 69.1874
+ 2024  3  2 69.1875
+ 2024  3  3 69.1875
+ 2024  3  4 69.1873
+ 2024  3  5 69.1870
+ 2024  3  6 69.1866
+ 2024  3  7 69.1865
+ 2024  3  8 69.1867
+ 2024  3  9 69.1872
+ 2024  3 10 69.1882
+ 2024  3 11 69.1894
+ 2024  3 12 69.1906
+ 2024  3 13 69.1917
+ 2024  3 14 69.1925
+ 2024  3 15 69.1931
+ 2024  3 16 69.1933
+ 2024  3 17 69.1933
+ 2024  3 18 69.1931
+ 2024  3 19 69.1931
+ 2024  3 20 69.1932
+ 2024  3 21 69.1934
+ 2024  3 22 69.1938
+ 2024  3 23 69.1943
+ 2024  3 24 69.1949
+ 2024  3 25 69.1956
+ 2024  3 26 69.1965
+ 2024  3 27 69.1972
+ 2024  3 28 69.1978
```

### Comparing `pyTMD-2.1.0/pyTMD/data/opoleloadcoefcmcor.txt.gz` & `pyTMD-2.1.1/pyTMD/data/opoleloadcoefcmcor.txt.gz`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/ser7.dat` & `pyTMD-2.1.1/pyTMD/data/ser7.dat`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      11 January 2024                                    Vol. XXXVII No. 002   
+      28 March 2024                                      Vol. XXXVII No. 013   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
@@ -49,413 +49,417 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   24  1  5  60314 0.13001 .00009 0.20517 .00009  0.007274 0.000014          
-   24  1  6  60315 0.12796 .00009 0.20607 .00009  0.006962 0.000016          
-   24  1  7  60316 0.12562 .00009 0.20641 .00009  0.006779 0.000020          
-   24  1  8  60317 0.12332 .00009 0.20663 .00009  0.006785 0.000014          
-   24  1  9  60318 0.12121 .00009 0.20656 .00009  0.007051 0.000014          
-   24  1 10  60319 0.11931 .00009 0.20632 .00009  0.007434 0.000013          
-   24  1 11  60320 0.11761 .00009 0.20651 .00009  0.007821 0.000012          
+   24  3 22  60391 -.01203 .00009 0.31646 .00009 -0.009756 0.000011          
+   24  3 23  60392 -.01131 .00009 0.31872 .00009 -0.010272 0.000012          
+   24  3 24  60393 -.01083 .00009 0.32172 .00009 -0.010914 0.000011          
+   24  3 25  60394 -.01072 .00009 0.32475 .00009 -0.011641 0.000008          
+   24  3 26  60395 -.01100 .00009 0.32746 .00009 -0.012477 0.000007          
+   24  3 27  60396 -.01149 .00009 0.33013 .00009 -0.013212 0.000004          
+   24  3 28  60397 -.01219 .00009 0.33295 .00009 -0.013764 0.000005          
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1458 - 0.0599 cos A - 0.0793 sin A + 0.0304 cos C - 0.0737 sin C  
-      y =  0.3539 - 0.0721 cos A + 0.0499 sin A - 0.0737 cos C - 0.0304 sin C  
-         UT1-UTC =  0.0067 + 0.00005 (MJD - 60328) - (UT2-UT1)                 
+      x =  0.1411 - 0.0983 cos A + 0.0325 sin A - 0.0503 cos C - 0.0517 sin C  
+      y =  0.3562 + 0.0277 cos A + 0.0872 sin A - 0.0517 cos C + 0.0503 sin C  
+         UT1-UTC =  0.0088 + 0.00007 (MJD - 60405) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60320)/365.25 and C = 2*pi*(MJD-60320)/435.          
+      where A = 2*pi*(MJD-60397)/365.25 and C = 2*pi*(MJD-60397)/435.          
                                                                                
-         TAI-UTC(MJD 60321) = 37.0                                             
+         TAI-UTC(MJD 60398) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60320)**0.80   S t = 0.00025 (MJD-60320)**0.75      
+      S x,y = 0.00068 (MJD-60397)**0.80   S t = 0.00025 (MJD-60397)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2024  1 12  60321       0.1157      0.2068      0.00818         
-       2024  1 13  60322       0.1137      0.2076      0.00836         
-       2024  1 14  60323       0.1117      0.2084      0.00827         
-       2024  1 15  60324       0.1095      0.2093      0.00791         
-       2024  1 16  60325       0.1073      0.2102      0.00738         
-       2024  1 17  60326       0.1050      0.2111      0.00681         
-       2024  1 18  60327       0.1028      0.2119      0.00633         
-       2024  1 19  60328       0.1005      0.2128      0.00606         
-       2024  1 20  60329       0.0983      0.2138      0.00607         
-       2024  1 21  60330       0.0962      0.2147      0.00635         
-       2024  1 22  60331       0.0940      0.2157      0.00683         
-       2024  1 23  60332       0.0919      0.2168      0.00740         
-       2024  1 24  60333       0.0898      0.2178      0.00796         
-       2024  1 25  60334       0.0877      0.2189      0.00843         
-       2024  1 26  60335       0.0857      0.2201      0.00875         
-       2024  1 27  60336       0.0836      0.2213      0.00888         
-       2024  1 28  60337       0.0816      0.2225      0.00882         
-       2024  1 29  60338       0.0797      0.2237      0.00857         
-       2024  1 30  60339       0.0777      0.2250      0.00817         
-       2024  1 31  60340       0.0758      0.2263      0.00767         
-       2024  2  1  60341       0.0739      0.2277      0.00713         
-       2024  2  2  60342       0.0720      0.2290      0.00665         
-       2024  2  3  60343       0.0701      0.2304      0.00628         
-       2024  2  4  60344       0.0683      0.2318      0.00608         
-       2024  2  5  60345       0.0665      0.2333      0.00607         
-       2024  2  6  60346       0.0647      0.2348      0.00622         
-       2024  2  7  60347       0.0630      0.2363      0.00645         
-       2024  2  8  60348       0.0613      0.2378      0.00663         
-       2024  2  9  60349       0.0596      0.2393      0.00662         
-       2024  2 10  60350       0.0579      0.2409      0.00630         
-       2024  2 11  60351       0.0563      0.2425      0.00566         
-       2024  2 12  60352       0.0547      0.2442      0.00476         
-       2024  2 13  60353       0.0532      0.2458      0.00376         
-       2024  2 14  60354       0.0516      0.2475      0.00284         
-       2024  2 15  60355       0.0501      0.2492      0.00215         
-       2024  2 16  60356       0.0487      0.2509      0.00178         
-       2024  2 17  60357       0.0472      0.2527      0.00172         
-       2024  2 18  60358       0.0458      0.2544      0.00192         
-       2024  2 19  60359       0.0445      0.2562      0.00228         
-       2024  2 20  60360       0.0431      0.2580      0.00269         
-       2024  2 21  60361       0.0418      0.2598      0.00306         
-       2024  2 22  60362       0.0406      0.2617      0.00332         
-       2024  2 23  60363       0.0393      0.2636      0.00342         
-       2024  2 24  60364       0.0381      0.2654      0.00334         
-       2024  2 25  60365       0.0370      0.2673      0.00309         
-       2024  2 26  60366       0.0359      0.2693      0.00270         
-       2024  2 27  60367       0.0348      0.2712      0.00223         
-       2024  2 28  60368       0.0337      0.2732      0.00175         
-       2024  2 29  60369       0.0327      0.2751      0.00133         
-       2024  3  1  60370       0.0317      0.2771      0.00103         
-       2024  3  2  60371       0.0308      0.2791      0.00089         
-       2024  3  3  60372       0.0298      0.2811      0.00091         
-       2024  3  4  60373       0.0290      0.2831      0.00110         
-       2024  3  5  60374       0.0281      0.2852      0.00137         
-       2024  3  6  60375       0.0273      0.2872      0.00163         
-       2024  3  7  60376       0.0266      0.2893      0.00174         
-       2024  3  8  60377       0.0258      0.2913      0.00157         
-       2024  3  9  60378       0.0252      0.2934      0.00104         
-       2024  3 10  60379       0.0245      0.2955      0.00017         
-       2024  3 11  60380       0.0239      0.2976     -0.00092         
-       2024  3 12  60381       0.0233      0.2997     -0.00205         
-       2024  3 13  60382       0.0228      0.3018     -0.00302         
-       2024  3 14  60383       0.0223      0.3040     -0.00370         
-       2024  3 15  60384       0.0218      0.3061     -0.00405         
-       2024  3 16  60385       0.0214      0.3082     -0.00411         
-       2024  3 17  60386       0.0210      0.3104     -0.00397         
-       2024  3 18  60387       0.0207      0.3125     -0.00373         
-       2024  3 19  60388       0.0203      0.3147     -0.00349         
-       2024  3 20  60389       0.0201      0.3168     -0.00334         
-       2024  3 21  60390       0.0198      0.3190     -0.00332         
-       2024  3 22  60391       0.0196      0.3211     -0.00348         
-       2024  3 23  60392       0.0195      0.3233     -0.00380         
-       2024  3 24  60393       0.0194      0.3255     -0.00427         
-       2024  3 25  60394       0.0193      0.3276     -0.00484         
-       2024  3 26  60395       0.0192      0.3298     -0.00544         
-       2024  3 27  60396       0.0192      0.3319     -0.00600         
-       2024  3 28  60397       0.0193      0.3341     -0.00645         
-       2024  3 29  60398       0.0193      0.3363     -0.00675         
-       2024  3 30  60399       0.0195      0.3384     -0.00687         
-       2024  3 31  60400       0.0196      0.3406     -0.00683         
-       2024  4  1  60401       0.0198      0.3427     -0.00666         
-       2024  4  2  60402       0.0200      0.3449     -0.00645         
-       2024  4  3  60403       0.0203      0.3470     -0.00633         
-       2024  4  4  60404       0.0205      0.3492     -0.00642         
-       2024  4  5  60405       0.0209      0.3513     -0.00684         
-       2024  4  6  60406       0.0212      0.3534     -0.00761         
-       2024  4  7  60407       0.0217      0.3555     -0.00867         
-       2024  4  8  60408       0.0221      0.3577     -0.00987         
-       2024  4  9  60409       0.0226      0.3598     -0.01101         
-       2024  4 10  60410       0.0231      0.3618     -0.01194         
-       2024  4 11  60411       0.0236      0.3639     -0.01253         
-       2024  4 12  60412       0.0242      0.3660     -0.01280         
-       2024  4 13  60413       0.0248      0.3681     -0.01281         
-       2024  4 14  60414       0.0255      0.3701     -0.01268         
-       2024  4 15  60415       0.0262      0.3722     -0.01252         
-       2024  4 16  60416       0.0269      0.3742     -0.01242         
-       2024  4 17  60417       0.0277      0.3762     -0.01245         
-       2024  4 18  60418       0.0284      0.3782     -0.01264         
-       2024  4 19  60419       0.0293      0.3802     -0.01300         
-       2024  4 20  60420       0.0301      0.3822     -0.01350         
-       2024  4 21  60421       0.0310      0.3842     -0.01411         
-       2024  4 22  60422       0.0319      0.3861     -0.01476         
-       2024  4 23  60423       0.0329      0.3880     -0.01538         
-       2024  4 24  60424       0.0339      0.3899     -0.01590         
-       2024  4 25  60425       0.0349      0.3918     -0.01626         
-       2024  4 26  60426       0.0359      0.3937     -0.01642         
-       2024  4 27  60427       0.0370      0.3956     -0.01638         
-       2024  4 28  60428       0.0381      0.3974     -0.01620         
-       2024  4 29  60429       0.0393      0.3993     -0.01591         
-       2024  4 30  60430       0.0405      0.4011     -0.01565         
-       2024  5  1  60431       0.0417      0.4028     -0.01554         
-       2024  5  2  60432       0.0429      0.4046     -0.01569         
-       2024  5  3  60433       0.0441      0.4064     -0.01614         
-       2024  5  4  60434       0.0454      0.4081     -0.01687         
-       2024  5  5  60435       0.0467      0.4098     -0.01779         
-       2024  5  6  60436       0.0481      0.4115     -0.01873         
-       2024  5  7  60437       0.0495      0.4131     -0.01952         
-       2024  5  8  60438       0.0508      0.4148     -0.02002         
-       2024  5  9  60439       0.0523      0.4164     -0.02017         
-       2024  5 10  60440       0.0537      0.4180     -0.02002         
-       2024  5 11  60441       0.0552      0.4196     -0.01966         
-       2024  5 12  60442       0.0567      0.4211     -0.01920         
-       2024  5 13  60443       0.0582      0.4226     -0.01876         
-       2024  5 14  60444       0.0598      0.4241     -0.01842         
-       2024  5 15  60445       0.0613      0.4256     -0.01821         
-       2024  5 16  60446       0.0629      0.4270     -0.01814         
-       2024  5 17  60447       0.0645      0.4284     -0.01821         
-       2024  5 18  60448       0.0662      0.4298     -0.01838         
-       2024  5 19  60449       0.0678      0.4312     -0.01859         
-       2024  5 20  60450       0.0695      0.4325     -0.01878         
-       2024  5 21  60451       0.0712      0.4339     -0.01888         
-       2024  5 22  60452       0.0729      0.4351     -0.01883         
-       2024  5 23  60453       0.0746      0.4364     -0.01858         
-       2024  5 24  60454       0.0764      0.4376     -0.01812         
-       2024  5 25  60455       0.0782      0.4388     -0.01748         
-       2024  5 26  60456       0.0800      0.4400     -0.01674         
-       2024  5 27  60457       0.0818      0.4411     -0.01600         
-       2024  5 28  60458       0.0836      0.4423     -0.01537         
-       2024  5 29  60459       0.0854      0.4433     -0.01495         
-       2024  5 30  60460       0.0873      0.4444     -0.01481         
-       2024  5 31  60461       0.0892      0.4454     -0.01493         
-       2024  6  1  60462       0.0910      0.4464     -0.01523         
-       2024  6  2  60463       0.0929      0.4474     -0.01558         
-       2024  6  3  60464       0.0948      0.4483     -0.01585         
-       2024  6  4  60465       0.0968      0.4492     -0.01588         
-       2024  6  5  60466       0.0987      0.4501     -0.01560         
-       2024  6  6  60467       0.1007      0.4509     -0.01501         
-       2024  6  7  60468       0.1026      0.4518     -0.01418         
-       2024  6  8  60469       0.1046      0.4525     -0.01321         
-       2024  6  9  60470       0.1066      0.4533     -0.01223         
-       2024  6 10  60471       0.1085      0.4540     -0.01133         
-       2024  6 11  60472       0.1105      0.4547     -0.01056         
-       2024  6 12  60473       0.1125      0.4553     -0.00994         
-       2024  6 13  60474       0.1146      0.4560     -0.00947         
-       2024  6 14  60475       0.1166      0.4566     -0.00911         
-       2024  6 15  60476       0.1186      0.4571     -0.00881         
-       2024  6 16  60477       0.1206      0.4576     -0.00852         
-       2024  6 17  60478       0.1227      0.4581     -0.00815         
-       2024  6 18  60479       0.1247      0.4586     -0.00767         
-       2024  6 19  60480       0.1267      0.4590     -0.00700         
-       2024  6 20  60481       0.1288      0.4594     -0.00614         
-       2024  6 21  60482       0.1308      0.4598     -0.00510         
-       2024  6 22  60483       0.1329      0.4601     -0.00394         
-       2024  6 23  60484       0.1349      0.4604     -0.00276         
-       2024  6 24  60485       0.1370      0.4607     -0.00167         
-       2024  6 25  60486       0.1390      0.4609     -0.00080         
-       2024  6 26  60487       0.1411      0.4611     -0.00021         
-       2024  6 27  60488       0.1431      0.4613      0.00012         
-       2024  6 28  60489       0.1452      0.4614      0.00025         
-       2024  6 29  60490       0.1472      0.4615      0.00032         
-       2024  6 30  60491       0.1493      0.4616      0.00046         
-       2024  7  1  60492       0.1513      0.4616      0.00080         
-       2024  7  2  60493       0.1534      0.4616      0.00143         
-       2024  7  3  60494       0.1554      0.4616      0.00235         
-       2024  7  4  60495       0.1574      0.4616      0.00352         
-       2024  7  5  60496       0.1594      0.4615      0.00486         
-       2024  7  6  60497       0.1615      0.4614      0.00624         
-       2024  7  7  60498       0.1635      0.4612      0.00758         
-       2024  7  8  60499       0.1655      0.4610      0.00881         
-       2024  7  9  60500       0.1675      0.4608      0.00989         
-       2024  7 10  60501       0.1695      0.4606      0.01083         
-       2024  7 11  60502       0.1714      0.4603      0.01167         
-       2024  7 12  60503       0.1734      0.4600      0.01245         
-       2024  7 13  60504       0.1754      0.4596      0.01324         
-       2024  7 14  60505       0.1773      0.4593      0.01410         
-       2024  7 15  60506       0.1793      0.4589      0.01510         
-       2024  7 16  60507       0.1812      0.4584      0.01628         
-       2024  7 17  60508       0.1831      0.4580      0.01765         
-       2024  7 18  60509       0.1850      0.4575      0.01920         
-       2024  7 19  60510       0.1869      0.4570      0.02085         
-       2024  7 20  60511       0.1888      0.4564      0.02251         
-       2024  7 21  60512       0.1906      0.4559      0.02402         
-       2024  7 22  60513       0.1925      0.4552      0.02524         
-       2024  7 23  60514       0.1943      0.4546      0.02607         
-       2024  7 24  60515       0.1961      0.4540      0.02651         
-       2024  7 25  60516       0.1979      0.4533      0.02662         
-       2024  7 26  60517       0.1997      0.4525      0.02657         
-       2024  7 27  60518       0.2015      0.4518      0.02653         
-       2024  7 28  60519       0.2032      0.4510      0.02666         
-       2024  7 29  60520       0.2050      0.4502      0.02706         
-       2024  7 30  60521       0.2067      0.4494      0.02776         
-       2024  7 31  60522       0.2084      0.4485      0.02874         
-       2024  8  1  60523       0.2100      0.4477      0.02990         
-       2024  8  2  60524       0.2117      0.4468      0.03114         
-       2024  8  3  60525       0.2133      0.4458      0.03235         
-       2024  8  4  60526       0.2149      0.4449      0.03344         
-       2024  8  5  60527       0.2165      0.4439      0.03435         
-       2024  8  6  60528       0.2181      0.4429      0.03505         
-       2024  8  7  60529       0.2197      0.4419      0.03555         
-       2024  8  8  60530       0.2212      0.4408      0.03590         
-       2024  8  9  60531       0.2227      0.4397      0.03617         
-       2024  8 10  60532       0.2242      0.4386      0.03643         
-       2024  8 11  60533       0.2256      0.4375      0.03678         
-       2024  8 12  60534       0.2271      0.4364      0.03727         
-       2024  8 13  60535       0.2285      0.4352      0.03795         
-       2024  8 14  60536       0.2299      0.4340      0.03881         
-       2024  8 15  60537       0.2312      0.4328      0.03978         
-       2024  8 16  60538       0.2326      0.4316      0.04079         
-       2024  8 17  60539       0.2339      0.4303      0.04171         
-       2024  8 18  60540       0.2352      0.4291      0.04241         
-       2024  8 19  60541       0.2364      0.4278      0.04277         
-       2024  8 20  60542       0.2377      0.4265      0.04275         
-       2024  8 21  60543       0.2389      0.4252      0.04243         
-       2024  8 22  60544       0.2401      0.4238      0.04198         
-       2024  8 23  60545       0.2412      0.4225      0.04158         
-       2024  8 24  60546       0.2423      0.4211      0.04130         
-       2024  8 25  60547       0.2434      0.4197      0.04132         
-       2024  8 26  60548       0.2445      0.4183      0.04169         
-       2024  8 27  60549       0.2456      0.4169      0.04230         
-       2024  8 28  60550       0.2466      0.4154      0.04309         
-       2024  8 29  60551       0.2476      0.4140      0.04383         
-       2024  8 30  60552       0.2485      0.4125      0.04456         
-       2024  8 31  60553       0.2495      0.4110      0.04513         
-       2024  9  1  60554       0.2504      0.4095      0.04555         
-       2024  9  2  60555       0.2512      0.4080      0.04572         
-       2024  9  3  60556       0.2521      0.4065      0.04574         
-       2024  9  4  60557       0.2529      0.4050      0.04570         
-       2024  9  5  60558       0.2537      0.4034      0.04552         
-       2024  9  6  60559       0.2544      0.4019      0.04537         
-       2024  9  7  60560       0.2551      0.4003      0.04528         
-       2024  9  8  60561       0.2558      0.3987      0.04535         
-       2024  9  9  60562       0.2565      0.3971      0.04553         
-       2024  9 10  60563       0.2571      0.3955      0.04588         
-       2024  9 11  60564       0.2577      0.3939      0.04634         
-       2024  9 12  60565       0.2583      0.3923      0.04687         
-       2024  9 13  60566       0.2588      0.3907      0.04743         
-       2024  9 14  60567       0.2593      0.3891      0.04783         
-       2024  9 15  60568       0.2598      0.3875      0.04791         
-       2024  9 16  60569       0.2603      0.3858      0.04757         
-       2024  9 17  60570       0.2607      0.3842      0.04683         
-       2024  9 18  60571       0.2611      0.3825      0.04578         
-       2024  9 19  60572       0.2614      0.3809      0.04452         
-       2024  9 20  60573       0.2617      0.3792      0.04335         
-       2024  9 21  60574       0.2620      0.3776      0.04234         
-       2024  9 22  60575       0.2623      0.3759      0.04164         
-       2024  9 23  60576       0.2625      0.3742      0.04119         
-       2024  9 24  60577       0.2627      0.3726      0.04092         
-       2024  9 25  60578       0.2629      0.3709      0.04076         
-       2024  9 26  60579       0.2630      0.3692      0.04068         
-       2024  9 27  60580       0.2631      0.3676      0.04054         
-       2024  9 28  60581       0.2632      0.3659      0.04023         
-       2024  9 29  60582       0.2632      0.3642      0.03981         
-       2024  9 30  60583       0.2633      0.3625      0.03932         
-       2024 10  1  60584       0.2632      0.3609      0.03868         
-       2024 10  2  60585       0.2632      0.3592      0.03808         
-       2024 10  3  60586       0.2631      0.3576      0.03742         
-       2024 10  4  60587       0.2630      0.3559      0.03696         
-       2024 10  5  60588       0.2629      0.3542      0.03663         
-       2024 10  6  60589       0.2627      0.3526      0.03651         
-       2024 10  7  60590       0.2625      0.3509      0.03662         
-       2024 10  8  60591       0.2623      0.3493      0.03680         
-       2024 10  9  60592       0.2620      0.3477      0.03706         
-       2024 10 10  60593       0.2617      0.3460      0.03740         
-       2024 10 11  60594       0.2614      0.3444      0.03769         
-       2024 10 12  60595       0.2611      0.3428      0.03785         
-       2024 10 13  60596       0.2607      0.3412      0.03770         
-       2024 10 14  60597       0.2603      0.3396      0.03720         
-       2024 10 15  60598       0.2599      0.3380      0.03641         
-       2024 10 16  60599       0.2594      0.3364      0.03545         
-       2024 10 17  60600       0.2589      0.3348      0.03445         
-       2024 10 18  60601       0.2584      0.3333      0.03369         
-       2024 10 19  60602       0.2579      0.3317      0.03321         
-       2024 10 20  60603       0.2573      0.3301      0.03312         
-       2024 10 21  60604       0.2567      0.3286      0.03325         
-       2024 10 22  60605       0.2561      0.3271      0.03351         
-       2024 10 23  60606       0.2554      0.3256      0.03374         
-       2024 10 24  60607       0.2547      0.3241      0.03400         
-       2024 10 25  60608       0.2540      0.3226      0.03410         
-       2024 10 26  60609       0.2533      0.3211      0.03405         
-       2024 10 27  60610       0.2526      0.3197      0.03380         
-       2024 10 28  60611       0.2518      0.3182      0.03337         
-       2024 10 29  60612       0.2510      0.3168      0.03280         
-       2024 10 30  60613       0.2501      0.3154      0.03220         
-       2024 10 31  60614       0.2493      0.3139      0.03171         
-       2024 11  1  60615       0.2484      0.3126      0.03140         
-       2024 11  2  60616       0.2475      0.3112      0.03131         
-       2024 11  3  60617       0.2466      0.3098      0.03143         
-       2024 11  4  60618       0.2456      0.3085      0.03169         
-       2024 11  5  60619       0.2447      0.3072      0.03211         
-       2024 11  6  60620       0.2437      0.3059      0.03257         
-       2024 11  7  60621       0.2427      0.3046      0.03302         
-       2024 11  8  60622       0.2416      0.3033      0.03332         
-       2024 11  9  60623       0.2406      0.3021      0.03342         
-       2024 11 10  60624       0.2395      0.3008      0.03324         
-       2024 11 11  60625       0.2384      0.2996      0.03282         
-       2024 11 12  60626       0.2373      0.2984      0.03212         
-       2024 11 13  60627       0.2362      0.2972      0.03137         
-       2024 11 14  60628       0.2350      0.2961      0.03065         
-       2024 11 15  60629       0.2339      0.2949      0.03010         
-       2024 11 16  60630       0.2327      0.2938      0.02989         
-       2024 11 17  60631       0.2315      0.2927      0.03005         
-       2024 11 18  60632       0.2302      0.2917      0.03041         
-       2024 11 19  60633       0.2290      0.2906      0.03087         
-       2024 11 20  60634       0.2277      0.2896      0.03122         
-       2024 11 21  60635       0.2265      0.2886      0.03145         
-       2024 11 22  60636       0.2252      0.2876      0.03152         
-       2024 11 23  60637       0.2239      0.2866      0.03139         
-       2024 11 24  60638       0.2226      0.2857      0.03110         
-       2024 11 25  60639       0.2212      0.2847      0.03056         
-       2024 11 26  60640       0.2199      0.2839      0.03008         
-       2024 11 27  60641       0.2185      0.2830      0.02962         
-       2024 11 28  60642       0.2172      0.2821      0.02924         
-       2024 11 29  60643       0.2158      0.2813      0.02903         
-       2024 11 30  60644       0.2144      0.2805      0.02896         
-       2024 12  1  60645       0.2130      0.2797      0.02909         
-       2024 12  2  60646       0.2116      0.2790      0.02938         
-       2024 12  3  60647       0.2101      0.2782      0.02978         
-       2024 12  4  60648       0.2087      0.2775      0.03018         
-       2024 12  5  60649       0.2072      0.2768      0.03055         
-       2024 12  6  60650       0.2058      0.2762      0.03074         
-       2024 12  7  60651       0.2043      0.2756      0.03067         
-       2024 12  8  60652       0.2029      0.2749      0.03022         
-       2024 12  9  60653       0.2014      0.2744      0.02965         
-       2024 12 10  60654       0.1999      0.2738      0.02901         
-       2024 12 11  60655       0.1984      0.2733      0.02835         
-       2024 12 12  60656       0.1969      0.2728      0.02778         
-       2024 12 13  60657       0.1954      0.2723      0.02751         
-       2024 12 14  60658       0.1939      0.2718      0.02763         
-       2024 12 15  60659       0.1924      0.2714      0.02810         
-       2024 12 16  60660       0.1909      0.2710      0.02864         
-       2024 12 17  60661       0.1893      0.2706      0.02923         
-       2024 12 18  60662       0.1878      0.2703      0.02974         
-       2024 12 19  60663       0.1863      0.2699      0.03008         
-       2024 12 20  60664       0.1848      0.2696      0.03032         
-       2024 12 21  60665       0.1832      0.2693      0.03035         
-       2024 12 22  60666       0.1817      0.2691      0.03026         
-       2024 12 23  60667       0.1802      0.2689      0.03011         
-       2024 12 24  60668       0.1786      0.2687      0.03000         
-       2024 12 25  60669       0.1771      0.2685      0.02991         
-       2024 12 26  60670       0.1756      0.2684      0.03001         
-       2024 12 27  60671       0.1741      0.2682      0.03030         
-       2024 12 28  60672       0.1725      0.2681      0.03085         
-       2024 12 29  60673       0.1710      0.2681      0.03161         
-       2024 12 30  60674       0.1695      0.2680      0.03245         
-       2024 12 31  60675       0.1680      0.2680      0.03326         
-       2025  1  1  60676       0.1665      0.2680      0.03395         
-       2025  1  2  60677       0.1649      0.2680      0.03445         
-       2025  1  3  60678       0.1634      0.2681      0.03478         
-       2025  1  4  60679       0.1619      0.2682      0.03485         
-       2025  1  5  60680       0.1604      0.2683      0.03466         
-       2025  1  6  60681       0.1590      0.2684      0.03433         
-       2025  1  7  60682       0.1575      0.2686      0.03399         
-       2025  1  8  60683       0.1560      0.2688      0.03381         
-       2025  1  9  60684       0.1545      0.2690      0.03397         
-       2025  1 10  60685       0.1531      0.2692      0.03443         
+       2024  3 29  60398      -0.0126      0.3355     -0.01421         
+       2024  3 30  60399      -0.0131      0.3380     -0.01443         
+       2024  3 31  60400      -0.0133      0.3405     -0.01443         
+       2024  4  1  60401      -0.0133      0.3430     -0.01424         
+       2024  4  2  60402      -0.0131      0.3454     -0.01392         
+       2024  4  3  60403      -0.0128      0.3479     -0.01360         
+       2024  4  4  60404      -0.0123      0.3504     -0.01346         
+       2024  4  5  60405      -0.0119      0.3529     -0.01363         
+       2024  4  6  60406      -0.0114      0.3555     -0.01414         
+       2024  4  7  60407      -0.0108      0.3580     -0.01499         
+       2024  4  8  60408      -0.0102      0.3605     -0.01606         
+       2024  4  9  60409      -0.0096      0.3630     -0.01716         
+       2024  4 10  60410      -0.0089      0.3655     -0.01807         
+       2024  4 11  60411      -0.0082      0.3680     -0.01870         
+       2024  4 12  60412      -0.0075      0.3704     -0.01900         
+       2024  4 13  60413      -0.0067      0.3728     -0.01906         
+       2024  4 14  60414      -0.0059      0.3752     -0.01899         
+       2024  4 15  60415      -0.0050      0.3776     -0.01888         
+       2024  4 16  60416      -0.0041      0.3800     -0.01882         
+       2024  4 17  60417      -0.0031      0.3824     -0.01888         
+       2024  4 18  60418      -0.0021      0.3847     -0.01908         
+       2024  4 19  60419      -0.0011      0.3870     -0.01944         
+       2024  4 20  60420       0.0000      0.3894     -0.01992         
+       2024  4 21  60421       0.0011      0.3916     -0.02048         
+       2024  4 22  60422       0.0023      0.3939     -0.02107         
+       2024  4 23  60423       0.0035      0.3962     -0.02162         
+       2024  4 24  60424       0.0047      0.3984     -0.02205         
+       2024  4 25  60425       0.0060      0.4006     -0.02230         
+       2024  4 26  60426       0.0073      0.4028     -0.02235         
+       2024  4 27  60427       0.0086      0.4050     -0.02220         
+       2024  4 28  60428       0.0100      0.4072     -0.02190         
+       2024  4 29  60429       0.0114      0.4093     -0.02154         
+       2024  4 30  60430       0.0128      0.4114     -0.02124         
+       2024  5  1  60431       0.0143      0.4135     -0.02111         
+       2024  5  2  60432       0.0158      0.4155     -0.02125         
+       2024  5  3  60433       0.0174      0.4176     -0.02171         
+       2024  5  4  60434       0.0190      0.4196     -0.02246         
+       2024  5  5  60435       0.0206      0.4216     -0.02341         
+       2024  5  6  60436       0.0222      0.4235     -0.02439         
+       2024  5  7  60437       0.0239      0.4255     -0.02523         
+       2024  5  8  60438       0.0256      0.4274     -0.02579         
+       2024  5  9  60439       0.0273      0.4292     -0.02603         
+       2024  5 10  60440       0.0291      0.4311     -0.02596         
+       2024  5 11  60441       0.0309      0.4329     -0.02570         
+       2024  5 12  60442       0.0327      0.4347     -0.02536         
+       2024  5 13  60443       0.0345      0.4365     -0.02503         
+       2024  5 14  60444       0.0364      0.4382     -0.02479         
+       2024  5 15  60445       0.0383      0.4399     -0.02467         
+       2024  5 16  60446       0.0403      0.4416     -0.02470         
+       2024  5 17  60447       0.0422      0.4432     -0.02486         
+       2024  5 18  60448       0.0442      0.4449     -0.02511         
+       2024  5 19  60449       0.0462      0.4464     -0.02541         
+       2024  5 20  60450       0.0482      0.4480     -0.02569         
+       2024  5 21  60451       0.0503      0.4495     -0.02588         
+       2024  5 22  60452       0.0524      0.4510     -0.02592         
+       2024  5 23  60453       0.0545      0.4525     -0.02577         
+       2024  5 24  60454       0.0566      0.4539     -0.02542         
+       2024  5 25  60455       0.0587      0.4553     -0.02490         
+       2024  5 26  60456       0.0609      0.4566     -0.02429         
+       2024  5 27  60457       0.0631      0.4579     -0.02368         
+       2024  5 28  60458       0.0653      0.4592     -0.02319         
+       2024  5 29  60459       0.0675      0.4605     -0.02291         
+       2024  5 30  60460       0.0697      0.4617     -0.02291         
+       2024  5 31  60461       0.0720      0.4629     -0.02316         
+       2024  6  1  60462       0.0742      0.4640     -0.02359         
+       2024  6  2  60463       0.0765      0.4651     -0.02407         
+       2024  6  3  60464       0.0788      0.4662     -0.02445         
+       2024  6  4  60465       0.0811      0.4672     -0.02459         
+       2024  6  5  60466       0.0835      0.4682     -0.02441         
+       2024  6  6  60467       0.0858      0.4692     -0.02391         
+       2024  6  7  60468       0.0882      0.4701     -0.02316         
+       2024  6  8  60469       0.0905      0.4710     -0.02227         
+       2024  6  9  60470       0.0929      0.4719     -0.02134         
+       2024  6 10  60471       0.0953      0.4727     -0.02048         
+       2024  6 11  60472       0.0977      0.4735     -0.01974         
+       2024  6 12  60473       0.1001      0.4742     -0.01913         
+       2024  6 13  60474       0.1025      0.4749     -0.01866         
+       2024  6 14  60475       0.1050      0.4756     -0.01829         
+       2024  6 15  60476       0.1074      0.4762     -0.01797         
+       2024  6 16  60477       0.1098      0.4768     -0.01766         
+       2024  6 17  60478       0.1123      0.4774     -0.01727         
+       2024  6 18  60479       0.1147      0.4779     -0.01675         
+       2024  6 19  60480       0.1172      0.4784     -0.01605         
+       2024  6 20  60481       0.1196      0.4788     -0.01514         
+       2024  6 21  60482       0.1221      0.4792     -0.01405         
+       2024  6 22  60483       0.1246      0.4796     -0.01282         
+       2024  6 23  60484       0.1270      0.4799     -0.01156         
+       2024  6 24  60485       0.1295      0.4802     -0.01039         
+       2024  6 25  60486       0.1320      0.4804     -0.00943         
+       2024  6 26  60487       0.1344      0.4806     -0.00874         
+       2024  6 27  60488       0.1369      0.4808     -0.00832         
+       2024  6 28  60489       0.1394      0.4809     -0.00809         
+       2024  6 29  60490       0.1418      0.4810     -0.00793         
+       2024  6 30  60491       0.1443      0.4811     -0.00769         
+       2024  7  1  60492       0.1467      0.4811     -0.00725         
+       2024  7  2  60493       0.1492      0.4811     -0.00653         
+       2024  7  3  60494       0.1516      0.4810     -0.00552         
+       2024  7  4  60495       0.1541      0.4809     -0.00425         
+       2024  7  5  60496       0.1565      0.4808     -0.00284         
+       2024  7  6  60497       0.1589      0.4806     -0.00138         
+       2024  7  7  60498       0.1613      0.4804      0.00002         
+       2024  7  8  60499       0.1638      0.4802      0.00129         
+       2024  7  9  60500       0.1662      0.4799      0.00239         
+       2024  7 10  60501       0.1686      0.4795      0.00334         
+       2024  7 11  60502       0.1709      0.4792      0.00416         
+       2024  7 12  60503       0.1733      0.4788      0.00490         
+       2024  7 13  60504       0.1757      0.4784      0.00562         
+       2024  7 14  60505       0.1780      0.4779      0.00638         
+       2024  7 15  60506       0.1804      0.4774      0.00720         
+       2024  7 16  60507       0.1827      0.4769      0.00817         
+       2024  7 17  60508       0.1850      0.4763      0.00931         
+       2024  7 18  60509       0.1873      0.4757      0.01063         
+       2024  7 19  60510       0.1896      0.4750      0.01207         
+       2024  7 20  60511       0.1918      0.4743      0.01357         
+       2024  7 21  60512       0.1941      0.4736      0.01499         
+       2024  7 22  60513       0.1963      0.4729      0.01620         
+       2024  7 23  60514       0.1985      0.4721      0.01711         
+       2024  7 24  60515       0.2007      0.4713      0.01770         
+       2024  7 25  60516       0.2029      0.4704      0.01804         
+       2024  7 26  60517       0.2050      0.4695      0.01827         
+       2024  7 27  60518       0.2072      0.4686      0.01854         
+       2024  7 28  60519       0.2093      0.4677      0.01900         
+       2024  7 29  60520       0.2114      0.4667      0.01973         
+       2024  7 30  60521       0.2135      0.4657      0.02074         
+       2024  7 31  60522       0.2155      0.4646      0.02199         
+       2024  8  1  60523       0.2175      0.4635      0.02340         
+       2024  8  2  60524       0.2195      0.4624      0.02486         
+       2024  8  3  60525       0.2215      0.4613      0.02626         
+       2024  8  4  60526       0.2235      0.4601      0.02752         
+       2024  8  5  60527       0.2254      0.4589      0.02862         
+       2024  8  6  60528       0.2273      0.4577      0.02952         
+       2024  8  7  60529       0.2292      0.4565      0.03027         
+       2024  8  8  60530       0.2311      0.4552      0.03089         
+       2024  8  9  60531       0.2329      0.4539      0.03147         
+       2024  8 10  60532       0.2347      0.4525      0.03206         
+       2024  8 11  60533       0.2365      0.4511      0.03272         
+       2024  8 12  60534       0.2382      0.4498      0.03351         
+       2024  8 13  60535       0.2400      0.4483      0.03445         
+       2024  8 14  60536       0.2417      0.4469      0.03555         
+       2024  8 15  60537       0.2433      0.4454      0.03678         
+       2024  8 16  60538       0.2450      0.4439      0.03807         
+       2024  8 17  60539       0.2466      0.4424      0.03932         
+       2024  8 18  60540       0.2481      0.4409      0.04039         
+       2024  8 19  60541       0.2497      0.4393      0.04116         
+       2024  8 20  60542       0.2512      0.4377      0.04157         
+       2024  8 21  60543       0.2527      0.4361      0.04165         
+       2024  8 22  60544       0.2541      0.4344      0.04152         
+       2024  8 23  60545       0.2555      0.4328      0.04135         
+       2024  8 24  60546       0.2569      0.4311      0.04134         
+       2024  8 25  60547       0.2583      0.4294      0.04159         
+       2024  8 26  60548       0.2596      0.4277      0.04215         
+       2024  8 27  60549       0.2609      0.4260      0.04298         
+       2024  8 28  60550       0.2622      0.4242      0.04398         
+       2024  8 29  60551       0.2634      0.4224      0.04504         
+       2024  8 30  60552       0.2646      0.4206      0.04605         
+       2024  8 31  60553       0.2657      0.4188      0.04694         
+       2024  9  1  60554       0.2668      0.4170      0.04766         
+       2024  9  2  60555       0.2679      0.4152      0.04817         
+       2024  9  3  60556       0.2690      0.4133      0.04851         
+       2024  9  4  60557       0.2700      0.4114      0.04871         
+       2024  9  5  60558       0.2710      0.4095      0.04882         
+       2024  9  6  60559       0.2719      0.4076      0.04893         
+       2024  9  7  60560       0.2728      0.4057      0.04909         
+       2024  9  8  60561       0.2737      0.4038      0.04936         
+       2024  9  9  60562       0.2745      0.4018      0.04978         
+       2024  9 10  60563       0.2753      0.3999      0.05035         
+       2024  9 11  60564       0.2761      0.3979      0.05105         
+       2024  9 12  60565       0.2768      0.3960      0.05184         
+       2024  9 13  60566       0.2775      0.3940      0.05263         
+       2024  9 14  60567       0.2782      0.3920      0.05329         
+       2024  9 15  60568       0.2788      0.3900      0.05370         
+       2024  9 16  60569       0.2794      0.3880      0.05376         
+       2024  9 17  60570       0.2799      0.3859      0.05345         
+       2024  9 18  60571       0.2804      0.3839      0.05284         
+       2024  9 19  60572       0.2809      0.3819      0.05210         
+       2024  9 20  60573       0.2813      0.3798      0.05144         
+       2024  9 21  60574       0.2817      0.3778      0.05101         
+       2024  9 22  60575       0.2821      0.3757      0.05092         
+       2024  9 23  60576       0.2824      0.3737      0.05116         
+       2024  9 24  60577       0.2827      0.3716      0.05164         
+       2024  9 25  60578       0.2830      0.3696      0.05224         
+       2024  9 26  60579       0.2832      0.3675      0.05285         
+       2024  9 27  60580       0.2834      0.3655      0.05337         
+       2024  9 28  60581       0.2835      0.3634      0.05375         
+       2024  9 29  60582       0.2836      0.3613      0.05397         
+       2024  9 30  60583       0.2837      0.3593      0.05405         
+       2024 10  1  60584       0.2837      0.3572      0.05401         
+       2024 10  2  60585       0.2837      0.3551      0.05393         
+       2024 10  3  60586       0.2836      0.3531      0.05385         
+       2024 10  4  60587       0.2836      0.3510      0.05386         
+       2024 10  5  60588       0.2834      0.3489      0.05399         
+       2024 10  6  60589       0.2833      0.3469      0.05427         
+       2024 10  7  60590       0.2831      0.3448      0.05471         
+       2024 10  8  60591       0.2829      0.3428      0.05528         
+       2024 10  9  60592       0.2826      0.3407      0.05593         
+       2024 10 10  60593       0.2823      0.3387      0.05659         
+       2024 10 11  60594       0.2820      0.3367      0.05718         
+       2024 10 12  60595       0.2816      0.3347      0.05756         
+       2024 10 13  60596       0.2812      0.3326      0.05764         
+       2024 10 14  60597       0.2808      0.3306      0.05737         
+       2024 10 15  60598       0.2803      0.3286      0.05676         
+       2024 10 16  60599       0.2798      0.3266      0.05594         
+       2024 10 17  60600       0.2793      0.3247      0.05508         
+       2024 10 18  60601       0.2787      0.3227      0.05437         
+       2024 10 19  60602       0.2781      0.3207      0.05398         
+       2024 10 20  60603       0.2774      0.3188      0.05394         
+       2024 10 21  60604       0.2767      0.3168      0.05419         
+       2024 10 22  60605       0.2760      0.3149      0.05463         
+       2024 10 23  60606       0.2753      0.3130      0.05511         
+       2024 10 24  60607       0.2745      0.3111      0.05551         
+       2024 10 25  60608       0.2737      0.3092      0.05577         
+       2024 10 26  60609       0.2729      0.3073      0.05583         
+       2024 10 27  60610       0.2720      0.3055      0.05571         
+       2024 10 28  60611       0.2711      0.3036      0.05544         
+       2024 10 29  60612       0.2702      0.3018      0.05506         
+       2024 10 30  60613       0.2692      0.3000      0.05464         
+       2024 10 31  60614       0.2682      0.2982      0.05426         
+       2024 11  1  60615       0.2672      0.2964      0.05396         
+       2024 11  2  60616       0.2662      0.2947      0.05381         
+       2024 11  3  60617       0.2651      0.2929      0.05386         
+       2024 11  4  60618       0.2640      0.2912      0.05411         
+       2024 11  5  60619       0.2629      0.2895      0.05446         
+       2024 11  6  60620       0.2617      0.2878      0.05480         
+       2024 11  7  60621       0.2605      0.2861      0.05508         
+       2024 11  8  60622       0.2593      0.2845      0.05517         
+       2024 11  9  60623       0.2580      0.2828      0.05507         
+       2024 11 10  60624       0.2568      0.2812      0.05458         
+       2024 11 11  60625       0.2555      0.2796      0.05385         
+       2024 11 12  60626       0.2542      0.2781      0.05292         
+       2024 11 13  60627       0.2528      0.2765      0.05186         
+       2024 11 14  60628       0.2514      0.2750      0.05090         
+       2024 11 15  60629       0.2501      0.2735      0.05022         
+       2024 11 16  60630       0.2486      0.2720      0.04990         
+       2024 11 17  60631       0.2472      0.2706      0.04987         
+       2024 11 18  60632       0.2457      0.2692      0.05009         
+       2024 11 19  60633       0.2443      0.2678      0.05045         
+       2024 11 20  60634       0.2428      0.2664      0.05076         
+       2024 11 21  60635       0.2412      0.2650      0.05084         
+       2024 11 22  60636       0.2397      0.2637      0.05069         
+       2024 11 23  60637       0.2381      0.2624      0.05040         
+       2024 11 24  60638       0.2365      0.2611      0.04992         
+       2024 11 25  60639       0.2349      0.2599      0.04937         
+       2024 11 26  60640       0.2333      0.2586      0.04882         
+       2024 11 27  60641       0.2317      0.2574      0.04824         
+       2024 11 28  60642       0.2300      0.2563      0.04776         
+       2024 11 29  60643       0.2283      0.2551      0.04745         
+       2024 11 30  60644       0.2267      0.2540      0.04727         
+       2024 12  1  60645       0.2250      0.2529      0.04722         
+       2024 12  2  60646       0.2232      0.2519      0.04730         
+       2024 12  3  60647       0.2215      0.2508      0.04755         
+       2024 12  4  60648       0.2197      0.2498      0.04779         
+       2024 12  5  60649       0.2180      0.2488      0.04784         
+       2024 12  6  60650       0.2162      0.2479      0.04768         
+       2024 12  7  60651       0.2144      0.2470      0.04723         
+       2024 12  8  60652       0.2126      0.2461      0.04649         
+       2024 12  9  60653       0.2108      0.2452      0.04548         
+       2024 12 10  60654       0.2090      0.2444      0.04429         
+       2024 12 11  60655       0.2072      0.2436      0.04316         
+       2024 12 12  60656       0.2053      0.2428      0.04221         
+       2024 12 13  60657       0.2035      0.2421      0.04155         
+       2024 12 14  60658       0.2016      0.2414      0.04121         
+       2024 12 15  60659       0.1997      0.2407      0.04110         
+       2024 12 16  60660       0.1979      0.2400      0.04115         
+       2024 12 17  60661       0.1960      0.2394      0.04122         
+       2024 12 18  60662       0.1941      0.2388      0.04114         
+       2024 12 19  60663       0.1922      0.2382      0.04088         
+       2024 12 20  60664       0.1903      0.2377      0.04046         
+       2024 12 21  60665       0.1884      0.2372      0.03987         
+       2024 12 22  60666       0.1865      0.2367      0.03928         
+       2024 12 23  60667       0.1846      0.2363      0.03871         
+       2024 12 24  60668       0.1827      0.2359      0.03818         
+       2024 12 25  60669       0.1808      0.2355      0.03783         
+       2024 12 26  60670       0.1788      0.2352      0.03761         
+       2024 12 27  60671       0.1769      0.2348      0.03760         
+       2024 12 28  60672       0.1750      0.2346      0.03792         
+       2024 12 29  60673       0.1731      0.2343      0.03825         
+       2024 12 30  60674       0.1712      0.2341      0.03878         
+       2024 12 31  60675       0.1693      0.2339      0.03932         
+       2025  1  1  60676       0.1674      0.2337      0.03987         
+       2025  1  2  60677       0.1654      0.2336      0.04015         
+       2025  1  3  60678       0.1635      0.2335      0.04013         
+       2025  1  4  60679       0.1616      0.2334      0.03978         
+       2025  1  5  60680       0.1597      0.2334      0.03922         
+       2025  1  6  60681       0.1578      0.2334      0.03839         
+       2025  1  7  60682       0.1559      0.2334      0.03752         
+       2025  1  8  60683       0.1541      0.2334      0.03679         
+       2025  1  9  60684       0.1522      0.2335      0.03622         
+       2025  1 10  60685       0.1503      0.2336      0.03592         
+       2025  1 11  60686       0.1484      0.2338      0.03595         
+       2025  1 12  60687       0.1466      0.2339      0.03618         
+       2025  1 13  60688       0.1447      0.2341      0.03653         
+       2025  1 14  60689       0.1429      0.2344      0.03683         
+       2025  1 15  60690       0.1411      0.2346      0.03699         
+       2025  1 16  60691       0.1392      0.2349      0.03687         
+       2025  1 17  60692       0.1374      0.2352      0.03658         
+       2025  1 18  60693       0.1356      0.2356      0.03608         
+       2025  1 19  60694       0.1339      0.2360      0.03549         
+       2025  1 20  60695       0.1321      0.2364      0.03484         
+       2025  1 21  60696       0.1303      0.2368      0.03423         
+       2025  1 22  60697       0.1286      0.2372      0.03376         
+       2025  1 23  60698       0.1268      0.2377      0.03354         
+       2025  1 24  60699       0.1251      0.2382      0.03357         
+       2025  1 25  60700       0.1234      0.2388      0.03373         
+       2025  1 26  60701       0.1217      0.2394      0.03404         
+       2025  1 27  60702       0.1200      0.2399      0.03442         
+       2025  1 28  60703       0.1184      0.2406      0.03473         
+       2025  1 29  60704       0.1167      0.2412      0.03486         
+       2025  1 30  60705       0.1151      0.2419      0.03461         
+       2025  1 31  60706       0.1135      0.2426      0.03407         
+       2025  2  1  60707       0.1119      0.2433      0.03321         
+       2025  2  2  60708       0.1103      0.2441      0.03218         
+       2025  2  3  60709       0.1088      0.2448      0.03108         
+       2025  2  4  60710       0.1072      0.2456      0.03013         
+       2025  2  5  60711       0.1057      0.2465      0.02949         
+       2025  2  6  60712       0.1042      0.2473      0.02910         
+       2025  2  7  60713       0.1027      0.2482      0.02899         
+       2025  2  8  60714       0.1013      0.2491      0.02908         
+       2025  2  9  60715       0.0998      0.2500      0.02929         
+       2025  2 10  60716       0.0984      0.2509      0.02940         
+       2025  2 11  60717       0.0970      0.2519      0.02939         
+       2025  2 12  60718       0.0957      0.2529      0.02917         
+       2025  2 13  60719       0.0943      0.2539      0.02873         
+       2025  2 14  60720       0.0930      0.2549      0.02815         
+       2025  2 15  60721       0.0917      0.2559      0.02742         
+       2025  2 16  60722       0.0904      0.2570      0.02660         
+       2025  2 17  60723       0.0891      0.2581      0.02574         
+       2025  2 18  60724       0.0879      0.2592      0.02496         
+       2025  2 19  60725       0.0867      0.2603      0.02431         
+       2025  2 20  60726       0.0855      0.2615      0.02375         
+       2025  2 21  60727       0.0844      0.2626      0.02338         
+       2025  2 22  60728       0.0832      0.2638      0.02308         
+       2025  2 23  60729       0.0821      0.2650      0.02281         
+       2025  2 24  60730       0.0810      0.2662      0.02246         
+       2025  2 25  60731       0.0800      0.2675      0.02192         
+       2025  2 26  60732       0.0790      0.2687      0.02113         
+       2025  2 27  60733       0.0780      0.2700      0.02010         
+       2025  2 28  60734       0.0770      0.2713      0.01878         
+       2025  3  1  60735       0.0760      0.2726      0.01719         
+       2025  3  2  60736       0.0751      0.2739      0.01557         
+       2025  3  3  60737       0.0742      0.2752      0.01413         
+       2025  3  4  60738       0.0733      0.2765      0.01292         
+       2025  3  5  60739       0.0725      0.2779      0.01216         
+       2025  3  6  60740       0.0717      0.2792      0.01166         
+       2025  3  7  60741       0.0709      0.2806      0.01154         
+       2025  3  8  60742       0.0702      0.2820      0.01155         
+       2025  3  9  60743       0.0694      0.2834      0.01160         
+       2025  3 10  60744       0.0687      0.2848      0.01160         
+       2025  3 11  60745       0.0681      0.2862      0.01134         
+       2025  3 12  60746       0.0674      0.2877      0.01086         
+       2025  3 13  60747       0.0668      0.2891      0.01024         
+       2025  3 14  60748       0.0662      0.2905      0.00952         
+       2025  3 15  60749       0.0657      0.2920      0.00879         
+       2025  3 16  60750       0.0652      0.2935      0.00806         
+       2025  3 17  60751       0.0647      0.2949      0.00742         
+       2025  3 18  60752       0.0642      0.2964      0.00697         
+       2025  3 19  60753       0.0638      0.2979      0.00673         
+       2025  3 20  60754       0.0634      0.2994      0.00667         
+       2025  3 21  60755       0.0630      0.3009      0.00685         
+       2025  3 22  60756       0.0626      0.3024      0.00711         
+       2025  3 23  60757       0.0623      0.3039      0.00742         
+       2025  3 24  60758       0.0620      0.3054      0.00759         
+       2025  3 25  60759       0.0618      0.3069      0.00751         
+       2025  3 26  60760       0.0616      0.3085      0.00707         
+       2025  3 27  60761       0.0614      0.3100      0.00638         
+       2025  3 28  60762       0.0612      0.3115      0.00535         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      60307  -111.33    0.59   -6.11    0.22   
+                      60375  -109.99    0.77   -8.31    0.25   
+                      60376  -110.26    0.77   -8.55    0.25   
+                      60377  -110.14    0.77   -8.82    0.25   
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      60307    0.239  0.233   -0.211   0.221          
+                      60375    0.292  0.306   -0.221   0.246          
+                      60376    0.292  0.306   -0.222   0.246          
+                      60377    0.291  0.306   -0.222   0.246
```

### Comparing `pyTMD-2.1.0/pyTMD/data/tab5.2e.txt` & `pyTMD-2.1.1/pyTMD/data/tab5.2e.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/tab5.3a.txt` & `pyTMD-2.1.1/pyTMD/data/tab5.3a.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/data/tab5.3b.txt` & `pyTMD-2.1.1/pyTMD/data/tab5.3b.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/eop.py` & `pyTMD-2.1.1/pyTMD/eop.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,17 @@
         return buffer
 
     # raise exception
     raise RuntimeError(f'Unable to download {FILE}')
 
 # PURPOSE: connects to servers and downloads finals files
 def update_finals_file(
-        username: str or None = None,
-        password: str or None = None,
-        timeout: int or None = 20,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = 20,
         verbose: bool = False,
         mode: oct = 0o775
     ):
     """
     Connects to servers and downloads finals EOP files
 
     Servers and Mirrors
```

### Comparing `pyTMD-2.1.0/pyTMD/interpolate.py` & `pyTMD-2.1.1/pyTMD/interpolate.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         ilat: np.ndarray,
         idata: np.ndarray,
         lon: np.ndarray,
         lat: np.ndarray,
         fill_value: float = None,
         dtype: str | np.dtype = np.float64,
         cutoff: int | float = np.inf,
-        EPSG: str or int = '4326',
+        EPSG: str | int = '4326',
         **kwargs
     ):
     """
     Nearest-neighbor (`NN`) extrapolation of valid model data using `kd-trees
     <https://docs.scipy.org/doc/scipy/reference/generated/
     scipy.spatial.cKDTree.html>`_
```

### Comparing `pyTMD-2.1.0/pyTMD/io/ATLAS.py` & `pyTMD-2.1.1/pyTMD/io/ATLAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 ATLAS.py
-Written by Tyler Sutterley (10/2023)
+Written by Tyler Sutterley (02/2024)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 netCDF4 files can be been compressed using gzip
 
 Reads netCDF4 ATLAS tidal solutions provided by Ohio State University and ESR
@@ -51,14 +51,15 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 02/2024: changed variable for setting global grid flag to is_global
     Updated 10/2023: add generic wrapper function for reading constituents
     Updated 04/2023: using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output ATLAS formatted netCDF4 files
         refactored interpolation routines into new module
@@ -215,21 +216,21 @@
         # input points convention (0:360)
         # tide model convention (-180:180)
         ilon[ilon > 180.0] -= 360.0
 
     # grid step size of tide model
     dlon = lon[1] - lon[0]
     # if global: extend limits
-    global_grid = False
+    is_global = False
     # replace original values with extend arrays/matrices
     if np.isclose(lon[-1] - lon[0], 360.0 - dlon):
-        lon = extend_array(lon, dlon)
-        bathymetry = extend_matrix(bathymetry)
+        lon = _extend_array(lon, dlon)
+        bathymetry = _extend_matrix(bathymetry)
         # set global grid flag
-        global_grid = True
+        is_global = True
     # create masks
     bathymetry.mask = (bathymetry.data == 0)
     # determine if any input points are outside of the model bounds
     invalid = (ilon < lon.min()) | (ilon > lon.max()) | \
               (ilat < lat.min()) | (ilat > lat.max())
 
     # number of points
@@ -278,16 +279,16 @@
             raise FileNotFoundError(str(model_file))
         # read constituent from netCDF4 file
         hc, cons = read_netcdf_file(model_file, kwargs['type'],
             compressed=kwargs['compressed'])
         # append constituent to list
         constituents.append(cons)
         # replace original values with extend matrices
-        if global_grid:
-            hc = extend_matrix(hc)
+        if is_global:
+            hc = _extend_matrix(hc)
         # update constituent mask with bathymetry mask
         hc.mask[:] |= bathymetry.mask[:]
         # interpolate amplitude and phase of the constituent
         if (kwargs['method'] == 'bilinear'):
             # replace invalid values with nan
             hc.data[hc.mask] = np.nan
             hci = pyTMD.interpolate.bilinear(lon, lat, hc, ilon, ilat,
@@ -390,16 +391,16 @@
     # read the tide grid file for bathymetry and spatial coordinates
     lon, lat, bathymetry = read_netcdf_grid(grid_file, kwargs['type'],
         compressed=kwargs['compressed'])
 
     # grid step size of tide model
     dlon = lon[1] - lon[0]
     # replace original values with extend arrays/matrices
-    lon = extend_array(lon, dlon)
-    bathymetry = extend_matrix(bathymetry)
+    lon = _extend_array(lon, dlon)
+    bathymetry = _extend_matrix(bathymetry)
     # save output constituents
     constituents = pyTMD.io.constituents(
         longitude=lon,
         latitude=lat,
         bathymetry=bathymetry.data,
         mask=bathymetry.mask
         )
@@ -410,15 +411,15 @@
         model_file = pathlib.Path(model_file).expanduser()
         if not model_file.exists():
             raise FileNotFoundError(str(model_file))
         # read constituent from netCDF4 file
         hc, cons = read_netcdf_file(model_file, kwargs['type'],
             compressed=kwargs['compressed'])
         # replace original values with extend matrices
-        hc = extend_matrix(hc)
+        hc = _extend_matrix(hc)
         hc.mask[:] |= bathymetry.mask[:]
         # append extended constituent
         constituents.append(cons,  hc)
 
     # return the complex form of the model constituents
     return constituents
 
@@ -607,61 +608,14 @@
     amplitude = ampl*kwargs['scale']
     # convert phase to degrees
     phase = ph*180.0/np.pi
     phase[phase < 0] += 360.0
     # return the interpolated values
     return (amplitude, phase, D)
 
-# PURPOSE: Extend a longitude array
-def extend_array(input_array: np.ndarray, step_size: float):
-    """
-    Extends a longitude array
-
-    Parameters
-    ----------
-    input_array: np.ndarray
-        array to extend
-    step_size: float
-        step size between elements of array
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended array
-    """
-    n = len(input_array)
-    temp = np.zeros((n+2), dtype=input_array.dtype)
-    # extended array [x-1,x0,...,xN,xN+1]
-    temp[0] = input_array[0] - step_size
-    temp[1:-1] = input_array[:]
-    temp[-1] = input_array[-1] + step_size
-    return temp
-
-# PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix: np.ndarray):
-    """
-    Extends a global matrix
-
-    Parameters
-    ----------
-    input_matrix: np.ndarray
-        matrix to extend
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended matrix
-    """
-    ny, nx = np.shape(input_matrix)
-    temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
-    temp[:,0] = input_matrix[:,-1]
-    temp[:,1:-1] = input_matrix[:,:]
-    temp[:,-1] = input_matrix[:,0]
-    return temp
-
 # PURPOSE: read grid file
 def read_netcdf_grid(
         input_file: str | pathlib.Path,
         variable: str,
         **kwargs
     ):
     """
@@ -1173,7 +1127,54 @@
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
     logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
+
+# PURPOSE: Extend a longitude array
+def _extend_array(input_array: np.ndarray, step_size: float):
+    """
+    Extends a longitude array
+
+    Parameters
+    ----------
+    input_array: np.ndarray
+        array to extend
+    step_size: float
+        step size between elements of array
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended array
+    """
+    n = len(input_array)
+    temp = np.zeros((n+2), dtype=input_array.dtype)
+    # extended array [x-1,x0,...,xN,xN+1]
+    temp[0] = input_array[0] - step_size
+    temp[1:-1] = input_array[:]
+    temp[-1] = input_array[-1] + step_size
+    return temp
+
+# PURPOSE: Extend a global matrix
+def _extend_matrix(input_matrix: np.ndarray):
+    """
+    Extends a global matrix
+
+    Parameters
+    ----------
+    input_matrix: np.ndarray
+        matrix to extend
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended matrix
+    """
+    ny, nx = np.shape(input_matrix)
+    temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
+    temp[:,0] = input_matrix[:,-1]
+    temp[:,1:-1] = input_matrix[:,:]
+    temp[:,-1] = input_matrix[:,0]
+    return temp
```

### Comparing `pyTMD-2.1.0/pyTMD/io/FES.py` & `pyTMD-2.1.1/pyTMD/io/FES.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,16 +232,16 @@
             # tide model convention (-180:180)
             ilon[ilon>180.0] -= 360.0
 
         # grid step size of tide model
         dlon = lon[1] - lon[0]
         # replace original values with extend arrays/matrices
         if np.isclose(lon[-1] - lon[0], 360.0 - dlon):
-            lon = extend_array(lon, dlon)
-            hc = extend_matrix(hc)
+            lon = _extend_array(lon, dlon)
+            hc = _extend_matrix(hc)
         # determine if any input points are outside of the model bounds
         invalid = (ilon < lon.min()) | (ilon > lon.max()) | \
                   (ilat < lat.min()) | (ilat > lat.max())
 
         # interpolate amplitude and phase of the constituent
         if (kwargs['method'] == 'bilinear'):
             # replace invalid values with nan
@@ -366,16 +366,16 @@
         elif kwargs['version'] in ('FES2012','FES2014','EOT20','HAMTIDE11'):
             # FES netCDF4 constituent files
             hc, lon, lat = read_netcdf_file(model_file, **kwargs)
         # grid step size of tide model
         dlon = lon[1] - lon[0]
         # replace original values with extend arrays/matrices
         if np.isclose(lon[-1] - lon[0], 360.0 - dlon):
-            lon = extend_array(lon, dlon)
-            hc = extend_matrix(hc)
+            lon = _extend_array(lon, dlon)
+            hc = _extend_matrix(hc)
         # append extended constituent
         constituents.append(cons, hc)
         # set model coordinates
         setattr(constituents, 'longitude', lon)
         setattr(constituents, 'latitude', lat)
 
     # return the complex form of the model constituents
@@ -528,61 +528,14 @@
     phase.data[phase.data < 0] += 360.0
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
-# PURPOSE: Extend a longitude array
-def extend_array(input_array: np.ndarray, step_size: float):
-    """
-    Extends a longitude array
-
-    Parameters
-    ----------
-    input_array: np.ndarray
-        array to extend
-    step_size: float
-        step size between elements of array
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended array
-    """
-    n = len(input_array)
-    temp = np.zeros((n+2), dtype=input_array.dtype)
-    # extended array [x-1,x0,...,xN,xN+1]
-    temp[0] = input_array[0] - step_size
-    temp[1:-1] = input_array[:]
-    temp[-1] = input_array[-1] + step_size
-    return temp
-
-# PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix: np.ndarray):
-    """
-    Extends a global matrix
-
-    Parameters
-    ----------
-    input_matrix: np.ndarray
-        matrix to extend
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended matrix
-    """
-    ny, nx = np.shape(input_matrix)
-    temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
-    temp[:,0] = input_matrix[:,-1]
-    temp[:,1:-1] = input_matrix[:,:]
-    temp[:,-1] = input_matrix[:,0]
-    return temp
-
 # PURPOSE: read FES ascii tide model grid files
 def read_ascii_file(
         input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read FES (Finite Element Solution) tide model file
@@ -846,7 +799,54 @@
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
     logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
+
+# PURPOSE: Extend a longitude array
+def _extend_array(input_array: np.ndarray, step_size: float):
+    """
+    Extends a longitude array
+
+    Parameters
+    ----------
+    input_array: np.ndarray
+        array to extend
+    step_size: float
+        step size between elements of array
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended array
+    """
+    n = len(input_array)
+    temp = np.zeros((n+2), dtype=input_array.dtype)
+    # extended array [x-1,x0,...,xN,xN+1]
+    temp[0] = input_array[0] - step_size
+    temp[1:-1] = input_array[:]
+    temp[-1] = input_array[-1] + step_size
+    return temp
+
+# PURPOSE: Extend a global matrix
+def _extend_matrix(input_matrix: np.ndarray):
+    """
+    Extends a global matrix
+
+    Parameters
+    ----------
+    input_matrix: np.ndarray
+        matrix to extend
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended matrix
+    """
+    ny, nx = np.shape(input_matrix)
+    temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
+    temp[:,0] = input_matrix[:,-1]
+    temp[:,1:-1] = input_matrix[:,:]
+    temp[:,-1] = input_matrix[:,0]
+    return temp
```

### Comparing `pyTMD-2.1.0/pyTMD/io/GOT.py` & `pyTMD-2.1.1/pyTMD/io/GOT.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,16 +215,16 @@
         elif (np.max(ilon) > 180.0) & (np.min(lon) < 0.0):
             # input points convention (0:360)
             # tide model convention (-180:180)
             ilon[ilon>180.0] -= 360.0
         # grid step size of tide model
         dlon = np.abs(lon[1] - lon[0])
         # replace original values with extend matrices
-        lon = extend_array(lon,dlon)
-        hc = extend_matrix(hc)
+        lon = _extend_array(lon,dlon)
+        hc = _extend_matrix(hc)
         # interpolate amplitude and phase of the constituent
         if (kwargs['method'] == 'bilinear'):
             # replace invalid values with nan
             hc[hc.mask] = np.nan
             # use quick bilinear to interpolate values
             hci = pyTMD.interpolate.bilinear(lon, lat, hc, ilon, ilat,
                 dtype=hc.dtype)
@@ -321,16 +321,16 @@
                 compressed=kwargs['compressed'])
         elif (kwargs['grid'] == 'netcdf'):
             hc, lon, lat, cons = read_netcdf_file(model_file,
                 compressed=kwargs['compressed'])
         # grid step size of tide model
         dlon = np.abs(lon[1] - lon[0])
         # replace original values with extend matrices
-        lon = extend_array(lon, dlon)
-        hc = extend_matrix(hc)
+        lon = _extend_array(lon, dlon)
+        hc = _extend_matrix(hc)
         # append extended constituent
         constituents.append(cons, hc)
         # set model coordinates
         setattr(constituents, 'longitude', lon)
         setattr(constituents, 'latitude', lat)
 
     # return the complex form of the model constituents
@@ -478,63 +478,14 @@
     phase.data[phase.data < 0] += 360.0
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
-# PURPOSE: Extend a longitude array
-def extend_array(input_array: np.ndarray, step_size: float):
-    """
-    Extends a longitude array
-
-    Parameters
-    ----------
-    input_array: np.ndarray
-        array to extend
-    step_size: float
-        step size between elements of array
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended array
-    """
-    n = len(input_array)
-    temp = np.zeros((n+3), dtype=input_array.dtype)
-    # extended array [x-1,x0,...,xN,xN+1,xN+2]
-    temp[0] = input_array[0] - step_size
-    temp[1:-2] = input_array[:]
-    temp[-2] = input_array[-1] + step_size
-    temp[-1] = input_array[-1] + 2.0*step_size
-    return temp
-
-# PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix: np.ndarray):
-    """
-    Extends a global matrix
-
-    Parameters
-    ----------
-    input_matrix: np.ndarray
-        matrix to extend
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended matrix
-    """
-    ny, nx = np.shape(input_matrix)
-    temp = np.ma.zeros((ny,nx+3), dtype=input_matrix.dtype)
-    temp[:,0] = input_matrix[:,-1]
-    temp[:,1:-2] = input_matrix[:,:]
-    temp[:,-2] = input_matrix[:,0]
-    temp[:,-1] = input_matrix[:,1]
-    return temp
-
 # PURPOSE: read GOT model grid files
 def read_ascii_file(
         input_file: str | pathlib.Path,
         **kwargs
     ):
     """
     Read Richard Ray's Global Ocean Tide (GOT) model file
@@ -746,7 +697,56 @@
     fileID.software_reference = pyTMD.version.project_name
     fileID.software_version = pyTMD.version.full_version
     # Output NetCDF structure information
     logging.info(str(FILE))
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
+
+# PURPOSE: Extend a longitude array
+def _extend_array(input_array: np.ndarray, step_size: float):
+    """
+    Extends a longitude array
+
+    Parameters
+    ----------
+    input_array: np.ndarray
+        array to extend
+    step_size: float
+        step size between elements of array
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended array
+    """
+    n = len(input_array)
+    temp = np.zeros((n+3), dtype=input_array.dtype)
+    # extended array [x-1,x0,...,xN,xN+1,xN+2]
+    temp[0] = input_array[0] - step_size
+    temp[1:-2] = input_array[:]
+    temp[-2] = input_array[-1] + step_size
+    temp[-1] = input_array[-1] + 2.0*step_size
+    return temp
+
+# PURPOSE: Extend a global matrix
+def _extend_matrix(input_matrix: np.ndarray):
+    """
+    Extends a global matrix
+
+    Parameters
+    ----------
+    input_matrix: np.ndarray
+        matrix to extend
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended matrix
+    """
+    ny, nx = np.shape(input_matrix)
+    temp = np.ma.zeros((ny,nx+3), dtype=input_matrix.dtype)
+    temp[:,0] = input_matrix[:,-1]
+    temp[:,1:-2] = input_matrix[:,:]
+    temp[:,-2] = input_matrix[:,0]
+    temp[:,-1] = input_matrix[:,1]
+    return temp
```

### Comparing `pyTMD-2.1.0/pyTMD/io/OTIS.py` & `pyTMD-2.1.1/pyTMD/io/OTIS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 OTIS.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (02/2024)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 
 Reads OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
@@ -55,14 +55,18 @@
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     crs.py: Coordinate Reference System (CRS) routines
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 02/2024: don't overwrite hu and hv in _interpolate_zeta
+        changed variable for setting global grid flag to is_global
+    Updated 01/2024: construct currents masks differently if not global
+        renamed currents masks and bathymetry interpolation functions
     Updated 12/2023: use new crs class for coordinate reprojection
     Updated 10/2023: fix transport variable entry for TMD3 models
     Updated 09/2023: prevent overwriting ATLAS compact x and y coordinates
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 04/2023: using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
         new function name for converting coordinate reference systems
@@ -182,15 +186,15 @@
     grid: str, default 'OTIS'
         Tide model file type to read
 
             - ``'ATLAS'``: reading a global solution with localized solutions
             - ``'OTIS'``: combined global or local solution
             - ``'TMD3'``: combined global or local netCDF4 solution
     apply_flexure: bool, default False
-        Apply ice flexure scaling factor to height constituents
+        Apply ice flexure scaling factor to height values
 
     Returns
     -------
     amplitude: np.ndarray
         amplitudes of tidal constituents
     phase: np.ndarray
         phases of tidal constituents
@@ -241,77 +245,69 @@
     ilat = np.atleast_1d(np.copy(ilat))
     # run wrapper function to convert coordinate systems of input lat/lon
     x,y = pyTMD.crs().convert(ilon, ilat, EPSG, 'F')
     # grid step size of tide model
     dx = xi[1] - xi[0]
     dy = yi[1] - yi[0]
 
-    # create current masks and bathymetry estimates
-    if (kwargs['type'] != 'z'):
-        mz,mu,mv = Muv(hz)
-        hu,hv = Huv(hz)
-        # invert current masks to be True for invalid points
-        mu = np.logical_not(mu).astype(mu.dtype)
-        mv = np.logical_not(mv).astype(mv.dtype)
-
     # if global: extend limits
-    global_grid = False
+    is_global = False
     # replace original values with extend arrays/matrices
     if np.isclose(xi[-1] - xi[0], 360.0 - dx) & (EPSG == '4326'):
-        xi = extend_array(xi, dx)
+        xi = _extend_array(xi, dx)
         # set global grid flag
-        global_grid = True
+        is_global = True
 
     # adjust longitudinal convention of input latitude and longitude
     # to fit tide model convention
     if (np.min(x) < np.min(xi)) & (EPSG == '4326'):
         x[x < 0] += 360.0
     if (np.max(x) > np.max(xi)) & (EPSG == '4326'):
         x[x > 180] -= 360.0
     # determine if any input points are outside of the model bounds
     invalid = (x < xi.min()) | (x > xi.max()) | (y < yi.min()) | (y > yi.max())
 
     # update masks for each type
     if (kwargs['type'] == 'z'):
         # replace original values with extend matrices
-        if global_grid:
-            hz = extend_matrix(hz)
-            mz = extend_matrix(mz)
+        if is_global:
+            hz = _extend_matrix(hz)
+            mz = _extend_matrix(mz)
         # masks zero values
         mask = (hz == 0) | mz.astype(bool)
         bathymetry = np.ma.array(hz, mask=mask)
     elif kwargs['type'] in ('u','U'):
-        # create current masks and bathymetry estimates
-        mz,mu,mv = Muv(hz)
-        hu,hv = Huv(hz)
+        # interpolate masks and bathymetry to u, v nodes
+        mu,mv = _mask_nodes(hz, is_global=is_global)
+        hu,hv = _interpolate_zeta(hz, is_global=is_global)
         # invert current masks to be True for invalid points
         mu = np.logical_not(mu).astype(mu.dtype)
         # replace original values with extend matrices
-        if global_grid:
-            hu = extend_matrix(hu)
-            mu = extend_matrix(mu)
+        if is_global:
+            hu = _extend_matrix(hu)
+            mu = _extend_matrix(mu)
         # masks zero values
         mask = (hu == 0) | mu.astype(bool)
         bathymetry = np.ma.array(hu, mask=mask)
-        # x coordinates for u transports
+        # x-coordinates for u transports
         xi -= dx/2.0
     elif kwargs['type'] in ('v','V'):
-        # create current masks and bathymetry estimates
-        mz,mu,mv = Muv(hz)
-        hu,hv = Huv(hz)
+        # interpolate masks and bathymetry to u, v nodes
+        mu,mv = _mask_nodes(hz, is_global=is_global)
+        hu,hv = _interpolate_zeta(hz, is_global=is_global)
         # invert current masks to be True for invalid points
         mv = np.logical_not(mv).astype(mv.dtype)
         # replace original values with extend matrices
-        if global_grid:
-            hv = extend_matrix(hv)
-            mv = extend_matrix(mv)
+        if is_global:
+            hv = _extend_matrix(hv)
+            mv = _extend_matrix(mv)
         # masks zero values
         mask = (hv == 0) | mv.astype(bool)
         bathymetry = np.ma.array(hv, mask=mask)
-        # y coordinates for v transports
+        # y-coordinates for v transports
         yi -= dy/2.0
 
     # interpolate bathymetry and mask to output points
     if (kwargs['method'] == 'bilinear'):
         # replace invalid values with nan
         bathymetry.data[bathymetry.mask] = np.nan
         # use quick bilinear to interpolate values
@@ -389,16 +385,16 @@
                 hc = read_netcdf_file(model_file, i, variable='v')
             elif isinstance(model_file,list):
                 u,hc = read_otis_transport(model_file[i], 0)
             else:
                 u,hc = read_otis_transport(model_file, i)
 
         # replace original values with extend matrices
-        if global_grid:
-            hc = extend_matrix(hc)
+        if is_global:
+            hc = _extend_matrix(hc)
         # copy mask to constituent
         hc.mask |= bathymetry.mask
 
         # interpolate amplitude and phase of the constituent
         if (kwargs['method'] == 'bilinear'):
             # replace zero values with nan
             hc.data[(hc==0) | hc.mask] = np.nan
@@ -487,15 +483,15 @@
     grid: str, default 'OTIS'
         Tide model file type to read
 
             - ``'ATLAS'``: reading a global solution with localized solutions
             - ``'OTIS'``: combined global or local solution
             - ``'TMD3'``: combined global or local netCDF4 solution
     apply_flexure: bool, default False
-        Apply ice flexure scaling factor to height constituents
+        Apply ice flexure scaling factor to height values
 
     Returns
     -------
     constituents: obj
         complex form of tide model constituents
     """
     # set default keyword arguments
@@ -523,60 +519,60 @@
     # invert tide mask to be True for invalid points
     mz = np.logical_not(mz).astype(mz.dtype)
     # grid step size of tide model
     dx = xi[1] - xi[0]
     dy = yi[1] - yi[0]
 
     # if global: extend limits
-    global_grid = False
+    is_global = False
     # replace original values with extend arrays/matrices
     if ((xi[-1] - xi[0]) == (360.0 - dx)) & (EPSG == '4326'):
-        xi = extend_array(xi, dx)
+        xi = _extend_array(xi, dx)
         # set global grid flag
-        global_grid = True
+        is_global = True
 
     # update masks for each type
     # save output constituents
     if (kwargs['type'] == 'z'):
         # replace original values with extend matrices
-        if global_grid:
-            hz = extend_matrix(hz)
-            mz = extend_matrix(mz)
+        if is_global:
+            hz = _extend_matrix(hz)
+            mz = _extend_matrix(mz)
         # masks zero values
         mask = (hz == 0) | mz.astype(bool)
         bathymetry = np.ma.array(hz, mask=mask)
     elif kwargs['type'] in ('u','U'):
-        # create current masks and bathymetry estimates
-        mz,mu,mv = Muv(hz)
-        hu,hv = Huv(hz)
+        # interpolate masks and bathymetry to u, v nodes
+        mu,mv = _mask_nodes(hz, is_global=is_global)
+        hu,hv = _interpolate_zeta(hz, is_global=is_global)
         # invert current masks to be True for invalid points
         mu = np.logical_not(mu).astype(mu.dtype)
         # replace original values with extend matrices
-        if global_grid:
-            hu = extend_matrix(hu)
-            mu = extend_matrix(mu)
+        if is_global:
+            hu = _extend_matrix(hu)
+            mu = _extend_matrix(mu)
         # masks zero values
         mask = (hu == 0) | mu.astype(bool)
         bathymetry = np.ma.array(hu, mask=mask)
-        # x coordinates for u transports
+        # x-coordinates for u transports
         xi -= dx/2.0
     elif kwargs['type'] in ('v','V'):
-        # create current masks and bathymetry estimates
-        mz,mu,mv = Muv(hz)
-        hu,hv = Huv(hz)
+        # interpolate masks and bathymetry to u, v nodes
+        mu,mv = _mask_nodes(hz, is_global=is_global)
+        hu,hv = _interpolate_zeta(hz, is_global=is_global)
         # invert current masks to be True for invalid points
         mv = np.logical_not(mv).astype(mv.dtype)
         # replace original values with extend matrices
-        if global_grid:
-            hv = extend_matrix(hv)
-            mv = extend_matrix(mv)
+        if is_global:
+            hv = _extend_matrix(hv)
+            mv = _extend_matrix(mv)
         # masks zero values
         mask = (hv == 0) | mv.astype(bool)
         bathymetry = np.ma.array(hv, mask=mask)
-        # y coordinates for v transports
+        # y-coordinates for v transports
         yi -= dy/2.0
 
     # read each constituent
     if isinstance(model_file, list):
         cons = [read_constituents(m)[0].pop() for m in model_file]
     else:
         cons,_ = read_constituents(model_file, grid=kwargs['grid'])
@@ -623,16 +619,16 @@
                 hc = read_netcdf_file(model_file, i, variable='v')
             elif isinstance(model_file,list):
                 u,hc = read_otis_transport(model_file[i], 0)
             else:
                 u,hc = read_otis_transport(model_file, i)
 
         # replace original values with extend matrices
-        if global_grid:
-            hc = extend_matrix(hc)
+        if is_global:
+            hc = _extend_matrix(hc)
         # copy mask to constituent
         hc.mask |= bathymetry.mask
         # append extended constituent
         constituents.append(c, hc)
 
     # return the complex form of the model constituents
     return constituents
@@ -812,61 +808,14 @@
     phase.data[phase.data < 0] += 360.0
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, D)
 
-# PURPOSE: Extend a longitude array
-def extend_array(input_array: np.ndarray, step_size: float):
-    """
-    Extends a longitude array
-
-    Parameters
-    ----------
-    input_array: np.ndarray
-        array to extend
-    step_size: float
-        step size between elements of array
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended array
-    """
-    n = len(input_array)
-    temp = np.zeros((n+2), dtype=input_array.dtype)
-    # extended array [x-1,x0,...,xN,xN+1]
-    temp[0] = input_array[0] - step_size
-    temp[1:-1] = input_array[:]
-    temp[-1] = input_array[-1] + step_size
-    return temp
-
-# PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix: np.ndarray):
-    """
-    Extends a global matrix
-
-    Parameters
-    ----------
-    input_matrix: np.ndarray
-        matrix to extend
-
-    Returns
-    -------
-    temp: np.ndarray
-        extended matrix
-    """
-    ny, nx = np.shape(input_matrix)
-    temp = np.ma.zeros((ny, nx+2), dtype=input_matrix.dtype)
-    temp[:,0] = input_matrix[:,-1]
-    temp[:,1:-1] = input_matrix[:,:]
-    temp[:,-1] = input_matrix[:,0]
-    return temp
-
 # PURPOSE: read tide grid file
 def read_otis_grid(input_file: str | pathlib.Path):
     """
     Read grid file to extract model coordinates, bathymetry, masks and indices
 
     Parameters
     ----------
@@ -1482,16 +1431,16 @@
     y30: np.ndarray
         y-coordinates of high-resolution tide model
     m30: np.ndarray
         high-resolution land/water mask
     """
     # create 2 arc-minute grid dimensions
     d30 = 1.0/30.0
-    x30 = np.arange(d30/2.0, 360.0+d30/2.0, d30)
-    y30 = np.arange(-90.0+d30/2.0, 90.0+d30/2.0, d30)
+    x30 = np.arange(d30/2.0, 360.0 + d30/2.0, d30)
+    y30 = np.arange(-90.0 + d30/2.0, 90.0 + d30/2.0, d30)
     # interpolate global mask to create initial 2 arc-minute mask
     xcoords=np.clip((len(xi)-1)*(x30-xi[0])/(xi[-1]-xi[0]),0,len(xi)-1)
     ycoords=np.clip((len(yi)-1)*(y30-yi[0])/(yi[-1]-yi[0]),0,len(yi)-1)
     IY,IX = np.meshgrid(np.around(ycoords), np.around(xcoords), indexing='ij')
     # interpolate with nearest-neighbors
     m30 = np.ma.zeros((len(y30),len(x30)), dtype=np.int8,fill_value=0)
     m30.data[:,:] = mz[IY.astype(np.int32), IX.astype(np.int32)]
@@ -1548,16 +1497,16 @@
         x-coordinates of high-resolution tide model
     ys: np.ndarray
         y-coordinates of high-resolution tide model
     zs: np.ndarray
         high-resolution tidal solution for variable
     """
     # create resampled grid dimensions
-    xs = np.arange(spacing/2.0, 360.0+spacing/2.0, spacing)
-    ys = np.arange(-90.0+spacing/2.0, 90.0+spacing/2.0, spacing)
+    xs = np.arange(spacing/2.0, 360.0 + spacing/2.0, spacing)
+    ys = np.arange(-90.0 + spacing/2.0, 90.0 + spacing/2.0, spacing)
     # interpolate global solution
     zs = np.ma.zeros((len(ys),len(xs)), dtype=zi.dtype)
     zs.mask = np.zeros((len(ys),len(xs)), dtype=bool)
     # test if combining elevation/transport variables with complex components
     if np.iscomplexobj(zs):
         f1 = scipy.interpolate.RectBivariateSpline(xi, yi, zi.real.T, kx=1,ky=1)
         f2 = scipy.interpolate.RectBivariateSpline(xi, yi, zi.imag.T, kx=1,ky=1)
@@ -1869,49 +1818,127 @@
             temp[2:4*nx-1:4] = v.real[m,:,ic]
             temp[3:4*nx:4] = v.imag[m,:,ic]
             temp.tofile(fid,format='>f4')
         fid.write(struct.pack('>i',constituent_header))
     # close the output OTIS file
     fid.close()
 
-# For a rectangular bathymetry grid:
-# construct masks for zeta, u and v nodes on a C-grid
-def Muv(hz: np.ndarray):
+# PURPOSE: Extend a longitude array
+def _extend_array(input_array: np.ndarray, step_size: float):
     """
-    Construct masks for zeta, u and v nodes on a C-grid
+    Extends a longitude array
+
+    Parameters
+    ----------
+    input_array: np.ndarray
+        array to extend
+    step_size: float
+        step size between elements of array
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended array
     """
-    ny, nx = np.shape(hz)
+    n = len(input_array)
+    temp = np.zeros((n+2), dtype=input_array.dtype)
+    # extended array [x-1,x0,...,xN,xN+1]
+    temp[0] = input_array[0] - step_size
+    temp[1:-1] = input_array[:]
+    temp[-1] = input_array[-1] + step_size
+    return temp
+
+# PURPOSE: Extend a global matrix
+def _extend_matrix(input_matrix: np.ndarray):
+    """
+    Extends a global matrix
+
+    Parameters
+    ----------
+    input_matrix: np.ndarray
+        matrix to extend
+
+    Returns
+    -------
+    temp: np.ndarray
+        extended matrix
+    """
+    ny, nx = np.shape(input_matrix)
+    temp = np.ma.zeros((ny, nx+2), dtype=input_matrix.dtype)
+    temp[:,0] = input_matrix[:,-1]
+    temp[:,1:-1] = input_matrix[:,:]
+    temp[:,-1] = input_matrix[:,0]
+    return temp
+
+# PURPOSE: construct masks for u and v nodes
+def _mask_nodes(hz: np.ndarray, is_global: bool = True):
+    """
+    Construct masks for u and v nodes on a C-grid
+
+    Parameters
+    ----------
+    hz: np.ndarray
+        bathymetry of grid centers
+    is_global: bool, default True
+        input grid is global in terms of longitude
+    """
+    # for grid center mask: find where bathymetry is greater than 0
     mz = (hz > 0).astype(int)
-    # x-indices
-    indx = np.zeros((nx), dtype=int)
-    indx[:-1] = np.arange(1,nx)
-    indx[-1] = 0
-    # y-indices
-    indy = np.zeros((ny), dtype=int)
-    indy[:-1] = np.arange(1,ny)
-    indy[-1] = 0
-    # calculate mu and mv
+    mu, mv = _interpolate_mask(mz, is_global=is_global)
+    # return the masks
+    return (mu, mv)
+
+# PURPOSE: interpolate mask to u and v nodes
+def _interpolate_mask(mz: np.ndarray, is_global: bool = True):
+    """
+    Interpolate mask from zeta nodes to u and v nodes on a C-grid
+
+    Parameters
+    ----------
+    mz: np.ndarray
+        mask at grid centers
+    is_global: bool, default True
+        input grid is global in terms of longitude
+    """
+    # shape of input mask
+    ny, nx = np.shape(mz)
+    # initialize integer masks for u and v grids
     mu = np.zeros((ny, nx), dtype=int)
     mv = np.zeros((ny, nx), dtype=int)
-    mu[indy,:] = mz*mz[indy,:]
-    mv[:,indx] = mz*mz[:,indx]
-    return (mu, mv, mz)
+    # wrap mask if global
+    mode = 'wrap' if is_global else 'edge'
+    # calculate masks on u and v grids
+    tmp = np.pad(mz, ((0, 0), (1, 0)), mode=mode)
+    mu[:,:] = (tmp[:,:-1]*tmp[:,1:])
+    tmp = np.pad(mz, ((1, 0), (0, 0)), mode='edge')
+    mv[:,:] = (tmp[:-1,:]*tmp[1:,:])
+    # return the masks
+    return (mu, mv)
 
-# PURPOSE: Interpolate bathymetry to zeta, u and v nodes on a C-grid
-def Huv(hz: np.ndarray):
+# PURPOSE: interpolate data to u and v nodes
+def _interpolate_zeta(hz: np.ndarray, is_global: bool = True):
     """
-    Interpolate bathymetry to zeta, u and v nodes on a C-grid
+    Interpolate data from zeta nodes to u and v nodes on a C-grid
+
+    Parameters
+    ----------
+    hz: np.ndarray
+        data at grid centers
+    is_global: bool, default True
+        input grid is global in terms of longitude
     """
+    # shape of input data
     ny, nx = np.shape(hz)
-    mu, mv, mz = Muv(hz)
-    # x-indices
-    indx = np.zeros((nx), dtype=int)
-    indx[0] = nx-1
-    indx[1:] = np.arange(1, nx)
-    # y-indices
-    indy = np.zeros((ny), dtype=int)
-    indy[0] = ny-1
-    indy[1:] = np.arange(1,ny)
-    # calculate hu and hv
-    hu = mu*(hz + hz[indy,:])/2.0
-    hv = mv*(hz + hz[:,indx])/2.0
+    # get masks for u and v nodes
+    mu, mv = _mask_nodes(hz)
+    # initialize data for u and v grids
+    hu = np.zeros((ny, nx), dtype=hz.dtype)
+    hv = np.zeros((ny, nx), dtype=hz.dtype)
+    # wrap data if global
+    mode = 'wrap' if is_global else 'edge'
+    # calculate data at u and v nodes
+    tmp = np.pad(hz, ((0, 0), (1, 0)), mode=mode)
+    hu[:,:] = 0.5*mu*(tmp[:,:-1] + tmp[:,1:])
+    tmp = np.pad(hz, ((1, 0), (0, 0)), mode='edge')
+    hv[:,:] = 0.5*mv*(tmp[:-1,:] + tmp[1:,:])
+    # return the interpolated data values
     return (hu, hv)
```

### Comparing `pyTMD-2.1.0/pyTMD/io/constituents.py` & `pyTMD-2.1.1/pyTMD/io/constituents.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/io/model.py` & `pyTMD-2.1.1/pyTMD/io/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 u"""
 model.py
-Written by Tyler Sutterley (11/2023)
+Written by Tyler Sutterley (04/2024)
 Retrieves tide model parameters for named tide models and
     from model definition files
 
 UPDATE HISTORY:
+    Updated 04/2024: append v-components of velocity only to netcdf format
     Updated 11/2023: revert TPXO9-atlas currents changes to separate dicts
     Updated 09/2023: fix scale values for TPXO9-atlas currents
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
         updated filenames for CATS2008-v2023 to final version
     Updated 06/2023: remap FES2012 e2 constituent to eps2
     Updated 04/2023: added global HAMTIDE11 model
         made ICESat, ICESat-2 and output file attributes properties
@@ -722,20 +723,24 @@
             model_files = {}
             model_files['u'] = ['u_q1_tpxo9_atlas_30','u_o1_tpxo9_atlas_30',
                 'u_p1_tpxo9_atlas_30','u_k1_tpxo9_atlas_30',
                 'u_n2_tpxo9_atlas_30','u_m2_tpxo9_atlas_30',
                 'u_s2_tpxo9_atlas_30','u_k2_tpxo9_atlas_30',
                 'u_m4_tpxo9_atlas_30','u_ms4_tpxo9_atlas_30',
                 'u_mn4_tpxo9_atlas_30','u_2n2_tpxo9_atlas_30']
-            model_files['v'] = ['v_q1_tpxo9_atlas_30','v_o1_tpxo9_atlas_30',
-                'v_p1_tpxo9_atlas_30','v_k1_tpxo9_atlas_30',
-                'v_n2_tpxo9_atlas_30','v_m2_tpxo9_atlas_30',
-                'v_s2_tpxo9_atlas_30','v_k2_tpxo9_atlas_30',
-                'v_m4_tpxo9_atlas_30','v_ms4_tpxo9_atlas_30',
-                'v_mn4_tpxo9_atlas_30','v_2n2_tpxo9_atlas_30']
+            # add v-component if format is netcdf
+            if (self.format == 'netcdf'):
+                model_files['v'] = ['v_q1_tpxo9_atlas_30',
+                    'v_o1_tpxo9_atlas_30','v_p1_tpxo9_atlas_30',
+                    'v_k1_tpxo9_atlas_30','v_n2_tpxo9_atlas_30',
+                    'v_m2_tpxo9_atlas_30','v_s2_tpxo9_atlas_30',
+                    'v_k2_tpxo9_atlas_30','v_m4_tpxo9_atlas_30',
+                    'v_ms4_tpxo9_atlas_30','v_mn4_tpxo9_atlas_30',
+                    'v_2n2_tpxo9_atlas_30']
+            # build model file dictionary
             self.model_file = {}
             for key,val in model_files.items():
                 self.model_file[key] = self.pathfinder(val)
             self.projection = '4326'
             self.scale = 1e-4
             self.version = 'v1'
             # model description and references
@@ -747,20 +752,24 @@
             model_files = {}
             model_files['u'] = ['u_q1_tpxo9_atlas_30_v2','u_o1_tpxo9_atlas_30_v2',
                 'u_p1_tpxo9_atlas_30_v2','u_k1_tpxo9_atlas_30_v2',
                 'u_n2_tpxo9_atlas_30_v2','u_m2_tpxo9_atlas_30_v2',
                 'u_s2_tpxo9_atlas_30_v2','u_k2_tpxo9_atlas_30_v2',
                 'u_m4_tpxo9_atlas_30_v2','u_ms4_tpxo9_atlas_30_v2',
                 'u_mn4_tpxo9_atlas_30_v2','u_2n2_tpxo9_atlas_30_v2']
-            model_files['v'] = ['v_q1_tpxo9_atlas_30_v2','v_o1_tpxo9_atlas_30_v2',
-                'v_p1_tpxo9_atlas_30_v2','v_k1_tpxo9_atlas_30_v2',
-                'v_n2_tpxo9_atlas_30_v2','v_m2_tpxo9_atlas_30_v2',
-                'v_s2_tpxo9_atlas_30_v2','v_k2_tpxo9_atlas_30_v2',
-                'v_m4_tpxo9_atlas_30_v2','v_ms4_tpxo9_atlas_30_v2',
-                'v_mn4_tpxo9_atlas_30_v2','v_2n2_tpxo9_atlas_30_v2']
+            # add v-component if format is netcdf
+            if (self.format == 'netcdf'):
+                model_files['v'] = ['v_q1_tpxo9_atlas_30_v2',
+                    'v_o1_tpxo9_atlas_30_v2','v_p1_tpxo9_atlas_30_v2',
+                    'v_k1_tpxo9_atlas_30_v2','v_n2_tpxo9_atlas_30_v2',
+                    'v_m2_tpxo9_atlas_30_v2','v_s2_tpxo9_atlas_30_v2',
+                    'v_k2_tpxo9_atlas_30_v2','v_m4_tpxo9_atlas_30_v2',
+                    'v_ms4_tpxo9_atlas_30_v2','v_mn4_tpxo9_atlas_30_v2',
+                    'v_2n2_tpxo9_atlas_30_v2']
+            # build model file dictionary
             self.model_file = {}
             for key,val in model_files.items():
                 self.model_file[key] = self.pathfinder(val)
             self.projection = '4326'
             self.scale = 1e-4
             self.version = 'v2'
             # model description and references
@@ -772,21 +781,25 @@
             model_files['u'] = ['u_q1_tpxo9_atlas_30_v3','u_o1_tpxo9_atlas_30_v3',
                 'u_p1_tpxo9_atlas_30_v3','u_k1_tpxo9_atlas_30_v3',
                 'u_n2_tpxo9_atlas_30_v3','u_m2_tpxo9_atlas_30_v3',
                 'u_s2_tpxo9_atlas_30_v3','u_k2_tpxo9_atlas_30_v3',
                 'u_m4_tpxo9_atlas_30_v3','u_ms4_tpxo9_atlas_30_v3',
                 'u_mn4_tpxo9_atlas_30_v3','u_2n2_tpxo9_atlas_30_v3',
                 'u_mf_tpxo9_atlas_30_v3','u_mm_tpxo9_atlas_30_v3']
-            model_files['v'] = ['v_q1_tpxo9_atlas_30_v3','v_o1_tpxo9_atlas_30_v3',
-                'v_p1_tpxo9_atlas_30_v3','v_k1_tpxo9_atlas_30_v3',
-                'v_n2_tpxo9_atlas_30_v3','v_m2_tpxo9_atlas_30_v3',
-                'v_s2_tpxo9_atlas_30_v3','v_k2_tpxo9_atlas_30_v3',
-                'v_m4_tpxo9_atlas_30_v3','v_ms4_tpxo9_atlas_30_v3',
-                'v_mn4_tpxo9_atlas_30_v3','v_2n2_tpxo9_atlas_30_v3',
-                'v_mf_tpxo9_atlas_30_v3','v_mm_tpxo9_atlas_30_v3']
+            # add v-component if format is netcdf
+            if (self.format == 'netcdf'):
+                model_files['v'] = ['v_q1_tpxo9_atlas_30_v3',
+                    'v_o1_tpxo9_atlas_30_v3','v_p1_tpxo9_atlas_30_v3',
+                    'v_k1_tpxo9_atlas_30_v3','v_n2_tpxo9_atlas_30_v3',
+                    'v_m2_tpxo9_atlas_30_v3','v_s2_tpxo9_atlas_30_v3',
+                    'v_k2_tpxo9_atlas_30_v3','v_m4_tpxo9_atlas_30_v3',
+                    'v_ms4_tpxo9_atlas_30_v3','v_mn4_tpxo9_atlas_30_v3',
+                    'v_2n2_tpxo9_atlas_30_v3','v_mf_tpxo9_atlas_30_v3',
+                    'v_mm_tpxo9_atlas_30_v3']
+            # build model file dictionary
             self.model_file = {}
             for key,val in model_files.items():
                 self.model_file[key] = self.pathfinder(val)
             self.projection = '4326'
             self.scale = 1e-4
             self.version = 'v3'
             # model description and references
@@ -798,21 +811,25 @@
             model_files['u'] = ['u_q1_tpxo9_atlas_30_v4','u_o1_tpxo9_atlas_30_v4',
                 'u_p1_tpxo9_atlas_30_v4','u_k1_tpxo9_atlas_30_v4',
                 'u_n2_tpxo9_atlas_30_v4','u_m2_tpxo9_atlas_30_v4',
                 'u_s2_tpxo9_atlas_30_v4','u_k2_tpxo9_atlas_30_v4',
                 'u_m4_tpxo9_atlas_30_v4','u_ms4_tpxo9_atlas_30_v4',
                 'u_mn4_tpxo9_atlas_30_v4','u_2n2_tpxo9_atlas_30_v4',
                 'u_mf_tpxo9_atlas_30_v4','u_mm_tpxo9_atlas_30_v4']
-            model_files['v'] = ['v_q1_tpxo9_atlas_30_v4','v_o1_tpxo9_atlas_30_v4',
-                'v_p1_tpxo9_atlas_30_v4','v_k1_tpxo9_atlas_30_v4',
-                'v_n2_tpxo9_atlas_30_v4','v_m2_tpxo9_atlas_30_v4',
-                'v_s2_tpxo9_atlas_30_v4','v_k2_tpxo9_atlas_30_v4',
-                'v_m4_tpxo9_atlas_30_v4','v_ms4_tpxo9_atlas_30_v4',
-                'v_mn4_tpxo9_atlas_30_v4','v_2n2_tpxo9_atlas_30_v4',
-                'v_mf_tpxo9_atlas_30_v4','v_mm_tpxo9_atlas_30_v4']
+            # add v-component if format is netcdf
+            if (self.format == 'netcdf'):
+                model_files['v'] = ['v_q1_tpxo9_atlas_30_v4',
+                    'v_o1_tpxo9_atlas_30_v4','v_p1_tpxo9_atlas_30_v4',
+                    'v_k1_tpxo9_atlas_30_v4','v_n2_tpxo9_atlas_30_v4',
+                    'v_m2_tpxo9_atlas_30_v4','v_s2_tpxo9_atlas_30_v4',
+                    'v_k2_tpxo9_atlas_30_v4','v_m4_tpxo9_atlas_30_v4',
+                    'v_ms4_tpxo9_atlas_30_v4','v_mn4_tpxo9_atlas_30_v4',
+                    'v_2n2_tpxo9_atlas_30_v4','v_mf_tpxo9_atlas_30_v4',
+                    'v_mm_tpxo9_atlas_30_v4']
+            # build model file dictionary
             self.model_file = {}
             for key,val in model_files.items():
                 self.model_file[key] = self.pathfinder(val)
             self.projection = '4326'
             self.scale = 1e-4
             self.version = 'v4'
             # model description and references
@@ -825,22 +842,25 @@
                 'u_p1_tpxo9_atlas_30_v5','u_k1_tpxo9_atlas_30_v5',
                 'u_n2_tpxo9_atlas_30_v5','u_m2_tpxo9_atlas_30_v5',
                 'u_s1_tpxo9_atlas_30_v5','u_s2_tpxo9_atlas_30_v5',
                 'u_k2_tpxo9_atlas_30_v5','u_m4_tpxo9_atlas_30_v5',
                 'u_ms4_tpxo9_atlas_30_v5','u_mn4_tpxo9_atlas_30_v5',
                 'u_2n2_tpxo9_atlas_30_v5','u_mf_tpxo9_atlas_30_v5',
                 'u_mm_tpxo9_atlas_30_v5']
-            model_files['v'] = ['v_q1_tpxo9_atlas_30_v5','v_o1_tpxo9_atlas_30_v5',
-                'v_p1_tpxo9_atlas_30_v5','v_k1_tpxo9_atlas_30_v5',
-                'v_n2_tpxo9_atlas_30_v5','v_m2_tpxo9_atlas_30_v5',
-                'v_s1_tpxo9_atlas_30_v5','v_s2_tpxo9_atlas_30_v5',
-                'v_k2_tpxo9_atlas_30_v5','v_m4_tpxo9_atlas_30_v5',
-                'v_ms4_tpxo9_atlas_30_v5','v_mn4_tpxo9_atlas_30_v5',
-                'v_2n2_tpxo9_atlas_30_v5','v_mf_tpxo9_atlas_30_v5',
-                'v_mm_tpxo9_atlas_30_v5']
+            # add v-component if format is netcdf
+            if (self.format == 'netcdf'):
+                model_files['v'] = ['u_q1_tpxo9_atlas_30_v5',
+                    'u_o1_tpxo9_atlas_30_v5','u_p1_tpxo9_atlas_30_v5',
+                    'u_k1_tpxo9_atlas_30_v5','u_n2_tpxo9_atlas_30_v5',
+                    'u_m2_tpxo9_atlas_30_v5','u_s1_tpxo9_atlas_30_v5',
+                    'u_s2_tpxo9_atlas_30_v5','u_k2_tpxo9_atlas_30_v5',
+                    'u_m4_tpxo9_atlas_30_v5','u_ms4_tpxo9_atlas_30_v5',
+                    'u_mn4_tpxo9_atlas_30_v5','u_2n2_tpxo9_atlas_30_v5',
+                    'u_mf_tpxo9_atlas_30_v5','u_mm_tpxo9_atlas_30_v5']
+            # build model file dictionary
             self.model_file = {}
             for key,val in model_files.items():
                 self.model_file[key] = self.pathfinder(val)
             self.projection = '4326'
             self.scale = 1e-4
             self.version = 'v5'
             # model description and references
```

### Comparing `pyTMD-2.1.0/pyTMD/io/ocean_pole_tide.py` & `pyTMD-2.1.1/pyTMD/io/ocean_pole_tide.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,23 +125,23 @@
         ilon = int(ln/dlon)
         ilat = int((90.0-lt)/dlat)
         ur[ilon,ilat] = urr + 1j*uri
         un[ilon,ilat] = unr + 1j*uni
         ue[ilon,ilat] = uer + 1j*uei
 
     # extend matrix for bilinear interpolation
-    glon = extend_array(glon,dlon)
-    ur = extend_matrix(ur)
-    un = extend_matrix(un)
-    ue = extend_matrix(ue)
+    glon = _extend_array(glon,dlon)
+    ur = _extend_matrix(ur)
+    un = _extend_matrix(un)
+    ue = _extend_matrix(ue)
     # return values
     return (ur, un, ue, glon, glat)
 
 # PURPOSE: Extend a longitude array
-def extend_array(input_array: np.ndarray, step_size: float):
+def _extend_array(input_array: np.ndarray, step_size: float):
     """
     Extends a longitude array
 
     Parameters
     ----------
     input_array: np.ndarray
         array to extend
@@ -158,15 +158,15 @@
     # extended array [x-1,x0,...,xN,xN+1]
     temp[0] = input_array[0] - step_size
     temp[1:-1] = input_array[:]
     temp[-1] = input_array[-1] + step_size
     return temp
 
 # PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix: np.ndarray):
+def _extend_matrix(input_matrix: np.ndarray):
     """
     Extends a global matrix
 
     Parameters
     ----------
     input_matrix: np.ndarray
         matrix to extend
```

### Comparing `pyTMD-2.1.0/pyTMD/load_constituent.py` & `pyTMD-2.1.1/pyTMD/load_constituent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 u"""
-load_constituent.py (09/2023)
+load_constituent.py (01/2024)
 Loads parameters for a given tidal constituent
 
 CALLING SEQUENCE:
     amplitude,phase,omega,alpha,species = load_constituent(c)
 
 INPUTS:
     c: tidal constituent ID
@@ -22,21 +22,22 @@
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 UPDATE HISTORY:
+    Updated 01/2024: moved constituent parameters function to arguments
     Updated 09/2023: deprecated in favor of pyTMD.predict function
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 07/2020: add more constituents from OTPSnc and function docstrings
     Updated 09/2017: Rewritten in Python
 """
 import warnings
-import pyTMD.predict
+import pyTMD.arguments
 
 def load_constituent(c):
     """
     Loads parameters for a given tidal constituent
 
     Parameters
     ----------
@@ -62,11 +63,11 @@
         Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
         Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
     # raise warning for deprecated function call
-    warnings.warn("Deprecated. Please use pyTMD.predict instead",
+    warnings.warn("Deprecated. Please use pyTMD.arguments instead",
         DeprecationWarning)
     # call updated function to not break current workflows
-    return pyTMD.predict._constituent_parameters(c)
+    return pyTMD.arguments._constituent_parameters(c)
```

### Comparing `pyTMD-2.1.0/pyTMD/load_nodal_corrections.py` & `pyTMD-2.1.1/pyTMD/load_nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/predict.py` & `pyTMD-2.1.1/pyTMD/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 u"""
 predict.py
-Written by Tyler Sutterley (01/2024)
+Written by Tyler Sutterley (02/2024)
 Prediction routines for ocean, load, equilibrium and solid earth tides
 
 REFERENCES:
     G. D. Egbert and S. Erofeeva, "Efficient Inverse Modeling of Barotropic
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 PROGRAM DEPENDENCIES:
     arguments.py: loads nodal corrections for tidal constituents
     astro.py: computes the basic astronomical mean longitudes
-    constants.py: calculate reference parameters for common ellipsoids
+    crs.py: Coordinate Reference System (CRS) routines
     spatial.py: utilities for working with geospatial data
 
 UPDATE HISTORY:
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
     Updated 01/2024: moved minor arguments calculation into new function
+        moved constituent parameters function from predict to arguments
     Updated 12/2023: phase_angles function renamed to doodson_arguments
     Updated 09/2023: moved constituent parameters function within this module
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 04/2023: using renamed astro mean_longitudes function
         using renamed arguments function for nodal corrections
         adding prediction routine for solid earth tides
         output solid earth tide corrections as combined XYZ components
@@ -43,15 +45,15 @@
     Updated 09/2017: Rewritten in Python
 """
 from __future__ import annotations
 
 import numpy as np
 import pyTMD.arguments
 import pyTMD.astro
-from pyTMD.constants import constants
+from pyTMD.crs import datum
 
 # PURPOSE: Predict tides at single times
 def map(t: float | np.ndarray,
         hc: np.ndarray,
         constituents: list | np.ndarray,
         deltat: float | np.ndarray = 0.0,
         corrections: str = 'OTIS'
@@ -98,15 +100,16 @@
     # allocate for output tidal elevation
     ht = np.ma.zeros((npts))
     ht.mask = np.zeros((npts), dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS', 'ATLAS', 'TMD3', 'netcdf'):
             # load parameters for each constituent
-            amp, ph, omega, alpha, species = _constituent_parameters(c)
+            amp, ph, omega, alpha, species = \
+                pyTMD.arguments._constituent_parameters(c)
             # add component for constituent to output tidal elevation
             th = omega*t*86400.0 + ph + pu[0,k]
         elif corrections in ('GOT', 'FES'):
             th = G[0,k]*np.pi/180.0 + pu[0,k]
         # sum over all tides
         ht.data[:] += pf[0,k]*hc.real[:,k]*np.cos(th) - \
             pf[0,k]*hc.imag[:,k]*np.sin(th)
@@ -163,15 +166,16 @@
     # allocate for output time series
     ht = np.ma.zeros((nt))
     ht.mask = np.zeros((nt), dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS', 'ATLAS', 'TMD3', 'netcdf'):
             # load parameters for each constituent
-            amp, ph, omega, alpha, species = _constituent_parameters(c)
+            amp, ph, omega, alpha, species = \
+                pyTMD.arguments._constituent_parameters(c)
             # add component for constituent to output tidal elevation
             th = omega*t*86400.0 + ph + pu[:,k]
         elif corrections in ('GOT', 'FES'):
             th = G[:,k]*np.pi/180.0 + pu[:,k]
         # sum over all tides
         ht.data[:] += pf[:,k]*hc.real[:,k]*np.cos(th) - \
             pf[:,k]*hc.imag[:,k]*np.sin(th)
@@ -228,15 +232,16 @@
     # allocate for output time series
     ht = np.ma.zeros((nt))
     ht.mask = np.zeros((nt), dtype=bool)
     # for each constituent
     for k,c in enumerate(constituents):
         if corrections in ('OTIS', 'ATLAS', 'TMD3', 'netcdf'):
             # load parameters for each constituent
-            amp, ph, omega, alpha, species = _constituent_parameters(c)
+            amp, ph, omega, alpha, species = \
+                pyTMD.arguments._constituent_parameters(c)
             # add component for constituent to output tidal time series
             th = omega*t*86400.0 + ph + pu[:,k]
         elif corrections in ('GOT', 'FES'):
             th = G[:,k]*np.pi/180.0 + pu[:,k]
         # sum over all tides at location
         ht.data[:] += pf[:,k]*hc.real[0,k]*np.cos(th) - \
             pf[:,k]*hc.imag[0,k]*np.sin(th)
@@ -450,15 +455,15 @@
         lpet = gamma_2*np.sqrt((4.0+1.0)/(4.0*np.pi))*np.outer(P20,Z/100.0)
     else:
         lpet = gamma_2*np.sqrt((4.0+1.0)/(4.0*np.pi))*P20*(Z/100.0)
     # return the long-period equilibrium tides
     return lpet
 
 # get IERS parameters
-_iers = constants(ellipsoid='IERS', units='MKS')
+_iers = datum(ellipsoid='IERS', units='MKS')
 
 # PURPOSE: estimate solid Earth tides due to gravitational attraction
 def solid_earth_tide(
         t: np.ndarray,
         XYZ: np.ndarray,
         SXYZ: np.ndarray,
         LXYZ: np.ndarray,
@@ -578,99 +583,14 @@
     dxt += _frequency_dependence_long_period(XYZ, MJD)
     # convert the permanent tide system if specified
     if (tide_system.lower() == 'mean_tide'):
         dxt += _free_to_mean(XYZ, h2, l2)
     # return the solid earth tide
     return dxt
 
-def _constituent_parameters(c):
-    """
-    Loads parameters for a given tidal constituent
-
-    Parameters
-    ----------
-    c: list
-        tidal constituent ID
-
-    Returns
-    -------
-    amplitude: float
-        amplitude of equilibrium tide for tidal constituent (meters)
-    phase: float
-        phase of tidal constituent (radians)
-    omega: float
-        angular frequency of constituent (radians)
-    alpha: float
-        load love number of tidal constituent
-    species: float
-        spherical harmonic dependence of quadrupole potential
-
-    References
-    ----------
-    .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
-        Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
-        Technology*, 19(2), 183--204, (2002).
-        `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
-
-    .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
-    """
-    # constituents array that are included in tidal program
-    cindex = ['m2', 's2', 'k1', 'o1', 'n2', 'p1', 'k2', 'q1', '2n2', 'mu2',
-        'nu2', 'l2', 't2', 'j1', 'm1', 'oo1', 'rho1', 'mf', 'mm', 'ssa',
-        'm4', 'ms4', 'mn4', 'm6', 'm8', 'mk3', 's6', '2sm2', '2mk3']
-    # species type (spherical harmonic dependence of quadrupole potential)
-    _species = np.array([2, 2, 1, 1, 2, 1, 2, 1, 2, 2, 2, 2, 2, 1, 1,
-        1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
-    # Load Love numbers
-    # alpha = correction factor for first order load tides
-    _alpha = np.array([0.693, 0.693, 0.736, 0.695, 0.693, 0.706, 0.693,
-        0.695, 0.693, 0.693, 0.693, 0.693, 0.693, 0.695, 0.695, 0.695, 0.695,
-        0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693, 0.693,
-        0.693, 0.693])
-    # omega: angular frequency of constituent, in radians
-    _omega = np.array([1.405189e-04, 1.454441e-04, 7.292117e-05, 6.759774e-05,
-        1.378797e-04, 7.252295e-05, 1.458423e-04, 6.495854e-05, 1.352405e-04,
-        1.355937e-04, 1.382329e-04, 1.431581e-04, 1.452450e-04, 7.556036e-05,
-        7.028195e-05, 7.824458e-05, 6.531174e-05, 0.053234e-04, 0.026392e-04,
-        0.003982e-04, 2.810377e-04, 2.859630e-04, 2.783984e-04, 4.215566e-04,
-        5.620755e-04, 2.134402e-04, 4.363323e-04, 1.503693e-04, 2.081166e-04])
-    # Astronomical arguments (relative to t0 = 1 Jan 0:00 1992)
-    # phases for each constituent are referred to the time when the phase of
-    # the forcing for that constituent is zero on the Greenwich meridian
-    _phase = np.array([1.731557546, 0.000000000, 0.173003674, 1.558553872,
-        6.050721243, 6.110181633, 3.487600001, 5.877717569, 4.086699633,
-        3.463115091, 5.427136701, 0.553986502, 0.052841931, 2.137025284,
-        2.436575100, 1.929046130, 5.254133027, 1.756042456, 1.964021610,
-        3.487600001, 3.463115091, 1.731557546, 1.499093481, 5.194672637,
-        6.926230184, 1.904561220, 0.000000000, 4.551627762, 3.809122439])
-    # amplitudes of equilibrium tide in meters
-    # _amplitude = np.array([0.242334,0.112743,0.141565,0.100661,0.046397,
-    _amplitude = np.array([0.2441, 0.112743, 0.141565, 0.100661, 0.046397,
-        0.046848, 0.030684, 0.019273, 0.006141, 0.007408, 0.008811, 0.006931,
-        0.006608, 0.007915, 0.007915, 0.004338, 0.003661, 0.042041, 0.022191,
-        0.019567, 0., 0., 0., 0., 0., 0., 0., 0., 0.])
-
-    # map between input constituent and cindex
-    j = [j for j,val in enumerate(cindex) if (val == c.lower())]
-    # set the values for the constituent
-    if j:
-        amplitude, = _amplitude[j]
-        phase, = _phase[j]
-        omega, = _omega[j]
-        alpha, = _alpha[j]
-        species, = _species[j]
-    else:
-        amplitude = 0.0
-        phase = 0.0
-        omega = 0.0
-        alpha = 0.0
-        species = 0
-    # return the values for the constituent
-    return (amplitude, phase, omega, alpha, species)
-
 def _out_of_phase_diurnal(
         XYZ: np.ndarray,
         SXYZ: np.ndarray,
         LXYZ: np.ndarray,
         F2_solar: np.ndarray,
         F2_lunar: np.ndarray
     ):
```

### Comparing `pyTMD-2.1.0/pyTMD/solve.py` & `pyTMD-2.1.1/pyTMD/solve/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
-solve.py
-Written by Tyler Sutterley (12/2023)
+constants.py
+Written by Tyler Sutterley (01/2024)
 Routines for estimating the harmonic constants for ocean tides
 
 REFERENCES:
     G. D. Egbert and S. Erofeeva, "Efficient Inverse Modeling of Barotropic
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 PYTHON DEPENDENCIES:
@@ -14,45 +14,44 @@
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     scipy: Scientific Tools for Python
         https://scipy.org
 
 PROGRAM DEPENDENCIES:
     arguments.py: loads nodal corrections for tidal constituents
     astro.py: computes the basic astronomical mean longitudes
-    predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 01/2024: moved to solve subdirectory
     Written 12/2023
 """
 
 from __future__ import annotations
 
 import numpy as np
 import scipy.linalg
-import pyTMD.predict
-from pyTMD.arguments import arguments
+import pyTMD.arguments
 
 def constants(t: float | np.ndarray,
         ht: np.ndarray,
-        constituents: list | np.ndarray,
+        constituents: str | list | np.ndarray,
         deltat: float | np.ndarray = 0.0,
         corrections: str = 'OTIS',
         solver: str = 'lstsq'
     ):
     """
     Estimate the harmonic constants for an elevation time series [1]_
 
     Parameters
     ----------
     t: float or np.ndarray
         days relative to 1992-01-01T00:00:00
     ht: np.ndarray
         elevation time series (meters)
-    constituents: list or np.ndarray
-        tidal constituent IDs
+    constituents: str, list or np.ndarray
+        tidal constituent ID(s)
     deltat: float or np.ndarray, default 0.0
         time correction for converting to Ephemeris Time (days)
     corrections: str, default 'OTIS'
         use nodal corrections from OTIS/ATLAS or GOT/FES models
     solver: str, default 'lstsq'
         least squares solver to use
 
@@ -73,37 +72,40 @@
     .. [1] G. D. Egbert and S. Y. Erofeeva, "Efficient Inverse Modeling of
         Barotropic Ocean Tides," *Journal of Atmospheric and Oceanic
         Technology*, 19(2), 183--204, (2002).
         `doi: 10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2`__
 
     .. __: https://doi.org/10.1175/1520-0426(2002)019<0183:EIMOBO>2.0.CO;2
     """
+    # check if input constituents is a string
+    if isinstance(constituents, str):
+        constituents = [constituents]
     # check that there are enough values for a time series fit
     nt = len(np.atleast_1d(t))
     nc = len(constituents)
     if (nt <= 2*nc):
         raise ValueError('Not enough values for fit')
     # check that the number of time values matches the number of height values
     if (nt != len(np.atleast_1d(ht))):
         raise ValueError('Dimension mismatch between input variables')
 
     # load the nodal corrections
     # convert time to Modified Julian Days (MJD)
-    pu, pf, G = arguments(t + 48622.0, constituents,
+    pu, pf, G = pyTMD.arguments.arguments(t + 48622.0, constituents,
         deltat=deltat, corrections=corrections)
 
     # create design matrix
     M = []
     # add constant term for mean
     M.append(np.ones_like(t))
     # add constituent terms
     for k,c in enumerate(constituents):
         if corrections in ('OTIS', 'ATLAS', 'TMD3', 'netcdf'):
             amp, ph, omega, alpha, species = \
-                pyTMD.predict._constituent_parameters(c)
+                pyTMD.arguments._constituent_parameters(c)
             th = omega*t*86400.0 + ph + pu[:,k]
         elif corrections in ('GOT', 'FES'):
             th = G[:,k]*np.pi/180.0 + pu[:,k]
         # add constituent to design matrix
         M.append(pf[:,k]*np.cos(th))
         M.append(-pf[:,k]*np.sin(th))
     # take the transpose of the design matrix
```

### Comparing `pyTMD-2.1.0/pyTMD/spatial.py` & `pyTMD-2.1.1/pyTMD/spatial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 spatial.py
-Written by Tyler Sutterley (10/2023)
+Written by Tyler Sutterley (03/2024)
 
 Utilities for reading, writing and operating on spatial data
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -15,17 +15,19 @@
         https://www.h5py.org/
     gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL)
         https://pypi.python.org/pypi/GDAL
     PyYAML: YAML parser and emitter for Python
         https://github.com/yaml/pyyaml
 
 PROGRAM DEPENDENCIES:
-    constants.py: calculate reference parameters for common ellipsoids
+    crs.py: Coordinate Reference System (CRS) routines
 
 UPDATE HISTORY:
+    Updated 03/2024: can calculate polar stereographic distortion for distances
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
     Updated 10/2023: can read from netCDF4 or HDF5 variable groups
         apply no formatting to columns in ascii file output
     Updated 09/2023: add function to invert field mapping keys and values
         use datetime64[ns] for parsing dates from ascii files
     Updated 08/2023: remove possible crs variables from output fields list
         place PyYAML behind try/except statement to reduce build size
     Updated 05/2023: use datetime parser within pyTMD.time module
@@ -73,18 +75,19 @@
 import re
 import io
 import copy
 import gzip
 import uuid
 import logging
 import pathlib
+import warnings
 import datetime
 import numpy as np
 import pyTMD.time
-from pyTMD.constants import constants
+from pyTMD.crs import datum
 import pyTMD.version
 # attempt imports
 try:
     import osgeo.gdal, osgeo.osr, osgeo.gdalconst
 except (AttributeError, ImportError, ModuleNotFoundError) as exc:
     logging.debug("GDAL not available")
 try:
@@ -786,15 +789,16 @@
         python dictionary of output attributes
     """
     # input data fields
     dimensions = ['time', 'lon', 'lat', 't', 'x', 'y']
     crs = ['crs', 'crs_wkt', 'crs_proj4', 'projection']
     fields = sorted(set(output.keys()) - set(dimensions) - set(crs))
     # Defining the NetCDF dimensions
-    ny, nx, nt = output[fields[0]].shape
+    reference_fields = [v for v in fields if output[v].ndim == 3]
+    ny, nx, nt = output[reference_fields[0]].shape
     fileID.createDimension('y', ny)
     fileID.createDimension('x', nx)
     fileID.createDimension('time', nt)
     # defining the NetCDF variables
     nc = {}
     for key, val in output.items():
         if key in fileID.variables:
@@ -835,15 +839,16 @@
         python dictionary of output attributes
     """
     # input data fields
     dimensions = ['time', 'lon', 'lat', 't', 'x', 'y']
     crs = ['crs', 'crs_wkt', 'crs_proj4', 'projection']
     fields = sorted(set(output.keys()) - set(dimensions) - set(crs))
     # Defining the NetCDF dimensions
-    nstation, nt = output[fields[0]].shape
+    reference_fields = [v for v in fields if output[v].ndim == 2]
+    nstation, nt = output[reference_fields[0]].shape
     fileID.createDimension('station', nstation)
     fileID.createDimension('time', nt)
     # defining the NetCDF variables
     nc = {}
     for key, val in output.items():
         if key in fileID.variables:
             nc[key] = fileID.variables[key]
@@ -1267,15 +1272,15 @@
         longitude (degrees east)
     """
     phi = np.arctan2(np.sin(lon*np.pi/180.0), np.cos(lon*np.pi/180.0))
     # convert phi from radians to degrees
     return phi*180.0/np.pi
 
 # get WGS84 parameters
-_wgs84 = constants(ellipsoid='WGS84', units='MKS')
+_wgs84 = datum(ellipsoid='WGS84', units='MKS')
 
 def to_cartesian(
         lon: np.ndarray,
         lat: np.ndarray,
         h: float | np.ndarray = 0.0,
         a_axis: float = _wgs84.a_axis,
         flat: float = _wgs84.flat
@@ -1624,47 +1629,59 @@
         zi = (1.0 - e12)*z[ind]/(t - l)
         # calculate latitude and height
         lat[ind] = np.arctan2(zi, ((1.0 - e12)*wi))/dtr
         h[ind] = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z[ind]-zi)**2.0)
     # return latitude, longitude and height
     return (lon, lat, h)
 
-def scale_areas(
+def scale_areas(*args, **kwargs):
+    warnings.warn("Deprecated. Please use pyTMD.spatial.scale_factors instead",
+        DeprecationWarning)
+    return scale_factors(*args, **kwargs)
+
+def scale_factors(
         lat: np.ndarray,
         flat: float = _wgs84.flat,
-        ref: float = 70.0
+        reference_latitude: float = 70.0,
+        metric: str = 'area'
     ):
     """
-    Calculates area scaling factors for a polar stereographic projection
-    including special case of at the exact pole [1]_ [2]_
+    Calculates scaling factors to account for polar stereographic
+    distortion including special case of at the exact pole [1]_ [2]_
 
     Parameters
     ----------
     lat: np.ndarray
         latitude (degrees north)
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
-    ref: float, default 70.0
+    reference_latitude: float, default 70.0
         reference latitude (true scale latitude)
+    metric: str, default 'area'
+        metric to calculate scaling factors
+
+            - ``'distance'``: scale factors for distance
+            - ``'area'``: scale factors for area
 
     Returns
     -------
     scale: np.ndarray
-        area scaling factors at input latitudes
+        scaling factors at input latitudes
 
     References
     ----------
     .. [1] J. P. Snyder, *Map Projections used by the U.S. Geological Survey*,
         Geological Survey Bulletin 1532, U.S. Government Printing Office, (1982).
     .. [2] JPL Technical Memorandum 3349-85-101
     """
+    assert metric.lower() in ['distance', 'area'], 'Unknown metric'
     # convert latitude from degrees to positive radians
     theta = np.abs(lat)*np.pi/180.0
     # convert reference latitude from degrees to positive radians
-    theta_ref = np.abs(ref)*np.pi/180.0
+    theta_ref = np.abs(reference_latitude)*np.pi/180.0
     # square of the eccentricity of the ellipsoid
     # ecc2 = (1-b**2/a**2) = 2.0*flat - flat^2
     ecc2 = 2.0*flat - flat**2
     # eccentricity of the ellipsoid
     ecc = np.sqrt(ecc2)
     # calculate ratio at input latitudes
     m = np.cos(theta)/np.sqrt(1.0 - ecc2*np.sin(theta)**2)
@@ -1673,10 +1690,14 @@
     # calculate ratio at reference latitude
     mref = np.cos(theta_ref)/np.sqrt(1.0 - ecc2*np.sin(theta_ref)**2)
     tref = np.tan(np.pi/4.0 - theta_ref/2.0)/((1.0 - ecc*np.sin(theta_ref)) / \
         (1.0 + ecc*np.sin(theta_ref)))**(ecc/2.0)
     # distance scaling
     k = (mref/m)*(t/tref)
     kp = 0.5*mref*np.sqrt(((1.0+ecc)**(1.0+ecc))*((1.0-ecc)**(1.0-ecc)))/tref
-    # area scaling
-    scale = np.where(np.isclose(theta, np.pi/2.0), 1.0/(kp**2), 1.0/(k**2))
+    if (metric.lower() == 'distance'):
+        # distance scaling
+        scale = np.where(np.isclose(theta, np.pi/2.0), 1.0/kp, 1.0/k)
+    elif (metric.lower() == 'area'):
+        # area scaling
+        scale = np.where(np.isclose(theta, np.pi/2.0), 1.0/(kp**2), 1.0/(k**2))
     return scale
```

### Comparing `pyTMD-2.1.0/pyTMD/time.py` & `pyTMD-2.1.1/pyTMD/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 u"""
 time.py
-Written by Tyler Sutterley (10/2023)
+Written by Tyler Sutterley (02/2024)
 Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 02/2024: move the immutable parameters in timescale class
     Updated 10/2023: add function to output timescale to string arrays
     Updated 06/2023: improve conversion of timescale to datetime arrays
     Updated 05/2023: add timescale class for converting between time scales
         added timescale to_datetime function to create datetime arrays
         allow epoch arguments to be numpy datetime64 variables or strings
         function to convert a string with time zone information to datetime
     Updated 04/2023: using pathlib to define and expand paths
@@ -611,46 +612,33 @@
 
     Attributes
     ----------
     leaps: np.ndarray
         Number of leap seconds
     MJD: np.ndarray
         Modified Julian Days
-    century: float
-        Days in a Julian century
-    day: float
-        Seconds in a day
-    turn: float
-        Fraction of a full turn
-    turndeg: float
-        Degrees in a full turn
-    tau: float
-        Radians in a full turn
-    deg2rad: float
-        Degrees to radians
-    deg2asec: float
-        Degrees to arcseconds
     """
+    # Julian century
+    century = 36525.0
+    # seconds per day
+    day = 86400.0
+    # 360 degrees
+    turn = 1.0
+    turndeg = 360.0
+    tau = 2.0*np.pi
+    # degrees to radians
+    deg2rad = np.pi/180.0
+    # degrees to arcseconds
+    deg2asec = 3600.0
+
     def __init__(self, MJD=None):
         # leap seconds
         self.leaps = None
         # modified Julian Days
         self.MJD = MJD
-        # Julian century
-        self.century = 36525.0
-        # seconds per day
-        self.day = 86400.0
-        # 360 degrees
-        self.turn = 1.0
-        self.turndeg = 360.0
-        self.tau = 2.0*np.pi
-        # degrees to radians
-        self.deg2rad = np.pi/180.0
-        # degrees to arcseconds
-        self.deg2asec = 3600.0
         # iterator
         self.__index__ = 0
 
     def from_deltatime(self,
             delta_time: np.ndarray,
             epoch: str | tuple | list | np.ndarray,
             standard: str = 'UTC'
```

### Comparing `pyTMD-2.1.0/pyTMD/tools.py` & `pyTMD-2.1.1/pyTMD/tools.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD/utilities.py` & `pyTMD-2.1.1/pyTMD/utilities.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/pyTMD.egg-info/PKG-INFO` & `pyTMD-2.1.1/pyTMD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyTMD-2.1.0/pyTMD.egg-info/SOURCES.txt` & `pyTMD-2.1.1/pyTMD.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 setup.py
 version.txt
 pyTMD/__init__.py
 pyTMD/arguments.py
 pyTMD/astro.py
 pyTMD/calc_astrol_longitudes.py
 pyTMD/check_points.py
+pyTMD/compute.py
 pyTMD/compute_tide_corrections.py
-pyTMD/constants.py
 pyTMD/convert_crs.py
 pyTMD/convert_ll_xy.py
 pyTMD/crs.py
 pyTMD/ellipse.py
 pyTMD/eop.py
 pyTMD/interpolate.py
 pyTMD/load_constituent.py
 pyTMD/load_nodal_corrections.py
 pyTMD/predict.py
-pyTMD/solve.py
 pyTMD/spatial.py
 pyTMD/time.py
 pyTMD/tools.py
 pyTMD/utilities.py
 pyTMD/version.py
 pyTMD.egg-info/PKG-INFO
 pyTMD.egg-info/SOURCES.txt
@@ -53,14 +52,16 @@
 pyTMD/io/FES.py
 pyTMD/io/GOT.py
 pyTMD/io/OTIS.py
 pyTMD/io/__init__.py
 pyTMD/io/constituents.py
 pyTMD/io/model.py
 pyTMD/io/ocean_pole_tide.py
+pyTMD/solve/__init__.py
+pyTMD/solve/constants.py
 scripts/arcticdata_tides.py
 scripts/aviso_fes_tides.py
 scripts/compute_LPET_elevations.py
 scripts/compute_LPT_displacements.py
 scripts/compute_OPT_displacements.py
 scripts/compute_SET_displacements.py
 scripts/compute_tidal_currents.py
```

### Comparing `pyTMD-2.1.0/scripts/arcticdata_tides.py` & `pyTMD-2.1.1/scripts/arcticdata_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/scripts/aviso_fes_tides.py` & `pyTMD-2.1.1/scripts/aviso_fes_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/scripts/compute_LPET_elevations.py` & `pyTMD-2.1.1/scripts/compute_LPET_elevations.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/scripts/compute_LPT_displacements.py` & `pyTMD-2.1.1/scripts/compute_LPT_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_LPT_displacements.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (02/2024)
 Calculates radial load pole tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -67,22 +67,22 @@
         https://pandas.pydata.org/
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
-    constants.py: gravitational and ellipsoidal parameters
     crs.py: Coordinate Reference System (CRS) routines
     eop.py: utilities for calculating Earth Orientation Parameters (EOP)
     spatial: utilities for reading, writing and operating on spatial data
     time.py: utilities for calculating time operations
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
     Updated 12/2023: use new crs class to get projection information
     Updated 10/2023: can write datetime as time column for csv files
     Updated 05/2023: use timescale class for time conversion operations
         use defaults from eop module for pole tide and EOP files
     Updated 04/2023: check if datetime before converting to seconds
         using pathlib to define and expand paths
     Updated 03/2023: added option for changing the IERS mean pole convention
@@ -240,15 +240,15 @@
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
     # tidal love number appropriate for the load tide
     hb2 = 0.6207
 
     # flatten heights
     h = np.ravel(dinput['data']) if ('data' in dinput.keys()) else 0.0
     # convert from geodetic latitude to geocentric latitude
     # calculate X, Y and Z from geodetic latitude and longitude
```

### Comparing `pyTMD-2.1.0/scripts/compute_OPT_displacements.py` & `pyTMD-2.1.1/scripts/compute_OPT_displacements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_OPT_displacements.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (02/2024)
 Calculates radial ocean pole load tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -86,14 +86,15 @@
     S. Desai, "Observing the pole tide with satellite altimetry", Journal of
         Geophysical Research: Oceans, 107(C11), 2002. doi: 10.1029/2001JC001224
     S. Desai, J. Wahr and B. Beckley "Revisiting the pole tide for and from
         satellite altimetry", Journal of Geodesy, 89(12), p1233-1243, 2015.
         doi: 10.1007/s00190-015-0848-7
 
 UPDATE HISTORY:
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
     Updated 12/2023: use new crs class to get projection information
     Updated 10/2023: can write datetime as time column for csv files
     Updated 05/2023: use timescale class for time conversion operations
         use defaults from eop module for pole tide and EOP files
     Updated 04/2023: check if datetime before converting to seconds
         using pathlib to define and expand paths
     Updated 03/2023: added option for changing the IERS mean pole convention
@@ -258,15 +259,15 @@
     # number of time points
     nt = len(time_decimal)
 
     # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
     # mean equatorial gravitational acceleration [m/s^2]
     ge = 9.7803278
     # density of sea water [kg/m^3]
     rho_w = 1025.0
     # tidal love number differential (1 + kl - hl) for pole tide frequencies
     gamma = 0.6870 + 0.0036j
```

### Comparing `pyTMD-2.1.0/scripts/compute_SET_displacements.py` & `pyTMD-2.1.1/scripts/compute_SET_displacements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_SET_displacements.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (02/2024)
 Calculates radial solid earth tide displacements for an input file
     following IERS Convention (2010) guidelines
     https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
@@ -93,14 +93,16 @@
         19(6), 529--531, (1992). doi: 10.1029/92GL00259
     J. M. Wahr, "Body tides on an elliptical, rotating, elastic
         and oceanless Earth", Geophysical Journal of the Royal
         Astronomical Society, 64(3), 677--703, (1981).
         doi: 10.1111/j.1365-246X.1981.tb02690.x
 
 UPDATE HISTORY:
+    Updated 02/2024: changed class name for ellipsoid parameters to datum
+    Updated 01/2024: refactored lunisolar ephemerides functions
     Updated 12/2023: use new crs class to get projection information
     Updated 10/2023: can write datetime as time column for csv files
     Updated 05/2023: use timescale class for time conversion operations
         add option for using higher resolution ephemerides from JPL
     Updated 04/2023: using pathlib to define and expand paths
     Written 04/2023
 """
@@ -227,30 +229,24 @@
             epoch=epoch1, standard=TIME_STANDARD)
     # convert tide times to dynamical time
     tide_time = timescale.tide + timescale.tt_ut1
     # number of time points
     nt = len(timescale)
 
     # earth and physical parameters for ellipsoid
-    units = pyTMD.constants(ELLIPSOID)
+    units = pyTMD.datum(ellipsoid=ELLIPSOID, units='MKS')
 
     # flatten heights
     h = np.ravel(dinput['data']) if ('data' in dinput.keys()) else 0.0
     # convert input coordinates to cartesian
     X, Y, Z = pyTMD.spatial.to_cartesian(lon, lat, h=h,
         a_axis=units.a_axis, flat=units.flat)
     # compute ephemerides for lunisolar coordinates
-    if (EPHEMERIDES.lower() == 'approximate'):
-        # get low-resolution solar and lunar ephemerides
-        SX, SY, SZ = pyTMD.astro.solar_ecef(timescale.MJD)
-        LX, LY, LZ = pyTMD.astro.lunar_ecef(timescale.MJD)
-    elif (EPHEMERIDES.upper() == 'JPL'):
-        # compute solar and lunar ephemerides from JPL kernel
-        SX, SY, SZ = pyTMD.astro.solar_ephemerides(timescale.MJD)
-        LX, LY, LZ = pyTMD.astro.lunar_ephemerides(timescale.MJD)
+    SX, SY, SZ = pyTMD.astro.solar_ecef(timescale.MJD, ephemerides=EPHEMERIDES)
+    LX, LY, LZ = pyTMD.astro.lunar_ecef(timescale.MJD, ephemerides=EPHEMERIDES)
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         tide_se = np.zeros((ny,nx,nt))
         # convert coordinates to column arrays
         XYZ = np.c_[X, Y, Z]
         for i in range(nt):
```

### Comparing `pyTMD-2.1.0/scripts/compute_tidal_currents.py` & `pyTMD-2.1.1/scripts/compute_tidal_currents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_tidal_currents.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (01/2024)
 Calculates zonal and meridional tidal currents for an input file
 
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 or Finite Element Solution (FES) models provided by AVISO
@@ -52,14 +52,15 @@
         spline
         linear
         nearest
         bilinear
     -E X, --extrapolate X: Extrapolate with nearest-neighbors
     -c X, --cutoff X: Extrapolation cutoff in kilometers
         set to inf to extrapolate for all points
+    --infer-minor: Infer the current values for minor constituents
     -f X, --fill-value X: Invalid value for spatial fields
     -V, --verbose: Verbose output of processing run
     -M X, --mode X: Permission mode of output file
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
@@ -90,14 +91,15 @@
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
     predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 01/2024: made the inferrence of minor constituents an option
     Updated 12/2023: use new crs class to get projection information
     Updated 10/2023: can write datetime as time column for csv files
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 05/2023: use timescale class for time conversion operations
     Updated 04/2023: using pathlib to define and expand paths
         using long_name and description attributes from model class
     Updated 02/2023: added functionality for time series type
@@ -191,14 +193,15 @@
     TIME_UNITS='days since 1858-11-17T00:00:00',
     TIME=None,
     TIME_STANDARD='UTC',
     PROJECTION='4326',
     METHOD='spline',
     EXTRAPOLATE=False,
     CUTOFF=None,
+    INFER_MINOR=False,
     FILL_VALUE=-9999.0,
     VERBOSE=False,
     MODE=0o775):
 
     # create logger for verbosity level
     loglevel = logging.INFO if VERBOSE else logging.CRITICAL
     logging.basicConfig(level=loglevel)
@@ -301,44 +304,56 @@
             deltat = timescale.tt_ut1
 
         # calculate complex phase in radians for Euler's
         cph = -1j*ph*np.pi/180.0
         # calculate constituent oscillation
         hc = amp*np.exp(cph)
 
-        # predict tidal currents at time and infer minor corrections
+        # predict tidal currents at time
         if (TYPE == 'grid'):
             tide[t] = np.ma.zeros((ny,nx,nt), fill_value=FILL_VALUE)
             tide[t].mask = np.zeros((ny,nx,nt),dtype=bool)
             for i in range(nt):
                 TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
                     deltat=deltat[i], corrections=model.format)
-                MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
-                    deltat=deltat[i], corrections=model.format)
+                # calculate values for minor constituents by inferrence
+                if INFER_MINOR:
+                    MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
+                        deltat=deltat[i], corrections=model.format)
+                else:
+                    MINOR = np.ma.zeros_like(TIDE)
                 # add major and minor components and reform grid
                 tide[t][:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
                 tide[t].mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask),
                     (ny,nx))
         elif (TYPE == 'drift'):
             tide[t] = np.ma.zeros((nt), fill_value=FILL_VALUE)
             tide[t].mask = np.any(hc.mask,axis=1)
             tide[t].data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
                 deltat=deltat, corrections=model.format)
-            minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
-                deltat=deltat, corrections=model.format)
-            tide[t].data[:] += minor.data[:]
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
+                    deltat=deltat, corrections=model.format)
+                tide[t].data[:] += minor.data[:]
         elif (TYPE == 'time series'):
             tide[t] = np.ma.zeros((nstation,nt), fill_value=FILL_VALUE)
             tide[t].mask = np.zeros((nstation,nt),dtype=bool)
             for s in range(nstation):
                 # calculate constituent oscillation for station
-                TIDE = pyTMD.predict.time_series(timescale.tide, hc[s,None,:], c,
-                    deltat=deltat, corrections=model.format)
-                MINOR = pyTMD.predict.infer_minor(timescale.tide, hc[s,None,:], c,
+                HC = hc[s,None,:]
+                TIDE = pyTMD.predict.time_series(timescale.tide, HC, c,
                     deltat=deltat, corrections=model.format)
+                # calculate values for minor constituents by inferrence
+                if INFER_MINOR:
+                    MINOR = pyTMD.predict.infer_minor(timescale.tide, HC, c,
+                        deltat=deltat, corrections=model.format)
+                else:
+                    MINOR = np.ma.zeros_like(TIDE)
+                # add major and minor components
                 tide[t].data[s,:] = TIDE.data[:] + MINOR.data[:]
                 tide[t].mask[s,:] = (TIDE.mask | MINOR.mask)
         # replace invalid values with fill value
         tide[t].data[tide[t].mask] = tide[t].fill_value
 
     # output netCDF4 and HDF5 file attributes
     # will be added to YAML header in csv files
@@ -494,14 +509,18 @@
         default=False, action='store_true',
         help='Extrapolate with nearest-neighbors')
     # extrapolation cutoff in kilometers
     # set to inf to extrapolate over all points
     parser.add_argument('--cutoff','-c',
         type=np.float64, default=10.0,
         help='Extrapolation cutoff in kilometers')
+    # infer minor constituents from major
+    parser.add_argument('--infer-minor',
+        default=False, action='store_true',
+        help='Infer the current values for minor constituents')
     # fill value for output spatial fields
     parser.add_argument('--fill-value','-f',
         type=float, default=-9999.0,
         help='Invalid value for spatial fields')
     # verbose output of processing run
     # print information about each input and output file
     parser.add_argument('--verbose','-V',
@@ -539,14 +558,15 @@
         TIME_UNITS=args.epoch,
         TIME=args.deltatime,
         TIME_STANDARD=args.standard,
         PROJECTION=args.projection,
         METHOD=args.interpolate,
         EXTRAPOLATE=args.extrapolate,
         CUTOFF=args.cutoff,
+        INFER_MINOR=args.infer_minor,
         FILL_VALUE=args.fill_value,
         VERBOSE=args.verbose,
         MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.1.0/scripts/compute_tidal_elevations.py` & `pyTMD-2.1.1/scripts/compute_tidal_elevations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_tidal_elevations.py
-Written by Tyler Sutterley (12/2023)
+Written by Tyler Sutterley (01/2024)
 Calculates tidal elevations for an input file
 
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -53,15 +53,16 @@
         spline
         linear
         nearest
         bilinear
     -E X, --extrapolate X: Extrapolate with nearest-neighbors
     -c X, --cutoff X: Extrapolation cutoff in kilometers
         set to inf to extrapolate for all points
-    --apply-flexure: Apply ice flexure scaling factor to height constituents
+    --infer-minor: Infer the height values for minor constituents
+    --apply-flexure: Apply ice flexure scaling factor to height values
         Only valid for models containing flexure fields
     -f X, --fill-value X: Invalid value for spatial fields
     -V, --verbose: Verbose output of processing run
     -M X, --mode X: Permission mode of output file
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
@@ -93,14 +94,15 @@
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
     predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 01/2024: made the inferrence of minor constituents an option
     Updated 12/2023: use new crs class to get projection information
     Updated 10/2023: can write datetime as time column for csv files
     Updated 08/2023: changed ESR netCDF4 format to TMD3 format
     Updated 05/2023: use timescale class for time conversion operations
     Updated 04/2023: check if datetime before converting to seconds
         using pathlib to define and expand paths
     Updated 02/2023: added functionality for time series type
@@ -195,14 +197,15 @@
     TIME_UNITS='days since 1858-11-17T00:00:00',
     TIME_STANDARD='UTC',
     TIME=None,
     PROJECTION='4326',
     METHOD='spline',
     EXTRAPOLATE=False,
     CUTOFF=None,
+    INFER_MINOR=False,
     APPLY_FLEXURE=False,
     FILL_VALUE=-9999.0,
     VERBOSE=False,
     MODE=0o775):
 
     # create logger for verbosity level
     loglevel = logging.INFO if VERBOSE else logging.CRITICAL
@@ -308,43 +311,55 @@
         deltat = timescale.tt_ut1
 
     # calculate complex phase in radians for Euler's
     cph = -1j*ph*np.pi/180.0
     # calculate constituent oscillation
     hc = amp*np.exp(cph)
 
-    # predict tidal elevations at time and infer minor corrections
+    # predict tidal elevations at time
     if (TYPE == 'grid'):
         tide = np.ma.zeros((ny,nx,nt), fill_value=FILL_VALUE)
         tide.mask = np.zeros((ny,nx,nt),dtype=bool)
         for i in range(nt):
             TIDE = pyTMD.predict.map(timescale.tide[i], hc, c,
                 deltat=deltat[i], corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
-                deltat=deltat[i], corrections=model.format)
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                MINOR = pyTMD.predict.infer_minor(timescale.tide[i], hc, c,
+                    deltat=deltat[i], corrections=model.format)
+            else:
+                MINOR = np.ma.zeros_like(TIDE)
             # add major and minor components and reform grid
             tide[:,:,i] = np.reshape((TIDE+MINOR), (ny,nx))
             tide.mask[:,:,i] = np.reshape((TIDE.mask | MINOR.mask), (ny,nx))
     elif (TYPE == 'drift'):
         tide = np.ma.zeros((nt), fill_value=FILL_VALUE)
         tide.mask = np.any(hc.mask,axis=1)
         tide.data[:] = pyTMD.predict.drift(timescale.tide, hc, c,
             deltat=deltat, corrections=model.format)
-        minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
-            deltat=deltat, corrections=model.format)
-        tide.data[:] += minor.data[:]
+        # calculate values for minor constituents by inferrence
+        if INFER_MINOR:
+            minor = pyTMD.predict.infer_minor(timescale.tide, hc, c,
+                deltat=deltat, corrections=model.format)
+            tide.data[:] += minor.data[:]
     elif (TYPE == 'time series'):
         tide = np.ma.zeros((nstation,nt), fill_value=FILL_VALUE)
         tide.mask = np.zeros((nstation,nt),dtype=bool)
         for s in range(nstation):
             # calculate constituent oscillation for station
-            TIDE = pyTMD.predict.time_series(timescale.tide, hc[s,None,:], c,
-                deltat=deltat, corrections=model.format)
-            MINOR = pyTMD.predict.infer_minor(timescale.tide, hc[s,None,:], c,
+            HC = hc[s,None,:]
+            TIDE = pyTMD.predict.time_series(timescale.tide, HC, c,
                 deltat=deltat, corrections=model.format)
+            # calculate values for minor constituents by inferrence
+            if INFER_MINOR:
+                MINOR = pyTMD.predict.infer_minor(timescale.tide, HC, c,
+                    deltat=deltat, corrections=model.format)
+            else:
+                MINOR = np.ma.zeros_like(TIDE)
+            # add major and minor components
             tide.data[s,:] = TIDE.data[:] + MINOR.data[:]
             tide.mask[s,:] = (TIDE.mask | MINOR.mask)
     # replace invalid values with fill value
     tide.data[tide.mask] = tide.fill_value
 
     # output netCDF4 and HDF5 file attributes
     # will be added to YAML header in csv files
@@ -490,18 +505,22 @@
         default=False, action='store_true',
         help='Extrapolate with nearest-neighbors')
     # extrapolation cutoff in kilometers
     # set to inf to extrapolate over all points
     parser.add_argument('--cutoff','-c',
         type=np.float64, default=10.0,
         help='Extrapolation cutoff in kilometers')
-    # apply flexure scaling factors to height constituents
+    # infer minor constituents from major
+    parser.add_argument('--infer-minor',
+        default=False, action='store_true',
+        help='Infer the height values for minor constituents')
+    # apply flexure scaling factors to height values
     parser.add_argument('--apply-flexure',
         default=False, action='store_true',
-        help='Apply ice flexure scaling factor to height constituents')
+        help='Apply ice flexure scaling factor to height values')
     # fill value for output spatial fields
     parser.add_argument('--fill-value','-f',
         type=float, default=-9999.0,
         help='Invalid value for spatial fields')
     # verbose output of processing run
     # print information about each input and output file
     parser.add_argument('--verbose','-V',
@@ -541,14 +560,15 @@
         TIME=args.deltatime,
         TIME_STANDARD=args.standard,
         PROJECTION=args.projection,
         METHOD=args.interpolate,
         EXTRAPOLATE=args.extrapolate,
         CUTOFF=args.cutoff,
         APPLY_FLEXURE=args.apply_flexure,
+        INFER_MINOR=args.infer_minor,
         FILL_VALUE=args.fill_value,
         VERBOSE=args.verbose,
         MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.1.0/scripts/reduce_OTIS_files.py` & `pyTMD-2.1.1/scripts/reduce_OTIS_files.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/scripts/usap_cats_tides.py` & `pyTMD-2.1.1/scripts/usap_cats_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/scripts/verify_box_tpxo.py` & `pyTMD-2.1.1/scripts/verify_box_tpxo.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.1.0/setup.py` & `pyTMD-2.1.1/setup.py`

 * *Files identical despite different names*

