# Comparing `tmp/gwsumm-2.2.3.tar.gz` & `tmp/gwsumm-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsumm-2.2.3.tar", last modified: Mon Mar  4 17:59:42 2024, max compression
+gzip compressed data, was "gwsumm-2.2.4.tar", last modified: Fri Apr  5 20:17:34 2024, max compression
```

## Comparing `gwsumm-2.2.3.tar` & `gwsumm-2.2.4.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.723610 gwsumm-2.2.3/
--rw-r--r--   0 iaraota    (501) staff       (20)      319 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.codeclimate.yml
--rw-r--r--   0 iaraota    (501) staff       (20)      184 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.codecov.yml
--rw-r--r--   0 iaraota    (501) staff       (20)      126 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.flake8
--rw-r--r--   0 iaraota    (501) staff       (20)       32 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.gitattributes
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.701233 gwsumm-2.2.3/.github/
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.704738 gwsumm-2.2.3/.github/workflows/
--rw-r--r--   0 iaraota    (501) staff       (20)     3669 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.github/workflows/build.yml
--rw-r--r--   0 iaraota    (501) staff       (20)      765 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.github/workflows/lint.yml
--rw-r--r--   0 iaraota    (501) staff       (20)      259 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.gitignore
--rw-r--r--   0 iaraota    (501) staff       (20)      645 2024-03-04 17:53:56.000000 gwsumm-2.2.3/.readthedocs.yaml
--rw-r--r--   0 iaraota    (501) staff       (20)     2667 2024-03-04 17:53:56.000000 gwsumm-2.2.3/CONTRIBUTING.md
--rw-r--r--   0 iaraota    (501) staff       (20)    35147 2024-03-04 17:53:56.000000 gwsumm-2.2.3/LICENSE
--rw-r--r--   0 iaraota    (501) staff       (20)       94 2024-03-04 17:53:56.000000 gwsumm-2.2.3/MANIFEST.in
--rw-r--r--   0 iaraota    (501) staff       (20)     4764 2024-03-04 17:59:42.723395 gwsumm-2.2.3/PKG-INFO
--rw-r--r--   0 iaraota    (501) staff       (20)     2358 2024-03-04 17:53:56.000000 gwsumm-2.2.3/README.rst
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.706585 gwsumm-2.2.3/docs/
--rw-r--r--   0 iaraota    (501) staff       (20)     6810 2024-03-04 17:53:56.000000 gwsumm-2.2.3/docs/Makefile
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.701407 gwsumm-2.2.3/docs/_static/
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.706732 gwsumm-2.2.3/docs/_static/css/
--rw-r--r--   0 iaraota    (501) staff       (20)     4997 2024-03-04 17:53:56.000000 gwsumm-2.2.3/docs/_static/css/custom.css
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.706872 gwsumm-2.2.3/docs/_templates/
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.707023 gwsumm-2.2.3/docs/_templates/autoclass/
--rw-r--r--   0 iaraota    (501) staff       (20)      928 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.707445 gwsumm-2.2.3/docs/_templates/autosummary/
--rw-r--r--   0 iaraota    (501) staff       (20)      170 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     1167 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      703 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      303 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/_templates/layout.html
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.707680 gwsumm-2.2.3/docs/api/
--rw-r--r--   0 iaraota    (501) staff       (20)       64 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/api/index.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      537 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/automation.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     1427 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/cli.rst
--rw-r--r--   0 iaraota    (501) staff       (20)    10467 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/conf.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.708397 gwsumm-2.2.3/docs/configuration/
--rw-r--r--   0 iaraota    (501) staff       (20)    12488 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/configuration/data.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     1887 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/configuration/format.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      908 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/configuration/index.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     3433 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/configuration/tabs.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      545 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/environment.yml
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.708767 gwsumm-2.2.3/docs/examples/
--rw-r--r--   0 iaraota    (501) staff       (20)    22257 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/examples/first.png
--rw-r--r--   0 iaraota    (501) staff       (20)    95352 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/examples/imc.png
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.708958 gwsumm-2.2.3/docs/images/
--rw-r--r--   0 iaraota    (501) staff       (20)   710629 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/images/screenshot.png
--rw-r--r--   0 iaraota    (501) staff       (20)     2948 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/index.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     6701 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/make.bat
--rw-r--r--   0 iaraota    (501) staff       (20)       28 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/modes.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     2864 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/overview.rst
--rw-r--r--   0 iaraota    (501) staff       (20)       79 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/plots.rst
--rw-r--r--   0 iaraota    (501) staff       (20)      100 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/states.rst
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.709863 gwsumm-2.2.3/docs/tabs/
--rw-r--r--   0 iaraota    (501) staff       (20)       53 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/tabs/api.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     1458 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/tabs/index.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     2368 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/tabs/modes.rst
--rw-r--r--   0 iaraota    (501) staff       (20)     2202 2024-03-04 17:53:57.000000 gwsumm-2.2.3/docs/tabs/websites.rst
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.711710 gwsumm-2.2.3/gwsumm/
--rw-r--r--   0 iaraota    (501) staff       (20)     1326 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)    28701 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/__main__.py
--rw-r--r--   0 iaraota    (501) staff       (20)      411 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm/_version.py
--rw-r--r--   0 iaraota    (501) staff       (20)    14914 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/archive.py
--rw-r--r--   0 iaraota    (501) staff       (20)    20413 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/batch.py
--rw-r--r--   0 iaraota    (501) staff       (20)    10806 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/channels.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.712926 gwsumm-2.2.3/gwsumm/config/
--rw-r--r--   0 iaraota    (501) staff       (20)    14290 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/config/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3229 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/config/defaults.ini
--rw-r--r--   0 iaraota    (501) staff       (20)      423 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/config/matplotlib.ini
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.713936 gwsumm-2.2.3/gwsumm/data/
--rw-r--r--   0 iaraota    (501) staff       (20)     2098 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)    18673 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/coherence.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8781 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/mathutils.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6643 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/range.py
--rw-r--r--   0 iaraota    (501) staff       (20)    16817 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/spectral.py
--rw-r--r--   0 iaraota    (501) staff       (20)    32307 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/timeseries.py
--rw-r--r--   0 iaraota    (501) staff       (20)     5424 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/data/utils.py
--rw-r--r--   0 iaraota    (501) staff       (20)     1263 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/globalv.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.714516 gwsumm-2.2.3/gwsumm/html/
--rw-r--r--   0 iaraota    (501) staff       (20)     1268 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6403 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/bootstrap.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8700 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/html5.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2539 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/static.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.715100 gwsumm-2.2.3/gwsumm/html/tests/
--rw-r--r--   0 iaraota    (501) staff       (20)      798 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/tests/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4293 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/tests/test_bootstrap.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6577 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/tests/test_html5.py
--rw-r--r--   0 iaraota    (501) staff       (20)     1947 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/html/tests/test_static.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2116 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/io.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3832 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/mode.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.716477 gwsumm-2.2.3/gwsumm/plot/
--rw-r--r--   0 iaraota    (501) staff       (20)     2834 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)    37186 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/builtin.py
--rw-r--r--   0 iaraota    (501) staff       (20)    27119 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/core.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.716850 gwsumm-2.2.3/gwsumm/plot/guardian/
--rw-r--r--   0 iaraota    (501) staff       (20)      911 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/guardian/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6353 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/guardian/__main__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     7919 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/guardian/core.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.717121 gwsumm-2.2.3/gwsumm/plot/guardian/tests/
--rw-r--r--   0 iaraota    (501) staff       (20)      807 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/guardian/tests/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2903 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/guardian/tests/test_main.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8243 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/mixins.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8000 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/noisebudget.py
--rw-r--r--   0 iaraota    (501) staff       (20)    14079 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/range.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2023 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/registry.py
--rw-r--r--   0 iaraota    (501) staff       (20)    58958 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/segments.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6023 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/sei.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.717554 gwsumm-2.2.3/gwsumm/plot/triggers/
--rw-r--r--   0 iaraota    (501) staff       (20)     1014 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/triggers/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     9012 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/triggers/__main__.py
--rw-r--r--   0 iaraota    (501) staff       (20)    21921 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/triggers/core.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.717842 gwsumm-2.2.3/gwsumm/plot/triggers/tests/
--rw-r--r--   0 iaraota    (501) staff       (20)      807 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/triggers/tests/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3902 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/triggers/tests/test_main.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4987 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/plot/utils.py
--rw-r--r--   0 iaraota    (501) staff       (20)    12722 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/segments.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.718371 gwsumm-2.2.3/gwsumm/state/
--rw-r--r--   0 iaraota    (501) staff       (20)     2023 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/state/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2034 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/state/all.py
--rw-r--r--   0 iaraota    (501) staff       (20)    12603 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/state/core.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3034 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/state/registry.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.720451 gwsumm-2.2.3/gwsumm/tabs/
--rw-r--r--   0 iaraota    (501) staff       (20)     1506 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)    29472 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/builtin.py
--rw-r--r--   0 iaraota    (501) staff       (20)    36826 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/core.py
--rw-r--r--   0 iaraota    (501) staff       (20)    39850 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/data.py
--rw-r--r--   0 iaraota    (501) staff       (20)    15759 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/etg.py
--rw-r--r--   0 iaraota    (501) staff       (20)    10248 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/fscan.py
--rw-r--r--   0 iaraota    (501) staff       (20)    10332 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/gracedb.py
--rw-r--r--   0 iaraota    (501) staff       (20)    14122 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/guardian.py
--rw-r--r--   0 iaraota    (501) staff       (20)     9258 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/management.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3611 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/misc.py
--rw-r--r--   0 iaraota    (501) staff       (20)     2107 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/registry.py
--rw-r--r--   0 iaraota    (501) staff       (20)    16837 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/sei.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4984 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tabs/stamp.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.722350 gwsumm-2.2.3/gwsumm/tests/
--rw-r--r--   0 iaraota    (501) staff       (20)      790 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/__init__.py
--rw-r--r--   0 iaraota    (501) staff       (20)     1170 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/common.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4780 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_archive.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4855 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_batch.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4208 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_channels.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8768 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_config.py
--rw-r--r--   0 iaraota    (501) staff       (20)     8903 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_data.py
--rw-r--r--   0 iaraota    (501) staff       (20)     1803 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_mode.py
--rw-r--r--   0 iaraota    (501) staff       (20)    10913 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_plot.py
--rw-r--r--   0 iaraota    (501) staff       (20)     4393 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_tabs.py
--rw-r--r--   0 iaraota    (501) staff       (20)     3782 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/tests/test_utils.py
--rw-r--r--   0 iaraota    (501) staff       (20)    16412 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/triggers.py
--rw-r--r--   0 iaraota    (501) staff       (20)     1032 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/units.py
--rw-r--r--   0 iaraota    (501) staff       (20)     6446 2024-03-04 17:53:57.000000 gwsumm-2.2.3/gwsumm/utils.py
-drwxr-xr-x   0 iaraota    (501) staff       (20)        0 2024-03-04 17:59:42.722538 gwsumm-2.2.3/gwsumm.egg-info/
--rw-r--r--   0 iaraota    (501) staff       (20)     4764 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/PKG-INFO
--rw-r--r--   0 iaraota    (501) staff       (20)     2986 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/SOURCES.txt
--rw-r--r--   0 iaraota    (501) staff       (20)        1 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/dependency_links.txt
--rw-r--r--   0 iaraota    (501) staff       (20)      204 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/entry_points.txt
--rw-r--r--   0 iaraota    (501) staff       (20)      410 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/requires.txt
--rw-r--r--   0 iaraota    (501) staff       (20)        7 2024-03-04 17:59:42.000000 gwsumm-2.2.3/gwsumm.egg-info/top_level.txt
--rw-r--r--   0 iaraota    (501) staff       (20)     2891 2024-03-04 17:53:57.000000 gwsumm-2.2.3/pyproject.toml
--rw-r--r--   0 iaraota    (501) staff       (20)       38 2024-03-04 17:59:42.723659 gwsumm-2.2.3/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.258291 gwsumm-2.2.4/
+-rw-r--r--   0 egoetz     (501) staff       (20)      319 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.codeclimate.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2020-04-07 19:56:04.000000 gwsumm-2.2.4/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      126 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       32 2020-04-07 19:56:04.000000 gwsumm-2.2.4/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.137534 gwsumm-2.2.4/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.151520 gwsumm-2.2.4/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3579 2024-03-26 21:53:27.000000 gwsumm-2.2.4/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      765 2024-03-26 21:53:27.000000 gwsumm-2.2.4/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      259 2023-11-01 22:18:02.000000 gwsumm-2.2.4/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      645 2024-03-25 16:15:43.000000 gwsumm-2.2.4/.readthedocs.yaml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2667 2021-03-09 19:10:52.000000 gwsumm-2.2.4/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.2.4/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       94 2023-11-01 22:18:02.000000 gwsumm-2.2.4/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-05 20:17:34.257513 gwsumm-2.2.4/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.2.4/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.161056 gwsumm-2.2.4/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6810 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.137925 gwsumm-2.2.4/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.161552 gwsumm-2.2.4/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.162195 gwsumm-2.2.4/docs/_templates/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.162833 gwsumm-2.2.4/docs/_templates/autoclass/
+-rw-r--r--   0 egoetz     (501) staff       (20)      928 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.164817 gwsumm-2.2.4/docs/_templates/autosummary/
+-rw-r--r--   0 egoetz     (501) staff       (20)      170 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1167 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      703 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      303 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/_templates/layout.html
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.165422 gwsumm-2.2.4/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       64 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      537 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/automation.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1427 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/cli.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10467 2023-11-01 22:18:02.000000 gwsumm-2.2.4/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.168513 gwsumm-2.2.4/docs/configuration/
+-rw-r--r--   0 egoetz     (501) staff       (20)    12488 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/data.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1887 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/format.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      908 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     3433 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/configuration/tabs.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      555 2024-03-25 16:02:23.000000 gwsumm-2.2.4/docs/environment.yml
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.170520 gwsumm-2.2.4/docs/examples/
+-rw-r--r--   0 egoetz     (501) staff       (20)    22257 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/examples/first.png
+-rw-r--r--   0 egoetz     (501) staff       (20)    95352 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/examples/imc.png
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.172240 gwsumm-2.2.4/docs/images/
+-rw-r--r--   0 egoetz     (501) staff       (20)   710629 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/images/screenshot.png
+-rw-r--r--   0 egoetz     (501) staff       (20)     2948 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     6701 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/make.bat
+-rw-r--r--   0 egoetz     (501) staff       (20)       28 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2864 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/overview.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)       79 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/plots.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      100 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/states.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.179014 gwsumm-2.2.4/docs/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)       53 2020-04-07 19:56:04.000000 gwsumm-2.2.4/docs/tabs/api.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1458 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2368 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2202 2023-11-01 16:21:08.000000 gwsumm-2.2.4/docs/tabs/websites.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.190977 gwsumm-2.2.4/gwsumm/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1326 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    28701 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-05 20:17:33.000000 gwsumm-2.2.4/gwsumm/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14914 2024-04-04 19:05:23.000000 gwsumm-2.2.4/gwsumm/archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10806 2024-04-05 20:16:21.000000 gwsumm-2.2.4/gwsumm/channels.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.196508 gwsumm-2.2.4/gwsumm/config/
+-rw-r--r--   0 egoetz     (501) staff       (20)    14290 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/defaults.ini
+-rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/config/matplotlib.ini
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.202891 gwsumm-2.2.4/gwsumm/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    18673 2022-09-15 15:47:20.000000 gwsumm-2.2.4/gwsumm/data/coherence.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/mathutils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7193 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/data/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16530 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/data/spectral.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32307 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/data/timeseries.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/data/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/globalv.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.206335 gwsumm-2.2.4/gwsumm/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/html/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6404 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/html/html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2591 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/static.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.209925 gwsumm-2.2.4/gwsumm/html/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/html/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4297 2024-04-04 18:06:28.000000 gwsumm-2.2.4/gwsumm/html/tests/test_bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/html/tests/test_html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1940 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/html/tests/test_static.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/io.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/mode.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.219878 gwsumm-2.2.4/gwsumm/plot/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2834 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    37328 2024-04-05 20:16:32.000000 gwsumm-2.2.4/gwsumm/plot/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    27119 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.222062 gwsumm-2.2.4/gwsumm/plot/guardian/
+-rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.223306 gwsumm-2.2.4/gwsumm/plot/guardian/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/guardian/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/plot/mixins.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8000 2023-11-02 17:15:14.000000 gwsumm-2.2.4/gwsumm/plot/noisebudget.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14079 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/plot/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/plot/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    58958 2024-03-19 23:14:10.000000 gwsumm-2.2.4/gwsumm/plot/segments.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/plot/sei.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.226093 gwsumm-2.2.4/gwsumm/plot/triggers/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.2.4/gwsumm/plot/triggers/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    21921 2023-11-02 17:15:14.000000 gwsumm-2.2.4/gwsumm/plot/triggers/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.227912 gwsumm-2.2.4/gwsumm/plot/triggers/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/plot/triggers/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4987 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/plot/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12722 2024-01-25 21:39:34.000000 gwsumm-2.2.4/gwsumm/segments.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.231658 gwsumm-2.2.4/gwsumm/state/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.2.4/gwsumm/state/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/state/all.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-11-01 16:21:08.000000 gwsumm-2.2.4/gwsumm/state/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/state/registry.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.244791 gwsumm-2.2.4/gwsumm/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    36826 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/tabs/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    39853 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/tabs/data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15759 2024-01-31 17:20:38.000000 gwsumm-2.2.4/gwsumm/tabs/etg.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.2.4/gwsumm/tabs/fscan.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tabs/gracedb.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14124 2024-03-26 21:53:27.000000 gwsumm-2.2.4/gwsumm/tabs/guardian.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/management.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tabs/misc.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tabs/sei.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.2.4/gwsumm/tabs/stamp.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.253845 gwsumm-2.2.4/gwsumm/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/common.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_channels.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-11-01 22:18:02.000000 gwsumm-2.2.4/gwsumm/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_mode.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10913 2024-02-09 21:54:30.000000 gwsumm-2.2.4/gwsumm/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_tabs.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16412 2024-03-19 23:14:10.000000 gwsumm-2.2.4/gwsumm/triggers.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.2.4/gwsumm/units.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.2.4/gwsumm/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-05 20:17:34.254606 gwsumm-2.2.4/gwsumm.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2986 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      204 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      410 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        7 2024-04-05 20:17:34.000000 gwsumm-2.2.4/gwsumm.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     2891 2024-04-04 18:06:28.000000 gwsumm-2.2.4/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-05 20:17:34.258451 gwsumm-2.2.4/setup.cfg
```

### Comparing `gwsumm-2.2.3/.github/workflows/build.yml` & `gwsumm-2.2.4/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -45,37 +45,35 @@
     # this is needed for conda environments to activate automatically
     defaults:
       run:
         shell: bash -el {0}
 
     steps:
     - name: Get source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Cache conda packages
