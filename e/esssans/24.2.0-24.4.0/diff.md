# Comparing `tmp/esssans-24.2.0.tar.gz` & `tmp/esssans-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esssans-24.2.0.tar", last modified: Wed Feb  7 09:04:16 2024, max compression
+gzip compressed data, was "esssans-24.4.0.tar", last modified: Fri Apr  5 12:59:02 2024, max compression
```

## Comparing `esssans-24.2.0.tar` & `esssans-24.4.0.tar`

### file list

```diff
@@ -1,129 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-07 09:04:02.000000 esssans-24.2.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.095375 esssans-24.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.095375 esssans-24.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-07 09:04:02.000000 esssans-24.2.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-07 09:04:02.000000 esssans-24.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-07 09:04:02.000000 esssans-24.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-02-07 09:04:02.000000 esssans-24.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-07 09:04:02.000000 esssans-24.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-07 09:04:02.000000 esssans-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 09:04:02.000000 esssans-24.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-07 09:04:16.111375 esssans-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-07 09:04:02.000000 esssans-24.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.095375 esssans-24.2.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-07 09:04:02.000000 esssans-24.2.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.095375 esssans-24.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.095375 esssans-24.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.099375 esssans-24.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/_templates/module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.099375 esssans-24.2.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.099375 esssans-24.2.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.099375 esssans-24.2.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/developer/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.099375 esssans-24.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/examples/loki-direct-beam.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/examples/sans2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/examples/zoom.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-07 09:04:02.000000 esssans-24.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-07 09:04:02.000000 esssans-24.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.103376 esssans-24.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-07 09:04:02.000000 esssans-24.2.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.103376 esssans-24.2.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-07 09:04:02.000000 esssans-24.2.0/resources/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-07 09:04:16.111375 esssans-24.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.091375 esssans-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.107375 esssans-24.2.0/src/esssans/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16992 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/beam_center_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/direct_beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/i_of_q.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.107375 esssans-24.2.0/src/esssans/isis/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/mantidio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/isis/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/src/esssans/loki/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/loki/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/loki/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/loki/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/loki/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/src/esssans/sans2d/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/sans2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/sans2d/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/sans2d/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/sans2d/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/sans2d/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-07 09:04:02.000000 esssans-24.2.0/src/esssans/uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/src/esssans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-07 09:04:16.000000 esssans-24.2.0/src/esssans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-07 09:04:16.000000 esssans-24.2.0/src/esssans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 09:04:16.000000 esssans-24.2.0/src/esssans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-07 09:04:16.000000 esssans-24.2.0/src/esssans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 09:04:16.000000 esssans-24.2.0/src/esssans.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/io_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/tests/loki/
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/loki/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/loki/directbeam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/loki/iofq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/package_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:04:16.111375 esssans-24.2.0/tests/sans2d/
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/sans2d/reduction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-07 09:04:02.000000 esssans-24.2.0/tests/uncertainty_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-07 09:04:02.000000 esssans-24.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.142093 esssans-24.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:58:52.000000 esssans-24.4.0/.copier-answers.ess.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 12:58:52.000000 esssans-24.4.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/ISSUE_TEMPLATE/high-level-requirement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 12:58:52.000000 esssans-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 12:58:52.000000 esssans-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-05 12:58:52.000000 esssans-24.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 12:58:52.000000 esssans-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 12:58:52.000000 esssans-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 12:58:52.000000 esssans-24.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 12:59:02.142093 esssans-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-05 12:58:52.000000 esssans-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-05 12:58:52.000000 esssans-24.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/common/beam-center-finder.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/common/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/sans2d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/zoom.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/loki/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20783 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/loki/loki-direct-beam.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-05 12:58:52.000000 esssans-24.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.130093 esssans-24.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.130093 esssans-24.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-05 12:58:52.000000 esssans-24.4.0/resources/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 12:59:02.142093 esssans-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.118093 esssans-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.118093 esssans-24.4.0/src/ess/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.134093 esssans-24.4.0/src/ess/isissans/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/mantidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/sans2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.134093 esssans-24.4.0/src/ess/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/src/ess/sans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/beam_center_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/direct_beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/i_of_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.142093 esssans-24.4.0/src/esssans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/i_of_q_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/io_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/isissans/
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/isissans/sans2d_reduction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/isissans/zoom_reduction_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/directbeam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13227 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/iofq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/uncertainty_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-05 12:58:52.000000 esssans-24.4.0/tox.ini
```

### Comparing `esssans-24.2.0/.github/workflows/ci.yml` & `esssans-24.4.0/.github/workflows/nightly_at_release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,40 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: CI
+name: Nightly tests at latest release
 
 on:
-  push:
-    branches:
-      - main
-      - release
-  pull_request:
+  workflow_dispatch:
+  schedule:
+    - cron: '0 1 * * 1-5'
 
 jobs:
-  formatting:
-    name: Formatting and static analysis
+  setup:
+    name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
-      min_tox_env: ${{ steps.vars.outputs.min_tox_env }}
+      release_tag: ${{ steps.release.outputs.release_tag }}
     steps:
       - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0  # history required so we can determine latest release tag
+      - name: Get last release tag from git
+        id: release
+        run: echo "release_tag=$(git describe --tags --abbrev=0 --match '[0-9]*.[0-9]*.[0-9]*')" >> $GITHUB_OUTPUT
       - name: Get Python version for other CI jobs
         id: vars
-        run: |
-          echo "min_python=$(cat .github/workflows/python-version-ci)" >> $GITHUB_OUTPUT
-          echo "min_tox_env=py$(cat .github/workflows/python-version-ci | sed 's/\.//g')" >> $GITHUB_OUTPUT
-      - uses: actions/setup-python@v4
-        with:
-          python-version-file: '.github/workflows/python-version-ci'
-      - run: python -m pip install --upgrade pip
-      - run: python -m pip install -r requirements/ci.txt
-      - run: tox -e static
-      - uses: stefanzweifel/git-auto-commit-action@v5
-        with:
-          commit_message: Apply automatic formatting
+        run: echo "min_python=$(cat .github/workflows/python-version-ci)" >> $GITHUB_OUTPUT
 
   tests:
     name: Tests
-    needs: formatting
+    needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
-          - version: '${{needs.formatting.outputs.min_python}}'
-            tox-env: '${{needs.formatting.outputs.min_tox_env}}'
+          - version: '${{needs.setup.outputs.min_python}}'
+            tox-env: 'nightly'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
-
-  docs:
-    needs: tests
-    uses: ./.github/workflows/docs.yml
-    with:
-      publish: false
-      linkcheck: ${{ contains(matrix.variant.os, 'ubuntu') && github.ref == 'refs/heads/main' }}
-      branch: ${{ github.head_ref == '' && github.ref_name || github.head_ref }}
+      checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `esssans-24.2.0/.github/workflows/docs.yml` & `esssans-24.4.0/.github/workflows/docs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Docs
 
 on:
   workflow_dispatch:
     inputs:
       publish:
         default: false
@@ -43,33 +40,34 @@
 
 jobs:
   docs:
     name: Build documentation
     runs-on: 'ubuntu-22.04'
     steps:
       - run: sudo apt install --yes graphviz pandoc
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
+          repository: ${{ github.event.pull_request.head.repo.full_name }}
           fetch-depth: 0  # history required so cmake can determine version
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e releasedocs -- ${VERSION}
         if: ${{ inputs.version != '' }}
       - run: tox -e docs
         if: ${{ inputs.version == '' }}
       - run: tox -e linkcheck
         if: ${{ inputs.linkcheck }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: docs_html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.4.3
+      - uses: JamesIves/github-pages-deploy-action@v4.5.0
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
```

### Comparing `esssans-24.2.0/.github/workflows/nightly_at_main.yml` & `esssans-24.4.0/.github/workflows/nightly_at_main.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Nightly test at main branch
 
 on:
   workflow_dispatch:
   schedule:
     - cron: '30 1 * * 1-5'
```

### Comparing `esssans-24.2.0/.github/workflows/nightly_at_release.yml` & `esssans-24.4.0/.github/workflows/unpinned.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: Nightly tests at latest release
+name: Unpinned tests at latest release
 
 on:
   workflow_dispatch:
   schedule:
-    - cron: '0 1 * * 1-5'
+    - cron: '0 2 * * 1'
 
 jobs:
   setup:
     name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
@@ -30,14 +27,14 @@
     name: Tests
     needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
           - version: '${{needs.setup.outputs.min_python}}'
-            tox-env: 'nightly'
+            tox-env: 'unpinned'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
       checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `esssans-24.2.0/.github/workflows/release.yml` & `esssans-24.4.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Release
 
 on:
   release:
     types: [published]
   workflow_dispatch:
 
@@ -14,77 +11,77 @@
 
 jobs:
   build_conda:
     name: Conda build
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: build-env
           create-args: >-
             conda-build
             boa
       - run: conda mambabuild --channel conda-forge --channel scipp --no-anaconda-upload --override-channels --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: conda-package-noarch
           path: conda/package/noarch/*.tar.bz2
 
   build_wheels:
     name: Wheels
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     environment: release
     permissions:
       id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.10
+      - uses: actions/download-artifact@v4
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
 
   upload_conda:
     name: Deploy Conda
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: upload-env
           # frozen python due to breaking removal of 'imp' in 3.12
           create-args: >-
             anaconda-client
             python=3.11
@@ -100,15 +97,15 @@
   assets:
     name: Upload docs
     needs: docs
     runs-on: 'ubuntu-22.04'
     permissions:
       contents: write  # This is needed so that the action can upload the asset
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
     - name: Zip documentation
       run: |
         mv docs_html documentation-${{ github.ref_name }}
         zip -r documentation-${{ github.ref_name }}.zip documentation-${{ github.ref_name }}
     - name: Upload release assets
       uses: svenstaro/upload-release-action@v2
       with:
```

### Comparing `esssans-24.2.0/.github/workflows/test.yml` & `esssans-24.4.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Test
 
 on:
   workflow_dispatch:
     inputs:
       os-variant:
         default: 'ubuntu-22.04'
@@ -44,21 +41,21 @@
         type: string
 
 jobs:
   test:
     runs-on: ${{ inputs.os-variant }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.checkout_ref }}
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ inputs.python-version }}
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r ${{ inputs.pip-recipe }}
       - run: tox -e ${{ inputs.tox-env }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         if: ${{ inputs.coverage-report }}
         with:
           name: CoverageReport
           path: coverage_html/
```

### Comparing `esssans-24.2.0/.pre-commit-config.yaml` & `esssans-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/CODE_OF_CONDUCT.md` & `esssans-24.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/CONTRIBUTING.md` & `esssans-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/LICENSE` & `esssans-24.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `esssans-24.2.0/PKG-INFO` & `esssans-24.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: esssans
-Version: 24.2.0
+Version: 24.4.0
 Summary: SANS data reduction for the European Spallation Source
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -38,28 +38,28 @@
 Project-URL: Source, https://github.com/scipp/esssans
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: graphviz
+Requires-Dist: essreduce
 Requires-Dist: plopp
 Requires-Dist: pythreejs
-Requires-Dist: sciline>=23.9.1
+Requires-Dist: sciline>=24.4.1
 Requires-Dist: scipp>=23.8.0
 Requires-Dist: scippneutron>=23.9.0
 Requires-Dist: scippnexus>=23.12.1
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/esssans.svg)](https://pypi.python.org/pypi/esssans)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/esssans/badges/version.svg)](https://anaconda.org/scipp/esssans)
```

### Comparing `esssans-24.2.0/README.md` & `esssans-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_static/anaconda-icon.js` & `esssans-24.4.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_static/favicon.ico` & `esssans-24.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_static/logo-dark.svg` & `esssans-24.4.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_static/logo.svg` & `esssans-24.4.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_templates/class-template.rst` & `esssans-24.4.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/_templates/module-template.rst` & `esssans-24.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/about/index.md` & `esssans-24.4.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/conf.py` & `esssans-24.4.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 # -*- coding: utf-8 -*-
 
 import doctest
 import os
 import sys
 
-import esssans
+from ess import sans
 
 sys.path.insert(0, os.path.abspath('.'))
 
 # General information about the project.
 project = u'ESSsans'
-copyright = u'2023 Scipp contributors'
+copyright = u'2024 Scipp contributors'
 author = u'Scipp contributors'
 
 html_show_sourcelink = True
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'sphinx.ext.mathjax',
     'sphinx.ext.napoleon',
+    'sphinx.ext.viewcode',
     'sphinx_autodoc_typehints',
     'sphinx_copybutton',
     'sphinx_design',
     'nbsphinx',
     'myst_parser',
 ]
 
+try:
+    import sciline.sphinxext.domain_types  # noqa: F401
+
+    extensions.append('sciline.sphinxext.domain_types')
+except ModuleNotFoundError:
+    pass
+
+
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "deflist",
     "dollarmath",
     "fieldlist",
     "html_admonition",
@@ -50,14 +59,15 @@
 autodoc_type_aliases = {
     'array_like': 'array_like',
 }
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
+    'scipp': ('https://scipp.github.io/', None),
 }
 
 # autodocs includes everything, even irrelevant API internals. autosummary
 # looks more suitable in the long run when the API grows.
 # For a nice example see how xarray handles its API documentation.
 autosummary_generate = True
 
@@ -69,14 +79,25 @@
 napoleon_type_aliases = {
     # objects without namespace: numpy
     "ndarray": "~numpy.ndarray",
 }
 typehints_defaults = 'comma'
 typehints_use_rtype = False
 
+sciline_domain_types_prefix = 'ess.sans'
+sciline_domain_types_aliases = {
+    'scipp._scipp.core.DataArray': 'scipp.DataArray',
+    'scipp._scipp.core.Dataset': 'scipp.Dataset',
+    'scipp._scipp.core.DType': 'scipp.DType',
+    'scipp._scipp.core.Unit': 'scipp.Unit',
+    'scipp._scipp.core.Variable': 'scipp.Variable',
+    'scipp.core.data_group.DataGroup': 'scipp.DataGroup',
+}
+
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 source_suffix = ['.rst', '.md']
@@ -87,17 +108,17 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
 # The short X.Y version.
-version = esssans.__version__
+version = sans.__version__
 # The full version, including alpha/beta/rc tags.
-release = esssans.__version__
+release = sans.__version__
 
 warning_is_error = True
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `esssans-24.2.0/docs/developer/coding-conventions.md` & `esssans-24.4.0/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/developer/dependency-management.md` & `esssans-24.4.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/docs/developer/getting-started.md` & `esssans-24.4.0/docs/developer/getting-started.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ## Running tests
 
 `````{tab-set}
 ````{tab-item} tox
 Run the tests using
 
 ```sh
-tox -e py39
+tox -e py310
 ```
 
 (or just `tox` if you want to run all environments).
 
 ````
 ````{tab-item} Manually
 Run the tests using
```

### Comparing `esssans-24.2.0/docs/examples/loki-direct-beam.ipynb` & `esssans-24.4.0/docs/user-guide/isis/sans2d.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9536722857592235%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Sans2d data reduction\\n'), (4, 'This notebook gives "*

 * *            'a concise overview of how to use the `esssans` package with Sciline, on the example '*

 * *            "of the data reduction of a Sans2d experiment.\\n'), (5, 'We begin with relevant "*

 * *            "imports:')], delete: [21, 20, 19, 18, 17, 16, 15, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, "*

 * *            "3, 0]}}, 1: {'source': {insert: [(3, 'from ess import sans\\n'), (4, 'from ess import "*

 * *            "isiss […]*

