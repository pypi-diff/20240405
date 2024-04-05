# Comparing `tmp/rimsschemedrawer-3.0.0.dev3.tar.gz` & `tmp/rimsschemedrawer-3.0.0.dev4.tar.gz`

## Comparing `rimsschemedrawer-3.0.0.dev3.tar` & `rimsschemedrawer-3.0.0.dev4.tar`

### file list

```diff
@@ -1,41 +1,58 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/INSTALLATION.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/requirements-dev.lock
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/requirements.lock
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.github/workflows/check_mode.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.github/workflows/package_testing.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/examples/example_titanium.json
--rw-r--r--   0        0        0    92421 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/examples/screenshot_titanium.png
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/scripts/ip_nist.json
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/scripts/ip_nist_reader.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/app.py
--rw-r--r--   0        0        0    43120 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/gui.py
--rw-r--r--   0        0        0    17732 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/json_parser.py
--rw-r--r--   0        0        0    16406 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/plotter.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/conftest.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/test_json_parser.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/test_plotter.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/test_scheme_table.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_cm.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_low_lying_cm.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_low_lying_nm.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_nm.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/ti.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/ti_new.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/ti_new_mixed_units.json
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/ti_old_style.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/w_cm-1.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/tests/data/w_nm.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/LICENSE
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/README.md
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/mkdocs.yml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/requirements-dev.lock
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/requirements.lock
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.github/workflows/check_mode.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.github/workflows/package_testing.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/dev.md
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/gui.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/index.md
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/install.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/api/gui.md
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/api/index.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/api/json_parser.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/api/plotter.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/api/utils.md
+-rw-r--r--   0        0        0   109919 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/gui_overview.png
+-rw-r--r--   0        0        0   147601 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/gui_overview.svg
+-rw-r--r--   0        0        0    66126 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/gui_scheme.png
+-rw-r--r--   0        0        0   144450 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/gui_scheme.svg
+-rw-r--r--   0        0        0   105965 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/gui_ti_scheme.png
+-rw-r--r--   0        0        0    49582 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/plot_window.png
+-rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/docs/img/plot_window_dark.png
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/examples/example_titanium.json
+-rw-r--r--   0        0        0    92421 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/examples/screenshot_titanium.png
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/scripts/ip_nist.json
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/scripts/ip_nist_reader.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/app.py
+-rw-r--r--   0        0        0    41640 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/gui.py
+-rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/json_parser.py
+-rw-r--r--   0        0        0    16632 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/plotter.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/conftest.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/test_json_parser.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/test_plotter.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/test_scheme_table.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_cm.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_low_lying_cm.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_low_lying_nm.json
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_nm.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/ti.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/ti_new.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/ti_new_mixed_units.json
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/ti_old_style.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/w_cm-1.json
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/tests/data/w_nm.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/LICENSE
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/README.md
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 rimsschemedrawer-3.0.0.dev4/PKG-INFO
```

### Comparing `rimsschemedrawer-3.0.0.dev3/.github/ISSUE_TEMPLATE/bug_report.md` & `rimsschemedrawer-3.0.0.dev4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/.github/ISSUE_TEMPLATE/feature_request.md` & `rimsschemedrawer-3.0.0.dev4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/.github/workflows/package_testing.yml` & `rimsschemedrawer-3.0.0.dev4/.github/workflows/package_testing.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
-
 name: tests
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
@@ -19,15 +16,15 @@
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - name: Checkout repo
       uses: actions/checkout@v4
     - name: Install the latest version of rye
-      uses: eifinger/setup-rye@v1
+      uses: eifinger/setup-rye@v2
     - name: Sync Rye
       run: |
         rye pin ${{ matrix.python-version }}
         rye sync
     - name: Run Tests for python interface
       run: rye run test
     - name: Run Lint on one python
```

### Comparing `rimsschemedrawer-3.0.0.dev3/.github/workflows/release.yml` & `rimsschemedrawer-3.0.0.dev4/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   build-linux:
     name: Release on PyPi
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
       - name: Install the latest version of rye
-        uses: eifinger/setup-rye@v1
+        uses: eifinger/setup-rye@v2
       - name: Sync Rye
         run: |
           rye pin ${{ env.PYTHON_VERSION }}
           rye sync
       - name: Build and release the controller
         run: |
           rye build
