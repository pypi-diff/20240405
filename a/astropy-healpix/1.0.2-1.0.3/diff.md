# Comparing `tmp/astropy_healpix-1.0.2.tar.gz` & `tmp/astropy_healpix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropy_healpix-1.0.2.tar", last modified: Tue Dec 12 15:43:26 2023, max compression
+gzip compressed data, was "astropy_healpix-1.0.3.tar", last modified: Fri Apr  5 21:13:40 2024, max compression
```

## Comparing `astropy_healpix-1.0.2.tar` & `astropy_healpix-1.0.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.704017 astropy_healpix-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.692017 astropy_healpix-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.692017 astropy_healpix-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-12-12 15:43:26.704017 astropy_healpix-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.696017 astropy_healpix-1.0.2/astropy_healpix/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix/_compiler.c
--rw-r--r--   0 runner    (1001) docker     (127)    15979 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/_core.c
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21722 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/healpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21815 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/high_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/interpolation.c
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/interpolation.h
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.696017 astropy_healpix-1.0.2/astropy_healpix/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/test_healpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/astropy_healpix/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.704017 astropy_healpix-1.0.2/astropy_healpix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-12 15:43:26.000000 astropy_healpix-1.0.2/astropy_healpix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.696017 astropy_healpix-1.0.2/cextern/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.700017 astropy_healpix-1.0.2/cextern/astrometry.net/
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/an-bool.h
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.c
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.h
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.inc
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.ph
--rw-r--r--   0 runner    (1001) docker     (127)    32656 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl.c
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl.inc
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/bl.ph
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/example.c
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/healpix-utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/healpix-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    40032 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/healpix.c
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/healpix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/keywords.h
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.c
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/os-features.h
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/permutedsort.c
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/permutedsort.h
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/qsort_reentrant.c
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/starutil.c
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/starutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/starutil.inc
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/stdint_msc.h
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/test_healpix-main.c
--rw-r--r--   0 runner    (1001) docker     (127)    21037 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/astrometry.net/test_healpix.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.700017 astropy_healpix-1.0.2/cextern/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/cextern/numpy/ieee754.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.704017 astropy_healpix-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.688017 astropy_healpix-1.0.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:26.704017 astropy_healpix-1.0.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/boundaries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/cone_search.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/healpy_compat.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/docs/references.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-12 15:43:26.708017 astropy_healpix-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2023-12-12 15:43:05.000000 astropy_healpix-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.812938 astropy_healpix-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.816938 astropy_healpix-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.816938 astropy_healpix-1.0.3/astropy_healpix/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix/_compiler.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/_core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21830 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/healpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21815 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/interpolation.c
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/interpolation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.820938 astropy_healpix-1.0.3/astropy_healpix/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/test_healpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/astropy_healpix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/astropy_healpix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 21:13:40.000000 astropy_healpix-1.0.3/astropy_healpix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.820938 astropy_healpix-1.0.3/cextern/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.824938 astropy_healpix-1.0.3/cextern/astrometry.net/
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/astrometry.net/CuTest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/astrometry.net/CuTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/astrometry.net/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/astrometry.net/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 21:13:24.000000 astropy_healpix-1.0.3/cextern/astrometry.net/an-bool.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.ph
+-rw-r--r--   0 runner    (1001) docker     (127)    32656 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/bl.ph
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/example.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/healpix-utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/healpix-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40032 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/healpix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/healpix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/keywords.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/os-features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/permutedsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/permutedsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/qsort_reentrant.c
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/starutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/starutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/starutil.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/stdint_msc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/test_healpix-main.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21037 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/astrometry.net/test_healpix.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.824938 astropy_healpix-1.0.3/cextern/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/cextern/numpy/ieee754.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.812938 astropy_healpix-1.0.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/boundaries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/cone_search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/healpy_compat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/docs/references.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-05 21:13:40.828938 astropy_healpix-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-05 21:13:25.000000 astropy_healpix-1.0.3/tox.ini
```

### Comparing `astropy_healpix-1.0.2/.github/workflows/ci_cron_weekly.yml` & `astropy_healpix-1.0.3/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/.github/workflows/ci_tests.yml` & `astropy_healpix-1.0.3/.github/workflows/ci_tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -81,10 +81,10 @@
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Test with tox
       run: |
         tox -e ${{ matrix.toxenv }}
     - name: Upload coverage to codecov
       if: "contains(matrix.toxenv, '-cov')"
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: ./coverage.xml
```

### Comparing `astropy_healpix-1.0.2/.gitignore` & `astropy_healpix-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/CHANGES.rst` & `astropy_healpix-1.0.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 .. _changes:
 
 *******
 Changes
 *******
 
