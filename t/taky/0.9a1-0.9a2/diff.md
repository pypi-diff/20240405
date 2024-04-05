# Comparing `tmp/taky-0.9a1.tar.gz` & `tmp/taky-0.9a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taky-0.9a1.tar", last modified: Sat Jan  1 17:20:46 2022, max compression
+gzip compressed data, was "taky-0.9a2.tar", last modified: Mon Jan 10 13:54:22 2022, max compression
```

## Comparing `taky-0.9a1.tar` & `taky-0.9a2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.096140 taky-0.9a1/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      163 2021-05-31 14:38:20.000000 taky-0.9a1/.coveragerc
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.088140 taky-0.9a1/.github/
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.088140 taky-0.9a1/.github/workflows/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2298 2021-05-31 14:38:20.000000 taky-0.9a1/.github/workflows/pylint.yml
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      157 2021-09-02 14:18:08.000000 taky-0.9a1/.gitignore
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      256 2021-03-05 22:51:07.000000 taky-0.9a1/.pre-commit-config.yaml
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    18104 2021-11-24 15:10:22.000000 taky-0.9a1/.pylintrc
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3783 2022-01-01 17:16:23.000000 taky-0.9a1/CHANGELOG
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1062 2021-01-18 14:09:53.000000 taky-0.9a1/LICENSE
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6153 2022-01-01 17:20:46.096140 taky-0.9a1/PKG-INFO
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4669 2021-05-31 14:38:20.000000 taky-0.9a1/README.md
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/doc/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10500 2022-01-01 16:54:45.000000 taky-0.9a1/doc/README_DEPLOYMENT.md
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1199 2021-09-03 13:55:06.000000 taky-0.9a1/doc/README_DEVELOPMENT.md
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6613 2021-11-24 16:50:52.000000 taky-0.9a1/doc/README_FEATURE_COMPARISON.md
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2622 2022-01-01 16:57:55.000000 taky-0.9a1/doc/README_QUICKSTART.md
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6768 2021-09-04 11:57:54.000000 taky-0.9a1/doc/README_SECURITY.md
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       21 2021-05-31 14:38:20.000000 taky-0.9a1/requirements-dev.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       46 2021-03-08 00:31:44.000000 taky-0.9a1/requirements.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       38 2022-01-01 17:20:46.096140 taky-0.9a1/setup.cfg
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1100 2021-03-05 22:51:07.000000 taky-0.9a1/setup.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/taky/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      181 2022-01-01 15:40:31.000000 taky-0.9a1/taky/__init__.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/taky/cli/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      227 2022-01-01 15:18:18.000000 taky-0.9a1/taky/cli/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1791 2022-01-01 15:18:18.000000 taky-0.9a1/taky/cli/__main__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3929 2021-11-24 15:18:12.000000 taky-0.9a1/taky/cli/build_client_cmd.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3723 2022-01-01 15:44:07.000000 taky-0.9a1/taky/cli/mgmt_cmds.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     5253 2021-11-27 17:29:45.000000 taky-0.9a1/taky/cli/setup_taky_cmd.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6445 2021-11-24 15:18:12.000000 taky-0.9a1/taky/cli/systemd_cmd.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4052 2022-01-01 15:49:41.000000 taky-0.9a1/taky/config.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/taky/cot/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      112 2021-02-27 14:53:56.000000 taky-0.9a1/taky/cot/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2861 2021-11-24 15:18:12.000000 taky-0.9a1/taky/cot/__main__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10787 2022-01-01 15:14:26.000000 taky-0.9a1/taky/cot/client.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2800 2022-01-01 15:44:07.000000 taky-0.9a1/taky/cot/mgmt.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/taky/cot/models/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      363 2021-03-05 22:51:07.000000 taky-0.9a1/taky/cot/models/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1470 2021-11-24 15:10:22.000000 taky-0.9a1/taky/cot/models/detail.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      105 2021-03-05 22:51:07.000000 taky-0.9a1/taky/cot/models/errors.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3294 2021-10-14 02:31:53.000000 taky-0.9a1/taky/cot/models/event.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4820 2021-09-02 14:10:17.000000 taky-0.9a1/taky/cot/models/geochat.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1467 2021-10-14 02:31:53.000000 taky-0.9a1/taky/cot/models/point.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4289 2021-10-14 02:31:53.000000 taky-0.9a1/taky/cot/models/takuser.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      359 2021-03-05 22:51:07.000000 taky-0.9a1/taky/cot/models/teams.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     9235 2022-01-01 15:18:07.000000 taky-0.9a1/taky/cot/persistence.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4430 2022-01-01 14:17:21.000000 taky-0.9a1/taky/cot/router.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10084 2022-01-01 15:31:19.000000 taky-0.9a1/taky/cot/server.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.096140 taky-0.9a1/taky/dps/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      662 2021-11-24 15:18:12.000000 taky-0.9a1/taky/dps/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4714 2022-01-01 15:31:19.000000 taky-0.9a1/taky/dps/__main__.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.096140 taky-0.9a1/taky/dps/views/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      106 2021-05-31 14:38:20.000000 taky-0.9a1/taky/dps/views/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     5502 2021-11-24 15:18:12.000000 taky-0.9a1/taky/dps/views/datapackage.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      652 2021-03-05 22:51:07.000000 taky-0.9a1/taky/dps/views/index.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      766 2021-03-05 22:51:07.000000 taky-0.9a1/taky/dps/views/kml.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      486 2021-12-31 18:24:10.000000 taky-0.9a1/taky/dps/views/version.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2656 2021-11-24 15:10:22.000000 taky-0.9a1/taky/dps/views/video.py
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.096140 taky-0.9a1/taky/util/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1501 2021-11-24 15:10:22.000000 taky-0.9a1/taky/util/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2081 2021-09-02 14:10:17.000000 taky-0.9a1/taky/util/datapackage.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3459 2021-09-02 14:10:17.000000 taky-0.9a1/taky/util/rotc.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4944 2021-03-05 22:51:07.000000 taky-0.9a1/taky/util/xmldeclstrip.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1232 2021-11-24 15:18:12.000000 taky-0.9a1/taky.conf.sample
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.092140 taky-0.9a1/taky.egg-info/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6153 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/PKG-INFO
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1484 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/SOURCES.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)        1 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/dependency_links.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      116 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/entry_points.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)        1 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/not-zip-safe
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       46 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/requires.txt
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       11 2022-01-01 17:20:45.000000 taky-0.9a1/taky.egg-info/top_level.txt
-drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-01 17:20:46.096140 taky-0.9a1/tests/
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      695 2021-06-03 13:31:27.000000 taky-0.9a1/tests/__init__.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2918 2021-06-03 13:31:27.000000 taky-0.9a1/tests/test_cot_event.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1679 2021-11-24 15:10:22.000000 taky-0.9a1/tests/test_geo_chat.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3789 2022-01-01 14:29:04.000000 taky-0.9a1/tests/test_router.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      828 2021-11-24 15:10:22.000000 taky-0.9a1/tests/test_takclient.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1478 2021-05-31 17:59:29.000000 taky-0.9a1/tests/test_takuser.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1638 2021-05-31 14:38:20.000000 taky-0.9a1/tests/test_xmldeclstrip.py
--rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      330 2021-05-31 14:38:20.000000 taky-0.9a1/tox.ini
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.060832 taky-0.9a2/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      163 2021-05-31 14:38:20.000000 taky-0.9a2/.coveragerc
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.052832 taky-0.9a2/.github/
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.052832 taky-0.9a2/.github/workflows/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2295 2022-01-05 04:38:38.000000 taky-0.9a2/.github/workflows/pylint.yml
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      157 2022-01-05 03:45:33.000000 taky-0.9a2/.gitignore
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      256 2021-03-05 22:51:07.000000 taky-0.9a2/.pre-commit-config.yaml
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    18104 2022-01-05 03:46:51.000000 taky-0.9a2/.pylintrc
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3783 2022-01-05 03:46:51.000000 taky-0.9a2/CHANGELOG
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1062 2021-01-18 14:09:53.000000 taky-0.9a2/LICENSE
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6644 2022-01-10 13:54:22.060832 taky-0.9a2/PKG-INFO
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     5104 2022-01-05 04:13:13.000000 taky-0.9a2/README.md
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.052832 taky-0.9a2/doc/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10500 2022-01-05 03:46:51.000000 taky-0.9a2/doc/README_DEPLOYMENT.md
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1199 2022-01-05 03:45:33.000000 taky-0.9a2/doc/README_DEVELOPMENT.md
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6613 2022-01-05 03:46:51.000000 taky-0.9a2/doc/README_FEATURE_COMPARISON.md
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2622 2022-01-05 03:46:51.000000 taky-0.9a2/doc/README_QUICKSTART.md
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6768 2022-01-05 03:45:33.000000 taky-0.9a2/doc/README_SECURITY.md
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       21 2022-01-05 03:45:33.000000 taky-0.9a2/requirements-dev.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       46 2021-03-08 00:31:44.000000 taky-0.9a2/requirements.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       38 2022-01-10 13:54:22.060832 taky-0.9a2/setup.cfg
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1100 2021-03-05 22:51:07.000000 taky-0.9a2/setup.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.052832 taky-0.9a2/taky/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      181 2022-01-05 03:46:51.000000 taky-0.9a2/taky/__init__.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.056832 taky-0.9a2/taky/cli/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      227 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1791 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/__main__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3929 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/build_client_cmd.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3723 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/mgmt_cmds.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     5253 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/setup_taky_cmd.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6445 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cli/systemd_cmd.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3992 2022-01-05 03:50:53.000000 taky-0.9a2/taky/config.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.056832 taky-0.9a2/taky/cot/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      112 2021-02-27 14:53:56.000000 taky-0.9a2/taky/cot/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2861 2022-01-10 13:53:50.000000 taky-0.9a2/taky/cot/__main__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10787 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/client.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2800 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/mgmt.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.056832 taky-0.9a2/taky/cot/models/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      363 2021-03-05 22:51:07.000000 taky-0.9a2/taky/cot/models/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1470 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/models/detail.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      105 2021-03-05 22:51:07.000000 taky-0.9a2/taky/cot/models/errors.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3294 2022-01-05 03:45:33.000000 taky-0.9a2/taky/cot/models/event.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4820 2022-01-05 03:45:33.000000 taky-0.9a2/taky/cot/models/geochat.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1467 2022-01-05 03:45:33.000000 taky-0.9a2/taky/cot/models/point.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4289 2022-01-05 03:45:33.000000 taky-0.9a2/taky/cot/models/takuser.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      359 2021-03-05 22:51:07.000000 taky-0.9a2/taky/cot/models/teams.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     9235 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/persistence.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4430 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/router.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)    10153 2022-01-05 03:46:51.000000 taky-0.9a2/taky/cot/server.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.056832 taky-0.9a2/taky/dps/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      662 2022-01-05 03:46:51.000000 taky-0.9a2/taky/dps/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4714 2022-01-05 03:46:51.000000 taky-0.9a2/taky/dps/__main__.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.060832 taky-0.9a2/taky/dps/views/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      106 2021-05-31 14:38:20.000000 taky-0.9a2/taky/dps/views/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     5502 2022-01-05 03:46:51.000000 taky-0.9a2/taky/dps/views/datapackage.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      652 2021-03-05 22:51:07.000000 taky-0.9a2/taky/dps/views/index.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      766 2021-03-05 22:51:07.000000 taky-0.9a2/taky/dps/views/kml.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      486 2022-01-05 03:46:51.000000 taky-0.9a2/taky/dps/views/version.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2656 2022-01-05 03:46:51.000000 taky-0.9a2/taky/dps/views/video.py
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.060832 taky-0.9a2/taky/util/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1501 2022-01-05 03:46:51.000000 taky-0.9a2/taky/util/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2081 2021-09-02 14:10:17.000000 taky-0.9a2/taky/util/datapackage.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3459 2021-09-02 14:10:17.000000 taky-0.9a2/taky/util/rotc.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     4944 2021-03-05 22:51:07.000000 taky-0.9a2/taky/util/xmldeclstrip.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1232 2022-01-05 03:46:51.000000 taky-0.9a2/taky.conf.sample
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.056832 taky-0.9a2/taky.egg-info/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     6644 2022-01-10 13:54:21.000000 taky-0.9a2/taky.egg-info/PKG-INFO
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1484 2022-01-10 13:54:22.000000 taky-0.9a2/taky.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)        1 2022-01-10 13:54:21.000000 taky-0.9a2/taky.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      116 2022-01-10 13:54:21.000000 taky-0.9a2/taky.egg-info/entry_points.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)        1 2022-01-10 13:51:00.000000 taky-0.9a2/taky.egg-info/not-zip-safe
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       46 2022-01-10 13:54:21.000000 taky-0.9a2/taky.egg-info/requires.txt
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)       11 2022-01-10 13:54:21.000000 taky-0.9a2/taky.egg-info/top_level.txt
+drwxrwxr-x   0 tkuester  (1000) tkuester  (1000)        0 2022-01-10 13:54:22.060832 taky-0.9a2/tests/
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      695 2022-01-05 03:45:33.000000 taky-0.9a2/tests/__init__.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     2918 2021-06-03 13:31:27.000000 taky-0.9a2/tests/test_cot_event.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1679 2022-01-05 03:46:51.000000 taky-0.9a2/tests/test_geo_chat.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     3789 2022-01-05 03:46:51.000000 taky-0.9a2/tests/test_router.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      828 2022-01-05 03:46:51.000000 taky-0.9a2/tests/test_takclient.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1478 2022-01-05 03:45:33.000000 taky-0.9a2/tests/test_takuser.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)     1638 2022-01-05 03:45:33.000000 taky-0.9a2/tests/test_xmldeclstrip.py
+-rw-rw-r--   0 tkuester  (1000) tkuester  (1000)      330 2022-01-05 03:45:33.000000 taky-0.9a2/tox.ini
```

### Comparing `taky-0.9a1/.github/workflows/pylint.yml` & `taky-0.9a2/.github/workflows/pylint.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       run: |
         python -m pip install --upgrade pip
         [ -f "requirements.txt" ] && pip install -r requirements.txt
         pip install pylint coverage
     - id: pylint
       name: Analyzing the code with pylint
       run: |
