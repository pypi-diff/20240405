# Comparing `tmp/potoroo-0.5.0.tar.gz` & `tmp/potoroo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potoroo-0.5.0.tar", last modified: Wed Apr  3 21:55:48 2024, max compression
+gzip compressed data, was "potoroo-0.6.0.tar", last modified: Fri Apr  5 05:17:18 2024, max compression
```

## Comparing `potoroo-0.5.0.tar` & `potoroo-0.6.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 21:55:40.000000 potoroo-0.5.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 21:55:40.000000 potoroo-0.5.0/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 21:55:40.000000 potoroo-0.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 21:55:40.000000 potoroo-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 21:55:40.000000 potoroo-0.5.0/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-03 21:55:40.000000 potoroo-0.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 21:55:40.000000 potoroo-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 21:55:40.000000 potoroo-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 21:55:40.000000 potoroo-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-03 21:55:40.000000 potoroo-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 21:55:40.000000 potoroo-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-03 21:55:40.000000 potoroo-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-03 21:55:48.947749 potoroo-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 21:55:40.000000 potoroo-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 21:55:40.000000 potoroo-0.5.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/potoroo.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-03 21:55:40.000000 potoroo-0.5.0/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 21:55:40.000000 potoroo-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 21:55:48.947749 potoroo-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-03 21:55:40.000000 potoroo-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.931748 potoroo-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/src/potoroo/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/_uow.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/src/potoroo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:55:45.000000 potoroo-0.5.0/src/potoroo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-03 21:55:40.000000 potoroo-0.5.0/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/test_potoroo.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 21:55:40.000000 potoroo-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.432897 potoroo-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 05:17:01.000000 potoroo-0.6.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 05:17:01.000000 potoroo-0.6.0/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 05:17:01.000000 potoroo-0.6.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:01.000000 potoroo-0.6.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.424897 potoroo-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.424897 potoroo-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 05:17:01.000000 potoroo-0.6.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-05 05:17:01.000000 potoroo-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 05:17:01.000000 potoroo-0.6.0/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-05 05:17:01.000000 potoroo-0.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-05 05:17:01.000000 potoroo-0.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-05 05:17:01.000000 potoroo-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 05:17:01.000000 potoroo-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-05 05:17:01.000000 potoroo-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-05 05:17:01.000000 potoroo-0.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 05:17:01.000000 potoroo-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-05 05:17:18.432897 potoroo-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-05 05:17:01.000000 potoroo-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-05 05:17:01.000000 potoroo-0.6.0/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-05 05:17:01.000000 potoroo-0.6.0/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-05 05:17:01.000000 potoroo-0.6.0/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-05 05:17:01.000000 potoroo-0.6.0/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 05:17:01.000000 potoroo-0.6.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/potoroo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 05:17:01.000000 potoroo-0.6.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:01.000000 potoroo-0.6.0/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-05 05:17:01.000000 potoroo-0.6.0/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 05:17:01.000000 potoroo-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 05:17:01.000000 potoroo-0.6.0/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-05 05:17:01.000000 potoroo-0.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 05:17:01.000000 potoroo-0.6.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-05 05:17:01.000000 potoroo-0.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 05:17:01.000000 potoroo-0.6.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-05 05:17:18.432897 potoroo-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-05 05:17:01.000000 potoroo-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.420897 potoroo-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.428897 potoroo-0.6.0/src/potoroo/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 05:17:01.000000 potoroo-0.6.0/src/potoroo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-05 05:17:01.000000 potoroo-0.6.0/src/potoroo/_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 05:17:01.000000 potoroo-0.6.0/src/potoroo/_uow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:01.000000 potoroo-0.6.0/src/potoroo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.432897 potoroo-0.6.0/src/potoroo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-05 05:17:18.000000 potoroo-0.6.0/src/potoroo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-05 05:17:18.000000 potoroo-0.6.0/src/potoroo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:17:18.000000 potoroo-0.6.0/src/potoroo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:17:12.000000 potoroo-0.6.0/src/potoroo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 05:17:18.000000 potoroo-0.6.0/src/potoroo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 05:17:18.000000 potoroo-0.6.0/src/potoroo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-05 05:17:01.000000 potoroo-0.6.0/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:17:18.432897 potoroo-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 05:17:01.000000 potoroo-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 05:17:01.000000 potoroo-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-05 05:17:01.000000 potoroo-0.6.0/tests/test_potoroo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 05:17:01.000000 potoroo-0.6.0/tox.ini
```

### Comparing `potoroo-0.5.0/.cruft.json` & `potoroo-0.6.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/.github/labels.yml` & `potoroo-0.6.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/.github/workflows/ci.yml` & `potoroo-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/.gitignore` & `potoroo-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/.pylintrc` & `potoroo-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/.readthedocs.yml` & `potoroo-0.6.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/CHANGELOG.md` & `potoroo-0.6.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,28 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/potoroo/compare/0.5.0...HEAD)
+## [Unreleased](https://github.com/bbugyi200/potoroo/compare/0.6.0...HEAD)
 
 No notable changes have been made.
 
 
