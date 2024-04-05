# Comparing `tmp/lcviz-0.2.0.tar.gz` & `tmp/lcviz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcviz-0.2.0.tar", last modified: Mon Feb 26 14:59:15 2024, max compression
+gzip compressed data, was "lcviz-0.3.0.tar", last modified: Fri Apr  5 19:19:08 2024, max compression
```

## Comparing `lcviz-0.2.0.tar` & `lcviz-0.3.0.tar`

### file list

```diff
@@ -1,122 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.076955 lcviz-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-26 14:59:01.000000 lcviz-0.2.0/.bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-26 14:59:01.000000 lcviz-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.056955 lcviz-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.064955 lcviz-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-26 14:59:01.000000 lcviz-0.2.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-26 14:59:01.000000 lcviz-0.2.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-26 14:59:01.000000 lcviz-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-26 14:59:01.000000 lcviz-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-26 14:59:01.000000 lcviz-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-26 14:59:01.000000 lcviz-0.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-26 14:59:01.000000 lcviz-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-26 14:59:01.000000 lcviz-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-26 14:59:01.000000 lcviz-0.2.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-26 14:59:01.000000 lcviz-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-02-26 14:59:15.076955 lcviz-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-02-26 14:59:01.000000 lcviz-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-26 14:59:01.000000 lcviz-0.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.064955 lcviz-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.064955 lcviz-0.2.0/docs/logos/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/logos/lcviz.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/logos/lcviz.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/logos/lcviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.064955 lcviz-0.2.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-26 14:59:01.000000 lcviz-0.2.0/docs/reference/api_plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/components/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/components/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/components/plugin_ephemeris_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/data/
--rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/data/HAT-P-11_Kepler_Q0_snippet.fits
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/data/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/data/icons/viewer_clone.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/lcviz_style.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/marks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/plugins/binning/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/binning/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/binning/binning.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.068955 lcviz-0.2.0/lcviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/coords_info/coords_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/ephemeris/ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/ephemeris/ephemeris.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/export_plot/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/export_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/export_plot/export_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/flatten/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flatten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flatten/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flatten/flatten.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/flux_column/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flux_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flux_column/flux_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/flux_column/flux_column.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/frequency_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/frequency_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/frequency_analysis/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/frequency_analysis/frequency_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/markers/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/metadata_viewer/metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/plot_options/plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.072955 lcviz-0.2.0/lcviz/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.076955 lcviz-0.2.0/lcviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_flux_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_plugin_plot_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-26 14:59:14.000000 lcviz-0.2.0/lcviz/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-02-26 14:59:01.000000 lcviz-0.2.0/lcviz/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.076955 lcviz-0.2.0/lcviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-02-26 14:59:15.000000 lcviz-0.2.0/lcviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-26 14:59:15.000000 lcviz-0.2.0/lcviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:59:15.000000 lcviz-0.2.0/lcviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:59:14.000000 lcviz-0.2.0/lcviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-26 14:59:15.000000 lcviz-0.2.0/lcviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 14:59:15.000000 lcviz-0.2.0/lcviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:59:15.076955 lcviz-0.2.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-02-26 14:59:01.000000 lcviz-0.2.0/notebooks/ConfigHelperHelper.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-26 14:59:01.000000 lcviz-0.2.0/notebooks/LCvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-26 14:59:01.000000 lcviz-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 14:59:01.000000 lcviz-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:59:15.076955 lcviz-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      614 2024-02-26 14:59:01.000000 lcviz-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-26 14:59:01.000000 lcviz-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.725497 lcviz-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 19:18:59.000000 lcviz-0.3.0/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 19:18:59.000000 lcviz-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.709497 lcviz-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-05 19:18:59.000000 lcviz-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.709497 lcviz-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 19:18:59.000000 lcviz-0.3.0/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-05 19:18:59.000000 lcviz-0.3.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-05 19:18:59.000000 lcviz-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 19:18:59.000000 lcviz-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 19:18:59.000000 lcviz-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-05 19:18:59.000000 lcviz-0.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-05 19:18:59.000000 lcviz-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 19:18:59.000000 lcviz-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 19:18:59.000000 lcviz-0.3.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 19:18:59.000000 lcviz-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-05 19:19:08.725497 lcviz-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-05 19:18:59.000000 lcviz-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 19:18:59.000000 lcviz-0.3.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.713497 lcviz-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.713497 lcviz-0.3.0/docs/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/logos/lcviz.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/logos/lcviz.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/logos/lcviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.713497 lcviz-0.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-05 19:18:59.000000 lcviz-0.3.0/docs/reference/api_plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.713497 lcviz-0.3.0/lcviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/components/plugin_ephemeris_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/data/HAT-P-11_Kepler_Q0_snippet.fits
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/data/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/data/icons/viewer_clone.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/lcviz_style.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/binning/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/binning/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/binning/binning.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/coords_info/coords_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24667 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/ephemeris/ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/ephemeris/ephemeris.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/export/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.717497 lcviz-0.3.0/lcviz/plugins/flatten/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flatten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flatten/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flatten/flatten.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/flux_column/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flux_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flux_column/flux_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/flux_column/flux_column.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/frequency_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/frequency_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/frequency_analysis/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/frequency_analysis/frequency_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/markers/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/metadata_viewer/metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/plot_options/plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/subset_plugin/subset_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.721497 lcviz-0.3.0/lcviz/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.725497 lcviz-0.3.0/lcviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_flux_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_plugin_plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_tray_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-05 19:18:59.000000 lcviz-0.3.0/lcviz/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.725497 lcviz-0.3.0/lcviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 19:19:08.000000 lcviz-0.3.0/lcviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:19:08.725497 lcviz-0.3.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-05 19:18:59.000000 lcviz-0.3.0/notebooks/ConfigHelperHelper.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-05 19:18:59.000000 lcviz-0.3.0/notebooks/LCvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-05 19:18:59.000000 lcviz-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 19:18:59.000000 lcviz-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:19:08.725497 lcviz-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      614 2024-04-05 19:18:59.000000 lcviz-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-05 19:18:59.000000 lcviz-0.3.0/tox.ini
```

### Comparing `lcviz-0.2.0/.github/workflows/ci_cron_weekly.yml` & `lcviz-0.3.0/.github/workflows/ci_cron_weekly.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 jobs:
   # The linkcheck job tests that the links in the docs point to real places
   # The if statement is to prevent cron from running on forks.
   linkcheck:
     runs-on: ubuntu-latest
     if: github.repository == 'spacetelescope/lcviz'
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python to build docs with sphinx
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Check links in docs using tox
@@ -31,19 +31,19 @@
 
   ci_cron_tests:
     name: Python 3.10 with latest dev versions of key dependencies
     runs-on: ubuntu-latest
     if: github.repository == 'spacetelescope/lcviz'
     steps:
     - name: Checkout code
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
     - name: Test with tox
```

### Comparing `lcviz-0.2.0/.github/workflows/ci_workflows.yml` & `lcviz-0.3.0/.github/workflows/ci_workflows.yml`

 * *Files 0% similar despite different names*

```diff
@@ -70,24 +70,24 @@
             python: '3.11'
             toxenv: py311-test-devdeps
             toxposargs: --remote-data --run-slow
             allow_failure: true
 
     steps:
     - name: Checkout code
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up python ${{ matrix.python }} on ${{ matrix.os }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python }}
     - name: Install base dependencies
       run: python -m pip install --upgrade pip tox
     - name: Test/run with tox
       run: tox -e ${{ matrix.toxenv }} -- ${{ matrix.toxposargs }}
     - name: Upload coverage to codecov
       if: "contains(matrix.toxenv, '-cov')"
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: ./coverage.xml
         verbose: true
```

### Comparing `lcviz-0.2.0/.github/workflows/publish.yml` & `lcviz-0.3.0/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if: github.repository == 'spacetelescope/lcviz'
 
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: 3.9
 
     - name: Install python-build and twine
       run: python -m pip install build "twine>=3.3"
 
     - name: Build package
