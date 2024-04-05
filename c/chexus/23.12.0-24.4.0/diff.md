# Comparing `tmp/chexus-23.12.0.tar.gz` & `tmp/chexus-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chexus-23.12.0.tar", last modified: Thu Dec 14 07:50:58 2023, max compression
+gzip compressed data, was "chexus-24.4.0.tar", last modified: Fri Apr  5 11:49:16 2024, max compression
```

## Comparing `chexus-23.12.0.tar` & `chexus-24.4.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.040066 chexus-23.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-14 07:50:47.000000 chexus-23.12.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.028066 chexus-23.12.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.028066 chexus-23.12.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-14 07:50:47.000000 chexus-23.12.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-14 07:50:47.000000 chexus-23.12.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-12-14 07:50:47.000000 chexus-23.12.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-12-14 07:50:47.000000 chexus-23.12.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-14 07:50:47.000000 chexus-23.12.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-14 07:50:47.000000 chexus-23.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-14 07:50:47.000000 chexus-23.12.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2023-12-14 07:50:58.040066 chexus-23.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-14 07:50:47.000000 chexus-23.12.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-14 07:50:47.000000 chexus-23.12.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/_static/anaconda-icon.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/_templates/module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.032066 chexus-23.12.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-14 07:50:47.000000 chexus-23.12.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-12-14 07:50:47.000000 chexus-23.12.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.036066 chexus-23.12.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-14 07:50:47.000000 chexus-23.12.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-14 07:50:58.040066 chexus-23.12.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.028066 chexus-23.12.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.036066 chexus-23.12.0/src/chexus/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2023-12-14 07:50:47.000000 chexus-23.12.0/src/chexus/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.040066 chexus-23.12.0/src/chexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-14 07:50:58.000000 chexus-23.12.0/src/chexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 07:50:58.036066 chexus-23.12.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-14 07:50:47.000000 chexus-23.12.0/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-14 07:50:47.000000 chexus-23.12.0/tests/validate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2023-12-14 07:50:47.000000 chexus-23.12.0/tests/validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-12-14 07:50:47.000000 chexus-23.12.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 11:48:56.000000 chexus-24.4.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.831132 chexus-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 11:48:56.000000 chexus-24.4.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-05 11:48:56.000000 chexus-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 11:48:56.000000 chexus-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-05 11:48:56.000000 chexus-24.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-05 11:48:56.000000 chexus-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 11:48:56.000000 chexus-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 11:48:56.000000 chexus-24.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 11:49:16.843132 chexus-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 11:48:56.000000 chexus-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 11:48:56.000000 chexus-24.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_static/anaconda-icon.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_templates/module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/_typehints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.835132 chexus-24.4.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-05 11:48:56.000000 chexus-24.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 11:48:56.000000 chexus-24.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.839132 chexus-24.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 11:48:56.000000 chexus-24.4.0/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 11:49:16.847132 chexus-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.831132 chexus-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/src/chexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-05 11:48:56.000000 chexus-24.4.0/src/chexus/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/src/chexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:49:16.000000 chexus-24.4.0/src/chexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:49:16.843132 chexus-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-05 11:48:56.000000 chexus-24.4.0/tests/validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 11:48:56.000000 chexus-24.4.0/tox.ini
```

### Comparing `chexus-23.12.0/.github/workflows/ci.yml` & `chexus-24.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/docs.yml` & `chexus-24.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/nightly_at_main.yml` & `chexus-24.4.0/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/nightly_at_release.yml` & `chexus-24.4.0/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/release.yml` & `chexus-24.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/test.yml` & `chexus-24.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.github/workflows/unpinned.yml` & `chexus-24.4.0/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/.pre-commit-config.yaml` & `chexus-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/CODE_OF_CONDUCT.md` & `chexus-24.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/CONTRIBUTING.md` & `chexus-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/LICENSE` & `chexus-24.4.0/LICENSE`

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

### Comparing `chexus-23.12.0/PKG-INFO` & `chexus-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chexus
-Version: 23.12.0
+Version: 24.4.0
 Summary: Validate and check NeXus files
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
```

### Comparing `chexus-23.12.0/README.md` & `chexus-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/conda/meta.yaml` & `chexus-24.4.0/conda/meta.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     - python>=3.10
 
 test:
   imports:
     - chexus
   requires:
     - pytest
