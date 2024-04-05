# Comparing `tmp/bolton-clack-0.3.8.tar.gz` & `tmp/bolton-clack-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolton-clack-0.3.8.tar", last modified: Thu Mar  7 15:07:19 2024, max compression
+gzip compressed data, was "bolton-clack-0.3.9.tar", last modified: Thu Mar  7 17:48:31 2024, max compression
```

## Comparing `bolton-clack-0.3.8.tar` & `bolton-clack-0.3.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.087848 bolton-clack-0.3.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.087848 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/clack.pytest_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/clack.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/clack.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/clack.xdg.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.091848 bolton-clack-0.3.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.083848 bolton-clack-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/src/bolton_clack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-07 15:07:19.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-07 15:07:19.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:07:19.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:07:15.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-07 15:07:19.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 15:07:19.000000 bolton-clack-0.3.8/src/bolton_clack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.095848 bolton-clack-0.3.8/src/clack/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_dynvars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/src/clack/xdg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.095848 bolton-clack-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    23814 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/__snapshots__/test_log.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:07:19.099848 bolton-clack-0.3.8/tests/data/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/data/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/data/e2e/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/data/e2e/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/e2e_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/test_clack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tests/test_xdg.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-07 15:07:10.000000 bolton-clack-0.3.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.816513 bolton-clack-0.3.9/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.820513 bolton-clack-0.3.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.820513 bolton-clack-0.3.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.820513 bolton-clack-0.3.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/clack.pytest_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/clack.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/clack.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/clack.xdg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.820513 bolton-clack-0.3.9/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.820513 bolton-clack-0.3.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.808513 bolton-clack-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/src/bolton_clack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-07 17:48:31.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-07 17:48:31.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 17:48:31.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 17:48:27.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-07 17:48:31.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 17:48:31.000000 bolton-clack-0.3.9/src/bolton_clack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.824513 bolton-clack-0.3.9/src/clack/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_dynvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/src/clack/xdg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.824513 bolton-clack-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.824513 bolton-clack-0.3.9/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    23814 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/__snapshots__/test_log.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:48:31.828513 bolton-clack-0.3.9/tests/data/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/data/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/data/e2e/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/data/e2e/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/e2e_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/test_clack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tests/test_xdg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-07 17:48:21.000000 bolton-clack-0.3.9/tox.ini
```

### Comparing `bolton-clack-0.3.8/.cruft.json` & `bolton-clack-0.3.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/.github/labels.yml` & `bolton-clack-0.3.9/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/.github/workflows/ci.yml` & `bolton-clack-0.3.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/.gitignore` & `bolton-clack-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/.pylintrc` & `bolton-clack-0.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/.readthedocs.yml` & `bolton-clack-0.3.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/CHANGELOG.md` & `bolton-clack-0.3.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,26 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/python-boltons/clack/compare/0.3.8...HEAD)
+## [Unreleased](https://github.com/python-boltons/clack/compare/0.3.9...HEAD)
 
 No notable changes have been made.
 
 
+## [0.3.9](https://github.com/python-boltons/clack/compare/0.3.8...0.3.9) - 2024-03-07
+
+### Added
+
+* Exposed the `clack_envvars_set()` method to the public clack API.
+
+
 ## [0.3.8](https://github.com/python-boltons/clack/compare/0.3.7...0.3.8) - 2024-03-07
 
 ### Added
 
 * Added support for reading `-v` option when initializing logrus the first time.
 
 ### Changed
```

### Comparing `bolton-clack-0.3.8/CONTRIBUTING.md` & `bolton-clack-0.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/Dockerfile` & `bolton-clack-0.3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/Makefile` & `bolton-clack-0.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/PKG-INFO` & `bolton-clack-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bolton-clack
-Version: 0.3.8
+Version: 0.3.9
 Summary: command-line application configuration kit (CLACK)... A wrapper around the `argparse` library that aims to handle _all_ application configuration.
 Home-page: https://github.com/python-boltons/clack
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: bolton-eris~=0.2.2
 Requires-Dist: bolton-logrus~=0.1.0
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: pydantic~=1.8
 Requires-Dist: pyyaml~=6.0