```

### Comparing `lcviz-0.2.0/.gitignore` & `lcviz-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/.readthedocs.yaml` & `lcviz-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/CHANGES.rst` & `lcviz-0.3.0/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-0.2.0 - unreleased
+0.4.0 - unreleased
+------------------
+
+0.3.0 - (04-05-2024)
+--------------------
+
+* Ability to create additional viewers. [#94]
+* Updates to use jdaviz 3.9. [#68]
+
+0.2.0 (02-26-2024)
 ------------------
 
 * Clone viewer tool. [#74, #91]
 
 * Flux column plugin to choose which column is treated as the flux column for each dataset. [#77]
 
 * Flatten plugin no longer creates new data entries, but instead appends a new column to the input
```

### Comparing `lcviz-0.2.0/CODE_OF_CONDUCT.md` & `lcviz-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/CONTRIBUTING.md` & `lcviz-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/LICENSE.rst` & `lcviz-0.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/PKG-INFO` & `lcviz-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcviz
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Jdaviz-based light curve analysis and visualization tool
 Author-email: JDADF Developers <kconroy@stsci.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Association of Universities for Research in Astronomy.
         All rights reserved.
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: astropy>=5.2
-Requires-Dist: jdaviz==3.8.*
+Requires-Dist: jdaviz==3.9.*
 Requires-Dist: lightkurve>=2.4.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-astropy; extra == "test"
 Requires-Dist: pytest-tornasync; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy[confv2]>=1.9.1; extra == "docs"
```

### Comparing `lcviz-0.2.0/README.rst` & `lcviz-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/conftest.py` & `lcviz-0.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/Makefile` & `lcviz-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/conf.py` & `lcviz-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/index.rst` & `lcviz-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/installation.rst` & `lcviz-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/logos/lcviz.ico` & `lcviz-0.3.0/docs/logos/lcviz.ico`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/logos/lcviz.svg` & `lcviz-0.3.0/docs/logos/lcviz.svg`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/logos/lcviz_icon.svg` & `lcviz-0.3.0/docs/logos/lcviz_icon.svg`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/make.bat` & `lcviz-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/docs/plugins.rst` & `lcviz-0.3.0/docs/plugins.rst`

 * *Files 1% similar despite different names*

```diff
@@ -314,37 +314,37 @@
 .. seealso::
 
   This plugin uses the following ``lightkurve`` implementations:
 
   * :meth:`lightkurve.LightCurve.bin`
 
 
-.. _export-plot:
+.. _export:
 
-Export Plot
-===========
+Export
+======
 
 This plugin allows exporting the plot in a given viewer to various image formats.
 
 
 .. admonition:: User API Example
     :class: dropdown
 
-    See the :class:`~lcviz.plugins.export_plot.export_plot.ExportViewer` user API documentation for more details.
+    See the :class:`~lcviz.plugins.export.export.Export` user API documentation for more details.
 
     .. code-block:: python
 
       from lcviz import LCviz
       lc = search_lightcurve("HAT-P-11", mission="Kepler",
                              cadence="long", quarter=10).download().flatten()
       lcviz = LCviz()
       lcviz.load_data(lc)
       lcviz.show()
 
-      export = lcviz.plugins['Export Plot']
-      export.save_figure('test.png')
+      export = lcviz.plugins['Export']
+      export.export('test.png')
 
 
 .. seealso::
 
     :ref:`Jdaviz Export Plot <jdaviz:imviz-export-plot>`
-        Jdaviz documentation on the Export Plot plugin.
+        Jdaviz documentation on the Export plugin.
```

### Comparing `lcviz-0.2.0/docs/reference/api_plugins.rst` & `lcviz-0.3.0/docs/reference/api_plugins.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 .. automodapi:: lcviz.plugins.binning.binning
   :no-inheritance-diagram:
 
 .. automodapi:: lcviz.plugins.ephemeris.ephemeris
   :no-inheritance-diagram:
 
-.. automodapi:: lcviz.plugins.export_plot.export_plot
+.. automodapi:: lcviz.plugins.export.export
   :no-inheritance-diagram:
 
 .. automodapi:: lcviz.plugins.flatten.flatten
   :no-inheritance-diagram:
 
 .. automodapi:: lcviz.plugins.frequency_analysis.frequency_analysis
   :no-inheritance-diagram:
```

### Comparing `lcviz-0.2.0/lcviz/__init__.py` & `lcviz-0.3.0/lcviz/__init__.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/components/components.py` & `lcviz-0.3.0/lcviz/components/components.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/components/plugin_ephemeris_select.vue` & `lcviz-0.3.0/lcviz/components/plugin_ephemeris_select.vue`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/conftest.py` & `lcviz-0.3.0/lcviz/conftest.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/data/HAT-P-11_Kepler_Q0_snippet.fits` & `lcviz-0.3.0/lcviz/data/HAT-P-11_Kepler_Q0_snippet.fits`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/events.py` & `lcviz-0.3.0/lcviz/events.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/helper.py` & `lcviz-0.3.0/lcviz/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,29 @@
 import os
 
 from lightkurve import LightCurve
 
 from glue.core.component_id import ComponentID
 from glue.core.link_helpers import LinkSame
 from jdaviz.core.helpers import ConfigHelper
+from lcviz.viewers import TimeScatterView
 
 __all__ = ['LCviz']
 
-_default_time_viewer_reference_name = 'flux-vs-time'
-
 custom_components = {'plugin-ephemeris-select': 'components/plugin_ephemeris_select.vue'}
 
 # Register pure vue component. This allows us to do recursive component instantiation only in the
 # vue component file
 for name, path in custom_components.items():
     ipyvue.register_component_from_file(None, name,
                                         os.path.join(os.path.dirname(__file__), path))
 
 
 def _get_range_subset_bounds(self, subset_state, *args, **kwargs):
-    # Instead of overriding the jdaviz version of this method on jdaviz.Application,
-    # we could put in jdaviz by (1) checking if helper has a
-    # _default_time_viewer_reference_name, (2) using the LCviz version if so, and (3)
-    # using the jdaviz version otherwise.
-    viewer = self.get_viewer(self._jdaviz_helper._default_time_viewer_reference_name)
+    viewer = self._jdaviz_helper.default_time_viewer._obj
     light_curve = viewer.data()[0]
     reference_time = light_curve.meta['reference_time']
     if viewer:
         # TODO: use display units once implemented in Glue for ScatterViewer
         # units = u.Unit(viewer.state.x_display_unit)
         units = u.Unit(viewer.time_unit)
     else:  # pragma: no cover
@@ -67,46 +62,41 @@
         'settings': {'configuration': 'lcviz',
                      'visible': {'menu_bar': False,
                                  'toolbar': True,
                                  'tray': True,
                                  'tab_headers': True},
                      'dense_toolbar': False,
                      'context': {'notebook': {'max_height': '600px'}}},
-        'toolbar': ['g-data-tools', 'g-subset-tools', 'lcviz-coords-info'],
+        'toolbar': ['g-data-tools', 'g-subset-tools', 'g-viewer-creator', 'lcviz-coords-info'],
         'tray': ['lcviz-metadata-viewer', 'flux-column',
                  'lcviz-plot-options', 'lcviz-subset-plugin',
                  'lcviz-markers', 'flatten', 'frequency-analysis', 'ephemeris',
-                 'binning', 'lcviz-export-plot'],
+                 'binning', 'lcviz-export'],
         'viewer_area': [{'container': 'col',
                          'children': [{'container': 'row',
                                        'viewers': [{'name': 'flux-vs-time',
                                                     'plot': 'lcviz-time-viewer',
                                                     'reference': 'flux-vs-time'}]}]}]}
 
     _component_ids = {}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._default_time_viewer_reference_name = _default_time_viewer_reference_name
 
         # override jdaviz behavior to support temporal subsets
         self.app._get_range_subset_bounds = (
             lambda *args, **kwargs: _get_range_subset_bounds(self.app, *args, **kwargs)
         )
 
         self.app._link_new_data = (
             lambda *args, **kwargs: _link_new_data(self.app, *args, **kwargs)
         )
 
         # inject custom css from lcviz_style.vue (on top of jdaviz styles)
-        if hasattr(self.app, '_add_style'):
-            # will be guaranteed after jdaviz 3.9
-            self.app._add_style((__file__, 'lcviz_style.vue'))
-        else:
-            self.app.set_style_template_file((__file__, 'lcviz_style.vue'))
+        self.app._add_style((__file__, 'lcviz_style.vue'))
 
         # set the link to read the docs
         self.app.docs_link = "https://lcviz.readthedocs.io"
 
     def load_data(self, data, data_label=None):
         """
         Load data into LCviz.
@@ -148,14 +138,47 @@
         Returns
         -------
         data : cls
             Data is returned as type cls with subsets applied.
         """
         return super()._get_data(data_label=data_label, mask_subset=subset, cls=cls)
 
+    @property
+    def default_time_viewer(self):
+        tvs = [viewer for vid, viewer in self.app._viewer_store.items()
+               if isinstance(viewer, TimeScatterView)]
+        if not len(tvs):
+            raise ValueError("no time viewers exist")
+        return tvs[0].user_api
+
+    @property
+    def _tray_tools(self):
+        """
+        Access API objects for plugins in the app toolbar.
+
+        Returns
+        -------
+        plugins : dict
+            dict of plugin objects
+        """
+        # TODO: provide user-friendly labels, user API, and move upstream to be public
+        # for now this is just useful for dev-debugging access to toolbar entries
+        from ipywidgets.widgets import widget_serialization
+        return {item['name']: widget_serialization['from_json'](item['widget'], None)
+                for item in self.app.state.tool_items}
+
+    def _get_clone_viewer_reference(self, reference):
+        base_name = reference.split("[")[0]
+        name = base_name
+        ind = 0
+        while name in self.viewers.keys():
+            ind += 1
+            name = f"{base_name}[{ind}]"
+        return name
+
     def _phase_comp_lbl(self, component):
         return f'phase:{component}'
 
     def _set_data_component(self, data, component_label, values):
         if component_label in self._component_ids:
             component_id = self._component_ids[component_label]
         else:
```

### Comparing `lcviz-0.2.0/lcviz/marks.py` & `lcviz-0.3.0/lcviz/marks.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/parsers.py` & `lcviz-0.3.0/lcviz/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from glue.config import data_translator
 from jdaviz.core.registries import data_parser_registry
 import lightkurve
 
+from lcviz.viewers import PhaseScatterView, TimeScatterView
+
 __all__ = ["light_curve_parser"]
 
 
 @data_parser_registry("light_curve_parser")
 def light_curve_parser(app, file_obj, data_label=None, show_in_viewer=True, **kwargs):
-    time_viewer_reference_name = app._jdaviz_helper._default_time_viewer_reference_name
-
     # load local FITS file from disk by its path:
     if isinstance(file_obj, str) and os.path.exists(file_obj):
         if data_label is None:
             data_label = os.path.splitext(os.path.basename(file_obj))[0]
 
         # read the light curve:
         light_curve = lightkurve.read(file_obj)
@@ -38,20 +38,19 @@
             light_curve['flux:orig_err'] = light_curve['flux_err']
         light_curve.meta['FLUX_ORIGIN'] = 'flux:orig'
 
     data = _data_with_reftime(app, light_curve)
     app.add_data(data, new_data_label)
 
     if show_in_viewer:
-        app.add_data_to_viewer(time_viewer_reference_name, new_data_label)
-
-        # add to any known phase viewers
-        ephem_plugin = app._jdaviz_helper.plugins.get('Ephemeris', None)
-        if ephem_plugin is not None:
-            for viewer_id in ephem_plugin._obj.phase_viewer_ids:
+        # add to any known time/phase viewers
+        for viewer_id, viewer in app._viewer_store.items():
+            if isinstance(viewer, TimeScatterView):
+                app.add_data_to_viewer(viewer_id, new_data_label)
+            elif isinstance(viewer, PhaseScatterView):
                 app.add_data_to_viewer(viewer_id, new_data_label)
 
 
 def _data_with_reftime(app, light_curve):
     # grab the first-found reference time in the data collection:
     ff_reference_time = None
     for existing_data in app.data_collection:
```

### Comparing `lcviz-0.2.0/lcviz/plugins/__init__.py` & `lcviz-0.3.0/lcviz/plugins/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from .binning.binning import *  # noqa
+from .viewer_creator.viewer_creator import *  # noqa
 from .coords_info.coords_info import *  # noqa
+
+from .binning.binning import *  # noqa
 from .ephemeris.ephemeris import *  # noqa
-from .export_plot.export_plot import *  # noqa
+from .export.export import *  # noqa
 from .flatten.flatten import *  # noqa
 from .flux_column.flux_column import *  # noqa
 from .frequency_analysis.frequency_analysis import *  # noqa
 from .markers.markers import *  # noqa
 from .metadata_viewer.metadata_viewer import *  # noqa
 from .plot_options.plot_options import *  # noqa
 from .subset_plugin.subset_plugin import *  # noqa
```

### Comparing `lcviz-0.2.0/lcviz/plugins/binning/binning.py` & `lcviz-0.3.0/lcviz/plugins/binning/binning.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import numpy as np
-from time import time
 from astropy.time import Time
-from traitlets import Bool, Float, observe
+from traitlets import Bool, observe
 from glue.config import data_translator
 
 from jdaviz.core.custom_traitlets import IntHandleEmpty
 from jdaviz.core.events import (ViewerAddedMessage, ViewerRemovedMessage)
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         DatasetSelectMixin, AddResultsMixin,
                                         skip_if_no_updates_since_last_active,
-                                        with_spinner)
+                                        with_spinner, with_temp_disable)
 from jdaviz.core.user_api import PluginUserApi
 
 from lcviz.components import FluxColumnSelectMixin
 from lcviz.events import EphemerisChangedMessage