+    - scipp
   source_files:
     - pyproject.toml
     - tests/
   commands:
     # We ignore warnings during release package builds
     - python -m pytest -Wignore tests
```

### Comparing `chexus-23.12.0/docs/_static/anaconda-icon.js` & `chexus-24.4.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/_templates/class-template.rst` & `chexus-24.4.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/_templates/module-template.rst` & `chexus-24.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/about/index.md` & `chexus-24.4.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/conf.py` & `chexus-24.4.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import os
 import sys
 
 import chexus
 
 sys.path.insert(0, os.path.abspath('.'))
 
+from _typehints import typehints_formatter_for  # noqa: E402
+
 # General information about the project.
 project = u'Chexus'
-copyright = u'2023 Scipp contributors'
+copyright = u'2024 Scipp contributors'
 author = u'Scipp contributors'
 
 html_show_sourcelink = True
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
@@ -50,14 +52,15 @@
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
 
@@ -68,14 +71,15 @@
 napoleon_preprocess_types = True
 napoleon_type_aliases = {
     # objects without namespace: numpy
     "ndarray": "~numpy.ndarray",
 }
 typehints_defaults = 'comma'
 typehints_use_rtype = False
+typehints_formatter = typehints_formatter_for('chexus')
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `chexus-23.12.0/docs/developer/coding-conventions.md` & `chexus-24.4.0/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/developer/dependency-management.md` & `chexus-24.4.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/docs/developer/getting-started.md` & `chexus-24.4.0/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/pyproject.toml` & `chexus-24.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/requirements/ci.txt` & `chexus-24.4.0/requirements/ci.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # via virtualenv
 filelock==3.13.1
     # via
     #   tox
     #   virtualenv
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.40
+gitpython==3.1.41
     # via -r ci.in
 idna==3.6
     # via requests
 packaging==23.2
     # via
     #   -r ci.in
     #   pyproject-api
@@ -44,13 +44,13 @@
     # via -r ci.in
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.11.4
+tox==4.12.1
     # via -r ci.in
 urllib3==2.1.0
     # via requests
 virtualenv==20.25.0
     # via tox
```

### Comparing `chexus-23.12.0/requirements/dev.txt` & `chexus-24.4.0/requirements/dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 -r docs.txt
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
 annotated-types==0.6.0
     # via pydantic
-anyio==4.1.0
+anyio==4.2.0
     # via jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
@@ -26,15 +26,15 @@
     # via jupyterlab
 cffi==1.16.0
     # via argon2-cffi-bindings
 click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
-copier==9.1.0
+copier==9.1.1
     # via -r dev.in
 dunamai==1.19.0
     # via copier
 fqdn==1.5.1
     # via jsonschema
 funcy==2.0
     # via copier
@@ -42,32 +42,32 @@
     # via jsonschema
 jinja2-ansible-filters==1.3.2
     # via copier
 json5==0.9.14
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.20.0
+jsonschema[format-nongpl]==4.21.0
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-events==0.9.0
     # via jupyter-server
-jupyter-lsp==2.2.1
+jupyter-lsp==2.2.2
     # via jupyterlab
-jupyter-server==2.12.1
+jupyter-server==2.12.5
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
-jupyter-server-terminals==0.5.0
+jupyter-server-terminals==0.5.1
     # via jupyter-server
-jupyterlab==4.0.9
+jupyterlab==4.0.10
     # via -r dev.in
 jupyterlab-server==2.25.2
     # via jupyterlab
 notebook-shim==0.2.3
     # via jupyterlab
 overrides==7.4.0
     # via jupyter-server
@@ -79,23 +79,23 @@
     # via pip-compile-multi
 plumbum==1.8.2
     # via copier
 prometheus-client==0.19.0
     # via jupyter-server
 pycparser==2.21
     # via cffi
-pydantic==2.5.2
+pydantic==2.5.3
     # via copier
-pydantic-core==2.14.5
+pydantic-core==2.14.6
     # via pydantic
 python-json-logger==2.0.7
     # via jupyter-events
-pyyaml-include==1.3.1
+pyyaml-include==1.3.2
     # via copier
