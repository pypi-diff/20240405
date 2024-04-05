# Comparing `tmp/kilosort-4.0.2.tar.gz` & `tmp/kilosort-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.2.tar", last modified: Mon Mar 11 15:44:42 2024, max compression
+gzip compressed data, was "kilosort-4.0.3.tar", last modified: Fri Apr  5 21:03:03 2024, max compression
```

## Comparing `kilosort-4.0.2.tar` & `kilosort-4.0.3.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.323474 kilosort-4.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.311473 kilosort-4.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.311473 kilosort-4.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-11 15:44:33.000000 kilosort-4.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-11 15:44:33.000000 kilosort-4.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-11 15:44:33.000000 kilosort-4.0.2/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-11 15:44:33.000000 kilosort-4.0.2/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.311473 kilosort-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-11 15:44:33.000000 kilosort-4.0.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-11 15:44:33.000000 kilosort-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-11 15:44:33.000000 kilosort-4.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-11 15:44:33.000000 kilosort-4.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 15:44:33.000000 kilosort-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-03-11 15:44:42.323474 kilosort-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-03-11 15:44:33.000000 kilosort-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.315474 kilosort-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/first_run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.315474 kilosort-4.0.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 15:44:33.000000 kilosort-4.0.2/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.319474 kilosort-4.0.2/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.323474 kilosort-4.0.2/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13195 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22256 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    32781 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    34981 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-11 15:44:33.000000 kilosort-4.0.2/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.323474 kilosort-4.0.2/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-03-11 15:44:42.000000 kilosort-4.0.2/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-11 15:44:42.000000 kilosort-4.0.2/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:44:42.000000 kilosort-4.0.2/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-11 15:44:42.000000 kilosort-4.0.2/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 15:44:42.000000 kilosort-4.0.2/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-11 15:44:33.000000 kilosort-4.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:44:42.323474 kilosort-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-11 15:44:33.000000 kilosort-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:44:42.323474 kilosort-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-11 15:44:33.000000 kilosort-4.0.2/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-11 15:44:33.000000 kilosort-4.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.940929 kilosort-4.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-05 21:02:45.000000 kilosort-4.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 21:02:45.000000 kilosort-4.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 21:02:45.000000 kilosort-4.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 21:02:45.000000 kilosort-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-05 21:03:03.956929 kilosort-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-05 21:02:45.000000 kilosort-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.948929 kilosort-4.0.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.948929 kilosort-4.0.3/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.952929 kilosort-4.0.3/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36385 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 21:02:45.000000 kilosort-4.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:03:03.956929 kilosort-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-05 21:02:45.000000 kilosort-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 21:02:45.000000 kilosort-4.0.3/tox.ini
```

### Comparing `kilosort-4.0.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `kilosort-4.0.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.3/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/.gitignore` & `kilosort-4.0.3/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -113,21 +113,27 @@
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
 
+# Visual Studio Code workspace settings
+.vscode
+
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # Test data
 tests/.test_data/
 tests/.test_data/*
+
+# docs/ copy of README
+docs/README.md
```

### Comparing `kilosort-4.0.2/.readthedocs.yml` & `kilosort-4.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/CODE_OF_CONDUCT.md` & `kilosort-4.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/LICENSE` & `kilosort-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/PKG-INFO` & `kilosort-4.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.2
+Version: 4.0.3
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,26 +17,29 @@
 Requires-Dist: tqdm
 Requires-Dist: torch>=1.6
 Requires-Dist: numba
 Requires-Dist: faiss-cpu
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
 Provides-Extra: gui
 Requires-Dist: pyqtgraph>=0.13.0; extra == "gui"
-Requires-Dist: pyqt5; extra == "gui"
-Requires-Dist: pyqt5.sip; extra == "gui"
-Requires-Dist: google-cloud-storage; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: pyqt6; extra == "gui"
+Requires-Dist: pyqt6.sip; extra == "gui"
 Requires-Dist: matplotlib; extra == "gui"
 Provides-Extra: all
 Requires-Dist: pyqtgraph>=0.13.0; extra == "all"