-from lcviz.helper import _default_time_viewer_reference_name
 from lcviz.marks import LivePreviewBinning
 from lcviz.parsers import _data_with_reftime
+from lcviz.viewers import TimeScatterView, PhaseScatterView
 from lcviz.components import EphemerisSelectMixin
 
 
 __all__ = ['Binning']
 
 
 @tray_registry('binning', label="Binning")
@@ -50,29 +48,27 @@
     uses_active_status = Bool(True).tag(sync=True)
 
     show_live_preview = Bool(True).tag(sync=True)
 
     n_bins = IntHandleEmpty(100).tag(sync=True)
     bin_enabled = Bool(True).tag(sync=True)
 
-    last_live_time = Float(0).tag(sync=True)
-    previews_temp_disable = Bool(False).tag(sync=True)
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._set_results_viewer()
 
         # TODO: replace with add_filter('not_from_this_plugin') if upstream PR accepted/released
         # https://github.com/spacetelescope/jdaviz/pull/2239
         def not_from_binning_plugin(data):
             return data.meta.get('Plugin', None) != self.__class__.__name__
         self.dataset.add_filter(not_from_binning_plugin)
 
-        self.hub.subscribe(self, ViewerAddedMessage, handler=self._set_results_viewer)
+        # TODO: viewer added also needs to repopulate marks
+        self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_add_viewer)
         self.hub.subscribe(self, ViewerRemovedMessage, handler=self._set_results_viewer)
         self.hub.subscribe(self, EphemerisChangedMessage, handler=self._on_ephemeris_update)
 
     @property
     def user_api(self):
         expose = ['show_live_preview', 'dataset', 'ephemeris', 'input_lc',
                   'n_bins', 'add_results', 'bin']
@@ -91,23 +87,23 @@
     @property
     def input_lc(self):
         return self.ephemeris.get_data_for_dataset(self.dataset)
 
     @property
     def marks(self):
         marks = {}
-        for id, viewer in self.app._viewer_store.items():
+        for viewer in self.app._viewer_store.values():
             for mark in viewer.figure.marks:
                 if isinstance(mark, LivePreviewBinning):
-                    marks[id] = mark
+                    marks[viewer.reference] = mark
                     break
             else:
                 mark = LivePreviewBinning(viewer, visible=self.is_active)
                 viewer.figure.marks = viewer.figure.marks + [mark]
-                marks[id] = mark
+                marks[viewer.reference] = mark
         return marks
 
     def _clear_marks(self):
         for mark in self.marks.values():
             if mark.visible:
                 mark.clear()
                 mark.visible = False
@@ -125,56 +121,58 @@
     @observe("ephemeris_selected")
     def _set_results_viewer(self, event={}):
         if not hasattr(self, 'ephemeris'):
             return
 
         def viewer_filter(viewer):
             if self.ephemeris_selected in self.ephemeris._manual_options:
-                return viewer.reference == _default_time_viewer_reference_name
-            if 'flux-vs-phase:' not in viewer.reference:
+                return isinstance(viewer, TimeScatterView)
+            if not isinstance(viewer, PhaseScatterView):
                 # ephemeris selected, but no active phase viewers
                 return False
-            return viewer.reference.split('flux-vs-phase:')[1] == self.ephemeris_selected
+            return viewer._ephemeris_component == self.ephemeris_selected
 
         self.add_results.viewer.filters = [viewer_filter]
 
+    def _on_add_viewer(self, msg):
+        self._set_results_viewer()
+        self._live_update()
+
     @observe('is_active', 'show_live_preview')
     def _toggle_marks(self, event={}):
         visible = self.show_live_preview and self.is_active
 
