# Comparing `tmp/ogusa-0.1.3.tar.gz` & `tmp/ogusa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogusa-0.1.3.tar", last modified: Mon Feb 12 23:18:00 2024, max compression
+gzip compressed data, was "ogusa-0.1.4.tar", last modified: Fri Apr  5 02:05:48 2024, max compression
```

## Comparing `ogusa-0.1.3.tar` & `ogusa-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:18:00.163147 ogusa-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-12 23:17:53.000000 ogusa-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-02-12 23:18:00.163147 ogusa-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-02-12 23:17:53.000000 ogusa-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:18:00.159146 ogusa-0.1.3/ogusa/
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/bequest_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/calibrate_chi_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/deterministic_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/estimate_beta_j.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/get_micro_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/labor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/macro_params.py
--rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/ogusa_default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/psid_data_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/psid_summ_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/transfer_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/wealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-02-12 23:17:54.000000 ogusa-0.1.3/ogusa/wealthinit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:18:00.163147 ogusa-0.1.3/ogusa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-02-12 23:18:00.000000 ogusa-0.1.3/ogusa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-12 23:18:00.000000 ogusa-0.1.3/ogusa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 23:18:00.000000 ogusa-0.1.3/ogusa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-12 23:18:00.000000 ogusa-0.1.3/ogusa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-12 23:18:00.000000 ogusa-0.1.3/ogusa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-12 23:17:54.000000 ogusa-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 23:18:00.163147 ogusa-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-12 23:17:54.000000 ogusa-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.396954 ogusa-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-05 02:05:44.000000 ogusa-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-05 02:05:48.396954 ogusa-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-05 02:05:44.000000 ogusa-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.392954 ogusa-0.1.4/ogusa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/bequest_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/calibrate_chi_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/deterministic_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/estimate_beta_j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/get_micro_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/labor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/macro_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/ogusa_default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/psid_data_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/psid_summ_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/transfer_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/wealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/wealthinit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.396954 ogusa-0.1.4/ogusa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 02:05:44.000000 ogusa-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:05:48.396954 ogusa-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-05 02:05:44.000000 ogusa-0.1.4/setup.py
```

### Comparing `ogusa-0.1.3/LICENSE` & `ogusa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/PKG-INFO` & `ogusa-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.3
+Version: 0.1.4
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.3/README.md` & `ogusa-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/bequest_transmission.py` & `ogusa-0.1.4/ogusa/bequest_transmission.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/calibrate.py` & `ogusa-0.1.4/ogusa/calibrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 
     def __init__(
         self,
         p,
         estimate_tax_functions=False,
         estimate_beta=False,
         estimate_chi_n=False,
+        estimate_pop=False,
         tax_func_path=None,
         iit_reform={},
         guid="",
         data="cps",
         client=None,
         num_workers=1,
     ):
         self.estimate_tax_functions = estimate_tax_functions
         self.estimate_beta = estimate_beta
         self.estimate_chi_n = estimate_chi_n
+        self.estimate_pop = estimate_pop
         if estimate_tax_functions:
             if tax_func_path is not None:
                 run_micro = False
             else:
                 run_micro = True
             self.tax_function_params = self.get_tax_function_parameters(
                 p,
@@ -38,58 +40,67 @@
                 guid,
                 data,
                 client,
                 num_workers,
                 run_micro=run_micro,
                 tax_func_path=tax_func_path,
             )
-        if estimate_beta:
+        if self.estimate_beta:
             self.beta_j = estimate_beta_j.beta_estimate(self)
         # if estimate_chi_n:
         #     chi_n = self.get_chi_n()
 
         # Macro estimation
         self.macro_params = macro_params.get_macro_params()
 
         # eta estimation
         self.eta = transfer_distribution.get_transfer_matrix(p.J, p.lambdas)
 
         # zeta estimation
         self.zeta = bequest_transmission.get_bequest_matrix(p.J, p.lambdas)
 
         # demographics