-      uses: actions/cache@v2
+      uses: actions/cache@v4
       env:
         # increment to reset cache
         CACHE_NUMBER: 0
       with:
         path: ~/conda_pkgs_dir
         key: ${{ runner.os }}-conda-${{ matrix.python-version }}-${{ env.CACHE_NUMBER }}
         restore-keys: ${{ runner.os }}-conda-${{ matrix.python-version }}-
 
     - name: Configure conda
-      uses: conda-incubator/setup-miniconda@v2
+      uses: conda-incubator/setup-miniconda@v3
       with:
         activate-environment: test
         miniforge-variant: Mambaforge
         python-version: ${{ matrix.python-version }}
         use-mamba: true
-        # this is needed for caching to work properly:
-        use-only-tar-bz2: true
 
     - name: Conda info
       run: conda info --all
 
     - name: Install dependencies
       run: |
         # parse requirements to install as much as possible with conda
@@ -109,18 +107,18 @@
         python -m coverage run --append --source gwsumm -m gwsumm.plot.triggers --help
         python -m coverage run --append --source gwsumm -m gwsumm.plot.guardian --help
 
     - name: Coverage report
       run: python -m coverage report --show-missing
 
     - name: Publish coverage to Codecov
-      uses: codecov/codecov-action@v1.2.1
+      uses: codecov/codecov-action@v4
       with:
         files: coverage.xml
         flags: ${{ runner.os }},python${{ matrix.python-version }}
 
     - name: Upload test results
       if: always()
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v4
       with:
         name: pytest-conda-${{ matrix.os }}-${{ matrix.python-version }}
         path: pytest.xml