```

### Comparing `rimsschemedrawer-3.0.0.dev3/examples/example_titanium.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/ti_old_style.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'scheme'": "{'ip_level': '55070'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "scheme": {
         "gs_level": "0",
         "gs_term": "3F2",
-        "ip_level": "55074",
+        "ip_level": "55070",
         "ip_term": "",
         "step_level0": "170.15",
         "step_level1": "386.88",
         "step_level2": "21469.5",
         "step_level3": "45498.85",
         "step_level4": "56844.45",
         "step_lowlying0": true,
```

### Comparing `rimsschemedrawer-3.0.0.dev3/examples/screenshot_titanium.png` & `rimsschemedrawer-3.0.0.dev4/examples/screenshot_titanium.png`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/scripts/ip_nist.json` & `rimsschemedrawer-3.0.0.dev4/scripts/ip_nist.json`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/scripts/ip_nist_reader.py` & `rimsschemedrawer-3.0.0.dev4/scripts/ip_nist_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     - Fl
     - Mc
     - Lv
     - Ts
     - Og
 """
 
-
 import json
 
 import requests
 
 
 def get_url(ele: str) -> str:
     """Get URL for csv file from NIST.
```

### Comparing `rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/gui.py` & `rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,39 +70,40 @@
         self.edt_ipterm = QtWidgets.QLineEdit()
         self.cmb_element = None
         self.cmb_lasers = None
         self.chk_lowlying = []
         self.chk_forbidden = []
 
         # settings line edits
+        self.edt_sett_plttitle = QtWidgets.QLineEdit()
         self.edt_sett_figwidth = QtWidgets.QLineEdit()
         self.edt_sett_figheight = QtWidgets.QLineEdit()
         self.edt_sett_fstitle = QtWidgets.QLineEdit()
         self.edt_sett_fsaxes = QtWidgets.QLineEdit()
         self.edt_sett_fsaxlbl = QtWidgets.QLineEdit()
         self.chk_sett_trans_strength = QtWidgets.QCheckBox("Transition strengths?")
         self.chk_sett_linebreaks = QtWidgets.QCheckBox("Line breaks?")
         self.chk_sett_showcmax = QtWidgets.QCheckBox()  # no label -> label in layout
         self.chk_sett_showcmax.setChecked(True)
         self.chk_sett_showevax = QtWidgets.QCheckBox("Show eV axis labels?")
         self.chk_sett_showevax.setChecked(True)
-        self.chk_plot_darkmode = QtWidgets.QCheckBox("Plot dark mode?")
+        self.drop_plot_style = QtWidgets.QComboBox()
+        self.drop_plot_style.addItems(ut.PLOT_STYLES)
         self.edt_sett_fslbl = QtWidgets.QLineEdit()
         self.edt_sett_headspace = QtWidgets.QLineEdit()
         self.edt_sett_arrwidth = QtWidgets.QLineEdit()
         self.edt_sett_arrheadwidth = QtWidgets.QLineEdit()
         self.edt_sett_preclambda = QtWidgets.QLineEdit()
         self.edt_sett_preclevel = QtWidgets.QLineEdit()
         self.rbtngrp_iplabel = QtWidgets.QButtonGroup()
         self.rbtn_iplable_top = QtWidgets.QRadioButton("Top")
         self.rbtn_iplable_bottom = QtWidgets.QRadioButton("Bott.")
         self.rbtngrp_sett_forbidden = QtWidgets.QButtonGroup()
         self.rbtn_sett_xoutarrow = QtWidgets.QRadioButton("x-out")
         self.rbtn_sett_nodisparrow = QtWidgets.QRadioButton("Don't show")
-        self.edt_sett_plttitle = QtWidgets.QLineEdit()
 
         # push buttons
         self.btn_plot = QtWidgets.QPushButton("Plot")
         self.btn_test = QtWidgets.QPushButton("Test")
         self.btn_load_conf = QtWidgets.QPushButton("Load Config")
         self.btn_save_conf = QtWidgets.QPushButton("Save Config")
         self.btn_reset_formatting = QtWidgets.QPushButton("Reset Formatting")
@@ -127,15 +128,15 @@
         self.show()
 
     def init_ui(self):
         """
         Initialize the UI
         """
         # bottom most row:
-        bottomrowindex = 12  # depends on how many settings entries there are!
+        bottomrowindex = 13  # depends on how many settings entries there are!
         if self.numberofsteps + 2 > bottomrowindex:
             bottomrowindex = self.numberofsteps + 2
 
         # define the grid layout
         layout = QtWidgets.QGridLayout()  # columns
 
         # ### column 1: labels for states
@@ -178,18 +179,14 @@
         lbl_forbidden = QtWidgets.QLabel("Forbidden?")
         lbl_forbidden.setFont(self.fontheader)
         layout.addWidget(lbl_forbidden, 0, 5, 1, 1)
         # Settings
         lbl_sett = QtWidgets.QLabel("Settings")
         lbl_sett.setFont(self.fontheader)
         layout.addWidget(lbl_sett, 0, 6, 1, 1)
-        # plot title
-        lbl_plttit = QtWidgets.QLabel("Plot Title")
-        lbl_plttit.setFont(self.fontheader)
-        layout.addWidget(lbl_plttit, 0, 8, 1, 1)
 
         # ground state
         lbl_gs = QtWidgets.QLabel("Ground state (cm<sup>-1</sup>)")
         layout.addWidget(lbl_gs, 1, 0, 1, 1)
         layout.addWidget(self.edt_gslevel, 1, 1, 1, 1)
         layout.addWidget(self.edt_gsterm, 1, 2, 1, 1)
         self.edt_gslevel.setToolTip("Set the ground state level in cm<sup>-1</sup>.")
@@ -309,150 +306,154 @@
         self.rbtngrp_iplabel.addButton(self.rbtn_iplable_bottom)
 
         # button group for how to display forbidden transitions
         self.rbtngrp_sett_forbidden.addButton(self.rbtn_sett_xoutarrow)
         self.rbtngrp_sett_forbidden.addButton(self.rbtn_sett_nodisparrow)
 
         # labels for settings
-        layout.addWidget(QtWidgets.QLabel("Figure Width x Height:"), 1, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Font size title:"), 2, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Font size axes:"), 3, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Font size axes label:"), 4, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Font size labels:"), 5, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Headspace (cm<sup>-1</sup>):"), 6, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Arrow width:"), 7, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Arrow head width:"), 8, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Precision wavelength:"), 9, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("Precision level:"), 10, 6, 1, 1)
-        layout.addWidget(QtWidgets.QLabel("IP label position:"), 11, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Plot Title"), 1, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Figure Width x Height:"), 2, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Font size title:"), 3, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Font size axes:"), 4, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Font size axes label:"), 5, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Font size labels:"), 6, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Headspace (cm<sup>-1</sup>):"), 7, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Arrow width:"), 8, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Arrow head width:"), 9, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Precision wavelength:"), 10, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("Precision level:"), 11, 6, 1, 1)
+        layout.addWidget(QtWidgets.QLabel("IP label position:"), 12, 6, 1, 1)
         layout.addWidget(
-            QtWidgets.QLabel("Display forbidden transitions:"), 12, 6, 1, 1
+            QtWidgets.QLabel("Display forbidden transitions:"), 13, 6, 1, 1
         )
         # line edits and buttons, include tooltips
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.edt_sett_figwidth)
+        layout.addWidget(self.edt_sett_plttitle, 1, 7, 1, 1)
+        self.edt_sett_plttitle.setToolTip("Title of the plot.")
         self.edt_sett_figwidth.setToolTip("Width of figure in inches.")
         tmplayout.addStretch()
         tmplayout.addWidget(QtWidgets.QLabel("x"))
         tmplayout.addStretch()
         tmplayout.addWidget(self.edt_sett_figheight)
         self.edt_sett_figheight.setToolTip("Height of figure in inches.")
-        layout.addLayout(tmplayout, 1, 7, 1, 1)
-        layout.addWidget(self.edt_sett_fstitle, 2, 7, 1, 1)
+        layout.addLayout(tmplayout, 2, 7, 1, 1)
+        layout.addWidget(self.edt_sett_fstitle, 3, 7, 1, 1)
         self.edt_sett_fstitle.setToolTip("Font size of the plot title.")
-        layout.addWidget(self.edt_sett_fsaxes, 3, 7, 1, 1)
+        layout.addWidget(self.edt_sett_fsaxes, 4, 7, 1, 1)
         self.edt_sett_fsaxes.setToolTip("Font size of axes ticks.")
-        layout.addWidget(self.edt_sett_fsaxlbl, 4, 7, 1, 1)
+        layout.addWidget(self.edt_sett_fsaxlbl, 5, 7, 1, 1)
         self.edt_sett_fsaxlbl.setToolTip("Font size of axes labels.")
         # transition_strengths
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.chk_sett_trans_strength)
         tmplayout.addStretch()
-        layout.addLayout(tmplayout, 3, 8, 1, 1)
+        layout.addLayout(tmplayout, 1, 8, 1, 1)
         self.chk_sett_trans_strength.setToolTip("Display the transition strength?")
         # line breaks
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.chk_sett_linebreaks)
         tmplayout.addStretch()
-        layout.addLayout(tmplayout, 4, 8, 1, 1)
+        layout.addLayout(tmplayout, 2, 8, 1, 1)
         self.chk_sett_linebreaks.setToolTip(
             "Should there be a line break between\n"
             "the state and the term symbol? Play\n"
             "with this to make the the plot look nicer."
         )
-        layout.addWidget(self.edt_sett_fslbl, 5, 7, 1, 1)
+        layout.addWidget(self.edt_sett_fslbl, 6, 7, 1, 1)
         # check box show cm-1 axis
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.chk_sett_showcmax)
         tmplayout.addStretch()
         tmplabel = QtWidgets.QLabel("Show cm-1 axis labels?")
         tmplayout.addWidget(tmplabel)
-        layout.addLayout(tmplayout, 5, 8, 1, 1)
+        layout.addLayout(tmplayout, 3, 8, 1, 1)
         self.chk_sett_showcmax.setToolTip(
             "Show the cm<sup>-1</sup> (left) axis? You can turn this off in case you "
             "want to stich plots together afterwards! This function will also hide the "
             "ticks."
         )
         tmplabel.setToolTip(
             "Show the cm<sup>-1</sup> (left) axis? You can turn this off in case you "
             "want to stich plots together afterwards! This function will also hide the "
             "ticks."
         )
         self.edt_sett_fslbl.setToolTip("Font size of the labels.")
-        layout.addWidget(self.edt_sett_headspace, 6, 7, 1, 1)
+        layout.addWidget(self.edt_sett_headspace, 7, 7, 1, 1)
         # check box show eV axis
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.chk_sett_showevax)
         tmplayout.addStretch()
-        layout.addLayout(tmplayout, 6, 8, 1, 1)
+        layout.addLayout(tmplayout, 4, 8, 1, 1)
         self.chk_sett_showevax.setToolTip(
             "Show the eV (right) axis? You can turn this\n"
             " off in case you want to stich plots together\n"
             "afterwards! This function will also hide the\n"
             "ticks."
         )
         self.edt_sett_headspace.setToolTip(
             "Set how much space is added on top of the "
-            "IP level: the head space. Adjust this "
+            "highest transition: the head space. Adjust this "
             "value whenever there is not enough space "
             "on top to fit all the text in. The value "
             "is given in cm<sup>-1</sup>."
         )
-        layout.addWidget(self.edt_sett_arrwidth, 7, 7, 1, 1)
+        layout.addWidget(self.edt_sett_arrwidth, 8, 7, 1, 1)
         self.edt_sett_arrwidth.setToolTip(
             "Set the width of the arrow line in\n"
             "undefine dunits. Play to get the ideal\n"
             "settings."
         )
