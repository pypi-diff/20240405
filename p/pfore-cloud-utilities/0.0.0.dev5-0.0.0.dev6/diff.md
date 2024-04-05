# Comparing `tmp/pfore-cloud-utilities-0.0.0.dev5.tar.gz` & `tmp/pfore-cloud-utilities-0.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfore-cloud-utilities-0.0.0.dev5.tar", last modified: Tue Mar 12 16:14:14 2024, max compression
+gzip compressed data, was "pfore-cloud-utilities-0.0.0.dev6.tar", last modified: Fri Apr  5 14:31:22 2024, max compression
```

## Comparing `pfore-cloud-utilities-0.0.0.dev5.tar` & `pfore-cloud-utilities-0.0.0.dev6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.201062 pfore-cloud-utilities-0.0.0.dev5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.205062 pfore-cloud-utilities-0.0.0.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.github/workflows/apply_code_linters.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.github/workflows/test_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1144 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.201062 pfore-cloud-utilities-0.0.0.dev5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/api-src/pfore_cloud_utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/fetching_secrets.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/docs/setting_databricks_connect.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.209062 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/azure_aad_token_generator.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/azure_blob_connector.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/databricks_workspace.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/define.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/singleton.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/azure_aad_token_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/azure_blob_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/databricks_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/define.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-12 16:14:14.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-12 16:14:14.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 16:14:14.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-12 16:14:14.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 16:14:14.000000 pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:14:14.213062 pfore-cloud-utilities-0.0.0.dev5/test/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-12 16:14:03.000000 pfore-cloud-utilities-0.0.0.dev5/test/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.720191 pfore-cloud-utilities-0.0.0.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.724191 pfore-cloud-utilities-0.0.0.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.github/workflows/apply_code_linters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.github/workflows/test_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1290 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.720191 pfore-cloud-utilities-0.0.0.dev6/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/api-src/pfore_cloud_utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/fetching_secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/docs/setting_databricks_connect.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.728191 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/azure_aad_token_generator.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/azure_blob_connector.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/databricks_workspace.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/define.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/singleton.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/azure_aad_token_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/azure_blob_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/databricks_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 14:31:22.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-05 14:31:22.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:31:22.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 14:31:22.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 14:31:22.000000 pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:22.732191 pfore-cloud-utilities-0.0.0.dev6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 14:31:10.000000 pfore-cloud-utilities-0.0.0.dev6/test/test_imports.py
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/.github/workflows/apply_code_linters.yml` & `pfore-cloud-utilities-0.0.0.dev6/.github/workflows/apply_code_linters.yml`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/.github/workflows/build_documentation.yml` & `pfore-cloud-utilities-0.0.0.dev6/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/.github/workflows/publish.yml` & `pfore-cloud-utilities-0.0.0.dev6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/.github/workflows/test_documentation.yml` & `pfore-cloud-utilities-0.0.0.dev6/.github/workflows/test_documentation.yml`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/.pre-commit-config.yaml` & `pfore-cloud-utilities-0.0.0.dev6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/CHANGELOG.rst` & `pfore-cloud-utilities-0.0.0.dev6/CHANGELOG.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 All notable changes to this project will be documented in this file.
 
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.0.0-dev6 (2024-04-05)
+-------------------------------
+
+* Added: full uppercase `Databricks` profiles e.g. `DEFAULT` are now supported.
+
 Version 0.0.0-dev5 (2024-03-12)
 -------------------------------
 
 * Changed: `core.AzureBlobConnector.list_blobs_in_directory()`
   now returns absolute paths instead of blobs basenames
   and do not include parent directory
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/CONTRIBUTING.rst` & `pfore-cloud-utilities-0.0.0.dev6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/PKG-INFO` & `pfore-cloud-utilities-0.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfore-cloud-utilities
-Version: 0.0.0.dev5
+Version: 0.0.0.dev6
 Summary: Provides utility functions for cloud-based workflows.
 Author: BahaEddine Abrougui
 Author-email: bahaeddine.abrougui@lidl.com
 Project-URL: repository, https://github.com/Bahaabrougui/pfore-cloud-utilities/
 Project-URL: documentation, https://bahaabrougui.github.io/pfore-cloud-utilities/index.html/
 Keywords: databricks,azure,mlops
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/README.rst` & `pfore-cloud-utilities-0.0.0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/.DS_Store` & `pfore-cloud-utilities-0.0.0.dev6/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/_templates/autosummary/class.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/authentication.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/conf.py` & `pfore-cloud-utilities-0.0.0.dev6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/fetching_secrets.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/fetching_secrets.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/index.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/install.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/overview.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/docs/setting_databricks_connect.rst` & `pfore-cloud-utilities-0.0.0.dev6/docs/setting_databricks_connect.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Setting up databricks-connect
 =============================
 
 To run code remotely on a databricks cluster, we'll use databricks-connect_
 package.
 
-It is important to note that development on clusters of versions `13.0` requires
-`Unity Catalog`_. This guide will cover legacy workspaces, on which
+It is important to note that development on clusters of versions `13.0`
+requires `Unity Catalog`_. This guide will cover legacy workspaces, on which
 `Unity Catalog`_ is not activated, therefore only clusters of versions `12.*`.
 
