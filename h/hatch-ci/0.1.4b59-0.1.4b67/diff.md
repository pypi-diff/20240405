# Comparing `tmp/hatch_ci-0.1.4b59.tar.gz` & `tmp/hatch-ci-0.1.4b67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "hatch-ci-0.1.4b67.tar", last modified: Fri Apr  5 16:14:37 2024, max compression
```

## Comparing `hatch_ci-0.1.4b59.tar` & `hatch-ci-0.1.4b67.tar`

### file list

```diff
@@ -1,98 +1,41 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.gitattributes
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/Makefile
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/NOTES.txt
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/README.md.original
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/TEMPLATE.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/TEMPLATE.md.original
--rwxr-xr-x   0        0        0     9427 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/make.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.github/workflows/master.yml
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.github/workflows/tags.yml
--rw-r--r--   0        0        0    31488 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/jquery.ba-throttle-debounce.min.js
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/jquery.hotkeys.js
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/jquery.isonscreen.js
--rw-r--r--   0        0        0    89083 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/jquery.min.js
--rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/jquery.tablesorter.min.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci___init___py.html
--rw-r--r--   0        0        0    36483 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci__support_py.html
--rw-r--r--   0        0        0    41629 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_cli_py.html
--rw-r--r--   0        0        0    37413 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_code_py.html
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_common_py.html
--rw-r--r--   0        0        0    13737 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_exceptions_py.html
--rw-r--r--   0        0        0    47788 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_fileos_py.html
--rw-r--r--   0        0        0    24946 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_hook_build_py.html
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_hook_metadata_py.html
--rw-r--r--   0        0        0    11649 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_hook_version_py.html
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_hooks_py.html
--rw-r--r--   0        0        0    88093 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_scm_py.html
--rw-r--r--   0        0        0    50343 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_script_py.html
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_text_py.html
--rw-r--r--   0        0        0    98723 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/src_hatch_ci_tools_py.html
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    59582 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/_support.py.html
--rw-r--r--   0        0        0    24108 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/code.py.html
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/exceptions.py.html
--rw-r--r--   0        0        0    26126 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/fileos.py.html
--rw-r--r--   0        0        0    12817 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/hook_build.py.html
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/hook_metadata.py.html
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/hook_version.py.html
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    49055 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    30881 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/text.py.html
--rw-r--r--   0        0        0    66500 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/build/qa-3.12-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/__init__.py.original
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/_build.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/_support.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/cli.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/code.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/common.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/exceptions.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/fileos.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/hook_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/hook_metadata.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/hook_version.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/script.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/text.py
--rw-r--r--   0        0        0    11574 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/conftest.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/requirements.txt
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_cli.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_code.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_conftest.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_e2e.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_exceptions.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_fileos.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_scm.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_script.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_text.py
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/test_tools.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/data/foobar-0.0.0-py3-none-any.whl
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/data/foobar-0.0.0.tar.gz
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/data/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/support/__init__.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/support/projects.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/support/resolver.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/tests/support/scripter.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/LICENSE.txt
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/README.md
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/pyproject.toml
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 hatch_ci-0.1.4b59/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.774263 hatch-ci-0.1.4b67/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-05 16:14:35.000000 hatch-ci-0.1.4b67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:14:37.774263 hatch-ci-0.1.4b67/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.766263 hatch-ci-0.1.4b67/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/src/hatch_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hook_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/src/hatch_ci/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:14:37.000000 hatch-ci-0.1.4b67/src/hatch_ci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:14:37.770263 hatch-ci-0.1.4b67/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 16:13:58.000000 hatch-ci-0.1.4b67/tests/test_tools.py
```

### Comparing `hatch_ci-0.1.4b59/README.md.original` & `hatch-ci-0.1.4b67/README.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/_support.py` & `hatch-ci-0.1.4b67/src/hatch_ci/_support.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/cli.py` & `hatch-ci-0.1.4b67/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/code.py` & `hatch-ci-0.1.4b67/src/hatch_ci/code.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/exceptions.py` & `hatch-ci-0.1.4b67/src/hatch_ci/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/fileos.py` & `hatch-ci-0.1.4b67/src/hatch_ci/fileos.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/hook_build.py` & `hatch-ci-0.1.4b67/src/hatch_ci/hook_build.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/hook_version.py` & `hatch-ci-0.1.4b67/src/hatch_ci/hook_version.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/scm.py` & `hatch-ci-0.1.4b67/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/script.py` & `hatch-ci-0.1.4b67/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/text.py` & `hatch-ci-0.1.4b67/src/hatch_ci/text.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/src/hatch_ci/tools.py` & `hatch-ci-0.1.4b67/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_cli.py` & `hatch-ci-0.1.4b67/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_code.py` & `hatch-ci-0.1.4b67/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_conftest.py` & `hatch-ci-0.1.4b67/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_e2e.py` & `hatch-ci-0.1.4b67/tests/test_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import pytest
 from build.__main__ import main as build
 
 import hatch_ci
 from hatch_ci import fileos, text
 
+pytestmark = pytest.mark.skipif(True, reason="not ready yet")
+
 
 def T(txt: str) -> str:  # noqa: N802
     return text.indent(txt, pre="").replace("\r", "").rstrip("\n")
 
 
 @pytest.fixture(scope="function")
 def project(git_project_factory, monkeypatch):