-        layout.addWidget(self.edt_sett_arrheadwidth, 8, 7, 1, 1)
+        layout.addWidget(self.edt_sett_arrheadwidth, 9, 7, 1, 1)
         self.edt_sett_arrheadwidth.setToolTip(
             "Set the width of the arrwo head in\n"
             "undefined units. Play to get the ideal\n"
             "settings."
         )
-        layout.addWidget(self.edt_sett_preclambda, 9, 7, 1, 1)
+        layout.addWidget(self.edt_sett_preclambda, 10, 7, 1, 1)
         self.edt_sett_preclambda.setToolTip(
             "Set the precision with which the wavelength\n" "is displayed on the plot."
         )
-        layout.addWidget(self.edt_sett_preclevel, 10, 7, 1, 1)
+        layout.addWidget(self.edt_sett_preclevel, 11, 7, 1, 1)
         self.edt_sett_preclevel.setToolTip(
             "Set the precision with which the wavenumber\n" "is displayed on the plot."
         )
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.rbtn_iplable_top)
         self.rbtn_iplable_top.setChecked(True)  # set top as default
         tmplayout.addStretch()
         tmplayout.addWidget(self.rbtn_iplable_bottom)
         self.rbtn_iplable_top.setToolTip("Display the IP label above the line.")
         self.rbtn_iplable_bottom.setToolTip("Display the IP label below the line.")
-        layout.addLayout(tmplayout, 11, 7, 1, 1)
+        layout.addLayout(tmplayout, 12, 7, 1, 1)
         tmplayout = QtWidgets.QHBoxLayout()
         tmplayout.addWidget(self.rbtn_sett_xoutarrow)
         self.rbtn_sett_xoutarrow.setChecked(True)  # set top as default
         tmplayout.addStretch()
         tmplayout.addWidget(self.rbtn_sett_nodisparrow)
         self.rbtn_sett_xoutarrow.setToolTip(
             "Show an arrow for forbidden transitions\n" "but cross it out."
         )
         self.rbtn_sett_nodisparrow.setToolTip(
             "Don't show arrows for forbidden\n" "transitions."
         )
-        layout.addLayout(tmplayout, 12, 7, 1, 1)
-        layout.addWidget(self.edt_sett_plttitle, 1, 8, 1, 1)
-        self.edt_sett_plttitle.setToolTip("Title of the plot.")
+        layout.addLayout(tmplayout, 13, 7, 1, 1)
 
         # plot dark mode?
-        tmplayout = QtWidgets.QHBoxLayout()
-        tmplayout.addWidget(self.chk_plot_darkmode)
-        tmplayout.addStretch()
-        layout.addLayout(tmplayout, 7, 8, 1, 1)
-        self.chk_plot_darkmode.setToolTip("Plot with dark background?")
+        plot_style_lbl = QtWidgets.QLabel("Plot Style")
+        layout.addWidget(plot_style_lbl, 5, 8, 1, 1)
+        layout.addWidget(self.drop_plot_style, 6, 8, 1, 1)
+        self.drop_plot_style.setToolTip(
+            "Select the plot style\n"
+            "- light: Light mode\n"
+            "- dark: Dark mode\n"
+            "- light transparent: Light mode with transparent background\n"
+            "- dark transparent: Dark mode with transparent background"
+        )
 
-        # set sizes
-        self.edt_sett_plttitle.setFixedSize(self.lineedit_size)
         # validators
         self.edt_sett_figwidth.setValidator(QtGui.QDoubleValidator())
         self.edt_sett_figheight.setValidator(QtGui.QDoubleValidator())
         self.edt_sett_fstitle.setValidator(QtGui.QIntValidator())
         self.edt_sett_fsaxes.setValidator(QtGui.QIntValidator())
         self.edt_sett_fsaxlbl.setValidator(QtGui.QIntValidator())
         self.edt_sett_fslbl.setValidator(QtGui.QIntValidator())
@@ -471,15 +472,15 @@
         self.edt_sett_headspace.setAlignment(QtCore.Qt.AlignRight)
         self.edt_sett_arrwidth.setAlignment(QtCore.Qt.AlignRight)
         self.edt_sett_arrheadwidth.setAlignment(QtCore.Qt.AlignRight)
         self.edt_sett_preclambda.setAlignment(QtCore.Qt.AlignRight)
         self.edt_sett_preclevel.setAlignment(QtCore.Qt.AlignRight)
 
         # push buttons
-        layout.addWidget(self.btn_plot, 2, 8, 1, 1)
+        layout.addWidget(self.btn_plot, 0, 8, 1, 1)
         if self.rundebug:
             layout.addWidget(self.btn_test, bottomrowindex, 3, 1, 1)
         layout.addWidget(self.btn_load_conf, bottomrowindex - 4, 8, 1, 1)
         layout.addWidget(self.btn_save_conf, bottomrowindex - 3, 8, 1, 1)
         layout.addWidget(self.btn_reset_formatting, bottomrowindex - 2, 8, 1, 1)
         layout.addWidget(self.btn_about, bottomrowindex - 1, 8, 1, 1)
         layout.addWidget(self.btn_quit, bottomrowindex, 8, 1, 1)
@@ -603,15 +604,19 @@
             )
 
             # set checkboxes
             set_checkbox(self.chk_sett_trans_strength, "show_transition_strength")
             set_checkbox(self.chk_sett_linebreaks, "line_breaks")
             set_checkbox(self.chk_sett_showcmax, "show_cm-1_axis")
             set_checkbox(self.chk_sett_showevax, "show_eV_axis")
-            set_checkbox(self.chk_plot_darkmode, "plot_darkmode")
+
+            # set plot style
+            self.drop_plot_style.setCurrentText(
+                ut.DEFAULT_SETTINGS["settings"]["plot_style"]
+            )
 
     def set_label_names(self):
         # get the unit
         unit = self.get_unit()
         # set the labels
         stepnumb = 0
         for it in range(self.numberofsteps):
@@ -643,19 +648,19 @@
             return "cm<sup>-1</sup>"
 
     def check_fields(self):
         """
         Check if the required fields are filled in.
         """
         # throw an error if not at least one box is filled
-        if self.edt_level[0].text() == "":
+        if self.edt_level[0].text() == "" or self.edt_gslevel.text() == "":
             QtWidgets.QMessageBox.warning(
                 self,
                 "No entries",
-                "Need at least one level to make a plot!",
+                "Need at least ground state and one level to make a plot!",
                 QtWidgets.QMessageBox.Ok,
             )
             return False
 
         # ip value
         try:
             _ = float(self.edt_iplevel.text())
@@ -670,26 +675,26 @@
         return True
 
     # buttons
     def plot(self):
         """
         Call the plotting window
         """
-        if self.rundebug:
-            print("Plotting...")
         if not self.check_fields():
             return
 
         # fill default values - if not already there
         self.fill_default_values()
 
         # open the plotting window
         data = self.write_json()
 