```

### Comparing `gwsumm-2.2.3/.github/workflows/lint.yml` & `gwsumm-2.2.4/.github/workflows/lint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
   cancel-in-progress: true
 
 jobs:
   flake8:
     name: Flake8
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install "flake8>=3.7.0"
     - name: Lint with flake8
```

### Comparing `gwsumm-2.2.3/.readthedocs.yaml` & `gwsumm-2.2.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/CONTRIBUTING.md` & `gwsumm-2.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/LICENSE` & `gwsumm-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/PKG-INFO` & `gwsumm-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.3
+Version: 2.2.4
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.0.0
+Requires-Dist: gwdetchar>=2.2.4
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.3/README.rst` & `gwsumm-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/Makefile` & `gwsumm-2.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/_static/css/custom.css` & `gwsumm-2.2.4/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/_templates/autoclass/class.rst` & `gwsumm-2.2.4/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/_templates/autosummary/class.rst` & `gwsumm-2.2.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/_templates/autosummary/module.rst` & `gwsumm-2.2.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/automation.rst` & `gwsumm-2.2.4/docs/automation.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/cli.rst` & `gwsumm-2.2.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/conf.py` & `gwsumm-2.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/configuration/data.rst` & `gwsumm-2.2.4/docs/configuration/data.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/configuration/format.rst` & `gwsumm-2.2.4/docs/configuration/format.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/configuration/index.rst` & `gwsumm-2.2.4/docs/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/configuration/tabs.rst` & `gwsumm-2.2.4/docs/configuration/tabs.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/environment.yml` & `gwsumm-2.2.4/docs/environment.yml`

 * *Files 23% similar despite different names*

```diff
@@ -24,10 +24,10 @@
   - pygments >=2.7.0
   - python-dateutil
   - python-ligo-lw
   - scipy >=1.2.0
   # docs
   - numpydoc
   - sphinx