-questionary==2.0.1
+questionary==1.10.0
     # via copier
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
@@ -107,15 +107,15 @@
     # via anyio
 terminado==0.18.0
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
-types-python-dateutil==2.8.19.14
+types-python-dateutil==2.8.19.20240106
     # via arrow
 uri-template==1.3.0
     # via jsonschema
 webcolors==1.13
     # via jsonschema
 websocket-client==1.7.0
     # via jupyter-server
```

### Comparing `chexus-23.12.0/requirements/make_base.py` & `chexus-24.4.0/requirements/make_base.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/requirements/static.txt` & `chexus-24.4.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/src/chexus/hdf5.py` & `chexus-24.4.0/src/chexus/hdf5.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/src/chexus/io.py` & `chexus-24.4.0/src/chexus/io.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/src/chexus/json.py` & `chexus-24.4.0/src/chexus/json.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/src/chexus/tree.py` & `chexus-24.4.0/src/chexus/tree.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/src/chexus/validate.py` & `chexus-24.4.0/src/chexus/validate.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,7 +77,11 @@
         total_checks += result.checks
         total_violations += result.fails
         details += result.format_details()
         summary += result.format_summary()
     summary += '\n'
     summary += f"Total: {total_violations}/{total_checks}"
     return f'{details}\n\n{summary}'
+
+
+def has_violations(results: dict[type, ValidationResult]) -> bool:
+    return any(result.fails for result in results.values())
```

### Comparing `chexus-23.12.0/src/chexus/validators.py` & `chexus-24.4.0/src/chexus/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 
     def applies_to(self, node: Dataset | Group) -> bool:
         return isinstance(node, Dataset) and 'units' in node.attrs
 
     def validate(self, node: Dataset | Group) -> Violation | None:
         units = node.attrs['units']
         invalid = ['hz']
+        if not isinstance(units, str):
+            return Violation(node.name, f'Invalid units type {type(units)}')
         # Units starting with NX_ are likely placeholders from the NeXus standard
         if units.startswith('NX_') or units in invalid:
             return Violation(node.name, f"Invalid units {units}")
 
 
 class index_has_units(Validator):
     def __init__(self) -> None:
@@ -201,14 +203,42 @@
         return isinstance(node, Dataset) and is_transformation(node)
 
     def validate(self, node: Dataset | Group) -> Violation | None:
         if 'depends_on' not in node.attrs:
             return Violation(node.name)
 
 