-        for viewer_id, mark in self.marks.items():
+        for viewer_ref, mark in self.marks.items():
             if not visible:
                 this_visible = False
             elif self.ephemeris_selected == 'No ephemeris':
                 this_visible = True
             else:
-                this_visible = viewer_id.split(':')[-1] == self.ephemeris_selected
+                viewer = self.app.get_viewer(viewer_ref)
+                viewer_ephem = getattr(viewer, '_ephemeris_component', None)
+                this_visible = viewer_ephem == self.ephemeris_selected
 
             mark.visible = this_visible
 
         if visible and event.get('name', '') in ('is_active', 'show_live_preview'):
             # then the marks themselves need to be updated
             self._live_update(event)
 
     @observe('flux_column_selected', 'dataset_selected',
              'ephemeris_selected',
-             'n_bins', 'previews_temp_disable')
+             'n_bins', 'previews_temp_disabled')
     @skip_if_no_updates_since_last_active()
+    @with_temp_disable(timeout=0.3)
     def _live_update(self, event={}):
         self.bin_enabled = self.n_bins != '' and self.n_bins > 0
 
         if not self.show_live_preview or not self.is_active or not self.bin_enabled:
             self._clear_marks()
             return
 
-        if self.previews_temp_disable:
-            return
-
-        start = time()
-
         if event.get('name', '') not in ('is_active', 'show_live_preview'):
             # mark visibility hasn't been handled yet
             self._toggle_marks()
 
         try:
             lc = self.bin(add_data=False)
         except Exception:
@@ -203,18 +201,14 @@
 
             if do_phase:
                 mark.update_ty(times, lc.flux.value)
             else:
                 mark.times = []
                 mark.update_xy(times, lc.flux.value)
 
-        self.last_live_time = np.round(time() - start, 2)
-        if self.last_live_time > 0.3:
-            self.previews_temp_disable = True
-
     def _on_ephemeris_update(self, msg):
         if not self.show_live_preview or not self.is_active:
             return
 
         if msg.ephemeris_label != self.ephemeris_selected:
             return
 
@@ -256,18 +250,19 @@
             # add data to the collection/viewer
             # NOTE: lc will have _LCVIZ_EPHEMERIS set if phase-folded
             self._set_results_viewer()
             self.add_results.add_results_from_plugin(data or lc)
 
             if self.ephemeris_selected != 'No ephemeris':
                 # prevent phase axis from becoming a time axis:
-                viewer_id = self.ephemeris_plugin._obj.phase_viewer_id
-                pv = self.app.get_viewer(viewer_id)
+                ephemeris_plugin = self.app._jdaviz_helper.plugins['Ephemeris']
                 phase_comp_lbl = self.app._jdaviz_helper._phase_comp_lbl(self.ephemeris_selected)
-                pv.state.x_att = self.app._jdaviz_helper._component_ids[phase_comp_lbl]
+                phase_comp = self.app._jdaviz_helper._component_ids[phase_comp_lbl]
+                for pv in ephemeris_plugin._obj._get_phase_viewers(self.ephemeris_selected):
+                    pv.state.x_att = phase_comp
                 # by resetting x_att, the preview marks may have dissappeared
                 self._live_update()
 
         return lc
 
     def vue_apply(self, event={}):
         self.bin(add_data=True)
```

### Comparing `lcviz-0.2.0/lcviz/plugins/binning/binning.vue` & `lcviz-0.3.0/lcviz/plugins/binning/binning.vue`

 * *Files 26% similar despite different names*

```diff
@@ -53,31 +53,19 @@
                  () => n_bins > 0 || 'Number of bins must be positive']"
         hint="Number of bins."
         persistent-hint
       >
       </v-text-field>
     </v-row>
 
-    <v-alert v-if="previews_temp_disable && show_live_preview" type='warning' style="margin-left: -12px; margin-right: -12px">
-      Live-updating is temporarily disabled (last update took {{last_live_time}}s)
-      <v-row justify='center'>
-        <j-tooltip tooltipcontent='hide live preview (can be re-enabled from the settings section in the plugin).' span_style="width: 100%">
-          <v-btn style='width: 100%' @click="show_live_preview = false">
-            disable previews
-          </v-btn>
-        </j-tooltip>
-      </v-row>
-      <v-row justify='center'>
-        <j-tooltip tooltipcontent='manually update live-previews based on current plugin inputs.' span_style="width: 100%">
-          <v-btn style='width: 100%' @click="previews_temp_disable = false">
-            update preview
-          </v-btn>
-        </j-tooltip>
-      </v-row>
-    </v-alert>
+    <plugin-previews-temp-disabled
+      :previews_temp_disabled.sync="previews_temp_disabled"
+      :previews_last_time="previews_last_time"
+      :show_live_preview.sync="show_live_preview"
+    />
 
     <plugin-add-results
       :label.sync="results_label"
       :label_default="results_label_default"
       :label_auto.sync="results_label_auto"
       :label_invalid_msg="results_label_invalid_msg"
       :label_overwrite="results_label_overwrite"
```

### Comparing `lcviz-0.2.0/lcviz/plugins/coords_info/coords_info.py` & `lcviz-0.3.0/lcviz/plugins/coords_info/coords_info.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/ephemeris/ephemeris.py` & `lcviz-0.3.0/lcviz/plugins/ephemeris/ephemeris.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,53 +126,47 @@
                   'ephemeris', 'ephemerides',
                   'update_ephemeris', 'create_phase_viewer',
                   'add_component', 'remove_component', 'rename_component',
                   'times_to_phases', 'phases_to_times', 'get_data',
                   'dataset', 'method', 'period_at_max_power', 'adopt_period_at_max_power']
         return PluginUserApi(self, expose=expose)
 
-    def _phase_comp_lbl(self, component):
+    def _phase_comp_lbl(self, component=None):
+        if component is None:
+            component = self.component_selected
         if self.app._jdaviz_helper is None:
             # duplicate logic from helper in case this is ever called before the helper
             # is fully intialized
             return f'phase:{component}'
         return self.app._jdaviz_helper._phase_comp_lbl(component)
 
     @property
     def phase_comp_lbl(self):
-        return self._phase_comp_lbl(self.component_selected)
+        return self._phase_comp_lbl()
 
-    def _phase_viewer_id(self, component):
-        return f'flux-vs-phase:{component}'
+    def _generate_phase_viewer_id(self, component=None):
+        if component is None:
+            component = self.component_selected
+        return self.app._jdaviz_helper._get_clone_viewer_reference(f'flux-vs-phase:{component}')
 
-    @property
-    def phase_viewer_ids(self):
-        viewer_ids = self.app.get_viewer_ids()
-        return [self._phase_viewer_id(component) for component in self.component.choices
-                if self._phase_viewer_id(component) in viewer_ids]
-
-    @property
-    def phase_viewer_id(self):
-        return self._phase_viewer_id(self.component_selected)
+    def _get_phase_viewers(self, lbl=None):
+        if lbl is None:
+            lbl = self.component_selected
+        return [viewer for vid, viewer in self.app._viewer_store.items()
+                if isinstance(viewer, PhaseScatterView)
+                and viewer._ephemeris_component == lbl]
 
     @property
     def default_phase_viewer(self):
         if not self.phase_viewer_exists:
             return None
         # we'll just treat the "default" as the first viewer connected to this
         # ephemeris component
         return self._get_phase_viewers()[0]
 
-    def _get_phase_viewers(self, lbl=None):
-        if lbl is None:
-            lbl = self.component_selected
-        return [viewer for vid, viewer in self.app._viewer_store.items()
-                if isinstance(viewer, PhaseScatterView)
-                and viewer.ephemeris_component == lbl]
-
     @property
     def ephemerides(self):
         return self._ephemerides
 
     @property
     def ephemeris(self):
         return self.ephemerides.get(self.component_selected, {})
@@ -265,58 +259,74 @@
                 )
 
                 new_links.append(new_link)
 
         dc.add_link(new_links)
 
         # update any plugin markers
-        # TODO: eventually might need to loop over multiple matching viewers
-        phase_viewer_id = self._phase_viewer_id(ephem_component)
-        if phase_viewer_id in self.app.get_viewer_ids():
-            phase_viewer = self.app.get_viewer(phase_viewer_id)
-            for mark in phase_viewer.custom_marks:
+        for viewer in self._get_phase_viewers(ephem_component):
+            for mark in viewer.custom_marks:
                 if hasattr(mark, 'update_phase_folding'):
                     mark.update_phase_folding()
 
         return phase_comp_lbl
 