-        PlotDisplay(data, parent=self, darkmode=self.chk_plot_darkmode.isChecked())
+        darkmode = "dark" in self.drop_plot_style.currentText()
+        transparent = "transparent" in self.drop_plot_style.currentText()
+        PlotDisplay(data, parent=self, darkmode=darkmode, transparent=transparent)
 
     def load_config(self, **kwargs):
         """
         Load a configuration file that has previously been saved
 
         :param kwargs:  <dict>  Dictionary with additional keyword arguments
             - fname: <Path>  Path to the file to load
@@ -708,166 +713,118 @@
             # user pressed cancel
             if filename == "":
                 return
 
             filename = Path(filename)
 
         self.user_path = filename.parent
-        # load the json file
-        load_dict = rimsschemedrawer.json_parser.json_reader(filename)
-        config_parser = rimsschemedrawer.json_parser.ConfigParser(load_dict)
 
-        # function for setting line edits
-        def set_line_edits(category, entry, lineedit):
-            """
-            Sets a given line edit from the dictionary, but also checks if available.
-            :param category:    <string>    Category the entry is in
-            :param entry:       <string>    Entry with the value
-            :param lineedit:    <QtWidgets.QLineEdit> The object for the text
-            """
-            try:
-                lineedit.setText(load_dict[category][entry])
-            except KeyError:
-                pass
+        # load the json file
+        _load_dict = rimsschemedrawer.json_parser.json_reader(filename)
+        try:
+            config_parser = rimsschemedrawer.json_parser.ConfigParser(_load_dict)
+        except Exception as err:
+            QtWidgets.QMessageBox.warning(
+                self,
+                "Error",
+                f"An error occurred while reading the file.\n{'\n'.join(err.args)}",
+                QtWidgets.QMessageBox.Ok,
+            )
+            return
 
         # set the settings for the levels
-        try:
-            if load_dict["scheme"]["unit"] == "nm":
-                self.rbtn_nm.setChecked(True)
-            else:
-                self.rbtn_cm.setChecked(True)
-        except KeyError:
-            pass
+        if config_parser.sett_unit_nm:
+            self.rbtn_nm.setChecked(True)
+        else:
+            self.rbtn_cm.setChecked(True)
 
-        set_line_edits("scheme", "gs_level", self.edt_gslevel)
-        set_line_edits("scheme", "gs_term", self.edt_gsterm)
+        self.edt_gslevel.setText(str(config_parser.gs_level))
+        self.edt_gsterm.setText(config_parser.gs_term_no_formatting)
         for it in range(
             len(self.edt_level)
         ):  # only loop through as many entries as there are
-            set_line_edits("scheme", f"step_level{it}", self.edt_level[it])
-            set_line_edits("scheme", f"step_term{it}", self.edt_term[it])
-            set_line_edits(
-                "scheme", f"trans_strength{it}", self.edt_transition_strengths[it]
-            )
             try:
-                if load_dict["scheme"][f"step_lowlying{it}"]:
-                    self.chk_lowlying[it].setChecked(True)
+                if config_parser.sett_unit_nm:
+                    value_list = config_parser.step_nm
                 else:
-                    self.chk_lowlying[it].setChecked(False)
-            except KeyError:
+                    value_list = config_parser.step_levels
+                self.edt_level[it].setText(str(value_list[it]))
+                self.edt_term[it].setText(config_parser.step_terms_no_formatting[it])
+
+                trans_strength = config_parser.transition_strengths[it]
+                if trans_strength > 0:
+                    self.edt_transition_strengths[it].setText(str(trans_strength))
+                self.chk_lowlying[it].setChecked(config_parser.is_low_lying[it])
+                self.chk_forbidden[it].setChecked(config_parser.step_forbidden[it])
+            except IndexError:
+                self.edt_level[it].setText("")
+                self.edt_term[it].setText("")
+                self.edt_transition_strengths[it].setText("")
                 self.chk_lowlying[it].setChecked(False)
-            try:
-                if load_dict["scheme"][f"step_forbidden{it}"]:
-                    self.chk_forbidden[it].setChecked(True)
-                else:
-                    self.chk_forbidden[it].setChecked(False)
-            except KeyError:
                 self.chk_forbidden[it].setChecked(False)
 
         # IP level
         self.cmb_element.setCurrentText(config_parser.element)
         if config_parser.element_guessed:
             QtWidgets.QMessageBox.information(
                 self,
                 f"Element set to {config_parser.element}",
                 "You used an old-style configuration file. "
                 "The software automatically guessed the element from the given "
                 "ionization potential. "
                 "Please check if this is correct and adjust if necessary.",
             )
-        set_line_edits("scheme", "ip_term", self.edt_ipterm)
+        self.edt_ipterm.setText(config_parser.ip_term_no_formatting)
 
         # set the lasers used
         self.cmb_lasers.setCurrentText(config_parser.lasers)
 
-        # program settings - alphabetically
-        set_line_edits("settings", "arrow_head_width", self.edt_sett_arrheadwidth)
-        set_line_edits("settings", "arrow_width", self.edt_sett_arrwidth)
-        set_line_edits("settings", "fig_height", self.edt_sett_figheight)
-        set_line_edits("settings", "fig_width", self.edt_sett_figwidth)
-        set_line_edits("settings", "fs_axes", self.edt_sett_fsaxes)
-        set_line_edits("settings", "fs_axes_labels", self.edt_sett_fsaxlbl)
-        set_line_edits("settings", "fs_labels", self.edt_sett_fslbl)
-        set_line_edits("settings", "fs_title", self.edt_sett_fstitle)
-        set_line_edits("settings", "headspace", self.edt_sett_headspace)
-        try:
-            if load_dict["settings"]["ip_label_pos"] == "Top":
-                self.rbtn_iplable_top.setChecked(True)
-            else:
-                self.rbtn_iplable_bottom.setChecked(True)
-        except KeyError:
-            if ut.DEFAULT_SETTINGS["settings"]["ip_label_pos"] == "Top":
-                self.rbtn_iplable_top.setChecked(True)
-            else:
-                self.rbtn_iplable_bottom.setChecked(True)
-        # how to display forbidden transitions
-        try:
-            if load_dict["settings"]["show_forbidden_transitions"] == "x-out":
-                self.rbtn_sett_xoutarrow.setChecked(True)
-            else:
-                self.rbtn_sett_nodisparrow.setChecked(True)
-        except KeyError:
-            if ut.DEFAULT_SETTINGS["settings"]["show_forbidden_transitions"] == "x-out":
-                self.rbtn_sett_xoutarrow.setChecked(True)
-            else:
-                self.rbtn_sett_nodisparrow.setChecked(True)
-        # transition strength
-        try:
-            if load_dict["settings"]["show_transition_strength"]:
-                self.chk_sett_trans_strength.setChecked(True)
-            else:
-                self.chk_sett_trans_strength.setChecked(False)
-        except KeyError:
-            self.chk_sett_trans_strength.setChecked(
-                ut.DEFAULT_SETTINGS["settings"]["show_transition_strength"]
-            )
-        # line breaks
-        try:
-            if load_dict["settings"]["line_breaks"]:
-                self.chk_sett_linebreaks.setChecked(True)
-            else:
-                self.chk_sett_linebreaks.setChecked(False)
-        except KeyError:
-            self.chk_sett_linebreaks.setChecked(
-                ut.DEFAULT_SETTINGS["settings"]["line_breaks"]
-            )
-        # show cm-1 axis
-        try:
-            if load_dict["settings"]["show_cm-1_axis"]:
-                self.chk_sett_showcmax.setChecked(True)
-            else:
-                self.chk_sett_showcmax.setChecked(False)
-        except KeyError:
-            self.chk_sett_showcmax.setChecked(
-                ut.DEFAULT_SETTINGS["settings"]["show_cm-1_axis"]
-            )
-        # show eV axis
-        try:
-            if load_dict["settings"]["show_eV_axis"]:
-                self.chk_sett_showevax.setChecked(True)
-            else:
-                self.chk_sett_showevax.setChecked(False)
-        except KeyError:
-            self.chk_sett_showevax.setChecked(
-                ut.DEFAULT_SETTINGS["settings"]["show_eV_axis"]
-            )
-        # plot darkmode
-        try:
-            if load_dict["settings"]["plot_darkmode"]:
-                self.chk_plot_darkmode.setChecked(True)
-            else:
-                self.chk_plot_darkmode.setChecked(False)
-        except KeyError:
-            self.chk_plot_darkmode.setChecked(
-                ut.DEFAULT_SETTINGS["settings"]["plot_darkmode"]
-            )
+        # settings
+        arrow_width, arrow_head_width = config_parser.sett_arrow_fmt
+        self.edt_sett_arrwidth.setText(str(arrow_width))
+        self.edt_sett_arrheadwidth.setText(str(arrow_head_width))
+
+        fig_width, fig_height = config_parser.sett_fig_size
+        self.edt_sett_figwidth.setText(str(fig_width))
+        self.edt_sett_figheight.setText(str(fig_height))
+
+        fs_axticks, fs_axlabels, fs_labels, fs_title = config_parser.sett_fontsize
+        self.edt_sett_fsaxes.setText(str(fs_axticks))
+        self.edt_sett_fsaxlbl.setText(str(fs_axlabels))
+        self.edt_sett_fslbl.setText(str(fs_labels))
+        self.edt_sett_fstitle.setText(str(fs_title))
 
-        set_line_edits("settings", "plot_title", self.edt_sett_plttitle)
-        set_line_edits("settings", "prec_level", self.edt_sett_preclevel)
-        set_line_edits("settings", "prec_wavelength", self.edt_sett_preclambda)
+        self.edt_sett_headspace.setText(str(config_parser.sett_headspace))
+
+        if config_parser.sett_ip_label_pos == "Top":
+            self.rbtn_iplable_top.setChecked(True)
+        else:
+            self.rbtn_iplable_bottom.setChecked(True)
+
+        (
+            show_cm1_axis,
+            show_ev_axis,
+            show_forbidden_transitions,
+            show_transition_strength,
+        ) = config_parser.sett_shows
+        if show_forbidden_transitions == "x-out":
+            self.rbtn_sett_xoutarrow.setChecked(True)
+        else:
+            self.rbtn_sett_nodisparrow.setChecked(True)
+
+        self.chk_sett_trans_strength.setChecked(show_transition_strength)
+        self.chk_sett_showcmax.setChecked(show_cm1_axis)
+        self.chk_sett_showevax.setChecked(show_ev_axis)
+        self.chk_sett_linebreaks.setChecked(config_parser.sett_line_breaks)
+        self.drop_plot_style.setCurrentText(config_parser.sett_plot_style)
+
+        self.edt_sett_plttitle.setText(config_parser.sett_title)
+        lambda_prec, level_prec = config_parser.sett_prec
+        self.edt_sett_preclambda.setText(str(lambda_prec))
+        self.edt_sett_preclevel.setText(str(level_prec))
 
     def write_json(self) -> dict:
         """Write the json dictionary to save or pass on.
 
         :return: JSON dictionary that can either be directly plotted or can be saved.
         """
         # create the dictionary to save
@@ -912,21 +869,21 @@
         savedict["settings"]["ip_label_pos"] = iptablepos
         if self.rbtn_sett_xoutarrow.isChecked():
             dispforbidden = "x-out"
         else:
             dispforbidden = "noshow"
         savedict["settings"]["show_forbidden_transitions"] = dispforbidden
         savedict["settings"]["plot_title"] = self.edt_sett_plttitle.text()
-        savedict["settings"][
-            "show_transition_strength"
-        ] = self.chk_sett_trans_strength.isChecked()
+        savedict["settings"]["show_transition_strength"] = (
+            self.chk_sett_trans_strength.isChecked()
+        )
         savedict["settings"]["line_breaks"] = self.chk_sett_linebreaks.isChecked()
         savedict["settings"]["show_cm-1_axis"] = self.chk_sett_showcmax.isChecked()
         savedict["settings"]["show_eV_axis"] = self.chk_sett_showevax.isChecked()
-        savedict["settings"]["plot_darkmode"] = self.chk_plot_darkmode.isChecked()
+        savedict["settings"]["plot_style"] = self.drop_plot_style.currentText()
 
         return savedict
 
     def save_config(self):
         """
         Save the current configuration as a .json file the user defines
         """
@@ -986,42 +943,53 @@
         """
         Development testing routine, with the according button
         """
         fname = Path.home().joinpath(
             "Documents/code/RIMSCode/RIMSSchemeDrawer/examples/example_titanium.json"
         )
         self.load_config(fname=fname)
+        self.user_path = Path(
+            "/home/reto/Documents/code/RIMSCode/rims-code.github.io/temp/out"
+        )
 
 
 class MplCanvas(FigureCanvasQTAgg):
     def __init__(self, width=5, height=4, dpi=100):
         super().__init__()
         fig = Figure(figsize=(width, height), dpi=dpi)
         self.axes = fig.add_subplot(111)
         super().__init__(fig)
 
 
 class PlotDisplay(QtWidgets.QMainWindow):
     def __init__(
-        self, json_data: dict, parent: QtWidgets.QWidget = None, darkmode: bool = False
+        self,
+        json_data: dict,
+        parent: QtWidgets.QWidget = None,
+        darkmode: bool = False,
+        transparent: bool = False,
     ):
         """Prepare the plot display window.
 
         :param json_data: Data according to rimsschemedrawer json format.
         :param parent: Parent widget.
         :param darkmode: Use dark background for plot?
