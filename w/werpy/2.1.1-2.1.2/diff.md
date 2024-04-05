# Comparing `tmp/werpy-2.1.1.tar.gz` & `tmp/werpy-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "werpy-2.1.1.tar", last modified: Mon Nov 27 10:41:20 2023, max compression
+gzip compressed data, was "werpy-2.1.2.tar", last modified: Fri Apr  5 04:01:35 2024, max compression
```

## Comparing `werpy-2.1.1.tar` & `werpy-2.1.2.tar`

### file list

```diff
@@ -1,48 +1,65 @@
--rw-rw-rw-   0        0        0     1827 2023-11-27 10:32:40.000000 werpy-2.1.1/.circleci/config.yml
--rw-rw-rw-   0        0        0    27165 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
--rw-rw-rw-   0        0        0    20097 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/assets/images/werpy-example-summaryp-results-word-error-rate-breakdown.png
--rw-rw-rw-   0        0        0    93938 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/assets/images/werpy-logo-word-error-rate.png
--rw-rw-rw-   0        0        0     2629 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/workflows/bandit.yml
--rw-rw-rw-   0        0        0     2521 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/workflows/codacy.yml
--rw-rw-rw-   0        0        0     3090 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0      724 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/workflows/pylint.yml
--rw-rw-rw-   0        0        0     1817 2023-11-27 10:32:40.000000 werpy-2.1.1/.github/workflows/wheels.yml
--rw-rw-rw-   0        0        0     3286 2023-11-27 10:32:40.000000 werpy-2.1.1/.gitignore
--rw-rw-rw-   0        0        0       76 2023-11-27 10:32:40.000000 werpy-2.1.1/.pylintrc
--rw-rw-rw-   0        0        0     9246 2023-11-27 10:32:40.000000 werpy-2.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0      739 2023-11-27 10:32:40.000000 werpy-2.1.1/CITATION.cff
--rw-rw-rw-   0        0        0     5559 2023-11-27 10:32:40.000000 werpy-2.1.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     4222 2023-11-27 10:32:40.000000 werpy-2.1.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1534 2023-11-27 10:32:40.000000 werpy-2.1.1/LICENSE
--rw-rw-rw-   0        0        0    10174 2023-11-27 10:32:40.000000 werpy-2.1.1/LICENSES/CYTHON_LICENSE
--rw-rw-rw-   0        0        0     1573 2023-11-27 10:32:40.000000 werpy-2.1.1/LICENSES/NUMPY_LICENSE
--rw-rw-rw-   0        0        0     1665 2023-11-27 10:32:40.000000 werpy-2.1.1/LICENSES/PANDAS_LICENSE
--rw-rw-rw-   0        0        0    10913 2023-11-27 10:32:40.000000 werpy-2.1.1/README.md
--rw-rw-rw-   0        0        0     2221 2023-11-27 10:32:40.000000 werpy-2.1.1/SECURITY.md
--rw-rw-rw-   0        0        0     1071 2023-11-27 10:32:40.000000 werpy-2.1.1/meson.build
--rw-rw-rw-   0        0        0     2417 2023-11-27 10:32:40.000000 werpy-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     7221 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_normalize.py
--rw-rw-rw-   0        0        0     4020 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_summary.py
--rw-rw-rw-   0        0        0     3858 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_summaryp.py
--rw-rw-rw-   0        0        0     5065 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_wer.py
--rw-rw-rw-   0        0        0     6519 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_werp.py
--rw-rw-rw-   0        0        0     7581 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_werps.py
--rw-rw-rw-   0        0        0     5664 2023-11-27 10:32:40.000000 werpy-2.1.1/tests/test_wers.py
--rw-rw-rw-   0        0        0      383 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__init__.py
--rw-rw-rw-   0        0        0     5935 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/metrics.cpython-311.pyc
--rw-rw-rw-   0        0        0     7449 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/normalize.cpython-311.pyc
--rw-rw-rw-   0        0        0     2885 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/summary.cpython-311.pyc
--rw-rw-rw-   0        0        0     2764 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/wer.cpython-311.pyc
--rw-rw-rw-   0        0        0     3744 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/werp.cpython-311.pyc
--rw-rw-rw-   0        0        0     3897 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/werps.cpython-311.pyc
--rw-rw-rw-   0        0        0     2615 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/__pycache__/wers.cpython-311.pyc
--rw-rw-rw-   0        0        0     1648 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/errorhandler.py
--rw-rw-rw-   0        0        0     3654 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/metrics.pyx
--rw-rw-rw-   0        0        0     3218 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/normalize.py
--rw-rw-rw-   0        0        0     2682 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/summary.py
--rw-rw-rw-   0        0        0     4423 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/summaryp.py
--rw-rw-rw-   0        0        0     2547 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/wer.py
--rw-rw-rw-   0        0        0     3473 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/werp.py
--rw-rw-rw-   0        0        0     3698 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/werps.py
--rw-rw-rw-   0        0        0     2068 2023-11-27 10:32:40.000000 werpy-2.1.1/werpy/wers.py
--rw-r--r--   0        0        0    14237 2023-11-27 10:41:21.153779 werpy-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3607 2024-04-05 03:50:45.000000 werpy-2.1.2/.circleci/config.yml
+-rw-rw-rw-   0        0        0    27165 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
+-rw-rw-rw-   0        0        0    20097 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/assets/images/werpy-example-summaryp-results-word-error-rate-breakdown.png
+-rw-rw-rw-   0        0        0    93938 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/assets/images/werpy-logo-word-error-rate.png
+-rw-rw-rw-   0        0        0      506 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/dependabot.yml
+-rw-rw-rw-   0        0        0     2629 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/workflows/bandit.yml
+-rw-rw-rw-   0        0        0     2521 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/workflows/codacy.yml
+-rw-rw-rw-   0        0        0     3090 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0      740 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/workflows/pylint.yml
+-rw-rw-rw-   0        0        0     1817 2024-04-05 03:50:45.000000 werpy-2.1.2/.github/workflows/wheels.yml
+-rw-rw-rw-   0        0        0     3286 2024-04-05 03:50:45.000000 werpy-2.1.2/.gitignore
+-rw-rw-rw-   0        0        0      121 2024-04-05 03:50:45.000000 werpy-2.1.2/.pylintrc
+-rw-rw-rw-   0        0        0     1103 2024-04-05 03:50:45.000000 werpy-2.1.2/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    10710 2024-04-05 03:50:45.000000 werpy-2.1.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0      739 2024-04-05 03:50:45.000000 werpy-2.1.2/CITATION.cff
+-rw-rw-rw-   0        0        0     5559 2024-04-05 03:50:45.000000 werpy-2.1.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     4222 2024-04-05 03:50:45.000000 werpy-2.1.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1539 2024-04-05 03:50:45.000000 werpy-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0    10174 2024-04-05 03:50:45.000000 werpy-2.1.2/LICENSES/CYTHON_LICENSE
+-rw-rw-rw-   0        0        0     1573 2024-04-05 03:50:45.000000 werpy-2.1.2/LICENSES/NUMPY_LICENSE
+-rw-rw-rw-   0        0        0     1665 2024-04-05 03:50:45.000000 werpy-2.1.2/LICENSES/PANDAS_LICENSE
+-rw-rw-rw-   0        0        0    11522 2024-04-05 03:50:45.000000 werpy-2.1.2/README.md
+-rw-rw-rw-   0        0        0     2221 2024-04-05 03:50:45.000000 werpy-2.1.2/SECURITY.md
+-rw-rw-rw-   0        0        0      638 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       38 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/requirements.in
+-rw-rw-rw-   0        0        0     1247 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1540 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0     2775 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/index.rst
+-rw-rw-rw-   0        0        0      687 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/installation.rst
+-rw-rw-rw-   0        0        0     1502 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/modules.rst
+-rw-rw-rw-   0        0        0    23606 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/images/werpy-example-summary-results-word-error-rate-breakdown.png
+-rw-rw-rw-   0        0        0    17660 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/images/werpy-example-summaryp-results-word-error-rate-breakdown.png
+-rw-rw-rw-   0        0        0     1682 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/index.rst
+-rw-rw-rw-   0        0        0     3293 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/normalization.rst
+-rw-rw-rw-   0        0        0     3595 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/summarization.rst
+-rw-rw-rw-   0        0        0     4274 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/weighted-word-error-rate.rst
+-rw-rw-rw-   0        0        0     4061 2024-04-05 03:50:45.000000 werpy-2.1.2/docs/source/usage/word-error-rate.rst
+-rw-rw-rw-   0        0        0     1071 2024-04-05 03:50:45.000000 werpy-2.1.2/meson.build
+-rw-rw-rw-   0        0        0     2514 2024-04-05 03:50:45.000000 werpy-2.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     7182 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_normalize.py
+-rw-rw-rw-   0        0        0     4560 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_summary.py
+-rw-rw-rw-   0        0        0     6034 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_summaryp.py
+-rw-rw-rw-   0        0        0     5109 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_wer.py
+-rw-rw-rw-   0        0        0     6424 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_werp.py
+-rw-rw-rw-   0        0        0     7543 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_werps.py
+-rw-rw-rw-   0        0        0     5696 2024-04-05 03:50:45.000000 werpy-2.1.2/tests/test_wers.py
+-rw-rw-rw-   0        0        0      383 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__init__.py
+-rw-rw-rw-   0        0        0     5935 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/metrics.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7449 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/normalize.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2885 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/summary.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2764 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/wer.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3744 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/werp.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3897 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/werps.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2615 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/__pycache__/wers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1665 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/errorhandler.py
+-rw-rw-rw-   0        0        0     3654 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/metrics.pyx
+-rw-rw-rw-   0        0        0     3200 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/normalize.py
+-rw-rw-rw-   0        0        0     2746 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/summary.py
+-rw-rw-rw-   0        0        0     4734 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/summaryp.py
+-rw-rw-rw-   0        0        0     2508 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/wer.py
+-rw-rw-rw-   0        0        0     3568 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/werp.py
+-rw-rw-rw-   0        0        0     3793 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/werps.py
+-rw-rw-rw-   0        0        0     2092 2024-04-05 03:50:45.000000 werpy-2.1.2/werpy/wers.py
+-rw-r--r--   0        0        0    14967 2024-04-05 04:01:36.500789 werpy-2.1.2/PKG-INFO
```

### Comparing `werpy-2.1.1/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png` & `werpy-2.1.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/assets/images/werpy-example-summaryp-results-word-error-rate-breakdown.png` & `werpy-2.1.2/.github/assets/images/werpy-example-summaryp-results-word-error-rate-breakdown.png`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/assets/images/werpy-logo-word-error-rate.png` & `werpy-2.1.2/.github/assets/images/werpy-logo-word-error-rate.png`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/workflows/bandit.yml` & `werpy-2.1.2/.github/workflows/bandit.yml`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/workflows/codacy.yml` & `werpy-2.1.2/.github/workflows/codacy.yml`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/workflows/codeql.yml` & `werpy-2.1.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.github/workflows/pylint.yml` & `werpy-2.1.2/.github/workflows/pylint.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `werpy-2.1.1/.github/workflows/wheels.yml` & `werpy-2.1.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/.gitignore` & `werpy-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/CHANGELOG.md` & `werpy-2.1.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,46 @@
 # CHANGELOG
 This changelog file outlines a chronologically ordered list of the changes made on this project. 
 It is organized by version and release date followed by a list of Enhancements, New Features, Bug Fixes, and/or Breaking Changes.
 <br /><br />
 
-## Version 2.1.1 (Latest)
+## Version 2.1.2 (Latest)
+**Released:** April 5, 2024<br />
+**Tag:** v2.1.2
+
+### Enhancements
+
+- Full compatibility with Python v3.12:
+  - The package has been thoroughly tested and verified to work seamlessly with Python v3.12.
+  - All dependencies have been updated and are also compliant with Python v3.12.
+
+- Added comprehensive package documentation using Sphinx and hosted on Read the Docs. The documentation covers installation instructions, usage guides, and worked examples of all feature functionality. Access the documentation at [https://werpy.readthedocs.io/](https://werpy.readthedocs.io/).
+
+- Updated the circleci config.yml file to support the compilation of Cython .pyx files.
+
+- Integrated codecov into the circleci config.yml file to generate comprehensive coverage reports.
+
+- Enhanced testing procedures to increase code coverage percentage.
+
+- Ensured compliance with the Black code formatting by modifying relevant files.
+
+
+### Changed
+
+- Bump jinja2 from 3.1.2 to 3.1.3 in /docs. ([#1](https://github.com/analyticsinmotion/werpy/pull/1))
+  - For more information please see the Jinja release documentation [https://github.com/pallets/jinja/releases](https://github.com/pallets/jinja/releases).
+
+- Bump sphinx-nefertiti from 0.2.1 to 0.2.3 ([#2](https://github.com/analyticsinmotion/werpy/pull/2))
+
+- Bump sphinx-nefertiti from 0.2.3 to 0.3.1 ([#3](https://github.com/analyticsinmotion/werpy/pull/3))
+
+
+<br /><br />
+
+## Version 2.1.1
 **Released:** November 27, 2023<br />
 **Tag:** v2.1.1
 
 ### Enhancements
 
 - Updated the meson.build file to align with the recommended approach for integrating Cython into the build process:
   - Added Cython to the list of languages utilized by the project.
```