-    def create_phase_viewer(self):
+    def create_phase_viewer(self, ephem_component=None):
         """
         Create a new phase viewer corresponding to ``component`` and populate the phase arrays
         with the current ephemeris, if necessary.
+
+        Parameters
+        ----------
+        ephem_component : str, optional
+            label of the component.  If not provided or ``None``, will default to plugin value.
         """
-        phase_viewer_id = self.phase_viewer_id
+        if ephem_component is None:
+            ephem_component = self.component_selected
+        phase_comp_lbl = self._phase_comp_lbl(ephem_component)
         dc = self.app.data_collection
 
         # check to see if this component already has a phase array.  We'll just check the first
         # item in the data-collection since the rest of the logic in this plugin /should/ populate
         # the arrays across all entries.
-        if self.phase_comp_lbl not in [comp.label for comp in dc[0].components]:
+        if phase_comp_lbl not in [comp.label for comp in dc[0].components]:
             self.update_ephemeris()  # calls _update_all_phase_arrays
 
-        create_phase_viewer = not self.phase_viewer_exists
-        if create_phase_viewer:
-            # TODO: stack horizontally by default?
-            self.app._on_new_viewer(NewViewerMessage(PhaseScatterView, data=None, sender=self.app),
-                                    vid=phase_viewer_id, name=phase_viewer_id)
-
-            time_viewer_item = self.app._get_viewer_item(self.app._jdaviz_helper._default_time_viewer_reference_name)  # noqa
-            for data in dc:
-                data_id = self.app._data_id_from_label(data.label)
-                visible = time_viewer_item['selected_data_items'].get(data_id, 'hidden')
-                self.app.set_data_visibility(phase_viewer_id, data.label, visible == 'visible')
+        phase_viewer_id = self._generate_phase_viewer_id(ephem_component)
+        # TODO: stack horizontally by default?
+        self.app._on_new_viewer(NewViewerMessage(PhaseScatterView, data=None, sender=self.app),
+                                vid=phase_viewer_id, name=phase_viewer_id,
+                                open_data_menu_if_empty=False)
 
+        # access new viewer, set bookkeeping for ephemeris component
         pv = self.app.get_viewer(phase_viewer_id)
-        if create_phase_viewer:
-            pv.state.x_min, pv.state.x_max = (self.wrap_at-1, self.wrap_at)
-        pv.state.x_att = self.app._jdaviz_helper._component_ids[self.phase_comp_lbl]
+        pv._ephemeris_component = ephem_component
+        # since we couldn't set ephemeris_component right away, _check_if_phase_viewer_exists
+        # might be out-of-date
+        self._check_if_phase_viewer_exists()
+
+        # set default data visibility
+        time_viewer_item = self.app._get_viewer_item(self.app._jdaviz_helper.default_time_viewer._obj.reference)  # noqa
+        for data in dc:
+            data_id = self.app._data_id_from_label(data.label)
+            visible = time_viewer_item['selected_data_items'].get(data_id, 'hidden')
+            self.app.set_data_visibility(phase_viewer_id, data.label, visible == 'visible')
+
+        # set x_att
+        phase_comp = self.app._jdaviz_helper._component_ids[phase_comp_lbl]
+        pv.state.x_att = phase_comp
+
+        # set viewer limits
+        pv.state.x_min, pv.state.x_max = (self.wrap_at-1, self.wrap_at)
+
         return pv.user_api
 
     def vue_create_phase_viewer(self, *args):
-        self.create_phase_viewer()
+        if not self.phase_viewer_exists:
+            self.create_phase_viewer()
 
     def vue_period_halve(self, *args):
         self.period /= 2
 
     def vue_period_double(self, *args):
         self.period *= 2
 
@@ -339,14 +349,15 @@
         self._ephemerides[new_lbl] = self._ephemerides.pop(old_lbl, {})
         for viewer in self._get_phase_viewers(old_lbl):
             self.app._update_viewer_reference_name(
                 viewer._ref_or_id,
                 viewer._ref_or_id.replace(old_lbl, new_lbl),
                 update_id=True
             )
+            viewer._ephemeris_component = new_lbl
 
         # update metadata entries so that they can be used for filtering applicable entries in
         # data menus
         for dc_item in self.app.data_collection:
             if dc_item.meta.get('_LCVIZ_EPHEMERIS', {}).get('ephemeris', None) == old_lbl:
                 dc_item.meta['_LCVIZ_EPHEMERIS']['ephemeris'] = new_lbl
         for data_item in self.app.state.data_items:
@@ -406,15 +417,15 @@
 
     def update_ephemeris(self, ephem_component=None, t0=None, period=None, dpdt=None, wrap_at=None):
         """
         Update the ephemeris for a given component.
 
         Parameters
         ----------
-        component : str, optional
+        ephem_component : str, optional
             label of the component.  If not provided or ``None``, will default to plugin value.
         t0 : float, optional
             value of t0 to replace
         period : float, optional
             value of period to replace
         dpdt : float, optional
             value of dpdt to replace
@@ -454,30 +465,32 @@
         if self.period <= 0:
             return
 
         def round_to_1(x):
             return round(x, -int(np.floor(np.log10(abs(x)))))
 
         # if phase-viewer doesn't yet exist in the app, create it now
-        self.create_phase_viewer()
+        if not self.phase_viewer_exists:
+            self.create_phase_viewer()
 
         # update value in the dictionary (to support multi-ephems)
         if event:
             self.update_ephemeris(**{event.get('name'): event.get('new')})
             # will call _update_all_phase_arrays
         else:
             self._update_all_phase_arrays(ephem_component=self.component_selected)
 
         # update zoom-limits if wrap_at was changed
         if event.get('name') == 'wrap_at':
             old = event.get('old') if event.get('old') != '' else self._prev_wrap_at
             if event.get('new') != '':
-                pvs = self.default_phase_viewer.state
                 delta_phase = event.get('new') - old
-                pvs.x_min, pvs.x_max = pvs.x_min + delta_phase, pvs.x_max + delta_phase
+                for pv in self._get_phase_viewers():
+                    pvs = pv.state
+                    pvs.x_min, pvs.x_max = pvs.x_min + delta_phase, pvs.x_max + delta_phase
                 # we need to cache the old value since it could become a string
                 # if the widget is cleared
                 self._prev_wrap_at = event.get('new')
 
         # update step-sizes
         self.period_step = round_to_1(self.period/5000)
         self.dpdt_step = max(round_to_1(abs(self.period * self.dpdt)/1000) if self.dpdt != 0 else 0,
```

### Comparing `lcviz-0.2.0/lcviz/plugins/ephemeris/ephemeris.vue` & `lcviz-0.3.0/lcviz/plugins/ephemeris/ephemeris.vue`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/export_plot/export_plot.py` & `lcviz-0.3.0/lcviz/plugins/markers/markers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,35 @@
-from jdaviz.configs.default.plugins import ExportViewer
+import numpy as np
+
+from jdaviz.configs.default.plugins import Markers
 from jdaviz.core.registries import tray_registry
 
-__all__ = ['ExportViewer']
+__all__ = ['Markers']
 
 
-@tray_registry('lcviz-export-plot', label="Export Plot")
-class ExportViewer(ExportViewer):
+@tray_registry('lcviz-markers', label="Markers")
+class Markers(Markers):
     """
-    See the :ref:`Export Plot Plugin Documentation <export-plot>` for more details.
+    See the :ref:`Markers Plugin Documentation <markers>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
-    * ``viewer`` (:class:`~jdaviz.core.template_mixin.ViewerSelect`):
-      Viewer to select for exporting the figure image.
-    * :meth:`save_figure`
+    * :meth:`clear_table`
+    * :meth:`~jdaviz.core.template_mixin.TableMixin.export_table`
     """
+    _default_table_values = {'time': np.nan,
+                             'phase': np.nan,
+                             'ephemeris': '',
+                             'flux': np.nan}
+
     def __init__(self, *args, **kwargs):
+        kwargs['headers'] = ['time', 'phase', 'ephemeris', 'flux', 'viewer']
         super().__init__(*args, **kwargs)
-        self.docs_link = f"https://lcviz.readthedocs.io/en/{self.vdocs}/plugins.html#export-plot"
+        self.docs_link = f"https://lcviz.readthedocs.io/en/{self.vdocs}/plugins.html#markers"
+
+    @property
+    def coords_info(self):
+        return self.app.session.application._tools['lcviz-coords-info']
```

