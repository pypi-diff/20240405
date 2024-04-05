# Comparing `tmp/astroplan-0.9.tar.gz` & `tmp/astroplan-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroplan-0.9.tar", last modified: Thu Jul 27 17:53:53 2023, max compression
+gzip compressed data, was "astroplan-0.9.1.tar", last modified: Wed Sep 20 15:42:50 2023, max compression
```

## Comparing `astroplan-0.9.tar` & `astroplan-0.9.1.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866352 astroplan-0.9/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.851363 astroplan-0.9/.github/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.854565 astroplan-0.9/.github/workflows/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2438 2023-06-05 01:40:13.000000 astroplan-0.9/.github/workflows/ci_tests.yml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      622 2022-10-11 18:10:24.000000 astroplan-0.9/.gitignore
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:11:36.000000 astroplan-0.9/.gitmodules
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      641 2023-03-17 00:33:25.000000 astroplan-0.9/.readthedocs.yml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3392 2023-07-27 17:29:43.000000 astroplan-0.9/CHANGES.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      795 2023-01-10 18:38:43.000000 astroplan-0.9/CITATION.bib
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1497 2022-10-11 18:10:24.000000 astroplan-0.9/LICENSE.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      477 2022-10-11 18:10:24.000000 astroplan-0.9/LONG_DESCRIPTION.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      339 2023-01-10 18:38:43.000000 astroplan-0.9/MANIFEST.in
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2507 2023-07-27 17:53:53.866453 astroplan-0.9/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2095 2023-07-27 17:52:32.000000 astroplan-0.9/README.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.856802 astroplan-0.9/astroplan/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1147 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      613 2022-10-11 18:11:36.000000 astroplan-0.9/astroplan/_astropy_init.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1629 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/conftest.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    50032 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/constraints.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1230 2023-01-10 18:38:43.000000 astroplan-0.9/astroplan/exceptions.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1760 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/moon.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    81969 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/observer.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10665 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/periodic.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859337 astroplan-0.9/astroplan/plots/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      317 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4443 2022-10-11 19:38:39.000000 astroplan-0.9/astroplan/plots/finder.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2728 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/mplstyles.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    11776 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/plots/sky.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859617 astroplan-0.9/astroplan/plots/tests/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/__init__.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859770 astroplan-0.9/astroplan/plots/tests/baseline_images/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    17609 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/baseline_images/test_image_example.png
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1357 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/test_sky.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23885 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/plots/time_dependent.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    42960 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/scheduling.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      273 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/setup_package.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10255 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/target.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.861543 astroplan-0.9/astroplan/tests/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      768 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/coveragerc
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23079 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_constraints.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1726 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_moon.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    53640 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_observer.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3438 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_periodic.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    15796 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_scheduling.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2982 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_target.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1066 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_utils.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     8539 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/utils.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      335 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan/version.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.858574 astroplan-0.9/astroplan.egg-info/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2507 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1856 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2022-10-11 18:22:53.000000 astroplan-0.9/astroplan.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      214 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/requires.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       10 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/top_level.txt
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.863224 astroplan-0.9/docs/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4581 2022-10-11 18:10:24.000000 astroplan-0.9/docs/Makefile
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.852090 astroplan-0.9/docs/_templates/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.863707 astroplan-0.9/docs/_templates/autosummary/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/module.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      112 2022-10-11 18:10:24.000000 astroplan-0.9/docs/api.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2022-10-11 18:10:24.000000 astroplan-0.9/docs/changelog.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     7564 2023-07-27 17:29:43.000000 astroplan-0.9/docs/conf.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.864540 astroplan-0.9/docs/faq/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1268 2022-10-11 18:11:36.000000 astroplan-0.9/docs/faq/contribute.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5833 2022-10-11 19:38:39.000000 astroplan-0.9/docs/faq/iers.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      328 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3313 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/precision.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2658 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/terminology.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2877 2023-07-27 17:29:43.000000 astroplan-0.9/docs/getting_started.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2645 2023-07-27 17:52:32.000000 astroplan-0.9/docs/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1736 2023-07-27 17:29:43.000000 astroplan-0.9/docs/installation.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4513 2022-10-11 18:10:24.000000 astroplan-0.9/docs/make.bat
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      377 2022-10-11 18:11:36.000000 astroplan-0.9/docs/references.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2023-03-17 00:33:25.000000 astroplan-0.9/docs/rtd-pip-requirements
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866046 astroplan-0.9/docs/tutorials/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    20189 2023-03-17 00:33:25.000000 astroplan-0.9/docs/tutorials/constraints.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      620 2022-10-11 18:10:24.000000 astroplan-0.9/docs/tutorials/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10948 2022-10-11 19:38:39.000000 astroplan-0.9/docs/tutorials/periodic.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    40914 2023-07-27 17:05:05.000000 astroplan-0.9/docs/tutorials/plots.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    35038 2022-10-11 18:10:24.000000 astroplan-0.9/docs/tutorials/scheduling.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3402 2022-10-11 18:11:36.000000 astroplan-0.9/docs/tutorials/speed.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    19085 2023-07-27 17:12:03.000000 astroplan-0.9/docs/tutorials/summer_triangle.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866220 astroplan-0.9/licenses/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9/licenses/README.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      132 2022-10-11 18:11:36.000000 astroplan-0.9/pyproject.toml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1759 2023-07-27 17:53:53.866874 astroplan-0.9/setup.cfg
--rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)     1943 2022-10-11 18:11:36.000000 astroplan-0.9/setup.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2929 2023-01-10 19:27:48.000000 astroplan-0.9/tox.ini
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.999814 astroplan-0.9.1/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.980046 astroplan-0.9.1/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.983708 astroplan-0.9.1/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2438 2023-06-05 01:40:13.000000 astroplan-0.9.1/.github/workflows/ci_tests.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      622 2022-10-11 18:10:24.000000 astroplan-0.9.1/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:11:36.000000 astroplan-0.9.1/.gitmodules
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      641 2023-03-17 00:33:25.000000 astroplan-0.9.1/.readthedocs.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3536 2023-09-20 15:29:49.000000 astroplan-0.9.1/CHANGES.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      795 2023-01-10 18:38:43.000000 astroplan-0.9.1/CITATION.bib
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1497 2022-10-11 18:10:24.000000 astroplan-0.9.1/LICENSE.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      477 2022-10-11 18:10:24.000000 astroplan-0.9.1/LONG_DESCRIPTION.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      339 2023-01-10 18:38:43.000000 astroplan-0.9.1/MANIFEST.in
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3074 2023-09-20 15:42:49.999701 astroplan-0.9.1/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2095 2023-07-27 17:52:32.000000 astroplan-0.9.1/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.987681 astroplan-0.9.1/astroplan/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1147 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      613 2022-10-11 18:11:36.000000 astroplan-0.9.1/astroplan/_astropy_init.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1629 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/conftest.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    50112 2023-09-20 15:27:38.000000 astroplan-0.9.1/astroplan/constraints.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1230 2023-01-10 18:38:43.000000 astroplan-0.9.1/astroplan/exceptions.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1760 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/moon.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    81969 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/observer.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10665 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/periodic.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.990296 astroplan-0.9.1/astroplan/plots/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      317 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/plots/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4443 2022-10-11 19:38:39.000000 astroplan-0.9.1/astroplan/plots/finder.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2728 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/plots/mplstyles.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    11776 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/plots/sky.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.990658 astroplan-0.9.1/astroplan/plots/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/plots/tests/__init__.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.990850 astroplan-0.9.1/astroplan/plots/tests/baseline_images/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    17609 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/plots/tests/baseline_images/test_image_example.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1357 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/plots/tests/test_sky.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23885 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/plots/time_dependent.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    42960 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/scheduling.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      273 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/setup_package.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10255 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/target.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.993353 astroplan-0.9.1/astroplan/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      768 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/coveragerc
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23079 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/tests/test_constraints.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1726 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/test_moon.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    53640 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/tests/test_observer.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3438 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/test_periodic.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    15796 2023-07-27 17:29:43.000000 astroplan-0.9.1/astroplan/tests/test_scheduling.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2982 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/test_target.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1066 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/tests/test_utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     8539 2022-10-11 18:10:24.000000 astroplan-0.9.1/astroplan/utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      337 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.989036 astroplan-0.9.1/astroplan.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3074 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1900 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      214 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       10 2023-09-20 15:42:49.000000 astroplan-0.9.1/astroplan.egg-info/top_level.txt
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.995702 astroplan-0.9.1/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4581 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.995973 astroplan-0.9.1/docs/_templates/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.996570 astroplan-0.9.1/docs/_templates/autosummary/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1110 2023-09-20 15:27:38.000000 astroplan-0.9.1/docs/_templates/layout.html
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      112 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/api.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/changelog.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     7976 2023-09-20 15:27:38.000000 astroplan-0.9.1/docs/conf.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.997388 astroplan-0.9.1/docs/faq/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1268 2022-10-11 18:11:36.000000 astroplan-0.9.1/docs/faq/contribute.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5833 2022-10-11 19:38:39.000000 astroplan-0.9.1/docs/faq/iers.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      328 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/faq/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3313 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/faq/precision.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2658 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/faq/terminology.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2877 2023-07-27 17:29:43.000000 astroplan-0.9.1/docs/getting_started.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2588 2023-09-20 15:27:38.000000 astroplan-0.9.1/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1736 2023-07-27 17:29:43.000000 astroplan-0.9.1/docs/installation.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4513 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/make.bat
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      377 2022-10-11 18:11:36.000000 astroplan-0.9.1/docs/references.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      208 2023-09-20 15:27:38.000000 astroplan-0.9.1/docs/robots.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2023-03-17 00:33:25.000000 astroplan-0.9.1/docs/rtd-pip-requirements
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.998544 astroplan-0.9.1/docs/tutorials/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    20189 2023-03-17 00:33:25.000000 astroplan-0.9.1/docs/tutorials/constraints.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      620 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/tutorials/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10948 2022-10-11 19:38:39.000000 astroplan-0.9.1/docs/tutorials/periodic.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    40914 2023-07-27 17:05:05.000000 astroplan-0.9.1/docs/tutorials/plots.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    35038 2022-10-11 18:10:24.000000 astroplan-0.9.1/docs/tutorials/scheduling.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3402 2022-10-11 18:11:36.000000 astroplan-0.9.1/docs/tutorials/speed.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    19085 2023-07-27 17:12:03.000000 astroplan-0.9.1/docs/tutorials/summer_triangle.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-09-20 15:42:49.998716 astroplan-0.9.1/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9.1/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      132 2022-10-11 18:11:36.000000 astroplan-0.9.1/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1759 2023-09-20 15:42:50.000276 astroplan-0.9.1/setup.cfg
+-rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)     1943 2022-10-11 18:11:36.000000 astroplan-0.9.1/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2929 2023-01-10 19:27:48.000000 astroplan-0.9.1/tox.ini
```

### Comparing `astroplan-0.9/.github/workflows/ci_tests.yml` & `astroplan-0.9.1/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/.gitignore` & `astroplan-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/.readthedocs.yml` & `astroplan-0.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/CHANGES.rst` & `astroplan-0.9.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-0.9 (unreleased)
+0.9.1 (2023-09-20)
+------------------
+
+- Fix bug when ``FixedTarget`` objects are passed to methods that calculate
+  lunar coordinates. [#568]
+
+0.9 (2023-07-27)
 ----------------
 
 - Fix time range in ``months_observable`` to not be only in 2014. Function now
   accepts argument ``time_range`` and defaults to the current year. [#458]
 
 - Fix ``Observer`` not having longtitude, latitude, and elevation parameters
   as class attributes. They are now properties calculated from the ``location``.
```

### Comparing `astroplan-0.9/CITATION.bib` & `astroplan-0.9.1/CITATION.bib`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/LICENSE.rst` & `astroplan-0.9.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/PKG-INFO` & `astroplan-0.9.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: astroplan
-Version: 0.9
-Summary: Observation planning package for astronomers
-Home-page: https://github.com/astropy/astroplan
-Author: Astroplan developers
-Author-email: astropy-dev@googlegroups.com
-License: BSD
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: plotting
-License-File: LICENSE.rst
-
 astroplan
 =========
 
 Observation planning package for astronomers
 
 * Code: https://github.com/astropy/astroplan
 * Docs: https://astroplan.readthedocs.io/
```

### Comparing `astroplan-0.9/astroplan/__init__.py` & `astroplan-0.9.1/astroplan/__init__.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/_astropy_init.py` & `astroplan-0.9.1/astroplan/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/conftest.py` & `astroplan-0.9.1/astroplan/conftest.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/constraints.py` & `astroplan-0.9.1/astroplan/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,14 +546,15 @@
     def compute_constraint(self, times, observer, targets):
         # use get_body rather than get sun here, since
         # it returns the Sun's coordinates in an observer
         # centred frame, so the separation is as-seen
         # by the observer.
         # 'get_sun' returns ICRS coords.
         sun = get_body('sun', times, location=observer.location)
+        targets = get_skycoord(targets)
         solar_separation = sun.separation(targets)
 
         if self.min is None and self.max is not None:
             mask = self.max >= solar_separation
         elif self.max is None and self.min is not None:
             mask = self.min <= solar_separation
         elif self.min is not None and self.max is not None:
@@ -591,14 +592,15 @@
 
     def compute_constraint(self, times, observer, targets):
         moon = get_body("moon", times, location=observer.location, ephemeris=self.ephemeris)
         # note to future editors - the order matters here
         # moon.separation(targets) is NOT the same as targets.separation(moon)
         # the former calculates the separation in the frame of the moon coord
         # which is GCRS, and that is what we want.
+        targets = get_skycoord(targets)
         moon_separation = moon.separation(targets)
 
         if self.min is None and self.max is not None:
             mask = self.max >= moon_separation
         elif self.max is None and self.min is not None:
             mask = self.min <= moon_separation
         elif self.min is not None and self.max is not None:
```

### Comparing `astroplan-0.9/astroplan/exceptions.py` & `astroplan-0.9.1/astroplan/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/moon.py` & `astroplan-0.9.1/astroplan/moon.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/observer.py` & `astroplan-0.9.1/astroplan/observer.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/periodic.py` & `astroplan-0.9.1/astroplan/periodic.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/finder.py` & `astroplan-0.9.1/astroplan/plots/finder.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/mplstyles.py` & `astroplan-0.9.1/astroplan/plots/mplstyles.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/sky.py` & `astroplan-0.9.1/astroplan/plots/sky.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/tests/baseline_images/test_image_example.png` & `astroplan-0.9.1/astroplan/plots/tests/baseline_images/test_image_example.png`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/tests/test_sky.py` & `astroplan-0.9.1/astroplan/plots/tests/test_sky.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/plots/time_dependent.py` & `astroplan-0.9.1/astroplan/plots/time_dependent.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/scheduling.py` & `astroplan-0.9.1/astroplan/scheduling.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/target.py` & `astroplan-0.9.1/astroplan/target.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/coveragerc` & `astroplan-0.9.1/astroplan/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_constraints.py` & `astroplan-0.9.1/astroplan/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_moon.py` & `astroplan-0.9.1/astroplan/tests/test_moon.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_observer.py` & `astroplan-0.9.1/astroplan/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_periodic.py` & `astroplan-0.9.1/astroplan/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_scheduling.py` & `astroplan-0.9.1/astroplan/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_target.py` & `astroplan-0.9.1/astroplan/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/tests/test_utils.py` & `astroplan-0.9.1/astroplan/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan/utils.py` & `astroplan-0.9.1/astroplan/utils.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/astroplan.egg-info/PKG-INFO` & `astroplan-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 Metadata-Version: 2.1
 Name: astroplan
-Version: 0.9
+Version: 0.9.1
 Summary: Observation planning package for astronomers
 Home-page: https://github.com/astropy/astroplan
 Author: Astroplan developers
 Author-email: astropy-dev@googlegroups.com
 License: BSD
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.rst
+Requires-Dist: numpy>=1.17
+Requires-Dist: astropy>=4
+Requires-Dist: pytz
+Requires-Dist: six
 Provides-Extra: all
+Requires-Dist: matplotlib>=1.4; extra == "all"
+Requires-Dist: astroquery; extra == "all"
 Provides-Extra: test
+Requires-Dist: pytest-astropy; extra == "test"
+Requires-Dist: pytest-mpl; extra == "test"
 Provides-Extra: docs
+Requires-Dist: sphinx-astropy[confv2]; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: matplotlib>=1.4; extra == "docs"
+Requires-Dist: astroquery; extra == "docs"
 Provides-Extra: plotting
-License-File: LICENSE.rst
+Requires-Dist: astroquery; extra == "plotting"
+Requires-Dist: matplotlib>=1.4; extra == "plotting"
 
 astroplan
 =========
 
 Observation planning package for astronomers
 
 * Code: https://github.com/astropy/astroplan
```

### Comparing `astroplan-0.9/astroplan.egg-info/SOURCES.txt` & `astroplan-0.9.1/astroplan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 docs/changelog.rst
 docs/conf.py
 docs/getting_started.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/references.txt
+docs/robots.txt
 docs/rtd-pip-requirements
+docs/_templates/layout.html
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/faq/contribute.rst
 docs/faq/iers.rst
 docs/faq/index.rst
 docs/faq/precision.rst
```

### Comparing `astroplan-0.9/docs/Makefile` & `astroplan-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/conf.py` & `astroplan-0.9.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # Note that not all possible configuration values are present in this file.
 #
 # All configuration values have a default. Some values are defined in
 # the global Astropy configuration which is loaded here before anything else.
 # See astropy.sphinx.conf for which values are set there.
 
 from configparser import ConfigParser
-from astroplan import __version__
 import sys
 import datetime
+from importlib import metadata
 
 try:
     from sphinx_astropy.conf.v2 import *  # noqa
 except ImportError:
     print('ERROR: the documentation requires the sphinx-astropy package to '
           'be installed')
     sys.exit(1)
@@ -66,18 +66,25 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 __import__(project)
 package = sys.modules[project]
 
-# The short X.Y version.
-version = package.__version__.split('-', 1)[0]
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+
 # The full version, including alpha/beta/rc tags.
-release = package.__version__
+release = metadata.version(project)
+# The short X.Y version.
+version = ".".join(release.split(".")[:2])
+
+# Only include dev docs in dev version.
+dev = "dev" in release
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # A NOTE ON HTML THEMES
 # The global astropy configuration uses a custom theme, 'bootstrap-astropy',
 # which is installed along with astropy. A different theme can be used or
@@ -169,17 +176,14 @@
 ]
 linkcheck_timeout = 180
 linkcheck_anchors = False
 
 # -- Turn on nitpicky mode for sphinx (to warn about references not found) ----
 nitpicky = True
 
-release = __version__
-dev = "dev" in release
-
 html_copy_source = False
 
 html_theme_options.update(  # noqa: F405
     {
         "github_url": "https://github.com/astropy/astroplan",
         "external_links": [
             {"name": "astropy docs", "url": "https://docs.astropy.org/en/stable/"},
@@ -194,14 +198,19 @@
     "is_development": dev,
     "github_user": "astropy",
     "github_repo": "astroplan",
     "github_version": "main",
     "doc_path": "docs",
 }
 
+# Add any extra paths that contain custom files (such as robots.txt or
+# .htaccess) here, relative to this directory. These files are copied
+# directly to the root of the documentation.
+html_extra_path = ["robots.txt"]
+
 #
 # Some warnings are impossible to suppress, and you can list specific references
 # that should be ignored in a nitpick-exceptions file which should be inside
 # the docs/ directory. The format of the file should be:
 #
 # <type> <class>
 #
```

### Comparing `astroplan-0.9/docs/faq/contribute.rst` & `astroplan-0.9.1/docs/faq/contribute.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/faq/iers.rst` & `astroplan-0.9.1/docs/faq/iers.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/faq/precision.rst` & `astroplan-0.9.1/docs/faq/precision.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/faq/terminology.rst` & `astroplan-0.9.1/docs/faq/terminology.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/getting_started.rst` & `astroplan-0.9.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/index.rst` & `astroplan-0.9.1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,34 +27,29 @@
 * `Docs <https://astroplan.readthedocs.io/>`_
 * `Issues <https://github.com/astropy/astroplan/issues>`_
 
 License: BSD-3
 
 .. _astroplan_docs:
 
-General Documentation
-=====================
+Documentation
+=============
 
 .. toctree::
    :maxdepth: 2
 
    installation
    getting_started
    tutorials/index
    faq/index
    api
    changelog
 
-.. _astroplan_authors:
-
-Authors
-=======
-
 Maintainers
------------
++++++++++++
 * `Brett Morris, including contributions from Google Summer of Code 2015 <https://www.google-melange.com/gsoc/project/details/google/gsoc2015/bmmorris/5707702298738688>`_
 
 Attribution
 +++++++++++
 
 If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_:
```

### Comparing `astroplan-0.9/docs/installation.rst` & `astroplan-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/make.bat` & `astroplan-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/constraints.rst` & `astroplan-0.9.1/docs/tutorials/constraints.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/index.rst` & `astroplan-0.9.1/docs/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/periodic.rst` & `astroplan-0.9.1/docs/tutorials/periodic.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/plots.rst` & `astroplan-0.9.1/docs/tutorials/plots.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/scheduling.rst` & `astroplan-0.9.1/docs/tutorials/scheduling.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/speed.rst` & `astroplan-0.9.1/docs/tutorials/speed.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/docs/tutorials/summer_triangle.rst` & `astroplan-0.9.1/docs/tutorials/summer_triangle.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/setup.cfg` & `astroplan-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/setup.py` & `astroplan-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.9/tox.ini` & `astroplan-0.9.1/tox.ini`

 * *Files identical despite different names*