+1.0.3 (2024-04-05)
+==================
+
+- Fixed compatibility with upcoming astropy 6.1.0 and numpy 2.0.0 releases. [#214, #215]
+
 1.0.2 (2023-12-12)
 ==================
 
 - lonlat_to_healpix now correctly returns -1 if the longitude or latitude is
   NaN or infinite. [#208]
 
 1.0.1 (2023-11-28)
```

### Comparing `astropy_healpix-1.0.2/LICENSE.md` & `astropy_healpix-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/PKG-INFO` & `astropy_healpix-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropy_healpix
-Version: 1.0.2
+Version: 1.0.3
 Summary: BSD-licensed HEALPix for Astropy
 Home-page: https://github.com/astropy/astropy-healpix
 Author: Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD 3-Clause
 Keywords: astronomy,astrophysics,astropy,healpix,coordinates
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astropy_healpix-1.0.2/README.rst` & `astropy_healpix-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/RELEASING.rst` & `astropy_healpix-1.0.3/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/_compiler.c` & `astropy_healpix-1.0.3/astropy_healpix/_compiler.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/_core.c` & `astropy_healpix-1.0.3/astropy_healpix/_core.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/bench.py` & `astropy_healpix-1.0.3/astropy_healpix/bench.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/conftest.py` & `astropy_healpix-1.0.3/astropy_healpix/conftest.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/core.py` & `astropy_healpix-1.0.3/astropy_healpix/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     'healpix_to_xyz',
     'bilinear_interpolation_weights',
     'interpolate_bilinear_lonlat',
     'boundaries_lonlat',
     'neighbours',
 ]
 
+_NUMPY_COPY_IF_NEEDED = False if np.__version__.startswith("1.") else None
+
 
 def _validate_order(order):
     # We also support upper-case, to support directly the values
     # ORDERING = {'RING', 'NESTED'} in FITS headers
     # This is currently undocumented in the docstrings.
     if order == 'nested' or order == 'NESTED':
         return 'nested'
@@ -365,16 +367,16 @@
     else:
         _validate_offset('y', dy)
 
     nside = np.asarray(nside, dtype=np.intc)
 
     lon, lat = func(healpix_index, nside, dx, dy)
 
-    lon = Longitude(lon, unit=u.rad, copy=False)
-    lat = Latitude(lat, unit=u.rad, copy=False)
+    lon = Longitude(lon, unit=u.rad, copy=_NUMPY_COPY_IF_NEEDED)
+    lat = Latitude(lat, unit=u.rad, copy=_NUMPY_COPY_IF_NEEDED)
 
     return lon, lat
 
 
 def lonlat_to_healpix(lon, lat, nside, return_offsets=False, order='ring'):
     """
     Convert longitudes/latitudes to HEALPix indices
```

### Comparing `astropy_healpix-1.0.2/astropy_healpix/healpy.py` & `astropy_healpix-1.0.3/astropy_healpix/healpy.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/high_level.py` & `astropy_healpix-1.0.3/astropy_healpix/high_level.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/interpolation.c` & `astropy_healpix-1.0.3/astropy_healpix/interpolation.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/setup_package.py` & `astropy_healpix-1.0.3/astropy_healpix/setup_package.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/tests/test_core.py` & `astropy_healpix-1.0.3/astropy_healpix/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/tests/test_healpy.py` & `astropy_healpix-1.0.3/astropy_healpix/tests/test_healpy.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/tests/test_high_level.py` & `astropy_healpix-1.0.3/astropy_healpix/tests/test_high_level.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/tests/test_utils.py` & `astropy_healpix-1.0.3/astropy_healpix/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix/utils.py` & `astropy_healpix-1.0.3/astropy_healpix/utils.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/astropy_healpix.egg-info/PKG-INFO` & `astropy_healpix-1.0.3/astropy_healpix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: astropy-healpix
-Version: 1.0.2
+Name: astropy_healpix
+Version: 1.0.3
 Summary: BSD-licensed HEALPix for Astropy
 Home-page: https://github.com/astropy/astropy-healpix
 Author: Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD 3-Clause
 Keywords: astronomy,astrophysics,astropy,healpix,coordinates
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astropy_healpix-1.0.2/astropy_healpix.egg-info/SOURCES.txt` & `astropy_healpix-1.0.3/astropy_healpix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/README.md` & `astropy_healpix-1.0.3/cextern/README.md`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/CuTest.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/CuTest.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/CuTest.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/CuTest.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/LICENSE` & `astropy_healpix-1.0.3/cextern/astrometry.net/LICENSE`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl-nl.inc` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl-nl.inc`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl.inc` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl.inc`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/bl.ph` & `astropy_healpix-1.0.3/cextern/astrometry.net/bl.ph`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/healpix-utils.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/healpix-utils.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/healpix-utils.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/healpix-utils.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/healpix.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/healpix.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/healpix.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/healpix.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/keywords.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/keywords.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/mathutil.inc` & `astropy_healpix-1.0.3/cextern/astrometry.net/mathutil.inc`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/os-features.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/os-features.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/permutedsort.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/permutedsort.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/permutedsort.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/permutedsort.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/qsort_reentrant.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/qsort_reentrant.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/starutil.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/starutil.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/starutil.inc` & `astropy_healpix-1.0.3/cextern/astrometry.net/starutil.inc`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/stdint_msc.h` & `astropy_healpix-1.0.3/cextern/astrometry.net/stdint_msc.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/test_healpix-main.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/test_healpix-main.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/astrometry.net/test_healpix.c` & `astropy_healpix-1.0.3/cextern/astrometry.net/test_healpix.c`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/cextern/numpy/ieee754.h` & `astropy_healpix-1.0.3/cextern/numpy/ieee754.h`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/Makefile` & `astropy_healpix-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/about.rst` & `astropy_healpix-1.0.3/docs/about.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/boundaries.rst` & `astropy_healpix-1.0.3/docs/boundaries.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/cone_search.rst` & `astropy_healpix-1.0.3/docs/cone_search.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/conf.py` & `astropy_healpix-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/coordinates.rst` & `astropy_healpix-1.0.3/docs/coordinates.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/getting_started.rst` & `astropy_healpix-1.0.3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/healpy_compat.rst` & `astropy_healpix-1.0.3/docs/healpy_compat.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/index.rst` & `astropy_healpix-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/installation.rst` & `astropy_healpix-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/interpolation.rst` & `astropy_healpix-1.0.3/docs/interpolation.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/make.bat` & `astropy_healpix-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/docs/performance.rst` & `astropy_healpix-1.0.3/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/environment-dev.yml` & `astropy_healpix-1.0.3/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/setup.cfg` & `astropy_healpix-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/setup.py` & `astropy_healpix-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `astropy_healpix-1.0.2/tox.ini` & `astropy_healpix-1.0.3/tox.ini`

 * *Files identical despite different names*