### Comparing `lcviz-0.2.0/lcviz/plugins/flatten/flatten.py` & `lcviz-0.3.0/lcviz/plugins/flatten/flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
-from time import time
 
-from traitlets import Bool, Float, Unicode, observe
+from traitlets import Bool, Unicode, observe
 
 from jdaviz.core.custom_traitlets import FloatHandleEmpty, IntHandleEmpty
 from jdaviz.core.events import ViewerAddedMessage
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         DatasetSelectMixin,
                                         AutoTextField,
                                         skip_if_no_updates_since_last_active,
-                                        with_spinner)
+                                        with_spinner, with_temp_disable)
 from jdaviz.core.user_api import PluginUserApi
 
 from lcviz.components import FluxColumnSelectMixin
 from lcviz.marks import LivePreviewTrend, LivePreviewFlattened
 from lcviz.utils import data_not_folded
 from lcviz.viewers import TimeScatterView, PhaseScatterView
 from lcviz.parsers import _data_with_reftime
@@ -66,17 +65,14 @@
 
     flux_label_label = Unicode().tag(sync=True)
     flux_label_default = Unicode().tag(sync=True)
     flux_label_auto = Bool(True).tag(sync=True)
     flux_label_invalid_msg = Unicode('').tag(sync=True)
     flux_label_overwrite = Bool(False).tag(sync=True)
 
-    last_live_time = Float(0).tag(sync=True)
-    previews_temp_disable = Bool(False).tag(sync=True)
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.flux_label = AutoTextField(self, 'flux_label_label',
                                         'flux_label_default', 'flux_label_auto',
                                         'flux_label_invalid_msg')
 
@@ -98,34 +94,34 @@
         return PluginUserApi(self, expose=expose)
 
     @property
     def marks(self):
         trend_marks = {}
         flattened_marks = {}
 
-        for id, viewer in self.app._viewer_store.items():
+        for viewer in self.app._viewer_store.values():
             needs_trend = isinstance(viewer, TimeScatterView) and not isinstance(viewer, PhaseScatterView)  # noqa
             needs_flattened = isinstance(viewer, (TimeScatterView, PhaseScatterView))
             for mark in viewer.figure.marks:
                 if isinstance(mark, LivePreviewTrend):
-                    trend_marks[id] = mark
+                    trend_marks[viewer.reference] = mark
                     needs_trend = False
                 elif isinstance(mark, LivePreviewFlattened):
-                    flattened_marks[id] = mark
+                    flattened_marks[viewer.reference] = mark
                     needs_flattened = False
                 if not needs_trend and not needs_flattened:
                     break
             if needs_trend:
                 mark = LivePreviewTrend(viewer, visible=self.is_active)
                 viewer.figure.marks = viewer.figure.marks + [mark]
-                trend_marks[id] = mark
+                trend_marks[viewer.reference] = mark
             if needs_flattened:
                 mark = LivePreviewFlattened(viewer, visible=self.is_active)
                 viewer.figure.marks = viewer.figure.marks + [mark]
-                flattened_marks[id] = mark
+                flattened_marks[viewer.reference] = mark
 
         return trend_marks, flattened_marks
 
     @observe('dataset_selected', 'flux_column_selected')
     def _set_default_label(self, event={}):
         '''Generate a label and set the results field to that value'''
         if not hasattr(self, 'dataset'):  # pragma: no cover
@@ -213,24 +209,22 @@
         if ((live_visible or trend_visible) and
                 event.get('name') in ('is_active', 'show_live_preview', 'show_trend_preview')):
             # then the marks themselves need to be updated
             self._live_update(event)
 
     @observe('dataset_selected', 'flux_column_selected',
              'window_length', 'polyorder', 'break_tolerance',
-             'niters', 'sigma', 'previews_temp_disable')
+             'niters', 'sigma', 'previews_temp_disabled')
     @skip_if_no_updates_since_last_active()
+    @with_temp_disable(0.3)
     def _live_update(self, event={}):
-        if self.previews_temp_disable:
-            return
         if self.dataset_selected == '' or self.flux_column_selected == '':
             self._clear_marks()
             return
 
-        start = time()
         try:
             output_lc, trend_lc = self.flatten(add_data=False)
         except Exception as e:
             self.flatten_err = str(e)
             self._clear_marks()
             return
         self.flatten_err = ''
@@ -249,18 +243,14 @@
         trend_marks, flattened_marks = self.marks
         for mark in trend_marks.values():
             # TODO: need to account for phasing
             mark.update_ty(times.value, trend_lc.flux.value)
         for mark in flattened_marks.values():
             mark.update_ty(times.value, output_flux)
 
-        self.last_live_time = np.round(time() - start, 2)
-        if self.last_live_time > 0.3:
-            self.previews_temp_disable = True
-
     def vue_apply(self, *args, **kwargs):
         try:
             self.flatten(add_data=True)
         except Exception as e:
             self.flatten_err = str(e)
         else:
             self.flatten_err = ''
```

### Comparing `lcviz-0.2.0/lcviz/plugins/flatten/flatten.vue` & `lcviz-0.3.0/lcviz/plugins/flatten/flatten.vue`

 * *Files 11% similar despite different names*

```diff
@@ -134,31 +134,20 @@
       :value.sync="flux_label_label"
       :default="flux_label_default"
       :auto.sync="flux_label_auto"
       :invalid_msg="flux_label_invalid_msg"
       hint="Label for flux column."
     ></plugin-auto-label>
 
-    <v-alert v-if="previews_temp_disable && (show_live_preview || show_trend_preview)" type='warning' style="margin-left: -12px; margin-right: -12px">
-      Live-updating is temporarily disabled (last update took {{last_live_time}}s)
-      <v-row justify='center'>
-        <j-tooltip tooltipcontent='hide live trend and flattened previews (can be re-enabled from the settings section in the plugin).' span_style="width: 100%">
-          <v-btn style='width: 100%' @click="() => {show_live_preview = false; show_trend_preview = false}">
-            disable previews
-          </v-btn>
-        </j-tooltip>
-      </v-row>
-      <v-row justify='center'>
-        <j-tooltip tooltipcontent='manually update live-previews based on current plugin inputs.' span_style="width: 100%">
-          <v-btn style='width: 100%' @click="previews_temp_disable = false">
-            update preview
-          </v-btn>
-        </j-tooltip>
-      </v-row>
-    </v-alert>
+    <plugin-previews-temp-disabled
+      :previews_temp_disabled.sync="previews_temp_disabled"
+      :previews_last_time="previews_last_time"
+      :show_live_preview="show_live_preview || show_trend_preview"
+      @disable_previews="() => {show_live_preview=false; show_trend_preview=false}"
+    />
 
     <v-row justify="end">
       <j-tooltip tooltipcontent="Flatten and select the new column as the adopted flux column">
         <plugin-action-button 
           :spinner="spinner"
           :disabled="flux_label_invalid_msg.length > 0"
           :results_isolated_to_plugin="false"
```

### Comparing `lcviz-0.2.0/lcviz/plugins/flux_column/flux_column.py` & `lcviz-0.3.0/lcviz/plugins/flux_column/flux_column.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/flux_column/flux_column.vue` & `lcviz-0.3.0/lcviz/plugins/flux_column/flux_column.vue`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/frequency_analysis/frequency_analysis.py` & `lcviz-0.3.0/lcviz/plugins/frequency_analysis/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/frequency_analysis/frequency_analysis.vue` & `lcviz-0.3.0/lcviz/plugins/frequency_analysis/frequency_analysis.vue`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/markers/markers.py` & `lcviz-0.3.0/lcviz/plugins/subset_plugin/subset_plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-import numpy as np
-
-from jdaviz.configs.default.plugins import Markers
+from jdaviz.configs.default.plugins import SubsetPlugin
 from jdaviz.core.registries import tray_registry
 
-__all__ = ['Markers']
+__all__ = ['SubsetPlugin']
 
 
-@tray_registry('lcviz-markers', label="Markers")
-class Markers(Markers):
+@tray_registry('lcviz-subset-plugin', label="Subset Tools")
+class SubsetPlugin(SubsetPlugin):
     """
-    See the :ref:`Markers Plugin Documentation <markers>` for more details.
+    See the :ref:`Subset Plugin Documentation <subset-tools>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
-    * :meth:`clear_table`
-    * :meth:`~jdaviz.core.template_mixin.TableMixin.export_table`
     """
-    _default_table_values = {'time': np.nan,
-                             'phase': np.nan,
-                             'ephemeris': '',
-                             'flux': np.nan}
-
     def __init__(self, *args, **kwargs):