-Requires-Dist: pyqt5; extra == "all"
-Requires-Dist: pyqt5.sip; extra == "all"
-Requires-Dist: google-cloud-storage; extra == "all"
+Requires-Dist: qtpy; extra == "all"
+Requires-Dist: pyqt6; extra == "all"
+Requires-Dist: pyqt6.sip; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 
 # Kilosort4
 
 [![Documentation Status](https://readthedocs.org/projects/kilosort/badge/?version=latest)](https://kilosort.readthedocs.io/en/latest/?badge=latest)
 ![tests](https://github.com/mouseland/kilosort/actions/workflows/test_and_deploy.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/kilosort.svg)](https://badge.fury.io/py/kilosort)
@@ -57,15 +60,19 @@
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
 **If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). 
+**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+
+**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04. 
 
@@ -101,18 +108,28 @@
 
 1. Open the GUI with `python -m kilosort`
 2. Select the path to the binary file and optionally the results directory. We recommend putting the binary file on an SSD for faster processing. 
 3. Select the probe configuration (mat files recommended, they actually exclude off channels unlike prb files)
 4. Hit `LOAD`. The data should now be visible.
 5. Hit `Run`. This will run the pipeline and output the results in a format compatible with Phy, the most popular spike sorting curating software.
 
-There is a warning that will always pop up when running Kilosort and/or using the BinaryFile class, but it's nothing to worry about:
+### Debugging qt.qpa.plugin error
+
+Some users have encountered the following error (or similar ones with slight variations) when attempting to launch the Kilosort4 GUI:
 ```
-UserWarning: The given NumPy array is not writable, and PyTorch does not support non-writable tensors. This means writing to this tensor will result in undefined behavior. You may want to copy the array to protect its data or make it writable before converting it to a tensor. This type of warning will be suppressed for the rest of this program. (Triggered internally at C:\cb\pytorch_1000000000000\work\torch\csrc\utils\tensor_numpy.cpp:205.)
+QObject::moveToThread: Current thread (0x2a7734988a0) is not the object's thread (0x2a77349d4e0).
+Cannot move to target thread (0x2a7734988a0)
+
+qt.qpa.plugin: Could not load the Qt platform plugin "windows" in "<FILEPATH>" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+
+Available platform plugins are: minimal, offscreen, webgl, windows.
 ```
+This is not specific to Kilosort4, it is a general problem with PyQt (the GUI library we chose to develop with) that doesn't appear to have a single cause or fix. If you encounter this error, please check [issue 597](https://github.com/MouseLand/Kilosort/issues/597) and [issue 613](https://github.com/MouseLand/Kilosort/issues/613) for some suggested solutions.
+
 
 ## Integration with Phy GUI
 
 [Phy](https://github.com/cortex-lab/phy) provides a manual clustering interface for refining the results of the algorithm. Kilosort4 automatically sets the "good" units in Phy based on a <10% estimated contamination rate with spikes from other neurons (computed from the refractory period violations relative to expected).
 
 Check out the [Phy](https://github.com/cortex-lab/phy) repo for more install instructions. We recommend installing Phy in its own environment to avoid package conflicts.
```

### Comparing `kilosort-4.0.2/README.md` & `kilosort-4.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,19 @@
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
 **If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). 
+**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+
+**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04. 
 
@@ -64,18 +68,28 @@
 
 1. Open the GUI with `python -m kilosort`
 2. Select the path to the binary file and optionally the results directory. We recommend putting the binary file on an SSD for faster processing. 
 3. Select the probe configuration (mat files recommended, they actually exclude off channels unlike prb files)
 4. Hit `LOAD`. The data should now be visible.
 5. Hit `Run`. This will run the pipeline and output the results in a format compatible with Phy, the most popular spike sorting curating software.
 
-There is a warning that will always pop up when running Kilosort and/or using the BinaryFile class, but it's nothing to worry about:
+### Debugging qt.qpa.plugin error
+
+Some users have encountered the following error (or similar ones with slight variations) when attempting to launch the Kilosort4 GUI:
 ```
-UserWarning: The given NumPy array is not writable, and PyTorch does not support non-writable tensors. This means writing to this tensor will result in undefined behavior. You may want to copy the array to protect its data or make it writable before converting it to a tensor. This type of warning will be suppressed for the rest of this program. (Triggered internally at C:\cb\pytorch_1000000000000\work\torch\csrc\utils\tensor_numpy.cpp:205.)
+QObject::moveToThread: Current thread (0x2a7734988a0) is not the object's thread (0x2a77349d4e0).
+Cannot move to target thread (0x2a7734988a0)
+
+qt.qpa.plugin: Could not load the Qt platform plugin "windows" in "<FILEPATH>" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+
+Available platform plugins are: minimal, offscreen, webgl, windows.
 ```
+This is not specific to Kilosort4, it is a general problem with PyQt (the GUI library we chose to develop with) that doesn't appear to have a single cause or fix. If you encounter this error, please check [issue 597](https://github.com/MouseLand/Kilosort/issues/597) and [issue 613](https://github.com/MouseLand/Kilosort/issues/613) for some suggested solutions.
+
 
 ## Integration with Phy GUI
 
 [Phy](https://github.com/cortex-lab/phy) provides a manual clustering interface for refining the results of the algorithm. Kilosort4 automatically sets the "good" units in Phy based on a <10% estimated contamination rate with spikes from other neurons (computed from the refractory period violations relative to expected).
 
 Check out the [Phy](https://github.com/cortex-lab/phy) repo for more install instructions. We recommend installing Phy in its own environment to avoid package conflicts.
```

### Comparing `kilosort-4.0.2/docs/Makefile` & `kilosort-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/conf.py` & `kilosort-4.0.3/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 # NOTE: To build locally, run the following from the top level of the Kilosort4
-#       repository: `sphinx-build -b html docs/source docs/build/html`
+#       repository:
+#       `conda install -c conda-forge pandoc`
+#       Then reinstall Kilosort4 with docs dependencies:
+#       `pip install -e .[docs]`
+#       Then build the html with:
+#       `sphinx-build -b html docs/ docs/build/html`
 #       For api: `sphinx-apidoc -f -o docs/source/api kilosort` (WIP)
-#                For now, add to api.rst manually instead.
+#                For now, add to api.rst manually instead.       
 
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
+# Download README from main branch when building documentation, following:
+# https://stackoverflow.com/questions/66495200/is-it-possible-to-include-external-rst-files-in-my-documentation
+from urllib.request import urlretrieve
+urlretrieve (
+    "https://raw.githubusercontent.com/MouseLand/Kilosort/main/README.md",
+    "README.md"
+)
+
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Kilosort4'
 copyright = '2024, Marius Pachitariu, Jacob Pennington & Carsen Stringer'
 author = 'Jacob Pennington (documentation)'
 release = '0.0.1'
@@ -54,15 +67,15 @@
 html_theme_options = {
     'canonical_url': '',
     'analytics_id': 'UA-XXXXXXX-1',  #  Provided by Google in your dashboard
     'logo_only': False,
     'display_version': True,
     'prev_next_buttons_location': 'top',
     'style_external_links': False,
-    'style_nav_header_background': 'black',
+    'style_nav_header_background': 'Gray',
     # Toc options
     'collapse_navigation': True,
     'sticky_navigation': True,
     'navigation_depth': 4,
     'includehidden': True,
     'titles_only': False
 }
```

### Comparing `kilosort-4.0.2/docs/drift.rst` & `kilosort-4.0.3/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/hardware.rst` & `kilosort-4.0.3/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/index.rst` & `kilosort-4.0.3/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 detailed comparisons to past versions of Kilosort and to other spike-sorting methods,
 please see our pre-print on `BioArxiv <https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1>`_.
 
 .. toctree::
    :maxdepth: 1
    :caption: Getting Started
 
-   installation
-   first_run
+   README <README.md>
+   gui_guide
+   parameters
+   multi_shank
    hardware
    drift
 
 .. toctree::
    :maxdepth: 1
    :caption: Tutorials
```

### Comparing `kilosort-4.0.2/docs/make.bat` & `kilosort-4.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.3/docs/tutorials/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/tutorials/load_data.ipynb` & `kilosort-4.0.3/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.3/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/CCG.py` & `kilosort-4.0.3/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/bench.py` & `kilosort-4.0.3/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/clustering_qr.py` & `kilosort-4.0.3/kilosort/clustering_qr.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,28 +324,33 @@
         raise ValueError(
             'Wall is empty after `clustering_qr.run`, cannot continue clustering.'
         )
 
     return clu, Wall
 
 
-def get_data_cpu(ops, xy, iC, PID, tF, ycenter,  xcenter, dmin = 20, dminx = 32, ncomps = 64):
+def get_data_cpu(ops, xy, iC, PID, tF, ycenter, xcenter, dmin=20, dminx=32,
+                 ncomps=64, ix=None, merge_dim=True):
     PID =  torch.from_numpy(PID).long()
 
     #iU = ops['iU'].cpu().numpy()
     #iC = ops['iCC'][:, ops['iU']]    
     #xcup, ycup = ops['xc'][iU], ops['yc'][iU]
     #xy = np.vstack((xcup, ycup))
     #xy = torch.from_numpy(xy)
     
     y0 = ycenter # xy[1].mean() - ycenter
     x0 = xcenter #xy[0].mean() - xcenter
 
     #print(dmin, dminx)
-    ix = torch.logical_and(torch.abs(xy[1] - y0) < dmin, torch.abs(xy[0] - x0) < dminx)
+    if ix is None:
+        ix = torch.logical_and(
+            torch.abs(xy[1] - y0) < dmin,
+            torch.abs(xy[0] - x0) < dminx
+            )
     #print(ix.nonzero()[:,0])
     igood = ix[PID].nonzero()[:,0]
 
     if len(igood)==0:
         return None, None,  None, None
 
     pid = PID[igood]
@@ -358,15 +363,20 @@
 
     dd = torch.zeros((nspikes, nchan, nfeatures))
     for j in ix.nonzero()[:,0]:
         ij = torch.nonzero(pid==j)[:, 0]
         #print(ij.sum())
         dd[ij.unsqueeze(-1), iC[:,j]-ch_min] = data[ij]
 
-    Xd = torch.reshape(dd, (nspikes, -1))
+    if merge_dim:
+        Xd = torch.reshape(dd, (nspikes, -1))
+    else:
+        # Keep channels and features separate
+        Xd = dd
+
     return Xd, ch_min, ch_max, igood
 
 
 
 def assign_clust(rows_neigh, iclust, kn, tones2, nclust):    
     NN = len(iclust)
```

### Comparing `kilosort-4.0.2/kilosort/datashift.py` & `kilosort-4.0.3/kilosort/datashift.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/gui/__init__.py` & `kilosort-4.0.3/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/gui/converter.py` & `kilosort-4.0.3/kilosort/gui/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 from pathlib import Path
 
 import numpy as np
-from PyQt5 import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets
 from kilosort.io import (
     RecordingExtractorAsArray, BinaryRWFile, spikeinterface_to_binary, load_probe
     )
 from kilosort.gui.logger import setup_logger
 
 logger = setup_logger(__name__)
 
@@ -18,16 +18,16 @@
     'Neuralynx': 'read_neuralynx',
     'Openephys': 'read_openephys',
     'Intan': 'read_intan'
 }
 
 
 class DataConversionBox(QtWidgets.QWidget):
-    disableInput = QtCore.pyqtSignal(bool)
-    fileObjectLoaded = QtCore.pyqtSignal(bool)
+    disableInput = QtCore.Signal(bool)
+    fileObjectLoaded = QtCore.Signal(bool)
 
     def __init__(self, gui):
         super().__init__()
         self.gui = gui
         self.setWindowTitle('Convert data (REQUIRES SPIKEINTERFACE)')
         self.filename = None
         self.filetype = None
@@ -79,17 +79,17 @@
         self.dtype_note = QtWidgets.QLabel(
             "NOTE: this is the dtype for the new .bin file.\nIf the existing file"
             " is not the same dtype, data may be altered."
         )
         self.dtype_selector = QtWidgets.QComboBox()
         supported_dtypes = BinaryRWFile.supported_dtypes
         self.dtype_selector.addItems([''] + supported_dtypes)
-        self.dtype_selector.setSizeAdjustPolicy(
-            QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
-        )
+        #self.dtype_selector.setSizeAdjustPolicy(
+        #    QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
+        #)
         self.dtype_selector.currentTextChanged.connect(self.set_dtype)
     
         layout.addWidget(self.stream_id_text, 0, 10, 1, 3)
         layout.addWidget(self.stream_id_input, 0, 13, 1, 3)
         layout.addWidget(self.stream_name_text, 1, 10, 1, 3)
         layout.addWidget(self.stream_name_input, 1, 13, 1, 3)
         layout.addWidget(self.dtype_text, 2, 10, 1, 3)
@@ -130,67 +130,67 @@
             "and select it like any other binary file."
         )
         layout.addWidget(self.crash_warning, 8, 0, 3, 16)
 
         self.setLayout(layout)
 
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def select_file(self):
         options = QtWidgets.QFileDialog.DontUseNativeDialog
         filename, _ = QtWidgets.QFileDialog.getOpenFileName(
             parent=self,
             caption="Choose file to load data from...",
             directory=self.gui.qt_settings.value('last_data_location'),
             options=options,
         )
         self.filename = filename
         self.filename_input.setText(filename)
         data_location = Path(filename).parent.as_posix()
         self.gui.qt_settings.setValue('last_data_location', data_location)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def select_folder(self):
         options = QtWidgets.QFileDialog.DontUseNativeDialog
         directory = QtWidgets.QFileDialog.getExistingDirectory(
             parent=self,
             caption="Choose directory to load data from...",
             directory=self.gui.qt_settings.value('last_data_location'),
             options=options,
         )
         self.filename = directory
         self.filename_input.setText(directory)
         data_location = Path(directory).as_posix()
         self.gui.qt_settings.setValue('last_data_location', data_location)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def select_filetype(self):
         self.filetype = self.filetype_selector.currentText()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def set_stream_id(self):
         stream_id = self.stream_id_input.text()
         if stream_id is None or stream_id == '':
             stream_id = None
         else:
             stream_id = stream_id
         self.stream_id = stream_id
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def set_stream_name(self):
         stream_name = self.stream_name_input.text()
         if stream_name == '':
             stream_name = None
         self.stream_name = stream_name
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def set_dtype(self):
         self.data_dtype = self.dtype_selector.currentText()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def load_as_wrapper(self):
         if None in [self.filename, self.filetype, self.data_dtype]:
             logger.exception(
                 'File name, file type, and data dtype must be specified.'
             )
             logger.exception(
                 f'File name: {self.filename}\nFile type: {self.filetype}\n'
@@ -226,15 +226,15 @@
         except ValueError:
             print(
                 'SpikeInterface recording contains no probe information,\n'
                 'could not write .prb file.'
             )
         self.gui.settings_box.check_load()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def convert_to_binary(self):
         # TODO: add option to specify chunksize for conversion
         if None in [self.filename, self.filetype, self.data_dtype]:
             logger.exception(
                 'File name, file type, and data dtype must be specified.'
             )
             logger.exception(
```

### Comparing `kilosort-4.0.2/kilosort/gui/data_view_box.py` & `kilosort-4.0.3/kilosort/gui/data_view_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 import pyqtgraph as pg
 from kilosort.gui.logger import setup_logger
 from kilosort.gui.palettes import COLORMAP_COLORS
-from PyQt5 import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets
 
 logger = setup_logger(__name__)
 
 
 class DataViewBox(QtWidgets.QGroupBox):
-    channelChanged = QtCore.pyqtSignal(int, int)
-    modeChanged = QtCore.pyqtSignal(str, int)
-    updateContext = QtCore.pyqtSignal(object)
-    intervalUpdated = QtCore.pyqtSignal()
+    channelChanged = QtCore.Signal(int, int)
+    modeChanged = QtCore.Signal(str, int)
+    updateContext = QtCore.Signal(object)
+    intervalUpdated = QtCore.Signal()
 
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
 
         self.gui = parent
 
         self.data_view_widget = KSPlotWidget(useOpenGL=True)
@@ -187,42 +187,40 @@
 
         layout.addLayout(data_view_layout, 85)
         layout.addLayout(data_controls_layout, 3)
         layout.addLayout(data_seek_layout, 10)
 
         self.setLayout(layout)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def on_tmin_edited(self):
         try:
             self.tmin = float(self.tmin_input.text())
             self.check_time_interval()
-            self.intervalUpdated.emit()
         except ValueError:
             logger.exception('Could not convert tmin to float.')
         except AssertionError:
             logger.exception('Invalid tmin,tmax: must have 0 <= tmin < tmax')
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def on_tmax_edited(self):
         try:
             self.tmax = float(self.tmax_input.text())
             self.check_time_interval()
-            self.intervalUpdated.emit()
         except ValueError:
             logger.exception('Could not convert tmax to float.')
         except AssertionError:
             logger.exception('Invalid tmin,tmax: must have 0 <= tmin < tmax')
 
     def check_time_interval(self):
         # TODO: any other checks needed?
         assert self.tmin >= 0
         assert self.tmin < self.tmax
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def on_views_clicked(self):
         current_state = {key: self.view_buttons[key].isChecked() for key in self._keys}
 
         if current_state != self.view_buttons_state:
             self.view_buttons_state = current_state
 
             for view, state in self.view_buttons_state.items():
@@ -240,30 +238,30 @@
                     else:
                         button.setStyleSheet(
                             "QPushButton {background-color: black; color: gray;}"
                         )
 
             self.update_plot()
 
-    @QtCore.pyqtSlot(float)
+    @QtCore.Slot(float)
     def on_wheel_scroll(self, direction):
         if self.context_set():
             self.shift_current_time(direction)
 
-    @QtCore.pyqtSlot(float)
+    @QtCore.Slot(float)
     def on_wheel_scroll_plus_control(self, direction):
         if self.context_set():
             self.change_displayed_channel_count(direction)
 
-    @QtCore.pyqtSlot(float)
+    @QtCore.Slot(float)
     def on_wheel_scroll_plus_shift(self, direction):
         if self.context_set():
             self.change_plot_range(direction)
 
-    @QtCore.pyqtSlot(float)
+    @QtCore.Slot(float)
     def on_wheel_scroll_plus_alt(self, direction):
         if self.context_set():
             self.change_plot_scaling(direction)
 
     def context_set(self):
         return self.get_context() is not None
 
@@ -428,15 +426,15 @@
         except ValueError:
             self.time_seek.setPos(self.seek_range[1] - self.plot_range)
 
     def change_sorting_status(self, status_dict):
         self.sorting_status = status_dict
         self.enable_view_buttons()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def enable_view_buttons(self):
         self.raw_button.click()
 
         if self.whitening_matrix is not None:
             self.whitened_button.setEnabled(True)
             self.whitened_button.setStyleSheet(
                 "QPushButton {background-color: black; color: white;}"
@@ -472,19 +470,19 @@
             lut=self.lookup_table,
             levels=(level_min, level_max),
             autoDownsample=False,
         )
         self.colormap_image = image_item
         self.plot_item.addItem(image_item)
 
-    @QtCore.pyqtSlot(object)
+    @QtCore.Slot(object)
     def set_whitening_matrix(self, array):
         self.whitening_matrix = array
 
-    @QtCore.pyqtSlot(object)
+    @QtCore.Slot(object)
     def set_highpass_filter(self, filter):
         self.highpass_filter = filter
 
     def update_plot(self, context=None):
         if context is None:
             context = self.gui.context
 
@@ -577,18 +575,18 @@
                 whitened_traces[to_display, :].T,
                 colormap_min,
                 colormap_max,
             )
 
 
 class KSPlotWidget(pg.PlotWidget):
-    signalChangeTimePoint = QtCore.pyqtSignal(float)
-    signalChangeChannel = QtCore.pyqtSignal(float)
-    signalChangeTimeRange = QtCore.pyqtSignal(float)
-    signalChangeScaling = QtCore.pyqtSignal(float)
+    signalChangeTimePoint = QtCore.Signal(float)
+    signalChangeChannel = QtCore.Signal(float)
+    signalChangeTimeRange = QtCore.Signal(float)
+    signalChangeScaling = QtCore.Signal(float)
 
     def __init__(self, *args, **kwargs):
         super(KSPlotWidget, self).__init__(*args, **kwargs)
 
     def wheelEvent(self, ev):
         delta = ev.angleDelta().y()
         if delta == 0:
```

### Comparing `kilosort-4.0.2/kilosort/gui/header_box.py` & `kilosort-4.0.3/kilosort/gui/header_box.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from kilosort import __version__
 from kilosort.gui.minor_gui_elements import help_popup_text, controls_popup_text
-from PyQt5 import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 
 class HeaderBox(QtWidgets.QWidget):
     def __init__(self, parent):
         QtWidgets.QWidget.__init__(self, parent=parent)
 
         self.gui = parent
@@ -12,24 +12,24 @@
 
         # self.kilosort_text = QtWidgets.QLabel()
         # self.kilosort_text.setText(f"Kilosort {__version__[:3]}")
         # self.kilosort_text.setFont(QtGui.QFont("Arial", 20, QtGui.QFont.Black))
 
         self.auto_load_check = QtWidgets.QCheckBox('Auto Load')
         if self.gui.auto_load:
-            self.auto_load_check.setCheckState(2)
+            self.auto_load_check.setCheckState(QtCore.Qt.CheckState.Checked)
         else:
-            self.auto_load_check.setCheckState(0)
+            self.auto_load_check.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self.auto_load_check.stateChanged.connect(self.check_auto_load)
 
         self.show_plots_check = QtWidgets.QCheckBox('Show Plots')
         if self.gui.show_plots:
-            self.show_plots_check.setCheckState(2)
+            self.show_plots_check.setCheckState(QtCore.Qt.CheckState.Checked)
         else:
-            self.show_plots_check.setCheckState(0)
+            self.show_plots_check.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self.show_plots_check.clicked.connect(self.check_show_plots)
 
         # TODO: connect the button clicks to open something in browser instead?
         #       like the paper and/or wiki.
         self.controls_button = QtWidgets.QPushButton("Controls")
         self.controls_button.setToolTip(controls_popup_text)
         #self.controls_button.clicked.connect(self.show_controls_popup)
@@ -51,21 +51,21 @@
         self.layout.addWidget(self.help_button)
         self.layout.addWidget(self.reset_gui_button)
         self.layout.addWidget(self.clear_cache_button)
 
         self.setLayout(self.layout)
 
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def check_auto_load(self):
         self.gui.auto_load = self.auto_load_check.isChecked()
         self.gui.qt_settings.setValue('auto_load', self.gui.auto_load)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def check_show_plots(self):
         self.gui.show_plots = self.show_plots_check.isChecked()
         self.gui.qt_settings.setValue('show_plots', self.gui.show_plots)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def clear_cache(self):
         self.gui.qt_settings.clear()
```

### Comparing `kilosort-4.0.2/kilosort/gui/logger.py` & `kilosort-4.0.3/kilosort/gui/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sys
 
-from PyQt5 import QtCore
+from qtpy import QtCore
 
 
 class QtHandler(logging.Handler):
     def __init__(self):
         logging.Handler.__init__(self)
 
     def emit(self, record):
@@ -13,15 +13,15 @@
         if record:
             XStream.stdout().write(f"{record}")
 
 
 class XStream(QtCore.QObject):
     _stdout = None
     _stderr = None
-    messageWritten = QtCore.pyqtSignal(str)
+    messageWritten = QtCore.Signal(str)
 
     def flush(self):
         pass
 
     def fileno(self):
         return -1
```

### Comparing `kilosort-4.0.2/kilosort/gui/main.py` & `kilosort-4.0.3/kilosort/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     RunBox,
     SettingsBox,
     DataConversionBox
 )
 from kilosort.gui.logger import setup_logger
 from kilosort.io import BinaryFiltered
 from kilosort.utils import DOWNLOADS_DIR, download_probes
-from PyQt5 import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 logger = setup_logger(__name__)
 
 
 class KiloSortGUI(QtWidgets.QMainWindow):
     def __init__(self, application, filename=None, device=None,
                  **kwargs):
@@ -28,15 +28,17 @@
         if device is None:
             if torch.cuda.is_available():
                 device = torch.device('cuda')
             else:
                 device = torch.device('cpu')
         self.device = device
 
-        if (filename is None) and self.qt_settings.contains('data_file_path'):
+        if filename is not None:
+            filename = Path(filename)
+        elif (filename is None) and self.qt_settings.contains('data_file_path'):
             filename = self.qt_settings.value('data_file_path')
         self.data_path = filename
 
         if self.qt_settings.contains('probe_layout'):
             self.probe_layout = self.qt_settings.value('probe_layout')
         else:
             self.probe_layout = None
@@ -150,18 +152,14 @@
                 self.shift_data(time_shift=-1)
             elif event.key() == QtCore.Qt.Key_Right:
                 self.shift_data(time_shift=1)
             elif event.key() == QtCore.Qt.Key_1:
                 self.toggle_mode("raw")
             elif event.key() == QtCore.Qt.Key_2:
                 self.toggle_mode("whitened")
-            elif event.key() == QtCore.Qt.Key_3:
-                self.toggle_mode("prediction")
-            elif event.key() == QtCore.Qt.Key_4:
-                self.toggle_mode("residual")
             else:
                 pass
             event.accept()
         else:
             event.ignore()
 
     def dragEnterEvent(self, event):
@@ -275,15 +273,15 @@
         if mode == "raw":
             self.data_view_box.raw_button.click()
         elif mode == "whitened":
             self.data_view_box.whitened_button.click()
         else:
             raise ValueError("Invalid mode requested!")
 
-    @QtCore.pyqtSlot(bool)
+    @QtCore.Slot(bool)
     def disable_all_input(self, value):
         self.settings_box.disable_all_input(value)
         self.run_box.disable_all_input(value)
 
     def load_data(self):
         self.set_parameters()
         self.do_load()
@@ -303,25 +301,27 @@
         assert params
 
         self.params = params
 
     def do_load(self):
         self.disable_all_input(True)
         QtWidgets.QApplication.setOverrideCursor(QtGui.QCursor(QtCore.Qt.CursorShape.WaitCursor))
-
-        self.prepare_for_new_context()
-        self.setup_context()
-        self.load_binary_files()
-        self.update_probe_view()
-        self.setup_data_view()
-        self.update_run_box()
-
-        self.disable_all_input(False)
-        self.data_view_box.whitened_button.click()
-        QtWidgets.QApplication.restoreOverrideCursor()
+        try:
+            self.prepare_for_new_context()
+            self.setup_context()
+            self.load_binary_files()
+            self.update_probe_view()
+            self.setup_data_view()
+            self.update_run_box()
+            self.data_view_box.whitened_button.click()
+        except Exception as e:
+            print(e)
+        finally:
+            self.disable_all_input(False)
+            QtWidgets.QApplication.restoreOverrideCursor()
 
     def load_binary_files(self):
         n_channels = self.params["n_chan_bin"]
         sample_rate = self.params["fs"]
         chan_map = self.probe_layout["chanMap"]
         xc = self.probe_layout["xc"]
         yc = self.probe_layout["yc"]
@@ -415,41 +415,41 @@
             data_path=self.data_path,
         )
 
     def setup_context_for_run(self):
         self.load_data()
         self.context["params"] = self.params
 
-    @QtCore.pyqtSlot(object)
+    @QtCore.Slot(object)
     def update_context(self, context):
         self.context = context
         self.update_probe_view()
         self.update_data_view()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def update_probe_view(self):
         self.probe_view_box.set_layout(self.context)
 
     def update_data_view(self):
         self.data_view_box.set_whitening_matrix(self.context.whitening_matrix)
         self.data_view_box.update_plot(self.context)
 
     def update_run_box(self):
         self.run_box.set_data_path(self.data_path)
         self.run_box.set_results_directory(self.results_directory)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def disable_run(self):
         self.run_box.disable_all_buttons()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def enable_run(self):
         self.run_box.reenable_buttons()
 
-    @QtCore.pyqtSlot(dict)
+    @QtCore.Slot(dict)
     def update_sorting_status(self, status_dict):
         self.run_box.change_sorting_status(status_dict)
         self.data_view_box.change_sorting_status(status_dict)
         self.probe_view_box.change_sorting_status(status_dict)
 
     def get_context(self):
         return self.context
@@ -488,17 +488,15 @@
 
             if self.context.filt_binary_file is not None:
                 self.context.filt_binary_file.close()
 
     def reset_gui(self):
         self.num_channels = None
         self.context = None
-
         self.close_binary_files()
-
         self.probe_view_box.reset()
         self.data_view_box.reset()
         self.settings_box.reset()
         self.message_log_box.reset()
 
     def closeEvent(self, event: QtGui.QCloseEvent):
         self.message_log_box.save_log_file()
```

### Comparing `kilosort-4.0.2/kilosort/gui/message_log_box.py` & `kilosort-4.0.3/kilosort/gui/message_log_box.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 from pathlib import Path
+import pprint
 
 from kilosort.gui.logger import XStream
-from PyQt5 import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 
 class MessageLogBox(QtWidgets.QGroupBox):
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
         self.setTitle("Message Log Box")
         self.gui = parent
         self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.log_box = QtWidgets.QPlainTextEdit()
         self.log_box.setReadOnly(True)
-        self.log_box.setLineWrapMode(200)
+        self.log_box.setLineWrapMode(QtWidgets.QPlainTextEdit.WidgetWidth) 
         self.log_box.setFont(QtGui.QFont("Monospace"))
-        self.layout.addWidget(self.log_box, 0, 0, 1, 2)
+        self.layout.addWidget(self.log_box, 0, 0, 1, 3)
 
         self.popout_button = QtWidgets.QPushButton('Show More')
         self.popout_button.clicked.connect(self.show_log_popout)
         self.layout.addWidget(self.popout_button, 1, 0, 1, 1)
         self.popout_window = ExpandedLog()
 
-        self.dump_button = QtWidgets.QPushButton('Dump Settings')
-        self.dump_button.clicked.connect(self.dump_settings)
-        self.layout.addWidget(self.dump_button, 1, 1, 1, 1)
+        self.dump_settings_button = QtWidgets.QPushButton('Dump Settings')
+        self.dump_settings_button.clicked.connect(self.dump_settings)
+        self.layout.addWidget(self.dump_settings_button, 1, 1, 1, 1)
+
+        self.dump_probe_button = QtWidgets.QPushButton('Dump Probe')
+        self.dump_probe_button.clicked.connect(self.dump_probe)
+        self.layout.addWidget(self.dump_probe_button, 1, 2, 1, 1)
 
         log_box_document = self.log_box.document()
         default_font = log_box_document.defaultFont()
         default_font.setPointSize(8)
         log_box_document.setDefaultFont(default_font)
 
         XStream.stdout().messageWritten.connect(self.update_text)
         XStream.stderr().messageWritten.connect(self.update_text)
 
 
-    @QtCore.pyqtSlot(str)
+    @QtCore.Slot(str)
     def update_text(self, text):
         self.log_box.moveCursor(QtGui.QTextCursor.End)
         self.log_box.appendPlainText(text)
         self.log_box.ensureCursorVisible()
         self.popout_window.update_text(text)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def show_log_popout(self):
         self.popout_window.show()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def dump_settings(self):
         # For debugging purposes, check for mismatch between displayed parameter
         # values and the values that are actually being used.
-        settings_text = str(self.gui.settings_box.settings)
+        settings_text = "settings = "
+        settings = self.gui.settings_box.settings.copy()
+        settings['probe'] = '... (use dump probe)'
+        s = pprint.pformat(settings, indent=4, sort_dicts=False)
+        settings_text += s[0] + '\n ' + s[1:-1] + '\n' + s[-1]
+
         self.update_text(settings_text)
 
+    @QtCore.Slot()
+    def dump_probe(self):
+        # For debugging purposes, make sure probe is loaded correctly.
+        probe_text = "probe = "
+        probe = self.gui.settings_box.settings['probe']
+        p = pprint.pformat(probe, indent=4, sort_dicts=False)
+        # insert `np.` so that text can be copied directly to code
+        p = 'np.array'.join(p.split('array'))
+        p = 'dtype=np.'.join(p.split('dtype='))
+        probe_text += p[0] + '\n ' + p[1:-1] + '\n' + p[-1]
+
+        self.update_text(probe_text)
+
     def prepare_for_new_context(self):
         self.save_log_file()
         self.log_box.clear()
 
     def save_log_file(self):
         context = self.get_context()
         if context is not None:
@@ -80,19 +103,19 @@
     def __init__(self):
         super().__init__()
 
         self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.log_box = QtWidgets.QPlainTextEdit()
         self.log_box.setReadOnly(True)
-        self.log_box.setLineWrapMode(400)
+        self.log_box.setLineWrapMode(QtWidgets.QPlainTextEdit.WidgetWidth) 
         self.log_box.setFont(QtGui.QFont("Monospace"))
         self.layout.addWidget(self.log_box, 0, 0, 1, 1)
         
-        center = QtWidgets.QDesktopWidget().availableGeometry().center()
+        center = QtWidgets.QApplication.screens()[0].availableGeometry().center()
         self.setGeometry(0, 0, 800, 500)
         geo = self.frameGeometry()
         geo.moveCenter(center)
         self.move(geo.topLeft())
 
     def update_text(self, text):
         self.log_box.moveCursor(QtGui.QTextCursor.End)
```

### Comparing `kilosort-4.0.2/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.3/kilosort/gui/minor_gui_elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from kilosort.gui.logger import setup_logger
-from PyQt5 import QtGui, QtWidgets
+from qtpy import QtGui, QtWidgets, QtCore
 
 logger = setup_logger(__name__)
 
 
 def create_prb(probe):
     chan_map = np.array(probe["chanMap"])
     xc, yc = np.array(probe["xc"]), np.array(probe["yc"])
@@ -31,32 +31,35 @@
     return probe_prb
 
 
 class ProbeBuilder(QtWidgets.QDialog):
     def __init__(self, parent, *args, **kwargs):
         super(ProbeBuilder, self).__init__(parent=parent, *args, **kwargs)
         self.parent = parent
+        self.setWindowFlags(
+            self.windowFlags() ^ QtCore.Qt.WindowContextHelpButtonHint
+            )
 
         self.map_name_value = QtWidgets.QLineEdit()
         self.map_name_label = QtWidgets.QLabel("Name for new channel map:")
 
         self.x_coords_value = QtWidgets.QLineEdit()
         self.x_coords_label = QtWidgets.QLabel("X-coordinates for each site:")
 
         self.y_coords_value = QtWidgets.QLineEdit()
         self.y_coords_label = QtWidgets.QLabel("Y-coordinates for each site:")
 
         self.k_coords_value = QtWidgets.QLineEdit()
         self.k_coords_label = QtWidgets.QLabel(
-            "Shrank index ('kcoords') for each " "site (leave blank for single shank):"
+            "Shank index ('kcoords') for each " "site (leave blank for single shank):"
         )
 
         self.channel_map_value = QtWidgets.QLineEdit()
         self.channel_map_label = QtWidgets.QLabel(
-            "Channel map (list of rows in the data file for each site):"
+            "Channel map (row in data file for each site, 0-indexed):"
         )
 
         self.input_list = [
             self.map_name_value,
             self.x_coords_value,
             self.y_coords_value,
             self.k_coords_value,
@@ -150,40 +153,41 @@
     def set_values_as_checked(self):
         self.values_checked = True
         self.okay_button.setDisabled(False)
 
     def check_inputs(self):
         try:
             map_name = self.map_name_value.text()
-            assert len(map_name.split()) == 1
+            assert len(map_name.split()) == 1, \
+                   'probe name cannot contain spaces'
 
             x_coords = eval(self.x_coords_value.text())
             y_coords = eval(self.y_coords_value.text())
-
             x_coords = np.array(x_coords, dtype=np.float64)
             y_coords = np.array(y_coords, dtype=np.float64)
-
-            assert len(x_coords) == len(y_coords)
+            assert len(x_coords) == len(y_coords), \
+                   'x and y positions must have same size'
 
             k_coords = self.k_coords_value.text()
             if k_coords == "":
-
                 k_coords = np.ones_like(x_coords, dtype=np.float64)
             else:
                 k_coords = np.array(eval(k_coords), dtype=np.float64)
-                assert x_coords.size == k_coords.size
+                assert x_coords.size == k_coords.size, \
+                       'contact positions and shank indices must have same size'
 
             channel_map = self.channel_map_value.text()
             if channel_map == "":
                 channel_map = np.arange(x_coords.size)
             else:
                 channel_map = np.array(eval(channel_map), dtype=np.int32)
-                assert x_coords.size == channel_map.size
-                assert channel_map.size == np.unique(channel_map).size
-                assert np.amax(channel_map) < channel_map.size
+                assert x_coords.size == channel_map.size, \
+                       'contact positions and channel map must be same size'
+                assert channel_map.size == np.unique(channel_map).size, \
+                       'channel map cannot contain repeats'
 
         except Exception as e:
             self.error_label.setText(str(e))
             self.error_label.show()
 
         else:
             self.map_name = map_name
@@ -219,18 +223,17 @@
 
 
 controls_popup_text = """
 <font style="font-family:Monospace">
 GUI Controls <br>
 ------------ <br>
 <br>
-[1 2 3 4]        - activate/deactivate raw/filtered/prediction/residual views of the dataset <br>
-[up/down]        - move through channels in traces mode <br>
+[1 2]        - activate/deactivate raw/filtered views of the dataset <br>
 [scroll]         - move forward/backward in time <br>
-[ctrl + scroll]  - add/remove channels in colormap mode; slide up/down probe in traces mode <br>
+[ctrl + scroll]  - add/remove channels in colormap mode;
 [alt + scroll]   - change data/colormap scaling <br>
 [shift + scroll] - zoom in/out in time <br>
 [left click]     - move forward/backward in time <br>
 <br>
 Mouse Controls for Plots <br>
 ------------------------ <br>
 <br>
@@ -240,15 +243,14 @@
 </font>
 """
 
 help_popup_text = """
 Welcome to Kilosort4!
 
 ##### Documentation #####
-Pykilosort is the Python port of Kilosort2, which was originally written in Matlab.
-For documentation of the underlying algorithm or the GUI, please visit https://github.com/MouseLand/Kilosort/wiki
+For documentation of the underlying algorithm or the GUI, please visit https://github.com/MouseLand/Kilosort/
 or https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1.
 
 ##### Troubleshooting #####
 1. Click 'Reset GUI' to clear any GUI problems or strange errors. If the problem persists, try 'Clear Cache' and restarting Kilosort. 
 2. If the problem persists, visit https://github.com/MouseLand/kilosort and create an issue there with as much detail about the problem as possible.  
 """
```

### Comparing `kilosort-4.0.2/kilosort/gui/palettes.py` & `kilosort-4.0.3/kilosort/gui/palettes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from PyQt5 import QtGui
+from qtpy import QtGui
 
 
 class DarkPalette(QtGui.QPalette):
     """Class that inherits from pyqtgraph.QtGui.QPalette and renders dark colours for the application."""
 
     def __init__(self):
         QtGui.QPalette.__init__(self)
```

### Comparing `kilosort-4.0.2/kilosort/gui/probe_view_box.py` & `kilosort-4.0.3/kilosort/gui/probe_view_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import pyqtgraph as pg
 from kilosort.gui.logger import setup_logger
-from PyQt5 import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 logger = setup_logger(__name__)
 
 
 class ProbeViewBox(QtWidgets.QGroupBox):
 
-    channelSelected = QtCore.pyqtSignal(int)
+    channelSelected = QtCore.Signal(int)
 
     def __init__(self, parent):
         super(ProbeViewBox, self).__init__(parent=parent)
         self.setTitle("Probe View")
         self.gui = parent
         self.probe_view = pg.PlotWidget()
         self.setup()
@@ -54,15 +54,15 @@
         self.xc, self.yc = self.active_layout["xc"], self.active_layout["yc"]
         self.channel_map_dict = {}
         for ind, (xc, yc) in enumerate(zip(self.xc, self.yc)):
             self.channel_map_dict[(xc, yc)] = ind
         self.total_channels = self.active_layout["n_chan"]
         self.channel_map = self.active_layout["chanMap"]
 
-    @QtCore.pyqtSlot(str, int)
+    @QtCore.Slot(str, int)
     def synchronize_data_view_mode(self, mode: str):
         if self.active_data_view_mode != mode:
             self.probe_view.clear()
             self.update_probe_view()
             self.active_data_view_mode = mode
 
     def change_sorting_status(self, status_dict):
@@ -81,19 +81,19 @@
             spots.append({
                 'pos': pos, 'size': size, 'pen': pen, 'brush': brush,
                 'symbol': symbol
                 })
 
         return spots
 
-    @QtCore.pyqtSlot(int, int)
+    @QtCore.Slot(int, int)
     def update_probe_view(self):
         self.create_plot()
 
-    @QtCore.pyqtSlot(object)
+    @QtCore.Slot(object)
     def preview_probe(self, probe):
         self.probe_view.clear()
         self.set_active_layout(probe)
         self.create_plot()
 
     def create_plot(self):
         spots = self.generate_spots_list()
```

### Comparing `kilosort-4.0.2/kilosort/gui/run_box.py` & `kilosort-4.0.3/kilosort/gui/run_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from PyQt5 import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from kilosort.gui.sorter import KiloSortWorker
 from kilosort.gui.sanity_plots import (
     PlotWindow, plot_drift_amount, plot_drift_scatter, plot_diagnostics,
     plot_spike_positions
     )
 
 
 class RunBox(QtWidgets.QGroupBox):
-    setupContextForRun = QtCore.pyqtSignal()
-    updateContext = QtCore.pyqtSignal(object)
-    sortingStepStatusUpdate = QtCore.pyqtSignal(dict)
-    disableInput = QtCore.pyqtSignal(bool)
+    setupContextForRun = QtCore.Signal()
+    updateContext = QtCore.Signal(object)
+    sortingStepStatusUpdate = QtCore.Signal(dict)
+    disableInput = QtCore.Signal(bool)
 
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
         self.setTitle("Run")
 
         self.parent = parent
 
@@ -66,15 +66,15 @@
         for button in self.buttons:
             button.setEnabled(False)
 
     def reenable_buttons(self):
         self.run_all_button.setEnabled(True)
         self.spike_sort_button.setEnabled(True)
         
-    @QtCore.pyqtSlot(bool)
+    @QtCore.Slot(bool)
     def disable_all_input(self, value):
         if value:
             self.disable_all_buttons()
         else:
             self.reenable_buttons()
 
     def set_data_path(self, data_path):
@@ -90,26 +90,26 @@
         self.sorting_status[step] = status
         self.sortingStepStatusUpdate.emit(self.sorting_status)
 
     def change_sorting_status(self, status_dict):
         self.sorting_status = status_dict
         self.reenable_buttons()
 
-    @QtCore.pyqtSlot(object)
+    @QtCore.Slot(object)
     def finished_spikesort(self, context):
         self.updateContext.emit(context)
         self.current_worker = None
         self.update_sorting_status("spikesort", True)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def spikesort(self):
         if self.get_current_context() is not None:
             self.run_steps("spikesort")
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def run_all(self):
         if self.get_current_context() is not None:
             self.run_steps([
                 # "preprocess",
                 "spikesort",
             ])
```

### Comparing `kilosort-4.0.2/kilosort/gui/sanity_plots.py` & `kilosort-4.0.3/kilosort/gui/sanity_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import pyqtgraph as pg
 import scipy
-import matplotlib
 import numpy as np
+import matplotlib
 import torch
-from PyQt5 import QtWidgets
+from qtpy import QtWidgets
 
 from kilosort.postprocessing import compute_spike_positions
 from kilosort.gui.palettes import PROBE_PLOT_COLORS
 
 _COLOR_CODES = ['b', 'g', 'r', 'c', 'm', 'y', 'k', 'w']
 
-
 class PlotWindow(QtWidgets.QWidget):
     def __init__(self, *args, title=None, width=500, height=400,
                  background=None, **kwargs):
         super().__init__()
         if title is not None:
             self.setWindowTitle(title)
         self.resize(width, height)
```

### Comparing `kilosort-4.0.2/kilosort/gui/settings_box.py` & `kilosort-4.0.3/kilosort/gui/settings_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import pprint
 from pathlib import Path
 import json
 
 import numpy as np
 import torch
-from PyQt5 import QtCore, QtWidgets, QtGui
+from qtpy import QtCore, QtWidgets, QtGui
 from scipy.io.matlab.miobase import MatReadError
 
 from kilosort.gui.logger import setup_logger
 from kilosort.gui.minor_gui_elements import ProbeBuilder, create_prb
 from kilosort.io import load_probe, BinaryRWFile
 from kilosort.parameters import MAIN_PARAMETERS, EXTRA_PARAMETERS
 
 
 logger = setup_logger(__name__)
 
 _DEFAULT_DTYPE = 'int16'
 _ALLOWED_FILE_TYPES = ['.bin', '.dat', '.bat', '.raw']  # For binary data
 
 class SettingsBox(QtWidgets.QGroupBox):
-    settingsUpdated = QtCore.pyqtSignal()
-    previewProbe = QtCore.pyqtSignal(object)
-    dataChanged = QtCore.pyqtSignal()
+    settingsUpdated = QtCore.Signal()
+    previewProbe = QtCore.Signal(object)
+    dataChanged = QtCore.Signal()
 
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
 
         self.gui = parent
         self.load_enabled = False
         self.use_file_object = False
@@ -178,41 +178,41 @@
         layout.addWidget(
             self.probe_preview_button, row_count, col2, rspan, cspan2)
         self.probe_preview_button.setDisabled(True)
         self.probe_preview_button.clicked.connect(self.show_probe_layout)
 
         row_count += rspan
         layout.addWidget(self.probe_layout_selector, row_count, col1, rspan, dbl)
-        self.probe_layout_selector.setSizeAdjustPolicy(
-            QtWidgets.QComboBox.AdjustToMinimumContentsLength
-        )
+        #self.probe_layout_selector.setSizeAdjustPolicy(
+        #    QtWidgets.QComboBox.AdjustToMinimumContentsLength
+        #)
         self.probe_layout_selector.currentTextChanged.connect(
             self.on_probe_layout_selected
         )
 
         # Add small vertical space for visual grouping
         row_count += rspan
         layout.addWidget(QtWidgets.QWidget(), row_count, 0, 1, dbl)
         row_count += 1
 
         layout.addWidget(self.dtype_selector_text, row_count, col1, rspan, cspan1)
         layout.addWidget(self.dtype_selector, row_count, col2, rspan, cspan2)
-        self.dtype_selector.setSizeAdjustPolicy(
-            QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
-        )
+        #self.dtype_selector.setSizeAdjustPolicy(
+        #    QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
+        #)
         self.dtype_selector.currentTextChanged.connect(
             self.on_data_dtype_selected
         )
 
         row_count += rspan
         layout.addWidget(self.device_selector_text, row_count, col1, rspan, cspan1)
         layout.addWidget(self.device_selector, row_count, col2, rspan, cspan2)
-        self.device_selector.setSizeAdjustPolicy(
-            QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
-        )
+        #self.device_selector.setSizeAdjustPolicy(
+        #    QtWidgets.QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLength
+        #)
         self.device_selector.currentTextChanged.connect(
             self.on_device_selected
         )
 
         for k in list(MAIN_PARAMETERS.keys()):
             row_count += rspan
             layout.addWidget(
@@ -277,15 +277,15 @@
                 d = str(self.gui.qt_settings.value(k))
             else:
                 # Use default value
                 d = str(p['default'])
             getattr(epw, f'{k}_input').setText(d)
             getattr(epw, f'{k}_input').editingFinished.emit()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def import_settings(self):
         # 1) open file dialog
         file_dialog_options = QtWidgets.QFileDialog.DontUseNativeDialog
         settings_file_name, _ = QtWidgets.QFileDialog.getOpenFileName(
             parent=self,
             caption="Choose .json file to load settings from...",
             directory=os.path.expanduser("~"),
@@ -306,15 +306,15 @@
             getattr(epw, f'{k}_input').editingFinished.emit()
 
         self.dtype_selector.setCurrentIndex(settings['misc']['dtype_idx'])
         self.probe_layout_selector.setCurrentIndex(settings['misc']['probe_idx'])
         self.device_selector.setCurrentIndex(settings['misc']['device_idx'])
 
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def export_settings(self):
         # 1) dump parameters to dict
         #       don't save entire settings dict, other stuff is data-specific
         settings = {'main': {}, 'extra': {}, 'misc': {}}
         for k in list(MAIN_PARAMETERS.keys()):
             settings['main'][k] = getattr(self, k)
         for k in list(EXTRA_PARAMETERS.keys()):
@@ -470,45 +470,45 @@
             self.settings[k] = getattr(self, k)
         for k in list(EXTRA_PARAMETERS.keys()):
             self.settings[k] = getattr(self.extra_parameters_window, k)
 
         if not self.check_valid_binary_path(self.data_file_path):
             return False
 
-        none_allowed = ['dmin', 'dminx', 'nt0min']
+        none_allowed = ['dmin', 'nt0min']
         for k, v in self.settings.items():
             if v is None and k not in none_allowed:
                 return False
         return True
     
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def update_parameter(self):
         parameter_key = self.sender().var_name
         parameter_info = MAIN_PARAMETERS[parameter_key]
         _check_parameter(self, self, parameter_key, parameter_info)
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def update_settings(self):
         if self.check_settings():
             if not self.results_directory_path.exists():
                 try:
                     os.makedirs(self.results_directory_path)
                     self.settingsUpdated.emit()
                 except Exception as e:
                     logger.exception(e)
                     self.disable_load()
 
             else:
                 self.settingsUpdated.emit()
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def show_probe_layout(self):
         self.previewProbe.emit(self.probe_layout)
 
-    @QtCore.pyqtSlot(str)
+    @QtCore.Slot(str)
     def on_probe_layout_selected(self, name):
         if name not in ["", "[new]", "other..."]:
             probe_path = Path(self.gui.new_probe_files_path).joinpath(name)
             try:
                 probe_layout = load_probe(probe_path)
                 self.save_probe_selection(probe_layout, probe_path.name)
 
@@ -772,20 +772,20 @@
             layout.addWidget(getattr(self, f'{k}_text'), row_count, col, 1, 3)
             layout.addWidget(getattr(self, f'{k}_input'), row_count, col+3, 1, 2)
             inp = getattr(self, f'{k}_input')
             inp.editingFinished.connect(self.update_parameter)
 
         self.setLayout(layout)
 
-        center = QtWidgets.QDesktopWidget().availableGeometry().center()
+        center = QtWidgets.QApplication.screens()[0].availableGeometry().center()
         geo = self.frameGeometry()
         geo.moveCenter(center)
         self.move(geo.topLeft())
 
-    @QtCore.pyqtSlot()
+    @QtCore.Slot()
     def update_parameter(self):
         parameter_key = self.sender().var_name
         parameter_info = EXTRA_PARAMETERS[parameter_key]
         _check_parameter(self, self.main_settings, parameter_key, parameter_info)
 
 
 def _check_parameter(sender_obj, main_obj, k, p):
```

### Comparing `kilosort-4.0.2/kilosort/gui/sorter.py` & `kilosort-4.0.3/kilosort/gui/sorter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import time
 
 import numpy as np
 import torch
-from PyQt5 import QtCore
+from qtpy import QtCore
 
 from kilosort.gui.logger import setup_logger
 from kilosort.run_kilosort import (
     initialize_ops, compute_preprocessing, compute_drift_correction,
     detect_spikes, cluster_spikes, save_sorting
     )
 
 logger = setup_logger(__name__)
 
 
 class KiloSortWorker(QtCore.QThread):
-    finishedPreprocess = QtCore.pyqtSignal(object)
-    finishedSpikesort = QtCore.pyqtSignal(object)
-    finishedAll = QtCore.pyqtSignal(object)
-    progress_bar = QtCore.pyqtSignal(int)
-    plotDataReady = QtCore.pyqtSignal(str)
+    finishedPreprocess = QtCore.Signal(object)
+    finishedSpikesort = QtCore.Signal(object)
+    finishedAll = QtCore.Signal(object)
+    progress_bar = QtCore.Signal(int)
+    plotDataReady = QtCore.Signal(str)
 
     def __init__(self, context, results_directory, steps,
                  device=torch.device('cuda'), file_object=None, *args, **kwargs):
         super(KiloSortWorker, self).__init__(*args, **kwargs)
         self.context = context
         self.data_path = context.data_path
         self.results_directory = results_directory
```

### Comparing `kilosort-4.0.2/kilosort/hierarchical.py` & `kilosort-4.0.3/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/io.py` & `kilosort-4.0.3/kilosort/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 from scipy.io import loadmat
 import numpy as np
 import torch
 from torch.fft import fft, ifft, fftshift
 
 from kilosort import CCG
 from kilosort.preprocessing import get_drift_matrix, fft_highpass
-from kilosort.postprocessing import remove_duplicates, compute_spike_positions
+from kilosort.postprocessing import (
+    remove_duplicates, compute_spike_positions, make_pc_features
+    )
+
+_torch_warning = ".*PyTorch does not support non-writable tensors"
 
 
 def find_binary(data_dir: Union[str, os.PathLike]) -> Path:
     """Find binary file in `data_dir`."""
 
     data_dir = Path(data_dir)
     filenames = list(data_dir.glob('*.bin')) + list(data_dir.glob('*.bat')) \
@@ -191,14 +195,27 @@
     templates = (Wall.unsqueeze(-1).cpu() * ops['wPCA'].cpu()).sum(axis=-2).numpy()
     templates = templates.transpose(0,2,1)
     templates_ind = np.tile(np.arange(Wall.shape[1])[np.newaxis, :], (templates.shape[0],1))
     np.save((results_dir / 'similar_templates.npy'), similar_templates)
     np.save((results_dir / 'templates.npy'), templates)
     np.save((results_dir / 'templates_ind.npy'), templates_ind)
     
+    # pc features
+    if save_extra_vars:
+        # Save tF first since it gets updated in-place
+        np.save(results_dir / 'tF.npy', tF.cpu().numpy())
+    # This will momentarily copy tF which is pretty large, but it's on CPU
+    # so the extra memory hopefully won't be an issue.
+    tF = tF[kept_spikes]
+    pc_features, pc_feature_ind = make_pc_features(
+        ops, spike_templates, spike_clusters, tF
+        )
+    np.save(results_dir / 'pc_features.npy', pc_features)
+    np.save(results_dir / 'pc_feature_ind.npy', pc_feature_ind)
+
     # contamination ratio
     acg_threshold = ops['settings']['acg_threshold']
     ccg_threshold = ops['settings']['ccg_threshold']
     is_ref, est_contam_rate = CCG.refract(spike_clusters, spike_times / ops['fs'],
                                           acg_threshold=acg_threshold,
                                           ccg_threshold=ccg_threshold)
 
@@ -227,22 +244,27 @@
             'sample_rate': ops['settings']['fs'],
             'hp_filtered': False }
     with open((results_dir / 'params.py'), 'w') as f: 
         for key in params.keys():
             f.write(f'{key} = {params[key]}\n')
 
     if save_extra_vars:
-        # Also save tF and Wall, for easier debugging/analysis
-        np.save(results_dir / 'tF.npy', tF.cpu().numpy())
+        # Also save Wall, for easier debugging/analysis
         np.save(results_dir / 'Wall.npy', Wall.cpu().numpy())
         # And full st, clu, amp arrays with no spikes removed
         np.save(results_dir / 'full_st.npy', st)
         np.save(results_dir / 'full_clu.npy', clu)
         np.save(results_dir / 'full_amp.npy', amplitudes)
 
+    # Remove cached .phy results if present from running Phy on a previous
+    # version of results in the same directory.
+    phy_cache_path = Path(results_dir / '.phy')
+    if phy_cache_path.is_dir():
+        shutil.rmtree(phy_cache_path)
+
     return results_dir, similar_templates, is_ref, est_contam_rate
 
 
 def save_ops(ops, results_dir=None):
     """Save intermediate `ops` dictionary to `results_dir/ops.npy`."""
 
     if results_dir is None:
@@ -309,15 +331,15 @@
 
         * always assume int16 files *
 
         adapted from https://github.com/MouseLand/suite2p/blob/main/suite2p/io/binary.py
         
         Parameters
         ----------
-        filename : str
+        filename : str or Path
             The filename of the file to read from or write to
         n_chan_bin : int
             number of channels
         file_object : array-like file object; optional.
             Must have 'shape' and 'dtype' attributes and support array-like
             indexing (e.g. [:100,:], [5, 7:10], etc). For example, a numpy
             array or memmap.
@@ -489,25 +511,32 @@
         # Shift data to +/- 2**15
         if self.dtype == 'uint16':
             data = data.astype('float32')
             data = data - 2**15
 
         nsamp = data.shape[-1]
         X = torch.zeros((self.n_chan_bin, self.NT + 2*self.nt), device=self.device)
-        # fix the data at the edges for the first and last batch
-        if ibatch == 0:
-            X[:, self.nt : self.nt+nsamp] = torch.from_numpy(data).to(self.device).float()
-            X[:, :self.nt] = X[:, self.nt : self.nt+1]
-            bstart = self.imin - self.nt
-        elif ibatch == self.n_batches-1:
-            X[:, :nsamp] = torch.from_numpy(data).to(self.device).float()
-            X[:, nsamp:] = X[:, nsamp-1:nsamp]
-            bend += self.nt
-        else:
-            X[:] = torch.from_numpy(data).to(self.device).float()
+
+        with warnings.catch_warnings():
+            # Don't need this, we know about the warning and it doesn't cause
+            # any problems. Doing this the "correct" way is much slower.
+            warnings.filterwarnings("ignore", message=_torch_warning)
+
+            # fix the data at the edges for the first and last batch
+            if ibatch == 0:
+                X[:, self.nt : self.nt+nsamp] = torch.from_numpy(data).to(self.device).float()
+                X[:, :self.nt] = X[:, self.nt : self.nt+1]
+                bstart = self.imin - self.nt
+            elif ibatch == self.n_batches-1:
+                X[:, :nsamp] = torch.from_numpy(data).to(self.device).float()
+                X[:, nsamp:] = X[:, nsamp-1:nsamp]
+                bend += self.nt
+            else:
+                X[:] = torch.from_numpy(data).to(self.device).float()
+    
         inds = [bstart, bend]
         if return_inds:
             return X, inds
         else:
             return X
         
 
@@ -652,15 +681,19 @@
                 X = (M @ self.whiten_mat) @ X
             else:
                 X = self.whiten_mat @ X
         return X
 
     def __getitem__(self, *items):
         samples = super().__getitem__(*items)
-        X = torch.from_numpy(samples.T).to(self.device).float()
+        with warnings.catch_warnings():
+            # Don't need this, we know about the warning and it doesn't cause
+            # any problems. Doing this the "correct" way is much slower.
+            warnings.filterwarnings("ignore", message=_torch_warning)
+            X = torch.from_numpy(samples.T).to(self.device).float()
         return self.filter(X)
         
     def padded_batch_to_torch(self, ibatch, ops=None, return_inds=False):
         if return_inds:
             X, inds = super().padded_batch_to_torch(ibatch, return_inds=return_inds)
             return self.filter(X, ops, ibatch), inds
         else:
```

### Comparing `kilosort-4.0.2/kilosort/parameters.py` & `kilosort-4.0.3/kilosort/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,16 @@
     # NOTE: if left as None, will be set to `int(20 * settings['nt']/61)`
     'nt0min': {
         'gui_name': 'nt0min', 'type': int, 'min': 0, 'max': np.inf,
         'exclude': [], 'default': None, 'step': 'spike detection',
         'description': 
             """
             Sample index for aligning waveforms, so that their minimum 
-            or maximum value happens here. Default of 20.
+            or maximum value happens here. Defaults to 
+            `int(20 * settings['nt']/61)`.
             """
     },
 
     'dmin': {
         'gui_name': 'dmin', 'type': float, 'min': 0, 'max': np.inf,
         'exclude': [0], 'default': None, 'step': 'spike detection',
         'description':
@@ -183,19 +184,21 @@
             Vertical spacing of template centers used for spike detection,
             in microns. Determined automatically by default.
             """
     },
 
     'dminx': {
         'gui_name': 'dminx', 'type': float, 'min': 0, 'max': np.inf,
-        'exclude': [0], 'default': None, 'step': 'spike detection',
+        'exclude': [0], 'default': 32, 'step': 'spike detection',
         'description':
             """
             Horizontal spacing of template centers used for spike detection,
-            in microns. Determined automatically by default.
+            in microns. The default 32um should work well for Neuropixels 1 and
+            Neuropixels 2 probes. For other probe geometries, try setting this 
+            to the median lateral distance between contacts to start.
             """
     },
 
     'min_template_size': {
         'gui_name': 'min template size', 'type': float, 'min': 0, 'max': np.inf,
         'exclude': [0], 'default': 10, 'step': 'spike detection',
         'description':
```

### Comparing `kilosort-4.0.2/kilosort/preprocessing.py` & `kilosort-4.0.3/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/run_kilosort.py` & `kilosort-4.0.3/kilosort/run_kilosort.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,17 +508,18 @@
     is_ref, est_contam_rate = CCG.refract(clu, st / ops['fs'],
                                           acg_threshold=acg_threshold,
                                           ccg_threshold=ccg_threshold)
 
     results = [ops, st, clu, similar_templates, is_ref, est_contam_rate]
 
     if load_extra_vars:
+        # NOTE: tF and Wall always go on CPU, not CUDA
         tF = np.load(results_dir / 'tF.npy')
-        tF = torch.from_numpy(tF).to(device)
+        tF = torch.from_numpy(tF)
         Wall = np.load(results_dir / 'Wall.npy')
-        Wall = torch.from_numpy(Wall).to(device)
+        Wall = torch.from_numpy(Wall)
         full_st = np.load(results_dir / 'full_st.npy')
         full_clu = np.load(results_dir / 'full_clu.npy')
         full_amp = np.load(results_dir / 'full_amp.npy')
         results.extend([tF, Wall, full_st, full_clu, full_amp])
 
     return results
```

### Comparing `kilosort-4.0.2/kilosort/simulation.py` & `kilosort-4.0.3/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/spikedetect.py` & `kilosort-4.0.3/kilosort/spikedetect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from io import StringIO
-import time
+import warnings
+
 from torch.nn.functional import max_pool2d, avg_pool2d, conv1d, max_pool1d
 import numpy as np
 import torch
 from sklearn.cluster import KMeans
 from sklearn.decomposition import TruncatedSVD
 from tqdm import tqdm
 
@@ -79,40 +80,28 @@
 def get_waves(ops, device=torch.device('cuda')):
     dd = np.load(template_path())
     wTEMP = torch.from_numpy(dd['wTEMP']).to(device)
     wPCA = torch.from_numpy(dd['wPCA']).to(device)
     return wPCA, wTEMP
 
 def template_centers(ops):
-    xmin, xmax, ymin, ymax = ops['xc'].min(), ops['xc'].max(), ops['yc'].min(), ops['yc'].max()
-    dmin = ops['settings'].get('dmin', None)
+    xmin, xmax, ymin, ymax = ops['xc'].min(), ops['xc'].max(), \
+                             ops['yc'].min(), ops['yc'].max()
+
+    dmin = ops['settings']['dmin']
     if dmin is None:
         # Try to determine a good value automatically based on contact positions.
         dmin = np.median(np.diff(np.unique(ops['yc'])))
     ops['dmin'] = dmin
     ops['yup'] = np.arange(ymin, ymax+.00001, dmin//2)
 
-    dminx = ops['settings'].get('dminx', None)
-    if dminx is None:
-        # Try to determine a good value automatically.
-        yunq = np.unique(ops['yc'])
-        mxc = np.NaN * np.ones(len(yunq))
-        for j in range(len(yunq)):
-            xc = ops['xc'][ops['yc']==yunq[j]]
-            if len(xc)>1:
-                mxc[j] = np.median(np.diff(np.sort(xc)))
-            else:
-                mxc[j] = 0
-        dminx = np.nanmedian(mxc)
-        dminx = np.maximum(1, dminx)
-    ops['dminx'] = dminx
-
+    ops['dminx'] = dminx = ops['settings']['dminx']
     nx = np.round((xmax - xmin) / (dminx/2)) + 1
-    
     ops['xup'] = np.linspace(xmin, xmax, int(nx))
+
     return ops
 
 
 def template_match(X, ops, iC, iC2, weigh, device=torch.device('cuda')):
     NT = X.shape[-1]
     nt = ops['nt']
     Nchan = ops['Nchan']
@@ -121,15 +110,15 @@
     tch0 = torch.zeros(1,device = device)
     tch1 = torch.ones(1,device = device)
 
     W = ops['wTEMP'].unsqueeze(1)
     B = conv1d(X.unsqueeze(1), W, padding=nt//2)
 
     nt0 = ops['settings']['nt0min']
-    nk = ops['settings']['n_pcs']
+    nk = ops['settings']['n_templates']
 
     niter = 40
     nb = (NT-1)//niter+1
     As    = torch.zeros((Nfilt, NT), device=device)
     Amaxs = torch.zeros((Nfilt, NT), device=device)
     imaxs = torch.zeros((Nfilt, NT), dtype = torch.int64, device=device)
 
@@ -211,18 +200,31 @@
 
     nC = ops['settings']['nearest_chans']
     nC2 = ops['settings']['nearest_templates']
     iC, ds = nearest_chans(ys, yc, xs, xc, nC, device=device)
     iC2, ds2 = nearest_chans(ys, ys, xs, xs, nC2, device=device)
 
     ds_torch = torch.from_numpy(ds).to(device).float()
-    weigh = torch.exp(- ds_torch.unsqueeze(-1) / (sig * (1+torch.arange(nsizes, device = device)))**2)
+    template_sizes = sig * (1+torch.arange(nsizes, device=device))
+    weigh = torch.exp(-ds_torch.unsqueeze(-1) / template_sizes**2)
     weigh = torch.permute(weigh, (2, 0, 1)).contiguous()
     weigh = weigh / (weigh**2).sum(1).unsqueeze(1)**.5
 
+    nan_weights = torch.isnan(weigh)
+    zero_weights = (weigh == 0)
+    if (nan_weights.sum() > 0) or (zero_weights.sum() > 0):
+        msg = """
+              NaNs and/or zeroes present in weights for spikedetect.run,
+              may need to adjust `min_template_size` and/or `dminx` 
+              for best results.\n
+              If you're using a probe with multiple shanks, see 
+              https://kilosort.readthedocs.io/en/latest/multi_shank.html
+              """
+        warnings.warn(msg, UserWarning)
+
     st = np.zeros((10**6, 6), 'float64')
     tF = np.zeros((10**6, nC , ops['settings']['n_pcs']), 'float32')
 
     k = 0
     nt = ops['nt']
     tarange = torch.arange(-(nt//2),nt//2+1, device = device)
     s = StringIO()
```

### Comparing `kilosort-4.0.2/kilosort/swarmsplitter.py` & `kilosort-4.0.3/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort/template_matching.py` & `kilosort-4.0.3/kilosort/template_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         nsp = len(stt)   
         if k+nsp>st.shape[0]:                     
             st = np.concatenate((st, np.zeros_like(st)), 0)
             tF  = torch.cat((tF,  torch.zeros_like(tF)), 0)
 
         stt = stt.double()
         #st[k:k+nsp,0] = ((stt[:,0]-nt)/ops['fs'] + ibatch * (ops['batch_size']/ops['fs'])).cpu().numpy()
-        st[k:k+nsp,0] = ((stt[:,0]-nt) + ibatch * (ops['batch_size'])).cpu().numpy() - nt//2 + ops['nt0min']
+        left_pad = 0 if ibatch == 0 else nt
+        st[k:k+nsp,0] = ((stt[:,0]-left_pad) + ibatch * (ops['batch_size'])).cpu().numpy() - nt//2 + ops['nt0min']
 
         st[k:k+nsp,1] = stt[:,1].cpu().numpy()
         st[k:k+nsp,2] = amps[:,0].cpu().numpy()
         
         tF[k:k+nsp]  = xfeat.transpose(0,1).cpu()#.numpy()
 
         k+= nsp
```

### Comparing `kilosort-4.0.2/kilosort/utils.py` & `kilosort-4.0.3/kilosort/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os, tempfile, shutil, pathlib
 from tqdm import tqdm
 from urllib.request import urlopen
+from urllib.error import HTTPError
 
 _DOWNLOADS_URL = 'https://www.kilosort.org/downloads'
 _DOWNLOADS_DIR_ENV = os.environ.get("KILOSORT_LOCAL_DOWNLOADS_PATH")
 _DOWNLOADS_DIR_DEFAULT = pathlib.Path.home().joinpath('.kilosort')
 DOWNLOADS_DIR = pathlib.Path(_DOWNLOADS_DIR_ENV) if _DOWNLOADS_DIR_ENV else _DOWNLOADS_DIR_DEFAULT
 PROBE_DIR = DOWNLOADS_DIR.joinpath('probes')
 
@@ -35,15 +36,19 @@
         probe_dir = PROBE_DIR
     probe_dir.mkdir(parents=True, exist_ok=True)
     for probe_name in probe_names:
         url = f'{_DOWNLOADS_URL}/{probe_name}'
         cached_file = os.fspath(probe_dir.joinpath(probe_name)) 
         if not os.path.exists(cached_file):
             print('Downloading: "{}" to {}\n'.format(url, cached_file))
-            download_url_to_file(url, cached_file, progress=True)
+            try:
+                download_url_to_file(url, cached_file, progress=True)
+            except HTTPError as e:
+                print(f'Unable to download probe {probe_name}, error:')
+                print(e)
 
 
 def download_url_to_file(url, dst, progress=True):
     r"""Download object at the given URL to a local path.
             Thanks to torch, slightly modified
     Args:
         url (string): URL of the object to download
```

### Comparing `kilosort-4.0.2/kilosort/wTEMP.npz` & `kilosort-4.0.3/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.3/kilosort.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.2
+Version: 4.0.3
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,26 +17,29 @@
 Requires-Dist: tqdm
 Requires-Dist: torch>=1.6
 Requires-Dist: numba
 Requires-Dist: faiss-cpu
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: myst_parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
 Provides-Extra: gui
 Requires-Dist: pyqtgraph>=0.13.0; extra == "gui"
-Requires-Dist: pyqt5; extra == "gui"
-Requires-Dist: pyqt5.sip; extra == "gui"
-Requires-Dist: google-cloud-storage; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: pyqt6; extra == "gui"
+Requires-Dist: pyqt6.sip; extra == "gui"
 Requires-Dist: matplotlib; extra == "gui"
 Provides-Extra: all
 Requires-Dist: pyqtgraph>=0.13.0; extra == "all"
-Requires-Dist: pyqt5; extra == "all"
-Requires-Dist: pyqt5.sip; extra == "all"
-Requires-Dist: google-cloud-storage; extra == "all"
+Requires-Dist: qtpy; extra == "all"
+Requires-Dist: pyqt6; extra == "all"
+Requires-Dist: pyqt6.sip; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 
 # Kilosort4
 
 [![Documentation Status](https://readthedocs.org/projects/kilosort/badge/?version=latest)](https://kilosort.readthedocs.io/en/latest/?badge=latest)
 ![tests](https://github.com/mouseland/kilosort/actions/workflows/test_and_deploy.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/kilosort.svg)](https://badge.fury.io/py/kilosort)
@@ -57,15 +60,19 @@
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
 **If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). 
+**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+
+**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04. 
 
@@ -101,18 +108,28 @@
 
 1. Open the GUI with `python -m kilosort`
 2. Select the path to the binary file and optionally the results directory. We recommend putting the binary file on an SSD for faster processing. 
 3. Select the probe configuration (mat files recommended, they actually exclude off channels unlike prb files)
 4. Hit `LOAD`. The data should now be visible.
 5. Hit `Run`. This will run the pipeline and output the results in a format compatible with Phy, the most popular spike sorting curating software.
 
-There is a warning that will always pop up when running Kilosort and/or using the BinaryFile class, but it's nothing to worry about:
+### Debugging qt.qpa.plugin error
+
+Some users have encountered the following error (or similar ones with slight variations) when attempting to launch the Kilosort4 GUI:
 ```
-UserWarning: The given NumPy array is not writable, and PyTorch does not support non-writable tensors. This means writing to this tensor will result in undefined behavior. You may want to copy the array to protect its data or make it writable before converting it to a tensor. This type of warning will be suppressed for the rest of this program. (Triggered internally at C:\cb\pytorch_1000000000000\work\torch\csrc\utils\tensor_numpy.cpp:205.)
+QObject::moveToThread: Current thread (0x2a7734988a0) is not the object's thread (0x2a77349d4e0).
+Cannot move to target thread (0x2a7734988a0)
+
+qt.qpa.plugin: Could not load the Qt platform plugin "windows" in "<FILEPATH>" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+
+Available platform plugins are: minimal, offscreen, webgl, windows.
 ```
+This is not specific to Kilosort4, it is a general problem with PyQt (the GUI library we chose to develop with) that doesn't appear to have a single cause or fix. If you encounter this error, please check [issue 597](https://github.com/MouseLand/Kilosort/issues/597) and [issue 613](https://github.com/MouseLand/Kilosort/issues/613) for some suggested solutions.
+
 
 ## Integration with Phy GUI
 
 [Phy](https://github.com/cortex-lab/phy) provides a manual clustering interface for refining the results of the algorithm. Kilosort4 automatically sets the "good" units in Phy based on a <10% estimated contamination rate with spikes from other neurons (computed from the refractory period violations relative to expected).
 
 Check out the [Phy](https://github.com/cortex-lab/phy) repo for more install instructions. We recommend installing Phy in its own environment to avoid package conflicts.
```

### Comparing `kilosort-4.0.2/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.3/kilosort.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 .github/ISSUE_TEMPLATE/installation_issue.yml
 .github/ISSUE_TEMPLATE/other.yml
 .github/workflows/test_and_deploy.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/drift.rst
-docs/first_run.rst
+docs/gui_guide.rst
 docs/hardware.rst
 docs/index.rst
-docs/installation.rst
 docs/make.bat
+docs/multi_shank.rst
+docs/parameters.rst
 docs/requirements.txt
 docs/tutorials/basic_example.ipynb
 docs/tutorials/load_data.ipynb
 docs/tutorials/make_probe.ipynb
 docs/tutorials/tutorials.rst
 kilosort/CCG.py
 kilosort/__init__.py
```

### Comparing `kilosort-4.0.2/tests/conftest.py` & `kilosort-4.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/tests/test_dtype.py` & `kilosort-4.0.3/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/tests/test_full_pipeline.py` & `kilosort-4.0.3/tests/test_full_pipeline.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/tests/test_io.py` & `kilosort-4.0.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/tests/test_preprocessing.py` & `kilosort-4.0.3/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.2/tox.ini` & `kilosort-4.0.3/tox.ini`

 * *Files identical despite different names*