+## [0.6.0](https://github.com/bbugyi200/potoroo/compare/0.5.0...0.6.0) - 2024-04-05
+
+### Changed
+
+* *BREAKING CHANGE*: Renamed `get_by_tag()` to `get_by_query()`.
+* *BREAKING CHANGE*: Renamed `remove_by_tag()` to `remove_by_query()`.
+* *BREAKING CHANGE*: Renamed `TaggedRepo` to `QueryRepo`.
+
+
 ## [0.5.0](https://github.com/bbugyi200/potoroo/compare/0.4.1...0.5.0) - 2024-04-03
 
 ### Changed
 
 * *BREAKING CHANGE*: Implement `remove_by_tag()` and `remove_by_key()` and
   change remove() to accept item.
```

### Comparing `potoroo-0.5.0/CONTRIBUTING.md` & `potoroo-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/Dockerfile` & `potoroo-0.6.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/Makefile` & `potoroo-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/PKG-INFO` & `potoroo-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potoroo
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python implementations of the Repository and UnitOfWork abstractions.
 Home-page: https://github.com/bbugyi200/potoroo
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `potoroo-0.5.0/README.md` & `potoroo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/bin/check_cc` & `potoroo-0.6.0/bin/check_cc`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/bin/publish_docs` & `potoroo-0.6.0/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/bin/quick-lints` & `potoroo-0.6.0/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/bin/render_all_cogs` & `potoroo-0.6.0/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/docs/Makefile` & `potoroo-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/docs/make.bat` & `potoroo-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/docs/source/conf.py` & `potoroo-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/lib/bugyi.sh` & `potoroo-0.6.0/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/requirements-dev.txt` & `potoroo-0.6.0/requirements-dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # via requests
 click==8.1.7
     # via
     #   black
     #   cookiecutter
     #   cruft
     #   pip-tools
-    #   typer-slim
+    #   typer
 cogapp==3.4.1
     # via -r requirements-dev.in
 cookiecutter==2.6.0
     # via cruft
 coverage[toml]==7.4.4
     # via pytest-cov
 cruft[pyproject]==2.15.0
@@ -166,19 +166,19 @@
 requests==2.31.0
     # via
     #   cookiecutter
     #   sphinx
 rich==13.7.1
     # via
     #   cookiecutter
-    #   typer-slim
+    #   typer
 setuptools-scm==8.0.4
     # via -r requirements-dev.in
 shellingham==1.5.4
-    # via typer-slim
+    # via typer
 six==1.16.0
     # via
     #   python-dateutil
     #   tox
 smmap==5.0.1
     # via gitdb
 snowballstemmer==2.2.0
@@ -232,31 +232,25 @@
     # via pylint
 tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
-typer==0.12.0
+typer==0.12.1
     # via cruft
