# Comparing `tmp/iam-sarif-report-2.3.1.tar.gz` & `tmp/iam-sarif-report-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam-sarif-report-2.3.1.tar", last modified: Wed Feb 28 19:41:33 2024, max compression
+gzip compressed data, was "iam-sarif-report-2.3.2.tar", last modified: Thu Apr  4 22:10:30 2024, max compression
```

## Comparing `iam-sarif-report-2.3.1.tar` & `iam-sarif-report-2.3.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.941819 iam-sarif-report-2.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.933819 iam-sarif-report-2.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.933819 iam-sarif-report-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.github/workflows/maintenance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-28 19:41:33.941819 iam-sarif-report-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/action.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.933819 iam-sarif-report-2.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.933819 iam-sarif-report-2.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      383 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/scripts/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2083 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/scripts/scrape_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 19:41:33.941819 iam-sarif-report-2.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.929819 iam-sarif-report-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.933819 iam-sarif-report-2.3.1/src/iam_sarif_report/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)   188967 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/checks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/src/iam_sarif_report/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/domain/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/domain/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/domain/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/src/iam_sarif_report/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/entrypoints/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/src/iam_sarif_report/service_layer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/service_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/service_layer/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/src/iam_sarif_report/service_layer/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-28 19:41:33.000000 iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.929819 iam-sarif-report-2.3.1/tests/data/policy_checks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/tests/data/policy_checks/findings/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/findings/arn-region-not-allowed.json
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/findings/redundant-action.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/tests/data/policy_checks/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/policies/arn-region-not-allowed.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/policies/redundant-action.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:41:33.937819 iam-sarif-report-2.3.1/tests/data/policy_checks/sarif/
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/sarif/arn-region-not-allowed.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/policy_checks/sarif/redundant-action.sarif
--rw-r--r--   0 runner    (1001) docker     (127)   115632 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/data/sarif-schema-2.1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-28 19:41:25.000000 iam-sarif-report-2.3.1/tests/test_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.598010 iam-sarif-report-2.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.598010 iam-sarif-report-2.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.github/workflows/maintenance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/action.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.598010 iam-sarif-report-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.598010 iam-sarif-report-2.3.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      383 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/scripts/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2083 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/scripts/scrape_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.594010 iam-sarif-report-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.598010 iam-sarif-report-2.3.2/src/iam_sarif_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189001 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/checks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/src/iam_sarif_report/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/domain/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/domain/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/domain/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/src/iam_sarif_report/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/entrypoints/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/src/iam_sarif_report/service_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/service_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/service_layer/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/src/iam_sarif_report/service_layer/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 22:10:30.000000 iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.594010 iam-sarif-report-2.3.2/tests/data/policy_checks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.602010 iam-sarif-report-2.3.2/tests/data/policy_checks/findings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/findings/arn-region-not-allowed.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/findings/redundant-action.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/tests/data/policy_checks/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/policies/arn-region-not-allowed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/policies/redundant-action.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:10:30.606010 iam-sarif-report-2.3.2/tests/data/policy_checks/sarif/
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/sarif/arn-region-not-allowed.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/policy_checks/sarif/redundant-action.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)   115632 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/data/sarif-schema-2.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-04 22:10:26.000000 iam-sarif-report-2.3.2/tests/test_converter.py
```

### Comparing `iam-sarif-report-2.3.1/.github/workflows/cd.yml` & `iam-sarif-report-2.3.2/.github/workflows/cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     name: Deploy Documentation
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: 3.x
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install '.[docs]'
       - run: mkdocs gh-deploy --force
 
   update-major-tag:
@@ -60,11 +60,11 @@
     environment: main
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
-      - uses: pypa/gh-action-pypi-publish@v1.8.11
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `iam-sarif-report-2.3.1/.github/workflows/ci.yml` & `iam-sarif-report-2.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/.github/workflows/maintenance.yaml` & `iam-sarif-report-2.3.2/.github/workflows/maintenance.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
           cache: pip
           cache-dependency-path: pyproject.toml
       - run: pip install --upgrade --no-input '.[scraper]'
       - run: cd scripts && ./scrape_checks.py
-      - uses: peter-evans/create-pull-request@v5
+      - uses: peter-evans/create-pull-request@v6
         with:
           title: '[:wrench:] Automated Checks Update'
           commit-message: Updates Access Analyzer checks
           body: |
             - Updates checks
 
             Auto Generated PullRequest updates checks
```