-        kwargs['headers'] = ['time', 'phase', 'ephemeris', 'flux', 'viewer']
         super().__init__(*args, **kwargs)
-        self.docs_link = f"https://lcviz.readthedocs.io/en/{self.vdocs}/plugins.html#markers"
-
-    @property
-    def coords_info(self):
-        return self.app.session.application._tools['lcviz-coords-info']
+        self.docs_link = f"https://lcviz.readthedocs.io/en/{self.vdocs}/plugins.html#subset-tools"
+        self.can_freeze = True
```

### Comparing `lcviz-0.2.0/lcviz/plugins/metadata_viewer/metadata_viewer.py` & `lcviz-0.3.0/lcviz/plugins/metadata_viewer/metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/plugins/plot_options/plot_options.py` & `lcviz-0.3.0/lcviz/plugins/plot_options/plot_options.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/tests/test_parser.py` & `lcviz-0.3.0/lcviz/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     assert isinstance(flux, u.Quantity)
     assert flux.unit.is_equivalent(u.electron / u.s)
 
 
 def test_apply_xrangerois(helper, light_curve_like_kepler_quarter):
     lc = light_curve_like_kepler_quarter
     helper.load_data(lc)
-    viewer = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    viewer = helper.default_time_viewer._obj
     subset_plugin = helper.plugins['Subset Tools']
 
     # the min/max of temporal regions can be defined in two ways:
     time_ranges = [
         [6, 8],  # in same units as the x axis, OR
         Time(['2011-07-19', '2011-07-23'])  # directly with a Time object
     ]
@@ -91,15 +91,15 @@
     np.testing.assert_allclose(subset_1_bounds_jd, [2455745., 2455747.])
     np.testing.assert_allclose(subset_2_bounds_jd, [2455761.50076602, 2455765.50076602])
 
 
 def test_apply_yrangerois(helper, light_curve_like_kepler_quarter):
     lc = light_curve_like_kepler_quarter
     helper.load_data(lc)