-        python3 -c "from pylint.lint import Run; ret = Run(['taky'], do_exit=False); print('::set-output name=score::%.2f' % ret.linter.stats['global_note'])"
+        python3 -c "from pylint.lint import Run; ret = Run(['taky'], do_exit=False); print('::set-output name=score::%.2f' % ret.linter.stats.global_note)"
     - id: tests
       name: Running unit tests, generating coverage
       run: |
         coverage run -m unittest || true
         COV_PCT=$(coverage report --include="taky/**" | awk '/TOTAL/{ print $NF }')
         echo "::set-output name=cov-pct::${COV_PCT}"
   badges:
```

### Comparing `taky-0.9a1/.pylintrc` & `taky-0.9a2/.pylintrc`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/CHANGELOG` & `taky-0.9a2/CHANGELOG`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/LICENSE` & `taky-0.9a2/LICENSE`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/PKG-INFO` & `taky-0.9a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taky
-Version: 0.9a1
+Version: 0.9a2
 Summary: A simple TAK server and COT router
 Home-page: https://github.com/tkuester/taky
 Author: Tim K
 Author-email: tpkuester@gmail.com
 License: UNKNOWN
 Description: # taky
         
@@ -114,25 +114,32 @@
         See the README_QUICKSTART.md guide in the `/doc` folder to get up and running!
         For more advanced setups, look at the README_DEPLOYMENT.md file!
         
         ## Development Status
         
         As far as the "Unicorn Test Readiness Level" goes, `taky` is not a high
         heritage space unicorn. We are somewhere between TRL 5 and 6. The horse is
-        outside, and we're tentatively calling it a unicorn.
+        outside, and we're tentatively calling it a unicorn. Users have reported that
+        `taky` worked well on ANW2C networks, L3Harris radios, passed custom COT
+        messages without complaint, and was even found in the field with coalition
+        forces!
         
         The COT server is the most mature part of the codebase. While some of the more
         esoteric configurations have not been tested, the standard SSL setup seems to
-        be rather solid, and performs well with heavy loads.
+        be rather solid, and performs well with heavy loads. That being said, there is
+        a known memory leak with the XML parser that hasn't been resolved.
         
         The Data Package server (DPS) is starting to mature, but has not been as
         extensively tested. Simple client-to-client and client-to-server transfers seem
         to work well, although some features like Video and posting tracks have not
         been implemented yet.
         
+        All said and done, don't trust this software with lives, wellbeing, or anything
+        of value. This software wasn't written with a "mission critical" level-of-care.
+        
         Feel free to checkout the
         [milestones](https://github.com/tkuester/taky/milestones) page to see what is
         planned for the next version of taky! Pull requests and issues are welcome!
         
 Platform: UNKNOWN
 Classifier: Topic :: Communications
 Classifier: Development Status :: 4 - Beta
```

