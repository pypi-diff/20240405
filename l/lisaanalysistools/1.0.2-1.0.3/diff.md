# Comparing `tmp/lisaanalysistools-1.0.2.tar.gz` & `tmp/lisaanalysistools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisaanalysistools-1.0.2.tar", last modified: Thu Mar 28 17:15:45 2024, max compression
+gzip compressed data, was "lisaanalysistools-1.0.3.tar", last modified: Fri Apr  5 07:54:53 2024, max compression
```

## Comparing `lisaanalysistools-1.0.2.tar` & `lisaanalysistools-1.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.309959 lisaanalysistools-1.0.2/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.2/CHANGELOG
--rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.2/LICENSE
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.307556 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-03-28 17:15:45.000000 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1802 2024-03-28 17:15:45.000000 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/SOURCES.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-28 17:15:45.000000 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/dependency_links.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-13 23:07:52.000000 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/not-zip-safe
--rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-03-28 17:15:45.000000 lisaanalysistools-1.0.2/LISAanalysistools.egg-info/top_level.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.2/MANIFEST.in
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.2/Makefile
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-03-28 17:15:45.308931 lisaanalysistools-1.0.2/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2156 2024-03-28 17:14:56.000000 lisaanalysistools-1.0.2/README.md
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.263959 lisaanalysistools-1.0.2/include/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/include/Detector.hpp
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.274012 lisaanalysistools-1.0.2/lisatools/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.2/lisatools/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-03-28 17:15:45.000000 lisaanalysistools-1.0.2/lisatools/_version.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    15329 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/analysiscontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9224 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/datacontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    12183 2024-03-28 17:12:30.000000 lisaanalysistools-1.0.2/lisatools/detector.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    34177 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/diagnostic.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5154 2024-02-20 21:17:07.000000 lisaanalysistools-1.0.2/lisatools/glitch.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.277895 lisaanalysistools-1.0.2/lisatools/sampling/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.2/lisatools/sampling/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sampling/likelihood.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.286504 lisaanalysistools-1.0.2/lisatools/sampling/moves/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1220 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/gbgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    51802 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/gbmultipletryrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    31152 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/gbspecialgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    90189 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/gbspecialstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14163 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/mbhspecialmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      469 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/placeholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/skymodehop.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    25092 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.2/lisatools/sampling/moves/specialforegroundmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    18461 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sampling/prior.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sampling/stopping.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sampling/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    27236 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/sensitivity.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.287633 lisaanalysistools-1.0.2/lisatools/sources/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-01 22:45:54.000000 lisaanalysistools-1.0.2/lisatools/sources/__init__.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.289412 lisaanalysistools-1.0.2/lisatools/sources/emri/
--rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-03-01 23:04:25.000000 lisaanalysistools-1.0.2/lisatools/sources/emri/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-03-05 21:50:21.000000 lisaanalysistools-1.0.2/lisatools/sources/emri/tdiwaveform.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9440 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/stochastic.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.294580 lisaanalysistools-1.0.2/lisatools/utils/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.2/lisatools/utils/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/utils/constants.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    33765 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.2/lisatools/utils/multigpudataholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/utils/pointeradjust.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6742 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/lisatools/utils/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-03-28 17:15:23.000000 lisaanalysistools-1.0.2/pyproject.toml
--rw-r--r--   0 mlkatz1    (502) staff       (20)       30 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/requirements-data.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       15 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/requirements-demo.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      263 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/requirements-dev.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       33 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/requirements-release.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      143 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/requirements.txt
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.301084 lisaanalysistools-1.0.2/scripts/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/data_download.py
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/generate-changelog.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/install-hooks.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/post-commit.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/run-tests.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/scripts/to_conda.bash
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-03-28 17:15:45.310361 lisaanalysistools-1.0.2/setup.cfg
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-03-27 20:31:21.000000 lisaanalysistools-1.0.2/setup.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-28 17:15:45.306202 lisaanalysistools-1.0.2/src/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/src/Detector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)   635525 2024-03-28 17:12:59.000000 lisaanalysistools-1.0.2/src/pycppdetector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.2/src/pycppdetector.pyx
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.212034 lisaanalysistools-1.0.3/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/CHANGELOG
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/LICENSE
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.209537 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1802 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-13 23:07:52.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/not-zip-safe
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/MANIFEST.in
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/Makefile
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-04-05 07:54:53.210898 lisaanalysistools-1.0.3/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2156 2024-04-05 07:51:03.000000 lisaanalysistools-1.0.3/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.151281 lisaanalysistools-1.0.3/include/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/include/Detector.hpp
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.166318 lisaanalysistools-1.0.3/lisatools/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/lisatools/_version.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15333 2024-04-04 00:21:39.000000 lisaanalysistools-1.0.3/lisatools/analysiscontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9224 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/datacontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    13852 2024-04-02 17:24:55.000000 lisaanalysistools-1.0.3/lisatools/detector.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    34177 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/diagnostic.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5154 2024-02-20 21:17:07.000000 lisaanalysistools-1.0.3/lisatools/glitch.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.171704 lisaanalysistools-1.0.3/lisatools/sampling/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/sampling/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/likelihood.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.182855 lisaanalysistools-1.0.3/lisatools/sampling/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1220 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbgroupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    51802 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbmultipletryrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    31152 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialgroupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    90189 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    14163 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/mbhspecialmove.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      469 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/placeholder.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/skymodehop.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    25092 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/specialforegroundmove.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    18461 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    27236 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sensitivity.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.184698 lisaanalysistools-1.0.3/lisatools/sources/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-01 22:45:54.000000 lisaanalysistools-1.0.3/lisatools/sources/__init__.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.186781 lisaanalysistools-1.0.3/lisatools/sources/emri/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-03-01 23:04:25.000000 lisaanalysistools-1.0.3/lisatools/sources/emri/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-03-05 21:50:21.000000 lisaanalysistools-1.0.3/lisatools/sources/emri/tdiwaveform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9440 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/stochastic.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.193304 lisaanalysistools-1.0.3/lisatools/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/constants.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    33765 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.3/lisatools/utils/multigpudataholder.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/pointeradjust.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6742 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-04-05 07:51:18.000000 lisaanalysistools-1.0.3/pyproject.toml
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       30 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-data.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       15 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-demo.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      263 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-dev.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       33 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-release.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      143 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements.txt
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.201184 lisaanalysistools-1.0.3/scripts/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/data_download.py
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/generate-changelog.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/install-hooks.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/post-commit.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/run-tests.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/to_conda.bash
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-05 07:54:53.212303 lisaanalysistools-1.0.3/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-03-27 20:31:21.000000 lisaanalysistools-1.0.3/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.207961 lisaanalysistools-1.0.3/src/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/src/Detector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)   636410 2024-04-05 07:51:47.000000 lisaanalysistools-1.0.3/src/pycppdetector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/src/pycppdetector.pyx
```

### Comparing `lisaanalysistools-1.0.2/LICENSE` & `lisaanalysistools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/LISAanalysistools.egg-info/PKG-INFO` & `lisaanalysistools-1.0.3/LISAanalysistools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.2
+Current Version: 1.0.3
 
 ## Authors/Developers
 
 * **Michael Katz**
 
 ### Contibutors