```diff
@@ -1,383 +1,479 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "9a935df3-c816-4829-99c3-2afa979b7611",
             "metadata": {},
             "source": [
-                "# Direct beam iterations for LoKI\n",
+                "# Sans2d data reduction\n",
                 "\n",
                 "## Introduction\n",
                 "\n",
-                "This notebook is used to compute the direct beam function for the LoKI detectors.\n",
-                "It uses data recorded during the detector test at the Larmor instrument.\n",
-                "\n",
-                "**Description of the procedure:**\n",
-                "\n",
-                "The idea behind the direct beam iterations is to determine an efficiency of the detectors as a function of wavelength.\n",
-                "To calculate this, it is possible to compute $I(Q)$ for the full wavelength range, and for individual slices (bands) of the wavelength range.\n",
-                "If the direct beam function used in the $I(Q)$ computation is correct, then $I(Q)$ curves for the full wavelength range and inside the bands should overlap.\n",
-                "\n",
-                "In the following notebook, we will:\n",
-                "\n",
-                "1. Create a pipeline to compute $I(Q)$ inside a set of wavelength bands (the number of wavelength bands will be the number of data points in the final direct beam function)\n",
-                "1. Create a flat direct beam function, as a function of wavelength, with wavelength bins corresponding to the wavelength bands\n",
-                "1. Calculate inside each band by how much one would have to multiply the final $I(Q)$ so that the curve would overlap with the full-range curve\n",
-                "   (we compute the full-range data by making a copy of the pipeline but setting only a single wavelength band that contains all wavelengths)\n",
-                "1. Multiply the direct beam values inside each wavelength band by this factor\n",
-                "1. Compare the full-range $I(Q)$ to a theoretical reference and add the corresponding additional scaling to the direct beam function\n",
-                "1. Iterate until the changes to the direct beam function become small"
+                "This notebook gives a concise overview of how to use the `esssans` package with Sciline, on the example of the data reduction of a Sans2d experiment.\n",
+                "We begin with relevant imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8c7f7cf7-0582-4953-a772-a0f87d1cf0e2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "import numpy as np\n",
                 "import scipp as sc\n",
                 "import sciline\n",
-                "import scippneutron as scn\n",
                 "import plopp as pp\n",
-                "import esssans as sans\n",
-                "from esssans.types import *\n",
-                "from esssans.direct_beam import direct_beam"
+                "from ess import sans\n",
+                "from ess import isissans as isis\n",
+                "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c21564a8-e742-4183-9edc-2c70c51d5863",
+            "id": "3da2d397-6206-4ed1-a98f-11b3aaf7e5b0",
             "metadata": {},
             "source": [
                 "## Define reduction parameters\n",
                 "\n",
-                "We define a dictionary containing the reduction parameters, with keys and types given by aliases or types defined in `esssans.types`:"
+                "We define the reduction parameters, with keys and types given by aliases or types defined in `ess.sans.types`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ce2841f0-bd9e-43c3-8cc5-52bb45f392ad",
+            "id": "d3f5e1ee-bd80-4301-9ff9-15c8ada3cf57",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = sans.loki.default_parameters.copy()\n",
+                "params = {}\n",
                 "\n",
-                "# List of files\n",
-                "params[FileList[SampleRun]] = ['60339-2022-02-28_2215.nxs']\n",
-                "params[FileList[BackgroundRun]] = ['60393-2022-02-28_2215.nxs']\n",
-                "params[FileList[TransmissionRun[SampleRun]]] = ['60394-2022-02-28_2215.nxs']\n",
-                "params[FileList[TransmissionRun[BackgroundRun]]] = ['60392-2022-02-28_2215.nxs']\n",
-                "params[FileList[EmptyBeamRun]] = ['60392-2022-02-28_2215.nxs']\n",
+                "params[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat'\n",
+                "params[Filename[SampleRun]] = 'SANS2D00063114.nxs'\n",
+                "params[Filename[BackgroundRun]] = 'SANS2D00063159.nxs'\n",
+                "params[Filename[EmptyBeamRun]] = 'SANS2D00063091.nxs'\n",
+                "params[OutFilename] = 'reduced.nxs'\n",
                 "\n",
-                "# Wavelength binning parameters\n",
-                "wavelength_min = sc.scalar(1.0, unit='angstrom')\n",
-                "wavelength_max = sc.scalar(13.0, unit='angstrom')\n",
-                "n_wavelength_bins = 200\n",
-                "n_wavelength_bands = 50\n",
+                "params[NeXusMonitorName[Incident]] = 'monitor2'\n",
+                "params[NeXusMonitorName[Transmission]] = 'monitor4'\n",
+                "\n",
+                "params[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')\n",
+                "params[isis.MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')\n",
                 "\n",
                 "params[WavelengthBins] = sc.linspace(\n",
-                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bins + 1\n",
-                ")\n",
-                "params[WavelengthBands] = sc.linspace(\n",
-                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bands + 1\n",
+                "    'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'\n",
                 ")\n",
                 "\n",
-                "params[BeamStopPosition] = sc.vector([-0.026, -0.022, 0.0], unit='m')\n",
-                "params[BeamStopRadius] = sc.scalar(0.042, unit='m')\n",
+                "params[isis.sans2d.LowCountThreshold] = sc.scalar(100, unit='counts')\n",
                 "\n",
+                "mask_interval = sc.array(dims=['wavelength'], values=[2.21, 2.59], unit='angstrom')\n",
+                "params[WavelengthMask] = sc.DataArray(\n",
+                "    sc.array(dims=['wavelength'], values=[True]),\n",
+                "    coords={'wavelength': mask_interval},\n",
+                ")\n",
+                "\n",
+                "params[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.6, num=141, unit='1/angstrom')\n",
+                "params[NonBackgroundWavelengthRange] = sc.array(\n",
+                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
+                ")\n",
                 "params[CorrectForGravity] = True\n",
                 "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[sans.ReturnEvents] = False\n",
-                "\n",
-                "params[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.3, num=101, unit='1/angstrom')"
+                "params[ReturnEvents] = True"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f2c3b542",
+            "id": "c21564a8-e742-4183-9edc-2c70c51d5863",
             "metadata": {},
             "source": [
                 "## Create pipeline using Sciline\n",
                 "\n",
-                "We use all providers available in `esssans` as well as the `loki`-specific providers,\n",
-                "which include I/O and mask setup specific to the [LoKI](https://europeanspallationsource.se/instruments/loki) instrument.\n",
-                "\n",
-                "We then build the pipeline which can be used to compute the (background subtracted) $I(Q)$."
+                "We use all providers available in `ess.sans` as well as the `isis` and `sans2d`-specific providers, which include I/O and mask setup specific to the [Sans2d](https://www.isis.stfc.ac.uk/Pages/sans2d.aspx) instrument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c1e0e90-da33-45e7-a464-4799f4fbc657",
+            "id": "85b955ba-a54d-4760-bb35-af9cbe1ada90",
             "metadata": {},
             "outputs": [],
             "source": [
-                "providers = sans.providers + sans.loki.providers\n",
+                "providers = (\n",
+                "    sans.providers + isis.providers + isis.data.providers + isis.sans2d.providers\n",
+                ")\n",
+                "providers = providers + (\n",
+                "    isis.data.transmission_from_background_run,\n",
+                "    isis.data.transmission_from_sample_run,\n",
+                "    sans.beam_center_from_center_of_mass,\n",
+                ")\n",
                 "\n",
-                "pipeline = sciline.Pipeline(providers, params=params)"
+                "pipeline = sciline.Pipeline(providers=providers, params=params)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "805c22ea-216f-4ae4-bcbb-9eb31656cfef",
+            "id": "39f70669-0771-4a59-8e10-95c9120d0e9e",
             "metadata": {},
             "source": [
+                "## Visualize the pipeline\n",
+                "\n",
                 "Before we begin computations, we can visualize the pipeline:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6eca12c4-e28c-4e45-8d3d-c5869746086b",
+            "id": "d71780b8-56d5-445f-9d43-635d3d5f406b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
+                "# left-right layout works better for this graph\n",
+                "pipeline.visualize(BackgroundSubtractedIofQ, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3756cd2e-d402-4ed0-8dcb-682eef769c00",
+            "id": "c19eeaf0",
             "metadata": {},
             "source": [
-                "## Expected intensity at zero Q\n",
+                "## Use the pipeline\n",
                 "\n",
-                "The sample used in the experiment has a known $I(Q)$ profile,\n",
-                "and we need it to calibrate the absolute intensity of our $I(Q)$ results\n",
-                "(relative differences between wavelength band and full-range results are not sufficient).\n",
+                "### Compute final result\n",
                 "\n",
-                "We load this theoretical reference curve, and compute the $I_{0}$ intensity at the lower $Q$ bound of the range covered by the instrument."
+                "We can now compute the background-subtracted $I(Q)$:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e8951c82-e726-49b3-b102-66bfb9cc53e1",
+            "id": "c8cf57ce",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from scipp.scipy.interpolate import interp1d\n",
-                "from esssans.loki.data import get_path\n",
-                "\n",
-                "Iq_theory = sc.io.load_hdf5(get_path('PolyGauss_I0-50_Rg-60.h5'))\n",
-                "f = interp1d(Iq_theory, 'Q')\n",
-                "I0 = f(sc.midpoints(params[QBins])).data[0]\n",
-                "I0"
+                "result = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "result.hist().plot(scale={'Q': 'log'}, norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "078fb21e-c4d5-49e7-bcca-7bacf93fbd19",
+            "id": "28532aa7",
             "metadata": {},
             "source": [
-                "## A single direct beam function for all layers\n",
-                "\n",
-                "As a first pass, we compute a single direct beam function for all the detector pixels combined.\n",
-                "\n",
-                "We compute the $I(Q)$ inside the wavelength bands and the full wavelength range,\n",
-                "derive a direct beam factor per wavelength band,\n",
-                "and also add absolute scaling using the reference $I_{0}$ value"
+                "As the result was computed in event-mode, we can also use a different $Q$-binning, without re-reducing the data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6ffa0b31-a43c-4f73-a568-5fa1ab2d61bf",
+            "id": "e0748a1a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "results = direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
-                "# Unpack the final result\n",
-                "iofq_full = results[-1]['iofq_full']\n",
-                "iofq_bands = results[-1]['iofq_bands']\n",
-                "direct_beam_function = results[-1]['direct_beam']"
+                "result.hist(Q=60).plot(scale={'Q': 'log'}, norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bc290019-85ea-406c-912d-75f1229f2ddf",
+            "id": "2359dd3d",
             "metadata": {},
             "source": [
-                "We now compare the $I(Q)$ curves in each wavelength band to the one for the full wavelength range (black)."
+                "In the above we used an upper bound for the uncertainties of the normalization factors.\n",
+                "We can also compute the result with dropped normalization-factor uncertainties.\n",
+                "This is incorrect, but is useful for understanding whether the normalization factors significantly contribute to the uncertainty of the result:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0055bce0-18f2-425d-937b-fb8e211247b1",
+            "id": "6a8e0b6b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot(\n",
-                "    {**sc.collapse(iofq_bands, keep='Q'), **{'full': iofq_full}},\n",
-                "    norm='log',\n",
-                "    color={'full': 'k'},\n",
-                "    legend=False,\n",
-                ")"
+                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.drop\n",
+                "result_drop = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "# Reset the UnsertaintyBroadcastMode to the old value\n",
+                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "sc.DataGroup(upper_bound=result, dropped=result_drop).hist().plot(norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d0a96015-061c-47ce-8384-2f34c8088332",
+            "id": "53ce1e48-b8a9-475a-b0ec-9ad204541543",
             "metadata": {},
             "source": [
-                "The overlap is satisfactory, and we can now inspect the direct beam function we have computed:"
+                "### Save reduced data to file\n",
+                "\n",
+                "`ess.sans` provides a function for saving the reduced data as an [NXcanSAS](https://manual.nexusformat.org/classes/applications/NXcanSAS.html) file.\n",
+                "It could be used directly with the `result` computed above, but we would have to provide the required metadata ourselves.\n",
+                "Instead, we use Sciline to get all required information directly from the pipeline: (See also the [File output](https://scipp.github.io/sciline/recipes/recipes.html#File-output) docs.)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d4b514c3-af6e-441f-82a5-28bfc0110248",
+            "id": "b83c7580-fba7-43d8-b9d0-1aeeebbe0301",
             "metadata": {},
             "outputs": [],
             "source": [
-                "direct_beam_function.plot(vmax=1)"
+                "from ess.sans.io import save_background_subtracted_iofq\n",
+                "\n",
+                "pipeline.bind_and_call(save_background_subtracted_iofq)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8b796452-7aaa-42fa-8cde-0c80a66ad1e2",
+            "id": "f39206c6",
             "metadata": {},
             "source": [
-                "Finally, as a sanity check, we compare our final $I(Q)$ for the full wavelength range to the theoretical reference:"
+                "### Compute intermediate results\n",
+                "\n",
+                "For inspection and debugging purposes we can also compute intermediate results.\n",
+                "To avoid repeated computation (including costly loading of files) we can request multiple results at once, including the final result, if desired.\n",
+                "For example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e491bd2d-5134-4837-b792-683f9ffd9e1d",
+            "id": "bb922379",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot({'reference': Iq_theory, 'data': iofq_full}, norm='log')"
+                "monitors = (\n",
+                "    WavelengthMonitor[SampleRun, Incident],\n",
+                "    WavelengthMonitor[SampleRun, Transmission],\n",
+                "    WavelengthMonitor[BackgroundRun, Incident],\n",
+                "    WavelengthMonitor[BackgroundRun, Transmission],\n",
+                ")\n",
+                "parts = (CleanSummedQ[SampleRun, Numerator], CleanSummedQ[SampleRun, Denominator])\n",
+                "iofqs = (IofQ[SampleRun], IofQ[BackgroundRun], BackgroundSubtractedIofQ)\n",
+                "keys = monitors + (MaskedData[SampleRun],) + parts + iofqs\n",
+                "\n",
+                "results = pipeline.compute(keys)\n",
+                "\n",
+                "display(sc.plot({str(key): results[key] for key in monitors}, norm='log'))\n",
+                "\n",
+                "display(\n",
+                "    isis.plot_flat_detector_xy(\n",
+                "        results[MaskedData[SampleRun]]['spectrum', :61440].hist(), norm='log'\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "wavelength = pipeline.compute(WavelengthBins)\n",
+                "display(\n",
+                "    results[CleanSummedQ[SampleRun, Numerator]]\n",
+                "    .hist(wavelength=wavelength)\n",
+                "    .transpose()\n",
+                "    .plot(norm='log')\n",
+                ")\n",
+                "display(results[CleanSummedQ[SampleRun, Denominator]].plot(norm='log'))\n",
+                "parts = {str(key): results[key].sum('wavelength') for key in parts}\n",
+                "display(sc.plot(parts, norm='log'))\n",
+                "\n",
+                "iofqs = {str(key): results[key] for key in iofqs}\n",
+                "iofqs = {key: val if val.bins is None else val.hist() for key, val in iofqs.items()}\n",
+                "display(sc.plot(iofqs, norm='log'))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0c616af7-b66c-4ae6-888e-1884d3ac9db1",
+            "id": "372b8d4f",
+            "metadata": {},
+            "source": [
+                "### Avoiding duplicate computation with parameter tables\n",
+                "\n",
+                "We have seen above that Sciline can avoid duplicate computation by requesting multiple results.\n",
+                "However, this is not always possible, for example if we want to compute the final result with different parameters.\n",
+                "In this case we can use parameter tables to avoid duplicate computation.\n",
+                "For example, we can compute the final result with different values for handling the uncertainties of the normalization factors.\n",
+                "This will avoid repeating loading files as well as some computation steps:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ceb079ee",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Direct beam function per layer\n",
+                "from typing import NewType\n",
                 "\n",
-                "The LoKI detector tubes are arranged in layers along the beam path,\n",
-                "where the layers closest to the sample will receive most of the scattered neutrons,\n",
-                "while occulting the layers behind them.\n",
+                "Mode = NewType('Mode', str)\n",
+                "param_table = sciline.ParamTable(\n",
+                "    Mode,\n",
+                "    {\n",
+                "        UncertaintyBroadcastMode: [\n",
+                "            UncertaintyBroadcastMode.upper_bound,\n",
+                "            UncertaintyBroadcastMode.drop,\n",
+                "        ]\n",
+                "    },\n",
+                "    index=[Mode('upper_bound'), Mode('drop')],\n",
+                ")\n",
+                "pipeline.set_param_table(param_table)\n",
+                "results = pipeline.compute(sciline.Series[Mode, BackgroundSubtractedIofQ])\n",
+                "sc.DataGroup(results).hist().plot(norm='log')"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "94062d33-04cb-4a4d-aef1-e5ec58c228c4",
+            "metadata": {},
+            "source": [
+                "## Wavelength bands\n",
                 "\n",
-                "A refinement to the above procedure is to compute a direct beam function for each layer of tubes individually.\n",
-                "We also use the 4 thick layers of tubes, but in principle,\n",
-                "this could also be done for 28 different layers (made from the `layer` and `straw` dimensions) if a run with enough events is provided (or many runs are combined together).\n",
+                "We can also compute $I(Q)$ inside a set of wavelength bands, instead of using the full wavelength range in one go.\n",
+                "This is useful for debugging purposes.\n",
                 "\n",
-                "The only other difference compared to the computation above is that we now want our final result to preserve the `'layer'` dimension,\n",
-                "so that the dimensions of our result are `['layer', 'Q']`."
+                "To achieve this, we need to supply the `WavelengthBands` parameter (as a two-dimensional variable),\n",
+                "representing the wavelength range for each band."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "64682705-3322-4003-8a56-f52f2523c8d4",
+            "id": "27068e8a-350f-4ea4-b4a4-2b13926905b5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[DimsToKeep] = ['layer']"
+                "pipeline[WavelengthBands] = sc.linspace(\n",
+                "    'wavelength', start=2.0, stop=16.0, num=11, unit='angstrom'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "92691c97-4883-41b4-b880-17e0359191a2",
+            "id": "cc3cac02-2cb4-4da5-a83d-8e6fb3d2c929",
             "metadata": {},
             "source": [
-                "Now we are able to run the direct-beam iterations on a per-layer basis:"
+                "Compute the result:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7e039618-d8c9-4201-9a9f-59738034786b",
+            "id": "6bd670f9-85db-4257-ab67-e296a7e8ecdf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "results = direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
-                "# Unpack the final result\n",
-                "iofq_full = results[-1]['iofq_full']\n",
-                "iofq_bands = results[-1]['iofq_bands']\n",
-                "direct_beam_function = results[-1]['direct_beam']"
+                "result = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "result"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "642c52a3-d174-4b75-b1ee-877231c316dd",
+            "id": "601d2a4f-1295-4918-8177-d2dca0b839f9",
             "metadata": {},
             "source": [
-                "We can now inspect the wavelength slices for the 4 layers."
+                "The result is two-dimensional and we over-plot all the bands onto the same axes:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "591cb3c7-63c4-427f-97c9-f2ad332d6c37",
+            "id": "d5df969d-79d1-443a-a71b-88faf8b57a37",
             "metadata": {},
             "outputs": [],
             "source": [
-                "plots = [\n",
-                "    pp.plot(\n",
-                "        {\n",
-                "            **sc.collapse(iofq_bands['layer', i], keep='Q'),\n",
-                "            **{'full': iofq_full['layer', i]},\n",
-                "        },\n",
-                "        norm='log',\n",
-                "        color={'full': 'k'},\n",
-                "        legend=False,\n",
-                "        title=f'Layer {i}',\n",
-                "    )\n",
-                "    for i in range(4)\n",
-                "]\n",
+                "pp.plot(sc.collapse(result.hist(), keep='Q'), norm='log')"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0977a3dc-eb5f-4067-80c5-cc19137cc915",
+            "metadata": {},
+            "source": [
+                "## Loading local files\n",
+                "\n",
+                "The data files used above are hosted on an external server, and downloaded on-the-fly (and cached) when computing the result.\n",
+                "\n",
+                "It is also possible to load local files from your hard drive, by using the `DataFolder` parameter.\n",
+                "We also need to insert the `isis.io.to_path` provider which supplies the file paths to the files in the folder.\n",
+                "\n",
+                "As an example, we will save our current direct beam to disk, and then re-load it using a pipeline that reads local files.\n",
                 "\n",
-                "(plots[0] + plots[1]) / (plots[2] + plots[3])"
+                "**Note** that is it not currently possible to mix local and cloud files in the same pipeline with the present setup."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "871743bf-32d0-4df1-a285-ba722a4198ef",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Direct beam computation currently uses the `get_path` provider which\n",
+                "# fetches files from the remote server\n",
+                "direct_beam = pipeline.get(DirectBeam)\n",
+                "direct_beam.visualize()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f35f4d14-58f2-437f-826c-b9ac74570e52",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Save the direct beam to disk\n",
+                "db_filename = 'my_local_direct_beam_file.h5'\n",
+                "direct_beam.compute().save_hdf5(db_filename)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9e1313fd-8f01-4a47-abf3-d641232b3d47",
+            "id": "8f712a5d-cab9-4878-9b74-5a6c9751e403",
             "metadata": {},
             "source": [
-                "Now the direct beam function inside each layer looks like:"
+                "We now modify our pipeline by setting the `DataFolder` parameter,\n",
+                "as well as our new direct beam filename. Finally, we insert the local file provider `to_path`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2fde077a-4d16-44b1-af0e-58216a8db57e",
+            "id": "27432974-0f06-4549-8ea5-4f75ff42fbc5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot(sc.collapse(direct_beam_function, keep='wavelength'))"
+                "pipeline[DataFolder] = '.'\n",
+                "pipeline[DirectBeamFilename] = db_filename\n",
+                "\n",
+                "# Insert provider for local files\n",
+                "pipeline.insert(isis.io.to_path)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2a49bcac-0283-4802-97f4-a5a8453383cf",
+            "id": "37be7d9a-92ec-468c-a36e-1c73682b1bda",
+            "metadata": {},
+            "source": [
+                "We can now see that `to_path` uses both the file name and the local folder to create a file path:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a5647adf-5606-4efa-9e18-2c2943d8250d",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "And finally, for completeness, we compare the $I(Q)$ to the theoretical reference inside each layer."
+                "db_local = pipeline.get(DirectBeam)\n",
+                "db_local.visualize()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a6411f70-f7e2-4061-8641-cc612a19a080",
+            "id": "446ef2a3-bf7d-404b-b493-0c65f71c1a03",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot({**{'reference': Iq_theory}, **sc.collapse(iofq_full, keep='Q')}, norm='log')"
+                "db_local.compute().plot()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -388,14 +484,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.2.0/docs/examples/sans2d.ipynb` & `esssans-24.4.0/docs/user-guide/loki/loki-direct-beam.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9332434380662016%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Direct beam iterations for LoKI\\n'), (4, 'This "*

 * *            "notebook is used to compute the direct beam function for the LoKI detectors.\\n'), "*

 * *            "(5, 'It uses data recorded during the detector test at the Larmor instrument.\\n'), "*

 * *            "(6, '\\n'), (7, '**Description of the procedure:**\\n'), (8, '\\n'), (9, 'The idea "*

 * *            'behind the direct beam iterations is to determine an efficiency of the detectors as a '*

 * *            "function […]*

```diff
@@ -1,20 +1,36 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "9a935df3-c816-4829-99c3-2afa979b7611",
             "metadata": {},
             "source": [
-                "# Sans2d data reduction\n",
+                "# Direct beam iterations for LoKI\n",
                 "\n",
                 "## Introduction\n",
                 "\n",
-                "This notebook gives a concise overview of how to use the `esssans` package with Sciline, on the example of the data reduction of a Sans2d experiment.\n",
-                "We begin with relevant imports:"
+                "This notebook is used to compute the direct beam function for the LoKI detectors.\n",
+                "It uses data recorded during the detector test at the Larmor instrument.\n",
+                "\n",
+                "**Description of the procedure:**\n",
+                "\n",
+                "The idea behind the direct beam iterations is to determine an efficiency of the detectors as a function of wavelength.\n",
+                "To calculate this, it is possible to compute $I(Q)$ for the full wavelength range, and for individual slices (bands) of the wavelength range.\n",
+                "If the direct beam function used in the $I(Q)$ computation is correct, then $I(Q)$ curves for the full wavelength range and inside the bands should overlap.\n",
+                "\n",
+                "In the following notebook, we will:\n",
+                "\n",
+                "1. Create a pipeline to compute $I(Q)$ inside a set of wavelength bands (the number of wavelength bands will be the number of data points in the final direct beam function)\n",
+                "1. Create a flat direct beam function, as a function of wavelength, with wavelength bins corresponding to the wavelength bands\n",
+                "1. Calculate inside each band by how much one would have to multiply the final $I(Q)$ so that the curve would overlap with the full-range curve\n",
+                "   (we compute the full-range data by making a copy of the pipeline but setting only a single wavelength band that contains all wavelengths)\n",
+                "1. Multiply the direct beam values inside each wavelength band by this factor\n",
+                "1. Compare the full-range $I(Q)$ to a theoretical reference and add the corresponding additional scaling to the direct beam function\n",
+                "1. Iterate until the changes to the direct beam function become small"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8c7f7cf7-0582-4953-a772-a0f87d1cf0e2",
             "metadata": {
@@ -23,368 +39,581 @@
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "import sciline\n",
                 "import scippneutron as scn\n",
                 "import plopp as pp\n",
-                "import esssans as sans\n",
-                "from esssans.types import *"
+                "from ess import sans\n",
+                "from ess import loki\n",
+                "from ess import isissans as isis\n",
+                "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c21564a8-e742-4183-9edc-2c70c51d5863",
             "metadata": {},
             "source": [
-                "## Create pipeline using Sciline\n",
+                "## Define reduction parameters\n",
                 "\n",
-                "We use all providers available in `esssans` as well as the `sans2d`-specific providers, which include I/O and mask setup specific to the [Sans2d](https://www.isis.stfc.ac.uk/Pages/sans2d.aspx) instrument:"
+                "We define a dictionary containing the reduction parameters, with keys and types given by aliases or types defined in `ess.sans.types`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "025fca0b-68a7-4d6e-a82a-86713cc3fca7",
+            "id": "ce2841f0-bd9e-43c3-8cc5-52bb45f392ad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline = sciline.Pipeline(\n",
-                "    sans.providers + sans.sans2d.providers,\n",
-                "    params=sans.sans2d.default_parameters,\n",
-                ")"
+                "params = loki.default_parameters.copy()\n",
+                "\n",
+                "# File names\n",
+                "params[Filename[SampleRun]] = '60339-2022-02-28_2215.nxs'\n",
+                "params[Filename[BackgroundRun]] = '60393-2022-02-28_2215.nxs'\n",
+                "params[Filename[TransmissionRun[SampleRun]]] = '60394-2022-02-28_2215.nxs'\n",
+                "params[Filename[TransmissionRun[BackgroundRun]]] = '60392-2022-02-28_2215.nxs'\n",
+                "params[Filename[EmptyBeamRun]] = '60392-2022-02-28_2215.nxs'\n",
+                "\n",
+                "# Wavelength binning parameters\n",
+                "wavelength_min = sc.scalar(1.0, unit='angstrom')\n",
+                "wavelength_max = sc.scalar(13.0, unit='angstrom')\n",
+                "n_wavelength_bins = 50\n",
+                "n_wavelength_bands = 50\n",
+                "\n",
+                "params[WavelengthBins] = sc.linspace(\n",
+                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bins + 1\n",
+                ")\n",
+                "params[WavelengthBands] = sc.linspace(\n",
+                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bands + 1\n",
+                ")\n",
+                "\n",
+                "masks = ['mask_new_July2022.xml']\n",
+                "banks = ['larmor_detector']\n",
+                "\n",
+                "params[CorrectForGravity] = True\n",
+                "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "params[ReturnEvents] = False\n",
+                "\n",
+                "params[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.3, num=101, unit='1/angstrom')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3da2d397-6206-4ed1-a98f-11b3aaf7e5b0",
+            "id": "f2c3b542",
             "metadata": {},
             "source": [
-                "# Define reduction parameters\n",
+                "## Create pipeline using Sciline\n",
+                "\n",
+                "We use all providers available in `esssans` as well as the `loki`-specific providers,\n",
+                "which include I/O and mask setup specific to the [LoKI](https://europeanspallationsource.se/instruments/loki) instrument.\n",
                 "\n",
-                "We define the reduction parameters, with keys and types given by aliases or types defined in `esssans.types`:"
+                "We then build the pipeline which can be used to compute the (background subtracted) $I(Q)$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bc2fffe1-a694-43b7-9234-e31da42d6df3",
-            "metadata": {
-                "tags": []
-            },
+            "id": "0c1e0e90-da33-45e7-a464-4799f4fbc657",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[FileList[BackgroundRun]] = ['SANS2D00063159.hdf5']\n",
-                "pipeline.insert(sans.transmission_from_background_run)\n",
-                "pipeline[FileList[SampleRun]] = ['SANS2D00063114.hdf5']\n",
-                "pipeline.insert(sans.transmission_from_sample_run)\n",
-                "pipeline[FileList[EmptyBeamRun]] = ['SANS2D00063091.hdf5']\n",
-                "pipeline[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.hdf5'\n",
-                "pipeline[OutFilename] = 'reduced.nxs'\n",
+                "providers = sans.providers + loki.providers + (isis.io.read_xml_detector_masking,)\n",
                 "\n",
-                "pipeline[WavelengthBins] = sc.linspace(\n",
-                "    'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'\n",
-                ")\n",
+                "pipeline = sciline.Pipeline(providers, params=params)\n",
+                "pipeline.insert(sans.merge_banks)\n",
+                "pipeline.set_param_series(PixelMaskFilename, masks)\n",
+                "pipeline.set_param_series(NeXusDetectorName, banks)\n",
                 "\n",
-                "pipeline[sans.sans2d.LowCountThreshold] = sc.scalar(100, unit='counts')\n",
-                "\n",
-                "mask_interval = sc.array(dims=['wavelength'], values=[2.21, 2.59], unit='angstrom')\n",
-                "pipeline[WavelengthMask] = sc.DataArray(\n",
-                "    sc.array(dims=['wavelength'], values=[True]),\n",
-                "    coords={'wavelength': mask_interval},\n",
-                ")\n",
+                "# Add providers that fetch data from online resource\n",
+                "for provider in loki.data.providers:\n",
+                "    pipeline.insert(provider)\n",
                 "\n",
-                "pipeline[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.6, num=141, unit='1/angstrom')\n",
-                "pipeline[NonBackgroundWavelengthRange] = sc.array(\n",
-                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
-                ")\n",
-                "pipeline[CorrectForGravity] = True\n",
-                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "pipeline[sans.ReturnEvents] = True"
+                "# In the present file, there is no sample information so we use a dummy sample provider\n",
+                "pipeline.insert(loki.io.dummy_load_sample)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c19eeaf0",
+            "id": "805c22ea-216f-4ae4-bcbb-9eb31656cfef",
             "metadata": {},
             "source": [
-                "## Use the pipeline\n",
+                "Before we begin computations, we can visualize the pipeline:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6eca12c4-e28c-4e45-8d3d-c5869746086b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pipeline.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "632e3c82-89d6-4899-b1c2-f9a318899c33",
+            "metadata": {},
+            "source": [
+                "## Finding the beam center\n",
+                "\n",
+                "Looking carefully at the pipeline above,\n",
+                "one will notice that there is a missing parameter from the pipeline: the red box that contains the `BeamCenter` type.\n",
+                "Before we can proceed with computing the direct beam function,\n",
+                "we therefore have to first determine the center of the beam.\n",
                 "\n",
-                "### Compute final result\n",
+                "There are more details on how this is done in the [beam center finder notebook](../common/beam-center-finder.ipynb),\n",
+                "but for now we simply reuse the pipeline (by making a copy),\n",
+                "and inserting the provider that will compute the beam center.\n",
                 "\n",
-                "We can get the graph for computing the background-subtracted $I(Q)$:"
+                "For now, we compute the beam center only for the rear detector (named 'larmor_detector') but apply it to all banks (currently there is only one bank).\n",
+                "The beam center may need to be computed or applied differently to each bank, see [scipp/esssans#28](https://github.com/scipp/esssans/issues/28)."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bdc15ab4-6ec6-4a29-81dc-1d00a8e890dc",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "bc_pipeline = pipeline.copy()\n",
+                "bc_pipeline.del_param_table(NeXusDetectorName)\n",
+                "bc_pipeline[NeXusDetectorName] = 'larmor_detector'\n",
+                "bc_pipeline.insert(sans.beam_center_from_center_of_mass)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a48c0f4d",
+            "id": "7cc2cf3b-973e-4425-93ea-deb30b12c956",
             "metadata": {},
             "outputs": [],
             "source": [
-                "iofq = pipeline.get(BackgroundSubtractedIofQ)"
+                "bc_pipeline.visualize(BeamCenter, compact=True, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "07c5c2cb",
+            "id": "b6bf5342-6768-4b65-882b-aefc9b583724",
             "metadata": {},
             "source": [
-                "Before we compute the result, we can visualize the pipeline:"
+                "We can now compute the value for the center"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bc186654",
+            "id": "6a17ac7c-de17-49c9-a02c-ca078eb7f023",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# left-right layout works better for this graph\n",
-                "iofq.visualize(graph_attr={'rankdir': 'LR'})"
+                "center = bc_pipeline.compute(BeamCenter)\n",
+                "center"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "505f26fc",
+            "id": "0814805a-9611-4951-a015-c12ae254b099",
             "metadata": {},
             "source": [
-                "Now we can compute the result:"
+                "and set that value onto our original pipeline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c8cf57ce",
+            "id": "e79181de-1de8-43a0-a934-e9407ebcd740",
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = iofq.compute()\n",
-                "result.hist().plot(scale={'Q': 'log'}, norm='log')"
+                "pipeline[BeamCenter] = center"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "28532aa7",
+            "id": "3756cd2e-d402-4ed0-8dcb-682eef769c00",
             "metadata": {},
             "source": [
-                "As the result was computed in event-mode, we can also use a different $Q$-binning, without re-reducing the data:"
+                "## Expected intensity at zero Q\n",
+                "\n",
+                "The sample used in the experiment has a known $I(Q)$ profile,\n",
+                "and we need it to calibrate the absolute intensity of our $I(Q)$ results\n",
+                "(relative differences between wavelength band and full-range results are not sufficient).\n",
+                "\n",
+                "We load this theoretical reference curve, and compute the $I_{0}$ intensity at the lower $Q$ bound of the range covered by the instrument."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e0748a1a",
+            "id": "e8951c82-e726-49b3-b102-66bfb9cc53e1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "result.hist(Q=60).plot(scale={'Q': 'log'}, norm='log')"
+                "from scipp.scipy.interpolate import interp1d\n",
+                "from ess.loki.data import get_path\n",
+                "\n",
+                "Iq_theory = sc.io.load_hdf5(get_path('PolyGauss_I0-50_Rg-60.h5'))\n",
+                "f = interp1d(Iq_theory, 'Q')\n",
+                "I0 = f(sc.midpoints(params[QBins])).data[0]\n",
+                "I0"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2359dd3d",
+            "id": "078fb21e-c4d5-49e7-bcca-7bacf93fbd19",
             "metadata": {},
             "source": [
-                "In the above we used an upper bound for the uncertainties of the normalization factors.\n",
-                "We can also compute the result with dropped normalization-factor uncertainties.\n",
-                "This is incorrect, but is useful for understanding whether the normalization factors significantly contribute to the uncertainty of the result:"
+                "## A single direct beam function for all layers\n",
+                "\n",
+                "As a first pass, we compute a single direct beam function for all the detector pixels combined.\n",
+                "\n",
+                "We compute the $I(Q)$ inside the wavelength bands and the full wavelength range,\n",
+                "derive a direct beam factor per wavelength band,\n",
+                "and also add absolute scaling using the reference $I_{0}$ value"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6a8e0b6b",
+            "id": "6ffa0b31-a43c-4f73-a568-5fa1ab2d61bf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.drop\n",
-                "result_drop = pipeline.compute(BackgroundSubtractedIofQ)\n",
-                "# Reset the UnsertaintyBroadcastMode to the old value\n",
-                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "sc.DataGroup(upper_bound=result, dropped=result_drop).hist().plot(norm='log')"
+                "results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "# Unpack the final result\n",
+                "iofq_full = results[-1]['iofq_full']\n",
+                "iofq_bands = results[-1]['iofq_bands']\n",
+                "direct_beam_function = results[-1]['direct_beam']"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "53ce1e48-b8a9-475a-b0ec-9ad204541543",
+            "id": "bc290019-85ea-406c-912d-75f1229f2ddf",
             "metadata": {},
             "source": [
-                "### Save reduced data to file\n",
-                "\n",
-                "`esssans` provides a function for saving the reduced data as an [NXcanSAS](https://manual.nexusformat.org/classes/applications/NXcanSAS.html) file.\n",
-                "It could be used directly with the `result` computed above, but we would have to provide the required metadata ourselves.\n",
-                "Instead, we use Sciline to get all required information directly from the pipeline: (See also the [File output](https://scipp.github.io/sciline/recipes/recipes.html#File-output) docs.)"
+                "We now compare the $I(Q)$ curves in each wavelength band to the one for the full wavelength range (black)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b83c7580-fba7-43d8-b9d0-1aeeebbe0301",
+            "id": "0055bce0-18f2-425d-937b-fb8e211247b1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from esssans.io import save_background_subtracted_iofq\n",
-                "\n",
-                "pipeline.bind_and_call(save_background_subtracted_iofq)"
+                "pp.plot(\n",
+                "    {**sc.collapse(iofq_bands, keep='Q'), **{'full': iofq_full}},\n",
+                "    norm='log',\n",
+                "    color={'full': 'k'},\n",
+                "    legend=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f39206c6",
+            "id": "d0a96015-061c-47ce-8384-2f34c8088332",
             "metadata": {},
             "source": [
-                "### Compute intermediate results\n",
-                "\n",
-                "For inspection and debugging purposes we can also compute intermediate results.\n",
-                "To avoid repeated computation (including costly loading of files) we can request multiple results at once, including the final result, if desired.\n",
-                "For example:"
+                "The overlap is satisfactory, and we can now inspect the direct beam function we have computed:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d4b514c3-af6e-441f-82a5-28bfc0110248",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "direct_beam_function.plot(vmax=1)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8b796452-7aaa-42fa-8cde-0c80a66ad1e2",
+            "metadata": {},
+            "source": [
+                "Finally, as a sanity check, we compare our final $I(Q)$ for the full wavelength range to the theoretical reference:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bb922379",
+            "id": "e491bd2d-5134-4837-b792-683f9ffd9e1d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from esssans.isis import plot_flat_detector_xy\n",
+                "pp.plot(\n",
+                "    {'reference': Iq_theory, 'data': iofq_full},\n",
+                "    color={'reference': 'darkgrey', 'data': 'C0'},\n",
+                "    norm='log',\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0c616af7-b66c-4ae6-888e-1884d3ac9db1",
+            "metadata": {},
+            "source": [
+                "## Direct beam function per layer\n",
                 "\n",
-                "monitors = (\n",
-                "    WavelengthMonitor[SampleRun, Incident],\n",
-                "    WavelengthMonitor[SampleRun, Transmission],\n",
-                "    WavelengthMonitor[BackgroundRun, Incident],\n",
-                "    WavelengthMonitor[BackgroundRun, Transmission],\n",
-                ")\n",
-                "parts = (CleanSummedQ[SampleRun, Numerator], CleanSummedQ[SampleRun, Denominator])\n",
-                "iofqs = (IofQ[SampleRun], IofQ[BackgroundRun], BackgroundSubtractedIofQ)\n",
-                "keys = monitors + (MaskedData[SampleRun],) + parts + iofqs\n",
-                "\n",
-                "results = pipeline.compute(keys)\n",
-                "\n",
-                "display(sc.plot({str(key): results[key] for key in monitors}, norm='log'))\n",
-                "\n",
-                "display(plot_flat_detector_xy(results[MaskedData[SampleRun]].sum('tof'), norm='log'))\n",
-                "\n",
-                "wavelength = pipeline.compute(WavelengthBins)\n",
-                "display(\n",
-                "    results[CleanSummedQ[SampleRun, Numerator]]\n",
-                "    .hist(wavelength=wavelength)\n",
-                "    .transpose()\n",
-                "    .plot(norm='log')\n",
-                ")\n",
-                "display(results[CleanSummedQ[SampleRun, Denominator]].plot(norm='log'))\n",
-                "parts = {str(key): results[key].sum('wavelength') for key in parts}\n",
-                "display(sc.plot(parts, norm='log'))\n",
+                "The LoKI detector tubes are arranged in layers along the beam path,\n",
+                "where the layers closest to the sample will receive most of the scattered neutrons,\n",
+                "while occulting the layers behind them.\n",
                 "\n",
-                "iofqs = {str(key): results[key] for key in iofqs}\n",
-                "iofqs = {key: val if val.bins is None else val.hist() for key, val in iofqs.items()}\n",
-                "display(sc.plot(iofqs, norm='log'))"
+                "A refinement to the above procedure is to compute a direct beam function for each layer of tubes individually.\n",
+                "We also use the 4 thick layers of tubes, but in principle,\n",
+                "this could also be done for 28 different layers (made from the `layer` and `straw` dimensions) if a run with enough events is provided (or many runs are combined together).\n",
+                "\n",
+                "The only other difference compared to the computation above is that we now want our final result to preserve the `'layer'` dimension,\n",
+                "so that the dimensions of our result are `['layer', 'Q']`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "64682705-3322-4003-8a56-f52f2523c8d4",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pipeline[DimsToKeep] = ['layer']"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "372b8d4f",
+            "id": "92691c97-4883-41b4-b880-17e0359191a2",
             "metadata": {},
             "source": [
-                "### Avoiding duplicate computation with parameter tables\n",
-                "\n",
-                "We have seen above that Sciline can avoid duplicate computation by requesting multiple results.\n",
-                "However, this is not always possible, for example if we want to compute the final result with different parameters.\n",
-                "In this case we can use parameter tables to avoid duplicate computation.\n",
-                "For example, we can compute the final result with different values for handling the uncertainties of the normalization factors.\n",
-                "This will avoid repeating loading files as well as some computation steps:"
+                "Now we are able to run the direct-beam iterations on a per-layer basis:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ceb079ee",
+            "id": "7e039618-d8c9-4201-9a9f-59738034786b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from typing import NewType\n",
+                "results_layers = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "# Unpack the final result\n",
+                "iofq_full_layers = results_layers[-1]['iofq_full']\n",
+                "iofq_bands_layers = results_layers[-1]['iofq_bands']\n",
+                "direct_beam_function_layers = results_layers[-1]['direct_beam']"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "642c52a3-d174-4b75-b1ee-877231c316dd",
+            "metadata": {},
+            "source": [
+                "We can now inspect the wavelength slices for the 4 layers."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "591cb3c7-63c4-427f-97c9-f2ad332d6c37",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plots = [\n",
+                "    pp.plot(\n",
+                "        {\n",
+                "            **sc.collapse(iofq_bands_layers['layer', i], keep='Q'),\n",
+                "            **{'full': iofq_full_layers['layer', i]},\n",
+                "        },\n",
+                "        norm='log',\n",
+                "        color={'full': 'k'},\n",
+                "        legend=False,\n",
+                "        title=f'Layer {i}',\n",
+                "    )\n",
+                "    for i in range(4)\n",
+                "]\n",
                 "\n",
-                "Mode = NewType('Mode', str)\n",
-                "param_table = sciline.ParamTable(\n",
-                "    Mode,\n",
-                "    {\n",
-                "        UncertaintyBroadcastMode: [\n",
-                "            UncertaintyBroadcastMode.upper_bound,\n",
-                "            UncertaintyBroadcastMode.drop,\n",
-                "        ]\n",
+                "(plots[0] + plots[1]) / (plots[2] + plots[3])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9e1313fd-8f01-4a47-abf3-d641232b3d47",
+            "metadata": {},
+            "source": [
+                "Now the direct beam function inside each layer looks like:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2fde077a-4d16-44b1-af0e-58216a8db57e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pp.plot(sc.collapse(direct_beam_function_layers, keep='wavelength'))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "2a49bcac-0283-4802-97f4-a5a8453383cf",
+            "metadata": {},
+            "source": [
+                "And finally, for completeness, we compare the $I(Q)$ to the theoretical reference inside each layer."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a6411f70-f7e2-4061-8641-cc612a19a080",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "layers = sc.collapse(iofq_full_layers, keep='Q')\n",
+                "pp.plot(\n",
+                "    {**{'reference': Iq_theory}, **layers},\n",
+                "    color={\n",
+                "        **{'reference': 'darkgrey'},\n",
+                "        **{key: f'C{i}' for i, key in enumerate(layers)},\n",
                 "    },\n",
-                "    index=[Mode('upper_bound'), Mode('drop')],\n",
-                ")\n",
-                "pipeline.set_param_table(param_table)\n",
-                "results = pipeline.compute(sciline.Series[Mode, BackgroundSubtractedIofQ])\n",
-                "sc.DataGroup(results).hist().plot(norm='log')"
+                "    norm='log',\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "94062d33-04cb-4a4d-aef1-e5ec58c228c4",
+            "id": "7cbff973-fbb7-4187-82e8-8e4fa82efcb8",
             "metadata": {},
             "source": [
-                "## Wavelength bands\n",
+                "## Combining multiple runs to boost signal\n",
+                "\n",
+                "It is common practise to combine the events from multiple runs to improve the statistics on the computed $I(Q)$,\n",
+                "and thus obtain a more robust direct beam function.\n",
                 "\n",
-                "We can also compute $I(Q)$ inside a set of wavelength bands, instead of using the full wavelength range in one go.\n",
-                "This is useful for debugging purposes.\n",
+                "To achieve this, we need to replace the `SampleRun` and `BackgroundRun` file names with parameter series.\n",
+                "We then need to supply additional providers which will merge the events from the runs appropriately\n",
+                "(note that these providers will merge both the detector and the monitor events).\n",
                 "\n",
-                "To achieve this, we need to supply the `WavelengthBands` parameter (as a two-dimensional variable),\n",
-                "representing the wavelength range for each band."
+                "We first define a list of file names for the sample and background runs (two files for each):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "27068e8a-350f-4ea4-b4a4-2b13926905b5",
+            "id": "bf5f23b0-e4b6-48d8-b98a-99ec5e56be4e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[WavelengthBands] = sc.linspace(\n",
-                "    'wavelength', start=2.0, stop=16.0, num=11, unit='angstrom'\n",
-                ")"
+                "del params[Filename[SampleRun]]\n",
+                "del params[Filename[BackgroundRun]]\n",
+                "\n",
+                "sample_runs = ['60250-2022-02-28_2215.nxs', '60339-2022-02-28_2215.nxs']\n",
+                "background_runs = ['60248-2022-02-28_2215.nxs', '60393-2022-02-28_2215.nxs']"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c3e2ff3d-2b3d-4ba7-b4ca-f0a5617d22dc",
+            "metadata": {},
+            "source": [
+                "We now construct a new pipeline, inserting parameter series and merging providers:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2a39bd50-5d63-4183-9afe-6d990548bc11",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Same as original pipeline, but without sample and background run file names\n",
+                "params[BeamCenter] = center\n",
+                "pipeline = sciline.Pipeline(providers, params=params)\n",
+                "for provider in loki.data.providers:\n",
+                "    pipeline.insert(provider)\n",
+                "pipeline.insert(sans.merge_banks)\n",
+                "pipeline.set_param_series(PixelMaskFilename, masks)\n",
+                "pipeline.set_param_series(NeXusDetectorName, banks)\n",
+                "\n",
+                "# Set parameter series for file names\n",
+                "pipeline.set_param_series(Filename[SampleRun], sample_runs)\n",
+                "pipeline.set_param_series(Filename[BackgroundRun], background_runs)\n",
+                "\n",
+                "# Add event merging provider\n",
+                "pipeline.insert(sans.merge_runs)\n",
+                "\n",
+                "# Add dummy sample provider\n",
+                "pipeline.insert(loki.io.dummy_load_sample)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cc3cac02-2cb4-4da5-a83d-8e6fb3d2c929",
+            "id": "6a50ef4f-a15c-4ae4-a8e7-666483a93da0",
             "metadata": {},
             "source": [
-                "Compute the result:"
+                "If we now visualize the pipeline,\n",
+                "we can see that every step for the `SampleRun` and `BackgroundRun` branches are now series of types (3D-looking boxes instead of flat rectangles).\n",
+                "There is also the new `merge_multiple_runs` step that combines the events from the two runs,\n",
+                "just before the normalization."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6bd670f9-85db-4257-ab67-e296a7e8ecdf",
+            "id": "4ab8426a-d7b9-4ffe-aa9b-e029b5888ae0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = pipeline.compute(BackgroundSubtractedIofQ)\n",
-                "result"
+                "pipeline.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "601d2a4f-1295-4918-8177-d2dca0b839f9",
+            "id": "1c674237-c85e-4e1f-b136-1d9f53494572",
             "metadata": {},
             "source": [
-                "The result is two-dimensional and we over-plot all the bands onto the same axes:"
+                "We run the direct beam iterations again and compare with our original results."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d5df969d-79d1-443a-a71b-88faf8b57a37",
+            "id": "0c132101-9dfc-4896-bb68-56a0878bfcef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.plot(sc.collapse(result.hist(), keep='Q'), norm='log')"
+                "results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "# Unpack the final result\n",
+                "iofq_full_new = results[-1]['iofq_full']\n",
+                "iofq_bands_new = results[-1]['iofq_bands']\n",
+                "direct_beam_function_new = results[-1]['direct_beam']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c731cf0c-4451-445f-a8bf-46a952ab171f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pp.plot({'one run': direct_beam_function, 'two runs': direct_beam_function_new})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "50f78446-b7e4-406a-a5fd-5548e18dedc6",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pp.plot(\n",
+                "    {'reference': Iq_theory, 'one run': iofq_full, 'two runs': iofq_full_new},\n",
+                "    color={'reference': 'darkgrey', 'one run': 'C0', 'two runs': 'C1'},\n",
+                "    norm='log',\n",
+                ")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -395,13 +624,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.2.0/docs/examples/zoom.ipynb` & `esssans-24.4.0/docs/user-guide/isis/zoom.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9805722707285207%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'from ess import sans\\n'), (3, 'from ess import "*

 * *            "isissans as isis\\n'), (4, 'from ess.sans.types import *')], delete: [4, 3, 2]}}, 5: "*

 * *            '{\'source\': {insert: [(1, "    DirectBeamFilename: '*

 * *            '\'Direct_Zoom_4m_8mm_100522.txt\',\\n"), (2, "    isis.CalibrationFilename: '*

 * *            '\'192tubeCalibration_11-02-2019_r5_10lines.nxs\',\\n"), (3, "    Filename[SampleRun]: '*

 * *            '\'ZOOM00034786.nxs\',\\n"), (4, "    Filename[E […]*

```diff
@@ -40,17 +40,17 @@
             "execution_count": null,
             "id": "319162e9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
                 "import sciline\n",
-                "import esssans as sans\n",
-                "import esssans.isis\n",
-                "from esssans.types import *"
+                "from ess import sans\n",
+                "from ess import isissans as isis\n",
+                "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "64783c51",
             "metadata": {},
             "source": [
@@ -61,31 +61,30 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "9e7cfc82",
             "metadata": {},
             "outputs": [],
             "source": [
                 "params = {\n",
-                "    sans.types.DirectBeamFilename: 'Direct_Zoom_4m_8mm_100522.txt',\n",
-                "    sans.isis.CalibrationFilename: '192tubeCalibration_11-02-2019_r5_10lines.nxs',\n",
-                "    sans.isis.Filename[sans.types.SampleRun]: 'ZOOM00034786.nxs',\n",
-                "    sans.isis.Filename[sans.types.EmptyBeamRun]: 'ZOOM00034787.nxs',\n",
-                "    sans.isis.SampleOffset: sc.vector([0.0, 0.0, 0.11], unit='m'),\n",
-                "    sans.isis.DetectorBankOffset: sc.vector([0.0, 0.0, 0.5], unit='m'),\n",
+                "    DirectBeamFilename: 'Direct_Zoom_4m_8mm_100522.txt',\n",
+                "    isis.CalibrationFilename: '192tubeCalibration_11-02-2019_r5_10lines.nxs',\n",
+                "    Filename[SampleRun]: 'ZOOM00034786.nxs',\n",
+                "    Filename[EmptyBeamRun]: 'ZOOM00034787.nxs',\n",
+                "    isis.SampleOffset: sc.vector([0.0, 0.0, 0.11], unit='m'),\n",
+                "    isis.DetectorBankOffset: sc.vector([0.0, 0.0, 0.5], unit='m'),\n",
                 "}\n",
                 "masks = [\n",
                 "    'andru_test.xml',\n",
                 "    'left_beg_18_2.xml',\n",
                 "    'right_beg_18_2.xml',\n",
                 "    'small_bs_232.xml',\n",
                 "    'small_BS_31032023.xml',\n",
                 "    'tube_1120_bottom.xml',\n",
                 "    'tubes_beg_18_2.xml',\n",
-                "]\n",
-                "masks = sciline.ParamTable(str, {sans.isis.PixelMaskFilename: masks}, index=masks)"
+                "]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8a8a4e01",
             "metadata": {},
             "source": [
@@ -103,26 +102,21 @@
                 "params[NeXusMonitorName[Transmission]] = 'monitor5'\n",
                 "\n",
                 "params[WavelengthBins] = sc.geomspace(\n",
                 "    'wavelength', start=1.75, stop=16.5, num=141, unit='angstrom'\n",
                 ")\n",
                 "\n",
                 "params[QBins] = sc.geomspace(dim='Q', start=0.004, stop=0.8, num=141, unit='1/angstrom')\n",
-                "qxy = {\n",
-                "    'Qx': sc.linspace(dim='Qx', start=-0.5, stop=0.5, num=101, unit='1/angstrom'),\n",
-                "    'Qy': sc.linspace(dim='Qy', start=-0.8, stop=0.8, num=101, unit='1/angstrom'),\n",
-                "}\n",
-                "# Uncomment to compute I(Qx, Qy) instead of I(Q)\n",
-                "# params[QxyBins] = qxy\n",
+                "\n",
                 "params[NonBackgroundWavelengthRange] = sc.array(\n",
                 "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
                 ")\n",
                 "params[CorrectForGravity] = True\n",
                 "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[sans.ReturnEvents] = False"
+                "params[ReturnEvents] = False"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b47024f",
             "metadata": {},
             "source": [
@@ -132,21 +126,22 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fdcaec37",
             "metadata": {},
             "outputs": [],
             "source": [
-                "providers = sans.providers + sans.isis.providers\n",
+                "providers = sans.providers + isis.providers + (isis.io.read_xml_detector_masking,)\n",
                 "providers = providers + (\n",
-                "    sans.transmission_from_background_run,\n",
-                "    sans.transmission_from_sample_run,\n",
+                "    isis.data.transmission_from_background_run,\n",
+                "    isis.data.transmission_from_sample_run,\n",
+                "    sans.beam_center_from_center_of_mass,\n",
                 ")\n",
                 "pipeline = sciline.Pipeline(providers, params=params)\n",
-                "pipeline.set_param_table(masks)"
+                "pipeline.set_param_series(PixelMaskFilename, masks)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "951aec10",
             "metadata": {},
             "source": [
@@ -161,26 +156,26 @@
             "execution_count": null,
             "id": "66237b3e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    from mantid import ConfigService\n",
-                "    import esssans.isis.mantidio\n",
+                "    import ess.isissans.mantidio\n",
                 "\n",
                 "    cfg = ConfigService.Instance()\n",
                 "    cfg.setLogLevel(3)  # Silence verbose load via Mantid\n",
                 "\n",
-                "    pipeline[sans.isis.DataFolder] = 'zoom_data'\n",
-                "    for provider in sans.isis.mantidio.providers:\n",
+                "    pipeline[DataFolder] = 'zoom_data'\n",
+                "    for provider in isis.mantidio.providers:\n",
                 "        pipeline.insert(provider)\n",
                 "except ImportError:\n",
-                "    import esssans.isis.data\n",
+                "    import ess.isissans.io\n",
                 "\n",
-                "    for provider in sans.isis.data.providers:\n",
+                "    for provider in isis.data.providers:\n",
                 "        pipeline.insert(provider)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "703ffc1e",
             "metadata": {},
@@ -189,15 +184,15 @@
                 "\n",
                 "### The reduction workflow"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cae69232",
+            "id": "029e7c10-3428-4c10-8a5d-fa49b807a785",
             "metadata": {},
             "outputs": [],
             "source": [
                 "iofq = pipeline.get(IofQ[SampleRun])\n",
                 "iofq.visualize(graph_attr={'rankdir': 'LR'}, compact=True)"
             ]
         },
@@ -213,15 +208,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "558327ff",
             "metadata": {},
             "outputs": [],
             "source": [
                 "da = iofq.compute()\n",
-                "da.plot(norm='log', scale={'Q': 'log'}, aspect='equal')"
+                "da.plot(norm='log', scale={'Q': 'log'})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5a7526fc",
             "metadata": {},
             "source": [
@@ -244,15 +239,15 @@
                 "keys = monitors + (MaskedData[SampleRun],) + parts + iofqs\n",
                 "\n",
                 "results = pipeline.compute(keys)\n",
                 "\n",
                 "display(sc.plot({str(key): results[key] for key in monitors}, norm='log'))\n",
                 "\n",
                 "display(\n",
-                "    sans.isis.plot_flat_detector_xy(\n",
+                "    isis.plot_flat_detector_xy(\n",
                 "        results[MaskedData[SampleRun]], norm='log', figsize=(6, 10)\n",
                 "    )\n",
                 ")\n",
                 "\n",
                 "wavelength = pipeline.compute(WavelengthBins)\n",
                 "display(\n",
                 "    results[CleanSummedQ[SampleRun, Numerator]]\n",
@@ -268,14 +263,41 @@
                 "}\n",
                 "display(sc.plot(parts, norm='log', scale={'Q': 'log'}))\n",
                 "\n",
                 "iofqs = {str(key): results[key] for key in iofqs}\n",
                 "iofqs = {key: val if val.bins is None else val.hist() for key, val in iofqs.items()}\n",
                 "display(sc.plot(iofqs, norm='log', scale={'Q': 'log'}, aspect='equal'))"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e63318c7-4d63-4133-97c3-feb56707caba",
+            "metadata": {},
+            "source": [
+                "## Computing Qx/Qy\n",
+                "\n",
+                "To compute $I(Q_{x}, Q_{y})$ instead of the one-dimensional $I(Q)$,\n",
+                "we can simply define some `QxyBins` in our parameters:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3879702d-424a-462f-8475-6056116d7d35",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pipeline[QxyBins] = {\n",
+                "    'Qx': sc.linspace(dim='Qx', start=-0.5, stop=0.5, num=101, unit='1/angstrom'),\n",
+                "    'Qy': sc.linspace(dim='Qy', start=-0.8, stop=0.8, num=101, unit='1/angstrom'),\n",
+                "}\n",
+                "\n",
+                "iqxqy = pipeline.compute(IofQ[SampleRun])\n",
+                "iqxqy.plot(norm='log', aspect='equal')"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -285,14 +307,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.2.0/pyproject.toml` & `esssans-24.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 
 # IMPORTANT:
 # Run 'tox -e deps' after making changes here. This will update requirement files.
 # Make sure to list one dependency per line.
 dependencies = [
   "dask",
   "graphviz",
+  "essreduce",
   "plopp",
   "pythreejs",
-  "sciline>=23.9.1",
+  "sciline>=24.4.1",
   "scipp>=23.8.0",
   "scippneutron>=23.9.0",
   "scippnexus>=23.12.1",  # 23.12.0 and below deadlock in threaded use
 ]
 
 dynamic = ["version"]
```

### Comparing `esssans-24.2.0/requirements/base.txt` & `esssans-24.4.0/requirements/nightly.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,159 @@
-# SHA1:d9131f52f58d87889ced7f09fded3a470b1c0a71
+# SHA1:16b2b3d983c096ba312d853cbfe99af3c40ea8c1
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
+-r basetest.txt
 asttokens==2.4.1
     # via stack-data
-backcall==0.2.0
-    # via ipython
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via dask
 cloudpickle==3.0.0
     # via dask
-comm==0.2.1
+comm==0.2.2
     # via ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.1.0
-    # via -r base.in
+dask==2024.4.1
+    # via -r nightly.in
 decorator==5.1.1
     # via ipython
+essreduce==24.3.11
+    # via -r nightly.in
 executing==2.0.1
     # via stack-data
-fonttools==4.47.2
+fonttools==4.50.0
     # via matplotlib
-fsspec==2023.12.2
+fsspec==2024.3.1
     # via dask
-graphviz==0.20.1
-    # via -r base.in
+graphviz==0.20.3
+    # via -r nightly.in
 h5py==3.10.0
     # via
     #   scippneutron
     #   scippnexus
 idna==3.6
     # via requests
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via dask
-importlib-resources==6.1.1
-    # via matplotlib
 ipydatawidgets==4.3.5
     # via pythreejs
-ipython==8.9.0
-    # via
-    #   -r base.in
-    #   ipywidgets
-ipywidgets==8.1.1
+ipython==8.23.0
+    # via ipywidgets
+ipywidgets==8.1.2
     # via
     #   ipydatawidgets
     #   pythreejs
 jedi==0.19.1
     # via ipython
-jupyterlab-widgets==3.0.9
+jupyterlab-widgets==3.0.10
     # via ipywidgets
 kiwisolver==1.4.5
     # via matplotlib
 locket==1.0.0
     # via partd
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via plopp
 matplotlib-inline==0.1.6
     # via ipython
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   h5py
     #   ipydatawidgets
     #   matplotlib
     #   pythreejs
     #   scipp
     #   scippneutron
     #   scipy
-packaging==23.2
-    # via
-    #   dask
-    #   matplotlib
-    #   pooch
 parso==0.8.3
     # via jedi
 partd==1.4.1
     # via dask
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via pooch
-plopp==24.1.1
-    # via -r base.in
-pooch==1.8.0
+plopp @ git+https://github.com/scipp/plopp@main
+    # via -r nightly.in
+pooch==1.8.1
     # via scippneutron
-prompt-toolkit==3.0.36
-    # via
-    #   -r base.in
-    #   ipython
+prompt-toolkit==3.0.43
+    # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pygments==2.17.2
     # via ipython
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   scippnexus
 pythreejs==2.4.2
-    # via -r base.in
+    # via -r nightly.in
 pyyaml==6.0.1
     # via dask
 requests==2.31.0
     # via pooch
-sciline==24.1.1
-    # via -r base.in
-scipp==23.12.0
+sciline @ git+https://github.com/scipp/sciline@main
+    # via -r nightly.in
+scipp @ https://github.com/scipp/scipp/releases/download/nightly/scipp-nightly-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
     # via
-    #   -r base.in
+    #   -r nightly.in
+    #   essreduce
     #   scippneutron
     #   scippnexus
-scippneutron==23.11.0
-    # via -r base.in
-scippnexus==23.12.1
+scippneutron @ git+https://github.com/scipp/scippneutron@main
+    # via -r nightly.in
+scippnexus @ git+https://github.com/scipp/scippnexus@main
     # via
-    #   -r base.in
+    #   -r nightly.in
+    #   essreduce
     #   scippneutron
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   scippneutron
     #   scippnexus
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 stack-data==0.6.3
     # via ipython
 toolz==0.12.1
     # via
     #   dask
     #   partd
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   comm
     #   ipython
     #   ipywidgets
     #   matplotlib-inline
     #   pythreejs
     #   traittypes
 traittypes==0.2.1
     # via ipydatawidgets
-urllib3==2.1.0
+typing-extensions==4.10.0
+    # via ipython
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
-widgetsnbextension==4.0.9
+widgetsnbextension==4.0.10
     # via ipywidgets
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.18.1
+    # via importlib-metadata
```

### Comparing `esssans-24.2.0/requirements/ci.txt` & `esssans-24.4.0/requirements/ci.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # SHA1:6344d52635ea11dca331a3bc6eb1833c4c64d585
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.2
+cachetools==5.3.3
     # via tox
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.41
+gitpython==3.1.43
     # via -r ci.in
 idna==3.6
     # via requests
-packaging==23.2
+packaging==24.0
     # via
     #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.4.0
     # via tox
 pyproject-api==1.6.1
     # via tox
 requests==2.31.0
     # via -r ci.in
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.12.1
+tox==4.14.2
     # via -r ci.in
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
-virtualenv==20.25.0
+virtualenv==20.25.1
     # via tox
```

### Comparing `esssans-24.2.0/requirements/dev.txt` & `esssans-24.4.0/requirements/dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,114 +10,122 @@
 -r docs.txt
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
 annotated-types==0.6.0
     # via pydantic
-anyio==4.2.0
-    # via jupyter-server
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 async-lru==2.0.4
     # via jupyterlab
 cffi==1.16.0
     # via argon2-cffi-bindings
-copier==9.1.1
+copier==9.2.0
     # via -r dev.in
-dunamai==1.19.0
+dunamai==1.19.2
     # via copier
 fqdn==1.5.1
     # via jsonschema
 funcy==2.0
     # via copier
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
 isoduration==20.11.0
     # via jsonschema
 jinja2-ansible-filters==1.3.2
     # via copier
-json5==0.9.14
+json5==0.9.24
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-events==0.9.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.2
+jupyter-lsp==2.2.4
     # via jupyterlab
-jupyter-server==2.12.5
+jupyter-server==2.13.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
-jupyter-server-terminals==0.5.2
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.11
+jupyterlab==4.1.5
     # via -r dev.in
-jupyterlab-server==2.25.2
+jupyterlab-server==2.25.4
     # via jupyterlab
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via jupyterlab
-overrides==7.6.0
+overrides==7.7.0
     # via jupyter-server
 pathspec==0.12.1
     # via copier
 pip-compile-multi==2.6.3
     # via -r dev.in
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via pip-compile-multi
 plumbum==1.8.2
     # via copier
-prometheus-client==0.19.0
+prometheus-client==0.20.0
     # via jupyter-server
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.5.3
+pydantic==2.6.4
     # via copier
-pydantic-core==2.14.6
+pydantic-core==2.16.3
     # via pydantic
 python-json-logger==2.0.7
     # via jupyter-events
-pyyaml-include==1.3.2
-    # via copier
 questionary==2.0.1
     # via copier
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
 send2trash==1.8.2
     # via jupyter-server
-sniffio==1.3.0
-    # via anyio
-terminado==0.18.0
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
 uri-template==1.3.0
     # via jsonschema
 webcolors==1.13
     # via jsonschema
 websocket-client==1.7.0
     # via jupyter-server
-wheel==0.42.0
+wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `esssans-24.2.0/requirements/docs.txt` & `esssans-24.4.0/requirements/docs.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,74 +20,74 @@
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
-debugpy==1.8.0
+debugpy==1.8.1
     # via ipykernel
 defusedxml==0.7.1
     # via nbconvert
 docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx
 fastjsonschema==2.19.1
     # via nbformat
 imagesize==1.4.1
     # via sphinx
-ipykernel==6.29.0
+ipykernel==6.29.4
     # via -r docs.in
 jinja2==3.1.3
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.3.0
     # via nbconvert
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.4
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
 myst-parser==2.0.0
     # via -r docs.in
-nbclient==0.9.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.14.2
+nbconvert==7.16.3
     # via nbsphinx
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
 nbsphinx==0.9.3
     # via -r docs.in
 nest-asyncio==1.6.0
@@ -98,19 +98,19 @@
     # via ipykernel
 pydata-sphinx-theme==0.15.2
     # via -r docs.in
 pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.32.1
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
@@ -119,15 +119,15 @@
     #   -r docs.in
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
-sphinx-autodoc-typehints==1.25.2
+sphinx-autodoc-typehints==2.0.0
     # via -r docs.in
 sphinx-copybutton==0.5.2
     # via -r docs.in
 sphinx-design==0.5.0
     # via -r docs.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
@@ -143,13 +143,13 @@
     # via sphinx
 tinycss2==1.2.1
     # via nbconvert
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-typing-extensions==4.9.0
+typing-extensions==4.10.0
     # via pydata-sphinx-theme
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
```

### Comparing `esssans-24.2.0/requirements/make_base.py` & `esssans-24.4.0/requirements/make_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import List
 
 import tomli
 
@@ -39,15 +36,15 @@
         f.write("\n".join(dependencies))
         f.write("\n")
 
 
 with open("../pyproject.toml", "rb") as toml_file:
     pyproject = tomli.load(toml_file)
     dependencies = pyproject["project"].get("dependencies")
-    if not dependencies:
+    if dependencies is None:
         raise RuntimeError("No dependencies found in pyproject.toml")
     dependencies = [dep.strip().strip('"') for dep in dependencies]
 
 write_dependencies("base", dependencies)
 
 
 def as_nightly(repo: str) -> str:
```

### Comparing `esssans-24.2.0/requirements/nightly.txt` & `esssans-24.4.0/requirements/base.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,169 @@
-# SHA1:2bc7b1dfb021783d1944cdb011794a7d75aa0763
+# SHA1:a7107dcab866c4c7fe8573b3c5cbaf22e7b1f587
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
--r basetest.txt
 asttokens==2.4.1
     # via stack-data
-certifi==2023.11.17
+backcall==0.2.0
+    # via ipython
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via dask
 cloudpickle==3.0.0
     # via dask
-comm==0.2.1
+comm==0.2.2
     # via ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.1.0
-    # via -r nightly.in
+dask==2024.4.1
+    # via -r base.in
 decorator==5.1.1
     # via ipython
+essreduce==24.3.11
+    # via -r base.in
 executing==2.0.1
     # via stack-data
-fonttools==4.47.2
+fonttools==4.50.0
     # via matplotlib
-fsspec==2023.12.2
+fsspec==2024.3.1
     # via dask
-graphviz==0.20.1
-    # via -r nightly.in
+graphviz==0.20.3
+    # via -r base.in
 h5py==3.10.0
     # via
     #   scippneutron
     #   scippnexus
 idna==3.6
     # via requests
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via dask
-importlib-resources==6.1.1
-    # via matplotlib
 ipydatawidgets==4.3.5
     # via pythreejs
-ipython==8.18.1
-    # via ipywidgets
-ipywidgets==8.1.1
+ipython==8.9.0
+    # via
+    #   -r base.in
+    #   ipywidgets
+ipywidgets==8.1.2
     # via
     #   ipydatawidgets
     #   pythreejs
 jedi==0.19.1
     # via ipython
-jupyterlab-widgets==3.0.9
+jupyterlab-widgets==3.0.10
     # via ipywidgets
 kiwisolver==1.4.5
     # via matplotlib
 locket==1.0.0
     # via partd
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via plopp
 matplotlib-inline==0.1.6
     # via ipython
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   h5py
     #   ipydatawidgets
     #   matplotlib
     #   pythreejs
     #   scipp
     #   scippneutron
     #   scipy
+packaging==24.0
+    # via
+    #   dask
+    #   matplotlib
+    #   pooch
 parso==0.8.3
     # via jedi
 partd==1.4.1
     # via dask
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via matplotlib
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via pooch
-plopp @ git+https://github.com/scipp/plopp@main
-    # via -r nightly.in
-pooch==1.8.0
+plopp==24.2.0
+    # via -r base.in
+pooch==1.8.1
     # via scippneutron
-prompt-toolkit==3.0.43
-    # via ipython
+prompt-toolkit==3.0.36
+    # via
+    #   -r base.in
+    #   ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pygments==2.17.2
     # via ipython
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   scippnexus
 pythreejs==2.4.2
-    # via -r nightly.in
+    # via -r base.in
 pyyaml==6.0.1
     # via dask
 requests==2.31.0
     # via pooch
-sciline @ git+https://github.com/scipp/sciline@main
-    # via -r nightly.in
-scipp @ https://github.com/scipp/scipp/releases/download/nightly/scipp-nightly-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+sciline==24.4.1
+    # via -r base.in
+scipp==24.2.0
     # via
-    #   -r nightly.in
+    #   -r base.in
+    #   essreduce
     #   scippneutron
     #   scippnexus
-scippneutron @ git+https://github.com/scipp/scippneutron@main
-    # via -r nightly.in
-scippnexus @ git+https://github.com/scipp/scippnexus@main
+scippneutron==24.3.0
+    # via -r base.in
+scippnexus==24.3.1
     # via
-    #   -r nightly.in
+    #   -r base.in
+    #   essreduce
     #   scippneutron
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   scippneutron
     #   scippnexus
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 stack-data==0.6.3
     # via ipython
 toolz==0.12.1
     # via
     #   dask
     #   partd
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   comm
     #   ipython
     #   ipywidgets
     #   matplotlib-inline
     #   pythreejs
     #   traittypes
 traittypes==0.2.1
     # via ipydatawidgets
-typing-extensions==4.9.0
-    # via ipython
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
-widgetsnbextension==4.0.9
+widgetsnbextension==4.0.10
     # via ipywidgets
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.18.1
+    # via importlib-metadata
```

### Comparing `esssans-24.2.0/resources/logo.svg` & `esssans-24.4.0/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/src/esssans/__init__.py` & `esssans-24.4.0/src/ess/sans/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
-# flake8: noqa
 import importlib.metadata
 
-try:
-    __version__ = importlib.metadata.version(__package__ or __name__)
-except importlib.metadata.PackageNotFoundError:
-    __version__ = "0.0.0"
-
 from . import (
     beam_center_finder,
     common,
     conversions,
     i_of_q,
     io,
-    loki,
+    masking,
     normalization,
-    sans2d,
 )
-from .common import transmission_from_background_run, transmission_from_sample_run
+from .beam_center_finder import beam_center_from_center_of_mass
 from .direct_beam import direct_beam
+from .i_of_q import merge_banks, merge_runs, no_bank_merge, no_run_merge
 from .types import BackgroundSubtractedIofQ, IofQ, ReturnEvents, SampleRun
 
+try:
+    __version__ = importlib.metadata.version(__package__ or __name__)
+except importlib.metadata.PackageNotFoundError:
+    __version__ = "0.0.0"
+
 providers = (
     *conversions.providers,
     *i_of_q.providers,
+    *masking.providers,
     *normalization.providers,
-    # Default to fast but potentially inaccurate beam center finder
-    beam_center_finder.beam_center_from_center_of_mass,
 )
 """
 List of providers for setting up a Sciline pipeline.
 
 This provides a default workflow, including a beam-center estimation based on a
 center-of-mass approach. Providers for loadings files are not included. Combine with
 the providers for a specific instrument, such as :py:data:`esssans.sans2d.providers`
@@ -43,19 +41,21 @@
 
 __all__ = [
     'BackgroundSubtractedIofQ',
     'IofQ',
     'SampleRun',
     'ReturnEvents',
     'beam_center_finder',
+    'beam_center_from_center_of_mass',
     'common',
     'conversions',
     'direct_beam',
     'i_of_q',
     'io',
-    'loki',
+    'masking',
+    'merge_banks',
+    'merge_runs',
+    'no_bank_merge',
+    'no_run_merge',
     'normalization',
     'providers',
-    'sans2d',
-    'transmission_from_sample_run',
-    'transmission_from_background_run',
 ]
```

### Comparing `esssans-24.2.0/src/esssans/beam_center_finder.py` & `esssans-24.4.0/src/ess/sans/beam_center_finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 from .conversions import (
     ElasticCoordTransformGraph,
     calibrate_positions,
     compute_Q,
     detector_to_wavelength,
     mask_wavelength,
 )
-from .i_of_q import merge_spectra
+from .i_of_q import bin_in_q, no_bank_merge, no_run_merge
 from .logging import get_logger
 from .normalization import (
     iofq_denominator,
     normalize,
     process_wavelength_bands,
     solid_angle,
 )
 from .types import (
     BeamCenter,
+    CalibratedMaskedData,
     DetectorPixelShape,
     IofQ,
     LabFrameTransform,
     MaskedData,
     NormWavelengthTerm,
     QBins,
     ReturnEvents,
@@ -160,27 +161,22 @@
     -------
     :
         A dictionary containing the intensity as a function of Q in each quadrant.
         The quadrants are named 'south-west', 'south-east', 'north-east', and
         'north-west'.
     """
     pi = sc.constants.pi.value
-    phi = data.transform_coords(
-        'phi', graph=graph, keep_intermediate=False, keep_inputs=False
-    ).coords['phi']
-    if phi.bins is not None or 'wavelength' in phi.dims:
-        # If gravity-correction is enabled, phi depends on wavelength (and event).
-        # We cannot handle this below, so we approximate phi by the mean value.
-        phi = phi.mean('wavelength')
     phi_bins = sc.linspace('phi', -pi, pi, 5, unit='rad')
     quadrants = ['south-west', 'south-east', 'north-east', 'north-west']
 
     providers = [
         compute_Q,
-        merge_spectra,
+        bin_in_q,
+        no_run_merge,
+        no_bank_merge,
         normalize,
         iofq_denominator,
         mask_wavelength,
         detector_to_wavelength,
         solid_angle,
         calibrate_positions,
         process_wavelength_bands,
@@ -191,23 +187,38 @@
     params[WavelengthBins] = wavelength_bins
     params[QBins] = q_bins
     params[DetectorPixelShape[SampleRun]] = pixel_shape
     params[LabFrameTransform[SampleRun]] = transform
     params[ElasticCoordTransformGraph] = graph
     params[BeamCenter] = _offsets_to_vector(data=data, xy=xy, graph=graph)
 
+    pipeline = sciline.Pipeline(providers, params=params)
+    pipeline[MaskedData[SampleRun]] = data
+    calibrated = pipeline.compute(CalibratedMaskedData[SampleRun])
+    with_phi = calibrated.transform_coords(
+        'phi', graph=graph, keep_intermediate=False, keep_inputs=False
+    )
+    # If gravity-correction is enabled, phi depends on wavelength (and event).
+    # We cannot handle this below, so we approximate phi by the mean value.
+    if ('phi' not in with_phi.coords) and ('phi' in with_phi.bins.coords):
+        # This is the case where we have a phi event coord but no coord at the top level
+        phi = with_phi.bins.coords['phi'].bins.mean()
+    else:
+        phi = with_phi.coords['phi']
+        if phi.bins is not None or 'wavelength' in phi.dims:
+            phi = phi.mean('wavelength')
+
     out = {}
     for i, quad in enumerate(quadrants):
         # Select pixels based on phi
         sel = (phi >= phi_bins[i]) & (phi < phi_bins[i + 1])
-        params[MaskedData[SampleRun]] = data[sel]
-        params[NormWavelengthTerm[SampleRun]] = (
+        pipeline[MaskedData[SampleRun]] = data[sel]
+        pipeline[NormWavelengthTerm[SampleRun]] = (
             norm if norm.dims == ('wavelength',) else norm[sel]
         )
-        pipeline = sciline.Pipeline(providers, params=params)
         out[quad] = pipeline.compute(IofQ[SampleRun])
     return out
 
 
 def _cost(xy: List[float], *args) -> float:
     """
     Cost function for determining how close the :math:`I(Q)` curves are in all four
@@ -260,21 +271,23 @@
     """  # noqa: E501
     iofq = _iofq_in_quadrants(xy, *args)
     all_q = sc.concat([sc.values(da) for da in iofq.values()], dim='quadrant')
     ref = all_q.mean('quadrant')
     c = (all_q - ref) ** 2
     out = (sc.sum(ref * c) / sc.sum(ref)).value
     logger = get_logger('sans')
-    logger.info(f'Beam center finder: x={xy[0]}, y={xy[1]}, cost={out}')
     if not np.isfinite(out):
-        raise ValueError(
+        out = np.inf
+        logger.info(
             'Non-finite value computed in cost. This is likely due to a division by '
-            'zero. Try restricting your Q range, or increasing the size of your Q bins '
-            'to improve statistics in the denominator.'
+            'zero. If the final results for the beam center are not satisfactory, '
+            'try restricting your Q range, or increasing the size of your Q bins to '
+            'improve statistics in the denominator.'
         )
+    logger.info(f'Beam center finder: x={xy[0]}, y={xy[1]}, cost={out}')
     return out
 
 
 BeamCenterFinderQBins = NewType('BeamCenterFinderQBins', sc.Variable)
 """Q binning used for the beam center finder"""
 
 BeamCenterFinderTolerance = NewType('BeamCenterFinderTolerance', float)
@@ -383,16 +396,16 @@
     result.
     We write 'as close as possible' because In the full :math:`I(Q)` reduction, there
     is a term :math:`D({\\lambda})` in the normalization called the 'direct beam' which
     gives the efficiency of the detectors as a function of wavelength.
     Because finding the beam center is required to compute the direct beam in the first
     place, we do not include this term in the computation of :math:`I(Q)` for finding
     the beam center. This changes the shape of the :math:`I(Q)` curve, but since it
-    changes it in the same manner for all :math:`{\\phi}` angles, this does not affect the
-    results for finding the beam center.
+    changes it in the same manner for all :math:`{\\phi}` angles, this does not affect
+    the results for finding the beam center.
 
     This is what is now implemented in this version of the algorithm.
     """  # noqa: E501
     from scipy.optimize import minimize
 
     logger = get_logger('sans')
```

### Comparing `esssans-24.2.0/src/esssans/common.py` & `esssans-24.4.0/src/ess/sans/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import uuid
 from typing import Optional
 
 import numpy as np
 import scipp as sc
 from scipp.constants import g
 
-from .types import BackgroundRun, LoadedFileContents, SampleRun, TransmissionRun
-
 
 def gravity_vector() -> sc.Variable:
     """
     Return a vector of 3 components, defining the magnitude and direction of the Earth's
     gravitational field.
     """
     return sc.vector(value=[0, -1, 0]) * g
@@ -57,46 +55,39 @@
         )
     if (dim in da.coords) and (da.coords[dim].ndim > 1):
         raise sc.DimensionError(
             'Cannot mask range on data with multi-dimensional coordinate. '
             f'Found dimensions {da.coords[dim].dims} for coordinate {dim}.'
         )
 
+    coord = (
+        da.bins.constituents['data'].coords[dim]
+        if da.bins is not None
+        else da.coords[dim]
+    )
+    edges = edges.to(unit=coord.unit)
     lu = sc.DataArray(data=mask.data, coords={dim: edges})
     if da.bins is not None:
-        if dim in da.coords:
-            new_bins = sc.array(
-                dims=[dim],
-                values=np.union1d(edges.values, da.coords[dim].values),
-                unit=edges.unit,
+        if dim not in da.coords:
+            underlying = da.bins.coords[dim]
+            new_bins = np.union1d(
+                edges.values,
+                np.array(
+                    [
+                        underlying.min().value,
+                        np.nextafter(underlying.max().value, np.inf),
+                    ]
+                ),
             )
-            out = da.bin({dim: new_bins})
-            out.masks[name] = sc.lookup(lu, dim)[sc.midpoints(new_bins, dim=dim)]
         else:
-            out = da.bin({dim: edges})
-            out.masks[name] = mask.data
+            new_bins = np.union1d(edges.values, da.coords[dim].values)
+        new_bins = sc.array(dims=[dim], values=new_bins, unit=edges.unit)
+        out = da.bin({dim: new_bins})
+        out.masks[name] = sc.lookup(lu, dim)[sc.midpoints(new_bins, dim=dim)]
     else:
         out = da.copy(deep=False)
         mask_values = sc.lookup(lu, dim)[da.coords[dim]]
         if da.coords.is_edges(dim):
             out.masks[name] = mask_values[dim, 1:] | mask_values[dim, :-1]
         else:
             out.masks[name] = mask_values
     return out
-
-
-def transmission_from_sample_run(
-    data: LoadedFileContents[SampleRun],
-) -> LoadedFileContents[TransmissionRun[SampleRun]]:
-    """
-    Use transmission from a sample run, instead of dedicated run.
-    """
-    return LoadedFileContents[TransmissionRun[SampleRun]](data)
-
-
-def transmission_from_background_run(
-    data: LoadedFileContents[BackgroundRun],
-) -> LoadedFileContents[TransmissionRun[BackgroundRun]]:
-    """
-    Use transmission from a background run, instead of dedicated run.
-    """
-    return LoadedFileContents[TransmissionRun[BackgroundRun]](data)
```

### Comparing `esssans-24.2.0/src/esssans/conversions.py` & `esssans-24.4.0/src/ess/sans/conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     CleanWavelengthMasked,
     CorrectForGravity,
     IofQPart,
     MaskedData,
     MonitorType,
     Numerator,
     QxyBins,
-    RawMonitor,
     RunType,
+    ScatteringRunType,
+    TofMonitor,
     WavelengthMask,
     WavelengthMonitor,
 )
 
 
 def cyl_x_unit_vector(gravity: sc.Variable, incident_beam: sc.Variable) -> sc.Variable:
     """
@@ -125,17 +126,21 @@
 
 def Qxy(Q: sc.Variable, phi: sc.Variable) -> dict[str, sc.Variable]:
     """
     Compute the Qx and Qy components of the scattering vector from the scattering angle,
     wavelength, and phi angle.
     """
     Qx = sc.cos(phi)
-    Qx *= Q
     Qy = sc.sin(phi)
-    Qy *= Q
+    if Q.bins is not None and phi.bins is not None:
+        Qx *= Q
+        Qy *= Q
+    else:
+        Qx = Qx * Q
+        Qy = Qy * Q
     return {'Qx': Qx, 'Qy': Qy}
 
 
 ElasticCoordTransformGraph = NewType('ElasticCoordTransformGraph', dict)
 MonitorCoordTransformGraph = NewType('MonitorCoordTransformGraph', dict)
 
 
@@ -192,70 +197,64 @@
     """
     return MonitorCoordTransformGraph(
         {**beamline.beamline(scatter=False), **tof.elastic_wavelength('tof')}
     )
 
 
 def monitor_to_wavelength(
-    monitor: RawMonitor[RunType, MonitorType], graph: MonitorCoordTransformGraph
+    monitor: TofMonitor[RunType, MonitorType], graph: MonitorCoordTransformGraph
 ) -> WavelengthMonitor[RunType, MonitorType]:
     return WavelengthMonitor[RunType, MonitorType](
-        monitor.transform_coords('wavelength', graph=graph)
+        monitor.transform_coords('wavelength', graph=graph, keep_inputs=False)
     )
 
 
 def calibrate_positions(
-    detector: MaskedData[RunType], beam_center: BeamCenter
-) -> CalibratedMaskedData[RunType]:
+    detector: MaskedData[ScatteringRunType], beam_center: BeamCenter
+) -> CalibratedMaskedData[ScatteringRunType]:
     """
     Calibrate pixel positions.
 
     Currently the only applied calibration is the beam-center offset.
     """
     detector = detector.copy(deep=False)
     detector.coords['position'] = detector.coords['position'] - beam_center
     return detector
 
 
 # TODO This demonstrates a problem: Transforming to wavelength should be possible
 # for RawData, MaskedData, ... no reason to restrict necessarily.
 # Would we be fine with just choosing on option, or will this get in the way for users?
 def detector_to_wavelength(
-    detector: CalibratedMaskedData[RunType],
+    detector: CalibratedMaskedData[ScatteringRunType],
     graph: ElasticCoordTransformGraph,
-) -> CleanWavelength[RunType, Numerator]:
-    return CleanWavelength[RunType, Numerator](
-        detector.transform_coords('wavelength', graph=graph)
+) -> CleanWavelength[ScatteringRunType, Numerator]:
+    return CleanWavelength[ScatteringRunType, Numerator](
+        detector.transform_coords('wavelength', graph=graph, keep_inputs=False)
     )
 
 
 def mask_wavelength(
-    da: CleanWavelength[RunType, IofQPart], mask: Optional[WavelengthMask]
-) -> CleanWavelengthMasked[RunType, IofQPart]:
+    da: CleanWavelength[ScatteringRunType, IofQPart], mask: Optional[WavelengthMask]
+) -> CleanWavelengthMasked[ScatteringRunType, IofQPart]:
     if mask is not None:
-        # If we have binned data and the wavelength coord is multi-dimensional, we need
-        # to make a single wavelength bin before we can mask the range.
-        if da.bins is not None:
-            dim = mask.dim
-            if (dim in da.bins.coords) and (dim in da.coords):
-                da = da.bin({dim: 1})
         da = mask_range(da, mask=mask)
-    return CleanWavelengthMasked[RunType, IofQPart](da)
+    return CleanWavelengthMasked[ScatteringRunType, IofQPart](da)
 
 
 def compute_Q(
-    data: CleanWavelengthMasked[RunType, IofQPart],
+    data: CleanWavelengthMasked[ScatteringRunType, IofQPart],
     graph: ElasticCoordTransformGraph,
     compute_Qxy: Optional[QxyBins],
-) -> CleanQ[RunType, IofQPart]:
+) -> CleanQ[ScatteringRunType, IofQPart]:
     """
     Convert a data array from wavelength to Q.
     """
     # Keep naming of wavelength dim, subsequent steps use a (Q[xy], wavelength) binning.
-    return CleanQ[RunType, IofQPart](
+    return CleanQ[ScatteringRunType, IofQPart](
         data.transform_coords(
             ('Qx', 'Qy') if compute_Qxy else 'Q',
             graph=graph,
             keep_intermediate=False,
             rename_dims=False,
         )
     )
```

### Comparing `esssans-24.2.0/src/esssans/data.py` & `esssans-24.4.0/src/ess/sans/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,17 @@
             env=f'ESS_{instrument.upper()}_DATA_DIR',
             base_url=f'https://public.esss.dk/groups/scipp/ess/{instrument}/'
             + '{version}/',
             version=version,
             registry=files,
         )
 
+    def __contains__(self, key):
+        return key in self._registry.registry
+
     def get_path(self, name: str, unzip: bool = False) -> str:
         """
         Get the path to a file in the registry.
 
         Parameters
         ----------
         name:
```

### Comparing `esssans-24.2.0/src/esssans/direct_beam.py` & `esssans-24.4.0/src/ess/sans/direct_beam.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import scipp as sc
 from sciline import Pipeline
 
 from .i_of_q import resample_direct_beam
 from .types import (
     BackgroundRun,
     BackgroundSubtractedIofQ,
-    CleanSummedQ,
     Denominator,
+    FinalSummedQ,
     Numerator,
     ProcessedWavelengthBands,
     SampleRun,
     WavelengthBands,
     WavelengthBins,
 )
 
@@ -100,34 +100,34 @@
     band_dim = (set(bands.dims) - {'wavelength'}).pop()
     full_wavelength_range = sc.concat([bands.min(), bands.max()], dim='wavelength')
 
     pipeline = pipeline.copy()
 
     wavelength_bins = pipeline.compute(WavelengthBins)
     parts = (
-        CleanSummedQ[SampleRun, Numerator],
-        CleanSummedQ[SampleRun, Denominator],
-        CleanSummedQ[BackgroundRun, Numerator],
-        CleanSummedQ[BackgroundRun, Denominator],
+        FinalSummedQ[SampleRun, Numerator],
+        FinalSummedQ[SampleRun, Denominator],
+        FinalSummedQ[BackgroundRun, Numerator],
+        FinalSummedQ[BackgroundRun, Denominator],
     )
     parts = pipeline.compute(parts)
     # Convert events to histograms to make normalization (in every iteration) cheap
     for key in [
-        CleanSummedQ[SampleRun, Numerator],
-        CleanSummedQ[BackgroundRun, Numerator],
+        FinalSummedQ[SampleRun, Numerator],
+        FinalSummedQ[BackgroundRun, Numerator],
     ]:
         parts[key] = parts[key].hist(wavelength=wavelength_bins)
 
     # For now we simply strip all uncertainties, since direct beam function is
     # computed without variances anyway.
     parts = {key: sc.values(result) for key, result in parts.items()}
     for key, part in parts.items():
         pipeline[key] = part
-    sample0 = parts[CleanSummedQ[SampleRun, Denominator]]
-    background0 = parts[CleanSummedQ[BackgroundRun, Denominator]]
+    sample0 = parts[FinalSummedQ[SampleRun, Denominator]]
+    background0 = parts[FinalSummedQ[BackgroundRun, Denominator]]
 
     results = []
 
     for _it in range(niter):
         # The first time we compute I(Q), the direct beam function is not in the
         # parameters, nor given by any providers, so it will be considered flat.
         # TODO: Should we have a check that DirectBeam cannot be computed from the
@@ -154,16 +154,19 @@
 
         # Scale denominator terms that were initially computed without direct beam
         # with the current direct beam function.
         db = resample_direct_beam(
             direct_beam=direct_beam_function,
             wavelength_bins=wavelength_bins,
         )
-        pipeline[CleanSummedQ[SampleRun, Denominator]] = sample0 * db
-        pipeline[CleanSummedQ[BackgroundRun, Denominator]] = background0 * db
+        db.coords['wavelength'] = sc.midpoints(
+            db.coords['wavelength'], dim='wavelength'
+        )
+        pipeline[FinalSummedQ[SampleRun, Denominator]] = sample0 * db
+        pipeline[FinalSummedQ[BackgroundRun, Denominator]] = background0 * db
 
         results.append(
             {
                 'iofq_full': iofq_full,
                 'iofq_bands': iofq_bands,
                 'direct_beam': direct_beam_function,
             }
```

### Comparing `esssans-24.2.0/src/esssans/i_of_q.py` & `esssans-24.4.0/src/ess/sans/i_of_q.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from typing import Optional
 
+import sciline
 import scipp as sc
 from scipp.scipy.interpolate import interp1d
 
 from .common import mask_range
 from .logging import get_logger
 from .types import (
     BackgroundRun,
     BackgroundSubtractedIofQ,
     CleanDirectBeam,
     CleanMonitor,
     CleanQ,
     CleanSummedQ,
+    CleanSummedQMergedBanks,
     DimsToKeep,
     DirectBeam,
+    Filename,
+    FinalSummedQ,
     IofQ,
     IofQPart,
     MonitorType,
+    NeXusDetectorName,
     NonBackgroundWavelengthRange,
     QBins,
     QxyBins,
     ReturnEvents,
     RunType,
     SampleRun,
+    ScatteringRunType,
     UncertaintyBroadcastMode,
     WavelengthBins,
     WavelengthMonitor,
 )
 from .uncertainty import broadcast_with_upper_bound_variances
 
 
@@ -127,22 +133,22 @@
         'wavelength',
         fill_value="extrapolate",
         bounds_error=False,
     )
     return CleanDirectBeam(func(wavelength_bins, midpoints=True))
 
 
-def merge_spectra(
-    data: CleanQ[RunType, IofQPart],
+def bin_in_q(
+    data: CleanQ[ScatteringRunType, IofQPart],
     q_bins: Optional[QBins],
     qxy_bins: Optional[QxyBins],
     dims_to_keep: Optional[DimsToKeep],
-) -> CleanSummedQ[RunType, IofQPart]:
+) -> CleanSummedQ[ScatteringRunType, IofQPart]:
     """
-    Merges all spectra:
+    Merges data from all pixels into a single I(Q) spectrum:
 
     * In the case of event data, events in all bins are concatenated
     * In the case of dense data, counts in all spectra are summed
 
     Parameters
     ----------
     data:
@@ -166,15 +172,22 @@
         # We make Qx the inner dim, such that plots naturally show Qx on the x-axis.
         edges = {'Qy': qxy_bins['Qy'], 'Qx': qxy_bins['Qx']}
     else:
         edges = {'Q': q_bins}
 
     if data.bins is not None:
         q_all_pixels = data.bins.concat(dims_to_reduce)
-        out = q_all_pixels.bin(**edges)
+        # q_all_pixels may just have a single bin now, which currently yields
+        # inferior performance when binning (no/bad multi-threading?).
+        # We operate on the content buffer for better multi-threaded performance.
+        if q_all_pixels.ndim == 0:
+            content = q_all_pixels.bins.constituents['data']
+            out = content.bin(**edges).assign_coords(q_all_pixels.coords)
+        else:
+            out = q_all_pixels.bin(**edges)
     else:
         # We want to flatten data to make histogramming cheaper (avoiding allocation of
         # large output before summing). We strip unnecessary content since it makes
         # flattening more expensive.
         stripped = data.copy(deep=False)
         for name, coord in data.coords.items():
             if (
@@ -204,17 +217,64 @@
                 if dim == helper_dim:
                     continue
                 if dim not in flat.coords:
                     flat.coords[dim] = sc.arange(dim, flat.sizes[dim])
             out = (
                 flat.flatten(to=str(uuid.uuid4()))
                 .group(*[flat.coords[dim] for dim in flat.dims if dim != helper_dim])
+                .drop_coords(dims_to_keep or ())
                 .hist(**edges)
             )
-    return CleanSummedQ[RunType, IofQPart](out.squeeze())
+    return CleanSummedQ[ScatteringRunType, IofQPart](out.squeeze())
+
+
+def no_bank_merge(
+    data: CleanSummedQ[ScatteringRunType, IofQPart]
+) -> CleanSummedQMergedBanks[ScatteringRunType, IofQPart]:
+    return CleanSummedQMergedBanks[ScatteringRunType, IofQPart](data)
+
+
+def no_run_merge(
+    data: CleanSummedQMergedBanks[ScatteringRunType, IofQPart]
+) -> FinalSummedQ[ScatteringRunType, IofQPart]:
+    return FinalSummedQ[ScatteringRunType, IofQPart](data)
+
+
+def _merge_contributions(data: list[sc.DataArray]) -> sc.DataArray:
+    if len(data) == 1:
+        return data[0]
+    reducer = sc.reduce(data)
+    return reducer.bins.concat() if data[0].bins is not None else reducer.sum()
+
+
+def merge_banks(
+    banks: sciline.Series[NeXusDetectorName, CleanSummedQ[ScatteringRunType, IofQPart]]
+) -> CleanSummedQMergedBanks[ScatteringRunType, IofQPart]:
+    """
+    Merge the events or counts from multiple detector banks into a single numerator or
+    denominator, before the normalization step.
+    """
+    return CleanSummedQMergedBanks[ScatteringRunType, IofQPart](
+        _merge_contributions(list(banks.values()))
+    )
+
+
+def merge_runs(
+    runs: sciline.Series[
+        Filename[ScatteringRunType],
+        CleanSummedQMergedBanks[ScatteringRunType, IofQPart],
+    ],
+) -> FinalSummedQ[ScatteringRunType, IofQPart]:
+    """
+    Merge the events or counts from multiple runs into a single numerator or
+    denominator, before the normalization step.
+    """
+    return FinalSummedQ[ScatteringRunType, IofQPart](
+        _merge_contributions(list(runs.values()))
+    )
 
 
 def subtract_background(
     sample: IofQ[SampleRun],
     background: IofQ[BackgroundRun],
     return_events: ReturnEvents,
 ) -> BackgroundSubtractedIofQ:
@@ -226,10 +286,12 @@
         background = background.bins.sum()
     return BackgroundSubtractedIofQ(sample - background)
 
 
 providers = (
     preprocess_monitor_data,
     resample_direct_beam,
-    merge_spectra,
+    bin_in_q,
     subtract_background,
+    no_bank_merge,
+    no_run_merge,
 )
```

### Comparing `esssans-24.2.0/src/esssans/io.py` & `esssans-24.4.0/src/ess/sans/io.py`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/src/esssans/isis/io.py` & `esssans-24.4.0/src/ess/isissans/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 """
 File loading functions for ISIS data, NOT using Mantid.
 """
-from typing import NewType, TypeVar
+from typing import NewType
 
-import sciline
 import scipp as sc
 
-from ..types import RunType
+from ..sans.types import (
+    DataFolder,
+    FilenameType,
+    FilePath,
+    MaskedDetectorIDs,
+    PixelMaskFilename,
+)
 
-PixelMaskFilename = NewType('PixelMaskFilename', str)
 CalibrationFilename = NewType('CalibrationFilename', str)
 
-FilenameType = TypeVar('FilenameType', bound=str)
-
-
-DataFolder = NewType('DataFolder', str)
-
-
-class FilePath(sciline.Scope[FilenameType, str], str):
-    """Path to a file"""
-
-
-class Filename(sciline.Scope[RunType, str], str):
-    """Filename of a run"""
-
-
-MaskedDetectorIDs = NewType('MaskedDetectorIDs', sc.Variable)
-"""1-D variable listing all masked detector IDs."""
-
 
 def to_path(filename: FilenameType, path: DataFolder) -> FilePath[FilenameType]:
     return f'{path}/{filename}'
 
 
 def read_xml_detector_masking(
     filename: FilePath[PixelMaskFilename],
```

### Comparing `esssans-24.2.0/src/esssans/isis/mantidio.py` & `esssans-24.4.0/src/ess/isissans/mantidio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 """
 File loading functions for ISIS data using Mantid.
 """
-from typing import NewType, NoReturn
+from typing import NewType, NoReturn, Optional
 
 import sciline
 import scipp as sc
 import scippneutron as scn
 from scipp.constants import g
 
-from ..types import (
-    DirectBeam,
-    DirectBeamFilename,
-    LoadedFileContents,
-    RunType,
-    SampleRun,
-)
-from .io import CalibrationFilename, Filename, FilePath
+from ..sans.types import DirectBeam, DirectBeamFilename, Filename, RunType, SampleRun
+from .data import LoadedFileContents
+from .io import CalibrationFilename, FilePath
 
 try:
     import mantid.api as _mantid_api
     import mantid.simpleapi as _mantid_simpleapi
     from mantid.api import MatrixWorkspace
 except ModuleNotFoundError:
     # Catch runtime usages of Mantid
     class _MantidFallback:
         def __getattr__(self, name: str) -> NoReturn:
             raise ImportError(
-                'Mantid is required to use `sans.isis.mantidio` ' 'but is not installed'
+                'Mantid is required to use `sans.isis.mantidio` but is not installed'
             ) from None
 
     _mantid_api = _MantidFallback()
     _mantid_simpleapi = _MantidFallback
     # Needed for type annotations
     MatrixWorkspace = object
 
@@ -45,15 +40,15 @@
 
 
 def _make_detector_info(ws: MatrixWorkspace) -> sc.DataGroup:
     det_info = scn.mantid.make_detector_info(ws, 'spectrum')
     return sc.DataGroup(det_info.coords)
 
 
-def get_detector_ids(ws: DataWorkspace[SampleRun]) -> sc.Variable:
+def _get_detector_ids(ws: DataWorkspace[SampleRun]) -> sc.Variable:
     det_info = _make_detector_info(ws)
     dim = 'spectrum'
     da = sc.DataArray(det_info['detector'], coords={dim: det_info[dim]})
     da = sc.sort(da, dim)  # sort by spectrum index
     if not sc.identical(
         da.coords[dim],
         sc.arange('detector', da.sizes['detector'], dtype='int32', unit=None),
@@ -76,23 +71,31 @@
     da = dg['data']
     del da.coords['spectrum']
     return DirectBeam(da)
 
 
 def from_data_workspace(
     ws: DataWorkspace[RunType],
-    calibration: CalibrationWorkspace,
+    calibration: Optional[CalibrationWorkspace],
 ) -> LoadedFileContents[RunType]:
-    _mantid_simpleapi.CopyInstrumentParameters(
-        InputWorkspace=calibration, OutputWorkspace=ws, StoreInADS=False
-    )
+    if calibration is not None:
+        _mantid_simpleapi.CopyInstrumentParameters(
+            InputWorkspace=calibration, OutputWorkspace=ws, StoreInADS=False
+        )
     up = ws.getInstrument().getReferenceFrame().vecPointingUp()
     dg = scn.from_mantid(ws)
+    det_ids = _get_detector_ids(ws)
+    # In some instruments (e.g. SANS2D), some pixels are used for other purposes (e.g.
+    # live acquisition). They have no detector ids, so we exclude them from the data.
+    for dim, shape in det_ids.sizes.items():
+        dg['data'] = dg['data'][dim, :shape]
     dg['data'] = dg['data'].squeeze()
-    dg['data'].coords['detector_id'] = get_detector_ids(ws)
+    if (dg['data'].bins is not None) and ('tof' in dg['data'].coords):
+        del dg['data'].coords['tof']
+    dg['data'].coords['detector_id'] = det_ids
     dg['data'].coords['gravity'] = sc.vector(value=-up) * g
     return LoadedFileContents[RunType](dg)
 
 
 def load_run(filename: FilePath[Filename[RunType]]) -> DataWorkspace[RunType]:
     loaded = _mantid_simpleapi.Load(
         Filename=str(filename), LoadMonitors=True, StoreInADS=False
```

### Comparing `esssans-24.2.0/src/esssans/isis/masking.py` & `esssans-24.4.0/src/ess/sans/masking.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,47 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
-from typing import NewType
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+"""
+Masking functions for the loki workflow.
+"""
+from typing import Optional
 
 import numpy as np
 import sciline
 import scipp as sc
 
-from ..types import MaskedData, RawData, RunType, SampleRun
-from .components import RawDataWithComponentUserOffsets
-from .io import MaskedDetectorIDs
-
-PixelMask = NewType('PixelMask', sc.Variable)
-
-
-def to_pixel_mask(data: RawData[SampleRun], masked: MaskedDetectorIDs) -> PixelMask:
-    """Convert a list of masked detector IDs to a pixel mask.
-
-    Parameters
-    ----------
-    data:
-        Raw data, defining the detector IDs.
-    masked:
-        The masked detector IDs.
-    """
-    ids = data.coords['detector_id']
-    mask = sc.zeros(sizes=ids.sizes, dtype='bool')
-    mask.values[np.isin(ids.values, masked.values)] = True
-    return PixelMask(mask)
+from .types import (
+    MaskedData,
+    MaskedDetectorIDs,
+    PixelMaskFilename,
+    ScatteringRunType,
+    TofData,
+)
 
 
 def apply_pixel_masks(
-    data: RawDataWithComponentUserOffsets[RunType],
-    masks: sciline.Series[str, PixelMask],
-) -> MaskedData[RunType]:
+    data: TofData[ScatteringRunType],
+    masked_ids: Optional[sciline.Series[PixelMaskFilename, MaskedDetectorIDs]],
+) -> MaskedData[ScatteringRunType]:
     """Apply pixel-specific masks to raw data.
-
-    This depends on the configured raw data (which has been configured with component
-    positions) since in principle we might apply pixel masks based on the component
-    positions. Currently the only masks are based on detector IDs.
+    The masks are based on detector IDs stored in XML files.
 
     Parameters
     ----------
     data:
         Raw data with configured component positions.
     masks:
         A series of masks.
     """
-    data = data.copy(deep=False)
-    for name, mask in masks.items():
-        data.masks[name] = mask
-    return MaskedData[RunType](data)
+    if masked_ids is not None:
+        data = data.copy(deep=False)
+        ids = data.coords[
+            'detector_number' if 'detector_number' in data.coords else 'detector_id'
+        ]
+        for name, masked in masked_ids.items():
+            mask = sc.zeros(sizes=ids.sizes, dtype='bool')
+            mask.values[np.isin(ids.values, masked.values)] = True
+            data.masks[name] = mask
+    return MaskedData[ScatteringRunType](data)
 
 
-providers = (
-    to_pixel_mask,
-    apply_pixel_masks,
-)
+providers = (apply_pixel_masks,)
```

### Comparing `esssans-24.2.0/src/esssans/isis/visualization.py` & `esssans-24.4.0/src/ess/isissans/visualization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 """
 Plotting functions for ISIS data.
 """
+import warnings
 from typing import Any
 
 import scipp as sc
 
 
 def plot_flat_detector_xy(
     da: sc.DataArray, pixels_per_tube: int = 512, **kwargs: Any
@@ -41,8 +42,11 @@
     else:
         raise ValueError(
             'Cannot plot 2-D instrument view of data array with non-constant '
             'y coordinate along tubes. Use scippneutron.instrument_view instead.'
         )
     plot_kwargs = dict(aspect='equal')
     plot_kwargs.update(kwargs)
-    return folded.plot(**plot_kwargs)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=RuntimeWarning)
+        out = folded.plot(**plot_kwargs)
+    return out
```

### Comparing `esssans-24.2.0/src/esssans/logging.py` & `esssans-24.4.0/src/ess/sans/logging.py`

 * *Files identical despite different names*

### Comparing `esssans-24.2.0/src/esssans/loki/data.py` & `esssans-24.4.0/src/ess/loki/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 
-from ..data import Registry
+from ..sans.data import Registry
+from ..sans.types import FilenameType, FilePath
 
 _registry = Registry(
     instrument='loki',
     files={
         # Files from LoKI@Larmor detector test experiment
         #
         # Background run 1 (no sample, sample holder/can only, no transmission monitor)
@@ -19,15 +20,20 @@
         '60392-2022-02-28_2215.nxs': 'md5:9ecc1a9a2c05a880144afb299fc11042',
         # Background run 2 (no sample, sample holder/can only, no transmission monitor)
         '60393-2022-02-28_2215.nxs': 'md5:bf550d0ba29931f11b7450144f658652',
         # Sample transmission run (sample + sample holder/can + transmission monitor)
         '60394-2022-02-28_2215.nxs': 'md5:c40f38a62337d86957af925296c4c615',
         # Analytical model for the I(Q) of the Poly-Gauss sample
         'PolyGauss_I0-50_Rg-60.h5': 'md5:f5d60d9c2286cb197b8cd4dc82db3d7e',
+        # XML file for the pixel mask
+        'mask_new_July2022.xml': 'md5:421b6dc9db74126ffbc5d88164d017b0',
     },
     version='2',
 )
 
 
-get_path = _registry.get_path
+def get_path(filename: FilenameType) -> FilePath[FilenameType]:
+    """Translate any filename to a path to the file obtained from pooch registries."""
+    return FilePath[FilenameType](_registry.get_path(filename))
 
-__all__ = ['get_path']
+
+providers = (get_path,)
```

### Comparing `esssans-24.2.0/src/esssans/normalization.py` & `esssans-24.4.0/src/ess/sans/normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 import scipp as sc
 from scipp.core import concepts
 
 from .types import (
     CalibratedMaskedData,
     CleanDirectBeam,
     CleanMonitor,
-    CleanSummedQ,
     CleanWavelength,
     Denominator,
     DetectorPixelShape,
     EmptyBeamRun,
+    FinalSummedQ,
     Incident,
     IofQ,
     LabFrameTransform,
     NormWavelengthTerm,
     Numerator,
     ProcessedWavelengthBands,
     ReturnEvents,
-    RunType,
+    ScatteringRunType,
     SolidAngle,
     Transmission,
     TransmissionFraction,
     TransmissionRun,
     UncertaintyBroadcastMode,
     WavelengthBands,
     WavelengthBins,
@@ -35,18 +35,18 @@
     broadcast_to_events_with_upper_bound_variances,
     broadcast_with_upper_bound_variances,
     drop_variances_if_broadcast,
 )
 
 
 def solid_angle(
-    data: CalibratedMaskedData[RunType],
-    pixel_shape: DetectorPixelShape[RunType],
-    transform: LabFrameTransform[RunType],
-) -> SolidAngle[RunType]:
+    data: CalibratedMaskedData[ScatteringRunType],
+    pixel_shape: DetectorPixelShape[ScatteringRunType],
+    transform: LabFrameTransform[ScatteringRunType],
+) -> SolidAngle[ScatteringRunType]:
     """
     Solid angle for cylindrical pixels.
 
     Note that the approximation is valid when the distance from sample
     to pixel is much larger than the length or the radius of the pixels.
 
     Parameters
@@ -76,15 +76,15 @@
 
     omega = _approximate_solid_angle_for_cylinder_shaped_pixel_of_detector(
         pixel_position=data.coords['position'] - data.coords['sample_position'],
         cylinder_axis=cylinder_axis,
         radius=radius,
         length=length,
     )
-    return SolidAngle[RunType](
+    return SolidAngle[ScatteringRunType](
         concepts.rewrap_reduced_data(
             prototype=data, data=omega, dim=set(data.dims) - set(omega.dims)
         )
     )
 
 
 def _approximate_solid_angle_for_cylinder_shaped_pixel_of_detector(
@@ -123,19 +123,21 @@
     cosalpha = sc.sqrt(
         1 - (sc.dot(pixel_position, cylinder_axis) / (norm_pp * norm_ca)) ** 2
     )
     return (2 * radius * length) * cosalpha / norm_pp**2
 
 
 def transmission_fraction(
-    sample_incident_monitor: CleanMonitor[TransmissionRun[RunType], Incident],
-    sample_transmission_monitor: CleanMonitor[TransmissionRun[RunType], Transmission],
+    sample_incident_monitor: CleanMonitor[TransmissionRun[ScatteringRunType], Incident],
+    sample_transmission_monitor: CleanMonitor[
+        TransmissionRun[ScatteringRunType], Transmission
+    ],
     direct_incident_monitor: CleanMonitor[EmptyBeamRun, Incident],
     direct_transmission_monitor: CleanMonitor[EmptyBeamRun, Transmission],
-) -> TransmissionFraction[RunType]:
+) -> TransmissionFraction[ScatteringRunType]:
     """
     Approximation based on equations in
     `CalculateTransmission <https://docs.mantidproject.org/v4.0.0/algorithms/CalculateTransmission-v1.html>`_
     documentation:
     ``(sample_transmission_monitor / direct_transmission_monitor) * (direct_incident_monitor / sample_incident_monitor)``
 
     This is equivalent to ``mantid.CalculateTransmission`` without fitting.
@@ -156,30 +158,30 @@
     -------
     :
         The transmission fraction computed from the monitor counts.
     """  # noqa: E501
     frac = (sample_transmission_monitor / direct_transmission_monitor) * (
         direct_incident_monitor / sample_incident_monitor
     )
-    return TransmissionFraction[RunType](frac)
+    return TransmissionFraction[ScatteringRunType](frac)
 
 
 _broadcasters = {
     UncertaintyBroadcastMode.drop: drop_variances_if_broadcast,
     UncertaintyBroadcastMode.upper_bound: broadcast_with_upper_bound_variances,
     UncertaintyBroadcastMode.fail: lambda x, sizes: x,
 }
 
 
 def iofq_norm_wavelength_term(
-    incident_monitor: CleanMonitor[RunType, Incident],
-    transmission_fraction: TransmissionFraction[RunType],
+    incident_monitor: CleanMonitor[ScatteringRunType, Incident],
+    transmission_fraction: TransmissionFraction[ScatteringRunType],
     direct_beam: Optional[CleanDirectBeam],
     uncertainties: UncertaintyBroadcastMode,
-) -> NormWavelengthTerm[RunType]:
+) -> NormWavelengthTerm[ScatteringRunType]:
     """
     Compute the wavelength-dependent contribution to the denominator term for the I(Q)
     normalization.
     Keeping this as a separate function allows us to compute it once during the
     iterations for finding the beam center, while the solid angle is recomputed
     for each iteration.
 
@@ -220,22 +222,22 @@
         dims.remove('wavelength')
         dims.append('wavelength')
         direct_beam = direct_beam.transpose(dims)
         broadcast = _broadcasters[uncertainties]
         out = direct_beam * broadcast(out, sizes=direct_beam.sizes)
     # Convert wavelength coordinate to midpoints for future histogramming
     out.coords['wavelength'] = sc.midpoints(out.coords['wavelength'])
-    return NormWavelengthTerm[RunType](out)
+    return NormWavelengthTerm[ScatteringRunType](out)
 
 
 def iofq_denominator(
-    wavelength_term: NormWavelengthTerm[RunType],
-    solid_angle: SolidAngle[RunType],
+    wavelength_term: NormWavelengthTerm[ScatteringRunType],
+    solid_angle: SolidAngle[ScatteringRunType],
     uncertainties: UncertaintyBroadcastMode,
-) -> CleanWavelength[RunType, Denominator]:
+) -> CleanWavelength[ScatteringRunType, Denominator]:
     """
     Compute the denominator term for the I(Q) normalization.
 
     In a SANS experiment, the scattering cross section :math:`I(Q)` is defined as
     (`Heenan et al. 1997 <https://doi.org/10.1107/S0021889897002173>`_):
 
     .. math::
@@ -293,15 +295,15 @@
     Returns
     -------
     :
         The denominator for the SANS I(Q) normalization.
     """  # noqa: E501
     broadcast = _broadcasters[uncertainties]
     denominator = solid_angle * broadcast(wavelength_term, sizes=solid_angle.sizes)
-    return CleanWavelength[RunType, Denominator](denominator)
+    return CleanWavelength[ScatteringRunType, Denominator](denominator)
 
 
 def process_wavelength_bands(
     wavelength_bands: Optional[WavelengthBands],
     wavelength_bins: WavelengthBins,
 ) -> ProcessedWavelengthBands:
     """
@@ -333,20 +335,20 @@
             'defining a start and an end wavelength, '
             f'got {wavelength_bands.sizes["wavelength"]}.'
         )
     return wavelength_bands
 
 
 def normalize(
-    numerator: CleanSummedQ[RunType, Numerator],
-    denominator: CleanSummedQ[RunType, Denominator],
+    numerator: FinalSummedQ[ScatteringRunType, Numerator],
+    denominator: FinalSummedQ[ScatteringRunType, Denominator],
     return_events: ReturnEvents,
     uncertainties: UncertaintyBroadcastMode,
     wavelength_bands: ProcessedWavelengthBands,
-) -> IofQ[RunType]:
+) -> IofQ[ScatteringRunType]:
     """
     Perform normalization of counts as a function of Q.
     If the numerator contains events, we use the sc.lookup function to perform the
     division.
 
     Parameters
     ----------
@@ -373,14 +375,16 @@
     wavelength_bounds = sc.sort(wavelength_bands.flatten(to=wav), wav)
     if numerator.bins is not None:
         # If in event mode the desired wavelength binning has not been applied, we need
         # it for splitting by bands, or restricting the range in case of a single band.
         numerator = numerator.bin(wavelength=wavelength_bounds)
 
     def _reduce(da: sc.DataArray) -> sc.DataArray:
+        if da.sizes[wav] == 1:  # Can avoid costly event-data da.bins.concat
+            return da.squeeze(wav)
         return da.sum(wav) if da.bins is None else da.bins.concat(wav)
 
     num_parts = []
     denom_parts = []
     for wav_range in sc.collapse(wavelength_bands, keep=wav).values():
         num_parts.append(_reduce(numerator[wav, wav_range[0] : wav_range[1]]))
         denom_parts.append(_reduce(denominator[wav, wav_range[0] : wav_range[1]]))
@@ -402,15 +406,18 @@
                 denominator = sc.values(denominator)
             else:
                 denominator = broadcast_to_events_with_upper_bound_variances(
                     denominator, events=numerator
                 )
     elif numerator.bins is not None:
         numerator = numerator.hist()
-    return IofQ[RunType](numerator / denominator)
+    numerator /= denominator.drop_coords(
+        [name for name in denominator.coords if name not in denominator.dims]
+    )
+    return IofQ[ScatteringRunType](numerator)
 
 
 providers = (
     transmission_fraction,
     iofq_norm_wavelength_term,
     iofq_denominator,
     normalize,
```

### Comparing `esssans-24.2.0/src/esssans/sans2d/general.py` & `esssans-24.4.0/src/ess/isissans/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """
-Loading and masking specific to the ISIS Sans2d instrument and files stored in Scipp's
-HDF5 format.
+Providers for the ISIS instruments.
 """
 import scipp as sc
 
-from ..types import (
+from ..sans.types import (
+    ConfiguredReducibleDataData,
+    ConfiguredReducibleMonitor,
     DetectorPixelShape,
-    Incident,
     LabFrameTransform,
-    LoadedFileContents,
     MonitorType,
     NeXusMonitorName,
     RawData,
     RawMonitor,
     RunNumber,
     RunTitle,
     RunType,
     SampleRun,
-    Transmission,
+    ScatteringRunType,
+    TofData,
+    TofMonitor,
 )
-
-default_parameters = {
-    NeXusMonitorName[Incident]: 'monitor2',
-    NeXusMonitorName[Transmission]: 'monitor4',
-}
+from .data import LoadedFileContents
 
 
 def get_detector_data(
     dg: LoadedFileContents[RunType],
 ) -> RawData[RunType]:
     return RawData[RunType](dg['data'])
 
 
-def get_monitor(
+def get_monitor_data(
     dg: LoadedFileContents[RunType], nexus_name: NeXusMonitorName[MonitorType]
 ) -> RawMonitor[RunType, MonitorType]:
     # See https://github.com/scipp/sciline/issues/52 why copy needed
     mon = dg['monitors'][nexus_name]['data'].copy()
     return RawMonitor[RunType, MonitorType](mon)
 
 
+def data_to_tof(
+    da: ConfiguredReducibleDataData[ScatteringRunType],
+) -> TofData[ScatteringRunType]:
+    """Dummy conversion of data to time-of-flight data.
+    The data already has a time-of-flight coordinate."""
+    return TofData[ScatteringRunType](da)
+
+
+def monitor_to_tof(
+    da: ConfiguredReducibleMonitor[RunType, MonitorType]
+) -> TofMonitor[RunType, MonitorType]:
+    """Dummy conversion of monitor data to time-of-flight data.
+    The monitor data already has a time-of-flight coordinate."""
+    return TofMonitor[RunType, MonitorType](da)
+
+
 def run_number(dg: LoadedFileContents[SampleRun]) -> RunNumber:
     """Get the run number from the raw sample data."""
     return RunNumber(int(dg['run_number']))
 
 
 def run_title(dg: LoadedFileContents[SampleRun]) -> RunTitle:
     """Get the run title from the raw sample data."""
     return RunTitle(dg['run_title'].value)
 
 
-def sans2d_tube_detector_pixel_shape() -> DetectorPixelShape[RunType]:
+def helium3_tube_detector_pixel_shape() -> DetectorPixelShape[ScatteringRunType]:
     # Pixel radius and length
     # found here:
     # https://github.com/mantidproject/mantid/blob/main/instrument/SANS2D_Definition_Tubes.xml
     R = 0.00405
     L = 0.002033984375
     pixel_shape = sc.DataGroup(
         {
@@ -75,20 +88,22 @@
             ),
             'nexus_class': 'NXcylindrical_geometry',
         }
     )
     return pixel_shape
 
 
-def lab_frame_transform() -> LabFrameTransform[RunType]:
+def lab_frame_transform() -> LabFrameTransform[ScatteringRunType]:
     # Rotate +y to -x
     return sc.spatial.rotation(value=[0, 0, 1 / 2**0.5, 1 / 2**0.5])
 
 
 providers = (
     get_detector_data,
-    get_monitor,
+    get_monitor_data,
+    data_to_tof,
+    monitor_to_tof,
     run_number,
     run_title,
     lab_frame_transform,
-    sans2d_tube_detector_pixel_shape,
+    helium3_tube_detector_pixel_shape,
 )
```

### Comparing `esssans-24.2.0/src/esssans/sans2d/masking.py` & `esssans-24.4.0/src/ess/isissans/sans2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-"""
-"""
+# Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 from typing import NewType, Optional
 
 import scipp as sc
 
-from ..types import MaskedData, RawData, RunType, SampleRun
+from ..sans.types import MaskedData, SampleRun, ScatteringRunType, TofData
 
 DetectorEdgeMask = NewType('DetectorEdgeMask', sc.Variable)
 """Detector edge mask"""
 
 LowCountThreshold = NewType('LowCountThreshold', sc.Variable)
 """Threshold below which detector pixels should be masked
 (low-counts on the edges of the detector panel, and the beam stop)"""
 
 SampleHolderMask = NewType('SampleHolderMask', sc.Variable)
 """Sample holder mask"""
 
 
-def detector_edge_mask(sample: RawData[SampleRun]) -> DetectorEdgeMask:
+def detector_edge_mask(
+    sample: TofData[SampleRun],
+) -> DetectorEdgeMask:
     mask_edges = (
         sc.abs(sample.coords['position'].fields.x) > sc.scalar(0.48, unit='m')
     ) | (sc.abs(sample.coords['position'].fields.y) > sc.scalar(0.45, unit='m'))
     return DetectorEdgeMask(mask_edges)
 
 
 def sample_holder_mask(
-    sample: RawData[SampleRun],
+    sample: TofData[SampleRun],
     low_counts_threshold: LowCountThreshold,
 ) -> SampleHolderMask:
-    summed = sample.sum('tof')
+    summed = sample.hist()
     holder_mask = (
         (summed.data < low_counts_threshold)
         & (sample.coords['position'].fields.x > sc.scalar(0, unit='m'))
         & (sample.coords['position'].fields.x < sc.scalar(0.42, unit='m'))
         & (sample.coords['position'].fields.y < sc.scalar(0.05, unit='m'))
         & (sample.coords['position'].fields.y > sc.scalar(-0.15, unit='m'))
     )
     return SampleHolderMask(holder_mask)
 
 
 def mask_detectors(
-    da: RawData[RunType],
+    da: TofData[ScatteringRunType],
     edge_mask: Optional[DetectorEdgeMask],
     holder_mask: Optional[SampleHolderMask],
-) -> MaskedData[RunType]:
+) -> MaskedData[ScatteringRunType]:
     """Apply pixel-specific masks to raw data.
 
     Parameters
     ----------
     da:
         Raw data.
     edge_mask:
@@ -58,11 +58,11 @@
         Mask for sample holder.
     """
     da = da.copy(deep=False)
     if edge_mask is not None:
         da.masks['edges'] = edge_mask
     if holder_mask is not None:
         da.masks['holder_mask'] = holder_mask
-    return MaskedData[RunType](da)
+    return MaskedData[ScatteringRunType](da)
 
 
 providers = (detector_edge_mask, sample_holder_mask, mask_detectors)
```

### Comparing `esssans-24.2.0/src/esssans/types.py` & `esssans-24.4.0/src/ess/sans/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,29 +20,38 @@
 EmptyBeamRun = NewType('EmptyBeamRun', int)
 """Run (sometimes called 'direct run') where the sample holder was empty.
 It is used for reading the data from the transmission monitor."""
 SampleRun = NewType('SampleRun', int)
 """Sample run: the run with the sample placed in the solvent inside the sample holder.
 """
 
-RunType = TypeVar(
-    'RunType',
-    BackgroundRun,
-    EmptyBeamRun,
+ScatteringRunType = TypeVar(
+    'ScatteringRunType',
     SampleRun,
+    BackgroundRun,
 )
-"""TypeVar used for specifying BackgroundRun, EmptyBeamRun or SampleRun"""
 
 
-class TransmissionRun(sciline.Scope[RunType, int], int):
-    """Mapping between RunType and transmission run.
+class TransmissionRun(sciline.Scope[ScatteringRunType, int], int):
+    """Mapping between ScatteringRunType and transmission run.
     In the case where no transmission run is provided, the transmission run should be
     the same as the measurement (sample or background) run."""
 
 
+RunType = TypeVar(
+    'RunType',
+    BackgroundRun,
+    EmptyBeamRun,
+    SampleRun,
+    # Note that mypy does not seem to like this nesting, may need to find a workaround
+    TransmissionRun[SampleRun],
+    TransmissionRun[BackgroundRun],
+)
+"""TypeVar used for specifying BackgroundRun, EmptyBeamRun or SampleRun"""
+
 # 1.2  Monitor types
 Incident = NewType('Incident', int)
 """Incident monitor"""
 Transmission = NewType('Transmission', int)
 """Transmission monitor"""
 MonitorType = TypeVar('MonitorType', Incident, Transmission)
 """TypeVar used for specifying Incident or Transmission monitor type"""
@@ -52,27 +61,26 @@
 """Numerator of IofQ"""
 Denominator = NewType('Denominator', sc.DataArray)
 """Denominator of IofQ"""
 IofQPart = TypeVar('IofQPart', Numerator, Denominator)
 """TypeVar used for specifying Numerator or Denominator of IofQ"""
 
 # 1.4  Entry paths in NeXus files
-NeXusSampleName = NewType('NeXusSampleName', str)
-"""Name of sample entry in NeXus file"""
-
-NeXusSourceName = NewType('NeXusSourceName', str)
-"""Name of source entry in NeXus file"""
-
 NeXusDetectorName = NewType('NeXusDetectorName', str)
 """Name of detector entry in NeXus file"""
 
+PixelShapePath = NewType('PixelShapePath', str)
+"""
+Name of the entry where the pixel shape is stored in the NeXus file
+"""
+
 TransformationPath = NewType('TransformationPath', str)
 """
-Name of the entry under which to store the transformation computed from the
-transformation chain, for the detectors and the monitors
+Name of the entry where the transformation computed from the
+transformation chain is stored, for the detectors and the monitors
 """
 
 # 2  Workflow parameters
 
 UncertaintyBroadcastMode = Enum(
     'UncertaintyBroadcastMode', ['drop', 'upper_bound', 'fail']
 )
@@ -140,122 +148,195 @@
 """Filename of the output"""
 
 
 class NeXusMonitorName(sciline.Scope[MonitorType, str], str):
     """Name of Incident|Transmission monitor in NeXus file"""
 
 
-class FileList(sciline.Scope[RunType, list], list):
-    """Filenames of BackgroundRun|EmptyBeamRun|SampleRun"""
+PixelMaskFilename = NewType('PixelMaskFilename', str)
+
+FilenameType = TypeVar('FilenameType', bound=str)
+
 
+DataFolder = NewType('DataFolder', str)
 
-BeamStopPosition = NewType('BeamStopPosition', sc.Variable)
-"""Approximate center of the beam stop position"""
 
-BeamStopRadius = NewType('BeamStopRadius', sc.Variable)
-"""Radius of the beam stop"""
+class FilePath(sciline.Scope[FilenameType, str], str):
+    """Path to a file"""
+
+
+class Filename(sciline.Scope[RunType, str], str):
+    """Filename of a run"""
+
+
+MaskedDetectorIDs = NewType('MaskedDetectorIDs', sc.Variable)
+"""1-D variable listing all masked detector IDs."""
+
 
 # 3  Workflow (intermediate) results
 
 
+class RawSource(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
+    """Raw source from NeXus file"""
+
+
+class RawSample(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
+    """Raw sample from NeXus file"""
+
+
 class SamplePosition(sciline.Scope[RunType, sc.Variable], sc.Variable):
     """Sample position"""
 
 
 class SourcePosition(sciline.Scope[RunType, sc.Variable], sc.Variable):
     """Source position"""
 
 
 DirectBeam = NewType('DirectBeam', sc.DataArray)
 """Direct beam"""
 
 
-class TransmissionFraction(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class TransmissionFraction(
+    sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray
+):
     """Transmission fraction"""
 
 
 CleanDirectBeam = NewType('CleanDirectBeam', sc.DataArray)
 """Direct beam after resampling to required wavelength bins"""
 
 
-class DetectorPixelShape(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
+class DetectorPixelShape(sciline.Scope[ScatteringRunType, sc.DataGroup], sc.DataGroup):
     """Geometry of the detector from description in nexus file."""
 
 
-class LabFrameTransform(sciline.Scope[RunType, sc.Variable], sc.Variable):
+class LabFrameTransform(sciline.Scope[ScatteringRunType, sc.Variable], sc.Variable):
     """Coordinate transformation from detector local coordinates
     to the sample frame of reference."""
 
 
-class SolidAngle(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class SolidAngle(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
     """Solid angle of detector pixels seen from sample position"""
 
 
-class LoadedFileContents(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
-    """The entire contents of a loaded file"""
+class LoadedNeXusDetector(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
+    """Detector data, loaded from a NeXus file, containing not only neutron events
+    but also pixel shape information, transformations, ..."""
+
+
+class LoadedNeXusMonitor(
+    sciline.ScopeTwoParams[RunType, MonitorType, sc.DataGroup], sc.DataGroup
+):
+    """Monitor data loaded from a NeXus file, containing not only neutron events
+    but also transformations, ..."""
+
+
+class RawData(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
+    """Raw detector data"""
+
+
+class ConfiguredReducibleDataData(
+    sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray
+):
+    """Raw event data where variances and necessary coordinates
+    (e.g. sample and source position) have been added, and where optionally some
+    user configuration was applied to some of the coordinates."""
+
+
+class TofData(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
+    """Data with a time-of-flight coordinate"""
+
+
+class TofMonitor(
+    sciline.ScopeTwoParams[RunType, MonitorType, sc.DataGroup], sc.DataGroup
+):
+    """Monitor data with a time-of-flight coordinate"""
 
 
-class RawData(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
-    """Raw data"""
+PixelMask = NewType('PixelMask', sc.Variable)
 
 
-class MaskedData(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class MaskedData(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
     """Raw data with pixel-specific masks applied"""
 
 
-class CalibratedMaskedData(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class CalibratedMaskedData(
+    sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray
+):
     """Raw data with pixel-specific masks applied and calibrated pixel positions"""
 
 
-class NormWavelengthTerm(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class NormWavelengthTerm(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
     """Normalization term (numerator) for IofQ before scaling with solid-angle."""
 
 
 class CleanWavelength(
-    sciline.ScopeTwoParams[RunType, IofQPart, sc.DataArray], sc.DataArray
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """
     Prerequisite for IofQ numerator or denominator.
 
     This can either be the sample or background counts, converted to wavelength,
     or the respective normalization terms computed from the respective solid angle,
     direct beam, and monitors.
     """
 
 
 class CleanWavelengthMasked(
-    sciline.ScopeTwoParams[RunType, IofQPart, sc.DataArray], sc.DataArray
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """Result of applying wavelength masking to :py:class:`CleanWavelength`"""
 
 
-class CleanQ(sciline.ScopeTwoParams[RunType, IofQPart, sc.DataArray], sc.DataArray):
+class CleanQ(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
     """Result of converting :py:class:`CleanWavelengthMasked` to Q"""
 
 
 class CleanSummedQ(
-    sciline.ScopeTwoParams[RunType, IofQPart, sc.DataArray], sc.DataArray
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """Result of histogramming/binning :py:class:`CleanQ` over all pixels into Q bins"""
 
 
-class IofQ(sciline.Scope[RunType, sc.DataArray], sc.DataArray):
+class CleanSummedQMergedBanks(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """CleanSummedQ with merged banks"""
+
+
+class FinalSummedQ(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """Final data into Q bins, in a state that is ready to be normalized."""
+
+
+class IofQ(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
     """I(Q)"""
 
 
 BackgroundSubtractedIofQ = NewType('BackgroundSubtractedIofQ', sc.DataArray)
 """I(Q) with background (given by I(Q) of the background run) subtracted"""
 
 
 class RawMonitor(
     sciline.ScopeTwoParams[RunType, MonitorType, sc.DataArray], sc.DataArray
 ):
     """Raw monitor data"""
 
 
+class ConfiguredReducibleMonitor(
+    sciline.ScopeTwoParams[RunType, MonitorType, sc.DataArray], sc.DataArray
+):
+    """Raw monitor data where variances and necessary coordinates
+    (e.g. source position) have been added, and where optionally some
+    user configuration was applied to some of the coordinates."""
+
+
 class WavelengthMonitor(
     sciline.ScopeTwoParams[RunType, MonitorType, sc.DataArray], sc.DataArray
 ):
     """Monitor data converted to wavelength"""
 
 
 class CleanMonitor(
```

### Comparing `esssans-24.2.0/src/esssans/uncertainty.py` & `esssans-24.4.0/src/ess/sans/uncertainty.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,31 +63,16 @@
     variances by the number of events in each bin. An explicit broadcast is performed
     to bypass Scipp's safety check on broadcasting variances.
 
     Details will be published in an upcoming publication by Simon Heybrock et al.
     """
     if da.variances is None:
         return da
-    constituents = events.bins.constituents
-
-    if 'Q' in constituents['data'].coords:
-        Q = constituents['data'].coords['Q']
-        constituents['data'] = sc.DataArray(
-            sc.ones(sizes=Q.sizes, dtype='float32'), coords={'Q': Q}
-        )
-        edges = {'Q': da.coords['Q']}
-    else:
-        Qx = constituents['data'].coords['Qx']
-        Qy = constituents['data'].coords['Qy']
-        constituents['data'] = sc.DataArray(
-            sc.ones(sizes=Qx.sizes, dtype='float32'),
-            coords={'Qx': Qx, 'Qy': Qy},
-        )
-        edges = {'Qy': da.coords['Qy'], 'Qx': da.coords['Qx']}
-    # Combine all bins of the events that correspond to the same bin in the input data
-    to_concat = set(events.dims) - set(da.dims)
-    binned = sc.DataArray(sc.bins(**constituents).bins.concat(to_concat))
-    counts = binned.hist(**edges)
-    da = da.copy()
-    da.variances *= counts.values
+    if da.sizes != events.sizes:
+        # This is a safety check, but we should never get here.
+        raise ValueError(f"Sizes {da.sizes} do not match event sizes {events.sizes}")
+    # Given how this function is used currently (in the context of normalization
+    # with matching binning in numerator and denominator, not using scipp.lookup),
+    # we can simply count the events in the existing binning.
+    da.variances *= events.bins.size().values
     da.data = sc.bins_like(events, da.data)
     return da
```

### Comparing `esssans-24.2.0/src/esssans.egg-info/PKG-INFO` & `esssans-24.4.0/src/esssans.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: esssans
-Version: 24.2.0
+Version: 24.4.0
 Summary: SANS data reduction for the European Spallation Source
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -38,28 +38,28 @@
 Project-URL: Source, https://github.com/scipp/esssans
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: graphviz
+Requires-Dist: essreduce
 Requires-Dist: plopp
 Requires-Dist: pythreejs
-Requires-Dist: sciline>=23.9.1
+Requires-Dist: sciline>=24.4.1
 Requires-Dist: scipp>=23.8.0
 Requires-Dist: scippneutron>=23.9.0
 Requires-Dist: scippnexus>=23.12.1
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/esssans.svg)](https://pypi.python.org/pypi/esssans)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/esssans/badges/version.svg)](https://anaconda.org/scipp/esssans)
```

### Comparing `esssans-24.2.0/tests/common_test.py` & `esssans-24.4.0/tests/common_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
 
-from esssans.common import mask_range
+from ess.sans.common import mask_range
 
 
 def test_mask_range_dense_data():
     x = sc.arange('x', 5.0, unit='m')
     da = sc.DataArray(data=x, coords={'x': x})
     mask = sc.DataArray(
         data=sc.array(dims=['x'], values=[True]),
@@ -65,16 +65,21 @@
     mask = sc.DataArray(
         data=sc.array(dims=['x'], values=[True]),
         coords={
             'x': sc.array(dims=['x'], values=[1.9, 3.001], unit='m'),
         },
     )
     masked = mask_range(binned, mask=mask, name='mymask')
-    assert masked.masks['mymask'].values.tolist() == [True]
-    assert sc.identical(masked.coords['x'], mask.coords['x'])
+    # This should make 3 bins that span the entire data range, and where the middle
+    # one is masked.
+    assert masked.masks['mymask'].values.tolist() == [False, True, False]
+    binned_full_range = binned.bin(x=1)
+    assert sc.identical(masked.coords['x'][0], binned_full_range.coords['x'][0])
+    assert sc.identical(masked.coords['x'][1:3], mask.coords['x'])
+    assert sc.identical(masked.coords['x'][3], binned_full_range.coords['x'][1])
 
 
 def test_mask_range_binned_data_has_prior_single_bin():
     x = sc.arange('x', 5.0, unit='m')
     da = sc.DataArray(data=x, coords={'x': x, 'y': x + x.max()})
     binned = da.bin(x=1)
     mask = sc.DataArray(
```

### Comparing `esssans-24.2.0/tests/io_test.py` & `esssans-24.4.0/tests/io_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import pytest
 import sciline
 import scipp as sc
 import scipp.testing
 import scippnexus as snx
 from scippnexus.application_definitions import nxcansas
 
-from esssans.io import save_background_subtracted_iofq
-from esssans.types import BackgroundSubtractedIofQ, OutFilename, RunNumber, RunTitle
+from ess.sans.io import save_background_subtracted_iofq
+from ess.sans.types import BackgroundSubtractedIofQ, OutFilename, RunNumber, RunTitle
 
 
 @pytest.mark.parametrize('use_edges', (True, False))
 def test_save_background_subtracted_iofq(use_edges, tmp_path):
     def background_subtracted_iofq() -> BackgroundSubtractedIofQ:
         i = sc.arange('Q', 0.0, 400.0)
         i.variances = i.values / 10
```

### Comparing `esssans-24.2.0/tests/loki/common.py` & `esssans-24.4.0/tests/loki/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,43 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-from typing import List, Optional
+from typing import Callable, List
 
 import scipp as sc
 
-from esssans.loki import default_parameters
-from esssans.types import (
+from ess import loki, sans
+from ess.sans.types import (
     BackgroundRun,
-    BeamStopPosition,
-    BeamStopRadius,
     CorrectForGravity,
     EmptyBeamRun,
-    FileList,
+    Filename,
+    NeXusDetectorName,
     QBins,
     QxyBins,
     ReturnEvents,
     SampleRun,
     TransmissionRun,
     UncertaintyBroadcastMode,
     WavelengthBins,
 )
 
 
-def make_params(
-    sample_runs: Optional[List[str]] = None,
-    background_runs: Optional[List[str]] = None,
-    qxy: bool = False,
-) -> dict:
-    params = default_parameters.copy()
-
-    if sample_runs is None:
-        sample_runs = ['60339-2022-02-28_2215.nxs']
-    if background_runs is None:
-        background_runs = ['60393-2022-02-28_2215.nxs']
-
-    # List of files
-    params[FileList[SampleRun]] = sample_runs
-    params[FileList[BackgroundRun]] = background_runs
-    params[FileList[TransmissionRun[SampleRun]]] = ['60394-2022-02-28_2215.nxs']
-    params[FileList[TransmissionRun[BackgroundRun]]] = ['60392-2022-02-28_2215.nxs']
-    params[FileList[EmptyBeamRun]] = ['60392-2022-02-28_2215.nxs']
+def make_params(qxy: bool = False) -> dict:
+    params = loki.default_parameters.copy()
+
+    params[NeXusDetectorName] = 'larmor_detector'
+    params[Filename[SampleRun]] = '60339-2022-02-28_2215.nxs'
+    params[Filename[BackgroundRun]] = '60393-2022-02-28_2215.nxs'
+    params[Filename[TransmissionRun[SampleRun]]] = '60394-2022-02-28_2215.nxs'
+    params[Filename[TransmissionRun[BackgroundRun]]] = '60392-2022-02-28_2215.nxs'
+    params[Filename[EmptyBeamRun]] = '60392-2022-02-28_2215.nxs'
 
     params[WavelengthBins] = sc.linspace(
         'wavelength', start=1.0, stop=13.0, num=51, unit='angstrom'
     )
-    params[BeamStopPosition] = sc.vector([-0.026, -0.022, 0.0], unit='m')
-    params[BeamStopRadius] = sc.scalar(0.042, unit='m')
     params[CorrectForGravity] = True
     params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound
     params[ReturnEvents] = False
 
     if qxy:
         params[QxyBins] = {
             'Qx': sc.linspace('Qx', -0.3, 0.3, 91, unit='1/angstrom'),
@@ -57,7 +45,27 @@
         }
     else:
         params[QBins] = sc.linspace(
             dim='Q', start=0.01, stop=0.3, num=101, unit='1/angstrom'
         )
 
     return params
+
+
+def loki_providers_no_beam_center_finder() -> List[Callable]:
+    from ess.isissans.io import read_xml_detector_masking
+
+    return list(
+        sans.providers
+        + loki.providers
+        + loki.data.providers
+        + (
+            read_xml_detector_masking,
+            loki.io.dummy_load_sample,
+        )
+    )
+
+
+def loki_providers() -> List[Callable]:
+    return loki_providers_no_beam_center_finder() + [
+        sans.beam_center_finder.beam_center_from_center_of_mass
+    ]
```

### Comparing `esssans-24.2.0/tests/loki/directbeam_test.py` & `esssans-24.4.0/tests/loki/directbeam_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import sys
 from pathlib import Path
-from typing import Callable, List
 
 import sciline
 import scipp as sc
 from scipp.scipy.interpolate import interp1d
 
-import esssans as sans
-from esssans.loki.data import get_path
-from esssans.types import DimsToKeep, QBins, WavelengthBands, WavelengthBins
+from ess import sans
+from ess.loki.data import get_path
+from ess.sans.types import DimsToKeep, QBins, WavelengthBands, WavelengthBins
 
 sys.path.insert(0, str(Path(__file__).resolve().parent))
-from common import make_params  # noqa: E402
+from common import loki_providers, make_params  # noqa: E402
 
 
 def _get_I0(qbins: sc.Variable) -> sc.Variable:
     Iq_theory = sc.io.load_hdf5(get_path('PolyGauss_I0-50_Rg-60.h5'))
     f = interp1d(Iq_theory, 'Q')
     return f(sc.midpoints(qbins)).data[0]
 
 
-def loki_providers() -> List[Callable]:
-    return list(sans.providers + sans.loki.providers)
-
-
 def test_can_compute_direct_beam_for_all_pixels():
     n_wavelength_bands = 10
     params = make_params()
     params[WavelengthBands] = sc.linspace(
         'wavelength',
         params[WavelengthBins].min(),
         params[WavelengthBins].max(),
```

### Comparing `esssans-24.2.0/tests/normalization_test.py` & `esssans-24.4.0/tests/normalization_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
 
-from esssans import normalization
-from esssans.sans2d.data import get_path
+from ess.isissans.data import get_path
+from ess.sans import normalization
 
 # See https://github.com/mantidproject/mantid/blob/main/instrument/SANS2D_Definition_Tubes.xml  # noqa: E501
 _SANS2D_PIXEL_RADIUS = 0.00405 * sc.Unit('m')
 _SANS2D_PIXEL_LENGTH = 0.002033984375 * sc.Unit('m')
-_SANS2D_SOLID_ANGLE_REFERENCE_FILE = 'SANS2D00063091.SolidAngle_from_mantid.hdf5'
+_SANS2D_SOLID_ANGLE_REFERENCE_FILE = 'SANS2D00063091.SolidAngle_from_mantid.h5'
 
 
 def _sans2d_geometry():
     R = _SANS2D_PIXEL_RADIUS.value
     L = _SANS2D_PIXEL_LENGTH.value
     pixel_shape = {
         'vertices': sc.vectors(
```

### Comparing `esssans-24.2.0/tests/sans2d/reduction_test.py` & `esssans-24.4.0/tests/isissans/sans2d_reduction_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,75 +2,93 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from typing import Callable, List
 
 import pytest
 import sciline
 import scipp as sc
 
-import esssans as sans
-from esssans.sans2d import default_parameters
-from esssans.types import (
+from ess import isissans as isis
+from ess import sans
+from ess.isissans import MonitorOffset, SampleOffset, sans2d
+from ess.sans.types import (
     BackgroundRun,
     BackgroundSubtractedIofQ,
     BeamCenter,
     CorrectForGravity,
     DirectBeam,
     DirectBeamFilename,
     EmptyBeamRun,
-    FileList,
+    Filename,
+    Incident,
     IofQ,
+    MaskedData,
+    NeXusMonitorName,
     NonBackgroundWavelengthRange,
     QBins,
     RawData,
     ReturnEvents,
     SampleRun,
     SolidAngle,
-    TransmissionRun,
+    Transmission,
     UncertaintyBroadcastMode,
     WavelengthBands,
     WavelengthBins,
     WavelengthMask,
 )
 
 
 def make_params() -> dict:
-    params = default_parameters.copy()
+    params = {}
     params[WavelengthBins] = sc.linspace(
         'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'
     )
     params[WavelengthMask] = sc.DataArray(
         data=sc.array(dims=['wavelength'], values=[True]),
         coords={
             'wavelength': sc.array(
                 dims=['wavelength'], values=[2.21, 2.59], unit='angstrom'
             )
         },
     )
-    params[sans.sans2d.LowCountThreshold] = sc.scalar(100.0, unit='counts')
+    params[sans2d.LowCountThreshold] = sc.scalar(100.0, unit='counts')
 
     params[QBins] = sc.linspace(
         dim='Q', start=0.01, stop=0.55, num=141, unit='1/angstrom'
     )
-    params[FileList[BackgroundRun]] = ['SANS2D00063159.hdf5']
-    params[FileList[TransmissionRun[BackgroundRun]]] = params[FileList[BackgroundRun]]
-    params[FileList[SampleRun]] = ['SANS2D00063114.hdf5']
-    params[FileList[TransmissionRun[SampleRun]]] = params[FileList[SampleRun]]
-    params[FileList[EmptyBeamRun]] = ['SANS2D00063091.hdf5']
-    params[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.hdf5'
+    params[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat'
+    params[Filename[SampleRun]] = 'SANS2D00063114.nxs'
+    params[Filename[BackgroundRun]] = 'SANS2D00063159.nxs'
+    params[Filename[EmptyBeamRun]] = 'SANS2D00063091.nxs'
+
+    params[NeXusMonitorName[Incident]] = 'monitor2'
+    params[NeXusMonitorName[Transmission]] = 'monitor4'
+    params[SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')
+    params[MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')
+
     params[NonBackgroundWavelengthRange] = sc.array(
         dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'
     )
     params[CorrectForGravity] = True
     params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound
     params[ReturnEvents] = False
     return params
 
 
 def sans2d_providers():
-    return list(sans.providers + sans.sans2d.providers)
+    return list(
+        sans.providers
+        + isis.providers
+        + isis.data.providers
+        + isis.sans2d.providers
+        + (
+            isis.data.transmission_from_background_run,
+            isis.data.transmission_from_sample_run,
+            sans.beam_center_finder.beam_center_from_center_of_mass,
+        )
+    )
 
 
 def test_can_create_pipeline():
     sciline.Pipeline(sans2d_providers(), params=make_params())
 
 
 @pytest.mark.parametrize(
@@ -162,15 +180,15 @@
 
     return dict(zip([get_type_hints(func)['return'] for func in funcs], funcs))
 
 
 def pixel_dependent_direct_beam(
     filename: DirectBeamFilename, shape: RawData[SampleRun]
 ) -> DirectBeam:
-    direct_beam = sans.sans2d.io.pooch_load_direct_beam(filename)
+    direct_beam = isis.data.load_direct_beam(isis.data.get_path(filename))
     sizes = {'spectrum': shape.sizes['spectrum'], **direct_beam.sizes}
     return DirectBeam(direct_beam.broadcast(sizes=sizes).copy())
 
 
 @pytest.mark.parametrize(
     'uncertainties',
     [UncertaintyBroadcastMode.drop, UncertaintyBroadcastMode.upper_bound],
@@ -181,81 +199,112 @@
     providers = as_dict(sans2d_providers())
     providers[DirectBeam] = pixel_dependent_direct_beam
     pipeline = sciline.Pipeline(providers.values(), params=params)
     result = pipeline.compute(BackgroundSubtractedIofQ)
     assert result.dims == ('Q',)
 
 
+MANTID_BEAM_CENTER = sc.vector([0.09288, -0.08195, 0], unit='m')
+
+
 def test_beam_center_from_center_of_mass_is_close_to_verified_result():
     params = make_params()
     providers = sans2d_providers()
     pipeline = sciline.Pipeline(providers, params=params)
     center = pipeline.compute(BeamCenter)
-    # This is the result we got with the pre-sciline implementation, using the full IofQ
-    # calculation. The difference is about 5 mm in X or Y, probably due to a bias
+    # This is the result obtained from Mantid, using the full IofQ
+    # calculation. The difference is about 3 mm in X or Y, probably due to a bias
     # introduced by the sample holder, which the center-of-mass approach cannot ignore.
-    center_pre_sciline_raw_solid_angle = sc.vector([0.0945643, -0.082074, 0], unit='m')
-    assert sc.allclose(
-        center, center_pre_sciline_raw_solid_angle, atol=sc.scalar(5e-3, unit='m')
-    )
+    assert sc.allclose(center, MANTID_BEAM_CENTER, atol=sc.scalar(3e-3, unit='m'))
 
 
 def test_beam_center_finder_without_direct_beam_reproduces_verified_result():
     params = make_params()
     params[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(
         'Q', 0.02, 0.3, 71, unit='1/angstrom'
     )
     del params[DirectBeamFilename]
     providers = sans2d_providers()
     providers.remove(sans.beam_center_finder.beam_center_from_center_of_mass)
     providers.append(sans.beam_center_finder.beam_center_from_iofq)
     pipeline = sciline.Pipeline(providers, params=params)
     center = pipeline.compute(BeamCenter)
-    # This is the result we got with the pre-sciline implementation
-    # The difference is that the reference result computed the solid angle only once,
-    # before applying any detector positions shifts.
-    center_pre_sciline_raw_solid_angle = sc.vector([0.0945643, -0.082074, 0], unit='m')
-    assert sc.allclose(
-        center, center_pre_sciline_raw_solid_angle, atol=sc.scalar(4e-3, unit='m')
+    assert sc.allclose(center, MANTID_BEAM_CENTER, atol=sc.scalar(2e-3, unit='m'))
+
+
+def test_beam_center_can_get_closer_to_verified_result_with_low_counts_mask():
+    def low_counts_mask(
+        sample: RawData[SampleRun],
+        low_counts_threshold: sans2d.LowCountThreshold,
+    ) -> sans2d.SampleHolderMask:
+        return sans2d.SampleHolderMask(sample.hist().data < low_counts_threshold)
+
+    params = make_params()
+    params[sans2d.LowCountThreshold] = sc.scalar(80.0, unit='counts')
+    params[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(
+        'Q', 0.02, 0.3, 71, unit='1/angstrom'
     )
+    del params[DirectBeamFilename]
+    providers = sans2d_providers()
+    providers.remove(sans2d.sample_holder_mask)
+    providers.remove(sans.beam_center_finder.beam_center_from_center_of_mass)
+    providers.append(sans.beam_center_finder.beam_center_from_iofq)
+    providers.append(low_counts_mask)
+    pipeline = sciline.Pipeline(providers, params=params)
+    center = pipeline.compute(BeamCenter)
+    assert sc.allclose(center, MANTID_BEAM_CENTER, atol=sc.scalar(5e-4, unit='m'))
 
 
 def test_beam_center_finder_works_with_direct_beam():
     params = make_params()
     params[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(
         'Q', 0.02, 0.3, 71, unit='1/angstrom'
     )
     providers = sans2d_providers()
     providers.remove(sans.beam_center_finder.beam_center_from_center_of_mass)
     providers.append(sans.beam_center_finder.beam_center_from_iofq)
     pipeline = sciline.Pipeline(providers, params=params)
-    center = pipeline.compute(BeamCenter)  # (0.0951122, -0.079375, 0)
-    center_no_direct_beam = sc.vector([0.0945643, -0.082074, 0], unit='m')
-
-    assert sc.allclose(center, center_no_direct_beam, atol=sc.scalar(1e-2, unit='m'))
+    center_with_direct_beam = pipeline.compute(BeamCenter)
+    assert sc.allclose(
+        center_with_direct_beam, MANTID_BEAM_CENTER, atol=sc.scalar(2e-3, unit='m')
+    )
 
 
 def test_beam_center_finder_works_with_pixel_dependent_direct_beam():
     params = make_params()
     params[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(
         'Q', 0.02, 0.3, 71, unit='1/angstrom'
     )
     providers = sans2d_providers()
     providers.remove(sans.beam_center_finder.beam_center_from_center_of_mass)
     providers.append(sans.beam_center_finder.beam_center_from_iofq)
     pipeline = sciline.Pipeline(providers, params=params)
     center_pixel_independent_direct_beam = pipeline.compute(BeamCenter)
 
-    direct_beam = (
-        pipeline.compute(DirectBeam)
-        .broadcast(sizes={'spectrum': 61440, 'wavelength': 175})
-        .copy()
-    )
+    direct_beam = pipeline.compute(DirectBeam)
+    pixel_dependent_direct_beam = direct_beam.broadcast(
+        sizes={
+            'spectrum': pipeline.compute(MaskedData[SampleRun]).sizes['spectrum'],
+            'wavelength': direct_beam.sizes['wavelength'],
+        }
+    ).copy()
 
-    providers = list(sans.providers + sans.sans2d.providers)
+    providers = sans2d_providers()
     providers.remove(sans.beam_center_finder.beam_center_from_center_of_mass)
     providers.append(sans.beam_center_finder.beam_center_from_iofq)
     pipeline = sciline.Pipeline(providers, params=params)
-    pipeline[DirectBeam] = direct_beam
+    pipeline[DirectBeam] = pixel_dependent_direct_beam
 
     center = pipeline.compute(BeamCenter)
     assert sc.identical(center, center_pixel_independent_direct_beam)
+
+
+def test_workflow_runs_without_gravity_if_beam_center_is_provided():
+    params = make_params()
+    params[CorrectForGravity] = False
+    pipeline = sciline.Pipeline(sans2d_providers(), params=params)
+    da = pipeline.compute(RawData[SampleRun])
+    del da.coords['gravity']
+    pipeline[RawData[SampleRun]] = da
+    pipeline[BeamCenter] = MANTID_BEAM_CENTER
+    result = pipeline.compute(BackgroundSubtractedIofQ)
+    assert result.dims == ('Q',)
```

### Comparing `esssans-24.2.0/tests/uncertainty_test.py` & `esssans-24.4.0/tests/uncertainty_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import scipp as sc
 from scipp.testing import assert_identical
 
-from esssans.uncertainty import broadcast_with_upper_bound_variances
+from ess.sans.uncertainty import broadcast_with_upper_bound_variances
 
 
 def test_broadcast_returns_original_if_no_new_dims():
     var = sc.ones(dims=['x', 'y'], shape=[2, 3], with_variances=True)
     assert broadcast_with_upper_bound_variances(var, {'x': 2}) is var
     assert broadcast_with_upper_bound_variances(var, {'y': 3}) is var
```

### Comparing `esssans-24.2.0/tox.ini` & `esssans-24.4.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py39
+envlist = py310
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 setenv =
   JUPYTER_PLATFORM_DIRS = 1
 commands = pytest {posargs}
@@ -11,24 +11,24 @@
 [testenv:nightly]
 deps = -r requirements/nightly.txt
 commands = pytest
 
 [testenv:unpinned]
 description = Test with unpinned dependencies, as a user would install now.
 deps =
+  -r requirements/basetest.txt
   esssans
-  pytest
 commands = pytest
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
 deps = -r requirements/docs.txt
 allowlist_externals=find
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
-           python -m sphinx -j2 -v -b doctest -d {toxworkdir}/docs_doctrees docs html
+           python -m sphinx -v -b doctest -d {toxworkdir}/docs_doctrees docs html
            find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
 
 [testenv:releasedocs]
 description = invoke sphinx-build to build the HTML docs from a released version
 skip_install = true
 deps =
   esssans=={posargs}
```