+        :param transparent: Use transparent background for plot?
         """
         super().__init__(parent=parent)
 
         if darkmode:
             plt.style.use("dark_background")
         else:
             plt.style.use("default")
         sc = MplCanvas(width=5, height=4, dpi=100)
         Plotter(json_data, fig_ax=(sc.figure, sc.axes))
+        if transparent:
+            sc.figure.patch.set_alpha(0.0)
+            sc.axes.patch.set_alpha(0.0)
 
         toolbar = NavigationToolbar(sc, self)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(toolbar)
         layout.addWidget(sc)
```

### Comparing `rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/json_parser.py` & `rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/json_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,24 +43,34 @@
 
     @property
     def gs_term(self) -> str:
         """Get the ground state term, formatted for plotting."""
         return ut.term_to_string(self._gs_term)
 
     @property
+    def gs_term_no_formatting(self) -> str:
+        """Get the ground state term, not formatted for plotting."""
+        return self._gs_term
+
+    @property
     def ip_level(self) -> float:
         """Get the ionization potential level."""
         return self._ip_level
 
     @property
     def ip_term(self) -> str:
         """Get the ionization potential term, formatted for plotting."""
         return ut.term_to_string(self._ip_term)
 
     @property
+    def ip_term_no_formatting(self):
+        """Get the ionization potential term, not formatted for plotting."""
+        return self._ip_term
+
+    @property
     def is_low_lying(self) -> np.ndarray:
         """Return a boolean array if a level is a low-lying state.
 
         This array has as many entries as there are steps in the scheme.
 
         :return: Boolean array if a level is a low-lying state.
         """
@@ -73,19 +83,14 @@
 
     @property
     def number_of_levels(self) -> int:
         """Get the number of steps in the scheme."""
         return self._num_steps
 
     @property
-    def rims_scheme(self) -> Dict:
-        """Return the full scheme parsed into a dictionary."""
-        return
-
-    @property
     def step_levels(self) -> np.ndarray:
         """Get all levels of the scheme."""
         return self._step_levels_cm
 
     @property
     def step_forbidden(self) -> np.ndarray:
         """Get all forbidden transitions."""
@@ -98,14 +103,19 @@
 
     @property
     def step_terms(self) -> np.ndarray:
         """Get the terms for all states, formatted for plotting."""
         return np.array([ut.term_to_string(it) for it in self._step_term])
 
     @property
+    def step_terms_no_formatting(self) -> np.ndarray:
+        """Get the terms for all states, not formatted for plotting."""
+        return self._step_term
+
+    @property
     def transition_strengths(self) -> np.ndarray:
         """Get the transition strength of all steps."""
         return self._transition_strength
 
     # SETTINGS PROPERTIES
 
     @property
@@ -113,22 +123,14 @@
         """Get the arrow formatting for the plot.
 
         :return: Arrow width, arrow head width.
         """
         return self._sett_arrow_fmt
 
     @property
-    def sett_darkmode(self) -> bool:
-        """Get the darkmode setting for the plot.
-
-        :return: Darkmode setting.
-        """
-        return self._sett_darkmode
-
-    @property
     def sett_fig_size(self) -> Tuple[float, float]:
         """Get the figure size for the plot.
 
         :return: Figure size: width, height
         """
         return self._sett_fig_size
 
@@ -160,26 +162,55 @@
         """Get the precisions for the plot.
 
         :return: Precisions for: wavelength, level
         """
         return self._sett_prec
 
     @property
+    def sett_plot_dark(self) -> bool:
+        """Get the darkmode setting for the plot.
+
+        :return: Darkmode setting.
+        """
+        return "dark" in self._sett_plot_style
+
+    @property
+    def sett_plot_style(self) -> str:
+        """Get the plot style setting for the plot.
+
+        :return: Plot style setting.
+        """
+        return self._sett_plot_style
+
+    @property
+    def sett_plot_transparent(self) -> bool:
+        """Get the transparent setting for the plot.
+
+        :return: Transparent setting.
+        """
+        return "transparent" in self._sett_plot_style
+
+    @property
     def sett_shows(self) -> Tuple[bool, bool, str, bool]:
         """Get the settings for the plot.
 
         :return: Settings for: cm-1 axis, eV axis, forbidden transitions, transition strength
         """
         return self._sett_shows
 
     @property
     def sett_title(self) -> str:
         """Get the title for the plot."""
         return self._sett_title
 
+    @property
+    def sett_unit_nm(self) -> bool:
+        """Return if the unit is in nm."""
+        return self._input_nm
+
     # METHODS
 
     def scheme_table(self, prec: int = 3, prec_strength: int = 1) -> Tuple[List, List]:
         """Create a scheme table for further processing.
 
         The headers are the following:
         - Step