-  - sphinx-automodapi
+  - sphinx-automodapi !=0.17.0
   - sphinx_bootstrap_theme
-  - sphinxcontrib-programoutput
+  - sphinxcontrib-programoutput
```

### Comparing `gwsumm-2.2.3/docs/examples/first.png` & `gwsumm-2.2.4/docs/examples/first.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/examples/imc.png` & `gwsumm-2.2.4/docs/examples/imc.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/images/screenshot.png` & `gwsumm-2.2.4/docs/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/index.rst` & `gwsumm-2.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/make.bat` & `gwsumm-2.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/overview.rst` & `gwsumm-2.2.4/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/tabs/index.rst` & `gwsumm-2.2.4/docs/tabs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/tabs/modes.rst` & `gwsumm-2.2.4/docs/tabs/modes.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/docs/tabs/websites.rst` & `gwsumm-2.2.4/docs/tabs/websites.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/__init__.py` & `gwsumm-2.2.4/gwsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/__main__.py` & `gwsumm-2.2.4/gwsumm/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/archive.py` & `gwsumm-2.2.4/gwsumm/archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/batch.py` & `gwsumm-2.2.4/gwsumm/batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/channels.py` & `gwsumm-2.2.4/gwsumm/channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/config/__init__.py` & `gwsumm-2.2.4/gwsumm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/config/defaults.ini` & `gwsumm-2.2.4/gwsumm/config/defaults.ini`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/data/__init__.py` & `gwsumm-2.2.4/gwsumm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/data/coherence.py` & `gwsumm-2.2.4/gwsumm/data/coherence.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/data/mathutils.py` & `gwsumm-2.2.4/gwsumm/data/mathutils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/data/range.py` & `gwsumm-2.2.4/gwsumm/data/range.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,29 +113,45 @@
             stride=stride, fftlength=fftlength, overlap=overlap, method=method)
         for sg in spectrograms:  # get contribution from each spectrogram
             outspec = astro.range_spectrogram(sg, **rangekwargs)
             outspec.channel = key
             add_spectrogram(outspec if 'energy' in rangekwargs else
                             outspec**(1/2.), key=key)
 
-    if return_:
-        return globalv.SPECTROGRAMS.get(key, SpectrogramList())
+    if not return_:
+        return
+
+    # return correct data, according to state segment
+    out = SpectrogramList()
+    for specgram in globalv.SPECTROGRAMS[key]:
+        for seg in segments:
+            if abs(seg) < specgram.dt.value:
+                continue
+            if specgram.span.intersects(seg):
+                common = specgram.span & type(seg)(seg[0],
+                                                   seg[1] + specgram.dt.value)
+                s = specgram.crop(*common)
+                if s.shape[0]:
+                    out.append(s)
+    return out.coalesce()
 
 
 @use_segmentlist
 def get_range_spectrum(channel, segments, config=None, cache=None, query=True,
                        nds=None, return_=True, nproc=1, datafind_error='raise',
                        frametype=None, stride=60, fftlength=None, overlap=None,
-                       method=None, which='all', **rangekwargs):
+                       method=None, which='all', state=None, **rangekwargs):
     """Compute percentile spectra of the range integrand from a set of
     spectrograms
     """
     name = str(channel)
-    cmin = '%s.min' % name
-    cmax = '%s.max' % name
+    if state:
+        name += f',{state}'
+    cmin = f'{name}.min'
+    cmax = f'{name}.max'
 
     if name not in globalv.SPECTRUM:
         speclist = get_range_spectrogram(
             channel, segments, config=config, cache=cache, query=query,
             nds=nds, return_=return_, nproc=nproc, frametype=frametype,
             datafind_error=datafind_error, method=method, stride=stride,
             fftlength=fftlength, overlap=overlap, **rangekwargs)
@@ -160,8 +176,8 @@
                 globalv.SPECTRUM[cmax])
     if which == 'mean':
         return globalv.SPECTRUM[name]
     if which == 'min':
         return globalv.SPECTRUM[cmin]
     if which == 'max':
         return globalv.SPECTRUM[cmax]
-    raise ValueError("Unrecognised value for `which`: %r" % which)
+    raise ValueError(f"Unrecognised value for `which`: {which}")
```