-    viewer = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    viewer = helper.default_time_viewer._obj
     subset_plugin = helper.plugins['Subset Tools']
 
     subset_plugin._obj.subset_selected = "Create New"
     viewer.apply_roi(YRangeROI(1, 1.05))
 
     subsets = helper.app.get_subsets()
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_plugin_binning.py` & `lcviz-0.3.0/lcviz/tests/test_plugin_binning.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     binning.n_bins = 150
     binned_lc = binning.bin(add_data=True)
     print(binned_lc)
 
 
 def test_plugin_binning(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
-    tv = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    tv = helper.default_time_viewer._obj
 
     b = helper.plugins['Binning']
     b._obj.plugin_opened = True
     ephem = helper.plugins['Ephemeris']
     ephem.period = 1.2345
     pv = ephem.create_phase_viewer()._obj
 
     with b.as_active():
         assert b.ephemeris == 'No ephemeris'
         assert len(_get_marks_from_viewer(tv)) == 1
-        assert len(_get_marks_from_viewer(pv)) == 0
+        assert len(_get_marks_from_viewer(pv)) == 1
         assert b._obj.ephemeris_dict == {}
 
         # update ephemeris will force re-phasing
         ephem.period = 1.111
 
         b.bin(add_data=True)
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_plugin_flatten.py` & `lcviz-0.3.0/lcviz/tests/test_plugin_flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     flatten.polyorder = 4
     flattened_lc = flatten.flatten(add_data=True)
     print(flattened_lc)
 
 
 def test_plugin_flatten(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
-    tv = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    tv = helper.default_time_viewer._obj
 
     ephem = helper.plugins['Ephemeris']
     pv = ephem.create_phase_viewer()._obj
     f = helper.plugins['Flatten']
 
     # no marks until plugin opened/active
     assert len(_get_marks_from_viewer(tv)) == 0
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_plugin_flux_column.py` & `lcviz-0.3.0/lcviz/tests/test_plugin_flux_column.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/tests/test_plugin_frequency_analysis.py` & `lcviz-0.3.0/lcviz/tests/test_plugin_frequency_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     freq.xunit = 'period'
     periodogram = freq.periodogram
     print(periodogram)
 
 
 def test_plugin_frequency_analysis(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
-    # tv = helper.app.get_viewer(helper._default_time_viewer_reference_name)
 
     freq = helper.plugins['Frequency Analysis']
     freq.open_in_tray()
 
     assert freq.method == 'Lomb-Scargle'
     assert freq._obj.err == ''
     assert isinstance(freq.periodogram, LombScarglePeriodogram)
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_plugin_markers.py` & `lcviz-0.3.0/lcviz/tests/test_plugin_markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     table = markers.export_table()
     print(table)
     markers.clear_table()
 
 
 def test_plugin_markers(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
-    tv = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    tv = helper.default_time_viewer._obj
 
     mp = helper.plugins['Markers']
     label_mouseover = mp._obj.coords_info
     mp.open_in_tray()
 
     # test event in flux-vs-time viewer
     label_mouseover._viewer_mouse_event(tv,
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_translator.py` & `lcviz-0.3.0/lcviz/tests/test_translator.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,15 @@
 
     # these times chosen by hand during Kepler Q0:
     near_transit = Time([
         '2009-05-02 02:51',
         '2009-05-02 03:52'
     ], format='iso')
 
-    viewer = helper.app.get_viewer(
-        helper._default_time_viewer_reference_name
-    )
+    viewer = helper.default_time_viewer._obj
     viewer.apply_roi(XRangeROI(*near_transit))
 
     columns_to_check = ['time', 'flux', 'flux_err']
     subset_translated = helper.get_data(subset='Subset 1')[columns_to_check]
     row_mask = (lc.time > near_transit[0]) & (lc.time < near_transit[1])
     lc_subset = lc[row_mask][columns_to_check]
```

### Comparing `lcviz-0.2.0/lcviz/tests/test_viewers.py` & `lcviz-0.3.0/lcviz/tests/test_viewers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 def test_reset_limits(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
-    tv = helper.app.get_viewer(helper._default_time_viewer_reference_name)
+    tv = helper.default_time_viewer._obj
 
     orig_xlims = (tv.state.x_min, tv.state.x_max)
     orig_ylims = (tv.state.y_min, tv.state.y_max)
     # set xmin and ymin to midpoints
     new_xmin = (tv.state.x_min + tv.state.x_max) / 2
     new_ymin = (tv.state.y_min + tv.state.y_max) / 2
     tv.state.x_min = new_xmin
@@ -19,11 +19,11 @@
     assert tv.state.y_min == orig_ylims[0]
 
 
 def test_clone(helper, light_curve_like_kepler_quarter):
     helper.load_data(light_curve_like_kepler_quarter)
 
     def_viewer = helper.viewers['flux-vs-time']
-    assert def_viewer._obj._get_clone_viewer_reference() == 'flux-vs-time[1]'
+    assert helper._get_clone_viewer_reference(def_viewer._obj.reference) == 'flux-vs-time[1]'
 
     new_viewer = def_viewer._obj.clone_viewer()
-    assert new_viewer._obj._get_clone_viewer_reference() == 'flux-vs-time[2]'
+    assert helper._get_clone_viewer_reference(new_viewer._obj.reference) == 'flux-vs-time[2]'
```

### Comparing `lcviz-0.2.0/lcviz/tools.py` & `lcviz-0.3.0/lcviz/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from jdaviz.core.tools import SidebarShortcutPlotOptions, SidebarShortcutExportPlot
 
 ICON_DIR = os.path.normpath(os.path.join(os.path.dirname(__file__), 'data', 'icons'))
 
 # point to the lcviz-version of plot options instead of jdaviz's
 SidebarShortcutPlotOptions.plugin_name = 'lcviz-plot-options'
-SidebarShortcutExportPlot.plugin_name = 'lcviz-export-plot'
+SidebarShortcutExportPlot.plugin_name = 'lcviz-export'
 
 
 __all__ = ['ViewerClone']
 
 
 @viewer_tool
 class ViewerClone(Tool):
```

### Comparing `lcviz-0.2.0/lcviz/utils.py` & `lcviz-0.3.0/lcviz/utils.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/lcviz/viewers.py` & `lcviz-0.3.0/lcviz/viewers.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,25 +206,16 @@
             #  2. Time objects, which get converted to work like (1) via the reference time
             if isinstance(roi.min, Time) or isinstance(roi.max, Time):
                 reference_time = self.data()[0].meta.get('reference_time', 0)
                 roi = roi.transformed(xfunc=lambda x: (x - reference_time).to_value(self.time_unit))
 
         super().apply_roi(roi, use_current=use_current)
 
-    def _get_clone_viewer_reference(self):
-        base_name = self.reference.split("[")[0]
-        name = base_name
-        ind = 0
-        while name in self.jdaviz_helper.viewers.keys():
-            ind += 1
-            name = f"{base_name}[{ind}]"
-        return name
-
     def clone_viewer(self):
-        name = self._get_clone_viewer_reference()
+        name = self.jdaviz_helper._get_clone_viewer_reference(self.reference)
 
         self.jdaviz_app._on_new_viewer(NewViewerMessage(self.__class__,
                                                         data=None,
                                                         sender=self.jdaviz_app),
                                        vid=name, name=name)
 
         this_viewer_item = self.jdaviz_app._get_viewer_item(self.reference)
@@ -232,34 +223,36 @@
         for data in self.jdaviz_app.data_collection:
             data_id = self.jdaviz_app._data_id_from_label(data.label)
             visible = this_viewer_item['selected_data_items'].get(data_id, 'hidden')
             self.jdaviz_app.set_data_visibility(name, data.label, visible == 'visible')
             # TODO: don't revert color when adding same data to a new viewer
             # (same happens when creating a phase-viewer from ephemeris plugin)
 
-        new_viewer = self.jdaviz_helper.viewers[name]._obj
+        new_viewer = self.jdaviz_app.get_viewer(name)
+        if hasattr(self, 'ephemeris_component'):
+            new_viewer._ephemeris_component = self._ephemeris_component
         for k, v in this_state.items():
             if k in ('layers',):
                 continue
             setattr(new_viewer.state, k, v)
 
         return new_viewer.user_api
 
 
-@viewer_registry("lcviz-phase-viewer", label="phase-vs-time")
+@viewer_registry("lcviz-phase-viewer", label="flux-vs-phase")
 class PhaseScatterView(TimeScatterView):
-    @property
-    def ephemeris_component(self):
-        return self.reference.split('[')[0].split(':')[-1]
+    def __init__(self, *args, **kwargs):
+        self._ephemeris_component = 'default'
+        super().__init__(*args, **kwargs)
 
     def _set_plot_x_axes(self, dc, component_labels, light_curve):
         # setting of y_att will be handled by ephemeris plugin
-        self.state.x_att = dc[0].components[component_labels.index(f'phase:{self.ephemeris_component}')]  # noqa
+        self.state.x_att = dc[0].components[component_labels.index(f'phase:{self._ephemeris_component}')]  # noqa
         self.figure.axes[0].label = 'phase'
         self.figure.axes[0].num_ticks = 5
 
     def times_to_phases(self, times):
         ephem = self.jdaviz_helper.plugins.get('Ephemeris', None)
         if ephem is None:
             raise ValueError("must have ephemeris plugin loaded to convert")
 
-        return ephem.times_to_phases(times, ephem_component=self.ephemeris_component)
+        return ephem.times_to_phases(times, ephem_component=self._ephemeris_component)
```

### Comparing `lcviz-0.2.0/lcviz.egg-info/PKG-INFO` & `lcviz-0.3.0/lcviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcviz
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Jdaviz-based light curve analysis and visualization tool
 Author-email: JDADF Developers <kconroy@stsci.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Association of Universities for Research in Astronomy.
         All rights reserved.
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: astropy>=5.2
-Requires-Dist: jdaviz==3.8.*
+Requires-Dist: jdaviz==3.9.*
 Requires-Dist: lightkurve>=2.4.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-astropy; extra == "test"
 Requires-Dist: pytest-tornasync; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy[confv2]>=1.9.1; extra == "docs"
```

### Comparing `lcviz-0.2.0/lcviz.egg-info/SOURCES.txt` & `lcviz-0.3.0/lcviz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 MANIFEST.in
 README.rst
 conftest.py
 pyproject.toml
 requirements.txt
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/publish.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/installation.rst
@@ -56,16 +57,16 @@
 lcviz/plugins/binning/binning.py
 lcviz/plugins/binning/binning.vue
 lcviz/plugins/coords_info/__init__.py
 lcviz/plugins/coords_info/coords_info.py
 lcviz/plugins/ephemeris/__init__.py
 lcviz/plugins/ephemeris/ephemeris.py
 lcviz/plugins/ephemeris/ephemeris.vue
-lcviz/plugins/export_plot/__init__.py
-lcviz/plugins/export_plot/export_plot.py
+lcviz/plugins/export/__init__.py
+lcviz/plugins/export/export.py
 lcviz/plugins/flatten/__init__.py
 lcviz/plugins/flatten/flatten.py
 lcviz/plugins/flatten/flatten.vue
 lcviz/plugins/flux_column/__init__.py
 lcviz/plugins/flux_column/flux_column.py
 lcviz/plugins/flux_column/flux_column.vue
 lcviz/plugins/frequency_analysis/__init__.py
@@ -75,21 +76,24 @@
 lcviz/plugins/markers/markers.py
 lcviz/plugins/metadata_viewer/__init__.py
 lcviz/plugins/metadata_viewer/metadata_viewer.py
 lcviz/plugins/plot_options/__init__.py
 lcviz/plugins/plot_options/plot_options.py
 lcviz/plugins/subset_plugin/__init__.py
 lcviz/plugins/subset_plugin/subset_plugin.py
+lcviz/plugins/viewer_creator/__init__.py
+lcviz/plugins/viewer_creator/viewer_creator.py
 lcviz/tests/__init__.py
 lcviz/tests/test_parser.py
 lcviz/tests/test_plugin_binning.py
 lcviz/tests/test_plugin_ephemeris.py
 lcviz/tests/test_plugin_flatten.py
 lcviz/tests/test_plugin_flux_column.py
 lcviz/tests/test_plugin_frequency_analysis.py
 lcviz/tests/test_plugin_markers.py
 lcviz/tests/test_plugin_metadata.py
 lcviz/tests/test_plugin_plot_options.py
 lcviz/tests/test_translator.py
+lcviz/tests/test_tray_viewer_creator.py
 lcviz/tests/test_viewers.py
 notebooks/ConfigHelperHelper.ipynb
 notebooks/LCvizExample.ipynb
```

### Comparing `lcviz-0.2.0/notebooks/ConfigHelperHelper.ipynb` & `lcviz-0.3.0/notebooks/ConfigHelperHelper.ipynb`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/notebooks/LCvizExample.ipynb` & `lcviz-0.3.0/notebooks/LCvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/pyproject.toml` & `lcviz-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
     "astropy>=5.2",
-    "jdaviz==3.8.*",
+    # NOTE: if/when we stop pinning a minor version of jdaviz, add jdaviz
+    # to devdeps in tox.ini
+    "jdaviz==3.9.*",
     "lightkurve>=2.4.1",
 ]
 dynamic = [
     "version",
 ]
 
 [project.readme]
@@ -93,14 +95,15 @@
 text_file_format = "rst"
 addopts = "--doctest-rst --import-mode=append"
 filterwarnings = [
     "error",
     "ignore:numpy\\.ndarray size changed:RuntimeWarning",
     "ignore:zmq\\.eventloop\\.ioloop is deprecated in pyzmq:DeprecationWarning",
     "ignore:((.|\n)*)Sentinel is not a public part of the traitlets API((.|\n)*)",
+    "ignore:datetime\\.datetime\\.utcfromtimestamp:DeprecationWarning",
     "ignore::DeprecationWarning:glue",
     "ignore::DeprecationWarning:bqplot",
     "ignore::DeprecationWarning:bqplot_image_gl",
     "ignore::DeprecationWarning:bqscales",
     "ignore::DeprecationWarning:ipykernel",
     "ignore::DeprecationWarning:traittypes",
     "ignore::DeprecationWarning:voila",
```

### Comparing `lcviz-0.2.0/setup.py` & `lcviz-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `lcviz-0.2.0/tox.ini` & `lcviz-0.3.0/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 # The following provides some specific pinnings for key packages
 deps =
     # NOTE: Add/remove as needed
     devdeps: astropy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
     devdeps: numpy>=0.0.dev0
-    devdeps: git+https://github.com/spacetelescope/jdaviz.git
+#    devdeps: git+https://github.com/spacetelescope/jdaviz.git
     devdeps: git+https://github.com/lightkurve/lightkurve.git
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     # Uncomment when we have all again in setup.cfg
     #alldeps: all
```