@@ -495,15 +526,15 @@
             get_value("show_cm-1_axis", bool),
             get_value("show_eV_axis", bool),
             get_value("show_forbidden_transitions", str),
             get_value("show_transition_strength", bool),
         )
 
         # Darkmode
-        self._sett_darkmode = get_value("plot_darkmode", bool)
+        self._sett_plot_style = get_value("plot_style", str)
 
 
 def json_reader(fin: Path) -> Dict:
     """Read a json file and return a dictionary.
 
     This can take old or new files and return the data that
     can be read by the program.
```

### Comparing `rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/plotter.py` & `rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         :param data: Dictionary with the data to plot, directly from json file.
         :param kwargs: Additional keyword arguments.
             - number_of_steps: How many scheme steps to consider, default is 7.
                 This number can be higher than the number of available steps!
             - fig_ax: Tuple of matplotlib figure and axes to plot on. Defaults to
                 creating new ones.
             - darkmode: Overwrite the darkmode settings from the config file.
+            - transparent: Overwrite the transparency settings from the config file.
         """
         self.config_parser = ConfigParser(data)
 
         # check if old style
         if self.config_parser.element_guessed:
             warnings.warn(
                 f"Old style input detected, where the IP is set manually. "
@@ -38,15 +39,18 @@
 
         # matplotlib parameters
         # tick size
         fsz_axes = self.config_parser.sett_fontsize[0]
         matplotlib.rc("xtick", labelsize=fsz_axes, direction="in")
         matplotlib.rc("ytick", labelsize=fsz_axes, direction="in")
 
-        darkmode = kwargs.get("darkmode", self.config_parser.sett_darkmode)
+        darkmode = kwargs.get("darkmode", self.config_parser.sett_plot_dark)
+        self.transparent = kwargs.get(
+            "transparent", self.config_parser.sett_plot_transparent
+        )
 
         # figure stuff
         if darkmode:
             plt.style.use("dark_background")
         else:
             plt.style.use("default")
 
@@ -75,14 +79,17 @@
     def axes(self) -> plt.Axes:
         """Return the axes."""
         return self._axes
 
     @property
     def figure(self) -> plt.Figure:
         """Return the figure."""
+        if self.transparent:
+            self._figure.patch.set_alpha(0.0)
+            self._figure.axes[0].patch.set_alpha(0.0)
         return self._figure
 
     def savefig(self, fout: str):
         """Save the figure to a file.
 
         :param fout: File name to save the plot to. The file extension determines
             the file type.
@@ -147,18 +154,16 @@
         term_symb_es_formatted = self.config_parser.step_terms[
             self.config_parser.is_low_lying
         ]
 
         # ymax:
         if ipvalue > totwavenumber_photons + wavenumber_gs:
             ymax = ipvalue + sett_headspace
-        elif totwavenumber_photons + wavenumber_gs - ipvalue < sett_headspace:
-            ymax = ipvalue + sett_headspace
         else:
-            ymax = totwavenumber_photons + wavenumber_gs
+            ymax = totwavenumber_photons + wavenumber_gs + sett_headspace
 
         # ### CREATE FIGURE ###
         a2 = self._axes.twinx()
         self._figure.set_size_inches(*self.config_parser.sett_fig_size, forward=True)
 
         # shade the level above the IP
         xshade = [0.0, 10.0]  # x-axis of the shade (which is never displayed)
```

### Comparing `rimsschemedrawer-3.0.0.dev3/src/rimsschemedrawer/utils.py` & `rimsschemedrawer-3.0.0.dev4/src/rimsschemedrawer/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
         "plot_title": "",
         "fig_width": 5,
         "fig_height": 8,
         "fs_title": 14,
         "fs_axes": 12,
         "fs_axes_labels": 12,
         "fs_labels": 12,
-        "headspace": 3000,
+        "headspace": 1300,
         "arrow_width": 0.2,
         "arrow_head_width": 0.6,
         "prec_wavelength": 3,
         "prec_level": 0,
         "line_breaks": False,
         "ip_label_pos": "Bottom",
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": True,
         "show_cm-1_axis": True,
         "show_eV_axis": True,
-        "plot_darkmode": False,
+        "plot_style": "light",
     },
     "scheme": {
         "gs_term": "",
         "ip_term": "",
     },
 }
 
@@ -142,14 +142,16 @@
     "Sg": 63000.0,
     "Bh": 62000.0,
     "Hs": 61000.0,
 }
 
 LASERS = ["Ti:Sa", "Dye", "Ti:Sa and Dye"]  # default is first entry - Ti:Sa
 
+PLOT_STYLES = ["light", "dark", "light transparent", "dark transparent"]
+
 
 def cm_2_to_nm(cm: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
     """Convert a wavenumber in cm^-1 to a wavelength in nm.
 
     :param cm: Wavenumber in cm^-1.
     :return: Wavelength in nm.
     """
@@ -219,22 +221,30 @@
     :param nm: Wavelength in nm.
     :return: Wavenumber in cm^-1.
     """
     return 1e7 / nm
 
 
 def term_to_string(tstr: str):
-    """
+    """Convert term symbol to LaTeX enabled string.
+
     Converts a term symbol string to a LaTeX enabled matplotlib string
+    If already a LaTeX string, just return it.
     :param tstr:   Input string to convert
     :return:       Output string LaTeX enabled for Matplotlib
     """
     if tstr == "":
         return None
 
+    latex_characters = ["{", "}", "^", "_"]
+    for lch in latex_characters:
+        if lch in tstr:
+            tstr = tstr.replace(" ", "\\,")
+            return f"${tstr}$"
+
     # some exceptionslike AI and IP
     if tstr == "IP":
         return "IP"
     if tstr == "AI":
         return "AI"
     if tstr == "Rydberg":
         return "Rydberg"
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/test_json_parser.py` & `rimsschemedrawer-3.0.0.dev4/tests/test_json_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import json
 
 import pytest
 import numpy as np
 
 import rimsschemedrawer.json_parser as jp
+import rimsschemedrawer.utils as ut
 
 
 @pytest.mark.parametrize("fname", ["ti.json", "w_nm.json"])
 def test_config_parser(data_path, fname):
     """Run through parser with all json files in the data folder."""
     fin = data_path.joinpath(fname)
     data = jp.json_reader(fin)
@@ -41,16 +42,16 @@
     fin_mixed = data_path.joinpath(fname[1])
     data = jp.json_reader(fin)
     data_mixed = jp.json_reader(fin_mixed)
 
     parser = jp.ConfigParser(data)
     parser_mixed = jp.ConfigParser(data_mixed)
 
-    assert not parser._input_nm
-    assert parser_mixed._input_nm
+    assert not parser.sett_unit_nm
+    assert parser_mixed.sett_unit_nm
 
     # make sure the steps are the same!
     np.testing.assert_almost_equal(
         parser_mixed._step_levels_cm, parser._step_levels_cm, decimal=1
     )
 
 
@@ -72,14 +73,31 @@
     fin = data_path.joinpath(fname)
     data = jp.json_reader(fin)
     parser = jp.ConfigParser(data)
 
     np.testing.assert_almost_equal(parser._steps_nm, nm_exp, decimal=3)
 
 
+def test_config_parser_fmt_terms(data_path):
+    """Ensure formatted and unformatted term symbols are available."""
+    fin = data_path.joinpath("ti.json")
+    data = jp.json_reader(fin)
+    parser = jp.ConfigParser(data)
+
+    gs_term_fmt_exp = ut.term_to_string(parser.gs_term_no_formatting)
+    ip_term_fmt_exp = ut.term_to_string(parser.ip_term_no_formatting)
+    step_terms_fmt_exp = [
+        ut.term_to_string(term) for term in parser.step_terms_no_formatting
+    ]
+
+    assert parser.gs_term == gs_term_fmt_exp
+    assert parser.ip_term == ip_term_fmt_exp
+    assert (parser.step_terms == step_terms_fmt_exp).all()
+
+
 def test_json_reader(data_path):
     """Check that a valid json file is returned."""
     fin = data_path.joinpath("ti.json")
     data = jp.json_reader(fin)
 
     assert isinstance(data, dict)
     assert "scheme" in data.keys()
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/test_plotter.py` & `rimsschemedrawer-3.0.0.dev4/tests/test_plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Test the plotter
 import pytest
 
 import rimsschemedrawer.json_parser
 from rimsschemedrawer.plotter import Plotter
 
 
-def test_plotter(data_path, tmp_path):
+@pytest.mark.parametrize("darkmode", [True, False])
+@pytest.mark.parametrize("transparent", [True, False])
+def test_plotter(data_path, tmp_path, darkmode, transparent):
     """Run through the plotter with a simple scheme, assert no errors."""
     fin = data_path.joinpath("ti.json")
     data = rimsschemedrawer.json_parser.json_reader(fin)
 
     fname = tmp_path.joinpath("test.pdf")
-    fig = Plotter(data)
+    fig = Plotter(data, darkmode=darkmode, transparent=transparent)
     fig.savefig(fname)
 
     assert fname.exists()
 
 
 def test_plotter_old_style(data_path):
     """Raise warning when old style file is detected."""
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/test_scheme_table.py` & `rimsschemedrawer-3.0.0.dev4/tests/test_scheme_table.py`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/test_utils.py` & `rimsschemedrawer-3.0.0.dev4/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,11 +83,18 @@
 
 @pytest.mark.parametrize("vals", [["3F2", "$^{3}$F$_{2}$"], ["4G1", "$^{4}$G$_{1}$"]])
 def test_term_to_string(vals):
     """Check that the term symbols are converted correctly."""
     assert ut.term_to_string(vals[0]) == vals[1]
 
 
+def test_term_to_string_latex():
+    """Return a string surrounded by $ if LaTeX characters found."""
+    str_in = "^{3}F_{2}"
+    str_exp = f"${str_in}$"
+    assert ut.term_to_string(str_in) == str_exp
+
+
 @pytest.mark.parametrize("val", ["IP", "AI", "Rydberg", "Ryd"])
 def test_term_to_string_no_change(val):
     """Leave these symbols / strings unchanged."""
     assert ut.term_to_string(val) == val
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_cm.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_nm.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {"'scheme'": "{'step_forbidden1': False, 'step_level0': '400.262', 'step_level1': '407.469', "*

 * *             "'step_level2': '771.908', 'trans_strength0': '', 'trans_strength2': '', 'unit': "*

 * *             "'nm'}",*

 * * "'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -1,23 +1,23 @@
 {
     "scheme": {
         "element": "W",
         "gs_level": "1000",
         "gs_term": "5D0",
         "ip_term": "",
         "step_forbidden0": false,
-        "step_forbidden1": true,
+        "step_forbidden1": false,
         "step_forbidden2": false,
         "step_forbidden3": false,
         "step_forbidden4": false,
         "step_forbidden5": false,
         "step_forbidden6": false,
-        "step_level0": "25983.609454",
-        "step_level1": "50525.35385",
-        "step_level2": "63480.26554",
+        "step_level0": "400.262",
+        "step_level1": "407.469",
+        "step_level2": "771.908",
         "step_level3": "",
         "step_level4": "",
         "step_level5": "",
         "step_level6": "",
         "step_lowlying0": false,
         "step_lowlying1": false,
         "step_lowlying2": false,
@@ -28,36 +28,36 @@
         "step_term0": "5F1",
         "step_term1": "5D2",
         "step_term2": "AI",
         "step_term3": "",
         "step_term4": "",
         "step_term5": "",
         "step_term6": "",
-        "trans_strength0": "1e6",
+        "trans_strength0": "",
         "trans_strength1": "",
-        "trans_strength2": "3.015e5",
+        "trans_strength2": "",
         "trans_strength3": "",
         "trans_strength4": "",
         "trans_strength5": "",
         "trans_strength6": "",
-        "unit": "cm<sup>-1</sup>"
+        "unit": "nm"
     },
     "settings": {
         "arrow_head_width": "0.6",
         "arrow_width": "0.2",
         "fig_height": "8",
         "fig_width": "5.2",
         "fs_axes": "12",
         "fs_axes_labels": "12",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "3000",
         "ip_label_pos": "Bottom",
         "line_breaks": true,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "2",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_low_lying_cm.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_low_lying_cm.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -49,15 +49,15 @@
         "fs_axes": "12",
         "fs_axes_labels": "14",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "2700",
         "ip_label_pos": "Top",
         "line_breaks": false,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "0",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_low_lying_nm.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/ti_new.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.959375%*

 * *Differences: {"'scheme'": "{'gs_level': '0', 'step_level2': '21469.5', 'step_level3': '45498.85', "*

 * *             "'step_level4': '56844.45', 'unit': 'cm<sup>-1</sup>'}",*

 * * "'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "scheme": {
         "element": "Ti",
-        "gs_level": "160",
+        "gs_level": "0",
         "gs_term": "3F2",
         "ip_term": "",
         "step_forbidden0": false,
         "step_forbidden1": false,
         "step_forbidden2": false,
         "step_forbidden3": false,
         "step_forbidden4": false,
         "step_forbidden5": false,
         "step_forbidden6": false,
         "step_level0": "170.15",
         "step_level1": "386.88",
-        "step_level2": "469.274",
-        "step_level3": "416.158",
-        "step_level4": "881.399",
+        "step_level2": "21469.5",
+        "step_level3": "45498.85",
+        "step_level4": "56844.45",
         "step_level5": "",
         "step_level6": "",
         "step_lowlying0": true,
         "step_lowlying1": true,
         "step_lowlying2": false,
         "step_lowlying3": false,
         "step_lowlying4": false,
@@ -35,29 +35,29 @@
         "trans_strength0": "",
         "trans_strength1": "",
         "trans_strength2": "",
         "trans_strength3": "",
         "trans_strength4": "",
         "trans_strength5": "",
         "trans_strength6": "",
-        "unit": "nm"
+        "unit": "cm<sup>-1</sup>"
     },
     "settings": {
         "arrow_head_width": "0.6",
         "arrow_width": "0.2",
         "fig_height": "8",
         "fig_width": "5",
         "fs_axes": "12",
         "fs_axes_labels": "14",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "2700",
         "ip_label_pos": "Top",
         "line_breaks": false,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "0",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/raised_ground_nm.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/w_nm.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9628048780487805%*

 * *Differences: {"'scheme'": "{'gs_level': '0', 'step_level0': '384.858', 'lasers': 'Ti:Sa'}",*

 * * "'settings'": "{'plot_style': 'dark transparent', delete: ['plot_darkmode']}"}*

```diff
@@ -1,21 +1,22 @@
 {
     "scheme": {
         "element": "W",
-        "gs_level": "1000",
+        "gs_level": "0",
         "gs_term": "5D0",
         "ip_term": "",
+        "lasers": "Ti:Sa",
         "step_forbidden0": false,
         "step_forbidden1": false,
         "step_forbidden2": false,
         "step_forbidden3": false,
         "step_forbidden4": false,
         "step_forbidden5": false,
         "step_forbidden6": false,
-        "step_level0": "400.262",
+        "step_level0": "384.858",
         "step_level1": "407.469",
         "step_level2": "771.908",
         "step_level3": "",
         "step_level4": "",
         "step_level5": "",
         "step_level6": "",
         "step_lowlying0": false,
@@ -49,15 +50,15 @@
         "fs_axes": "12",
         "fs_axes_labels": "12",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "3000",
         "ip_label_pos": "Bottom",
         "line_breaks": true,
-        "plot_darkmode": false,
+        "plot_style": "dark transparent",
         "plot_title": "",
         "prec_level": "2",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/ti.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/ti.json`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/ti_new.json` & `rimsschemedrawer-3.0.0.dev4/examples/example_titanium.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9382220795892169%*

 * *Differences: {"'scheme'": "{'gs_level': '0.0', 'lasers': 'Ti:Sa'}",*

 * * "'settings'": "{'fig_height': '8.0', 'fig_width': '5.0', 'fs_axes': '12.0', 'fs_axes_labels': "*

 * *               "'14.0', 'fs_labels': '12.0', 'fs_title': '14.0', 'headspace': '2700.0', "*

 * *               "'show_transition_strength': True}"}*

```diff
@@ -1,13 +1,14 @@
 {
     "scheme": {
         "element": "Ti",
-        "gs_level": "0",
+        "gs_level": "0.0",
         "gs_term": "3F2",
         "ip_term": "",
+        "lasers": "Ti:Sa",
         "step_forbidden0": false,
         "step_forbidden1": false,
         "step_forbidden2": false,
         "step_forbidden3": false,
         "step_forbidden4": false,
         "step_forbidden5": false,
         "step_forbidden6": false,
@@ -40,26 +41,26 @@
         "trans_strength5": "",
         "trans_strength6": "",
         "unit": "cm<sup>-1</sup>"
     },
     "settings": {
         "arrow_head_width": "0.6",
         "arrow_width": "0.2",
-        "fig_height": "8",
-        "fig_width": "5",
-        "fs_axes": "12",
-        "fs_axes_labels": "14",
-        "fs_labels": "12",
-        "fs_title": "14",
-        "headspace": "2700",
+        "fig_height": "8.0",
+        "fig_width": "5.0",
+        "fs_axes": "12.0",
+        "fs_axes_labels": "14.0",
+        "fs_labels": "12.0",
+        "fs_title": "14.0",
+        "headspace": "2700.0",
         "ip_label_pos": "Top",
         "line_breaks": false,
         "plot_darkmode": false,
         "plot_title": "",
         "prec_level": "0",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
-        "show_transition_strength": false
+        "show_transition_strength": true
     }
 }
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/ti_new_mixed_units.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/ti_new_mixed_units.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -49,15 +49,15 @@
         "fs_axes": "12",
         "fs_axes_labels": "14",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "2700",
         "ip_label_pos": "Top",
         "line_breaks": false,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "0",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/w_cm-1.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/w_cm-1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -49,15 +49,15 @@
         "fs_axes": "12",
         "fs_axes_labels": "12",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "3000",
         "ip_label_pos": "Bottom",
         "line_breaks": true,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "2",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/tests/data/w_nm.json` & `rimsschemedrawer-3.0.0.dev4/tests/data/raised_ground_cm.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9445121951219512%*

 * *Differences: {"'scheme'": "{'gs_level': '1000', 'step_forbidden1': True, 'step_level0': '25983.609454', "*

 * *             "'step_level1': '50525.35385', 'step_level2': '63480.26554', 'trans_strength0': "*

 * *             "'1e6', 'trans_strength2': '3.015e5', 'unit': 'cm<sup>-1</sup>', delete: ['lasers']}",*

 * * "'settings'": "{'plot_style': 'light', delete: ['plot_darkmode']}"}*

```diff
@@ -1,24 +1,23 @@
 {
     "scheme": {
         "element": "W",
-        "gs_level": "0",
+        "gs_level": "1000",
         "gs_term": "5D0",
         "ip_term": "",
-        "lasers": "Ti:Sa",
         "step_forbidden0": false,
-        "step_forbidden1": false,
+        "step_forbidden1": true,
         "step_forbidden2": false,
         "step_forbidden3": false,
         "step_forbidden4": false,
         "step_forbidden5": false,
         "step_forbidden6": false,
-        "step_level0": "384.858",
-        "step_level1": "407.469",
-        "step_level2": "771.908",
+        "step_level0": "25983.609454",
+        "step_level1": "50525.35385",
+        "step_level2": "63480.26554",
         "step_level3": "",
         "step_level4": "",
         "step_level5": "",
         "step_level6": "",
         "step_lowlying0": false,
         "step_lowlying1": false,
         "step_lowlying2": false,
@@ -29,36 +28,36 @@
         "step_term0": "5F1",
         "step_term1": "5D2",
         "step_term2": "AI",
         "step_term3": "",
         "step_term4": "",
         "step_term5": "",
         "step_term6": "",
-        "trans_strength0": "",
+        "trans_strength0": "1e6",
         "trans_strength1": "",
-        "trans_strength2": "",
+        "trans_strength2": "3.015e5",
         "trans_strength3": "",
         "trans_strength4": "",
         "trans_strength5": "",
         "trans_strength6": "",
-        "unit": "nm"
+        "unit": "cm<sup>-1</sup>"
     },
     "settings": {
         "arrow_head_width": "0.6",
         "arrow_width": "0.2",
         "fig_height": "8",
         "fig_width": "5.2",
         "fs_axes": "12",
         "fs_axes_labels": "12",
         "fs_labels": "12",
         "fs_title": "14",
         "headspace": "3000",
         "ip_label_pos": "Bottom",
         "line_breaks": true,
-        "plot_darkmode": false,
+        "plot_style": "light",
         "plot_title": "",
         "prec_level": "2",
         "prec_wavelength": "3",
         "show_cm-1_axis": true,
         "show_eV_axis": true,
         "show_forbidden_transitions": "x-out",
         "show_transition_strength": false
```

### Comparing `rimsschemedrawer-3.0.0.dev3/LICENSE` & `rimsschemedrawer-3.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `rimsschemedrawer-3.0.0.dev3/pyproject.toml` & `rimsschemedrawer-3.0.0.dev4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rimsschemedrawer"
-version = "3.0.0dev3"
+version = "3.0.0dev4"
 description = "Drawing of RIMS schemes in python and/or with a Python GUI."
 authors = [
     { name = "Reto Trappitsch", email = "reto@galactic-forensics.space" }
 ]
 dependencies = [
     "matplotlib>=3.7.4",
     "numpy>=1.24.4",
@@ -17,29 +17,33 @@
 rimsschemedrawer = "rimsschemedrawer.app:run_gui"
 
 [project.optional-dependencies]
 gui = [
     "PyQt6>=6.6.1",
     "qtpy>=2.4.1",
 ]
+docs = [
+    "mkdocs>=1.5.3",
+    "mkdocs-material>=9.5.12",
+    "mkdocstrings[python]>=0.24.1",
+]
 
 [project.urls]
 Homepage = "https://github.com/RIMS-Code/RIMSSchemeDrawer"
 Documentation = "https://github.com/RIMS-Code/RIMSSchemeDrawer"
 Repository = "https://github.com/RIMS-Code/RIMSSchemeDrawer.git"
 Issues = "https://github.com/RIMS-Code/RIMSSchemeDrawer/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
-    "ruff>=0.1.14",
     "pytest>=7.4.4",
     "hypothesis>=6.97.1",
     "pytest-cov>=4.1.0",
     "requests>=2.31.0",
 ]
 
 [tool.rye.scripts]
@@ -53,12 +57,13 @@
 packages = ["src/rimsschemedrawer"]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = "--cov -v"
 filterwarnings = 'ignore:datetime.datetime.utcfromtimestamp\(\) is deprecated:DeprecationWarning'  # 3rd party
 
+
+
 [tool.box]
 builder = "rye"
 app_entry = "rimsschemedrawer.app:run_gui"
-app_name = "rimsschemedrawer[gui]"
-optional_deps = "gui"
+python_version = "3.12"
```