```

### Comparing `bolton-clack-0.3.8/README.md` & `bolton-clack-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/bin/check_cc` & `bolton-clack-0.3.9/bin/check_cc`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/bin/publish_docs` & `bolton-clack-0.3.9/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/bin/quick-lints` & `bolton-clack-0.3.9/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/bin/render_all_cogs` & `bolton-clack-0.3.9/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/docs/Makefile` & `bolton-clack-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/docs/make.bat` & `bolton-clack-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/docs/source/conf.py` & `bolton-clack-0.3.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/lib/bugyi.sh` & `bolton-clack-0.3.9/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/requirements-dev.in` & `bolton-clack-0.3.9/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/requirements-dev.txt` & `bolton-clack-0.3.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/requirements.txt` & `bolton-clack-0.3.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/setup.cfg` & `bolton-clack-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/setup.py` & `bolton-clack-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 ###############################################################################
 DESCRIPTION = (
     "command-line application configuration kit (CLACK)... A wrapper around"
     " the `argparse` library that aims to handle _all_ application"
     " configuration."
 )
 SUPPORTED_PYTHON_VERSIONS = [
-    (3, 8),
     (3, 9),
     (3, 10),
+    (3, 11),
+    (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.3.8"}
+USE_SCM_VERSION = {"fallback_version": "0.3.9"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `bolton-clack-0.3.8/src/bolton_clack.egg-info/PKG-INFO` & `bolton-clack-0.3.9/src/bolton_clack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bolton-clack
-Version: 0.3.8
+Version: 0.3.9
 Summary: command-line application configuration kit (CLACK)... A wrapper around the `argparse` library that aims to handle _all_ application configuration.
 Home-page: https://github.com/python-boltons/clack
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: bolton-eris~=0.2.2
 Requires-Dist: bolton-logrus~=0.1.0
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: pydantic~=1.8
 Requires-Dist: pyyaml~=6.0
```

### Comparing `bolton-clack-0.3.8/src/bolton_clack.egg-info/SOURCES.txt` & `bolton-clack-0.3.9/src/bolton_clack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/__init__.py` & `bolton-clack-0.3.9/src/clack/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 """
 
 import logging as _logging
 
 from . import types, xdg
 from ._config import Config
 from ._config_file import YAMLConfigFile
-from ._dynvars import get_config
+from ._dynvars import clack_envvars_set, get_config
 from ._helpers import (
     comma_list_or_file,
     filter_cli_args,
     new_command_factory,
     register_runner_factory,
 )
 from ._main import main_factory
 from ._parser import Parser
 
 
 __all__ = [
     "Config",
     "Parser",
     "YAMLConfigFile",
+    "clack_envvars_set",
     "comma_list_or_file",
     "filter_cli_args",
     "get_config",
     "main_factory",
     "new_command_factory",
     "register_runner_factory",
     "types",
     "xdg",
 ]
 
 __author__ = "Bryan M Bugyi"
 __email__ = "bryanbugyi34@gmail.com"
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())
```

### Comparing `bolton-clack-0.3.8/src/clack/_config.py` & `bolton-clack-0.3.9/src/clack/_config.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/_config_file.py` & `bolton-clack-0.3.9/src/clack/_config_file.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/_dynvars.py` & `bolton-clack-0.3.9/src/clack/_dynvars.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/_helpers.py` & `bolton-clack-0.3.9/src/clack/_helpers.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/_main.py` & `bolton-clack-0.3.9/src/clack/_main.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/_parser.py` & `bolton-clack-0.3.9/src/clack/_parser.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/pytest_plugin.py` & `bolton-clack-0.3.9/src/clack/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/types.py` & `bolton-clack-0.3.9/src/clack/types.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/src/clack/xdg.py` & `bolton-clack-0.3.9/src/clack/xdg.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/targets.mk` & `bolton-clack-0.3.9/targets.mk`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/__snapshots__/test_log.ambr` & `bolton-clack-0.3.9/tests/__snapshots__/test_log.ambr`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/conftest.py` & `bolton-clack-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/data/e2e/simple.py` & `bolton-clack-0.3.9/tests/data/e2e/simple.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/data/e2e/subcommands.py` & `bolton-clack-0.3.9/tests/data/e2e/subcommands.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/e2e_helpers.py` & `bolton-clack-0.3.9/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/shared.py` & `bolton-clack-0.3.9/tests/shared.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/test_clack.py` & `bolton-clack-0.3.9/tests/test_clack.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/test_e2e.py` & `bolton-clack-0.3.9/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/test_log.py` & `bolton-clack-0.3.9/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `bolton-clack-0.3.8/tests/test_xdg.py` & `bolton-clack-0.3.9/tests/test_xdg.py`

 * *Files identical despite different names*