### Comparing `iam-sarif-report-2.3.1/.gitignore` & `iam-sarif-report-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/LICENSE` & `iam-sarif-report-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/PKG-INFO` & `iam-sarif-report-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-sarif-report
-Version: 2.3.1
+Version: 2.3.2
 Author-email: George Alton <georgealton@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 George Alton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,15 +38,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0
 Requires-Dist: click==8.1.7
 Requires-Dist: punq==0.7.0
-Requires-Dist: boto3==1.34.23
+Requires-Dist: boto3==1.34.74
 Requires-Dist: sarif_om==1.0.4
 Requires-Dist: jschema_to_python==1.2.3
 Requires-Dist: typing_extensions==4.1.1; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `iam-sarif-report-2.3.1/README.md` & `iam-sarif-report-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/action.yaml` & `iam-sarif-report-2.3.2/action.yaml`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/pyproject.toml` & `iam-sarif-report-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 dependencies = [
   "attrs==23.2.0",
   "click==8.1.7",
   "punq==0.7.0",
-  "boto3==1.34.23",
+  "boto3==1.34.74",
   "sarif_om==1.0.4",
   "jschema_to_python==1.2.3",
   "typing_extensions==4.1.1; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `iam-sarif-report-2.3.1/scripts/scrape_checks.py` & `iam-sarif-report-2.3.2/scripts/scrape_checks.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/checks.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/checks.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/reporter.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/reporter.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/adapters/validator.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/adapters/validator.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/bootstrap.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/bootstrap.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/checks.json` & `iam-sarif-report-2.3.2/src/iam_sarif_report/checks.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990740740740741%*

 * *Differences: {"'error_missing_resource'": "{'short_description': 'All policies except role trust policies must "*

 * *                             "include a `Resource` or\\n`NotResource` element.', 'description': "*

 * *                             "'All policies except role trust policies must include a `Resource` "*

 * *                             'or\\n`NotResource` element.\\n\\n**Related terms**\\n\\n  * '*

 * *                             '[Resource '*

 * *                             'element](./reference_policies_elements_resource.htm […]*

```diff
@@ -260,17 +260,17 @@
     "error_missing_quote_in_variable": {
         "description": "When you add a variable to your policy, you can specify a default value for\nthe variable. If a variable is not present, AWS uses the default text that you\nprovide.\n\nTo add a default value to a variable, surround the default value with single\nquotes (`' '`), and separate the variable text and the default value with a\ncomma and space (`, `).\n\nFor example, if a principal is tagged with `team=yellow`, they can access the\n``DOC-EXAMPLE-BUCKET`` Amazon S3 bucket with the name ``DOC-EXAMPLE-\nBUCKET`-yellow`. A policy with this resource might allow team members to\naccess their own resources, but not those of other teams. For users without\nteam tags, you might set a default value of `company-wide`. These users can\naccess only the ``DOC-EXAMPLE-BUCKET`-company-wide` bucket where they can view\nbroad information, such as instructions for joining a team.\n\n    \n    \n    \"Resource\":\"arn:aws:s3:::DOC-EXAMPLE-BUCKET-${aws:PrincipalTag/team, 'company-wide'}\"\n\n**Related terms**\n\n  * [IAM policy elements: Variables](./reference_policies_variables.html)",
         "name": "MissingQuoteInVariable",
         "short_description": "When you add a variable to your policy, you can specify a default value for\nthe variable. If a variable is not present, AWS uses the default text that you\nprovide.",
         "url": "https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-reference-policy-checks.html#access-analyzer-reference-policy-checks-error-missing-quote-in-variable"
     },
     "error_missing_resource": {
-        "description": "Identity-based policies must include a `Resource` or `NotResource` element.\n\n**Related terms**\n\n  * [Resource element](./reference_policies_elements_resource.html)\n\n  * [NotResource element](./reference_policies_elements_notresource.html)\n\n  * [Identity-based policies and resource-based policies](./access_policies_identity-vs-resource.html)\n\n  * [Overview of JSON policies](./access_policies.html#access_policies-json)",
+        "description": "All policies except role trust policies must include a `Resource` or\n`NotResource` element.\n\n**Related terms**\n\n  * [Resource element](./reference_policies_elements_resource.html)\n\n  * [NotResource element](./reference_policies_elements_notresource.html)\n\n  * [Identity-based policies and resource-based policies](./access_policies_identity-vs-resource.html)\n\n  * [Overview of JSON policies](./access_policies.html#access_policies-json)",
         "name": "MissingResource",
-        "short_description": "Identity-based policies must include a `Resource` or `NotResource` element.",
+        "short_description": "All policies except role trust policies must include a `Resource` or\n`NotResource` element.",
         "url": "https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-reference-policy-checks.html#access-analyzer-reference-policy-checks-error-missing-resource"
     },
     "error_missing_statement": {
         "description": "A JSON policy must include a statement.\n\n**Related terms**\n\n  * [JSON policy elements](./reference_policies_elements.html)",
         "name": "MissingStatement",
         "short_description": "A JSON policy must include a statement.",
         "url": "https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-reference-policy-checks.html#access-analyzer-reference-policy-checks-error-missing-statement"
```

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/domain/converter.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/domain/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,15 @@
         return to_json(sarif.SarifLog(schema_uri=schema, version=version, runs=[run]))
 
     def get_rules(
         self, results: Iterable[sarif.Result]
     ) -> Iterable[sarif.ReportingDescriptor]:
         matched_rules = {result.rule_id for result in results if result.rule_id}
         for rule_id in matched_rules:
-            check = self.checks_repository.get(rule_id)
-            if check:
+            if check := self.checks_repository.get(rule_id):
                 yield self.check_to_reporting_descriptor(check)
 
     def check_to_reporting_descriptor(self, check: Check) -> sarif.ReportingDescriptor:
         return sarif.ReportingDescriptor(
             id=check.id,
             name=check.name,
             help=sarif.MultiformatMessageString(
```

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/domain/definitions.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/domain/definitions.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/entrypoints/cli.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report/service_layer/handlers.py` & `iam-sarif-report-2.3.2/src/iam_sarif_report/service_layer/handlers.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/PKG-INFO` & `iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-sarif-report
-Version: 2.3.1
+Version: 2.3.2
 Author-email: George Alton <georgealton@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 George Alton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -38,15 +38,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0
 Requires-Dist: click==8.1.7
 Requires-Dist: punq==0.7.0
-Requires-Dist: boto3==1.34.23
+Requires-Dist: boto3==1.34.74
 Requires-Dist: sarif_om==1.0.4
 Requires-Dist: jschema_to_python==1.2.3
 Requires-Dist: typing_extensions==4.1.1; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: nox; extra == "dev"
```

### Comparing `iam-sarif-report-2.3.1/src/iam_sarif_report.egg-info/SOURCES.txt` & `iam-sarif-report-2.3.2/src/iam_sarif_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/conftest.py` & `iam-sarif-report-2.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/data/policy_checks/findings/arn-region-not-allowed.json` & `iam-sarif-report-2.3.2/tests/data/policy_checks/findings/arn-region-not-allowed.json`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/data/policy_checks/findings/redundant-action.json` & `iam-sarif-report-2.3.2/tests/data/policy_checks/findings/redundant-action.json`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/data/policy_checks/sarif/arn-region-not-allowed.sarif` & `iam-sarif-report-2.3.2/tests/data/policy_checks/sarif/arn-region-not-allowed.sarif`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/data/policy_checks/sarif/redundant-action.sarif` & `iam-sarif-report-2.3.2/tests/data/policy_checks/sarif/redundant-action.sarif`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/data/sarif-schema-2.1.0.json` & `iam-sarif-report-2.3.2/tests/data/sarif-schema-2.1.0.json`

 * *Files identical despite different names*

### Comparing `iam-sarif-report-2.3.1/tests/test_converter.py` & `iam-sarif-report-2.3.2/tests/test_converter.py`

 * *Files identical despite different names*

