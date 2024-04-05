# Comparing `tmp/ex_fuzzy-1.1.0.tar.gz` & `tmp/ex_fuzzy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.0.tar", last modified: Fri Apr  5 13:45:47 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.1.tar", last modified: Fri Apr  5 15:41:19 2024, max compression
```

## Comparing `ex_fuzzy-1.1.0.tar` & `ex_fuzzy-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.972296 ex_fuzzy-1.1.0/
--rw-rw-rw-   0        0        0     3679 2024-04-05 13:45:47.971283 ex_fuzzy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2801 2024-03-13 11:20:26.000000 ex_fuzzy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.934263 ex_fuzzy-1.1.0/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.963675 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      255 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2630 2024-04-05 13:39:34.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    42930 2024-04-05 13:22:39.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17292 2024-04-04 10:16:57.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11458 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    39187 2024-04-05 13:20:29.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25690 2024-04-05 13:35:53.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.945573 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     3679 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 13:45:47.973007 ex_fuzzy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-05 13:42:47.000000 ex_fuzzy-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.970773 ex_fuzzy-1.1.0/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.197286 ex_fuzzy-1.1.1/
+-rw-rw-rw-   0        0        0     3679 2024-04-05 15:41:19.196516 ex_fuzzy-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2801 2024-03-13 11:20:26.000000 ex_fuzzy-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.147572 ex_fuzzy-1.1.1/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.187916 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      255 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    42930 2024-04-05 13:22:39.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11458 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    39187 2024-04-05 13:20:29.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.169590 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     3679 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-05 15:41:19.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 15:41:18.000000 ex_fuzzy-1.1.1/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:41:19.197286 ex_fuzzy-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-05 15:41:14.000000 ex_fuzzy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:41:19.194003 ex_fuzzy-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.1/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.0/PKG-INFO` & `ex_fuzzy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.0/README.md` & `ex_fuzzy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,12 +60,13 @@
             print(res)
 
     if plot_partitions:
         fl_classifier.plot_fuzzy_variables()
 
     if plot_rules:
         vis_rules.visualize_rulebase(fl_classifier.rule_base, export_path=export_path)
+        
     if return_rules:
         return res
```

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         :param name: string.
         :param secondMF_lower: four real numbers. Parameters of the lower trapezoid/gaussian function.
         :param secondMF_upper: four real numbers. Parameters of the upper trapezoid/gaussian function.
         :param domain: list of two numbers. Limits of the domain of the fuzzy set.
         '''
         if mnt.save_usage_flag:
             mnt.usage_data[mnt.usage_categories.FuzzySets][self.type().name] += 1
+            
         self.name = name
         self.domain = domain
         self.membership_parameters = membership_parameters
 
 
     def membership(self, x: np.array) -> np.array:
         '''
```

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,28 +568,28 @@
     NEW_FUZZY_SETS = enum.Enum(
         "FUZZY_SETS",
         [(es.name, es.value) for es in fs.FUZZY_SETS] + [(es.name, es.value) for es in new_fuzzy_sets_enum]
         )
     fs.FUZZY_SETS = NEW_FUZZY_SETS
 
 
-def mcc_loss(ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.99, beta:float=0.0125, gamma:float=0.0125) -> float:
+def mcc_loss(ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.99, beta:float=0.0125, gamma:float=0.0125, precomputed_truth=None) -> float:
 
         '''
         Fitness function for the optimization problem. Uses only the MCC, ignores the size penalization terms.
 
 
         :param ruleBase: RuleBase object
         :param X: array of train samples. X shape = (n_samples, n_features)
         :param y: array of train labels. y shape = (n_samples,)
         :param tolerance: float. Tolerance for the size evaluation.
         :param alpha: ignored.
         :param beta: ignored.
         :param gamma: ignored.
         :return: float. Fitness value.
         '''
-        ev_object = evr.evalRuleBase(ruleBase, X, y)
+        ev_object = evr.evalRuleBase(ruleBase, X, y, precomputed_truth=precomputed_truth)
         ev_object.add_rule_weights()
 
         score_acc = ev_object.classification_eval()
         
         return score_acc
```

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.1/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.1/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex-fuzzy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.0/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.1/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/setup.py` & `ex_fuzzy-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.0/tests/test_centroids.py` & `ex_fuzzy-1.1.1/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/tests/test_classification.py` & `ex_fuzzy-1.1.1/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/tests/test_eval_tools.py` & `ex_fuzzy-1.1.1/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.1/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.0/tests/test_utils.py` & `ex_fuzzy-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