### Comparing `werpy-2.1.1/CITATION.cff` & `werpy-2.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/CODE_OF_CONDUCT.md` & `werpy-2.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/CONTRIBUTING.md` & `werpy-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/LICENSE` & `werpy-2.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Analytics in Motion
+Copyright (c) 2023-2024, Analytics in Motion
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `werpy-2.1.1/LICENSES/CYTHON_LICENSE` & `werpy-2.1.2/LICENSES/CYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/LICENSES/NUMPY_LICENSE` & `werpy-2.1.2/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/LICENSES/PANDAS_LICENSE` & `werpy-2.1.2/LICENSES/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/README.md` & `werpy-2.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
 
-<h1 align="left">werpy - Word Error Rate for Python
+<h1 align="center">Word Error Rate for Python
 <a href="https://twitter.com/intent/tweet?text=Introducing%20%23werpy%20-%20the%20Python%20package%20for%20fast%20and%20accurate%20Word%20Error%20Rate%20(WER)%20calculation.%20Analyze%20text%20accuracy%2C%20enhance%20%23NLP%20models%2C%20and%20improve%20%23SpeechRecognition%20systems.%20Try%20it%20now%3A%20&url=https://github.com/analyticsinmotion/werpy&via=analyticsmotion&hashtags=PythonPackage,WordErrorRate,WER,NLP">
     <img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social" alt="Tweet">
   </a>
 </h1>
 
 <!-- badges: start -->
 
 | | |
 | --- | --- |
-| Meta | [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp; [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp; ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp; [![Analytics in Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-rounded.svg)](https://www.analyticsinmotion.com) |
-| Testing | [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp; [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp; [![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp; [![Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml)&nbsp;&nbsp; <!--[![CircleCI](https://dl.circleci.com/status-badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)&nbsp;&nbsp;--> |
-| Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![PyPI Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/werpy)&nbsp;&nbsp; [![sourcerank](https://img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/werpy)&nbsp;&nbsp; |
-
+| Meta | [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11%7C3.12-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp; [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;<!-- ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;--> [![Black Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)&nbsp;&nbsp; [![Analytics in Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-rounded.svg)](https://www.analyticsinmotion.com) |
+| Testing | [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp; [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp; [![CodeFactor](https://www.codefactor.io/repository/github/analyticsinmotion/werpy/badge)](https://www.codefactor.io/repository/github/analyticsinmotion/werpy)&nbsp;&nbsp; <!--[![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp;--> <!--[![Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml)&nbsp;&nbsp;--> [![CircleCI](https://dl.circleci.com/status-badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)&nbsp;&nbsp; [![codecov](https://codecov.io/gh/analyticsinmotion/werpy/graph/badge.svg?token=GGT823AVM8)](https://codecov.io/gh/analyticsinmotion/werpy) |
+| Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![PyPI Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/werpy)&nbsp;&nbsp;<!--[![sourcerank](https://img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/werpy)&nbsp;&nbsp;--> [![Documentation Status](https://readthedocs.org/projects/werpy/badge/?version=latest)](https://werpy.readthedocs.io/en/latest/?badge=latest)&nbsp;&nbsp; |
 
 
 <!-- badges: end -->
 
 ## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
-It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
+It has been designed with the flexibility to handle multiple input data types such as strings, lists and NumPy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
 Additionally, the summary function provides a comprehensive breakdown of the calculated results to assist in analyzing the specific errors quickly and in more detail.
 <br />
 
 ## Functions available in werpy
 The following table provides an overview of the functions that can be used in werpy.
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/
 52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
-************ wweerrppyy -- WWoorrdd EErrrroorr RRaattee ffoorr PPyytthhoonn_[[_TT_ww_ee_ee_tt_]] ************
+                ************ WWoorrdd EErrrroorr RRaattee ffoorr PPyytthhoonn_[[_TT_ww_ee_ee_tt_]] ************
 | | | | --- | --- | | Meta | [![Python Version](https://img.shields.io/badge/
-python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://
-www.python.org/downloads/)   [![werpy License](https://img.shields.io/badge/
-License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/
-blob/main/LICENSE)   ![Maintained](https://img.shields.io/badge/Maintained%3F-
-yes-green.svg)   [![Analytics in Motion](https://raw.githubusercontent.com/
-analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-
-rounded.svg)](https://www.analyticsinmotion.com) | | Testing | [![CodeQL]
-(https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/
-badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/
-codeql.yml)   [![Codacy Security Scan](https://github.com/analyticsinmotion/
-werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/
-analyticsinmotion/werpy/actions/workflows/codacy.yml)   [![Pylint](https://
-github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)]
-(https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)   [!
-[Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/
-bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/
-workflows/bandit.yml)   | | Package | [![Pypi](https://img.shields.io/pypi/v/
-werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)   [![PyPI
-Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https:
-//pypi.org/project/werpy/)   [![Downloads](https://static.pepy.tech/badge/
-werpy)](https://pepy.tech/project/werpy)   [![sourcerank](https://
-img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/
-werpy)   | ## What is werpy? **werpy** is a powerful yet lightweight Python
-package that rapidly calculates and analyzes the Word Error Rate (WER) between
-two sets of text. It has been designed with the flexibility to handle multiple
-input data types such as strings, lists and numpy arrays.
+python-3.8%7C3.9%7C3.10%7C3.11%7C3.12-blue?logo=python&logoColor=ffdd54)]
+(https://www.python.org/downloads/)   [![werpy License](https://img.shields.io/
+badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/
+werpy/blob/main/LICENSE)   [![Black Code Style](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black)   [![Analytics in
+Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/
+assets/images/analytics-in-motion-github-badge-rounded.svg)](https://
+www.analyticsinmotion.com) | | Testing | [![CodeQL](https://github.com/
+analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://
+github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)   [![Codacy
+Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/
+codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/
+workflows/codacy.yml)   [![CodeFactor](https://www.codefactor.io/repository/
+github/analyticsinmotion/werpy/badge)](https://www.codefactor.io/repository/
+github/analyticsinmotion/werpy)   [![CircleCI](https://dl.circleci.com/status-
+badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://
+dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)  
+[![codecov](https://codecov.io/gh/analyticsinmotion/werpy/graph/
+badge.svg?token=GGT823AVM8)](https://codecov.io/gh/analyticsinmotion/werpy) | |
+Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)]
+(https://pypi.org/project/werpy/)   [![PyPI Downloads](https://img.shields.io/
+pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)   [!
+[Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/
+werpy)   [![Documentation Status](https://readthedocs.org/projects/werpy/badge/
+?version=latest)](https://werpy.readthedocs.io/en/latest/?badge=latest)   | ##
+What is werpy? **werpy** is a powerful yet lightweight Python package that
+rapidly calculates and analyzes the Word Error Rate (WER) between two sets of
+text. It has been designed with the flexibility to handle multiple input data
+types such as strings, lists and NumPy arrays.
 The package also includes a full set of features such as normalizing the input
 text to account for data collection variability and the capability to easily
 assign different weights/penalties to specific error classifications
 (insertions, deletions, and substitutions). Additionally, the summary function
 provides a comprehensive breakdown of the calculated results to assist in
 analyzing the specific errors quickly and in more detail.
 ## Functions available in werpy The following table provides an overview of the
```