```

### Comparing `lisaanalysistools-1.0.2/LISAanalysistools.egg-info/SOURCES.txt` & `lisaanalysistools-1.0.3/LISAanalysistools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/Makefile` & `lisaanalysistools-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/PKG-INFO` & `lisaanalysistools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.2
+Current Version: 1.0.3
 
 ## Authors/Developers
 
 * **Michael Katz**
 
 ### Contibutors
```

### Comparing `lisaanalysistools-1.0.2/README.md` & `lisaanalysistools-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.2
+Current Version: 1.0.3
 
 ## Authors/Developers
 
 * **Michael Katz**
 
 ### Contibutors
```

### Comparing `lisaanalysistools-1.0.2/include/Detector.hpp` & `lisaanalysistools-1.0.3/include/Detector.hpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/analysiscontainer.py` & `lisaanalysistools-1.0.3/lisatools/analysiscontainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         """
         if noise_only and source_only:
             raise ValueError("noise_only and source only cannot both be True.")
         elif noise_only:
             return noise_likelihood_term(self.sens_mat)
         elif source_only:
             return residual_source_likelihood_term(
-                self.data_res_arr, self.sens_mat, **kwargs
+                self.data_res_arr, psd=self.sens_mat, **kwargs
             )
         else:
             return residual_full_source_and_noise_likelihood(
                 self.data_res_arr, self.sens_mat, **kwargs
             )
 
     def _calculate_signal_operation(
```

### Comparing `lisaanalysistools-1.0.2/lisatools/datacontainer.py` & `lisaanalysistools-1.0.3/lisatools/datacontainer.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/detector.py` & `lisaanalysistools-1.0.3/lisatools/detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 class Orbits(ABC):
     """LISA Orbit Base Class
 
     Args:
         filename: File name. File should be in the style of LISAOrbits
 
