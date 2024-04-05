# Comparing `tmp/hipscat-import-0.2.5.tar.gz` & `tmp/hipscat-import-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-import-0.2.5.tar", last modified: Fri Mar  8 21:16:11 2024, max compression
+gzip compressed data, was "hipscat-import-0.2.6.tar", last modified: Fri Apr  5 16:37:36 2024, max compression
```

## Comparing `hipscat-import-0.2.5.tar` & `hipscat-import-0.2.6.tar`

### file list

```diff
@@ -1,276 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.176858 hipscat-import-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.136858 hipscat-import-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.136858 hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.136858 hipscat-import-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-08 21:16:11.176858 hipscat-import-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.136858 hipscat-import-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.136858 hipscat-import-0.2.5/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/arguments.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.140858 hipscat-import-0.2.5/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/panstarrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/sdss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/catalogs/temp_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.140858 hipscat-import-0.2.5/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/guide/dask_on_ray.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.140858 hipscat-import-0.2.5/docs/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/notebooks/unequal_schema.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.140858 hipscat-import-0.2.5/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/neowise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/ps1_detections_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/ps1_otmo_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/sdss_wget.bash
--rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/tic_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 21:16:11.176858 hipscat-import-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.144858 hipscat-import-0.2.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.144858 hipscat-import-0.2.5/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 21:16:10.000000 hipscat-import-0.2.5/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.144858 hipscat-import-0.2.5/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10080 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/catalog/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.144858 hipscat-import-0.2.5/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.144858 hipscat-import-0.2.5/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/src/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/soap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/soap/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/soap/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/soap/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/soap/run_soap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/src/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/verification/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/src/hipscat_import/verification/run_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-08 21:16:11.000000 hipscat-import-0.2.5/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-03-08 21:16:11.000000 hipscat-import-0.2.5/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:16:11.000000 hipscat-import-0.2.5/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-08 21:16:11.000000 hipscat-import-0.2.5/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-08 21:16:11.000000 hipscat-import-0.2.5/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.148858 hipscat-import-0.2.5/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.128858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.128858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.128858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.128858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.152858 hipscat-import-0.2.5/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.156858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.156858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.156858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.156858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.160858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.160858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.160858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.160858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.164858 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.168858 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/0_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/1_47.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_176.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_177.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_178.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_179.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_180.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_181.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_182.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_183.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_184.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_185.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_186.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/2_187.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.132858 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.168858 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/gaia_minimum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/hipscat_index.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/hipscat_index.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/multiindex.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_round_trip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/tests/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/soap/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/soap/test_run_soap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/test_pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/test_runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:16:11.172858 hipscat-import-0.2.5/tests/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/verification/test_run_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-08 21:16:01.000000 hipscat-import-0.2.5/tests/hipscat_import/verification/test_verification_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.556177 hipscat-import-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.556177 hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/arguments.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/panstarrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/sdss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/catalogs/temp_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/guide/dask_on_ray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.560177 hipscat-import-0.2.6/docs/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/notebooks/unequal_schema.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.564177 hipscat-import-0.2.6/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/neowise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/ps1_detections_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/ps1_otmo_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/sdss_wget.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/tic_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.564177 hipscat-import-0.2.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.564177 hipscat-import-0.2.6/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/catalog/run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/src/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/soap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/soap/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/soap/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/soap/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/soap/run_soap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/src/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/verification/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/src/hipscat_import/verification/run_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 16:37:36.000000 hipscat-import-0.2.6/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.568177 hipscat-import-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19177 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.556177 hipscat-import-0.2.6/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.572177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.576177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.580177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.580177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.580177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 16:37:27.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.580177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.584177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.584177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.584177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.552177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.588177 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.588177 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/0_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/1_47.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_176.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_177.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_178.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_179.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_180.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_181.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_182.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_183.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_184.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_185.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_186.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/2_187.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.556177 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.556177 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.592177 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.592177 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/gaia_minimum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/hipscat_index.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/hipscat_index.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/multiindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.592177 hipscat-import-0.2.6/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_round_trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/tests/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/soap/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/soap/test_run_soap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/test_pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:37:36.596177 hipscat-import-0.2.6/tests/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/verification/test_run_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 16:37:28.000000 hipscat-import-0.2.6/tests/hipscat_import/verification/test_verification_arguments.py
```

### Comparing `hipscat-import-0.2.5/.copier-answers.yml` & `hipscat-import-0.2.6/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.gitattributes` & `hipscat-import-0.2.6/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat-import-0.2.6/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/pull_request_template.md` & `hipscat-import-0.2.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/workflows/build-documentation.yml` & `hipscat-import-0.2.6/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/workflows/pre-commit-ci.yml` & `hipscat-import-0.2.6/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/workflows/publish-to-pypi.yml` & `hipscat-import-0.2.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/workflows/smoke-test.yml` & `hipscat-import-0.2.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.github/workflows/testing-and-coverage.yml` & `hipscat-import-0.2.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.gitignore` & `hipscat-import-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.pre-commit-config.yaml` & `hipscat-import-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/.setup_dev.sh` & `hipscat-import-0.2.6/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/LICENSE` & `hipscat-import-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/PKG-INFO` & `hipscat-import-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.2.5
+Version: 0.2.6
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -39,15 +39,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask<=2024.2.0
 Requires-Dist: dask[distributed]
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.2.6
+Requires-Dist: hipscat>=0.2.9
 Requires-Dist: ipykernel
 Requires-Dist: pandas<2.1.0
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: tqdm
 Requires-Dist: numpy<1.25
 Requires-Dist: fsspec<=2024.2.0