### Comparing `gwsumm-2.2.3/gwsumm/data/spectral.py` & `gwsumm-2.2.4/gwsumm/data/spectral.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 import numpy
 
 from scipy import interpolate
 
 from astropy import units
 
-from gwpy.segments import DataQualityFlag
 from gwpy.frequencyseries import FrequencySeries
 from gwpy.spectrogram import SpectrogramList
 
 from .. import (globalv, io)
 from ..utils import (vprint, safe_eval)
 from ..channels import (
     get_channel,
@@ -324,62 +323,55 @@
 
 # -- spectrum -----------------------------------------------------------------
 
 @use_segmentlist
 def get_spectrum(channel, segments, config=None, cache=None,
                  query=True, nds=None, format='power', return_=True,
                  frametype=None, nproc=1, datafind_error='raise',
-                 **fftparams):
-    """Retrieve the time-series and generate a spectrogram of the given
+                 state=None, **fftparams):
+    """Retrieve the time-series and generate a spectrum of the given
     channel
     """
     channel = get_channel(channel)
-    if isinstance(segments, DataQualityFlag):
-        name = ','.join([channel.ndsname, segments.name])
-        segments = segments.active
-    else:
-        name = channel.ndsname
-    name += ',%s' % format
 
     # read data for all sub-channels
     specs = []
     channels = list(parse_math_definition(str(channel))[0])
     if len(channels) == 0:
         channels = [channel]
     for c in channels:
         specs.append(_get_spectrum(c, segments, config=config, cache=cache,
                                    query=query, nds=nds, format=format,
                                    return_=return_, frametype=frametype,
                                    nproc=nproc,
                                    datafind_error=datafind_error,
+                                   state=state,
                                    **fftparams))
     if return_ and len(channels) == 1:
         return specs[0]
     elif return_:
         return [get_with_math(
                     channel, segments, _get_spectrum, _get_spectrum,
                     config=config, format=format, return_=True,
                     which=which)[0] for which in ['mean', 'min', 'max']]
 
 
 def _get_spectrum(channel, segments, config=None, cache=None, query=True,
                   nds=None, format='power', return_=True, which='all',
-                  **fftparams):
-    """Retrieve the time-series and generate a spectrogram of the given
+                  state=None, **fftparams):
+    """Retrieve the time-series and generate a spectrum of the given
     channel
     """
     channel = get_channel(channel)