### Comparing `taky-0.9a1/README.md` & `taky-0.9a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,21 +106,28 @@
 See the README_QUICKSTART.md guide in the `/doc` folder to get up and running!
 For more advanced setups, look at the README_DEPLOYMENT.md file!
 
 ## Development Status
 
 As far as the "Unicorn Test Readiness Level" goes, `taky` is not a high
 heritage space unicorn. We are somewhere between TRL 5 and 6. The horse is
-outside, and we're tentatively calling it a unicorn.
+outside, and we're tentatively calling it a unicorn. Users have reported that
+`taky` worked well on ANW2C networks, L3Harris radios, passed custom COT
+messages without complaint, and was even found in the field with coalition
+forces!
 
 The COT server is the most mature part of the codebase. While some of the more
 esoteric configurations have not been tested, the standard SSL setup seems to
-be rather solid, and performs well with heavy loads.
+be rather solid, and performs well with heavy loads. That being said, there is
+a known memory leak with the XML parser that hasn't been resolved.
 
 The Data Package server (DPS) is starting to mature, but has not been as
 extensively tested. Simple client-to-client and client-to-server transfers seem
 to work well, although some features like Video and posting tracks have not
 been implemented yet.
 
+All said and done, don't trust this software with lives, wellbeing, or anything
+of value. This software wasn't written with a "mission critical" level-of-care.
+
 Feel free to checkout the
 [milestones](https://github.com/tkuester/taky/milestones) page to see what is
 planned for the next version of taky! Pull requests and issues are welcome!
```

### Comparing `taky-0.9a1/doc/README_DEPLOYMENT.md` & `taky-0.9a2/doc/README_DEPLOYMENT.md`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/doc/README_DEVELOPMENT.md` & `taky-0.9a2/doc/README_DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/doc/README_FEATURE_COMPARISON.md` & `taky-0.9a2/doc/README_FEATURE_COMPARISON.md`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/doc/README_QUICKSTART.md` & `taky-0.9a2/doc/README_QUICKSTART.md`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/doc/README_SECURITY.md` & `taky-0.9a2/doc/README_SECURITY.md`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/setup.py` & `taky-0.9a2/setup.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cli/__main__.py` & `taky-0.9a2/taky/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cli/build_client_cmd.py` & `taky-0.9a2/taky/cli/build_client_cmd.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cli/mgmt_cmds.py` & `taky-0.9a2/taky/cli/mgmt_cmds.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cli/setup_taky_cmd.py` & `taky-0.9a2/taky/cli/setup_taky_cmd.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cli/systemd_cmd.py` & `taky-0.9a2/taky/cli/systemd_cmd.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/config.py` & `taky-0.9a2/taky/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,24 @@
     @param explicit Don't return a default
     """
     if path is None:
         if os.path.exists("taky.conf"):
             path = os.path.abspath("taky.conf")
         elif os.path.exists("/etc/taky/taky.conf"):
             path = "/etc/taky/taky.conf"
-        else:
-            raise FileNotFoundError("Unable to find config file")
 
-    if explicit and not os.path.exists(path):
+    if explicit and not (path and os.path.exists(path)):
         raise FileNotFoundError("Config file required, but not present")
 
     ret_config = configparser.ConfigParser(allow_no_value=True)
     ret_config.read_dict(DEFAULT_CFG)
 
     lgr = logging.getLogger("load_config")
 
-    if os.path.exists(path):
+    if path and os.path.exists(path):
         lgr.info("Loading config file from %s", path)
         with open(path, "r") as cfg_fp:
             ret_config.read_file(cfg_fp, source=path)
 
     # TODO: Deprecate
     if ret_config.has_option("taky", "hostname") or ret_config.has_option(
         "taky", "public_ip"
```

### Comparing `taky-0.9a1/taky/cot/__main__.py` & `taky-0.9a2/taky/cot/__main__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/client.py` & `taky-0.9a2/taky/cot/client.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/mgmt.py` & `taky-0.9a2/taky/cot/mgmt.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/models/detail.py` & `taky-0.9a2/taky/cot/models/detail.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/models/event.py` & `taky-0.9a2/taky/cot/models/event.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/models/geochat.py` & `taky-0.9a2/taky/cot/models/geochat.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/models/point.py` & `taky-0.9a2/taky/cot/models/point.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/models/takuser.py` & `taky-0.9a2/taky/cot/models/takuser.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/persistence.py` & `taky-0.9a2/taky/cot/persistence.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/router.py` & `taky-0.9a2/taky/cot/router.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/cot/server.py` & `taky-0.9a2/taky/cot/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,16 @@
         self.router.client_connect(client)
 
     def client_disconnect(self, client, reason=None):
         """
         Disconnect a client from the server
         """
         client.disconnect(reason)
-        client = self.clients.pop(client.sock)
+        if client.sock in self.clients:
+            client = self.clients.pop(client.sock)
 
         if isinstance(client, TAKClient):
             self.router.client_disconnect(client)
 
     def loop(self):
         """
         Main loop. Call outside this object in a "while True" block.
@@ -273,14 +274,15 @@
 
         # Prune sockets
         now = time.time()
         prune_sox = list(self.clients.items())
         for (sock, client) in prune_sox:
             if client.is_closed:
                 self.client_disconnect(client, "Is closed")
+                continue
 
             if not client.ready and (now - client.connected) > 10:
                 self.client_disconnect(client, "SSL Handshake timeout")
 
     def shutdown(self):
         """
         Disconnect all clients, close server socket.
```

### Comparing `taky-0.9a1/taky/dps/__init__.py` & `taky-0.9a2/taky/dps/__init__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/dps/__main__.py` & `taky-0.9a2/taky/dps/__main__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/dps/views/datapackage.py` & `taky-0.9a2/taky/dps/views/datapackage.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/dps/views/index.py` & `taky-0.9a2/taky/dps/views/index.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/dps/views/kml.py` & `taky-0.9a2/taky/dps/views/kml.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/dps/views/video.py` & `taky-0.9a2/taky/dps/views/video.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/util/__init__.py` & `taky-0.9a2/taky/util/__init__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/util/datapackage.py` & `taky-0.9a2/taky/util/datapackage.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/util/rotc.py` & `taky-0.9a2/taky/util/rotc.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky/util/xmldeclstrip.py` & `taky-0.9a2/taky/util/xmldeclstrip.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky.conf.sample` & `taky-0.9a2/taky.conf.sample`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/taky.egg-info/PKG-INFO` & `taky-0.9a2/taky.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taky
-Version: 0.9a1
+Version: 0.9a2
 Summary: A simple TAK server and COT router
 Home-page: https://github.com/tkuester/taky
 Author: Tim K
 Author-email: tpkuester@gmail.com
 License: UNKNOWN
 Description: # taky
         
@@ -114,25 +114,32 @@
         See the README_QUICKSTART.md guide in the `/doc` folder to get up and running!
         For more advanced setups, look at the README_DEPLOYMENT.md file!
         
         ## Development Status
         
         As far as the "Unicorn Test Readiness Level" goes, `taky` is not a high
         heritage space unicorn. We are somewhere between TRL 5 and 6. The horse is
-        outside, and we're tentatively calling it a unicorn.
+        outside, and we're tentatively calling it a unicorn. Users have reported that
+        `taky` worked well on ANW2C networks, L3Harris radios, passed custom COT
+        messages without complaint, and was even found in the field with coalition
+        forces!
         
         The COT server is the most mature part of the codebase. While some of the more
         esoteric configurations have not been tested, the standard SSL setup seems to
-        be rather solid, and performs well with heavy loads.
+        be rather solid, and performs well with heavy loads. That being said, there is
+        a known memory leak with the XML parser that hasn't been resolved.
         
         The Data Package server (DPS) is starting to mature, but has not been as
         extensively tested. Simple client-to-client and client-to-server transfers seem
         to work well, although some features like Video and posting tracks have not
         been implemented yet.
         
+        All said and done, don't trust this software with lives, wellbeing, or anything
+        of value. This software wasn't written with a "mission critical" level-of-care.
+        
         Feel free to checkout the
         [milestones](https://github.com/tkuester/taky/milestones) page to see what is
         planned for the next version of taky! Pull requests and issues are welcome!
         
 Platform: UNKNOWN
 Classifier: Topic :: Communications
 Classifier: Development Status :: 4 - Beta
```

### Comparing `taky-0.9a1/taky.egg-info/SOURCES.txt` & `taky-0.9a2/taky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/__init__.py` & `taky-0.9a2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_cot_event.py` & `taky-0.9a2/tests/test_cot_event.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_geo_chat.py` & `taky-0.9a2/tests/test_geo_chat.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_router.py` & `taky-0.9a2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_takclient.py` & `taky-0.9a2/tests/test_takclient.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_takuser.py` & `taky-0.9a2/tests/test_takuser.py`

 * *Files identical despite different names*

### Comparing `taky-0.9a1/tests/test_xmldeclstrip.py` & `taky-0.9a2/tests/test_xmldeclstrip.py`

 * *Files identical despite different names*