-        self.demographic_params = demographics.get_pop_objs(
-            p.E,
-            p.S,
-            p.T,
-            0,
-            99,
-            initial_data_year=p.start_year - 1,
-            final_data_year=p.start_year,
-        )
+        if estimate_pop:
+            self.demographic_params = demographics.get_pop_objs(
+                p.E,
+                p.S,
+                p.T,
+                0,
+                99,
+                initial_data_year=p.start_year - 1,
+                final_data_year=p.start_year,
+            )
 
-        # demographics for 80 period lives (needed for getting e below)
-        demog80 = demographics.get_pop_objs(
-            20,
-            80,
-            p.T,
-            0,
-            99,
-            initial_data_year=p.start_year - 1,
-            final_data_year=p.start_year,
-        )
+            # demographics for 80 period lives (needed for getting e below)
+            demog80 = demographics.get_pop_objs(
+                20,
+                80,
+                p.T,
+                0,
+                99,
+                initial_data_year=p.start_year - 1,
+                final_data_year=p.start_year,
+            )
 
-        # earnings profiles
-        self.e = income.get_e_interp(
-            p.S,
-            self.demographic_params["omega_SS"],
-            demog80["omega_SS"],
-            p.lambdas,
-            plot=False,
-        )
+            # earnings profiles
+            self.e = income.get_e_interp(
+                p.S,
+                self.demographic_params["omega_SS"],
+                demog80["omega_SS"],
+                p.lambdas,
+                plot=False,
+            )
+        else:
+            self.e = income.get_e_interp(
+                p.S,
+                p.omega_SS,
+                p.omega_SS,
+                p.lambdas,
+                plot=False,
+            )
 
     # Tax Functions
     def get_tax_function_parameters(
         self,
         p,
         iit_reform={},
         guid="",
@@ -330,10 +341,11 @@
             dict["beta_annual"] = self.beta
         if self.estimate_chi_n:
             dict["chi_n"] = self.chi_n
         dict["eta"] = self.eta
         dict["zeta"] = self.zeta
         dict.update(self.macro_params)
         dict["e"] = self.e
-        dict.update(self.demographic_params)
+        if self.estimate_pop:
+            dict.update(self.demographic_params)
 
         return dict
```

### Comparing `ogusa-0.1.3/ogusa/calibrate_chi_n.py` & `ogusa-0.1.4/ogusa/calibrate_chi_n.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/constants.py` & `ogusa-0.1.4/ogusa/constants.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/deterministic_profiles.py` & `ogusa-0.1.4/ogusa/deterministic_profiles.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/estimate_beta_j.py` & `ogusa-0.1.4/ogusa/estimate_beta_j.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/get_micro_data.py` & `ogusa-0.1.4/ogusa/get_micro_data.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/income.py` & `ogusa-0.1.4/ogusa/income.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/labor.py` & `ogusa-0.1.4/ogusa/labor.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/macro_params.py` & `ogusa-0.1.4/ogusa/macro_params.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/ogusa_default_parameters.json` & `ogusa-0.1.4/ogusa/ogusa_default_parameters.json`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/psid_data_setup.py` & `ogusa-0.1.4/ogusa/psid_data_setup.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/psid_summ_stats.py` & `ogusa-0.1.4/ogusa/psid_summ_stats.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/transfer_distribution.py` & `ogusa-0.1.4/ogusa/transfer_distribution.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/utils.py` & `ogusa-0.1.4/ogusa/utils.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/wealth.py` & `ogusa-0.1.4/ogusa/wealth.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa/wealthinit.py` & `ogusa-0.1.4/ogusa/wealthinit.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/ogusa.egg-info/PKG-INFO` & `ogusa-0.1.4/ogusa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.3
+Version: 0.1.4
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.3/ogusa.egg-info/SOURCES.txt` & `ogusa-0.1.4/ogusa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.3/setup.py` & `ogusa-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="ogusa",
-    version="0.1.3",
+    version="0.1.4",
     author="Jason DeBacker and Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="USA calibration for OG-Core",
     long_description=readme,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