### Comparing `werpy-2.1.1/SECURITY.md` & `werpy-2.1.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/meson.build` & `werpy-2.1.2/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 project(
     'werpy', 
     'c', 'cython',
-    version : '2.1.1',
+    version : '2.1.2',
     license: 'BSD-3',
     meson_version: '>= 1.1.0',
     default_options : [
         'buildtype=debugoptimized',
         'warning_level=3',
         'c_std=c11'
         ]
```

### Comparing `werpy-2.1.1/pyproject.toml` & `werpy-2.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'wheel', 
     'Cython', 
     'numpy'
 ]
 
 [project]
 name = 'werpy'
-version = '2.1.1'
+version = '2.1.2'
 description = 'A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER).'
 readme = 'README.md'
 requires-python = '>=3.8'
 license = {file = 'LICENSE'}
 authors = [
   {name = 'Ross Armstrong', email = 'ross.armstrong@analyticsinmotion.com'},
 ]
@@ -55,19 +55,26 @@
   "numpy>=1.21.6; python_version<'3.11'",
   "numpy>=1.23.2; python_version>='3.11'",
   "pandas>=1.3.0"
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/analyticsinmotion/werpy"
 "Repository" = "https://github.com/analyticsinmotion/werpy"
+"Documentation" = "https://werpy.readthedocs.io/"
 "Bug Tracker" = "https://github.com/analyticsinmotion/werpy/issues"
 
 
+[project.optional-dependencies]
+docs = [
+    "sphinx==7.2.6",
+    "sphinx-nefertiti== 0.3.2",
+]
+
+
 # For localized testing of the package on Windows OS
 #[tool.cibuildwheel]
 #build = "cp38-* cp39-* cp310-* cp311-* cp312-*"
 #skip = "*-win32 *-manylinux_i686 *-manylinux2010_i686 *-manylinux2014_i686 *-manylinux_aarch64 *-manylinux_ppc64le *-manylinux_s390x *-musllinux_i686 *-musllinux_aarch64 *-musllinux_ppc64le *-musllinux_s390x"
 
 #[tool.cibuildwheel.windows]
 #build = "cp38-* cp39-* cp310-* cp311-* cp312-*"
```

### Comparing `werpy-2.1.1/tests/test_normalize.py` & `werpy-2.1.2/tests/test_normalize.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,127 +19,131 @@
 To run the tests, execute this module as the main program.
 
 Note: If the 'normalize' module is not imported successfully, 
 an ImportError is raised to ensure that the required module is available for testing.
 """
 
 import unittest
+from werpy.normalize import normalize
 
-try:
-    from werpy.normalize import normalize
-except ImportError as exc:
-    raise ImportError("The 'normalize' module could not be imported. Make sure it is installed.") from exc
 
 class TestNormalize(unittest.TestCase):
     """
     TestNormalize - Unit tests for the 'normalize' function in 'werpy.normalize'.
 
-    This class defines test cases to verify the correctness of the 'normalize' function, 
-    which is responsible for normalizing translations, both reference and hypothesis, 
+    This class defines test cases to verify the correctness of the 'normalize' function,
+    which is responsible for normalizing translations, both reference and hypothesis,
     to enable word error rate (WER) calculations.
 
     Test cases:
     - 'test_normalize_reference_translation': Test the normalization of reference translations.
     - 'test_normalize_hypothesis_translation': Test the normalization of hypothesis translations.
     - 'test_normalize_string': Test the normalization of a single string.
 
-    Each test case compares the output of the 'normalize' function with the expected normalized translations 
+    Each test case compares the output of the 'normalize' function with the expected normalized translations
     and raises an AssertionError if the actual output does not match the expected values.
 
     Attributes:
         None
 
     Methods:
         - 'test_normalize_reference_translation': Test the normalization of reference translations.
         - 'test_normalize_hypothesis_translation': Test the normalization of hypothesis translations.
         - 'test_normalize_string': Test the normalization of a single string.
 
     To run the tests, execute this class as part of the test suite in the main program.
 
-    Note: If the 'normalize' module is not imported successfully, 
+    Note: If the 'normalize' module is not imported successfully,
     an ImportError is raised to ensure that the required module is available for testing.
     """
+
     def test_normalize_reference(self):
         """
         Test the normalization of reference translations.
         """
         reference = [
-            '     It is consumed domestically           and exported to other countries.     ',
-            'The Sugar Bear character was popular enough to have occasional premium toys.',
-            'It is one of the most watched television networks in the country.',
-            'It could be carried and prepared by the individual soldier.',
-            'He was executed in a Lubyanka prison cellar.',
-            'Rufino Street in Makati, right inside the Makati Central Business District.',
-            'Its estuary is considered to have abnormally low rates of dissolved oxygen.',
-            'He later cited his first wife Anita as the inspiration for the song.',
-            'Gadya is the nearest rural locality.',
-            'Taxes are a tool in the adjustment of the economy.'
+            "     It is consumed domestically           and exported to other countries.     ",
+            "The Sugar Bear character was popular enough to have occasional premium toys.",
+            "It is one of the most watched television networks in the country.",
+            "It could be carried and prepared by the individual soldier.",
+            "He was executed in a Lubyanka prison cellar.",
+            "Rufino Street in Makati, right inside the Makati Central Business District.",
+            "Its estuary is considered to have abnormally low rates of dissolved oxygen.",
+            "He later cited his first wife Anita as the inspiration for the song.",
+            "Gadya is the nearest rural locality.",
+            "Taxes are a tool in the adjustment of the economy.",
         ]
         expected_normalized_reference = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bear character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in a lubyanka prison cellar',
-            'rufino street in makati right inside the makati central business district',
-            'its estuary is considered to have abnormally low rates of dissolved oxygen',
-            'he later cited his first wife anita as the inspiration for the song',
-            'gadya is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
+            "it is consumed domestically and exported to other countries",
+            "the sugar bear character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in a lubyanka prison cellar",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "gadya is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
         ]
 
-        try:
-            self.assertEqual(normalize(reference), expected_normalized_reference)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_normalize_reference: {e}")
-
+        self.assertEqual(normalize(reference), expected_normalized_reference)
 
     def test_normalize_hypothesis(self):
         """
         Test the normalization of hypothesis translations.
         """
         hypothesis = [
-            'it is consumed domestically and exported to other countries ',
-            'the sugar bare character was popular enough to have occasional premium toys ',
-            'it is one of the most watched television networks in the country ',
-            'it could be carried and prepared by the individual soldier ',
-            'he was executed in alabianca prison seller ',
-            'rofino street in mccauti right inside the macasi central business district ',
+            "it is consumed domestically and exported to other countries ",
+            "the sugar bare character was popular enough to have occasional premium toys ",
+            "it is one of the most watched television networks in the country ",
+            "it could be carried and prepared by the individual soldier ",
+            "he was executed in alabianca prison seller ",
+            "rofino street in mccauti right inside the macasi central business district ",
             "it's estiary is considered to have a normally low rates of dissolved oxygen ",
-            'he later sighted his first wife anita as the inspiration for the song ',
-            'gadia is the nearest rural locality ',
-            'taxes are a tool in the adjustment of the economy '
+            "he later sighted his first wife anita as the inspiration for the song ",
+            "gadia is the nearest rural locality ",
+            "taxes are a tool in the adjustment of the economy ",
         ]
         expected_normalized_hypothesis = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bare character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in alabianca prison seller',
-            'rofino street in mccauti right inside the macasi central business district',
-            'its estiary is considered to have a normally low rates of dissolved oxygen',
-            'he later sighted his first wife anita as the inspiration for the song',
-            'gadia is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
+            "it is consumed domestically and exported to other countries",
+            "the sugar bare character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in alabianca prison seller",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "gadia is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
         ]
 
-        try:
-            self.assertEqual(normalize(hypothesis), expected_normalized_hypothesis)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_normalize_hypothesis: {e}")
-
+        self.assertEqual(normalize(hypothesis), expected_normalized_hypothesis)
 
     def test_normalize_string(self):
         """
         Test the normalization of a single string.
         """
-        reference = normalize(" it's Consumed Domestically  And exported to other countries.")
+        reference = normalize(
+            " it's Consumed Domestically  And exported to other countries."
+        )
+
+        expected_normalized_reference = (
+            "its consumed domestically and exported to other countries"
+        )
+
+        self.assertEqual(normalize(reference), expected_normalized_reference)
 
-        expected_normalized_reference = 'its consumed domestically and exported to other countries'
+    def test_normalize_integers(self):
+        """
+        Test the normalize function with numerical reference and hypothesis inputs.
+
+        This test evaluates the NORMALIZE function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an TypeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        with self.assertRaises(TypeError):
+            normalize(ref)
 
-        try:
-            self.assertEqual(normalize(reference), expected_normalized_reference)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_normalize_string: {e}")
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_summary.py` & `werpy-2.1.2/tests/test_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,67 +17,88 @@
 
 Note: If the 'summary' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
 import pandas as pd
+from werpy.summary import summary
 
-try:
-    from werpy.summary import summary
-except ImportError as exc:
-    raise ImportError("The 'summary' module could not be imported. Make sure it is installed.") from exc
 
 class TestSummary(unittest.TestCase):
     """
-    This class contains unit tests for the 'summary' function, which calculates the Word Error Rate (WER) 
+    This class contains unit tests for the 'summary' function, which calculates the Word Error Rate (WER)
     between reference and hypothesis text sequences, displaying the summary results as a dataframe.
     """
+
     def test_summary_example_1(self):
         """
         Test the summary function with multiple reference and hypothesis strings.
 
-        This test evaluates the SUMMARY function with multiple reference and hypothesis text sequences. 
+        This test evaluates the SUMMARY function with multiple reference and hypothesis text sequences.
         It verifies that the calculated SUMMARY dataframe aligns with the expected output dataframe.
 
         """