-    if isinstance(segments, DataQualityFlag):
-        name = ','.join([channel.ndsname, segments.name])
-        segments = segments.active
-    else:
-        name = channel.ndsname
-    name += ',%s' % format
-    cmin = '%s.min' % name
-    cmax = '%s.max' % name
+
+    name = f'{channel.ndsname},{format}'
+    if state:
+        name = f'{channel.ndsname},{state},{format}'
+    cmin = f'{name}.min'
+    cmax = f'{name}.max'
 
     if name not in globalv.SPECTRUM:
         if os.path.isfile(channel.ndsname):
             globalv.SPECTRUM[name] = io.read_frequencyseries(channel.ndsname)
             globalv.SPECTRUM[cmin] = globalv.SPECTRUM[name]
             globalv.SPECTRUM[cmax] = globalv.SPECTRUM[name]
         else:
@@ -420,8 +412,8 @@
                 globalv.SPECTRUM[cmax])
     if which == 'mean':
         return globalv.SPECTRUM[name]
     if which == 'min':
         return globalv.SPECTRUM[cmin]
     if which == 'max':
         return globalv.SPECTRUM[cmax]
-    raise ValueError("Unrecognised value for `which`: %r" % which)
+    raise ValueError(f"Unrecognised value for `which`: {which}")
```

### Comparing `gwsumm-2.2.3/gwsumm/data/timeseries.py` & `gwsumm-2.2.4/gwsumm/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/data/utils.py` & `gwsumm-2.2.4/gwsumm/data/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/globalv.py` & `gwsumm-2.2.4/gwsumm/globalv.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/html/__init__.py` & `gwsumm-2.2.4/gwsumm/html/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/html/bootstrap.py` & `gwsumm-2.2.4/gwsumm/html/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,17 +146,17 @@
     """
     current, chref = states[default]
     page = markup.page()
     page.ul(class_='nav navbar-nav')
     page.li(class_='nav-item dropdown')
     page.a(str(current), class_='nav-link dropdown-toggle', href='#',
            id_='states', role='button', title='Show/hide state menu',
-           **{'data-toggle': 'dropdown'})
+           **{'data-bs-toggle': 'dropdown'})
     page.div(
-        class_='dropdown-menu dropdown-menu-right state-switch shadow',
+        class_='dropdown-menu dropdown-menu-end state-switch shadow',
         id_='statemenu',
     )
     page.h6('Select below to view this page in another state (different '
             'time segments).', class_='dropdown-header')
     page.div('', class_='dropdown-divider')
     for i, (state, href) in enumerate(states):
         page.a(str(state), class_='dropdown-item state', title=str(state),
```

### Comparing `gwsumm-2.2.3/gwsumm/html/html5.py` & `gwsumm-2.2.4/gwsumm/html/html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/html/static.py` & `gwsumm-2.2.4/gwsumm/html/static.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,41 +20,42 @@
 
 This module mainly declares the resources used by standard on HTML pages
 """
 
 from collections import OrderedDict
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
-__credits__ = 'Alex Urban <alexander.urban@ligo.org>'
+__credits__ = ('Alex Urban <alexander.urban@ligo.org>,'
+               ' Evan Goetz <evan.goetz@ligo.org>')
 
 
 # build collection of CSS resources
 CSS = OrderedDict((
     ('font-awesome', 'https://cdnjs.cloudflare.com/ajax/libs/'
-                     'font-awesome/5.15.1/css/fontawesome.min.css'),
+                     'font-awesome/6.5.1/css/fontawesome.min.css'),
     ('font-awesome-solid', 'https://cdnjs.cloudflare.com/ajax/libs/'
-                           'font-awesome/5.15.1/css/solid.min.css'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.2/'
+                           'font-awesome/6.5.1/css/solid.min.css'),
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.4/'
                     'lib/gwbootstrap.min.css'),
 ))
 
 # build collection of javascript resources
 JS = OrderedDict((
-    ('jquery', 'https://code.jquery.com/jquery-3.5.1.min.js'),
-    ('jquery-ui', 'https://code.jquery.com/ui/1.12.1/jquery-ui.min.js'),
+    ('jquery', 'https://code.jquery.com/jquery-3.7.1.min.js'),
+    ('jquery-ui', 'https://code.jquery.com/ui/1.13.2/jquery-ui.min.js'),
     ('moment', 'https://cdnjs.cloudflare.com/ajax/libs/'
-               'moment.js/2.29.1/moment.min.js'),
-    ('bootstrap', 'https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/'
+               'moment.js/2.30.1/moment.min.js'),
+    ('bootstrap', 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/'
                   'dist/js/bootstrap.bundle.min.js'),
-    ('fancybox', 'https://cdnjs.cloudflare.com/ajax/libs/'
-                 'fancybox/3.5.7/jquery.fancybox.min.js'),
+    ('fancybox', 'https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/'
+                 'dist/fancybox/fancybox.umd.js'),
     ('datepicker', 'https://cdnjs.cloudflare.com/ajax/libs/'
                    'bootstrap-datepicker/1.9.0/js/'
                    'bootstrap-datepicker.min.js'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.2/'
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.4/'
                     'lib/gwbootstrap-extra.min.js'),
 ))
 
 
 # -- utilities ----------------------------------------------------------------
 
 def get_css():