-The first step would be to create a :file:`databricks-connect` file under your
+The first step would be to create a :file:`.databricks-connect` file under your
 home directory. The file will have the following structure:
 
 .. code-block:: cfg
 
     {
       "host": "<link-to-databricks-workspace",
       "token": "<your-personal-access-token",
       "cluster_id": "<id-to-your-cluster>",
       "org_id": "<org-id>",
       "port": "<cluster-port, default is 15001>"
     }
 
+**Note**: It is possible to create the file manually and copy-paste the above
+content, or you can also run the command `databricks-connect configure`,
+this will prompts to fill in the host, token and other attributes and then will
+automatically creates and saves the file under the home directory.
+
 Both `cluster_id` and `org_id` can be fetched from the cluster url. When you
 click on a cluster from the databricks UI, the url will look like:
 :file:`https://<host>/?o=<org-id>#setting/clusters/<cluster-id>/`
 where the string after **?o=** is the **org_id** and the string
 after **/clusters/** is the **cluster_id**.
 
 Once the file is set up, you'll have to create a virtual env with a python
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/__init__.py` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/__pycache__/__init__.cpython-39.pyc` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/azure_aad_token_generator.cpython-39.pyc` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/azure_aad_token_generator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/azure_blob_connector.cpython-39.pyc` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/azure_blob_connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/databricks_workspace.cpython-39.pyc` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/databricks_workspace.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/__pycache__/singleton.cpython-39.pyc` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/__pycache__/singleton.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/azure_aad_token_generator.py` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/azure_aad_token_generator.py`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/azure_blob_connector.py` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/azure_blob_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import io
-import typing
+from typing import IO
+from typing import AnyStr
+from typing import Iterable
+from typing import List
+from typing import Union
 
 from azure.core.exceptions import ResourceExistsError
 from azure.identity import ClientSecretCredential
 from azure.identity import DefaultAzureCredential
 from azure.storage.blob import BlobServiceClient
 from azure.storage.blob import ContainerClient
 
@@ -61,15 +65,20 @@
             )
         self._blob_service_client = BlobServiceClient(
             account_url=self._account_url,
             credential=credentials,
             logging_enable=True,
         )
 
-    def upload(self, contents: bytes, container_name: str, path: str) -> None:
+    def upload(
+            self,
+            contents: Union[bytes, str, Iterable[AnyStr], IO[AnyStr]],
+            container_name: str,
+            path: str,
+            ) -> None:
         """Uploads content in bytes to a blob container.
 
         Args:
             contents: Contents to upload, in bytes
             container_name: Name of the blob container, if it doesn't
                 exist it will be created as long as permission scope allows it
             path: Blob path to write to
@@ -104,15 +113,15 @@
             bytes_io_obj.seek(0)
             return bytes_io_obj.read()
 
     def list_blobs_in_directory(
             self,
             container_name: str,
             path: str,
-    ) -> typing.List[str]:
+    ) -> List[str]:
         """Lists blobs in a subdirectory for a given path in the blob storage.
 
         Args:
             container_name: Name of the blob container
             path: Path to subdirectory
 
         Returns:
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/databricks_workspace.py` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/databricks_workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
-import configparser
 import os
+import re
 
 from databricks.sdk import WorkspaceClient
 
 from .singleton import Singleton
 
 
 class DatabricksWorkspace(metaclass=Singleton):
@@ -24,19 +24,19 @@
     def __init__(self):
         databricks_config_file = f'{os.path.expanduser("~")}/.databrickscfg'
         if not os.path.exists(databricks_config_file):
             raise FileNotFoundError(
                 'Please set up a databricks configuration profile first.'
             )
         # Read configuration file to dynamically fetch profiles
-        config = configparser.ConfigParser()
-        config.read(databricks_config_file)
+        with open(databricks_config_file, 'r') as file:
+            workspaces = re.findall(r'\[([^\]]+)\]', file.read())
         self.workspacesClients = {
             workspace: WorkspaceClient(profile=workspace)
-            for workspace in config.sections()
+            for workspace in workspaces
         }
 
 
 def get_workspace_secret_value(
     secret_key: str,
     workspace: str,
     scope: str,
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities/core/singleton.py` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities/core/singleton.py`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/PKG-INFO` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfore-cloud-utilities
-Version: 0.0.0.dev5
+Version: 0.0.0.dev6
 Summary: Provides utility functions for cloud-based workflows.
 Author: BahaEddine Abrougui
 Author-email: bahaeddine.abrougui@lidl.com
 Project-URL: repository, https://github.com/Bahaabrougui/pfore-cloud-utilities/
 Project-URL: documentation, https://bahaabrougui.github.io/pfore-cloud-utilities/index.html/
 Keywords: databricks,azure,mlops
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pfore_cloud_utilities.egg-info/SOURCES.txt` & `pfore-cloud-utilities-0.0.0.dev6/pfore_cloud_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfore-cloud-utilities-0.0.0.dev5/pyproject.toml` & `pfore-cloud-utilities-0.0.0.dev6/pyproject.toml`

 * *Files identical despite different names*