-typer-cli==0.12.0
-    # via typer
-typer-slim[standard]==0.12.0
-    # via
-    #   typer
-    #   typer-cli
 types-python-dateutil==2.9.0.20240316
     # via arrow
 typing-extensions==4.10.0
     # via
     #   astroid
     #   black
     #   mypy
     #   setuptools-scm
-    #   typer-slim
+    #   typer
 urllib3==2.2.1
     # via requests
 virtualenv==20.25.1
     # via tox
 wheel==0.43.0
     # via pip-tools
```

### Comparing `potoroo-0.5.0/setup.cfg` & `potoroo-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/setup.py` & `potoroo-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "Python implementations of the Repository and UnitOfWork abstractions."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.5.0"}
+USE_SCM_VERSION = {"fallback_version": "0.6.0"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `potoroo-0.5.0/src/potoroo/_repo.py` & `potoroo-0.6.0/src/potoroo/_repo.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Generic, Optional, TypeVar
 
 from eris import ErisResult, Err, Ok
 
 
 K = TypeVar("K")
 V = TypeVar("V")
-T = TypeVar("T")
+Q = TypeVar("Q")
 
 
 class BasicRepo(Generic[K, V], abc.ABC):
     """The simplest possible Repository type."""
 
     @abc.abstractmethod
     def add(self, item: V, /, *, key: K = None) -> ErisResult[K]:
@@ -67,35 +67,36 @@
         return Ok(old_item)
 
     @abc.abstractmethod
     def all(self) -> ErisResult[list[V]]:
         """Retrieve all items stored in this repo."""
 
 
-class TaggedRepo(Repo[K, V], Generic[K, V, T], abc.ABC):
-    """A Repository that is aware of some kind of "tags".
+class QueryRepo(Repo[K, V], Generic[K, V, Q], abc.ABC):
+    """A Repository that is aware of some kind of "querys".
 
     Adds the ability to retrieve / delete a group of objects based off of some
-    arbitrary "tag" type.
+    arbitrary "query" type.
 
-    NOTE: In general, K can be expected to be a primitive type, whereas T is
+    NOTE: In general, K can be expected to be a primitive type, whereas Q is
       often a custom user-defined type.
     """
 
     @abc.abstractmethod
-    def get_by_tag(self, tag: T) -> ErisResult[list[V]]:
-        """Retrieve a group of items that meet the given tag's criteria."""
+    def get_by_query(self, query: Q) -> ErisResult[list[V]]:
+        """Retrieve a group of items that meet the given query's criteria."""
 
-    def remove_by_tag(self, tag: T) -> ErisResult[list[V]]:
-        """Remove a group of items that meet the given tag's criteria."""
-        items_result = self.get_by_tag(tag)
+    def remove_by_query(self, query: Q) -> ErisResult[list[V]]:
+        """Remove a group of items that meet the given query's criteria."""
+        items_result = self.get_by_query(query)
         err: Optional[Err] = None
         if isinstance(items_result, Err):
             err = Err(
-                "An error occurred while fetching items to be removed by tag."
+                "An error occurred while fetching items to be removed by"
+                " query."
             ).chain(items_result)
             return err
 
         deleted_items: list[V] = []
         items = items_result.ok()
         for item in items:
             deleted_item_result = self.remove(item)
```

### Comparing `potoroo-0.5.0/src/potoroo/_uow.py` & `potoroo-0.6.0/src/potoroo/_uow.py`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/src/potoroo.egg-info/PKG-INFO` & `potoroo-0.6.0/src/potoroo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potoroo
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python implementations of the Repository and UnitOfWork abstractions.
 Home-page: https://github.com/bbugyi200/potoroo
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `potoroo-0.5.0/src/potoroo.egg-info/SOURCES.txt` & `potoroo-0.6.0/src/potoroo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `potoroo-0.5.0/targets.mk` & `potoroo-0.6.0/targets.mk`

 * *Files identical despite different names*