+class chopper_frequency_units_invalid(Validator):
+    def __init__(self) -> None:
+        super().__init__(
+            "chopper_frequency_unit_invalid",
+            "The unit of NXdisk_chopper.rotation_speed should have dimension 1/Time",
+        )
+
+    def applies_to(self, node: Dataset | Group) -> bool:
+        return (
+            isinstance(node, Group)
+            and node.attrs.get('NX_class') == 'NXdisk_chopper'
+            and 'rotation_speed' in node.children
+        )
+
+    def validate(self, node: Dataset | Group) -> Violation | None:
+        import scipp as sc
+
+        if 'units' in node.children.get('rotation_speed').attrs:
+            unit = node.children.get('rotation_speed').attrs.get('units')
+            try:
+                sc.scalar(1, unit=unit).to(unit='Hz')
+            except sc.UnitError:
+                pass
+            else:
+                return
+        return Violation(node.name)
+
+
 physical_components = [
     'NXaperture',
     'NXattenuator',
     'NXbeam',
     'NXbeam_stop',
     'NXbending_magnet',
     'NXcapillary',
@@ -254,22 +284,27 @@
         return False
 
     def validate(self, node: Dataset | Group) -> Violation | None:
         if 'depends_on' not in node.children:
             return Violation(node.name)
 
 
-def base_validators():
-    return [
+def base_validators(*, has_scipp=True):
+    validators = [
         depends_on_missing(),
         depends_on_target_missing(),
         float_dataset_units_missing(),
         group_has_units(),
         index_has_units(),
         mask_has_units(),
         non_numeric_dataset_has_units(),
         NX_class_attr_missing(),
         NX_class_is_legacy(),
         transformation_depends_on_missing(),
         transformation_offset_units_missing(),
         units_invalid(),
     ]
+    if has_scipp:
+        validators += [
+            chopper_frequency_units_invalid(),
+        ]
+    return validators
```

### Comparing `chexus-23.12.0/src/chexus.egg-info/PKG-INFO` & `chexus-24.4.0/src/chexus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chexus
-Version: 23.12.0
+Version: 24.4.0
 Summary: Validate and check NeXus files
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
```

### Comparing `chexus-23.12.0/src/chexus.egg-info/SOURCES.txt` & `chexus-24.4.0/src/chexus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .github/workflows/nightly_at_main.yml
 .github/workflows/nightly_at_release.yml
 .github/workflows/python-version-ci
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/unpinned.yml
 conda/meta.yaml
+docs/_typehints.py
 docs/conf.py
 docs/index.md
 docs/_static/anaconda-icon.js
 docs/_templates/class-template.rst
 docs/_templates/doc_version.html
 docs/_templates/module-template.rst
 docs/about/index.md
```

### Comparing `chexus-23.12.0/tests/validate_test.py` & `chexus-24.4.0/tests/validate_test.py`

 * *Files identical despite different names*

### Comparing `chexus-23.12.0/tests/validators_test.py` & `chexus-24.4.0/tests/validators_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,21 +251,55 @@
     )
     assert chexus.validators.transformation_offset_units_missing().applies_to(bad)
     result = chexus.validators.transformation_offset_units_missing().validate(bad)
     assert isinstance(result, chexus.Violation)
     assert result.name == 'x'
 
 
-@pytest.mark.parametrize('units', ['NX_LENGTH', 'NX_DIMENSIONLESS', 'hz'])
+@pytest.mark.parametrize('units', ['NX_LENGTH', 'NX_DIMENSIONLESS', 'hz', ['m']])
 def test_units_invalid(units: str):
     good = chexus.Dataset(
         name='x', shape=None, dtype=float, parent=None, attrs={'units': ''}
     )
     assert chexus.validators.units_invalid().applies_to(good)
     assert chexus.validators.units_invalid().validate(good) is None
     bad = chexus.Dataset(
         name='x', shape=None, dtype=float, parent=None, attrs={'units': units}
     )
     assert chexus.validators.units_invalid().applies_to(bad)
     result = chexus.validators.units_invalid().validate(bad)
     assert isinstance(result, chexus.Violation)
     assert result.name == 'x'
+
+
+@pytest.mark.parametrize(
+    'units, good',
+    [
+        ('hz', False),
+        ('', False),
+        ('m/s', False),
+        ('1/year', True),
+        ('Hz', True),
+        ('MHz', True),
+        ('1/ms', True),
+    ],
+)
+def test_NXdisk_chopper_units(units: str, good: bool):
+    group = chexus.Group(
+        name='x',
+        attrs={'NX_class': 'NXdisk_chopper'},
+    )
+    group.children['rotation_speed'] = chexus.Dataset(
+        name='x/rotation_speed',
+        value=1.0,
+        shape=None,
+        dtype=float,
+        parent=group,
+        attrs={'units': units},
+    )
+    assert chexus.validators.chopper_frequency_units_invalid().applies_to(group)
+    result = chexus.validators.chopper_frequency_units_invalid().validate(group)
+    if good:
+        assert result is None
+    else:
+        assert isinstance(result, chexus.Violation)
+        assert result.name == 'x'
```

### Comparing `chexus-23.12.0/tox.ini` & `chexus-24.4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 [testenv:nightly]
 deps = -r requirements/nightly.txt
 commands = pytest
 
 [testenv:unpinned]
 description = Test with unpinned dependencies, as a user would install now.
 deps =
+  -r requirements/basetest.txt
   chexus
-  pytest
 commands = pytest
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
 deps = -r requirements/docs.txt
 allowlist_externals=find
 commands = python -m sphinx -j2 -v -b html -d {toxworkdir}/docs_doctrees docs html
@@ -59,9 +59,9 @@
 [testenv:deps]
 description = Update dependencies by running pip-compile-multi
 deps =
   pip-compile-multi
   tomli
 skip_install = true
 changedir = requirements
-commands = python ./make_base.py
+commands = python ./make_base.py --nightly scipp
            pip-compile-multi -d . --backtracking
```