-        ref = ['it is consumed domestically and exported to other countries',
-               'rufino street in makati right inside the makati central business district',
-               'its estuary is considered to have abnormally low rates of dissolved oxygen',
-               'he later cited his first wife anita as the inspiration for the song',
-               'no one else could claim that']
-        hyp = ['it is consumed domestically and exported to other countries',
-               'rofino street in mccauti right inside the macasi central business district',
-               'its estiary is considered to have a normally low rates of dissolved oxygen',
-               'he later sighted his first wife anita as the inspiration for the song',
-               'no one else could claim that']
+        ref = [
+            "it is consumed domestically and exported to other countries",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "no one else could claim that",
+        ]
+        hyp = [
+            "it is consumed domestically and exported to other countries",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "no one else could claim that",
+        ]
 
         # Generate the actual_result DataFrame
         actual_result = summary(ref, hyp)
 
-        expected_result = pd.DataFrame({
-            'wer': [0.000000, 0.272727, 0.250000, 0.076923, 0.000000],
-            'ld': [0, 3, 3, 1, 0],
-            'm': [9, 11, 12, 13, 6],
-            'insertions': [0, 0, 1, 0, 0],
-            'deletions': [0, 0, 0, 0, 0],
-            'substitutions': [0, 3, 2, 1, 0],
-            'inserted_words': [[], [], ['a'], [], []],
-            'deleted_words': [[], [], [], [], []],
-            'substituted_words': [[],
-                                  [('rufino', 'rofino'), ('makati', 'mccauti'), ('makati', 'macasi')],
-                                  [('estuary', 'estiary'), ('abnormally', 'normally')],
-                                  [('cited', 'sighted')],
-                                  []]
-            })
+        expected_result = pd.DataFrame(
+            {
+                "wer": [0.000000, 0.272727, 0.250000, 0.076923, 0.000000],
+                "ld": [0, 3, 3, 1, 0],
+                "m": [9, 11, 12, 13, 6],
+                "insertions": [0, 0, 1, 0, 0],
+                "deletions": [0, 0, 0, 0, 0],
+                "substitutions": [0, 3, 2, 1, 0],
+                "inserted_words": [[], [], ["a"], [], []],
+                "deleted_words": [[], [], [], [], []],
+                "substituted_words": [
+                    [],
+                    [("rufino", "rofino"), ("makati", "mccauti"), ("makati", "macasi")],
+                    [("estuary", "estiary"), ("abnormally", "normally")],
+                    [("cited", "sighted")],
+                    [],
+                ],
+            }
+        )
         # Set the data type of the "ld" column to int64
-        #expected_result['ld'] = expected_result['ld'].astype('int32')
+        # expected_result['ld'] = expected_result['ld'].astype('int32')
 
         try:
             pd.testing.assert_frame_equal(expected_result, actual_result)
             print("DataFrames are equal.")
-        except AssertionError as e:
-            print("DataFrames are not equal. Differences:\n", e)
+        except AssertionError as error:  # pragma: no cover
+            print("DataFrames are not equal. Differences:\n", error)
+
+    def test_summary_example_2(self):
+        """
+        Test the summary function with numerical reference and hypothesis inputs.
+
+        This test evaluates the SUMMARY function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in wer module
+        expected_result = None
+
+        self.assertEqual(summary(ref, hyp), expected_result)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_summaryp.py` & `werpy-2.1.2/tests/test_summaryp.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,63 +19,131 @@
 
 Note: If the 'summaryp' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
 import pandas as pd
+from werpy.summaryp import summaryp
 
-try:
-    from werpy.summaryp import summaryp
-except ImportError as exc:
-    raise ImportError("The 'summaryp' module could not be imported. Make sure it is installed.") from exc
 
 class TestSummaryp(unittest.TestCase):
     """
-    This class contains unit tests for the 'summaryp' function, which calculates the Word Error Rate (WER) 
+    This class contains unit tests for the 'summaryp' function, which calculates the Word Error Rate (WER)
     between reference and hypothesis text sequences, displaying the summary results as a dataframe.
     """
+
     def test_summaryp_example_1(self):
         """
         Test the summaryp function with multiple reference and hypothesis strings.
 
-        This test evaluates the SUMMARYP function with multiple reference and hypothesis text sequences. 
+        This test evaluates the SUMMARYP function with multiple reference and hypothesis text sequences.
         It verifies that the calculated SUMMARYP dataframe aligns with the expected output dataframe.
 
         """
-        ref = ['the tower caused minor discontent because it blocked sight lines of central park',
-               'her father was an alderman in the city government', 
-               'he was commonly referred to as the blacksmith of ballinalee']
-        hyp = ['the tower caused minor discontent because it blocked sightlines of central park',
-               'our father was an alderman in the city government', 
-               'he was commonly referred to as the blacksmith of balen alley']
+        ref = [
+            "the tower caused minor discontent because it blocked sight lines of central park",
+            "her father was an alderman in the city government",
+            "he was commonly referred to as the blacksmith of ballinalee",
+        ]
+        hyp = [
+            "the tower caused minor discontent because it blocked sightlines of central park",
+            "our father was an alderman in the city government",
+            "he was commonly referred to as the blacksmith of balen alley",
+        ]
 
         # Generate the actual_result DataFrame
-        actual_result = summaryp(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
+        actual_result = summaryp(
+            ref,
+            hyp,
+            insertions_weight=0.5,
+            deletions_weight=0.5,
+            substitutions_weight=1,
+        )
 
         data = {
-            'wer': [0.15384615384615385, 0.1111111111111111, 0.2],
-            'werp': [0.11538461538461539, 0.1111111111111111, 0.15],
-            'ld': [2, 1, 2],
-            'm': [13, 9, 10],
-            'insertions': [0, 0, 1],
-            'deletions': [1, 0, 0],
-            'substitutions': [1, 1, 1],
-            'inserted_words': [[], [], ['balen']],
-            'deleted_words': [['sight'], [], []],
-            'substituted_words': [[('lines', 'sightlines')], [('her', 'our')], [('ballinalee', 'alley')]]
-            }
+            "wer": [0.15384615384615385, 0.1111111111111111, 0.2],
+            "werp": [0.11538461538461539, 0.1111111111111111, 0.15],
+            "ld": [2, 1, 2],
+            "m": [13, 9, 10],
+            "insertions": [0, 0, 1],
+            "deletions": [1, 0, 0],
+            "substitutions": [1, 1, 1],
+            "inserted_words": [[], [], ["balen"]],
+            "deleted_words": [["sight"], [], []],
+            "substituted_words": [
+                [("lines", "sightlines")],
+                [("her", "our")],
+                [("ballinalee", "alley")],
+            ],
+        }
 
         expected_result = pd.DataFrame(data)
 
         # Set the data type of the "ld" column to int64
-        #expected_result['ld'] = expected_result['ld'].astype('int32')
+        # expected_result['ld'] = expected_result['ld'].astype('int32')
+
+        try:
+            pd.testing.assert_frame_equal(expected_result, actual_result)
+            print("DataFrames are equal.")
+        except AssertionError as error:  # pragma: no cover
+            print("DataFrames are not equal. Differences:\n", error)
+
+    def test_summaryp_example_2(self):
+        """
+        Test the summaryp function with multiple reference and hypothesis strings.
+
+        This test evaluates the SUMMARYP function with multiple reference and hypothesis text sequences.
+        It verifies that the calculated SUMMARYP dataframe aligns with the expected output dataframe.
+
+        """
+        ref = "the tower caused minor discontent because it blocked sight lines of central park"
+        hyp = "the tower caused minor discontent because it blocked sightlines of central park"
+
+        # Generate the actual_result DataFrame
+        actual_result = summaryp(
+            ref,
+            hyp,
+            insertions_weight=0.5,
+            deletions_weight=0.5,
+            substitutions_weight=1,
+        )
+
+        data = {
+            "wer": [0.15384615384615385],
+            "werp": [0.11538461538461539],
+            "ld": [2],
+            "m": [13],
+            "insertions": [0],
+            "deletions": [1],
+            "substitutions": [1],
+            "inserted_words": [[]],
+            "deleted_words": [["sight"]],
+            "substituted_words": [[("lines", "sightlines")]],
+        }
+
+        expected_result = pd.DataFrame(data)
 
         try:
             pd.testing.assert_frame_equal(expected_result, actual_result)
             print("DataFrames are equal.")
-        except AssertionError as e:
-            print("DataFrames are not equal. Differences:\n", e)
+        except AssertionError as error:  # pragma: no cover
+            print("DataFrames are not equal. Differences:\n", error)
+
+    def test_summaryp_example_3(self):
+        """
+        Test the summaryp function with numerical reference and hypothesis inputs.
+
+        This test evaluates the SUMMARYP function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in wer module
+        expected_result = None
+
+        self.assertEqual(summaryp(ref, hyp, 0.5, 0.5, 1), expected_result)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_wer.py` & `werpy-2.1.2/tests/test_wer.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,90 +20,93 @@
 For more details on the 'wer' function and how to use it, please refer to the 'werpy' package documentation.
 
 Note: If the 'wer' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
+from werpy.wer import wer
 
-try:
-    from werpy.wer import wer
-except ImportError as exc:
-    raise ImportError("The 'wer' module could not be imported. Make sure it is installed.") from exc
 
 class TestWer(unittest.TestCase):
     """
-    This class contains unit tests for the 'wer' function, which calculates the Word Error Rate (WER) 
+    This class contains unit tests for the 'wer' function, which calculates the Word Error Rate (WER)
     between reference and hypothesis text sequences.
     """
+
     def test_wer_example_1(self):
         """
         Test the wer function with a simple example.
 
-        This test checks the WER function with a basic example of reference and hypothesis strings 
+        This test checks the WER function with a basic example of reference and hypothesis strings
         and ensures that the calculated WER matches the expected result.
         """
-        try:
-            self.assertEqual(wer('i love cold pizza', 'i love pizza'), 0.25)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wer_example_1: {e}")
-
+        self.assertEqual(wer("i love cold pizza", "i love pizza"), 0.25)
 
     def test_wer_example_2(self):
         """
         Test the wer function with multiple reference and hypothesis strings.
 
-        This test evaluates the WER function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WER function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WER aligns with the expected result.
 
         """
-        ref = ['i love cold pizza','the sugar bear character was popular']
-        hyp = ['i love pizza','the sugar bare character was popular']
+        ref = ["i love cold pizza", "the sugar bear character was popular"]
+        hyp = ["i love pizza", "the sugar bare character was popular"]
         expected_result = 0.2
 