-
     """
 
     def __init__(self, filename: str) -> None:
         self.filename = filename
         self._setup()
         self.configured = False
 
@@ -47,42 +46,54 @@
 
     @property
     def link_space_craft_e(self) -> List[int]:
         """Sender (second) spacecraft"""
         return [int(str(link_i)[1]) for link_i in self.LINKS]
 
     def _setup(self) -> None:
+        """Read in orbital data from file and store."""
         with self.open() as f:
             for key in f.attrs.keys():
                 setattr(self, key + "_base", f.attrs[key])
 
     @property
     def filename(self) -> str:
         """Orbit file name."""
         return self._filename
 
     @filename.setter
     def filename(self, filename: str) -> None:
         """Set file name."""
+
         assert isinstance(filename, str)
+
+        # get path
         path_to_this_file = __file__.split("detector.py")[0]
+
+        # make sure orbit_files directory exists in the right place
         if not os.path.exists(path_to_this_file + "orbit_files/"):
             os.mkdir(path_to_this_file + "orbit_files/")
         path_to_this_file = path_to_this_file + "orbit_files/"
+
         if not os.path.exists(path_to_this_file + filename):
+            # download files from github if they are not there
             github_file = f"https://github.com/mikekatz04/LISAanalysistools/raw/main/lisatools/orbit_files/{filename}"
             r = requests.get(github_file)
+
+            # if not success
             if r.status_code != 200:
                 raise ValueError(
                     f"Cannot find {filename} within default files located at github.com/mikekatz04/LISAanalysistools/lisatools/orbit_files/."
                 )
 
+            # write the contents to a local file
             with open(path_to_this_file + filename, "wb") as f:
                 f.write(r.content)
 
+        # store
         self._filename = path_to_this_file + filename
 
     def open(self) -> h5py.File:
         """Opens the h5 file in the proper mode.
 
         Returns:
             H5 file object: Opened file.