```

### Comparing `hatch_ci-0.1.4b59/tests/test_exceptions.py` & `hatch-ci-0.1.4b67/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_fileos.py` & `hatch-ci-0.1.4b67/tests/test_fileos.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_scm.py` & `hatch-ci-0.1.4b67/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_script.py` & `hatch-ci-0.1.4b67/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_text.py` & `hatch-ci-0.1.4b67/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/tests/test_tools.py` & `hatch-ci-0.1.4b67/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/LICENSE.txt` & `hatch-ci-0.1.4b67/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.1.4b59/README.md` & `hatch-ci-0.1.4b67/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,40 @@
+Metadata-Version: 2.1
+Name: hatch-ci
+Version: 0.1.4b67
+Summary: Hatch plugin for ci system versioning
+Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
+License: MIT
+Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
+Project-URL: Source, https://github.com/cav71/hatch-ci
+Keywords: git,hatch,plugin,scm,version
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: hatchling>=1.1.0
+Requires-Dist: typing-extensions
+Requires-Dist: jinja2
+
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
-[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.1.4)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/0)
+[![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 > **NOTE** This is a beta branch!
 
@@ -142,8 +167,8 @@
 | `version-file` | `str` | None    | A file where to write __version__/__hash__ variables |
 | `paths` | `list[str]|str` | None | A list of paths to process |
 | `fixers` | `list[dict[str,str]]` | None | A list of dict, each key is a string to replace with the value |
 
 
 ## License
 
-`hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch_ci-0.1.4b59/pyproject.toml` & `hatch-ci-0.1.4b67/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-[build-system]
-requires = ["hatchling>=1.1.0", "typing-extensions", "hatch-ci", "jinja2"]
+__version__ = "0.1.4"
+__hash__ = "0.1.4"
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-ci"
-dynamic = ["version"]
+version = "0.1.4b67"
 description = "Hatch plugin for ci system versioning"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
-packages = ["src/hatch_ci"]
 keywords = [
   "git",
   "hatch",
   "plugin",
   "scm",
   "version",
 ]
@@ -40,41 +39,41 @@
 [project.scripts]
 hatch-ci = "hatch_ci:script.main"
 
 [project.urls]
 Issues = "https://github.com/cav71/hatch-ci/issues"
 Source = "https://github.com/cav71/hatch-ci"
 
-[project.entry-points.hatch]
-ci = "hatch_ci.hooks"
-
-[tool.hatch.version]
-source = "ci"
-version-file = "src/hatch_ci/__init__.py"
-
-[tool.hatch.build.hooks.ci]
-version-file = "src/hatch_ci/__init__.py"
-process-replace = [
-    # for the github actions
-    [ 're:(https://github.com/.+/actions/workflows/)(master)(.yml/badge.svg)',
-        '\1{{ ctx.workflow }}\3' ],
-    [ 're:(https://github.com/.+/actions)/(workflows/)(master.yml)(?!/)',
-        '\1/runs/{{ ctx.runid }}' ],
-
-    # for the codecov part
-    [ 're:(https://codecov.io/gh/.+/branch)/master(/graph/badge.svg[?]token=.+)',
-        '\1/{{ ctx.branch|urlquote }}\2' ],
-    [ 're:(https://codecov.io/gh/.+/branch)/master(?!/)',
-        '\1/{{ ctx.branch|urlquote }}' ]
-]
-
-process-paths = [
-  "README.md",
-  "TEMPLATE.md"
-]
+#[project.entry-points.hatch]
+#ci = "hatch_ci.hooks"
+#
+#[tool.hatch.version]
+#source = "ci"
+#version-file = "src/hatch_ci/__init__.py"
+#
+#[tool.hatch.build.hooks.ci]
+#version-file = "src/hatch_ci/__init__.py"
+#process-replace = [
+#    # for the github actions
+#    [ 're:(https://github.com/.+/actions/workflows/)(master)(.yml/badge.svg)',
+#        '\1{{ ctx.workflow }}\3' ],
+#    [ 're:(https://github.com/.+/actions)/(workflows/)(master.yml)(?!/)',
+#        '\1/runs/{{ ctx.runid }}' ],
+#
+#    # for the codecov part
+#    [ 're:(https://codecov.io/gh/.+/branch)/master(/graph/badge.svg[?]token=.+)',
+#        '\1/{{ ctx.branch|urlquote }}\2' ],
+#    [ 're:(https://codecov.io/gh/.+/branch)/master(?!/)',
+#        '\1/{{ ctx.branch|urlquote }}' ]
+#]
+#
+#process-paths = [
+#  "README.md",
+#  "TEMPLATE.md"
+#]
 
 
 [tool.ruff]
 target-version = "py38"
 line-length = 88
 
 [tool.ruff.lint]
```

### Comparing `hatch_ci-0.1.4b59/PKG-INFO` & `hatch-ci-0.1.4b67/src/hatch_ci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b59
+Version: 0.1.4b67
 Summary: Hatch plugin for ci system versioning
-Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
-Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
-License-File: LICENSE.txt
+Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
+Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: hatchling>=1.1.0
-Requires-Dist: jinja2
 Requires-Dist: typing-extensions
-Description-Content-Type: text/markdown
+Requires-Dist: jinja2
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
@@ -167,8 +167,8 @@
 | `version-file` | `str` | None    | A file where to write __version__/__hash__ variables |
 | `paths` | `list[str]|str` | None | A list of paths to process |
 | `fixers` | `list[dict[str,str]]` | None | A list of dict, each key is a string to replace with the value |
 
 
 ## License
 
-`hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`hatch-ci` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