```

### Comparing `gwsumm-2.2.3/gwsumm/html/tests/__init__.py` & `gwsumm-2.2.4/gwsumm/html/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/html/tests/test_bootstrap.py` & `gwsumm-2.2.4/gwsumm/html/tests/test_bootstrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,29 +79,29 @@
 
 
 def test_state_switcher():
     switcher = bootstrap.state_switcher([('Test', '#test')])
     assert parse_html(str(switcher)) == parse_html(
         '<ul class="nav navbar-nav">\n<li class="nav-item dropdown">\n'
         '<a class="nav-link dropdown-toggle" href="#" id="states" role='
-        '"button" title="Show/hide state menu" data-toggle="dropdown">Test</a>'
-        '\n<div class="dropdown-menu dropdown-menu-right state-switch shadow" '
-        'id="statemenu">\n<h6 class="dropdown-header">Select below to view '
-        'this page in another state (different time segments).</h6>\n<div '
-        'class="dropdown-divider"></div>\n<a class="dropdown-item state" '
+        '"button" title="Show/hide state menu" data-bs-toggle="dropdown">Test'
+        '</a>\n<div class="dropdown-menu dropdown-menu-end state-switch '
+        'shadow" id="statemenu">\n<h6 class="dropdown-header">Select below to '
+        'view this page in another state (different time segments).</h6>\n'
+        '<div class="dropdown-divider"></div>\n<a class="dropdown-item state" '
         'title="Test" id="state_test" onclick="jQuery(this).load_state'
         '(&quot;#test&quot;);">Test</a>\n</div>\n</li>\n</ul>')
 
 
 def test_base_map_dropdown():
     menu = bootstrap.base_map_dropdown('test', id_='id')
     assert parse_html(str(menu)) == parse_html(
         '<div class="navbar-brand border border-white '
         'rounded" id="id">test</div>')
     # test with bases
     menu_wbases = bootstrap.base_map_dropdown('test', bases={'key': 'value'})
     assert parse_html(str(menu_wbases)) == parse_html(
         '<div class="dropdown base-map">\n<a href="#" class="navbar-brand '
         'nav-link border border-white rounded dropdown-toggle" role="button" '
-        'data-toggle="dropdown">test</a>\n<div class="dropdown-menu '
+        'data-bs-toggle="dropdown">test</a>\n<div class="dropdown-menu '
         'dropdown-1-col shadow">\n<a title="key" class="dropdown-item" '
         'data-new-base="value">key</a>\n</div>\n</div>')
```

### Comparing `gwsumm-2.2.3/gwsumm/html/tests/test_html5.py` & `gwsumm-2.2.4/gwsumm/html/tests/test_html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/html/tests/test_static.py` & `gwsumm-2.2.4/gwsumm/html/tests/test_static.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'fancybox',
         'datepicker',
         'gwbootstrap',
     ]
     # test list of files
     js_files = list(x.split('/')[-1] for x in js.values())
     assert js_files == [
-        'jquery-3.5.1.min.js',
+        'jquery-3.7.1.min.js',
         'jquery-ui.min.js',
         'moment.min.js',
         'bootstrap.bundle.min.js',
-        'jquery.fancybox.min.js',
+        'fancybox.umd.js',
         'bootstrap-datepicker.min.js',
         'gwbootstrap-extra.min.js',
     ]
```

### Comparing `gwsumm-2.2.3/gwsumm/io.py` & `gwsumm-2.2.4/gwsumm/io.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/mode.py` & `gwsumm-2.2.4/gwsumm/mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/__init__.py` & `gwsumm-2.2.4/gwsumm/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/builtin.py` & `gwsumm-2.2.4/gwsumm/plot/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,30 +508,32 @@
             else:
                 valid = SegmentList([self.span])
 
             if self.type == 'coherence-spectrum':
                 data = get_coherence_spectrum(
                     [str(channel), str(channel2)], valid, query=False)
             elif self.type == 'range-spectrum':
-                data = get_range_spectrum(str(channel), valid, query=False)
+                data = get_range_spectrum(str(channel), valid, query=False,
+                                          state=valid)
             elif self.type == 'cumulative-range-spectrum':
-                data = get_range_spectrum(
-                    str(channel), valid, query=False, which='mean')
+                data = get_range_spectrum(str(channel), valid, query=False,
+                                          which='mean', state=valid)
                 if str(data.unit) == 'Mpc':
                     data = (data**3).cumsum() ** (1/3.)
                 else:
                     data = (data**2).cumsum() ** (1/2.)
                 try:
                     data = (100 * data / data[-1],)
                 except IndexError:
                     data = tuple()
             else:
                 try:
                     data = get_spectrum(str(channel), valid, query=False,
-                                        format=sdform, method=method)
+                                        format=sdform, method=method,
+                                        state=valid)
                 except ValueError as exc:
                     # math op failed beacuse one of the datasets is empty
                     if (
                             'could not be broadcast' in str(exc) and
                             '(0,)' in str(exc)
                     ):
                         data = []