@@ -92,15 +103,15 @@
 
         """
         f = h5py.File(self.filename, "r")
         return f
 
     @property
     def t_base(self) -> np.ndarray:
-        """Light travel times along links from file."""
+        """Time array from file."""
         with self.open() as f:
             t_base = np.arange(self.size_base) * self.dt_base
         return t_base
 
     @property
     def ltt_base(self) -> np.ndarray:
         """Light travel times along links from file."""
@@ -113,22 +124,22 @@
         """Normal unit vectors towards receiver along links from file."""
         with self.open() as f:
             n = f["tcb"]["n"][:]
         return n
 
     @property
     def x_base(self) -> np.ndarray:
-        """Light travel times along links from file."""
+        """Spacecraft position from file."""
         with self.open() as f:
             x = f["tcb"]["x"][:]
         return x
 
     @property
     def v_base(self) -> np.ndarray:
-        """Light travel times along links from file."""
+        """Spacecraft velocities from file."""
         with self.open() as f:
             v = f["tcb"]["v"][:]
         return v
 
     @property
     def t(self) -> np.ndarray:
         """Configured time array."""
@@ -150,43 +161,43 @@
     @ltt.setter
     def ltt(self, ltt: np.ndarray) -> np.ndarray:
         """Set light travel time."""
         assert ltt.shape[0] == len(self.t)
 
     @property
     def n(self) -> np.ndarray:
-        """Light travel time."""
+        """Normal vectors along links."""
         self._check_configured()
         return self._n
 
     @n.setter
     def n(self, n: np.ndarray) -> np.ndarray:
-        """Set light travel time."""
+        """Set Normal vectors along links."""
         return self._n
 
     @property
     def x(self) -> np.ndarray:
-        """Light travel time."""
+        """Spacecraft positions."""
         self._check_configured()
         return self._x
 
     @x.setter
     def x(self, x: np.ndarray) -> np.ndarray:
-        """Set light travel time."""
+        """Set Spacecraft positions."""
         return self._x
 
     @property
     def v(self) -> np.ndarray:
-        """Light travel time."""
+        """Spacecraft velocities."""
         self._check_configured()
         return self._v
 
     @v.setter
     def v(self, v: np.ndarray) -> np.ndarray:
-        """Set light travel time."""
+        """Set Spacecraft velocities."""
         return self._v
 
     def configure(
         self,
         t_arr: Optional[np.ndarray] = None,
         dt: Optional[float] = None,
         linear_interp_setup: Optional[bool] = False,
@@ -286,14 +297,15 @@
                 "Asking for c++ class. Need to set linear_interp_setup = True when configuring."
             )
         self._pycppdetector = pycppDetector(*self._pycppdetector_args)
         return self._pycppdetector
 
     @property
     def pycppdetector_args(self) -> tuple:
+        """args for the c++ class."""
         return self._pycppdetector_args
 
     @pycppdetector_args.setter
     def pycppdetector_args(self, pycppdetector_args: tuple) -> None:
         self._pycppdetector_args = pycppdetector_args
 
     @property
@@ -307,71 +319,131 @@
             raise ValueError(
                 "Cannot request property. Need to use configure() method first."
             )
 
     def get_light_travel_times(
         self, t: float | np.ndarray, link: int
     ) -> float | np.ndarray:
+        """Compute light travel time as a function of time.
+
+        Computes with the c++ backend.
+
+        Args:
+            t: Time array in seconds.
+            link: which link. Must be ``in self.LINKS``.
+
+        Returns:
+            Light travel times.
+
+        """
         return self.pycppdetector.get_light_travel_time(t, link)
 
     def get_normal_unit_vec(self, t: float | np.ndarray, link: int) -> np.ndarray:
+        """Compute link normal vector as a function of time.
+
+        Computes with the c++ backend.
+
+        Args:
+            t: Time array in seconds.
+            link: which link. Must be ``in self.LINKS``.
+
+        Returns:
+            Link normal vectors.
+
+        """
         return self.pycppdetector.get_normal_unit_vec(t, link)
 
     def get_pos(self, t: float | np.ndarray, sc: int) -> np.ndarray:
+        """Compute spacecraft position as a function of time.
+
+        Computes with the c++ backend.
+
+        Args:
+            t: Time array in seconds.
+            sc: which spacecraft. Must be ``in self.SC``.
+
+        Returns:
+            Spacecraft positions.
+
+        """
         return self.pycppdetector.get_pos(t, sc)
 
     @property
     def ptr(self) -> int:
-        """pointer to c-class"""
+        """pointer to c++ class"""
         return self.pycppdetector.ptr
 
 
 class EqualArmlengthOrbits(Orbits):
-    """Equal Armlength Orbits"""
+    """Equal Armlength Orbits
+
+    Orbit file: equalarmlength-orbits.h5
+
+    """
 
     def __init__(self):
-        # TODO: fix this up
         super().__init__("equalarmlength-orbits.h5")
 
 
+class ESAOrbits(Orbits):
+    """ESA Orbits
+
+    Orbit file: esa-trailing-orbits.h5
+
+    """
+
+    def __init__(self):
+        # TODO: fix this up
+        super().__init__("esa-trailing-orbits.h5")
+
+
 class DefaultOrbits(EqualArmlengthOrbits):
-    """Set default orbit class to Equal Arm Length orbits for now."""
+    """Set default orbit class to Equal Armlength orbits for now."""
 
     pass
 
 
 @dataclass
 class LISAModelSettings:
     """Required LISA model settings:
 
-    TODO: rename these
-
     Args:
         Soms_d: OMS displacement noise.
         Sa_a: Acceleration noise.