@@ -67,14 +67,16 @@
 <img src="https://github.com/lincc-frameworks/tape/blob/main/docs/DARK_Combo_sm.png?raw=true" width="300" height="100">
 
 # hipscat-import
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/hipscat-import?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/hipscat-import/)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/hipscat-import.svg?color=blue&logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/hipscat-import)
+
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/astronomy-commons/hipscat-import/smoke-test.yml)](https://github.com/astronomy-commons/hipscat-import/actions/workflows/smoke-test.yml)
 [![codecov](https://codecov.io/gh/astronomy-commons/hipscat-import/branch/main/graph/badge.svg)](https://codecov.io/gh/astronomy-commons/hipscat-import)
 [![Read the Docs](https://img.shields.io/readthedocs/hipscat-import)](https://hipscat-import.readthedocs.io/)
 
 ## HiPSCat import - Utility for ingesting large survey data into HiPSCat structure.
 
 Check out our [ReadTheDocs site](https://hipscat-import.readthedocs.io/en/latest/)
@@ -87,15 +89,13 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/guide/contributing.html)
 for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
-founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
-Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `hipscat-import-0.2.5/README.md` & `hipscat-import-0.2.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <img src="https://github.com/lincc-frameworks/tape/blob/main/docs/DARK_Combo_sm.png?raw=true" width="300" height="100">
 
 # hipscat-import
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/hipscat-import?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/hipscat-import/)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/hipscat-import.svg?color=blue&logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/hipscat-import)
+
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/astronomy-commons/hipscat-import/smoke-test.yml)](https://github.com/astronomy-commons/hipscat-import/actions/workflows/smoke-test.yml)
 [![codecov](https://codecov.io/gh/astronomy-commons/hipscat-import/branch/main/graph/badge.svg)](https://codecov.io/gh/astronomy-commons/hipscat-import)
 [![Read the Docs](https://img.shields.io/readthedocs/hipscat-import)](https://hipscat-import.readthedocs.io/)
 
 ## HiPSCat import - Utility for ingesting large survey data into HiPSCat structure.
 
 Check out our [ReadTheDocs site](https://hipscat-import.readthedocs.io/en/latest/)
@@ -21,15 +23,13 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/guide/contributing.html)
 for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
-founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
-Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `hipscat-import-0.2.5/docs/Makefile` & `hipscat-import-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/arguments.rst` & `hipscat-import-0.2.6/docs/catalogs/arguments.rst`

 * *Files 5% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 We use the ``InputReader`` class to read files in chunks and pass the chunks
 along to the map/reduce stages. We've provided reference implementations for 
 reading CSV, FITS, and Parquet input files, but you can subclass the reader 
 type to suit whatever input files you've got.
 
 You only need to provide the ``file_reader`` argument if you are using a custom file reader
-or passing parameters to the file reader. For example you might use ``file_reader=CsvReader(separator="\s+")``
+or passing parameters to the file reader. For example you might use ``file_reader=CsvReader(sep="\s+")``
 to parse a whitespace separated file.
 
 You can find the full API documentation for 
 :py:class:`hipscat_import.catalog.file_readers.InputReader`
 
 .. code-block:: python
 
@@ -199,18 +199,35 @@
 should adjust your parameters.
 
 For more discussion of the ``pixel_threshold`` argument and a strategy for setting
 this parameter, see notebook :doc:`/notebooks/estimate_pixel_threshold`
 
 For more discussion of the "Binning" and all other stages, see :doc:`temp_files`
 
-Alternatively, you can use the ``constant_healpix_order`` argument. This will 
-**ignore** both of the ``pixel_threshold`` and ``highest_healpix_order`` arguments
-and the catalog will be partitioned by healpix pixels at the
-``constant_healpix_order``. This can be useful for very sparse datasets.
+Sparse Datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+For sparse datasets you might want to force your catalog partitioning to avoid
+partitions with very large area on they sky. 
+
+Why? If you have sparse data that you know you will want to cross-match or join
+to a catalog that is much denser, you may find yourself trying to match a large
+(in terms of area on the sky) pixel to thousands of smaller pixels in the denser
+catalog that occupy the same large region in the sky. Using more pixels of higher
+order will have some inefficiencies in terms of on-disk storage, but will be 
+easier to compute joins and cross-matches to large datasets.
+
+There are two strategies for tweaking the partitioning:
+
+* **order range** - use the ``lowest_healpix_order`` argument, in addition
+  to the ``highest_healpix_order``.
+* **constant order** - use the ``constant_healpix_order`` argument. This will 
+  **ignore** the ``pixel_threshold``, ``highest_healpix_order``, and 
+  ``lowest_healpix_order`` arguments and the catalog will be partitioned by 
+  healpix pixels at the ``constant_healpix_order``.
 
 Progress Reporting
 -------------------------------------------------------------------------------
 
 By default, we will display some progress bars during pipeline execution. To 
 disable these (e.g. when you expect no output to standard out), you can set
 ``progress_bar=False``.
```

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/allwise.rst` & `hipscat-import-0.2.6/docs/catalogs/public/allwise.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     type_frame = pd.read_csv("allwise_types.csv")
     type_map = dict(zip(type_frame["name"], type_frame["type"]))
 
     args = ImportArguments(
         output_artifact_name="allwise",
         input_path="/path/to/allwise/",
         file_reader=CsvReader(
+            chunksize=250_000,
             header=None,
-            separator="|",
+            sep="|",
             column_names=type_frame["name"].values.tolist(),
             type_map=type_map,
-            chunksize=250_000,
         ),
         use_schema_file="allwise_schema.parquet",
         ra_column="ra",
         dec_column="dec",
         sort_columns="source_id",
         pixel_threshold=1_000_000,
         highest_healpix_order=7,
```

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/index.rst` & `hipscat-import-0.2.6/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/neowise.rst` & `hipscat-import-0.2.6/docs/catalogs/public/neowise.rst`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     type_map = dict(zip(type_frame["name"], type_frame["type"]))
 
     args = ImportArguments(
         output_artifact_name="neowise_1",
         input_path="/path/to/neowiser_year8/",
         file_reader=CsvReader(
             header=None,
-            separator="|",
+            sep="|",
             column_names=type_frame["name"].values.tolist(),
             type_map=type_map,
             chunksize=250_000,
         ).read,
         ra_column="RA",
         dec_column="DEC",
         pixel_threshold=2_000_000,
```

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/panstarrs.rst` & `hipscat-import-0.2.6/docs/catalogs/public/panstarrs.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/sdss.rst` & `hipscat-import-0.2.6/docs/catalogs/public/sdss.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/tic.rst` & `hipscat-import-0.2.6/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/public/zubercal.rst` & `hipscat-import-0.2.6/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/catalogs/temp_files.rst` & `hipscat-import-0.2.6/docs/catalogs/temp_files.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/conf.py` & `hipscat-import-0.2.6/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 templates_path = []
 exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 
 # This assumes that sphinx-build is called from the root directory
 master_doc = "index"
-html_theme = "sphinx_rtd_theme"
+
+html_theme = "sphinx_book_theme"
+
+html_static_path = ["_static"]
+html_css_files = ["custom.css"]
 
 extensions = [
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
     "autoapi.extension",
```

### Comparing `hipscat-import-0.2.5/docs/guide/contact.rst` & `hipscat-import-0.2.6/docs/guide/contact.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/guide/contributing.rst` & `hipscat-import-0.2.6/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/guide/dask_on_ray.rst` & `hipscat-import-0.2.6/docs/guide/dask_on_ray.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/guide/index_table.rst` & `hipscat-import-0.2.6/docs/guide/index_table.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/guide/margin_cache.rst` & `hipscat-import-0.2.6/docs/guide/margin_cache.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/index.rst` & `hipscat-import-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat-import-0.2.6/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/notebooks/unequal_schema.ipynb` & `hipscat-import-0.2.6/docs/notebooks/unequal_schema.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/allwise_schema.parquet` & `hipscat-import-0.2.6/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/allwise_types.csv` & `hipscat-import-0.2.6/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/neowise_schema.parquet` & `hipscat-import-0.2.6/docs/static/neowise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/neowise_types.csv` & `hipscat-import-0.2.6/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/ps1_detections_types.csv` & `hipscat-import-0.2.6/docs/static/ps1_detections_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/ps1_otmo_types.csv` & `hipscat-import-0.2.6/docs/static/ps1_otmo_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/sdss_wget.bash` & `hipscat-import-0.2.6/docs/static/sdss_wget.bash`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/tic_schema.parquet` & `hipscat-import-0.2.6/docs/static/tic_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/docs/static/tic_types.csv` & `hipscat-import-0.2.6/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/pyproject.toml` & `hipscat-import-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "dask<=2024.2.0",
     "dask[distributed]",
     "deprecated",
     "healpy",
-    "hipscat >= 0.2.6",
+    "hipscat >= 0.2.9",
     "ipykernel", # Support for Jupyter notebooks
     "pandas < 2.1.0",
     "pyarrow",
     "pyyaml",
     "tqdm",
     "numpy < 1.25",
     "fsspec <= 2024.2.0", # Remove when pyarrow updates to reflect api changes
```

### Comparing `hipscat-import-0.2.5/src/.pylintrc` & `hipscat-import-0.2.6/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/catalog/arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/catalog/arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     resume: bool = True
     """if there are existing intermediate resume files, should we
     read those and continue to create a new catalog where we left off"""
     constant_healpix_order: int = -1
     """healpix order to use when mapping. if this is
     a positive number, this will be the order of all final pixels and we
     will not combine pixels according to the threshold"""
+    lowest_healpix_order: int = 0
+    """the lowest possible healpix order that we will use for the final 
+    catalog partitioning. setting this higher than 0 will prevent creating
+    partitions with a large area on the sky."""
     highest_healpix_order: int = 7
     """healpix order to use when mapping. this will
     not necessarily be the order used in the final catalog, as we may combine
     pixels that don't meed the threshold"""
     pixel_threshold: int = 1_000_000
     """maximum number of rows for a single resulting pixel.
     we may combine hierarchically until we near the ``pixel_threshold``"""
@@ -79,19 +83,24 @@
     def __post_init__(self):
         self._check_arguments()
 
     def _check_arguments(self):
         """Check existence and consistency of argument values"""
         super()._check_arguments()
 
+        if self.lowest_healpix_order == self.highest_healpix_order:
+            self.constant_healpix_order = self.lowest_healpix_order
         if self.constant_healpix_order >= 0:
             check_healpix_order_range(self.constant_healpix_order, "constant_healpix_order")
             self.mapping_healpix_order = self.constant_healpix_order
         else:
             check_healpix_order_range(self.highest_healpix_order, "highest_healpix_order")
+            check_healpix_order_range(
+                self.lowest_healpix_order, "lowest_healpix_order", upper_bound=self.highest_healpix_order
+            )
             if not 100 <= self.pixel_threshold <= 1_000_000_000:
                 raise ValueError("pixel_threshold should be between 100 and 1,000,000,000")
             self.mapping_healpix_order = self.highest_healpix_order
 
         if self.catalog_type not in ("source", "object"):
             raise ValueError("catalog_type should be one of `source` or `object`")
 
@@ -145,14 +154,15 @@
             "input_paths": self.input_paths,
             "input_file_list": self.input_file_list,
             "ra_column": self.ra_column,
             "dec_column": self.dec_column,
             "use_hipscat_index": self.use_hipscat_index,
             "sort_columns": self.sort_columns,
             "constant_healpix_order": self.constant_healpix_order,
+            "lowest_healpix_order": self.lowest_healpix_order,
             "highest_healpix_order": self.highest_healpix_order,
             "pixel_threshold": self.pixel_threshold,
             "mapping_healpix_order": self.mapping_healpix_order,
             "debug_stats_only": self.debug_stats_only,
             "file_reader_info": file_reader_info,
         }
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/catalog/file_readers.py` & `hipscat-import-0.2.6/src/hipscat_import/catalog/file_readers.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,52 +9,45 @@
 
 # pylint: disable=too-few-public-methods,too-many-arguments
 
 
 def get_file_reader(
     file_format,
     chunksize=500_000,
-    header="infer",
     schema_file=None,
     column_names=None,
     skip_column_names=None,
     type_map=None,
-    separator=",",
     **kwargs,
 ):
     """Get a generator file reader for common file types
 
     Args:
         file_format (str): specifier for the file type and extension.
             Currently supported formats include:
 
             - `csv`, comma separated values. may also be tab- or pipe-delimited
               includes `.csv.gz` and other compressed csv files
             - `fits`, flexible image transport system. often used for astropy tables.
             - `parquet`, compressed columnar data format
 
         chunksize (int): number of rows to read in a single iteration.
-        header (int, list of int, None, default 'infer'): for CSV files, rows to
-            use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): for CSV files, the names of columns if no header
             is available. for fits files, a list of columns to *keep*.
         skip_column_names (list[str]): for fits files, a list of columns to remove.
         type_map (dict): for CSV files, the data types to use for columns
-        separator (str): for CSV files, the character used for separation.
     """
     if "csv" in file_format:
         return CsvReader(
             chunksize=chunksize,
-            header=header,
             schema_file=schema_file,
             column_names=column_names,
             type_map=type_map,
-            separator=separator,
             **kwargs,
         )
     if file_format == "fits":
         return FitsReader(
             chunksize=chunksize,
             column_names=column_names,
             skip_column_names=skip_column_names,
@@ -66,19 +59,21 @@
     raise NotImplementedError(f"File Format: {file_format} not supported")
 
 
 class InputReader(abc.ABC):
     """Base class for chunking file readers."""
 
     @abc.abstractmethod
-    def read(self, input_file):
+    def read(self, input_file, read_columns=None):
         """Read the input file, or chunk of the input file.
 
         Args:
             input_file(str): path to the input file.
+            read_columns(List[str]): subset of columns to read.
+                if None, all columns are read
         Yields:
             DataFrame containing chunk of file info.
         """
 
     @abc.abstractmethod
     def provenance_info(self) -> dict:
         """Create dictionary of parameters for provenance tracking.
@@ -110,88 +105,81 @@
         chunksize (int): number of rows to read in a single iteration.
         header (int, list of int, None, default 'infer'): rows to
             use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): the names of columns if no header is available
         type_map (dict): the data types to use for columns
-        separator (str): the character used for separation. Use '\\s+' to
-            process whitespace separated files.
         parquet_kwargs (dict): additional keyword arguments to use when
             reading the parquet schema metadata.
         kwargs (dict): additional keyword arguments to use when reading
             the CSV files.
     """
 
     def __init__(
         self,
         chunksize=500_000,
         header="infer",
         schema_file=None,
         column_names=None,
         type_map=None,
-        separator=",",
         parquet_kwargs=None,
         **kwargs,
     ):
         self.chunksize = chunksize
         self.header = header
         self.schema_file = schema_file
         self.column_names = column_names
         self.type_map = type_map
-        self.separator = separator
         self.parquet_kwargs = parquet_kwargs
         self.kwargs = kwargs
 
-    def read(self, input_file):
-        self.regular_file_exists(input_file, **self.kwargs)
-
         if self.schema_file:
             if self.parquet_kwargs is None:
                 self.parquet_kwargs = {}
             schema_parquet = file_io.load_parquet_to_pandas(
                 FilePointer(self.schema_file),
                 **self.parquet_kwargs,
             )
 
-        use_column_names = None
         if self.column_names:
-            use_column_names = self.column_names
+            self.kwargs["names"] = self.column_names
         elif not self.header and self.schema_file:
-            use_column_names = schema_parquet.columns
+            self.kwargs["names"] = schema_parquet.columns
 
-        use_type_map = None
         if self.type_map:
-            use_type_map = self.type_map
+            self.kwargs["dtype"] = self.type_map
         elif self.schema_file:
-            use_type_map = schema_parquet.dtypes.to_dict()
+            self.kwargs["dtype"] = schema_parquet.dtypes.to_dict()
+
+    def read(self, input_file, read_columns=None):
+        self.regular_file_exists(input_file, **self.kwargs)
+
+        if read_columns:
+            self.kwargs["usecols"] = read_columns
 
         with file_io.load_csv_to_pandas(
             FilePointer(input_file),
             chunksize=self.chunksize,
-            sep=self.separator,
             header=self.header,
-            names=use_column_names,
-            dtype=use_type_map,
             **self.kwargs,
         ) as reader:
             yield from reader
 
     def provenance_info(self) -> dict:
-        str_type_map = {}
+        str_kwargs = {}
         if self.type_map:
-            str_type_map = {key: str(value) for (key, value) in self.type_map.items()}
+            str_kwargs = {key: str(value) for (key, value) in self.kwargs.items()}
         provenance_info = {
             "input_reader_type": "CsvReader",
             "chunksize": self.chunksize,
-            "header": self.header,
             "schema_file": self.schema_file,
-            "separator": self.separator,
             "column_names": self.column_names,
-            "type_map": str_type_map,
+            "parquet_kwargs": self.parquet_kwargs,
+            "kwargs": str_kwargs,
         }
         return provenance_info
 
 
 class FitsReader(InputReader):
     """Chunked FITS file reader.
 
@@ -219,17 +207,19 @@
 
     def __init__(self, chunksize=500_000, column_names=None, skip_column_names=None, **kwargs):
         self.chunksize = chunksize
         self.column_names = column_names
         self.skip_column_names = skip_column_names
         self.kwargs = kwargs
 
-    def read(self, input_file):
+    def read(self, input_file, read_columns=None):
         self.regular_file_exists(input_file, **self.kwargs)
         table = Table.read(input_file, memmap=True, **self.kwargs)
+        if read_columns:
+            table.keep_columns(read_columns)
         if self.column_names:
             table.keep_columns(self.column_names)
         elif self.skip_column_names:
             table.remove_columns(self.skip_column_names)
 
         total_rows = len(table)
         read_rows = 0
@@ -257,15 +247,15 @@
             into memory at once.
     """
 
     def __init__(self, chunksize=500_000, **kwargs):
         self.chunksize = chunksize
         self.kwargs = kwargs
 
-    def read(self, input_file):
+    def read(self, input_file, read_columns=None):
         self.regular_file_exists(input_file, **self.kwargs)
         parquet_file = pq.ParquetFile(input_file, **self.kwargs)
         for smaller_table in parquet_file.iter_batches(batch_size=self.chunksize, use_pandas_metadata=True):
             yield smaller_table.to_pandas()
 
     def provenance_info(self) -> dict:
         provenance_info = {
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/catalog/map_reduce.py` & `hipscat-import-0.2.6/src/hipscat_import/catalog/map_reduce.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,36 +35,27 @@
 def _iterate_input_file(
     input_file: FilePointer,
     file_reader: InputReader,
     highest_order,
     ra_column,
     dec_column,
     use_hipscat_index=False,
+    read_columns=None,
 ):
     """Helper function to handle input file reading and healpix pixel calculation"""
     if not file_reader:
         raise NotImplementedError("No file reader implemented")
 
-    required_columns = [ra_column, dec_column]
-
-    for chunk_number, data in enumerate(file_reader.read(input_file)):
+    for chunk_number, data in enumerate(file_reader.read(input_file, read_columns=read_columns)):
         if use_hipscat_index:
             if data.index.name == HIPSCAT_ID_COLUMN:
                 mapped_pixels = hipscat_id_to_healpix(data.index, target_order=highest_order)
-            elif HIPSCAT_ID_COLUMN in data.columns:
-                mapped_pixels = hipscat_id_to_healpix(data[HIPSCAT_ID_COLUMN], target_order=highest_order)
             else:
-                raise ValueError(
-                    f"Invalid column names in input file: {HIPSCAT_ID_COLUMN} not in {input_file}"
-                )
+                mapped_pixels = hipscat_id_to_healpix(data[HIPSCAT_ID_COLUMN], target_order=highest_order)
         else:
-            if not all(x in data.columns for x in required_columns):
-                raise ValueError(
-                    f"Invalid column names in input file: {', '.join(required_columns)} not in {input_file}"
-                )
             # Set up the pixel data
             mapped_pixels = hp.ang2pix(
                 2**highest_order,
                 data[ra_column].to_numpy(copy=False, dtype=float),
                 data[dec_column].to_numpy(copy=False, dtype=float),
                 lonlat=True,
                 nest=True,
@@ -99,16 +90,22 @@
         one-dimensional numpy array of long integers where the value at each index corresponds
         to the number of objects found at the healpix pixel.
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
     histo = pixel_math.empty_histogram(highest_order)
+
+    if use_hipscat_index:
+        read_columns = [HIPSCAT_ID_COLUMN]
+    else:
+        read_columns = [ra_column, dec_column]
+
     for _, _, mapped_pixels in _iterate_input_file(
-        input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index
+        input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index, read_columns
     ):
         mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
         mapped_pixel = mapped_pixel.astype(np.int64)
         histo[mapped_pixel] += count_at_pixel.astype(np.int64)
     ResumePlan.write_partial_histogram(tmp_path=resume_path, mapping_key=mapping_key, histogram=histo)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/catalog/resume_plan.py` & `hipscat-import-0.2.6/src/hipscat_import/catalog/resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/catalog/run_import.py` & `hipscat-import-0.2.6/src/hipscat_import/catalog/run_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,21 @@
                 histogram=raw_histogram,
                 constant_healpix_order=args.constant_healpix_order,
             )
         else:
             alignment = pixel_math.generate_alignment(
                 raw_histogram,
                 highest_order=args.highest_healpix_order,
+                lowest_order=args.lowest_healpix_order,
                 threshold=args.pixel_threshold,
             )
             destination_pixel_map = pixel_math.compute_pixel_map(
                 raw_histogram,
                 highest_order=args.highest_healpix_order,
+                lowest_order=args.lowest_healpix_order,
                 threshold=args.pixel_threshold,
             )
         step_progress.update(1)
 
     if not args.debug_stats_only:
         alignment_future = client.scatter(alignment)
         _split_pixels(args, alignment_future, client)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/index/arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/index/arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utility to hold all arguments required throughout indexing"""
 
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from hipscat.catalog import Catalog
 from hipscat.catalog.index.index_catalog_info import IndexCatalogInfo
 from hipscat.io.validation import is_valid_catalog
 
 from hipscat_import.runtime_arguments import RuntimeArguments
 
@@ -13,14 +13,16 @@
 @dataclass
 class IndexArguments(RuntimeArguments):
     """Data class for holding indexing arguments"""
 
     ## Input
     input_catalog_path: str = ""
     input_catalog: Optional[Catalog] = None
+    input_storage_options: Union[Dict[Any, Any], None] = None
+    """optional dictionary of abstract filesystem credentials for the INPUT."""
     indexing_column: str = ""
     extra_columns: List[str] = field(default_factory=list)
 
     ## Output
     include_hipscat_index: bool = True
     """Include the hipscat spatial partition index."""
     include_order_pixel: bool = True
@@ -50,17 +52,19 @@
             raise ValueError("input_catalog_path is required")
         if not self.indexing_column:
             raise ValueError("indexing_column is required")
 
         if not self.include_hipscat_index and not self.include_order_pixel:
             raise ValueError("At least one of include_hipscat_index or include_order_pixel must be True")
 
-        if not is_valid_catalog(self.input_catalog_path):
+        if not is_valid_catalog(self.input_catalog_path, storage_options=self.input_storage_options):
             raise ValueError("input_catalog_path not a valid catalog")
-        self.input_catalog = Catalog.read_from_hipscat(catalog_path=self.input_catalog_path)
+        self.input_catalog = Catalog.read_from_hipscat(
+            catalog_path=self.input_catalog_path, storage_options=self.input_storage_options
+        )
 
         if self.compute_partition_size < 100_000:
             raise ValueError("compute_partition_size must be at least 100_000")
 
     def to_catalog_info(self, total_rows) -> IndexCatalogInfo:
         """Catalog-type-specific dataset info."""
         info = {
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/index/map_reduce.py` & `hipscat-import-0.2.6/src/hipscat_import/index/map_reduce.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 from hipscat.io import paths
 from hipscat.pixel_math.hipscat_id import HIPSCAT_ID_COLUMN
 
 
-def read_leaf_file(input_file, include_columns, include_hipscat_index, drop_duplicates):
+def read_leaf_file(input_file, include_columns, include_hipscat_index, drop_duplicates, storage_options):
     """Mapping function called once per input file.
 
     Reads the leaf parquet file, and returns with appropriate columns and duplicates dropped."""
     data = pd.read_parquet(
         input_file,
         columns=include_columns,
         engine="pyarrow",
+        storage_options=storage_options,
     )
 
     data = data.reset_index()
     if not include_hipscat_index:
         data = data.drop(columns=[HIPSCAT_ID_COLUMN])
 
     if drop_duplicates:
@@ -46,14 +47,15 @@
                 pixel_number=pixel.pixel,
             )
             for pixel in args.input_catalog.get_healpix_pixels()
         ],
         include_columns=include_columns,
         include_hipscat_index=args.include_hipscat_index,
         drop_duplicates=args.drop_duplicates,
+        storage_options=args.input_storage_options,
     )
 
     if args.include_order_pixel:
         ## Take out the hive dictionary behavior that turns these into int32.
         data["Norder"] = data["Norder"].astype(np.uint8)
         data["Dir"] = data["Dir"].astype(np.uint64)
         data["Npix"] = data["Npix"].astype(np.uint64)
@@ -68,10 +70,11 @@
     data = data.repartition(partition_size=args.compute_partition_size)
 
     # Now just write it out to leaf parquet files!
     result = data.to_parquet(
         path=index_dir,
         engine="pyarrow",
         compute_kwargs={"partition_size": args.compute_partition_size},
+        storage_options=args.output_storage_options,
     )
     client.compute(result)
     return len(data)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,34 +34,35 @@
     margin_pairs_df = pd.DataFrame(
         zip(norders, part_pix, margin_pix),
         columns=["partition_order", "partition_pixel", "margin_pixel"],
     )
     return margin_pairs_df
 
 
-def _create_margin_directory(stats, output_path):
+def _create_margin_directory(stats, output_path, storage_options):
     """Creates directories for all the catalog partitions."""
     for healpixel in stats:
         order = healpixel.order
         pix = healpixel.pixel
 
         destination_dir = paths.pixel_directory(output_path, order, pix)
-        file_io.make_directory(destination_dir, exist_ok=True)
+        file_io.make_directory(destination_dir, exist_ok=True, storage_options=storage_options)
 
 
 def _map_to_margin_shards(client, args, partition_pixels, margin_pairs):
     """Create all the jobs for mapping partition files into the margin cache."""
     futures = []
     mp_future = client.scatter(margin_pairs, broadcast=True)
     for pix in partition_pixels:
         partition_file = paths.pixel_catalog_file(args.input_catalog_path, pix.order, pix.pixel)
         futures.append(
             client.submit(
                 mcmr.map_pixel_shards,
                 partition_file=partition_file,
+                input_storage_options=args.input_storage_options,
                 margin_pairs=mp_future,
                 margin_threshold=args.margin_threshold,
                 output_path=args.tmp_path,
                 margin_order=args.margin_order,
                 ra_column=args.catalog.catalog_info.ra_column,
                 dec_column=args.catalog.catalog_info.dec_column,
             )
@@ -82,17 +83,19 @@
 
     for pix in partition_pixels:
         futures.append(
             client.submit(
                 mcmr.reduce_margin_shards,
                 intermediate_directory=args.tmp_path,
                 output_path=args.catalog_path,
+                output_storage_options=args.output_storage_options,
                 partition_order=pix.order,
                 partition_pixel=pix.pixel,
                 original_catalog_metadata=paths.get_common_metadata_pointer(args.input_catalog_path),
+                input_storage_options=args.input_storage_options,
             )
         )
 
     for _ in tqdm(
         as_completed(futures),
         desc="Reducing ",
         total=len(futures),
@@ -115,27 +118,29 @@
     # get the negative tree pixels
     negative_pixels = args.catalog.generate_negative_tree_pixels()
 
     combined_pixels = partition_stats + negative_pixels
 
     margin_pairs = _find_partition_margin_pixel_pairs(combined_pixels, args.margin_order)
 
-    _create_margin_directory(combined_pixels, args.catalog_path)
+    _create_margin_directory(combined_pixels, args.catalog_path, args.output_storage_options)
 
     _map_to_margin_shards(
         client=client,
         args=args,
         partition_pixels=partition_stats,
         margin_pairs=margin_pairs,
     )
 
     _reduce_margin_shards(client=client, args=args, partition_pixels=combined_pixels)
 
     with tqdm(total=4, desc="Finishing", disable=not args.progress_bar) as step_progress:
-        parquet_metadata.write_parquet_metadata(args.catalog_path)
+        parquet_metadata.write_parquet_metadata(
+            args.catalog_path, storage_options=args.output_storage_options
+        )
         step_progress.update(1)
         total_rows = 0
         metadata_path = paths.get_parquet_metadata_pointer(args.catalog_path)
         for row_group in parquet_metadata.read_row_group_fragments(
             metadata_path, storage_options=args.output_storage_options
         ):
             total_rows += row_group.num_rows
@@ -147,14 +152,19 @@
 
         step_progress.update(1)
         margin_catalog_info = args.to_catalog_info(int(total_rows))
         write_metadata.write_provenance_info(
             catalog_base_dir=args.catalog_path,
             dataset_info=margin_catalog_info,
             tool_args=args.provenance_info(),
+            storage_options=args.output_storage_options,
         )
         write_metadata.write_catalog_info(
-            catalog_base_dir=args.catalog_path, dataset_info=margin_catalog_info
+            catalog_base_dir=args.catalog_path,
+            dataset_info=margin_catalog_info,
+            storage_options=args.output_storage_options,
         )
         step_progress.update(1)
-        file_io.remove_directory(args.tmp_path, ignore_errors=True)
+        file_io.remove_directory(
+            args.tmp_path, ignore_errors=True, storage_options=args.output_storage_options
+        )
         step_progress.update(1)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 from dataclasses import dataclass
+from typing import Any, Dict, Union
 
 import healpy as hp
 from hipscat.catalog import Catalog
 from hipscat.catalog.margin_cache.margin_cache_catalog_info import MarginCacheCatalogInfo
 from hipscat.io.validation import is_valid_catalog
 
 from hipscat_import.runtime_arguments import RuntimeArguments
@@ -22,26 +23,30 @@
     doing more precise boundary checking. this value must be greater than the highest
     order of healpix partitioning in the source catalog. if `margin_order` is left
     default or set to -1, then the `margin_order` will be set dynamically to the
     highest partition order plus 1."""
 
     input_catalog_path: str = ""
     """the path to the hipscat-formatted input catalog."""
+    input_storage_options: Union[Dict[Any, Any], None] = None
+    """optional dictionary of abstract filesystem credentials for the INPUT."""
 
     def __post_init__(self):
         self._check_arguments()
 
     def _check_arguments(self):
         super()._check_arguments()
         if not self.input_catalog_path:
             raise ValueError("input_catalog_path is required")
-        if not is_valid_catalog(self.input_catalog_path):
+        if not is_valid_catalog(self.input_catalog_path, storage_options=self.input_storage_options):
             raise ValueError("input_catalog_path not a valid catalog")
 
-        self.catalog = Catalog.read_from_hipscat(self.input_catalog_path)
+        self.catalog = Catalog.read_from_hipscat(
+            self.input_catalog_path, storage_options=self.input_storage_options
+        )
 
         highest_order = self.catalog.partition_info.get_highest_order()
         margin_pixel_k = highest_order + 1
         if self.margin_order > -1:
             if self.margin_order < margin_pixel_k:
                 raise ValueError(
                     "margin_order must be of a higher order "
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/margin_cache/margin_cache_map_reduce.py` & `hipscat-import-0.2.6/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 from hipscat.pixel_math.hipscat_id import HIPSCAT_ID_COLUMN
 
 from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory
 
 
 def map_pixel_shards(
     partition_file,
+    input_storage_options,
     margin_pairs,
     margin_threshold,
     output_path,
     margin_order,
     ra_column,
     dec_column,
 ):
     """Creates margin cache shards from a source partition file."""
-    data = file_io.load_parquet_to_pandas(partition_file)
+    data = file_io.load_parquet_to_pandas(partition_file, storage_options=input_storage_options)
 
     data["margin_pixel"] = hp.ang2pix(
         2**margin_order,
         data[ra_column].values,
         data[dec_column].values,
         lonlat=True,
         nest=True,
@@ -96,32 +97,40 @@
 
         final_df.to_parquet(shard_path)
 
         del data, margin_data, final_df
 
 
 def reduce_margin_shards(
-    intermediate_directory, output_path, partition_order, partition_pixel, original_catalog_metadata
+    intermediate_directory,
+    output_path,
+    output_storage_options,
+    partition_order,
+    partition_pixel,
+    original_catalog_metadata,
+    input_storage_options,
 ):
     """Reduce all partition pixel directories into a single file"""
     shard_dir = get_pixel_cache_directory(
         intermediate_directory, HealpixPixel(partition_order, partition_pixel)
     )
     if file_io.does_file_or_directory_exist(shard_dir):
         data = ds.dataset(shard_dir, format="parquet")
         full_df = data.to_table().to_pandas()
         margin_cache_dir = paths.pixel_directory(output_path, partition_order, partition_pixel)
-        file_io.make_directory(margin_cache_dir, exist_ok=True)
+        file_io.make_directory(margin_cache_dir, exist_ok=True, storage_options=output_storage_options)
 
         if len(full_df):
-            schema = file_io.read_parquet_metadata(original_catalog_metadata).schema.to_arrow_schema()
+            schema = file_io.read_parquet_metadata(
+                original_catalog_metadata, storage_options=input_storage_options
+            ).schema.to_arrow_schema()
 
             schema = (
                 schema.append(pa.field("margin_Norder", pa.uint8()))
                 .append(pa.field("margin_Dir", pa.uint64()))
                 .append(pa.field("margin_Npix", pa.uint64()))
             )
 
             margin_cache_file_path = paths.pixel_catalog_file(output_path, partition_order, partition_pixel)
 
-            full_df.to_parquet(margin_cache_file_path, schema=schema)
+            full_df.to_parquet(margin_cache_file_path, schema=schema, storage_options=output_storage_options)
             file_io.remove_directory(shard_dir)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/pipeline.py` & `hipscat-import-0.2.6/src/hipscat_import/pipeline.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/pipeline_resume_plan.py` & `hipscat-import-0.2.6/src/hipscat_import/pipeline_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/runtime_arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/soap/arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/soap/arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from typing import Any, Dict, Union
 
 from hipscat.catalog.association_catalog.association_catalog import AssociationCatalogInfo
 from hipscat.catalog.catalog_type import CatalogType
 from hipscat.io.validation import is_valid_catalog
 
 from hipscat_import.runtime_arguments import RuntimeArguments
 
@@ -10,19 +11,23 @@
 @dataclass
 class SoapArguments(RuntimeArguments):
     """Data class for holding source-object association arguments"""
 
     ## Input - Object catalog
     object_catalog_dir: str = ""
     object_id_column: str = ""
+    object_storage_options: Union[Dict[Any, Any], None] = None
+    """optional dictionary of abstract filesystem credentials for the OBJECT catalog."""
 
     ## Input - Source catalog
     source_catalog_dir: str = ""
     source_object_id_column: str = ""
     source_id_column: str = ""
+    source_storage_options: Union[Dict[Any, Any], None] = None
+    """optional dictionary of abstract filesystem credentials for the SOURCE catalog."""
 
     resume: bool = True
     """if there are existing intermediate resume files, should we
     read those and continue to run the pipeline where we left off"""
     write_leaf_files: bool = False
     """Should we also write out leaf parquet files (e.g. Norder/Dir/Npix.parquet)
     that represent the full association table"""
@@ -34,22 +39,22 @@
 
     def _check_arguments(self):
         super()._check_arguments()
         if not self.object_catalog_dir:
             raise ValueError("object_catalog_dir is required")
         if not self.object_id_column:
             raise ValueError("object_id_column is required")
-        if not is_valid_catalog(self.object_catalog_dir):
+        if not is_valid_catalog(self.object_catalog_dir, storage_options=self.object_storage_options):
             raise ValueError("object_catalog_dir not a valid catalog")
 
         if not self.source_catalog_dir:
             raise ValueError("source_catalog_dir is required")
         if not self.source_object_id_column:
             raise ValueError("source_object_id_column is required")
-        if not is_valid_catalog(self.source_catalog_dir):
+        if not is_valid_catalog(self.source_catalog_dir, storage_options=self.source_storage_options):
             raise ValueError("source_catalog_dir not a valid catalog")
 
         if self.compute_partition_size < 100_000:
             raise ValueError("compute_partition_size must be at least 100_000")
 
     def to_catalog_info(self, total_rows) -> AssociationCatalogInfo:
         """Catalog-type-specific dataset info."""
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/soap/map_reduce.py` & `hipscat-import-0.2.6/src/hipscat_import/soap/map_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pyarrow.parquet as pq
 from hipscat.catalog.association_catalog.partition_join_info import PartitionJoinInfo
 from hipscat.io import FilePointer, file_io, paths
+from hipscat.io.file_io.file_pointer import get_fs, strip_leading_slash_for_pyarrow
 from hipscat.io.parquet_metadata import get_healpix_pixel_from_metadata
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from hipscat.pixel_math.healpix_pixel_function import get_pixel_argsort
 
 from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory
 from hipscat_import.soap.arguments import SoapArguments
 from hipscat_import.soap.resume_plan import SoapPlan
@@ -18,17 +19,17 @@
 
 def _count_joins_for_object(source_data, source_pixel, object_pixel, soap_args):
     object_path = paths.pixel_catalog_file(
         catalog_base_dir=soap_args.object_catalog_dir,
         pixel_order=object_pixel.order,
         pixel_number=object_pixel.pixel,
     )
-    object_data = file_io.load_parquet_to_pandas(object_path, columns=[soap_args.object_id_column]).set_index(
-        soap_args.object_id_column
-    )
+    object_data = file_io.load_parquet_to_pandas(
+        object_path, columns=[soap_args.object_id_column], storage_options=soap_args.object_storage_options
+    ).set_index(soap_args.object_id_column)
 
     joined_data = source_data.merge(object_data, how="inner", left_index=True, right_index=True)
 
     rows_written = len(joined_data)
     if not soap_args.write_leaf_files or rows_written == 0:
         return rows_written
 
@@ -98,17 +99,17 @@
         pixel_order=source_pixel.order,
         pixel_number=source_pixel.pixel,
     )
     if soap_args.write_leaf_files and soap_args.source_object_id_column != soap_args.source_id_column:
         read_columns = [soap_args.source_object_id_column, soap_args.source_id_column]
     else:
         read_columns = [soap_args.source_object_id_column]
-    source_data = file_io.load_parquet_to_pandas(source_path, columns=read_columns).set_index(
-        soap_args.source_object_id_column
-    )
+    source_data = file_io.load_parquet_to_pandas(
+        source_path, columns=read_columns, storage_options=soap_args.source_storage_options
+    ).set_index(soap_args.source_object_id_column)
 
     remaining_sources = len(source_data)
     results = []
 
     for object_pixel in object_pixels:
         if remaining_sources < 1:
             break
@@ -124,15 +125,15 @@
     ## mark that some sources were not joined
     if remaining_sources > 0:
         results.append([-1, -1, remaining_sources])
 
     _write_count_results(soap_args.tmp_path, source_pixel, results)
 
 
-def combine_partial_results(input_path, output_path) -> int:
+def combine_partial_results(input_path, output_path, output_storage_options) -> int:
     """Combine many partial CSVs into single partition join info.
     Also write out a debug file with counts of unmatched sources, if any.
 
     Args:
         input_path(str): intermediate directory with partial result CSVs. likely, the
             directory used in the previous `count_joins` call as `cache_path`
         output_path(str): directory to write the combined results CSVs.
@@ -152,32 +153,35 @@
     matched = matched.loc[matched["num_rows"] > 0]
     unmatched = dataframe.loc[dataframe["Norder"] == -1]
 
     file_io.write_dataframe_to_csv(
         dataframe=matched,
         file_pointer=file_io.append_paths_to_pointer(output_path, "partition_join_info.csv"),
         index=False,
+        storage_options=output_storage_options,
     )
 
     if len(unmatched) > 0:
         file_io.write_dataframe_to_csv(
             dataframe=unmatched,
             file_pointer=file_io.append_paths_to_pointer(output_path, "unmatched_sources.csv"),
             index=False,
+            storage_options=output_storage_options,
         )
 
     primary_only = matched.groupby(["Norder", "Dir", "Npix"])["num_rows"].sum().reset_index()
     file_io.write_dataframe_to_csv(
         dataframe=primary_only,
         file_pointer=file_io.append_paths_to_pointer(output_path, "partition_info.csv"),
         index=False,
+        storage_options=output_storage_options,
     )
 
     join_info = PartitionJoinInfo(matched)
-    join_info.write_to_metadata_files(output_path)
+    join_info.write_to_metadata_files(output_path, storage_options=output_storage_options)
 
     return primary_only["num_rows"].sum()
 
 
 def reduce_joins(
     soap_args: SoapArguments, object_pixel: HealpixPixel, object_key: str, delete_input_files: bool = True
 ):
@@ -209,18 +213,22 @@
     shards = []
     for shard_file_name in shard_file_list:
         shards.append(pq.read_table(shard_file_name))
 
     # Write all of the shards into a single parquet file, one row-group-per-shard.
     starting_catalog_path = FilePointer(str(soap_args.catalog_path))
     destination_dir = paths.pixel_directory(starting_catalog_path, object_pixel.order, object_pixel.pixel)
-    file_io.make_directory(destination_dir, exist_ok=True)
+    file_io.make_directory(destination_dir, exist_ok=True, storage_options=soap_args.output_storage_options)
 
     output_file = paths.pixel_catalog_file(starting_catalog_path, object_pixel.order, object_pixel.pixel)
-    with pq.ParquetWriter(output_file, shards[0].schema) as writer:
+    file_system, output_file = get_fs(
+        file_pointer=output_file, storage_options=soap_args.output_storage_options
+    )
+    output_file = strip_leading_slash_for_pyarrow(output_file, protocol=file_system.protocol)
+    with pq.ParquetWriter(output_file, shards[0].schema, filesystem=file_system) as writer:
         for table in shards:
             writer.write_table(table)
 
     # Delete the intermediate shards.
     if delete_input_files:
         file_io.remove_directory(pixel_dir, ignore_errors=True)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/soap/resume_plan.py` & `hipscat-import-0.2.6/src/hipscat_import/soap/resume_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,24 @@
             self.count_keys = []
 
             ## Validate existing resume state.
             if self.is_counting_done():
                 return
             step_progress.update(1)
 
-            self.object_catalog = Catalog.read_from_hipscat(args.object_catalog_dir)
+            self.object_catalog = Catalog.read_from_hipscat(
+                args.object_catalog_dir, storage_options=args.object_storage_options
+            )
             source_map_file = file_io.append_paths_to_pointer(self.tmp_path, self.SOURCE_MAP_FILE)
             if file_io.does_file_or_directory_exist(source_map_file):
                 source_pixel_map = np.load(source_map_file, allow_pickle=True)["arr_0"].item()
             else:
-                source_catalog = Catalog.read_from_hipscat(args.source_catalog_dir)
+                source_catalog = Catalog.read_from_hipscat(
+                    args.source_catalog_dir, storage_options=args.source_storage_options
+                )
                 source_pixel_map = source_to_object_map(self.object_catalog, source_catalog)
                 np.savez_compressed(source_map_file, source_pixel_map)
             self.count_keys = self.get_sources_to_count(source_pixel_map=source_pixel_map)
             self.reduce_keys = self.get_objects_to_reduce()
             file_io.make_directory(
                 file_io.append_paths_to_pointer(self.tmp_path, self.REDUCING_STAGE),
                 exist_ok=True,
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/soap/run_soap.py` & `hipscat-import-0.2.6/src/hipscat_import/soap/run_soap.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,33 +49,46 @@
         resume_plan.wait_for_reducing(futures)
 
     # All done - write out the metadata
     with tqdm(
         total=4, desc=PipelineResumePlan.get_formatted_stage_name("Finishing"), disable=not args.progress_bar
     ) as step_progress:
         if args.write_leaf_files:
-            parquet_metadata.write_parquet_metadata(args.catalog_path)
+            parquet_metadata.write_parquet_metadata(
+                args.catalog_path,
+                storage_options=args.output_storage_options,
+            )
             total_rows = 0
             metadata_path = paths.get_parquet_metadata_pointer(args.catalog_path)
-            for row_group in parquet_metadata.read_row_group_fragments(metadata_path):
+            for row_group in parquet_metadata.read_row_group_fragments(
+                metadata_path,
+                storage_options=args.output_storage_options,
+            ):
                 total_rows += row_group.num_rows
             partition_join_info = PartitionJoinInfo.read_from_file(
                 metadata_path, storage_options=args.output_storage_options
             )
             partition_join_info.write_to_csv(
                 catalog_path=args.catalog_path, storage_options=args.output_storage_options
             )
         else:
-            total_rows = combine_partial_results(args.tmp_path, args.catalog_path)
+            total_rows = combine_partial_results(
+                args.tmp_path, args.catalog_path, args.output_storage_options
+            )
         step_progress.update(1)
         total_rows = int(total_rows)
         catalog_info = args.to_catalog_info(total_rows)
         write_metadata.write_provenance_info(
             catalog_base_dir=args.catalog_path,
             dataset_info=catalog_info,
             tool_args=args.provenance_info(),
+            storage_options=args.output_storage_options,
         )
         step_progress.update(1)
-        write_metadata.write_catalog_info(dataset_info=catalog_info, catalog_base_dir=args.catalog_path)
+        write_metadata.write_catalog_info(
+            dataset_info=catalog_info,
+            catalog_base_dir=args.catalog_path,
+            storage_options=args.output_storage_options,
+        )
         step_progress.update(1)
         resume_plan.clean_resume_files()
         step_progress.update(1)
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import/verification/arguments.py` & `hipscat-import-0.2.6/src/hipscat_import/verification/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import/verification/run_verification.py` & `hipscat-import-0.2.6/src/hipscat_import/verification/run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/src/hipscat_import.egg-info/PKG-INFO` & `hipscat-import-0.2.6/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.2.5
+Version: 0.2.6
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -39,15 +39,15 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask<=2024.2.0
 Requires-Dist: dask[distributed]
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.2.6
+Requires-Dist: hipscat>=0.2.9
 Requires-Dist: ipykernel
 Requires-Dist: pandas<2.1.0
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
 Requires-Dist: tqdm
 Requires-Dist: numpy<1.25
 Requires-Dist: fsspec<=2024.2.0
@@ -67,14 +67,16 @@
 <img src="https://github.com/lincc-frameworks/tape/blob/main/docs/DARK_Combo_sm.png?raw=true" width="300" height="100">
 
 # hipscat-import
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/hipscat-import?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/hipscat-import/)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/hipscat-import.svg?color=blue&logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/hipscat-import)
+
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/astronomy-commons/hipscat-import/smoke-test.yml)](https://github.com/astronomy-commons/hipscat-import/actions/workflows/smoke-test.yml)
 [![codecov](https://codecov.io/gh/astronomy-commons/hipscat-import/branch/main/graph/badge.svg)](https://codecov.io/gh/astronomy-commons/hipscat-import)
 [![Read the Docs](https://img.shields.io/readthedocs/hipscat-import)](https://hipscat-import.readthedocs.io/)
 
 ## HiPSCat import - Utility for ingesting large survey data into HiPSCat structure.
 
 Check out our [ReadTheDocs site](https://hipscat-import.readthedocs.io/en/latest/)
@@ -87,15 +89,13 @@
 * LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
   ([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
+See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/guide/contributing.html)
 for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
-founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
-Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `hipscat-import-0.2.5/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat-import-0.2.6/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
 docs/requirements.txt
+docs/_static/custom.css
 docs/catalogs/arguments.rst
 docs/catalogs/temp_files.rst
 docs/catalogs/public/allwise.rst
 docs/catalogs/public/index.rst
 docs/catalogs/public/neowise.rst
 docs/catalogs/public/panstarrs.rst
 docs/catalogs/public/sdss.rst
```

### Comparing `hipscat-import-0.2.5/tests/.pylintrc` & `hipscat-import-0.2.6/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/conftest.py` & `hipscat-import-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,27 +125,27 @@
     assert len(frame.columns) == 3
     assert np.all(frame.columns == ["id", "ra", "dec"])
 
 
 def test_csv_reader_pipe_delimited(formats_pipe_csv, tmp_path):
     """Verify we can read a pipe-delimited csv file without a header row."""
     total_chunks = 0
-    for frame in CsvReader(header=None, separator="|").read(formats_pipe_csv):
+    for frame in CsvReader(header=None, sep="|").read(formats_pipe_csv):
         total_chunks += 1
         assert len(frame) == 3
         assert np.all(frame[0] == ["AA", "BB", "CC"])
 
     assert total_chunks == 1
 
     ## Provide header names and types in a few formats
     frame = next(
         CsvReader(
-            header=None,
-            separator="|",
             column_names=["letters", "ints", "empty", "numeric"],
+            header=None,
+            sep="|",
         ).read(formats_pipe_csv)
     )
     assert len(frame) == 3
     assert np.all(frame["letters"] == ["AA", "BB", "CC"])
     column_types = frame.dtypes.to_dict()
     expected_column_types = {
         "letters": object,
@@ -153,23 +153,23 @@
         "empty": float,
         "numeric": float,
     }
     assert np.all(column_types == expected_column_types)
 
     frame = next(
         CsvReader(
-            header=None,
-            separator="|",
             column_names=["letters", "ints", "empty", "numeric"],
             type_map={
                 "letters": object,
                 "ints": int,
                 "empty": "Int64",
                 "numeric": int,
             },
+            header=None,
+            sep="|",
         ).read(formats_pipe_csv)
     )
     assert len(frame) == 3
     assert np.all(frame["letters"] == ["AA", "BB", "CC"])
     column_types = frame.dtypes.to_dict()
     expected_column_types = {
         "letters": object,
@@ -188,18 +188,15 @@
         ]
     )
     schema_file = os.path.join(tmp_path, "metadata.parquet")
     pq.write_metadata(parquet_schema_types, schema_file)
 
     frame = next(
         CsvReader(
-            header=None,
-            separator="|",
-            schema_file=schema_file,
-            parquet_kwargs={"dtype_backend": "numpy_nullable"},
+            schema_file=schema_file, header=None, sep="|", parquet_kwargs={"dtype_backend": "numpy_nullable"}
         ).read(formats_pipe_csv)
     )
 
     assert len(frame) == 3
     assert np.all(frame["letters"] == ["AA", "BB", "CC"])
     column_types = frame.dtypes.to_dict()
     expected_column_types = {
@@ -211,15 +208,15 @@
     assert np.all(column_types == expected_column_types)
 
 
 def test_csv_reader_provenance_info(tmp_path, basic_catalog_info):
     """Test that we get some provenance info and it is parseable into JSON."""
     reader = CsvReader(
         header=None,
-        separator="|",
+        sep="|",
         column_names=["letters", "ints", "empty", "numeric"],
         type_map={
             "letters": object,
             "ints": int,
             "empty": "Int64",
             "numeric": int,
         },
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     expected = hist.empty_histogram(0)
     expected[11] = 131
     npt.assert_array_equal(result, expected)
 
 
 def test_map_headers_wrong(formats_headers_csv):
     """Test loading the a file with non-default headers (without specifying right headers)"""
-    with pytest.raises(ValueError, match="header"):
+    with pytest.raises(ValueError, match="columns expected but not found"):
         mr.map_to_pixels(
             input_file=formats_headers_csv,
             file_reader=get_file_reader("csv"),
             highest_order=0,
             ra_column="ra",
             dec_column="dec",
             resume_path="",
@@ -152,15 +152,15 @@
 
     expected = hist.empty_histogram(0)
     expected[11] = 131
 
     result = read_partial_histogram(tmp_path, "map_0")
     npt.assert_array_equal(result, expected)
 
-    with pytest.raises(ValueError, match="_hipscat_index not in"):
+    with pytest.raises(ValueError, match="columns expected but not found"):
         mr.map_to_pixels(
             input_file=small_sky_single_file,
             file_reader=get_file_reader("csv"),
             highest_order=0,
             ra_column="NOPE",
             dec_column="NOPE",
             use_hipscat_index=True,  # no pre-existing index! expect failure.
@@ -174,15 +174,14 @@
     os.makedirs(os.path.join(tmp_path, "histograms"))
     input_file = os.path.join(mixed_schema_csv_dir, "input_01.csv")
     mr.map_to_pixels(
         input_file=input_file,
         file_reader=get_file_reader(
             "csv",
             schema_file=mixed_schema_csv_parquet,
-            parquet_kwargs={"dtype_backend": "numpy_nullable"},
         ),
         highest_order=0,
         ra_column="ra",
         dec_column="dec",
         resume_path=tmp_path,
         mapping_key="map_0",
     )
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_resume_plan.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_run_import.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/catalog/test_run_round_trip.py` & `hipscat-import-0.2.6/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import glob
 import os
 from pathlib import Path
 
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
+import pyarrow as pa
+import pyarrow.parquet as pq
 import pytest
 from hipscat.catalog.catalog import Catalog
 from hipscat.pixel_math.hipscat_id import hipscat_id_to_healpix
 
 import hipscat_import.catalog.run_import as runner
 from hipscat_import.catalog.arguments import ImportArguments
 from hipscat_import.catalog.file_readers import CsvReader, get_file_reader
@@ -76,31 +78,51 @@
         input_file_list=[
             Path(mixed_schema_csv_dir) / "input_01.csv",
             Path(mixed_schema_csv_dir) / "input_02.csv",
         ],
         output_path=Path(tmp_path),
         dask_tmp=Path(tmp_path),
         highest_healpix_order=1,
-        file_reader=get_file_reader("csv", chunksize=1, schema_file=Path(mixed_schema_csv_parquet)),
+        file_reader=get_file_reader(
+            "csv",
+            chunksize=1,
+            schema_file=Path(mixed_schema_csv_parquet),
+            parquet_kwargs={"dtype_backend": "numpy_nullable"},
+        ),
         progress_bar=False,
     )
 
-    with pytest.raises(RuntimeError, match="Some reducing stages failed"):
-        runner.run(args, dask_client)
-
-    ## Try again, but with the schema specified.
-    args.use_schema_file = mixed_schema_csv_parquet
-    args.output_artifact_name = "mixed_csv_good"
     runner.run(args, dask_client)
 
     # Check that the catalog parquet file exists
     output_file = os.path.join(args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet")
 
     assert_parquet_file_ids(output_file, "id", [*range(700, 708)])
 
+    # Check that the schema is correct for leaf parquet and _metadata files
+    expected_parquet_schema = pa.schema(
+        [
+            pa.field("id", pa.int64()),
+            pa.field("ra", pa.float64()),
+            pa.field("dec", pa.float64()),
+            pa.field("ra_error", pa.int64()),
+            pa.field("dec_error", pa.int64()),
+            pa.field("comment", pa.string()),
+            pa.field("code", pa.string()),
+            pa.field("Norder", pa.uint8()),
+            pa.field("Dir", pa.uint64()),
+            pa.field("Npix", pa.uint64()),
+            pa.field("_hipscat_index", pa.uint64()),
+        ]
+    )
+    schema = pq.read_metadata(output_file).schema.to_arrow_schema()
+    assert schema.equals(expected_parquet_schema, check_metadata=False)
+    schema = pq.read_metadata(os.path.join(args.catalog_path, "_metadata")).schema.to_arrow_schema()
+    assert schema.equals(expected_parquet_schema, check_metadata=False)
+
 
 @pytest.mark.dask
 def test_import_preserve_index(
     dask_client,
     formats_pandasindex,
     assert_parquet_file_ids,
     assert_parquet_file_index,
@@ -310,33 +332,72 @@
     data_frame = pd.read_parquet(output_file, engine="pyarrow")
     assert len(data_frame) == 14
     ids = data_frame["id"]
     assert np.logical_and(ids >= 700, ids < 832).all()
 
 
 @pytest.mark.dask
+def test_import_lowest_healpix_order(
+    dask_client,
+    small_sky_parts_dir,
+    tmp_path,
+):
+    """Test basic execution.
+    - tests that all the final tiles are at the lowest healpix order,
+        and that we don't create tiles where there is no data.
+    """
+    args = ImportArguments(
+        output_artifact_name="small_sky_object_catalog",
+        input_path=small_sky_parts_dir,
+        file_reader="csv",
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        lowest_healpix_order=2,
+        highest_healpix_order=4,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog metadata file exists
+    catalog = Catalog.read_from_hipscat(args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == args.catalog_path
+    # Check that the partition info file exists - all pixels at order 2!
+    assert all(pixel.order == 2 for pixel in catalog.partition_info.get_healpix_pixels())
+
+    # Pick a parquet file and make sure it contains as many rows as we expect
+    output_file = os.path.join(args.catalog_path, "Norder=2", "Dir=0", "Npix=178.parquet")
+
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert len(data_frame) == 14
+    ids = data_frame["id"]
+    assert np.logical_and(ids >= 700, ids < 832).all()
+
+
+@pytest.mark.dask
 def test_import_starr_file(
     dask_client,
     formats_dir,
     assert_parquet_file_ids,
     tmp_path,
 ):
     """Test basic execution.
     - tests that we can run pipeline with a totally unknown file type, so long
       as a valid InputReader implementation is provided.
     """
 
     class StarrReader(CsvReader):
         """Shallow subclass"""
 
-        def read(self, input_file):
+        def read(self, input_file, read_columns=None):
             files = glob.glob(f"{input_file}/**.starr")
             files.sort()
             for file in files:
-                return super().read(file)
+                return super().read(file, read_columns)
 
     args = ImportArguments(
         output_artifact_name="starr",
         input_file_list=[formats_dir],
         file_reader=StarrReader(),
         output_path=tmp_path,
         dask_tmp=tmp_path,
@@ -470,15 +531,14 @@
 
     args = ImportArguments(
         output_artifact_name="gaia_minimum",
         input_file_list=[input_file],
         file_reader=CsvReader(
             comment="#",
             schema_file=schema_file,
-            parquet_kwargs={"dtype_backend": "numpy_nullable"},
         ),
         ra_column="ra",
         dec_column="dec",
         sort_columns="solution_id",
         use_schema_file=schema_file,
         output_path=tmp_path,
         dask_tmp=tmp_path,
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/conftest.py` & `hipscat-import-0.2.6/tests/hipscat_import/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat-import-0.2.6/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/gaia_minimum.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/gaia_minimum.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/hipscat_index.csv` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/hipscat_index.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/hipscat_index.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/hipscat_index.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/multiindex.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/multiindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat-import-0.2.6/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/index/test_index_argument.py` & `hipscat-import-0.2.6/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat-import-0.2.6/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/index/test_run_index.py` & `hipscat-import-0.2.6/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,11 +153,12 @@
         output_path=tmp_path,
         output_artifact_name="catalog_cache",
     )
 
     mc._create_margin_directory(
         stats=args.catalog.partition_info.get_healpix_pixels(),
         output_path=args.catalog_path,
+        storage_options=None,
     )
 
     output = file_io.append_paths_to_pointer(args.catalog_path, "Norder=0", "Dir=0")
     assert file_io.does_file_or_directory_exist(output)
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,20 @@
 
     basic_data_shard_df = test_df
 
     basic_data_shard_df.to_parquet(first_shard_path)
     basic_data_shard_df.to_parquet(second_shard_path)
 
     margin_cache_map_reduce.reduce_margin_shards(
-        intermediate_dir, tmp_path, 1, 21, original_catalog_metadata=schema_path
+        intermediate_dir,
+        tmp_path,
+        None,
+        1,
+        21,
+        original_catalog_metadata=schema_path,
+        input_storage_options=None,
     )
 
     result_path = paths.pixel_catalog_file(tmp_path, 1, 21)
 
     validate_result_dataframe(result_path, 720)
     assert not os.path.exists(shard_dir)
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/margin_cache/test_margin_round_trip.py` & `hipscat-import-0.2.6/tests/hipscat_import/margin_cache/test_margin_round_trip.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/soap/conftest.py` & `hipscat-import-0.2.6/tests/hipscat_import/soap/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/soap/test_run_soap.py` & `hipscat-import-0.2.6/tests/hipscat_import/soap/test_run_soap.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,39 @@
     assert catalog.catalog_path == small_sky_soap_args.catalog_path
     assert len(catalog.get_join_pixels()) == 14
     assert catalog.catalog_info.total_rows == 17161
     assert not catalog.catalog_info.contains_leaf_files
 
 
 @pytest.mark.dask
+def test_object_to_self(dask_client, tmp_path, small_sky_object_catalog):
+    """Test creating association between object and source catalogs."""
+    small_sky_soap_args = SoapArguments(
+        object_catalog_dir=small_sky_object_catalog,
+        object_id_column="id",
+        source_catalog_dir=small_sky_object_catalog,
+        source_object_id_column="id",
+        output_path=tmp_path,
+        overwrite=True,
+        progress_bar=False,
+        source_id_column="id",
+        output_artifact_name="small_sky_object_to_source",
+    )
+    runner.run(small_sky_soap_args, dask_client)
+
+    ## Check that the association data can be parsed as a valid association catalog.
+    catalog = AssociationCatalog.read_from_hipscat(small_sky_soap_args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == small_sky_soap_args.catalog_path
+    assert len(catalog.get_join_pixels()) == 1
+    assert catalog.catalog_info.total_rows == 131
+    assert not catalog.catalog_info.contains_leaf_files
+
+
+@pytest.mark.dask
 def test_object_to_source_with_leaves(
     dask_client, tmp_path, small_sky_object_catalog, small_sky_source_catalog, assert_text_file_matches
 ):
     """Test creating association between object and source catalogs."""
     small_sky_soap_args = SoapArguments(
         object_catalog_dir=small_sky_object_catalog,
         object_id_column="id",
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_arguments.py` & `hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_map_reduce.py` & `hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_map_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             "join_Npix",
             "num_rows",
         ],
     )
     partitions_csv_file = os.path.join(input_path, "0_11.csv")
     join_info.to_csv(partitions_csv_file, index=False)
 
-    total_num_rows = combine_partial_results(input_path, output_path)
+    total_num_rows = combine_partial_results(input_path, output_path, None)
     assert total_num_rows == 131
 
     result = pd.read_csv(os.path.join(output_path, "partition_join_info.csv"))
     assert len(result) == 2
 
     result = pd.read_csv(os.path.join(output_path, "unmatched_sources.csv"))
     assert len(result) == 1
```

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/soap/test_soap_resume_plan.py` & `hipscat-import-0.2.6/tests/hipscat_import/soap/test_soap_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/test_pipeline_resume_plan.py` & `hipscat-import-0.2.6/tests/hipscat_import/test_pipeline_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/test_runtime_arguments.py` & `hipscat-import-0.2.6/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/verification/test_run_verification.py` & `hipscat-import-0.2.6/tests/hipscat_import/verification/test_run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.2.5/tests/hipscat_import/verification/test_verification_arguments.py` & `hipscat-import-0.2.6/tests/hipscat_import/verification/test_verification_arguments.py`

 * *Files identical despite different names*