```

### Comparing `gwsumm-2.2.3/gwsumm/plot/core.py` & `gwsumm-2.2.4/gwsumm/plot/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/guardian/__init__.py` & `gwsumm-2.2.4/gwsumm/plot/guardian/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/guardian/__main__.py` & `gwsumm-2.2.4/gwsumm/plot/guardian/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/guardian/core.py` & `gwsumm-2.2.4/gwsumm/plot/guardian/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/guardian/tests/__init__.py` & `gwsumm-2.2.4/gwsumm/plot/guardian/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/guardian/tests/test_main.py` & `gwsumm-2.2.4/gwsumm/plot/guardian/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/mixins.py` & `gwsumm-2.2.4/gwsumm/plot/mixins.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/noisebudget.py` & `gwsumm-2.2.4/gwsumm/plot/noisebudget.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/range.py` & `gwsumm-2.2.4/gwsumm/plot/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/registry.py` & `gwsumm-2.2.4/gwsumm/plot/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/segments.py` & `gwsumm-2.2.4/gwsumm/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/sei.py` & `gwsumm-2.2.4/gwsumm/plot/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/triggers/__init__.py` & `gwsumm-2.2.4/gwsumm/plot/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/triggers/__main__.py` & `gwsumm-2.2.4/gwsumm/plot/triggers/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/triggers/core.py` & `gwsumm-2.2.4/gwsumm/plot/triggers/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/triggers/tests/__init__.py` & `gwsumm-2.2.4/gwsumm/plot/triggers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/triggers/tests/test_main.py` & `gwsumm-2.2.4/gwsumm/plot/triggers/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/plot/utils.py` & `gwsumm-2.2.4/gwsumm/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/segments.py` & `gwsumm-2.2.4/gwsumm/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/state/__init__.py` & `gwsumm-2.2.4/gwsumm/state/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/state/all.py` & `gwsumm-2.2.4/gwsumm/state/all.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/state/core.py` & `gwsumm-2.2.4/gwsumm/state/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/state/registry.py` & `gwsumm-2.2.4/gwsumm/state/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/__init__.py` & `gwsumm-2.2.4/gwsumm/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/builtin.py` & `gwsumm-2.2.4/gwsumm/tabs/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/core.py` & `gwsumm-2.2.4/gwsumm/tabs/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/data.py` & `gwsumm-2.2.4/gwsumm/tabs/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
             page.div(class_='mt-2', id='accordion')
             for i, (flag, padding) in enumerate(allflags):
                 flag = get_segments(flag, [self.span], query=False,
                                     padding={flag: padding})
                 page.div(class_='card border-info mb-1 shadow-sm')
                 page.div(class_='card-header text-white bg-info')
                 page.a(flag.name, class_='card-link cis-link collapsed',
-                       href='#flag%d' % i, **{'data-toggle': 'collapse',
+                       href='#flag%d' % i, **{'data-bs-toggle': 'collapse',
                                               'aria-expanded': 'false'})
                 page.div.close()  # card-header
                 page.div(id_='flag%d' % i, class_='collapse',
                          **{'data-parent': '#accordion'})
                 page.div(class_='card-body')
                 # write segment summary
                 page.p('This flag was defined and had a known state during '
```

### Comparing `gwsumm-2.2.3/gwsumm/tabs/etg.py` & `gwsumm-2.2.4/gwsumm/tabs/etg.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/fscan.py` & `gwsumm-2.2.4/gwsumm/tabs/fscan.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/gracedb.py` & `gwsumm-2.2.4/gwsumm/tabs/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/guardian.py` & `gwsumm-2.2.4/gwsumm/tabs/guardian.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         for i, bit in enumerate(self.grdstates):
             name = self.grdstates[bit].strip('*')
             page.div(class_='card border-info mb-1 shadow-sm', id=str(bit))
             # heading
             page.div(class_='card-header text-white bg-info')
             page.a('%s [%d]' % (name, bit), href='#collapse-%d' % bit,
                    class_='card-link cis-link collapsed',
-                   **{'data-toggle': 'collapse', 'aria-expandedt': 'false'})
+                   **{'data-bs-toggle': 'collapse', 'aria-expanded': 'false'})
             page.div.close()  # card-header
 
             # body
             page.div(id='collapse-%d' % bit, class_='collapse',
                      **{'data-parent': '#accordion'})
             page.div(class_='card-body')
```

### Comparing `gwsumm-2.2.3/gwsumm/tabs/management.py` & `gwsumm-2.2.4/gwsumm/tabs/management.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/misc.py` & `gwsumm-2.2.4/gwsumm/tabs/misc.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/registry.py` & `gwsumm-2.2.4/gwsumm/tabs/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/sei.py` & `gwsumm-2.2.4/gwsumm/tabs/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tabs/stamp.py` & `gwsumm-2.2.4/gwsumm/tabs/stamp.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/__init__.py` & `gwsumm-2.2.4/gwsumm/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/common.py` & `gwsumm-2.2.4/gwsumm/tests/common.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_archive.py` & `gwsumm-2.2.4/gwsumm/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_batch.py` & `gwsumm-2.2.4/gwsumm/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_channels.py` & `gwsumm-2.2.4/gwsumm/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_config.py` & `gwsumm-2.2.4/gwsumm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_data.py` & `gwsumm-2.2.4/gwsumm/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_mode.py` & `gwsumm-2.2.4/gwsumm/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_plot.py` & `gwsumm-2.2.4/gwsumm/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_tabs.py` & `gwsumm-2.2.4/gwsumm/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/tests/test_utils.py` & `gwsumm-2.2.4/gwsumm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/triggers.py` & `gwsumm-2.2.4/gwsumm/triggers.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/units.py` & `gwsumm-2.2.4/gwsumm/units.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm/utils.py` & `gwsumm-2.2.4/gwsumm/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/gwsumm.egg-info/PKG-INFO` & `gwsumm-2.2.4/gwsumm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.3
+Version: 2.2.4
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.0.0
+Requires-Dist: gwdetchar>=2.2.4
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.3/gwsumm.egg-info/SOURCES.txt` & `gwsumm-2.2.4/gwsumm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.3/pyproject.toml` & `gwsumm-2.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   "Topic :: Scientific/Engineering :: Astronomy",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 dependencies = [
   "astropy >=3.0.0",
   "gwdatafind >=1.1.1",
-  "gwdetchar >=2.0.0",
+  "gwdetchar >=2.2.4",
   "gwpy >=2.0.0",
   "gwtrigfind",
   "lalsuite",
   "ligo-segments",
   "lscsoft-glue >=1.60.0",
   "lxml",
   "markdown",
```

