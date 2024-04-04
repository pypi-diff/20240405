# Comparing `tmp/qbraid-core-0.1.0.dev3.tar.gz` & `tmp/qbraid-core-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.0.dev3.tar", last modified: Tue Apr  2 21:39:00 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.0.dev4.tar", last modified: Thu Apr  4 23:09:23 2024, max compression
```

## Comparing `qbraid-core-0.1.0.dev3.tar` & `qbraid-core-0.1.0.dev4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.993282 qbraid-core-0.1.0.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.993282 qbraid-core-0.1.0.dev3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.993282 qbraid-core-0.1.0.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.993282 qbraid-core-0.1.0.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.993282 qbraid-core-0.1.0.dev3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.997282 qbraid-core-0.1.0.dev3/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.997282 qbraid-core-0.1.0.dev3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.997282 qbraid-core-0.1.0.dev3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:59.997282 qbraid-core-0.1.0.dev3/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.001282 qbraid-core-0.1.0.dev3/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.001282 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.001282 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.001282 qbraid-core-0.1.0.dev3/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 21:38:59.000000 qbraid-core-0.1.0.dev3/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tests/test_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:39:00.005282 qbraid-core-0.1.0.dev3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-02 21:38:53.000000 qbraid-core-0.1.0.dev3/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.702338 qbraid-core-0.1.0.dev4/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.706338 qbraid-core-0.1.0.dev4/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 23:09:23.000000 qbraid-core-0.1.0.dev4/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:09:23.714338 qbraid-core-0.1.0.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:09:23.710338 qbraid-core-0.1.0.dev4/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-04 23:09:16.000000 qbraid-core-0.1.0.dev4/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.0.dev4/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/workflows/docs.yml` & `qbraid-core-0.1.0.dev4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/workflows/format.yml` & `qbraid-core-0.1.0.dev4/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/workflows/main.yml` & `qbraid-core-0.1.0.dev4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/workflows/publish.yml` & `qbraid-core-0.1.0.dev4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.github/workflows/test-publish.yml` & `qbraid-core-0.1.0.dev4/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/.gitignore` & `qbraid-core-0.1.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/LICENSE` & `qbraid-core-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/PKG-INFO` & `qbraid-core-0.1.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -76,14 +76,16 @@
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
 
 ```python
 >>> from qbraid_core import QbraidSession
 >>> session = QbraidSession(api_key='API_KEY')
 >>> session.save_config()
+>>> session.get_available_services()
+['environments', 'quantum']
 ```
 
 Other credential configuration methods can be found [here](https://docs.qbraid.com/projects/cli/en/latest/tree/qbraid_configure.html).
 
 ### Verify setup
 
 After configuring your qBraid credentials, verify your setup by running the following from a Python interpreter:
```

### Comparing `qbraid-core-0.1.0.dev3/README.md` & `qbraid-core-0.1.0.dev4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
 
 ```python
 >>> from qbraid_core import QbraidSession
 >>> session = QbraidSession(api_key='API_KEY')
 >>> session.save_config()
+>>> session.get_available_services()
+['environments', 'quantum']
 ```
 
 Other credential configuration methods can be found [here](https://docs.qbraid.com/projects/cli/en/latest/tree/qbraid_configure.html).
 
 ### Verify setup
 
 After configuring your qBraid credentials, verify your setup by running the following from a Python interpreter:
```

### Comparing `qbraid-core-0.1.0.dev3/docs/Makefile` & `qbraid-core-0.1.0.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.0.dev4/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/cards/python.png` & `qbraid-core-0.1.0.dev4/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/cards/terminal.png` & `qbraid-core-0.1.0.dev4/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/css/custom.css` & `qbraid-core-0.1.0.dev4/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.0.dev4/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/favicon.ico` & `qbraid-core-0.1.0.dev4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/_static/logo.png` & `qbraid-core-0.1.0.dev4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/conf.py` & `qbraid-core-0.1.0.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/index.rst` & `qbraid-core-0.1.0.dev4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/docs/make.bat` & `qbraid-core-0.1.0.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/pyproject.toml` & `qbraid-core-0.1.0.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.0.dev3"
+version = "0.1.0.dev4"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["qbraid", "quantum", "cloud"]
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/__init__.py` & `qbraid-core-0.1.0.dev4/qbraid_core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,44 +20,48 @@
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    client
-   register_client
-   discover_services
    setup_default_session
 
 Exceptions
 ------------
 
 .. autosummary::
    :toctree: ../stubs/
 
    QbraidException
    AuthError
    ConfigError
    RequestsApiError
+   ResourceNotFoundError
+   UserNotFoundError
 
 """
-from ._warnings import _check_version, _disable_urllib3
 from .client import QbraidClient
 from .exceptions import (
     AuthError,
     ConfigError,
     QbraidException,
     RequestsApiError,
     ResourceNotFoundError,
     UserNotFoundError,
 )
-from .registry import discover_services, register_client
 from .retry import PostForcelistRetry
 from .session import QbraidSession
 
+try:
+    # Injected in _version.py during the build process.
+    from ._version import __version__
+except ImportError:
+    __version__ = ""
+
 # Hold the default session in a global variable, but don't initialize it yet.
 _DEFAULT_SESSION = None
 
 
 def setup_default_session(**kwargs):
     """
     Set up a default session, passing through any parameters to the session
@@ -100,12 +104,25 @@
         service_name (str): The name of the service for which to create the client.
         **kwargs: Keyword arguments for session customization, used only if creating
                   a new default session.
 
     Returns:
         A service client instance.
     """
-    return _get_default_session().client(*args, **kwargs)
-
-
-_disable_urllib3()
-_check_version("qbraid-core")
+    session = _get_default_session()
+    _ = session.get_available_services()  # Ensure the session is initialized
+    return session.client(*args, **kwargs)
+
+
+__all__ = [
+    "QbraidClient",
+    "QbraidSession",
+    "PostForcelistRetry",
+    "client",
+    "setup_default_session",
+    "QbraidException",
+    "AuthError",
+    "ConfigError",
+    "RequestsApiError",
+    "ResourceNotFoundError",
+    "UserNotFoundError",
+]
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/_warnings.py` & `qbraid-core-0.1.0.dev4/qbraid_core/_compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,38 @@
 
 """
 Module for emitting and disabling warnings at top level.
 
 """
 import warnings
 
-import urllib3
-
 from .exceptions import QbraidException
 from .system import get_latest_package_version, get_local_package_version
 
 
 def _warn_new_version(local: str, latest: str) -> bool:
     """Returns True if you should warn user about updated package version,
     False otherwise."""
+    if not local or not latest:
+        return False
+
     installed_major, installed_minor = map(int, local.split(".")[:2])
     latest_major, latest_minor = map(int, latest.split(".")[:2])
 
     return (installed_major, installed_minor) < (latest_major, latest_minor)
 
 
-def _check_version(package: str) -> None:
+def check_version(package: str) -> None:
     """Emits UserWarning if updated package version exists."""
     try:
         latest_version = get_latest_package_version(package)
         local_version = get_local_package_version(package)
 
         if _warn_new_version(local_version, latest_version):
             warnings.warn(
                 f"You are using {package} version {local_version}, however, version "
                 f"{latest_version} is available. To avoid compatibility issues, consider "
                 "upgrading.",
                 UserWarning,
             )
     except QbraidException:
         pass
-
-
-# coverage: ignore
-def _disable_urllib3() -> None:
-    """Disables urllib3 InsecureRequestWarning warning."""
-    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/client.py` & `qbraid-core-0.1.0.dev4/qbraid_core/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 
 """
 import datetime
 import os
 import re
 from typing import Optional
 
+from ._compat import check_version
 from .exceptions import AuthError, RequestsApiError, ResourceNotFoundError, UserNotFoundError
 from .session import QbraidSession
 
 
 class QbraidClient:
     """Base class for qBraid micro-service clients."""
 
     def __init__(self, session: Optional[QbraidSession] = None):
         self.session = session or QbraidSession()
+        check_version("qbraid-core")
 
     @property
     def session(self) -> QbraidSession:
         """The QbraidSession used to make requests."""
         return self._session
 
     @session.setter
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/exceptions.py` & `qbraid-core-0.1.0.dev4/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/registry.py` & `qbraid-core-0.1.0.dev4/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/retry.py` & `qbraid-core-0.1.0.dev4/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/create.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from pathlib import Path
 from typing import Union
 
 from qbraid_core.system import replace_str
 
 from .state import update_install_status
 
-logging.basicConfig(
-    level=logging.ERROR,
-    format="%(asctime)s - %(levelname)s - %(message)s",
-)
+logger = logging.getLogger(__name__)
 
 
 def create_local_venv(slug_path: Union[str, Path], prompt: str) -> None:
     """Create virtual environment and swap PS1 display name."""
     try:
         # Ensure slug_path is a Path object
         slug_path = Path(slug_path)
@@ -39,9 +36,9 @@
 
         for file in activate_files:
             file_path = scripts_path / file
             replace_str("(pyenv)", f"({prompt})", str(file_path))
 
         update_install_status(slug_path, 1, 1)
     except Exception as err:  # pylint: disable=broad-exception-caught
-        logging.error("Error creating virtual environment: %s", err)
+        logger.error("Error creating virtual environment: %s", err)
         update_install_status(slug_path, 1, 0, message=str(err))
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
 from qbraid_core.system import is_valid_python
 
 from .validate import is_valid_slug
 
-logging.basicConfig(
-    level=logging.ERROR,
-    format="%(asctime)s - %(levelname)s - %(message)s",
-)
+logger = logging.getLogger(__name__)
 
 
 def get_default_envs_paths() -> List[Path]:
     """
     Returns a list of paths to qBraid environments.
 
     If the QBRAID_ENVS_PATH environment variable is set, it splits the variable by ':' to
@@ -95,15 +92,15 @@
         if sys.platform == "win32":
             python_path = slug_path.joinpath("pyenv", "Scripts", "python.exe")
         else:
             python_path = slug_path.joinpath("pyenv", "bin", "python")
         if is_valid_python(python_path):
             return str(python_path)
     except Exception as err:  # pylint: disable=broad-exception-caught
-        logging.error("Error determining Python path: %s", err)
+        logger.error("Error determining Python path: %s", err)
 
     return sys.executable
 
 
 def installed_envs_data() -> Tuple[Dict[str, Path], Dict[str, str]]:
     """Gather paths and aliases for all installed qBraid environments."""
     installed = {}
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,45 +9,42 @@
 import json
 import logging
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from .paths import get_env_path
 
-logging.basicConfig(
-    level=logging.ERROR,
-    format="%(asctime)s - %(levelname)s - %(message)s",
-)
+logger = logging.getLogger(__name__)
 
 
 def install_status_codes(slug: str) -> Dict[str, Union[int, str]]:
     """Return environment's install status codes."""
 
     def read_from_json(file_path: Path) -> Dict[str, Union[int, str]]:
         try:
             with file_path.open("r", encoding="utf-8") as file:
                 json_data = json.load(file)
                 return json_data.get("install", {})
         except (IOError, json.JSONDecodeError) as err:
-            logging.error("Error reading state.json: %s", err)
+            logger.error("Error reading state.json: %s", err)
             return {}
 
     def read_from_txt(file_path: Path) -> Dict[str, Union[int, str]]:
         data = {}
         try:
             with file_path.open("r", encoding="utf-8") as file:
                 lines = file.readlines()
                 for line in lines:
                     key, value = line.split(":", 1)
                     if key in ["complete", "success"]:
                         data[key] = int(value.strip())
                     elif key == "message":
                         data[key] = value.strip()
         except IOError as err:
-            logging.error("Error reading install_status.txt: %s", err)
+            logger.error("Error reading install_status.txt: %s", err)
         return data
 
     slug_path = get_env_path(slug)
     status_json_path = slug_path / "state.json"
     status_txt_path = slug_path / "install_status.txt"
 
     data = {"complete": 1, "success": 1, "message": ""}
@@ -79,15 +76,15 @@
         # r+ mode for reading and writing
         with state_json_path.open("r+", encoding="utf-8") as file:
             try:
                 data = json.load(file)
                 file.seek(0)  # Reset file position to the beginning
             except json.JSONDecodeError as err:
                 # Keep default data if JSON is invalid
-                logging.error("Error opening state.json: %s", err)
+                logger.error("Error opening state.json: %s", err)
 
             # Update the data
             data["install"]["complete"] = complete
             data["install"]["success"] = success
             data["install"]["message"] = message
 
             # Write updated data back to state.json
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.0.dev4/qbraid_core/services/quantum/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
 from qbraid_core.system import get_active_site_packages_path, get_venv_site_packages_path
 
 from .exceptions import QbraidException
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 SUPPORTED_QJOB_LIBS = ["braket"]
 
 
 def _check_proxy(
     proxy_spec: Tuple[str, ...], slug_path: Optional[Path] = None
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/session.py` & `qbraid-core-0.1.0.dev4/qbraid_core/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 
 """
 import configparser
 import logging
 import os
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
+import urllib3
 from requests import RequestException, Response, Session
 from requests.adapters import HTTPAdapter
 
 from .exceptions import AuthError, ConfigError, RequestsApiError, UserNotFoundError
 from .registry import client_registry, discover_services
 from .retry import STATUS_FORCELIST, PostForcelistRetry
 
 if TYPE_CHECKING:
     import qbraid_core
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 DEFAULT_ENDPOINT_URL = "https://api.qbraid.com/api"
 DEFAULT_CONFIG_PATH = os.path.join(os.path.expanduser("~"), ".qbraid", "qbraidrc")
 DEFAULT_CONFIG_SECTION = "default"
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
 
 class QbraidSession(Session):  # pylint: disable=too-many-instance-attributes
     """Custom session with handling of request urls and authentication.
 
     This is a child class of :py:class:`requests.Session`. It handles qbraid
     authentication with custom headers, has SSL verification disabled
     for compatibility with lab, and returns all responses as jsons for
@@ -254,16 +256,16 @@
             service_name: Name of the service.
 
         Returns:
             qbraid_core.QbraidClient: Client for the specified service.
         """
         client_class = client_registry.get(service_name)
         if not client_class:
-            raise ValueError(f"Service {service_name} not registered")
-        return client_class(sessin=self)
+            raise ValueError(f"Service '{service_name}' not registered")
+        return client_class(session=self)
 
     def _initialize_retry(
         self, retries_total: int, retries_connect: int, backoff_factor: float
     ) -> None:
         """Set the session retry policy.
 
         Args:
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/system/__init__.py` & `qbraid-core-0.1.0.dev4/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/system/executables.py` & `qbraid-core-0.1.0.dev4/qbraid_core/system/executables.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import shutil
 import stat
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def is_exe(fpath: Union[str, Path]) -> bool:
     """
     Return true if fpath is a file we have access to that is executable.
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/system/generic.py` & `qbraid-core-0.1.0.dev4/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/system/packages.py` & `qbraid-core-0.1.0.dev4/qbraid_core/system/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pathlib import Path
 
 import requests
 
 from .exceptions import QbraidSystemError
 from .executables import get_python_version_from_cfg, get_python_version_from_exe
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def get_venv_site_packages_path(venv_path: Path) -> Path:
     """
     Determines the site-packages directory for a given virtual environment in an OS-agnostic manner.
     Automatically selects the Python version if a single version is present in the 'lib' directory.
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core/system/threader.py` & `qbraid-core-0.1.0.dev4/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.0.dev4/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -76,14 +76,16 @@
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
 
 ```python
 >>> from qbraid_core import QbraidSession
 >>> session = QbraidSession(api_key='API_KEY')
 >>> session.save_config()
+>>> session.get_available_services()
+['environments', 'quantum']
 ```
 
 Other credential configuration methods can be found [here](https://docs.qbraid.com/projects/cli/en/latest/tree/qbraid_configure.html).
 
 ### Verify setup
 
 After configuring your qBraid credentials, verify your setup by running the following from a Python interpreter:
```

### Comparing `qbraid-core-0.1.0.dev3/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.0.dev4/qbraid_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 docs/_static/cards/terminal.png
 docs/_static/css/custom.css
 docs/_static/css/s4defs-roles.css
 docs/api/qbraid_core.rst
 docs/api/qbraid_core.services.rst
 docs/api/qbraid_core.system.rst
 qbraid_core/__init__.py
+qbraid_core/_compat.py
 qbraid_core/_version.py
-qbraid_core/_warnings.py
 qbraid_core/client.py
 qbraid_core/exceptions.py
 qbraid_core/registry.py
 qbraid_core/retry.py
 qbraid_core/session.py
 qbraid_core.egg-info/PKG-INFO
 qbraid_core.egg-info/SOURCES.txt
@@ -57,14 +57,14 @@
 qbraid_core/system/executables.py
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 tests/__init__.py
 tests/conftest.py
 tests/test_client.py
+tests/test_compat.py
 tests/test_environments.py
 tests/test_session.py
 tests/test_system.py
-tests/test_warnings.py
 tests/fixtures/__init__.py
 tests/fixtures/environments.py
 tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.0.dev3/tests/fixtures/environments.py` & `qbraid-core-0.1.0.dev4/tests/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/tests/test_client.py` & `qbraid-core-0.1.0.dev4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/tests/test_environments.py` & `qbraid-core-0.1.0.dev4/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/tests/test_session.py` & `qbraid-core-0.1.0.dev4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/tests/test_system.py` & `qbraid-core-0.1.0.dev4/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev3/tests/test_warnings.py` & `qbraid-core-0.1.0.dev4/tests/test_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 Unit tests related to qBraid core functionality and system configurations.
 
 """
 import pytest
 
-from qbraid_core._warnings import _warn_new_version
+from qbraid_core._compat import _warn_new_version
 
 check_version_data = [
     # local, API, warn
     ("0.1.0", "0.1.1", False),
     ("1.0.7", "1.0.8", False),
     ("1.3.2", "2.0.6", True),
     ("0.1.0", "0.3.0", True),
```

### Comparing `qbraid-core-0.1.0.dev3/tools/verify_headers.py` & `qbraid-core-0.1.0.dev4/tools/verify_headers.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,110 +5,150 @@
 
 """
 Script to verify qBraid copyright file headers
 
 """
 import os
 import sys
+from typing import List, Optional
 
 # ANSI escape codes
 BLUE = "\033[94m"
 BOLD = "\033[1m"
 RESET = "\033[0m"
 
-header = """# Copyright (c) 2024, qBraid Development Team
+DEFAULT_HEADER = """# Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 """
 
-header_gpl = """# Copyright (C) 2024 qBraid
+DEFAULT_HEADER_GPL = """# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 """
 
-header_2023 = header.replace("2024", "2023")
-header_gpl_2023 = header_gpl.replace("2024", "2023")
-
-skip_files = ["qbraid_core/_version.py"]
-
-failed_headers = []
-fixed_headers = []
 
+def verify_headers(
+    src_paths: List[str],
+    header_type: str = "default",
+    skip_files: Optional[List[str]] = None,
+    fix: bool = False,
+) -> None:
+    if header_type == "default":
+        header = DEFAULT_HEADER
+    elif header_type == "gpl":
+        header = DEFAULT_HEADER_GPL
+    else:
+        raise ValueError("Invalid header type")
 
-def should_skip(file_path: str, content: str) -> bool:
-    if file_path in skip_files:
-        return True
+    header_2023 = header.replace("2024", "2023")
 
-    if os.path.basename(file_path) == "__init__.py":
-        return not content.strip()
+    skip_files = skip_files or []
 
-    skip_header_tag = "# qbraid: skip-header"
-    line_number = 0
+    failed_headers = []
+    fixed_headers = []
 
-    for line in content.splitlines():
-        line_number += 1
-        if 5 <= line_number <= 30 and skip_header_tag in line:
+    def should_skip(file_path: str, content: str) -> bool:
+        if file_path in skip_files:
             return True
-        if line_number > 30:
-            break
 
-    return False
+        if os.path.basename(file_path) == "__init__.py":
+            return not content.strip()
 
+        skip_header_tag = "# qbraid: skip-header"
+        line_number = 0
 
-def replace_or_add_header(file_path: str, fix: bool = False) -> None:
-    with open(file_path, "r", encoding="ISO-8859-1") as f:
-        content = f.read()
-
-    if (
-        content.startswith(header)
-        or content.startswith(header_2023)
-        or content.startswith(header_gpl)
-        or content.startswith(header_gpl_2023)
-        or should_skip(file_path, content)
-    ):
-        return
+        for line in content.splitlines():
+            line_number += 1
+            if 5 <= line_number <= 30 and skip_header_tag in line:
+                return True
+            if line_number > 30:
+                break
+
+        return False
+
+    def replace_or_add_header(file_path: str, fix: bool = False) -> None:
+        with open(file_path, "r", encoding="ISO-8859-1") as f:
+            content = f.read()
+
+        if (
+            content.startswith(header)
+            or content.startswith(header_2023)
+            or should_skip(file_path, content)
+        ):
+            return
+
+        if not fix:
+            failed_headers.append(file_path)
+            return
+
+        # Add or replace the header
+        lines = content.splitlines()
+        first_non_comment_line_index = next(
+            (i for i, line in enumerate(lines) if not line.strip().startswith("#")), None
+        )
+
+        new_content_lines = [header.rstrip("\r\n")] + (
+            lines[first_non_comment_line_index:] if first_non_comment_line_index is not None else []
+        )
+        new_content = "\n".join(new_content_lines) + "\n"
 
-    if not fix:
-        failed_headers.append(file_path)
+        with open(file_path, "w", encoding="ISO-8859-1") as f:
+            f.write(new_content)
+
+        fixed_headers.append(file_path)
         return
 
-    lines = content.splitlines()
+    def process_files_in_directory(directory: str, fix: bool = False) -> int:
+        count = 0
+        if not os.path.isdir(directory):
+            return count
+        for root, _, files in os.walk(directory):
+            for file in files:
+                if file.endswith(".py"):
+                    file_path = os.path.join(root, file)
+                    replace_or_add_header(file_path, fix)
+                    count += 1
+        return count
 
-    comment_lines = []
-    first_skipped_line = None
-    for index, line in enumerate(lines):
-        if line.startswith("#"):
-            comment_lines.append(line)
+    checked = 0
+    for item in src_paths:
+        if os.path.isdir(item):
+            checked += process_files_in_directory(item, fix)
+        elif os.path.isfile(item) and item.endswith(".py"):
+            replace_or_add_header(item, fix)
+            checked += 1
         else:
-            first_skipped_line = index
-            break
-
-    new_content_lines = [header.rstrip("\r\n")] + lines[first_skipped_line:]
-    new_content = "\n".join(new_content_lines) + "\n"
+            failed_headers.append(item)
+            print(f"Directory not found: {item}")
 
-    with open(file_path, "w", encoding="ISO-8859-1") as f:
-        f.write(new_content)
+    if not fix:
+        if failed_headers:
+            for file in failed_headers:
+                print(f"failed {os.path.relpath(file)}")
+            num_failed = len(failed_headers)
+            s1, s2 = ("", "s") if num_failed == 1 else ("s", "")
+            sys.stderr.write(f"\n{num_failed} file header{s1} need{s2} updating.\n")
+        else:
+            print("All file header checks passed!")
 
-    fixed_headers.append(file_path)
-
-
-def process_files_in_directory(directory: str, fix: bool = False) -> int:
-    count = 0
-    for root, _, files in os.walk(directory):
-        for file in files:
-            if file.endswith(".py"):
-                file_path = os.path.join(root, file)
-                replace_or_add_header(file_path, fix)
-                count += 1
-    return count
+    else:
+        for file in fixed_headers:
+            print(f"fixed {os.path.relpath(file)}")
+        num_fixed = len(fixed_headers)
+        num_ok = checked - num_fixed
+        s_fixed = "" if num_fixed == 1 else "s"
+        s_ok = "" if num_ok == 1 else "s"
+        print("\nAll done! ✨ 🚀 ✨")
+        print(f"{num_fixed} header{s_fixed} fixed, {num_ok} header{s_ok} left unchanged.")
 
 
 def display_help() -> None:
     help_message = """
     Usage: python verify_headers.py SRC [OPTIONS] ...
 
     This script checks for copyright headers at the specified path.
@@ -128,46 +168,15 @@
         display_help()
 
     # Check if at least two arguments are provided and the first argument is not a flag
     if len(sys.argv) < 2 or sys.argv[1].startswith("--"):
         print("Usage: python verify_headers.py SRC [OPTIONS] ...")
         sys.exit(1)
 
+    skip_files = ["qbraid_core/_version.py"]
     script_directory = os.path.dirname(os.path.abspath(__file__))
     project_directory = os.path.abspath(os.path.join(script_directory, ".."))
     skip_files = [os.path.join(project_directory, file_path) for file_path in skip_files]
 
     fix = "--fix" in sys.argv
     files_and_dirs = [arg for arg in sys.argv[1:] if arg != "--fix"]
-
-    checked = 0
-    for item in files_and_dirs:
-        full_path = os.path.join(project_directory, item)
-        if os.path.isdir(full_path):
-            checked += process_files_in_directory(full_path, fix)
-        elif os.path.isfile(full_path) and full_path.endswith(".py"):
-            replace_or_add_header(full_path, fix)
-            checked += 1
-        else:
-            failed_headers.append(full_path)
-            print(f"Directory not found: {full_path}")
-
-    if not fix:
-        if failed_headers:
-            for file in failed_headers:
-                print(f"failed {os.path.relpath(file)}")
-            num_failed = len(failed_headers)
-            s1, s2 = ("", "s") if num_failed == 1 else ("s", "")
-            sys.stderr.write(f"\n{num_failed} file header{s1} need{s2} updating.\n")
-            sys.exit(1)
-        else:
-            print("All file header checks passed!")
-
-    else:
-        for file in fixed_headers:
-            print(f"fixed {os.path.relpath(file)}")
-        num_fixed = len(fixed_headers)
-        num_ok = checked - num_fixed
-        s_fixed = "" if num_fixed == 1 else "s"
-        s_ok = "" if num_ok == 1 else "s"
-        print("\nAll done! ✨ 🚀 ✨")
-        print(f"{num_fixed} header{s_fixed} fixed, {num_ok} header{s_ok} left unchanged.")
+    verify_headers(files_and_dirs, fix=fix, skip_files=skip_files)
```