-        try:
-            self.assertEqual(wer(ref, hyp), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wer_example_2: {e}")
-
+        self.assertEqual(wer(ref, hyp), expected_result)
 
     def test_wer_example_3(self):
         """
         Test the wer function with longer text sequences.
 
-        This test assesses the WER function's performance with longer reference and hypothesis text sequences. 
+        This test assesses the WER function's performance with longer reference and hypothesis text sequences.
         It verifies that the calculated WER closely matches the expected result.
 
         """
         ref = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bear character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in a lubyanka prison cellar',
-            'rufino street in makati right inside the makati central business district',
-            'its estuary is considered to have abnormally low rates of dissolved oxygen',
-            'he later cited his first wife anita as the inspiration for the song',
-            'gadya is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bear character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in a lubyanka prison cellar",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "gadya is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         hyp = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bare character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in alabianca prison seller',
-            'rofino street in mccauti right inside the macasi central business district',
-            'its estiary is considered to have a normally low rates of dissolved oxygen',
-            'he later sighted his first wife anita as the inspiration for the song',
-            'gadia is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bare character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in alabianca prison seller",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "gadia is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         expected_result = 0.11650485436893204
 
-        try:
-            self.assertEqual(wer(ref, hyp), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wer_example_3: {e}")
+        self.assertEqual(wer(ref, hyp), expected_result)
+
+    def test_wer_example_4(self):
+        """
+        Test the wer function with numerical reference and hypothesis inputs.
+
+        This test evaluates the WER function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in wer module
+        expected_result = None
+
+        self.assertEqual(wer(ref, hyp), expected_result)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_werp.py` & `werpy-2.1.2/tests/test_werp.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,128 +16,130 @@
 For more details on the 'werp' function and how to use it, please refer to the 'werpy' package documentation.
 
 Note: If the 'werp' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
+from werpy.werp import werp
 
-try:
-    from werpy.werp import werp
-except ImportError as exc:
-    raise ImportError("The 'werp' module could not be imported. Make sure it is installed.") from exc
 
 class TestWerp(unittest.TestCase):
     """
-    This class contains unit tests for the 'werp' function, which calculates the weighted Word Error Rate (WER) 
+    This class contains unit tests for the 'werp' function, which calculates the weighted Word Error Rate (WER)
     between reference and hypothesis text sequences.
     """
+
     def test_werp_example_1(self):
         """
         Test the werp function with a simple example.
 
-        This test checks the WERP function with a basic example of reference and hypothesis strings 
+        This test checks the WERP function with a basic example of reference and hypothesis strings
         and ensures that the calculated WERP matches the expected result.
         """
-        try:
-            self.assertEqual(werp('i love cold pizza', 'i love pizza', 0.5, 0.5, 1), 0.125)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werp_example_1: {e}")
-
+        self.assertEqual(werp("i love cold pizza", "i love pizza", 0.5, 0.5, 1), 0.125)
 
     def test_werp_example_2(self):
         """
         Test the werp function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERP function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERP function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERP aligns with the expected results.
 
         """
-        ref = ['i love cold pizza','the sugar bear character was popular']
-        hyp = ['i love pizza','the sugar bare character was popular']
+        ref = ["i love cold pizza", "the sugar bear character was popular"]
+        hyp = ["i love pizza", "the sugar bare character was popular"]
         expected_result = 0.15
 
-        try:
-            self.assertEqual(werp(
-                ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1
-                ), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werp_example_2: {e}")
-
+        self.assertEqual(
+            werp(
+                ref,
+                hyp,
+                insertions_weight=0.5,
+                deletions_weight=0.5,
+                substitutions_weight=1,
+            ),
+            expected_result,
+        )
 
     def test_werp_example_3(self):
         """
         Test the werp function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERP function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERP function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERP aligns with the expected results.
 
         """
-        ref = ['no one else could claim that','she cited multiple reasons why']
-        hyp = ['no one else could claim that','she sighted multiple reasons why']
+        ref = ["no one else could claim that", "she cited multiple reasons why"]
+        hyp = ["no one else could claim that", "she sighted multiple reasons why"]
         expected_result = 0.09090909090909091
 
-        try:
-            self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werp_example_3: {e}")
-
+        self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
 
     def test_werp_example_4(self):
         """
         Test the werp function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERP function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERP function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERP aligns with the expected results.
 
         """
-        ref = ['it was beautiful and sunny today']
-        hyp = ['it was a beautiful and sunny day']
+        ref = ["it was beautiful and sunny today"]
+        hyp = ["it was a beautiful and sunny day"]
         expected_result = 0.25
 
-        try:
-            self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werp_example_4: {e}")
-
+        self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
 
     def test_werp_example_5(self):
         """
         Test the werp function with longer text sequences.
 
-        This test assesses the WERP function's performance with longer reference and hypothesis text sequences. 
+        This test assesses the WERP function's performance with longer reference and hypothesis text sequences.
         It verifies that the calculated WERP closely matches the expected results.
 
         """
         ref = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bear character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in a lubyanka prison cellar',
-            'rufino street in makati right inside the makati central business district',
-            'its estuary is considered to have abnormally low rates of dissolved oxygen',
-            'he later cited his first wife anita as the inspiration for the song',
-            'gadya is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bear character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in a lubyanka prison cellar",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "gadya is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         hyp = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bare character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in alabianca prison seller',
-            'rofino street in mccauti right inside the macasi central business district',
-            'its estiary is considered to have a normally low rates of dissolved oxygen',
-            'he later sighted his first wife anita as the inspiration for the song',
-            'gadia is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bare character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in alabianca prison seller",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "gadia is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         expected_result = 0.10679611650485436
 
-        try:
-            self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werp_example_4: {e}")
+        self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
+
+    def test_werp_example_6(self):
+        """
+        Test the werp function with numerical reference and hypothesis inputs.
+
+        This test evaluates the WERP function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in werp module
+        expected_result = None
+
+        self.assertEqual(werp(ref, hyp, 0.5, 0.5, 1), expected_result)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_werps.py` & `werpy-2.1.2/tests/test_werps.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,148 +17,161 @@
 For more details on the 'werps' function and how to use it, please refer to the 'werpy' package documentation.
 
 Note: If the 'werps' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
+from werpy.werps import werps
 
-try:
-    from werpy.werps import werps
-except ImportError as exc:
-    raise ImportError("The 'werps' module could not be imported. Make sure it is installed.") from exc
 
 class TestWerps(unittest.TestCase):
     """
-    This class contains unit tests for the 'werps' function, which calculates the weighted Word Error Rate (WER) 
+    This class contains unit tests for the 'werps' function, which calculates the weighted Word Error Rate (WER)
     between reference and hypothesis text sequences.
     """
+
     def test_werps_example_1(self):
         """
         Test the werps function with a simple example.
 
-        This test checks the WERPS function with a basic example of reference and hypothesis strings 
+        This test checks the WERPS function with a basic example of reference and hypothesis strings
         and ensures that the calculated WERPS matches the expected result.
         """
-        try:
-            self.assertEqual(werps('i love cold pizza', 'i love pizza', 0.5, 0.5, 1), 0.125)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_1: {e}")
-
+        self.assertEqual(werps("i love cold pizza", "i love pizza", 0.5, 0.5, 1), 0.125)
 
     def test_werps_example_2(self):
         """
         Test the werps function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERPS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERPS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERPS aligns with the expected results.
 
         """
-        ref = ['i love cold pizza','the sugar bear character was popular']
-        hyp = ['i love pizza','the sugar bare character was popular']
+        ref = ["i love cold pizza", "the sugar bear character was popular"]
+        hyp = ["i love pizza", "the sugar bare character was popular"]
         expected_result = [0.125, 0.16666666666666666]
 
-        try:
-            self.assertEqual(werps(
-                ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1
-                ), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_2: {e}")
-
+        self.assertEqual(
+            werps(
+                ref,
+                hyp,
+                insertions_weight=0.5,
+                deletions_weight=0.5,
+                substitutions_weight=1,
+            ),
+            expected_result,
+        )
 
     def test_werps_example_3(self):
         """
         Test the werps function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERPS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERPS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERPS aligns with the expected results.
 
         """
-        ref = ['no one else could claim that','she cited multiple reasons why']
-        hyp = ['no one else could claim that','she sighted multiple reasons why']
+        ref = ["no one else could claim that", "she cited multiple reasons why"]
+        hyp = ["no one else could claim that", "she sighted multiple reasons why"]
         expected_result = [0.0, 0.2]
 
-        try:
-            self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_3: {e}")
-
+        self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
 
     def test_werps_example_4(self):
         """
         Test the werps function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERPS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERPS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERPS aligns with the expected results.
 
         """
-        ref = ['it was beautiful and sunny today']
-        hyp = ['it was a beautiful and sunny day']
+        ref = ["it was beautiful and sunny today"]
+        hyp = ["it was a beautiful and sunny day"]
         expected_result = [0.25]
 
-        try:
-            self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_4: {e}")
-
+        self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
 
     def test_werps_example_5(self):
         """
         Test the werps function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERPS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERPS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WERPS aligns with the expected results.
 
         """
-        ref = ['it blocked sight lines of central park', 'her father was an alderman in the city government']
-        hyp = ['it blocked sightlines of central park', 'our father was an elder man in the city government']
+        ref = [
+            "it blocked sight lines of central park",
+            "her father was an alderman in the city government",
+        ]
+        hyp = [
+            "it blocked sightlines of central park",
+            "our father was an elder man in the city government",
+        ]
         expected_result = [0.21428571428571427, 0.2777777777777778]
 
-        try:
-            self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_5: {e}")
-
+        self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
 
     def test_werps_example_6(self):
         """
         Test the werps function with longer text sequences.
 
-        This test assesses the WERPS function's performance with longer reference and hypothesis text sequences. 
+        This test assesses the WERPS function's performance with longer reference and hypothesis text sequences.
         It verifies that the calculated WERPS closely matches the expected results.
 
         """
         ref = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bear character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in a lubyanka prison cellar',
-            'rufino street in makati right inside the makati central business district',
-            'its estuary is considered to have abnormally low rates of dissolved oxygen',
-            'he later cited his first wife anita as the inspiration for the song',
-            'gadya is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bear character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in a lubyanka prison cellar",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "gadya is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         hyp = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bare character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in alabianca prison seller',
-            'rofino street in mccauti right inside the macasi central business district',
-            'its estiary is considered to have a normally low rates of dissolved oxygen',
-            'he later sighted his first wife anita as the inspiration for the song',
-            'gadia is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
-        expected_result = [0.0, 0.08333333333333333, 0.0, 0.0, 0.3125, 0.2727272727272727,
-                           0.20833333333333334, 0.07692307692307693, 0.16666666666666666, 0.0]
-
-
-        try:
-            self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_werps_example_6: {e}")
+            "it is consumed domestically and exported to other countries",
+            "the sugar bare character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in alabianca prison seller",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "gadia is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
+        expected_result = [
+            0.0,
+            0.08333333333333333,
+            0.0,
+            0.0,
+            0.3125,
+            0.2727272727272727,
+            0.20833333333333334,
+            0.07692307692307693,
+            0.16666666666666666,
+            0.0,
+        ]
+
+        self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
+
+    def test_werps_example_7(self):
+        """
+        Test the werps function with numerical reference and hypothesis inputs.
+
+        This test evaluates the WERPS function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in werps module
+        expected_result = None
+
+        self.assertEqual(werps(ref, hyp, 0.5, 0.5, 1), expected_result)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/tests/test_wers.py` & `werpy-2.1.2/tests/test_wers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,109 +16,118 @@
 For more details on the 'wers' function and how to use it, please refer to the 'werpy' package documentation.
 
 Note: If the 'wers' module is not imported successfully, an ImportError is raised 
 to ensure that the required module is available for testing.
 """
 
 import unittest
+from werpy.wers import wers
 
-try:
-    from werpy.wers import wers
-except ImportError as exc:
-    raise ImportError("The 'wers' module could not be imported. Make sure it is installed.") from exc
 
 class TestWers(unittest.TestCase):
     """
-    This class contains unit tests for the 'wers' function, which calculates the Word Error Rate (WER) 
+    This class contains unit tests for the 'wers' function, which calculates the Word Error Rate (WER)
     between reference and hypothesis text sequences.
     """
+
     def test_wers_example_1(self):
         """
         Test the wers function with a simple example.
 
-        This test checks the WERS function with a basic example of reference and hypothesis strings 
+        This test checks the WERS function with a basic example of reference and hypothesis strings
         and ensures that the calculated WER matches the expected result.
         """
-        try:
-            self.assertEqual(wers('i love cold pizza', 'i love pizza'), 0.25)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wers_example_1: {e}")
-
+        self.assertEqual(wers("i love cold pizza", "i love pizza"), 0.25)
 
     def test_wers_example_2(self):
         """
         Test the wers function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WER aligns with the expected results.
 
         """
-        ref = ['i love cold pizza','the sugar bear character was popular']
-        hyp = ['i love pizza','the sugar bare character was popular']
+        ref = ["i love cold pizza", "the sugar bear character was popular"]
+        hyp = ["i love pizza", "the sugar bare character was popular"]
         expected_result = [0.25, 0.16666666666666666]
 
-        try:
-            self.assertEqual(wers(ref, hyp), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wers_example_2: {e}")
-
+        self.assertEqual(wers(ref, hyp), expected_result)
 
     def test_wers_example_3(self):
         """
         Test the wers function with multiple reference and hypothesis strings.
 
-        This test evaluates the WERS function with multiple reference and hypothesis text sequences. 
+        This test evaluates the WERS function with multiple reference and hypothesis text sequences.
         It verifies that the calculated WER aligns with the expected results.
 
         """
-        ref = ['no one else could claim that','she cited multiple reasons why']
-        hyp = ['no one else could claim that','she sighted multiple reasons why']
+        ref = ["no one else could claim that", "she cited multiple reasons why"]
+        hyp = ["no one else could claim that", "she sighted multiple reasons why"]
         expected_result = [0.0, 0.2]
 
-        try:
-            self.assertEqual(wers(ref, hyp), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wers_example_3: {e}")
-
+        self.assertEqual(wers(ref, hyp), expected_result)
 
     def test_wers_example_4(self):
         """
         Test the wers function with longer text sequences.
 
-        This test assesses the WERS function's performance with longer reference and hypothesis text sequences. 
+        This test assesses the WERS function's performance with longer reference and hypothesis text sequences.
         It verifies that the calculated WER closely matches the expected results.
 
         """
         ref = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bear character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in a lubyanka prison cellar',
-            'rufino street in makati right inside the makati central business district',
-            'its estuary is considered to have abnormally low rates of dissolved oxygen',
-            'he later cited his first wife anita as the inspiration for the song',
-            'gadya is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
+            "it is consumed domestically and exported to other countries",
+            "the sugar bear character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in a lubyanka prison cellar",
+            "rufino street in makati right inside the makati central business district",
+            "its estuary is considered to have abnormally low rates of dissolved oxygen",
+            "he later cited his first wife anita as the inspiration for the song",
+            "gadya is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
         hyp = [
-            'it is consumed domestically and exported to other countries',
-            'the sugar bare character was popular enough to have occasional premium toys',
-            'it is one of the most watched television networks in the country',
-            'it could be carried and prepared by the individual soldier',
-            'he was executed in alabianca prison seller',
-            'rofino street in mccauti right inside the macasi central business district',
-            'its estiary is considered to have a normally low rates of dissolved oxygen',
-            'he later sighted his first wife anita as the inspiration for the song',
-            'gadia is the nearest rural locality',
-            'taxes are a tool in the adjustment of the economy'
-            ]
-        expected_result = [0.0, 0.08333333333333333, 0.0, 0.0, 0.375, 0.2727272727272727,
-                           0.25, 0.07692307692307693, 0.16666666666666666, 0.0]
-
-        try:
-            self.assertEqual(wers(ref, hyp), expected_result)
-        except AssertionError as e:
-            self.fail(f"Assertion error in test_wers_example_4: {e}")
+            "it is consumed domestically and exported to other countries",
+            "the sugar bare character was popular enough to have occasional premium toys",
+            "it is one of the most watched television networks in the country",
+            "it could be carried and prepared by the individual soldier",
+            "he was executed in alabianca prison seller",
+            "rofino street in mccauti right inside the macasi central business district",
+            "its estiary is considered to have a normally low rates of dissolved oxygen",
+            "he later sighted his first wife anita as the inspiration for the song",
+            "gadia is the nearest rural locality",
+            "taxes are a tool in the adjustment of the economy",
+        ]
+        expected_result = [
+            0.0,
+            0.08333333333333333,
+            0.0,
+            0.0,
+            0.375,
+            0.2727272727272727,
+            0.25,
+            0.07692307692307693,
+            0.16666666666666666,
+            0.0,
+        ]
+
+        self.assertEqual(wers(ref, hyp), expected_result)
+
+    def test_wers_example_5(self):
+        """
+        Test the wers function with numerical reference and hypothesis inputs.
+
+        This test evaluates the WERS function with numerical reference and hypothesis inputs.
+        It verifies that the numerical input will raise an AttributeError.
+
+        """
+        ref = [1, 2, 3, 4]
+        hyp = [2, 3, 3, 3]
+        # The actual return value is None from the try/except block in wers module
+        expected_result = None
+
+        self.assertEqual(wers(ref, hyp), expected_result)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `werpy-2.1.1/werpy/__pycache__/metrics.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/normalize.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/normalize.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/summary.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/summary.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/wer.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/wer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/werp.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/werp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/werps.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/werps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/__pycache__/wers.cpython-311.pyc` & `werpy-2.1.2/werpy/__pycache__/wers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/errorhandler.py` & `werpy-2.1.2/werpy/errorhandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,16 @@
         This function will return a ragged array containing the Word Error Rate, Levenshtein distance, the number of
         words in the reference sequence, insertions count, deletions count, substitutions count, a list of inserted
         words, a list of deleted words and a list of substituted words.
     """
     try:
         word_error_rate_breakdown = metrics(reference, hypothesis)
     except ValueError as exc:
-        raise ValueError("The Reference and Hypothesis input parameters must have the same number of elements.") from\
-            exc
+        raise ValueError(
+            "The Reference and Hypothesis input parameters must have the same number of elements."
+        ) from exc
     except AttributeError as exc:
-        raise AttributeError("All text should be in a string format. Please check your input does not include any "
-                             "Numeric data types.") from exc
+        raise AttributeError(
+            "All text should be in a string format. Please check your input does not include any "
+            "Numeric data types."
+        ) from exc
     return word_error_rate_breakdown
```

### Comparing `werpy-2.1.1/werpy/metrics.pyx` & `werpy-2.1.2/werpy/metrics.pyx`

 * *Files identical despite different names*

### Comparing `werpy-2.1.1/werpy/normalize.py` & `werpy-2.1.2/werpy/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 """
 
 import string
 
 
 def normalize(text):
     """
-    This function serves as a versatile text preprocessing tool, designed to transform 
-    text data into an optimal format for a variety of natural language processing tasks, 
+    This function serves as a versatile text preprocessing tool, designed to transform
+    text data into an optimal format for a variety of natural language processing tasks,
     such as calculating the Word Error Rate (WER).
-    
-    Its core functionalities encompass removing punctuation, converting text to 
-    lowercase, and eliminating unnecessary whitespace. 
+
+    Its core functionalities encompass removing punctuation, converting text to
+    lowercase, and eliminating unnecessary whitespace.
 
     Parameters
     ----------
     text : str, list, tuple or numpy array
         The input text to be normalized.
-    
+
     Raises
     ------
     TypeError
         If the input is not a valid data type such as (int, float, bool, range, dict,
         bytes, bytearray, complex) or if the input contains nested data (e.g., a list of
         lists), the function raises a TypeError.
 
     Returns
     -------
     str or list
-        If the input is a string, the function returns the normalized string. If the 
-        input is a list, tuple, or numpy array of strings, it returns a list of 
+        If the input is a string, the function returns the normalized string. If the
+        input is a list, tuple, or numpy array of strings, it returns a list of
         normalized strings.
-    
+
     Examples
     --------
     >>> reference = normalize(" it's Consumed Domestically  And exported to other countries.")
     >>> print(reference)
     its consumed domestically and exported to other countries
     >>> reference
     'its consumed domestically and exported to other countries'
@@ -64,19 +64,21 @@
 
     normalized_text = []
     translate_table = [0 if c in string.punctuation.encode() else c for c in range(256)]
     translate_bytes = bytes(translate_table)
 
     for sentence in text:
         if not isinstance(sentence, str):
-            raise TypeError("Input must be String, List, Tuple, or NumPy Array. "
-                            "All data types should be flat, have a depth of 1 and "
-                            "contain no nested elements.")        
+            raise TypeError(
+                "Input must be String, List, Tuple, or NumPy Array. "
+                "All data types should be flat, have a depth of 1 and "
+                "contain no nested elements."
+            )
         cleaned_sentence = sentence.encode().translate(translate_bytes).decode().lower()
-        cleaned_sentence = cleaned_sentence.rstrip('\x00').replace('\x00', '')
-        cleaned_sentence = ' '.join(cleaned_sentence.split())
+        cleaned_sentence = cleaned_sentence.rstrip("\x00").replace("\x00", "")
+        cleaned_sentence = " ".join(cleaned_sentence.split())
         normalized_text.append(cleaned_sentence)
 
     if is_string_flag:
         return normalized_text[0]
 
     return normalized_text
```

### Comparing `werpy-2.1.1/werpy/summary.py` & `werpy-2.1.2/werpy/summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 from .errorhandler import error_handler
 
 
 def summary(reference, hypothesis):
     """
-    This function provides a comprehensive breakdown of the calculated results including the WER, Levenshtein 
+    This function provides a comprehensive breakdown of the calculated results including the WER, Levenshtein
     Distance and all the insertion, deletion and substitution errors.
 
     Parameters
     ----------
     reference : str, list or numpy array
         The ground truth transcription of a recorded speech or the expected output of a live speech.
     hypothesis : str, list or numpy array
@@ -50,11 +50,20 @@
     except (ValueError, AttributeError) as err:
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
         word_error_rate_breakdown = word_error_rate_breakdown.tolist()
     else:
         word_error_rate_breakdown = [word_error_rate_breakdown.tolist()]
-    columns = ['wer', 'ld', 'm', 'insertions', 'deletions', 'substitutions', 'inserted_words', 'deleted_words',
-                   'substituted_words']    
+    columns = [
+        "wer",
+        "ld",
+        "m",
+        "insertions",
+        "deletions",
+        "substitutions",
+        "inserted_words",
+        "deleted_words",
+        "substituted_words",
+    ]
     df = pd.DataFrame(word_error_rate_breakdown, columns=columns)
     return df
```

### Comparing `werpy-2.1.1/werpy/summaryp.py` & `werpy-2.1.2/werpy/summaryp.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 """
 
 import numpy as np
 import pandas as pd
 from .errorhandler import error_handler
 
 
-def summaryp(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
+def summaryp(
+    reference,
+    hypothesis,
+    insertions_weight=1,
+    deletions_weight=1,
+    substitutions_weight=1,
+):
     """
     This function provides a comprehensive breakdown of the calculated results including the WER, weighted
     WER, Levenshtein Distance and all the insertion, deletion and substitution errors.
 
     Parameters
     ----------
     reference : str, list or numpy array
@@ -59,27 +65,54 @@
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
         word_error_rate_breakdown = word_error_rate_breakdown.tolist()
         transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown)
         weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
         weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
-        weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
+        weighted_substitutions = (
+            transform_word_error_rate_breakdown[5] * substitutions_weight
+        )
         m = transform_word_error_rate_breakdown[2]
-        weighted_errors = sum((weighted_insertions, weighted_deletions, weighted_substitutions))
+        weighted_errors = sum(
+            (weighted_insertions, weighted_deletions, weighted_substitutions)
+        )
         werps_result = (weighted_errors / m).tolist()
     else:
         word_error_rate_breakdown = [word_error_rate_breakdown.tolist()]
         weighted_insertions = word_error_rate_breakdown[0][3] * insertions_weight
         weighted_deletions = word_error_rate_breakdown[0][4] * deletions_weight
         weighted_substitutions = word_error_rate_breakdown[0][5] * substitutions_weight
         m = word_error_rate_breakdown[0][2]
-        weighted_errors = sum((weighted_insertions, weighted_deletions, weighted_substitutions))
+        weighted_errors = sum(
+            (weighted_insertions, weighted_deletions, weighted_substitutions)
+        )
         werps_result = weighted_errors / m
 
-    columns = ['wer', 'ld', 'm', 'insertions', 'deletions', 'substitutions', 'inserted_words', 'deleted_words',
-                   'substituted_words']    
+    columns = [
+        "wer",
+        "ld",
+        "m",
+        "insertions",
+        "deletions",
+        "substitutions",
+        "inserted_words",
+        "deleted_words",
+        "substituted_words",
+    ]
     df = pd.DataFrame(word_error_rate_breakdown, columns=columns)
-    df['werp'] = werps_result
-    df = df[['wer', 'werp', 'ld', 'm', 'insertions', 'deletions', 'substitutions', 'inserted_words'
-             , 'deleted_words', 'substituted_words']]
+    df["werp"] = werps_result
+    df = df[
+        [
+            "wer",
+            "werp",
+            "ld",
+            "m",
+            "insertions",
+            "deletions",
+            "substitutions",
+            "inserted_words",
+            "deleted_words",
+            "substituted_words",
+        ]
+    ]
     return df
```

### Comparing `werpy-2.1.1/werpy/wer.py` & `werpy-2.1.2/werpy/wer.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,13 +49,16 @@
     """
     try:
         word_error_rate_breakdown = error_handler(reference, hypothesis)
     except (ValueError, AttributeError) as err:
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
-        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
-        wer_result = (np.sum(transform_word_error_rate_breakdown[1])) / (np.sum(transform_word_error_rate_breakdown[
-                                                                                     2]))
+        transform_word_error_rate_breakdown = np.transpose(
+            word_error_rate_breakdown.tolist()
+        )
+        wer_result = (np.sum(transform_word_error_rate_breakdown[1])) / (
+            np.sum(transform_word_error_rate_breakdown[2])
+        )
     else:
         wer_result = word_error_rate_breakdown[0]
     return wer_result
```

### Comparing `werpy-2.1.1/werpy/werp.py` & `werpy-2.1.2/werpy/werp.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,21 @@
     - werp(reference, hypothesis)
 """
 
 import numpy as np
 from .errorhandler import error_handler
 
 
-def werp(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
+def werp(
+    reference,
+    hypothesis,
+    insertions_weight=1,
+    deletions_weight=1,
+    substitutions_weight=1,
+):
     """
     This function calculates a weighted Word Error Rate for the entire reference and hypothesis texts. It allows the
     insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
     Parameters
     ----------
     reference : str, list or numpy array
@@ -63,20 +69,26 @@
     """
     try:
         word_error_rate_breakdown = error_handler(reference, hypothesis)
     except (ValueError, AttributeError) as err:
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
-        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        transform_word_error_rate_breakdown = np.transpose(
+            word_error_rate_breakdown.tolist()
+        )
         weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
         weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
-        weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
+        weighted_substitutions = (
+            transform_word_error_rate_breakdown[5] * substitutions_weight
+        )
         m = np.sum(transform_word_error_rate_breakdown[2])
     else:
         weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
         weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
         weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
         m = np.sum(word_error_rate_breakdown[2])
-    weighted_errors = np.sum([weighted_insertions, weighted_deletions, weighted_substitutions])
+    weighted_errors = np.sum(
+        [weighted_insertions, weighted_deletions, weighted_substitutions]
+    )
     werp_result = weighted_errors / m
     return werp_result
```

### Comparing `werpy-2.1.1/werpy/werps.py` & `werpy-2.1.2/werpy/werps.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,21 @@
     - werps(reference, hypothesis)
 """
 
 import numpy as np
 from .errorhandler import error_handler
 
 
-def werps(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
+def werps(
+    reference,
+    hypothesis,
+    insertions_weight=1,
+    deletions_weight=1,
+    substitutions_weight=1,
+):
     """
     This function calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. It
     allows the insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
     Parameters
     ----------
     reference : str, list or numpy array
@@ -57,25 +63,31 @@
     """
     try:
         word_error_rate_breakdown = error_handler(reference, hypothesis)
     except (ValueError, AttributeError) as err:
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
-        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        transform_word_error_rate_breakdown = np.transpose(
+            word_error_rate_breakdown.tolist()
+        )
         weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
         weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
-        weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
+        weighted_substitutions = (
+            transform_word_error_rate_breakdown[5] * substitutions_weight
+        )
         m = transform_word_error_rate_breakdown[2]
     else:
         weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
         weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
         weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
         m = word_error_rate_breakdown[2]
 
-    weighted_errors = sum((weighted_insertions, weighted_deletions, weighted_substitutions))
+    weighted_errors = sum(
+        (weighted_insertions, weighted_deletions, weighted_substitutions)
+    )
     werps_result = weighted_errors / m
 
     if isinstance(word_error_rate_breakdown[0], float):
         return werps_result
 
     return werps_result.tolist()
```

### Comparing `werpy-2.1.1/werpy/wers.py` & `werpy-2.1.2/werpy/wers.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,12 +44,14 @@
     """
     try:
         word_error_rate_breakdown = error_handler(reference, hypothesis)
     except (ValueError, AttributeError) as err:
         print(f"{type(err).__name__}: {str(err)}")
         return None
     if isinstance(word_error_rate_breakdown[0], np.ndarray):
-        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        transform_word_error_rate_breakdown = np.transpose(
+            word_error_rate_breakdown.tolist()
+        )
         wers_result = transform_word_error_rate_breakdown[0].tolist()
     else:
         wers_result = word_error_rate_breakdown[0]
     return wers_result
```

### Comparing `werpy-2.1.1/PKG-INFO` & `werpy-2.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: werpy
-Version: 2.1.1
+Version: 2.1.2
 Summary: A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER).
 Keywords: wer word error rate python python package stt speech-to-text levenshtein distance nlp metrics
 Author-Email: Ross Armstrong <ross.armstrong@analyticsinmotion.com>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Analytics in Motion
+        Copyright (c) 2023-2024, Analytics in Motion
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -49,47 +49,49 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Project-URL: Homepage, https://github.com/analyticsinmotion/werpy
 Project-URL: Repository, https://github.com/analyticsinmotion/werpy
+Project-URL: Documentation, https://werpy.readthedocs.io/
 Project-URL: Bug tracker, https://github.com/analyticsinmotion/werpy/issues
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.21.6; python_version < "3.11"
 Requires-Dist: numpy>=1.23.2; python_version >= "3.11"
 Requires-Dist: pandas>=1.3.0
+Requires-Dist: sphinx==7.2.6; extra == "docs"
+Requires-Dist: sphinx-nefertiti==0.3.2; extra == "docs"
+Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
 
-<h1 align="left">werpy - Word Error Rate for Python
+<h1 align="center">Word Error Rate for Python
 <a href="https://twitter.com/intent/tweet?text=Introducing%20%23werpy%20-%20the%20Python%20package%20for%20fast%20and%20accurate%20Word%20Error%20Rate%20(WER)%20calculation.%20Analyze%20text%20accuracy%2C%20enhance%20%23NLP%20models%2C%20and%20improve%20%23SpeechRecognition%20systems.%20Try%20it%20now%3A%20&url=https://github.com/analyticsinmotion/werpy&via=analyticsmotion&hashtags=PythonPackage,WordErrorRate,WER,NLP">
     <img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social" alt="Tweet">
   </a>
 </h1>
 
 <!-- badges: start -->
 
 | | |
 | --- | --- |
-| Meta | [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp; [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp; ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp; [![Analytics in Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-rounded.svg)](https://www.analyticsinmotion.com) |
-| Testing | [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp; [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp; [![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp; [![Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml)&nbsp;&nbsp; <!--[![CircleCI](https://dl.circleci.com/status-badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)&nbsp;&nbsp;--> |
-| Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![PyPI Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/werpy)&nbsp;&nbsp; [![sourcerank](https://img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/werpy)&nbsp;&nbsp; |
-
+| Meta | [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11%7C3.12-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp; [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;<!-- ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;--> [![Black Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)&nbsp;&nbsp; [![Analytics in Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-rounded.svg)](https://www.analyticsinmotion.com) |
+| Testing | [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp; [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp; [![CodeFactor](https://www.codefactor.io/repository/github/analyticsinmotion/werpy/badge)](https://www.codefactor.io/repository/github/analyticsinmotion/werpy)&nbsp;&nbsp; <!--[![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp;--> <!--[![Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/bandit.yml)&nbsp;&nbsp;--> [![CircleCI](https://dl.circleci.com/status-badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)&nbsp;&nbsp; [![codecov](https://codecov.io/gh/analyticsinmotion/werpy/graph/badge.svg?token=GGT823AVM8)](https://codecov.io/gh/analyticsinmotion/werpy) |
+| Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![PyPI Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)&nbsp;&nbsp; [![Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/werpy)&nbsp;&nbsp;<!--[![sourcerank](https://img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/werpy)&nbsp;&nbsp;--> [![Documentation Status](https://readthedocs.org/projects/werpy/badge/?version=latest)](https://werpy.readthedocs.io/en/latest/?badge=latest)&nbsp;&nbsp; |
 
 
 <!-- badges: end -->
 
 ## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
-It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
+It has been designed with the flexibility to handle multiple input data types such as strings, lists and NumPy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
 Additionally, the summary function provides a comprehensive breakdown of the calculated results to assist in analyzing the specific errors quickly and in more detail.
 <br />
 
 ## Functions available in werpy
 The following table provides an overview of the functions that can be used in werpy.
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: werpy Version: 2.1.1 Summary: A powerful yet
+Metadata-Version: 2.1 Name: werpy Version: 2.1.2 Summary: A powerful yet
 lightweight Python package to calculate and analyze the Word Error Rate (WER).
 Keywords: wer word error rate python python package stt speech-to-text
 levenshtein distance nlp metrics Author-Email: Ross Armstrong
-analyticsinmotion.com> License: BSD 3-Clause License Copyright (c) 2023,
+analyticsinmotion.com> License: BSD 3-Clause License Copyright (c) 2023-2024,
 Analytics in Motion Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
 and the following disclaimer in the documentation and/or other materials
 provided with the distribution. 3. Neither the name of the copyright holder nor
@@ -32,50 +32,54 @@
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
-Mathematics Project-URL: Homepage, https://github.com/analyticsinmotion/werpy
-Project-URL: Repository, https://github.com/analyticsinmotion/werpy Project-
-URL: Bug tracker, https://github.com/analyticsinmotion/werpy/issues Requires-
-Python: >=3.8 Requires-Dist: numpy>=1.21.6; python_version < "3.11" Requires-
-Dist: numpy>=1.23.2; python_version >= "3.11" Requires-Dist: pandas>=1.3.0
-Description-Content-Type: text/markdown ![werpy-logo-word-error-rate](https://
-user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-
-c2b5ef6f80e9.png)
-************ wweerrppyy -- WWoorrdd EErrrroorr RRaattee ffoorr PPyytthhoonn_[[_TT_ww_ee_ee_tt_]] ************
+Mathematics Project-URL: Repository, https://github.com/analyticsinmotion/werpy
+Project-URL: Documentation, https://werpy.readthedocs.io/ Project-URL: Bug
+tracker, https://github.com/analyticsinmotion/werpy/issues Requires-Python:
+>=3.8 Requires-Dist: numpy>=1.21.6; python_version < "3.11" Requires-Dist:
+numpy>=1.23.2; python_version >= "3.11" Requires-Dist: pandas>=1.3.0 Requires-
+Dist: sphinx==7.2.6; extra == "docs" Requires-Dist: sphinx-nefertiti==0.3.2;
+extra == "docs" Provides-Extra: docs Description-Content-Type: text/markdown !
+[werpy-logo-word-error-rate](https://user-images.githubusercontent.com/
+52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
+                ************ WWoorrdd EErrrroorr RRaattee ffoorr PPyytthhoonn_[[_TT_ww_ee_ee_tt_]] ************
 | | | | --- | --- | | Meta | [![Python Version](https://img.shields.io/badge/
-python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://
-www.python.org/downloads/)   [![werpy License](https://img.shields.io/badge/
-License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/
-blob/main/LICENSE)   ![Maintained](https://img.shields.io/badge/Maintained%3F-
-yes-green.svg)   [![Analytics in Motion](https://raw.githubusercontent.com/
-analyticsinmotion/.github/main/assets/images/analytics-in-motion-github-badge-
-rounded.svg)](https://www.analyticsinmotion.com) | | Testing | [![CodeQL]
-(https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/
-badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/
-codeql.yml)   [![Codacy Security Scan](https://github.com/analyticsinmotion/
-werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/
-analyticsinmotion/werpy/actions/workflows/codacy.yml)   [![Pylint](https://
-github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)]
-(https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)   [!
-[Bandit](https://github.com/analyticsinmotion/werpy/actions/workflows/
-bandit.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/
-workflows/bandit.yml)   | | Package | [![Pypi](https://img.shields.io/pypi/v/
-werpy?label=PyPI&color=blue)](https://pypi.org/project/werpy/)   [![PyPI
-Downloads](https://img.shields.io/pypi/dm/werpy?label=PyPI%20downloads)](https:
-//pypi.org/project/werpy/)   [![Downloads](https://static.pepy.tech/badge/
-werpy)](https://pepy.tech/project/werpy)   [![sourcerank](https://
-img.shields.io/librariesio/sourcerank/pypi/werpy)](https://libraries.io/pypi/
-werpy)   | ## What is werpy? **werpy** is a powerful yet lightweight Python
-package that rapidly calculates and analyzes the Word Error Rate (WER) between
-two sets of text. It has been designed with the flexibility to handle multiple
-input data types such as strings, lists and numpy arrays.
+python-3.8%7C3.9%7C3.10%7C3.11%7C3.12-blue?logo=python&logoColor=ffdd54)]
+(https://www.python.org/downloads/)   [![werpy License](https://img.shields.io/
+badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/
+werpy/blob/main/LICENSE)   [![Black Code Style](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black)   [![Analytics in
+Motion](https://raw.githubusercontent.com/analyticsinmotion/.github/main/
+assets/images/analytics-in-motion-github-badge-rounded.svg)](https://
+www.analyticsinmotion.com) | | Testing | [![CodeQL](https://github.com/
+analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://
+github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)   [![Codacy
+Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/
+codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/
+workflows/codacy.yml)   [![CodeFactor](https://www.codefactor.io/repository/
+github/analyticsinmotion/werpy/badge)](https://www.codefactor.io/repository/
+github/analyticsinmotion/werpy)   [![CircleCI](https://dl.circleci.com/status-
+badge/img/gh/analyticsinmotion/werpy/tree/main.svg?style=svg)](https://
+dl.circleci.com/status-badge/redirect/gh/analyticsinmotion/werpy/tree/main)  
+[![codecov](https://codecov.io/gh/analyticsinmotion/werpy/graph/
+badge.svg?token=GGT823AVM8)](https://codecov.io/gh/analyticsinmotion/werpy) | |
+Package | [![Pypi](https://img.shields.io/pypi/v/werpy?label=PyPI&color=blue)]
+(https://pypi.org/project/werpy/)   [![PyPI Downloads](https://img.shields.io/
+pypi/dm/werpy?label=PyPI%20downloads)](https://pypi.org/project/werpy/)   [!
+[Downloads](https://static.pepy.tech/badge/werpy)](https://pepy.tech/project/
+werpy)   [![Documentation Status](https://readthedocs.org/projects/werpy/badge/
+?version=latest)](https://werpy.readthedocs.io/en/latest/?badge=latest)   | ##
+What is werpy? **werpy** is a powerful yet lightweight Python package that
+rapidly calculates and analyzes the Word Error Rate (WER) between two sets of
+text. It has been designed with the flexibility to handle multiple input data
+types such as strings, lists and NumPy arrays.
 The package also includes a full set of features such as normalizing the input
 text to account for data collection variability and the capability to easily
 assign different weights/penalties to specific error classifications
 (insertions, deletions, and substitutions). Additionally, the summary function
 provides a comprehensive breakdown of the calculated results to assist in
 analyzing the specific errors quickly and in more detail.
 ## Functions available in werpy The following table provides an overview of the
```