+        orbits: Orbital information.
         name: Name of model.
 
     """
 
     Soms_d: float
     Sa_a: float
     orbits: Orbits
     name: str
 
 
 class LISAModel(LISAModelSettings, ABC):
-    """Model for the LISA Constellation"""
+    """Model for the LISA Constellation
+
+    This includes sensitivity information computed in
+    :module:`lisatools.sensitivity` and orbital information
+    contained in an :class:`Orbits` class object.
+
+    This class is used to house high-level methods useful
+    to various needed computations.
+
+    """
 
     def __str__(self) -> str:
         out = "LISA Constellation Configurations Settings:\n"
         for key, item in self.__dict__.items():
             out += f"{key}: {item}\n"
         return out
 
 
+# defaults
 scirdv1 = LISAModel((15.0e-12) ** 2, (3.0e-15) ** 2, DefaultOrbits(), "scirdv1")
 proposal = LISAModel((10.0e-12) ** 2, (3.0e-15) ** 2, DefaultOrbits(), "proposal")
 mrdv1 = LISAModel((10.0e-12) ** 2, (2.4e-15) ** 2, DefaultOrbits(), "mrdv1")
 sangria = LISAModel((10.0e-12) ** 2, (2.4e-15) ** 2, DefaultOrbits(), "sangria")
 
 __stock_list_models__ = [scirdv1, proposal, mrdv1, sangria]
 __stock_list_models_name__ = [tmp.name for tmp in __stock_list_models__]
```

### Comparing `lisaanalysistools-1.0.2/lisatools/diagnostic.py` & `lisaanalysistools-1.0.3/lisatools/diagnostic.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/glitch.py` & `lisaanalysistools-1.0.3/lisatools/glitch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/likelihood.py` & `lisaanalysistools-1.0.3/lisatools/sampling/likelihood.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/gbgroupstretch.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbgroupstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/gbmultipletryrj.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbmultipletryrj.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/gbspecialgroupstretch.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialgroupstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/gbspecialstretch.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/mbhspecialmove.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/mbhspecialmove.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/skymodehop.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/skymodehop.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/moves/specialforegroundmove.py` & `lisaanalysistools-1.0.3/lisatools/sampling/moves/specialforegroundmove.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/prior.py` & `lisaanalysistools-1.0.3/lisatools/sampling/prior.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/stopping.py` & `lisaanalysistools-1.0.3/lisatools/sampling/stopping.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sampling/utility.py` & `lisaanalysistools-1.0.3/lisatools/sampling/utility.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sensitivity.py` & `lisaanalysistools-1.0.3/lisatools/sensitivity.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/sources/emri/tdiwaveform.py` & `lisaanalysistools-1.0.3/lisatools/sources/emri/tdiwaveform.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/stochastic.py` & `lisaanalysistools-1.0.3/lisatools/stochastic.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/utils/constants.py` & `lisaanalysistools-1.0.3/lisatools/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/utils/multigpudataholder.py` & `lisaanalysistools-1.0.3/lisatools/utils/multigpudataholder.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/utils/pointeradjust.py` & `lisaanalysistools-1.0.3/lisatools/utils/pointeradjust.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/lisatools/utils/utility.py` & `lisaanalysistools-1.0.3/lisatools/utils/utility.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/scripts/data_download.py` & `lisaanalysistools-1.0.3/scripts/data_download.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/scripts/generate-changelog.bash` & `lisaanalysistools-1.0.3/scripts/generate-changelog.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/scripts/run-tests.bash` & `lisaanalysistools-1.0.3/scripts/run-tests.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/scripts/to_conda.bash` & `lisaanalysistools-1.0.3/scripts/to_conda.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/setup.py` & `lisaanalysistools-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/src/Detector.cpp` & `lisaanalysistools-1.0.3/src/Detector.cpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.2/src/pycppdetector.cpp` & `lisaanalysistools-1.0.3/src/pycppdetector.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "include/Detector.hpp"
         ],
         "include_dirs": [
             "src",
             "./include",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "lisatools.cutils.detector",
         "sources": [
             "src/pycppdetector.pyx",
             "src/Detector.cpp"
         ]
@@ -47,18 +47,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -142,14 +142,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -203,14 +205,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -264,60 +268,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -400,14 +427,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1523,177 +1553,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1723,42 +1753,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9lisatools_6cutils_8detector_pycppDetector;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2260,30 +2290,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -3476,261 +3506,261 @@
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3739,29 +3769,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3772,15 +3802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3789,29 +3819,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3822,15 +3852,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3839,29 +3869,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3872,15 +3902,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3889,29 +3919,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3922,15 +3952,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3939,29 +3969,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3972,217 +4002,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4198,15 +4228,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4214,68 +4244,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4283,15 +4313,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4306,15 +4336,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4330,15 +4360,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4346,68 +4376,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4415,15 +4445,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4438,15 +4468,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4462,15 +4492,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4478,68 +4508,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4547,15 +4577,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4570,170 +4600,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8927,26 +8957,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-39lllatm/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
@@ -9231,41 +9261,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11913,18 +11943,18 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -11970,23 +12000,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `lisaanalysistools-1.0.2/src/pycppdetector.pyx` & `lisaanalysistools-1.0.3/src/pycppdetector.pyx`

 * *Files identical despite different names*

