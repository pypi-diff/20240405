# Comparing `tmp/ex_fuzzy-1.0.7.tar.gz` & `tmp/ex_fuzzy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.0.7.tar", last modified: Wed Mar 20 14:42:14 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.0.tar", last modified: Fri Apr  5 13:45:47 2024, max compression
```

## Comparing `ex_fuzzy-1.0.7.tar` & `ex_fuzzy-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-20 14:42:14.423256 ex_fuzzy-1.0.7/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3743 2024-03-20 14:42:14.423256 ex_fuzzy-1.0.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2743 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-20 14:42:14.415256 ex_fuzzy-1.0.7/ex_fuzzy/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-20 14:42:14.419256 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      245 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6005 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10830 2024-03-20 12:37:39.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7216 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14982 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2549 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    40339 2024-03-20 12:32:13.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14404 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5981 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3589 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11211 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    36284 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26317 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24535 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15380 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-20 14:42:14.423256 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3743 2024-03-20 14:42:14.000000 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      777 2024-03-20 14:42:14.000000 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-20 14:42:14.000000 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-03-20 14:42:14.000000 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-03-20 14:42:14.000000 ex_fuzzy-1.0.7/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-20 14:42:14.423256 ex_fuzzy-1.0.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1722 2024-03-20 14:41:07.000000 ex_fuzzy-1.0.7/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-20 14:42:14.423256 ex_fuzzy-1.0.7/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1233 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/tests/test_centroids.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1907 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/tests/test_classification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      774 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/tests/test_eval_tools.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1770 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/tests/test_fuzzy_sets.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4088 2024-03-20 12:24:00.000000 ex_fuzzy-1.0.7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.972296 ex_fuzzy-1.1.0/
+-rw-rw-rw-   0        0        0     3679 2024-04-05 13:45:47.971283 ex_fuzzy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2801 2024-03-13 11:20:26.000000 ex_fuzzy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.934263 ex_fuzzy-1.1.0/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.963675 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      255 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2630 2024-04-05 13:39:34.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    42930 2024-04-05 13:22:39.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17292 2024-04-04 10:16:57.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11458 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    39187 2024-04-05 13:20:29.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25690 2024-04-05 13:35:53.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.945573 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     3679 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 13:45:47.000000 ex_fuzzy-1.1.0/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:45:47.973007 ex_fuzzy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-05 13:42:47.000000 ex_fuzzy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:45:47.970773 ex_fuzzy-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.0/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.0.7/PKG-INFO` & `ex_fuzzy-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,78 @@
-Metadata-Version: 2.1
-Name: ex_fuzzy
-Version: 1.0.7
-Summary: Library to perform explainable AI using fuzzy logic.
-Home-page: https://github.com/Fuminides/ex-fuzzy
-Download-URL: https://pypi.org/project/ex-fuzzy/
-Maintainer: Javier Fumanal Idocin
-Maintainer-email: javierfumanalidocin@gmail.com
-License: GPL-3.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: matplotlib
-Requires-Dist: pymoo
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
-
-# Ex-Fuzzy
-ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
-
-Some of the tools available in this library include:
-
-- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
-- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
-- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
-- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
-
-## Main Characteristics
-
-### Easy to use
-
-ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
-
-### Reusable code
-
-Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
-
-### Sci-py like interface
-
-ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
-
-### Visualization
-
-Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
-
-
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
-  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
-  
-</p>
-
-## Dependencies
-
-- Numpy
-- Pandas
-- Matplotlib
-- Networkx
-- Pymoo
-
-## Installation
-
-You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
-
-`pip install ex-fuzzy`
-
-
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
-
-All rights reserved, 2021-2024
-
-
+Metadata-Version: 2.1
+Name: ex_fuzzy
+Version: 1.1.0
+Summary: Library to perform explainable AI using fuzzy logic.
+Home-page: https://github.com/Fuminides/ex-fuzzy
+Download-URL: https://pypi.org/project/ex-fuzzy/
+Maintainer: Javier Fumanal Idocin
+Maintainer-email: javierfumanalidocin@gmail.com
+License: GPL-3.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+
+# Ex-Fuzzy
+ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
+
+Some of the tools available in this library include:
+
+- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
+- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
+- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
+- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
+
+## Main Characteristics
+
+### Easy to use
+
+ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
+
+### Reusable code
+
+Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
+
+### Sci-py like interface
+
+ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
+
+### Visualization
+
+Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
+
+
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
+  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
+  
+</p>
+
+## Dependencies
+
+- Numpy
+- Pandas
+- Matplotlib
+- Networkx
+- Pymoo
+
+## Installation
+
+You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
+
+`pip install ex-fuzzy`
+
+
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
+
+All rights reserved, 2021-2024
+
+
```

### Comparing `ex_fuzzy-1.0.7/README.md` & `ex_fuzzy-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# Ex-Fuzzy
-ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
-
-Some of the tools available in this library include:
-
-- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
-- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
-- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
-- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
-
-## Main Characteristics
-
-### Easy to use
-
-ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
-
-### Reusable code
-
-Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
-
-### Sci-py like interface
-
-ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
-
-### Visualization
-
-Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
-
-
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
-  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
-  
-</p>
-
-## Dependencies
-
-- Numpy
-- Pandas
-- Matplotlib
-- Networkx
-- Pymoo
-
-## Installation
-
-You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
-
-`pip install ex-fuzzy`
-
-
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
-
-All rights reserved, 2021-2024
-
-
+# Ex-Fuzzy
+ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
+
+Some of the tools available in this library include:
+
+- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
+- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
+- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
+- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
+
+## Main Characteristics
+
+### Easy to use
+
+ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
+
+### Reusable code
+
+Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
+
+### Sci-py like interface
+
+ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
+
+### Visualization
+
+Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
+
+
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
+  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
+  
+</p>
+
+## Dependencies
+
+- Numpy
+- Pandas
+- Matplotlib
+- Networkx
+- Pymoo
+
+## Installation
+
+You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
+
+`pip install ex-fuzzy`
+
+
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
+
+All rights reserved, 2021-2024
+
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-# -*- coding: utf-8 -*-
-"""
-This is the source file that contains functions to compute centroids for the case of IV fuzzy sets,
-which are commonly used when using the IV-T2 fuzzy sets.
-"""
-import numpy as np
-
-
-def center_of_masses(z: np.array, w: np.array) -> np.array:
-    '''
-    Computes the ponderated centroid with normalized weighting.
-
-    :param z: Vector of the referencial values.
-    :param w: Vector of the fuzzy memberships.
-    :return: The ponderated sum.
-    '''
-    return z @ w / np.sum(w)
-
-
-def compute_centroid_t2_l(z: np.array, memberships: np.array) -> float:
-    '''
-    Computes the Karnik and Mendel algorithm to find the centroid of an IV fuzzy set.
-
-    :param z: Vector of the referencial values.
-    :param memberships: vector of the fuzzy memberships.
-    :return: The centroid.
-    '''
-    centros = np.mean(memberships, axis=1)
-    w = centros
-
-    yhat = center_of_masses(z, w)
-
-    yhat_2 = None
-
-    while(yhat != yhat_2):
-        try:
-            k = np.argwhere((z - yhat) >= 0)[-1][0]
-            k = min(len(centros)-1, k)
-        except IndexError:
-            k = 0
-
-        # k_vector = np.argwhere((z - yhat) > 0)
-        # k = k_vector[0][0] + 1
-        w[0:k] = memberships[:, 1][:k]
-        w[k:] = memberships[:, 0][k:]
-
-        yhat_2 = yhat
-        yhat = center_of_masses(z, w)
-
-    return yhat
-
-
-def compute_centroid_t2_r(z: np.array, memberships: np.array) -> float:
-    '''
-    Computes the Karnik and Mendel algorithm to find the right component of a centroid of an IV fuzzy set.
-
-    :param z: Vector of the referencial values.
-    :param memberships: vector of the fuzzy memberships.
-    :return: The lowest membership of the centroid.
-    '''
-    centros = np.mean(memberships, axis=1)
-    w = centros
-
-    yhat = center_of_masses(z, w)
-
-    yhat_2 = None
-
-    while(yhat != yhat_2):
-        try:
-            k = np.argwhere((z - yhat) >= 0)[-1][0]
-            k = min(len(centros)-1, k)
-        except IndexError:
-            k = 0
-
-        w[0:k+1] = memberships[:, 0][:k+1]
-        w[k+1:] = memberships[:, 1][k+1:]
-
-        yhat_2 = yhat
-        yhat = center_of_masses(z, w)
-
-    return yhat
-
-
-def consequent_centroid_r(antecedent_memberships: np.array, centroids_r: np.array) -> float:
-    '''
-    Computes the Karnik and Mendel algorithm to find the right component of a centroid of an IV fuzzy set
-    using the centroids of the consequents and the antecedents memeberships.
-
-    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
-    :param centroids_r: M sized vector. Contains the referencial values.
-    :return: the IV centroid.
-    '''
-
-    memberships_left = antecedent_memberships[:, 0]
-    memberships_right = antecedent_memberships[:, 1]
-    initial_f = (memberships_left + memberships_right) / 2
-
-    yhat = center_of_masses(centroids_r, initial_f)
-    yhat2 = None
-
-    while(yhat != yhat2):
-        try:
-            r_R = np.argwhere((yhat - centroids_r) >= 0)[-1][0]
-            r_R = min(len(centroids_r)-1, r_R)
-        except IndexError:
-            r_R = 0
-
-        new_memberships = initial_f
-        new_memberships[0:r_R+1] = memberships_left[0:r_R+1]
-        new_memberships[r_R+1:] = memberships_right[r_R+1:]
-
-        yhat2 = yhat
-        if np.sum(new_memberships) == 0:
-            yhat = 0
-        else:
-            yhat = center_of_masses(centroids_r, new_memberships)
-
-    return yhat2
-
-
-def consequent_centroid_l(antecedent_memberships: np.array, centroids_l: np.array) -> float:
-    '''
-    Computes the Karnik and Mendel algorithm to find the left component of a centroid of an IV fuzzy set
-    using the centroids of the consequents and the antecedent memberships.
-
-    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
-    :param centroids_r: M sized vector. Contains the referencial values.
-    :return: the IV centroid.
-    '''
-
-    memberships_left = antecedent_memberships[:, 0]
-    memberships_right = antecedent_memberships[:, 1]
-    initial_f = (memberships_left + memberships_right) / 2
-
-    # (memberships_right * centroids_r) / np.sum(memberships_right)
-    yhat = center_of_masses(centroids_l, initial_f)
-    yhat2 = -100
-
-    #R = np.where(yhat - centroids_r)[0]
-    while(yhat != yhat2):
-        try:
-            r_R = np.argwhere((yhat - centroids_l) >= 0)[-1][0]
-            r_R = min(len(centroids_l)-1, r_R)
-        except IndexError:
-            r_R = 0
-
-        new_memberships = initial_f
-        new_memberships[0:r_R+1] = memberships_right[0:r_R+1]
-        new_memberships[r_R+1:] = memberships_left[r_R+1:]
-        yhat2 = yhat
-        if np.sum(new_memberships) == 0:
-            yhat = 0
-        else:
-            yhat = center_of_masses(centroids_l, new_memberships)
-
-    return yhat2
-
-
-def compute_centroid_iv(z: np.array, memberships: np.array) -> np.array:
-    '''
-    Computes Karnik and Mendel algorithm to find the centroid of a iv fuzzy set. 
-
-    :param z: Vector of the referencial values.
-    :param memberships: vector of the fuzzy memberships.
-    :return: The centroid.
-    '''
-    res = np.zeros((2,))
-    res[0] = compute_centroid_t2_l(z, memberships)
-    res[1] = compute_centroid_t2_r(z, memberships)
-    return res
-
-
-def consequent_centroid(antecedent_memberships: np.array, centroids: np.array) -> np.array:
-    '''
-    Computes Karnik and Mendel algorithm to find the centroid of a consequent iv fuzzy set given the centroids of the consequents
-    and the antecedents memberships. 
-
-    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
-    :param centroids: M x 2 matrix. M rules and iv dimension (2). Vector of centroids.
-    :return: The centroid.
-    '''
-    centroids_l = centroids[:, 0]
-    centroids_r = centroids[:, 1]
-    res = np.zeros((2,))
-
-    res[0] = consequent_centroid_l(antecedent_memberships, centroids_l)
-    res[1] = consequent_centroid_r(antecedent_memberships, centroids_r)
-
-    return res
-
-
-
+# -*- coding: utf-8 -*-
+"""
+This is the source file that contains functions to compute centroids for the case of IV fuzzy sets,
+which are commonly used when using the IV-T2 fuzzy sets.
+"""
+import numpy as np
+
+
+def center_of_masses(z: np.array, w: np.array) -> np.array:
+    '''
+    Computes the ponderated centroid with normalized weighting.
+
+    :param z: Vector of the referencial values.
+    :param w: Vector of the fuzzy memberships.
+    :return: The ponderated sum.
+    '''
+    return z @ w / np.sum(w)
+
+
+def compute_centroid_t2_l(z: np.array, memberships: np.array) -> float:
+    '''
+    Computes the Karnik and Mendel algorithm to find the centroid of an IV fuzzy set.
+
+    :param z: Vector of the referencial values.
+    :param memberships: vector of the fuzzy memberships.
+    :return: The centroid.
+    '''
+    centros = np.mean(memberships, axis=1)
+    w = centros
+
+    yhat = center_of_masses(z, w)
+
+    yhat_2 = None
+
+    while(yhat != yhat_2):
+        try:
+            k = np.argwhere((z - yhat) >= 0)[-1][0]
+            k = min(len(centros)-1, k)
+        except IndexError:
+            k = 0
+
+        # k_vector = np.argwhere((z - yhat) > 0)
+        # k = k_vector[0][0] + 1
+        w[0:k] = memberships[:, 1][:k]
+        w[k:] = memberships[:, 0][k:]
+
+        yhat_2 = yhat
+        yhat = center_of_masses(z, w)
+
+    return yhat
+
+
+def compute_centroid_t2_r(z: np.array, memberships: np.array) -> float:
+    '''
+    Computes the Karnik and Mendel algorithm to find the right component of a centroid of an IV fuzzy set.
+
+    :param z: Vector of the referencial values.
+    :param memberships: vector of the fuzzy memberships.
+    :return: The lowest membership of the centroid.
+    '''
+    centros = np.mean(memberships, axis=1)
+    w = centros
+
+    yhat = center_of_masses(z, w)
+
+    yhat_2 = None
+
+    while(yhat != yhat_2):
+        try:
+            k = np.argwhere((z - yhat) >= 0)[-1][0]
+            k = min(len(centros)-1, k)
+        except IndexError:
+            k = 0
+
+        w[0:k+1] = memberships[:, 0][:k+1]
+        w[k+1:] = memberships[:, 1][k+1:]
+
+        yhat_2 = yhat
+        yhat = center_of_masses(z, w)
+
+    return yhat
+
+
+def consequent_centroid_r(antecedent_memberships: np.array, centroids_r: np.array) -> float:
+    '''
+    Computes the Karnik and Mendel algorithm to find the right component of a centroid of an IV fuzzy set
+    using the centroids of the consequents and the antecedents memeberships.
+
+    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
+    :param centroids_r: M sized vector. Contains the referencial values.
+    :return: the IV centroid.
+    '''
+
+    memberships_left = antecedent_memberships[:, 0]
+    memberships_right = antecedent_memberships[:, 1]
+    initial_f = (memberships_left + memberships_right) / 2
+
+    yhat = center_of_masses(centroids_r, initial_f)
+    yhat2 = None
+
+    while(yhat != yhat2):
+        try:
+            r_R = np.argwhere((yhat - centroids_r) >= 0)[-1][0]
+            r_R = min(len(centroids_r)-1, r_R)
+        except IndexError:
+            r_R = 0
+
+        new_memberships = initial_f
+        new_memberships[0:r_R+1] = memberships_left[0:r_R+1]
+        new_memberships[r_R+1:] = memberships_right[r_R+1:]
+
+        yhat2 = yhat
+        if np.sum(new_memberships) == 0:
+            yhat = 0
+        else:
+            yhat = center_of_masses(centroids_r, new_memberships)
+
+    return yhat2
+
+
+def consequent_centroid_l(antecedent_memberships: np.array, centroids_l: np.array) -> float:
+    '''
+    Computes the Karnik and Mendel algorithm to find the left component of a centroid of an IV fuzzy set
+    using the centroids of the consequents and the antecedent memberships.
+
+    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
+    :param centroids_r: M sized vector. Contains the referencial values.
+    :return: the IV centroid.
+    '''
+
+    memberships_left = antecedent_memberships[:, 0]
+    memberships_right = antecedent_memberships[:, 1]
+    initial_f = (memberships_left + memberships_right) / 2
+
+    # (memberships_right * centroids_r) / np.sum(memberships_right)
+    yhat = center_of_masses(centroids_l, initial_f)
+    yhat2 = -100
+
+    #R = np.where(yhat - centroids_r)[0]
+    while(yhat != yhat2):
+        try:
+            r_R = np.argwhere((yhat - centroids_l) >= 0)[-1][0]
+            r_R = min(len(centroids_l)-1, r_R)
+        except IndexError:
+            r_R = 0
+
+        new_memberships = initial_f
+        new_memberships[0:r_R+1] = memberships_right[0:r_R+1]
+        new_memberships[r_R+1:] = memberships_left[r_R+1:]
+        yhat2 = yhat
+        if np.sum(new_memberships) == 0:
+            yhat = 0
+        else:
+            yhat = center_of_masses(centroids_l, new_memberships)
+
+    return yhat2
+
+
+def compute_centroid_iv(z: np.array, memberships: np.array) -> np.array:
+    '''
+    Computes Karnik and Mendel algorithm to find the centroid of a iv fuzzy set. 
+
+    :param z: Vector of the referencial values.
+    :param memberships: vector of the fuzzy memberships.
+    :return: The centroid.
+    '''
+    res = np.zeros((2,))
+    res[0] = compute_centroid_t2_l(z, memberships)
+    res[1] = compute_centroid_t2_r(z, memberships)
+    return res
+
+
+def consequent_centroid(antecedent_memberships: np.array, centroids: np.array) -> np.array:
+    '''
+    Computes Karnik and Mendel algorithm to find the centroid of a consequent iv fuzzy set given the centroids of the consequents
+    and the antecedents memberships. 
+
+    :param antecedent_memberships: M x 2 matrix. M rules and iv dimension (2). Vector of memberships.
+    :param centroids: M x 2 matrix. M rules and iv dimension (2). Vector of centroids.
+    :return: The centroid.
+    '''
+    centroids_l = centroids[:, 0]
+    centroids_r = centroids[:, 1]
+    res = np.zeros((2,))
+
+    res[0] = consequent_centroid_l(antecedent_memberships, centroids_l)
+    res[1] = consequent_centroid_r(antecedent_memberships, centroids_r)
+
+    return res
+
+
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,212 +1,209 @@
-'''
-Module that contains classifiers that uses two step genetic optimization and rule mining based on the support of the candidate rules. 
-
-'''
-
-import numpy as np
-from sklearn.base import ClassifierMixin
-
-try:
-    from . import fuzzy_sets as fs
-    from . import evolutionary_fit as evf
-    from . import rule_mining as rm
-    from . import utils
-    from . import maintenance as mnt
-except:
-    import fuzzy_sets as fs
-    import evolutionary_fit as evf
-    import rule_mining as rm
-    import utils
-    import maintenance as mnt
-
-
-class RuleMineClassifier(ClassifierMixin):
-    """A classifier that works by mining a set of candidate rules with a minimum support, confidence and lift, and then using a genetic algorithm that chooses
-    the optimal combination of those rules."""
-
-    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0,
-                verbose=False, n_class: int=None, runner: int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
-        '''
-        Inits the optimizer with the corresponding parameters.
-
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param tolerance: tolerance for the support/dominance score of the rules.
-        :param verbose: if True, prints the progress of the optimization.
-        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
-        :param runner: number of threads to use.
-        :param linguistic_variables: linguistic variables per antecedent.
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.Classification]['data_mining'] += 1
-        
-        self.nAnts = nAnts
-        self.fl_classifier = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, 
-                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
-        self.fuzzy_type = fuzzy_type
-        self.tolerance = tolerance
-
-
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, random_seed:int=33):
-        '''
-        Trains the model with the given data.
-
-        :param X: samples to train.
-        :param y: labels for each sample.
-        :param random_seed: random seed for reproducibility. It is pased to the optimization algorithm.
-        '''
-        fuzzy_vars = utils.construct_partitions(X, self.fuzzy_type)
-        candidate_rules = rm.multiclass_mine_rulebase(X, y, fuzzy_vars, self.tolerance, max_depth=self.nAnts)
-        self.fl_classifier.fit(X, y, checkpoints=0, candidate_rules=candidate_rules, n_gen=n_gen, pop_size=pop_size, random_seed=random_seed)
-
-
-    def predict(self, X: np.array) -> np.array:
-        '''
-        Predict for each sample the corresponding class.
-
-        :param X: samples to predict.
-        :return: a class for each sample.
-        '''
-        # Make predictions using the fitted model
-        y_pred = self.fl_classifier.predict(X)
-
-        return y_pred
-    
-
-    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
-        # Returns the classifier that performs the final predictions
-        return self.fl_classifier
-    
-
-
-class FuzzyRulesClassifier(ClassifierMixin):
-    """A classifier that works by performing a double optimization process. First, it creates a candidate rule base using genetic optimization
-    and then uses it as a basis to obtain a better one that satisfies the constrain of antecedents and number of rules."""
-
-    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0, 
-                 verbose=False, n_class: int=None, runner: int=1, expansion_factor:int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
-        '''
-        Inits the optimizer with the corresponding parameters.
-
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param tolerance: tolerance for the dominance score of the rules.
-        :param verbose: if True, prints the progress of the optimization.
-        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
-        :param runner: number of threads to use.
-        :param expansion_factor: if > 1, it will compute inthe first optimization process n times the nRules parameters. (So that the search space for the second step is bigger)
-        :param linguistic_variables: linguistic variables per antecedent.
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.Classification]['double_go'] += 1
-
-
-        self.fl_classifier1 = evf.BaseFuzzyRulesClassifier(nRules=nRules* expansion_factor, linguistic_variables=linguistic_variables, nAnts=nAnts, # We give this one more number rules so that then the second optimization has a bigger search space
-                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
-        self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
-                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
-        self.fuzzy_type = fuzzy_type
-        self.tolerance = tolerance
-
-
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, random_seed:int=33):
-        '''
-        Trains the model with the given data.
-
-        :param X: samples to train.
-        :param y: labels for each sample.
-        :param n_gen: number of generations to compute in the genetic optimization.
-        :param pop_size: number of subjects per generation.
-        :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
-        :param n_runner: number of threds to use.
-        :param random_seed: random seed for reproducibility. It is pased to the optimization algorithm.
-        '''
-        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, random_seed=random_seed)
-        self.phase1_rules = self.fl_classifier1.rule_base
-        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules, random_seed=random_seed)
-        
-
-    def predict(self, X: np.array) -> np.array:
-        '''
-        Predcit for each sample the correspondent class.
-
-        :param X: samples to predict.
-        :return: a class for each sample.
-        '''
-        # Make predictions using the fitted model
-        y_pred = self.fl_classifier2.predict(X)
-
-        return y_pred
-    
-
-    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
-        # Returns the classifier that performs the final predictions
-        return self.fl_classifier2
-    
-
-class RuleFineTuneClassifier(ClassifierMixin):
-    """A classifier that works by mining a set of candidate rules with a minimum support and then uses a two step genetic optimization that chooses
-    the optimal combination of those rules and fine tunes them."""
-
-    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0, 
-                 verbose=False, n_class: int=None, runner: int=1, expansion_factor:int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
-        '''
-        Inits the optimizer with the corresponding parameters.
-
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param tolerance: tolerance for the dominance score of the rules.
-        :param verbose: if True, prints the progress of the optimization.
-        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
-        :param linguistic_variables: linguistic variables per antecedent.
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.Classification]['double_go'] += 1
-            mnt.usage_data[mnt.usage_categories.Classification]['data_mining'] += 1
-
-        self.fl_classifier1 = evf.BaseFuzzyRulesClassifier(nRules=nRules* expansion_factor, linguistic_variables=linguistic_variables, nAnts=nAnts, # We give this one more number rules so that then the second optimization has a bigger search space
-                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
-        self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
-                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
-        self.fuzzy_type = fuzzy_type
-        self.tolerance = tolerance
-
-
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, n_runner:int=1, random_seed:int=33):
-        '''
-        Trains the model with the given data.
-
-        :param X: samples to train.
-        :param y: labels for each sample.
-        :param n_gen: number of generations to compute in the genetic optimization.
-        :param pop_size: number of subjects per generation.
-        :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
-        :param n_runner: number of threds to use.
-        :param random_seed: random seed for reproducibility. It is pased to the optimization algorithm.
-        '''
-        candidate_rules = rm.multiclass_mine_rulebase(X, y, self.fl_classifier1.lvs, self.tolerance)
-
-        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, candidate_rules=candidate_rules, random_seed=random_seed)
-        self.phase1_rules = self.fl_classifier1.rule_base
-        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules, random_seed=random_seed)
-
-
-    def predict(self, X: np.array) -> np.array:
-        '''
-        Predcit for each sample the correspondent class.
-
-        :param X: samples to predict.
-        :return: a class for each sample.
-        '''
-        # Make predictions using the fitted model
-        y_pred = self.fl_classifier.predict(X)
-
-        return y_pred
-    
-
-    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
-        # Returns the classifier that performs the final predictions
+'''
+Module that contains classifiers that uses two step genetic optimization and rule mining based on the support of the candidate rules. 
+
+'''
+
+import numpy as np
+from sklearn.base import ClassifierMixin
+
+try:
+    from . import fuzzy_sets as fs
+    from . import evolutionary_fit as evf
+    from . import rule_mining as rm
+    from . import utils
+    from . import maintenance as mnt
+except:
+    import fuzzy_sets as fs
+    import evolutionary_fit as evf
+    import rule_mining as rm
+    import utils
+    import maintenance as mnt
+
+
+class RuleMineClassifier(ClassifierMixin):
+    """A classifier that works by mining a set of candidate rules with a minimum support, confidence and lift, and then using a genetic algorithm that chooses
+    the optimal combination of those rules."""
+
+    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0,
+                verbose=False, n_class: int=None, runner: int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
+        '''
+        Inits the optimizer with the corresponding parameters.
+
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param tolerance: tolerance for the support/dominance score of the rules.
+        :param verbose: if True, prints the progress of the optimization.
+        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
+        :param runner: number of threads to use.
+        :param linguistic_variables: linguistic variables per antecedent.
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.Classification]['data_mining'] += 1
+        
+        self.nAnts = nAnts
+        self.fl_classifier = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, 
+                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
+        self.fuzzy_type = fuzzy_type
+        self.tolerance = tolerance
+
+
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50):
+        '''
+        Trains the model with the given data.
+
+        :param X: samples to train.
+        :param y: labels for each sample.
+        '''
+        fuzzy_vars = utils.construct_partitions(X, self.fuzzy_type)
+        candidate_rules = rm.multiclass_mine_rulebase(X, y, fuzzy_vars, self.tolerance, max_depth=self.nAnts)
+        self.fl_classifier.fit(X, y, checkpoints=0, candidate_rules=candidate_rules, n_gen=n_gen, pop_size=pop_size)
+
+
+    def predict(self, X: np.array) -> np.array:
+        '''
+        Predict for each sample the corresponding class.
+
+        :param X: samples to predict.
+        :return: a class for each sample.
+        '''
+        # Make predictions using the fitted model
+        y_pred = self.fl_classifier.predict(X)
+
+        return y_pred
+    
+
+    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
+        # Returns the classifier that performs the final predictions
+        return self.fl_classifier
+    
+
+
+class FuzzyRulesClassifier(ClassifierMixin):
+    """A classifier that works by performing a double optimization process. First, it creates a candidate rule base using genetic optimization
+    and then uses it as a basis to obtain a better one that satisfies the constrain of antecedents and number of rules."""
+
+    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0, 
+                 verbose=False, n_class: int=None, runner: int=1, expansion_factor:int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
+        '''
+        Inits the optimizer with the corresponding parameters.
+
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param tolerance: tolerance for the dominance score of the rules.
+        :param verbose: if True, prints the progress of the optimization.
+        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
+        :param runner: number of threads to use.
+        :param expansion_factor: if > 1, it will compute inthe first optimization process n times the nRules parameters. (So that the search space for the second step is bigger)
+        :param linguistic_variables: linguistic variables per antecedent.
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.Classification]['double_go'] += 1
+
+
+        self.fl_classifier1 = evf.BaseFuzzyRulesClassifier(nRules=nRules* expansion_factor, linguistic_variables=linguistic_variables, nAnts=nAnts, # We give this one more number rules so that then the second optimization has a bigger search space
+                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
+        self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
+                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
+        self.fuzzy_type = fuzzy_type
+        self.tolerance = tolerance
+
+
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0):
+        '''
+        Trains the model with the given data.
+
+        :param X: samples to train.
+        :param y: labels for each sample.
+        :param n_gen: number of generations to compute in the genetic optimization.
+        :param pop_size: number of subjects per generation.
+        :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
+        :param n_runner: number of threds to use.
+        '''
+        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints)
+        self.phase1_rules = self.fl_classifier1.rule_base
+        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules)
+        
+
+    def predict(self, X: np.array) -> np.array:
+        '''
+        Predcit for each sample the correspondent class.
+
+        :param X: samples to predict.
+        :return: a class for each sample.
+        '''
+        # Make predictions using the fitted model
+        y_pred = self.fl_classifier2.predict(X)
+
+        return y_pred
+    
+
+    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
+        # Returns the classifier that performs the final predictions
+        return self.fl_classifier2
+    
+
+class RuleFineTuneClassifier(ClassifierMixin):
+    """A classifier that works by mining a set of candidate rules with a minimum support and then uses a two step genetic optimization that chooses
+    the optimal combination of those rules and fine tunes them."""
+
+    def __init__(self, nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0, 
+                 verbose=False, n_class: int=None, runner: int=1, expansion_factor:int=1, linguistic_variables: list[fs.fuzzyVariable]=None) -> None:
+        '''
+        Inits the optimizer with the corresponding parameters.
+
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param tolerance: tolerance for the dominance score of the rules.
+        :param verbose: if True, prints the progress of the optimization.
+        :param n_class: number of classes in the problem. If None (default) the classifier will compute it empirically.
+        :param linguistic_variables: linguistic variables per antecedent.
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.Classification]['double_go'] += 1
+            mnt.usage_data[mnt.usage_categories.Classification]['data_mining'] += 1
+
+        self.fl_classifier1 = evf.BaseFuzzyRulesClassifier(nRules=nRules* expansion_factor, linguistic_variables=linguistic_variables, nAnts=nAnts, # We give this one more number rules so that then the second optimization has a bigger search space
+                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
+        self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
+                                            fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
+        self.fuzzy_type = fuzzy_type
+        self.tolerance = tolerance
+
+
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, n_runner:int=1):
+        '''
+        Trains the model with the given data.
+
+        :param X: samples to train.
+        :param y: labels for each sample.
+        :param n_gen: number of generations to compute in the genetic optimization.
+        :param pop_size: number of subjects per generation.
+        :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
+        :param n_runner: number of threds to use.
+        '''
+        candidate_rules = rm.multiclass_mine_rulebase(X, y, self.fl_classifier1.lvs, self.tolerance)
+
+        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, candidate_rules=candidate_rules)
+        self.phase1_rules = self.fl_classifier1.rule_base
+        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules)
+
+
+    def predict(self, X: np.array) -> np.array:
+        '''
+        Predcit for each sample the correspondent class.
+
+        :param X: samples to predict.
+        :return: a class for each sample.
+        '''
+        # Make predictions using the fitted model
+        y_pred = self.fl_classifier.predict(X)
+
+        return y_pred
+    
+
+    def internal_classifier(self) -> evf.BaseFuzzyRulesClassifier:
+        # Returns the classifier that performs the final predictions
         return self.fl_classifier2
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-"""
-Functions that contain some general functions to eval already fitted fuzzy rule based models.
-It can also be used to visualize rules and fuzzy partitions.
-"""
-import numpy as np
-import pandas as pd
-from sklearn.metrics import matthews_corrcoef
-
-try:
-      from . import evolutionary_fit as evf
-      from . import vis_rules
-except ImportError:
-      import evolutionary_fit as evf
-      import vis_rules
-
-
-def eval_fuzzy_model(fl_classifier: evf.BaseFuzzyRulesClassifier, X_train: np.array, y_train: np.array,
-                     X_test: np.array, y_test: np.array, plot_rules=True, print_rules=True, plot_partitions=True, 
-                     return_rules=False, print_accuracy=True, print_matthew=True, export_path:str=None) -> None:
-    '''
-    Function that evaluates a fuzzy rule based model. It also plots the rules and the fuzzy partitions.
-
-    :param fl_classifier: Fuzzy rule based model.
-    :param X_train: Training data.
-    :param y_train: Training labels.
-    :param X_test: Test data.
-    :param y_test: Test labels.
-    :param plot_rules: If True, it plots the rules.
-    :param print_rules: If True, it prints the rules.
-    :param plot_partitions: If True, it plots the fuzzy partitions.
-    :return: None
-    '''
-    # Get the unique classes from the classifier
-    unique_classes = fl_classifier.classes_
-    # Convert the names from the labels to the corresponding class
-    y_train = np.array([list(unique_classes).index(str(y)) for y in y_train])
-    y_test = np.array([list(unique_classes).index(str(y)) for y in y_test])
-    
-    if print_accuracy:
-      print('------------')
-      print('ACCURACY')
-      print('Train performance: ' +
-            str(np.mean(np.equal(y_train, fl_classifier.predict(X_train)))))
-      print('Test performance: ' +
-            str(np.mean(np.equal(y_test, fl_classifier.predict(X_test)))))
-      print('------------')
-    if print_matthew:
-      print('MATTHEW CORRCOEF')
-      print('Train performance: ' +
-            str(matthews_corrcoef(y_train, fl_classifier.predict(X_train))))
-      print('Test performance: ' +
-            str(matthews_corrcoef(y_test, fl_classifier.predict(X_test))))
-      print('------------')
-
-    if plot_rules:
-        vis_rules.visualize_rulebase(fl_classifier.rule_base, export_path=export_path)
-    if print_rules or return_rules:
-        res = fl_classifier.print_rules(return_rules)
-
-        if print_rules:
-            print(res)
-
-    if plot_partitions:
-        fl_classifier.plot_fuzzy_variables()
-
-    if return_rules:
-        return res
+"""
+Functions that contain some general functions to eval already fitted fuzzy rule based models.
+It can also be used to visualize rules and fuzzy partitions.
+"""
+import numpy as np
+import pandas as pd
+from sklearn.metrics import matthews_corrcoef
+
+try:
+      from . import evolutionary_fit as evf
+      from . import vis_rules
+except ImportError:
+      import evolutionary_fit as evf
+      import vis_rules
+
+
+def eval_fuzzy_model(fl_classifier: evf.BaseFuzzyRulesClassifier, X_train: np.array, y_train: np.array,
+                     X_test: np.array, y_test: np.array, plot_rules=True, print_rules=True, plot_partitions=True, 
+                     return_rules=False, print_accuracy=True, print_matthew=True, export_path:str=None) -> None:
+    '''
+    Function that evaluates a fuzzy rule based model. It also plots the rules and the fuzzy partitions.
+
+    :param fl_classifier: Fuzzy rule based model.
+    :param X_train: Training data.
+    :param y_train: Training labels.
+    :param X_test: Test data.
+    :param y_test: Test labels.
+    :param plot_rules: If True, it plots the rules.
+    :param print_rules: If True, it prints the rules.
+    :param plot_partitions: If True, it plots the fuzzy partitions.
+    :return: None
+    '''
+    # Get the unique classes from the classifier
+    unique_classes = fl_classifier.classes_
+    # Convert the names from the labels to the corresponding class
+    y_train = np.array([list(unique_classes).index(str(y)) for y in y_train])
+    y_test = np.array([list(unique_classes).index(str(y)) for y in y_test])
+    
+    if print_accuracy:
+      print('------------')
+      print('ACCURACY')
+      print('Train performance: ' +
+            str(np.mean(np.equal(y_train, fl_classifier.predict(X_train)))))
+      print('Test performance: ' +
+            str(np.mean(np.equal(y_test, fl_classifier.predict(X_test)))))
+      print('------------')
+    if print_matthew:
+      print('MATTHEW CORRCOEF')
+      print('Train performance: ' +
+            str(matthews_corrcoef(y_train, fl_classifier.predict(X_train))))
+      print('Test performance: ' +
+            str(matthews_corrcoef(y_test, fl_classifier.predict(X_test))))
+      print('------------')
+
+
+    if print_rules or return_rules:
+        res = fl_classifier.print_rules(return_rules)
+
+        if print_rules:
+            print(res)
+
+    if plot_partitions:
+        fl_classifier.plot_fuzzy_variables()
+
+    if plot_rules:
+        vis_rules.visualize_rulebase(fl_classifier.rule_base, export_path=export_path)
+    if return_rules:
+        return res
+    
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,919 +1,947 @@
-"""
-This is a the source file that contains the class to train/fit the rulebase using a genetic algorithm.
-
-"""
-import numpy as np
-import pandas as pd
-
-from sklearn.model_selection import StratifiedKFold
-from sklearn.metrics import matthews_corrcoef
-from sklearn.base import ClassifierMixin
-from pymoo.algorithms.soo.nonconvex.ga import GA
-from pymoo.core.problem import Problem
-from pymoo.optimize import minimize
-from pymoo.operators.sampling.rnd import IntegerRandomSampling
-from pymoo.operators.crossover.sbx import SBX
-from pymoo.operators.mutation.pm import PolynomialMutation
-from pymoo.core.variable import Integer
-from multiprocessing.pool import ThreadPool
-from pymoo.core.problem import StarmapParallelization
-
-try:
-    from . import fuzzy_sets as fs
-    from . import rules
-    from . import eval_rules as evr
-    from . import vis_rules
-    from . import maintenance as mnt
-except ImportError:
-    import fuzzy_sets as fs
-    import rules
-    import eval_rules as evr
-    import vis_rules
-    import maintenance as mnt
-
-
-
-class BaseFuzzyRulesClassifier(ClassifierMixin):
-    '''
-    Class that is used as a classifier for a fuzzy rule based system. Supports precomputed and optimization of the linguistic variables.
-    '''
-
-    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = fs.FUZZY_SETS.t1, tolerance: float = 0.0,
-                 n_linguist_variables: int = 3, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
-                 domain: list[float] = None, n_class: int=None, precomputed_rules: rules.MasterRuleBase =None, runner: int=1) -> None:
-        '''
-        Inits the optimizer with the corresponding parameters.
-
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param tolerance: tolerance for the dominance score of the rules.
-        :param n_linguist_variables: number of linguistic variables per antecedent.
-        :param verbose: if True, prints the progress of the optimization.
-        :param linguistic_variables: list of fuzzyVariables type. If None (default) the optimization process will init+optimize them.
-        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
-        :param n_class: names of the classes in the problem. If None (default) the classifier will compute it empirically.
-        :param precomputed_rules: MasterRuleBase object. If not None, the classifier will use the rules in the object and ignore the conflicting parameters.
-        :param runner: number of threads to use. If None (default) the classifier will use 1 thread.
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
-
-        if precomputed_rules is not None:
-            self.nRules = len(precomputed_rules.get_rules())
-            self.nAnts = len(precomputed_rules.get_rules()[0].antecedents)
-            self.n_class = len(precomputed_rules)
-            self.classes_ = precomputed_rules.consequent_names
-            self.rule_base = precomputed_rules
-        else:
-            self.nRules = nRules
-            self.nAnts = nAnts
-            self.classes_ = n_class
-
-        self.custom_loss = None
-        self.verbose = verbose
-        self.tolerance = tolerance
-        
-
-        if runner > 1:
-            pool = ThreadPool(runner)
-            self.thread_runner = StarmapParallelization(pool.starmap)
-        else:
-            self.thread_runner = None
-        
-        if linguistic_variables is not None:
-            if mnt.save_usage_flag:
-                mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
-            # If the linguistic variables are precomputed then we act accordingly
-            self.lvs = linguistic_variables
-            self.n_linguist_variables = len(
-                self.lvs[0].linguistic_variable_names())
-            self.domain = None
-            self.fuzzy_type = self.lvs[0].fuzzy_type()
-        else:
-            if mnt.save_usage_flag:
-                mnt.usage_data[mnt.usage_categories.Funcs]['opt_labels'] += 1
-
-            # If not, then we need the parameters sumistered by the user.
-            self.lvs = None
-            self.fuzzy_type = fuzzy_type
-            self.n_linguist_variables = n_linguist_variables
-            self.domain = domain
-
-        self.alpha_ = 0.950
-        self.beta_ = 0.025
-        self.gamma_ = 0.025
-
-    def customized_loss(self, loss_function):
-        '''
-        Function to customize the loss function used for the optimization.
-
-        :param loss_function: function that takes as input the true labels and the predicted labels and returns a float.
-        :return: None
-        '''
-        self.custom_loss = loss_function
-
-
-    def fit(self, X: np.array, y: np.array, n_gen:int=70, pop_size:int=30,
-            checkpoints:int=0, candidate_rules:rules.MasterRuleBase=None, initial_rules:rules.MasterRuleBase=None,
-            random_seed:int=33):
-        '''
-        Fits a fuzzy rule based classifier using a genetic algorithm to the given data.
-
-        :param X: numpy array samples x features
-        :param y: labels. integer array samples (x 1)
-        :param n_gen: integer. Number of generations to run the genetic algorithm.
-        :param pop_size: integer. Population size for each gneration.
-        :param checkpoints: integer. Number of checkpoints to save the best rulebase found so far.
-        :param candidate_rules: if these rules exist, the optimization process will choose the best rules from this set. If None (default) the rules will be generated from scratch.
-        :return: None. The classifier is fitted to the data.
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
-            
-        if self.classes_ is None:
-            if isinstance(y, pd.Series):
-                self.classes_ = [str(aux) for aux in y.unique()]
-                # Convert the names in the label vector to integer classes
-                y = np.array(y.replace(self.classes_, np.arange(len(self.classes_))))
-            else:
-                self.classes_ = [str(aux) for aux in np.unique(y)]
-            
-        if candidate_rules is None:
-            if initial_rules is not None:
-                self.fuzzy_type = initial_rules.fuzzy_type()
-                self.n_linguist_variables = initial_rules.n_linguist_variables()
-                self.domain = [fv.domain for fv in initial_rules[0].antecedents]
-                self.nRules = len(initial_rules.get_rules())
-                self.nAnts = len(initial_rules.get_rules()[0].antecedents)
-
-            if self.lvs is None:
-                # If Fuzzy variables need to be optimized.
-                problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, tolerance=self.tolerance, n_classes=len(np.unique(y)),
-                                    n_linguist_variables=self.n_linguist_variables, fuzzy_type=self.fuzzy_type, domain=self.domain, thread_runner=self.thread_runner,
-                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
-            else:
-                # If Fuzzy variables are already precomputed.
-                problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, n_classes=len(np.unique(y)),
-                                    linguistic_variables=self.lvs, domain=self.domain, tolerance=self.tolerance, thread_runner=self.thread_runner,
-                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
-        else:
-            self.fuzzy_type = candidate_rules.fuzzy_type()
-            self.n_linguist_variables = candidate_rules.n_linguist_variables()
-            problem = ExploreRuleBases(X, y, n_classes=len(np.unique(y)), cancidate_rules=candidate_rules, thread_runner=self.thread_runner, nRules=self.nRules)
-
-        if self.custom_loss is not None:
-            problem.fitness_func = self.custom_loss
-
-        if initial_rules is not None:
-            rules_gene = problem.encode_rulebase(initial_rules, self.lvs is None)
-            rules_gene = (np.ones((pop_size, len(rules_gene))) * rules_gene).astype(int)
-        else:
-            rules_gene = IntegerRandomSampling()
-
-        algorithm = GA(
-            pop_size=pop_size,
-            crossover=SBX(prob=.3, eta=3.0),
-            mutation=PolynomialMutation(eta=7.0),
-            sampling=rules_gene,
-            eliminate_duplicates=False)
-        
-
-        if checkpoints > 0:
-            if self.verbose:
-                print('=================================================')
-                print('n_gen  |  n_eval  |     f_avg     |     f_min    ')
-                print('=================================================')
-            algorithm.setup(problem, seed=random_seed, termination=('n_gen', n_gen)) # 33? Soon...
-            for k in range(n_gen):
-                algorithm.next()
-                res = algorithm
-                if self.verbose:
-                    print('%-6s | %-8s | %-8s | %-8s' % (res.n_gen, res.evaluator.n_eval, res.pop.get('F').mean(), res.pop.get('F').min()))
-                if k % checkpoints == 0:
-                    with open("checkpoint_" + str(algorithm.n_gen), "w") as f:
-                        pop = algorithm.pop
-                        fitness_last_gen = pop.get('F')
-                        best_solution_arg = np.argmin(fitness_last_gen)
-                        best_individual = pop.get('X')[best_solution_arg, :]
-
-                        rule_base = problem._construct_ruleBase(
-                            best_individual, self.fuzzy_type)
-                        eval_performance = evr.evalRuleBase(
-                            rule_base, np.array(X), y)
-                        
-                        eval_performance.add_full_evaluation()  
-                        # self.rename_fuzzy_variables() This wont work on checkpoints!
-                        rule_base.purge_rules(self.tolerance)
-                        rule_base.rename_cons(self.classes_)
-                        checkpoint_rules = rule_base.print_rules(True)
-                        f.write(checkpoint_rules)     
-
-        else:
-            res = minimize(problem,
-                        algorithm,
-                        # termination,
-                        ("n_gen", n_gen),
-                        copy_algorithm=False,
-                        save_history=False,
-                        seed=random_seed,
-                        verbose=self.verbose)
-        
-        pop = res.pop
-        fitness_last_gen = pop.get('F')
-        best_solution = np.argmin(fitness_last_gen)
-        best_individual = pop.get('X')[best_solution, :]
-
-        
-        self.performance = 1 - fitness_last_gen[best_solution]
-
-        try:
-            self.var_names = list(X.columns)
-            self.X = X.values
-        except AttributeError:
-            self.X = X
-            self.var_names = [str(ix) for ix in range(X.shape[1])]
-
-        self.rule_base = problem._construct_ruleBase(
-        best_individual, self.fuzzy_type)
-        self.rule_base.rename_cons(self.classes_)
-
-        self.eval_performance = evr.evalRuleBase(
-        self.rule_base, np.array(X), y)
-
-        self.eval_performance.add_full_evaluation()  
-        if self.lvs is None:
-            self.rename_fuzzy_variables()
-        self.eval_performance.add_classification_metrics()
-        self.rule_base.purge_rules(self.tolerance)
-        
-
-    def load_master_rule_base(self, rule_base: rules.MasterRuleBase) -> None:
-        '''
-        Loads a master rule base to be used in the prediction process.
-
-        :param rule_base: ruleBase object.
-        :return: None
-        '''
-        self.rule_base = rule_base
-        self.nRules = len(rule_base.get_rules())
-        self.nAnts = len(rule_base.get_rules()[0].antecedents)
-        self.n_class = len(rule_base)
-        self.classes_ = rule_base.consequent_names()
-        
-
-    def forward(self, X: np.array) -> np.array:
-        '''
-        Returns the predicted class for each sample.
-
-        :param X: np array samples x features.
-        :return: np array samples (x 1) with the predicted class.
-        '''
-        try:
-            X = X.values  # If X was a pandas dataframe
-        except AttributeError:
-            pass
-        
-        return self.rule_base.winning_rule_predict(X)
-        
-
-    def predict(self, X: np.array) -> np.array:
-        '''
-        Returns the predicted class for each sample.
-
-        :param X: np array samples x features.
-        :return: np array samples (x 1) with the predicted class.
-        '''
-        return self.forward(X)
-
-
-    def print_rules(self, return_rules:bool=False) -> None:
-        '''
-        Print the rules contained in the fitted rulebase.
-        '''
-        return self.rule_base.print_rules(return_rules)
-
-
-    def plot_fuzzy_variables(self) -> None:
-        '''
-        Plot the fuzzy partitions in each fuzzy variable.
-        '''
-        fuzzy_variables = self.rule_base.rule_bases[0].antecedents
-
-        for ix, fv in enumerate(fuzzy_variables):
-            vis_rules.plot_fuzzy_variable(fv)
-
-
-    def rename_fuzzy_variables(self) -> None:
-        '''
-        Renames the linguist labels so that high, low and so on are consistent. It does so usually after an optimization process.
-
-        :return: None. Names are sorted accorded to the central point of the fuzzy memberships.
-        '''
-
-        for ix in range(len(self.rule_base)):
-            fuzzy_variables = self.rule_base.rule_bases[ix].antecedents
-
-            for jx, fv in enumerate(fuzzy_variables):
-                # I feel so extraordinary, lifes got a hold on me...
-                new_order_values = []
-                possible_names = FitRuleBase.vl_names[self.n_linguist_variables]
-
-                for zx, fuzzy_set in enumerate(fv.linguistic_variables):
-                    studied_fz = fuzzy_set.type()
-                    
-                    if studied_fz == fs.FUZZY_SETS.temporal:
-                        studied_fz = fuzzy_set.inside_type()
-
-                    if studied_fz == fs.FUZZY_SETS.t1:
-                        f1 = np.mean(
-                            fuzzy_set.membership_parameters[0] + fuzzy_set.membership_parameters[1])
-                    elif (studied_fz == fs.FUZZY_SETS.t2):
-                        f1 = np.mean(
-                            fuzzy_set.secondMF_upper[0] + fuzzy_set.secondMF_upper[1])
-                    elif studied_fz == fs.FUZZY_SETS.gt2:
-                        sec_memberships = fuzzy_set.secondary_memberships.values()
-                        f1 = float(list(fuzzy_set.secondary_memberships.keys())[np.argmax(
-                            [fzm.membership_parameters[2] for ix, fzm in enumerate(sec_memberships)])])
-
-                    new_order_values.append(f1)
-
-                new_order = np.argsort(np.array(new_order_values))
-                fuzzy_sets_vl = fv.linguistic_variables
-
-                for jx, x in enumerate(new_order):
-                    fuzzy_sets_vl[x].name = possible_names[jx]
-
-
-    def get_rulebase(self) -> list[np.array]:
-        '''
-        Get the rulebase obtained after fitting the classifier to the data.
-
-        :return: a matrix format for the rulebase.
-        '''
-        return self.rule_base.get_rulebase_matrix()
-    
-
-    def reparametrice_loss(self, alpha:float, beta:float, gamma:float) -> None:
-        '''
-        Changes the parameters in the loss function. 
-
-        :note: Does not check for convexity preservation. The user can play with these parameters as it wills.
-        :param alpha: controls the MCC term.
-        :param beta: controls the average rule size loss.
-        :param gamma: controls the number of rules loss.
-        '''
-        self.alpha_ = alpha
-        self.beta_ = beta
-        self.gamma_ = gamma
-
-class ExploreRuleBases(Problem):
-    '''
-    Class to model as pymoo problem the fitting of a rulebase to a set of data given a series of candidate rules for a classification problem using Evolutionary strategies
-    Supports type 1 and t2.
-    '''
-
-    def __init__(self, X: np.array, y: np.array, nRules: int, n_classes: int, cancidate_rules: rules.MasterRuleBase, thread_runner: StarmapParallelization=None, tolerance:float = 0.01) -> None:
-        '''
-        Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
-
-        :param X: np array or pandas dataframe samples x features.
-        :param y: np vector containing the target classes. vector sample
-        :param n_class: number of classes in the problem. If None (as default) it will be computed from the data.
-        :param cancidate_rules: MasterRuleBase object. If not None, the classifier will use the rules in the object and ignore the conflicting parameters.
-        '''
-        try:
-            self.var_names = list(X.columns)
-            self.X = X.values
-        except AttributeError:
-            self.X = X
-            self.var_names = [str(ix) for ix in range(X.shape[1])]
-
-        self.tolerance = tolerance
-        self.fuzzy_type = cancidate_rules.fuzzy_type()
-        self.y = y
-        self.nCons = 1  # This is fixed to MISO rules.
-        self.n_classes = n_classes
-        self.candidate_rules = cancidate_rules
-        self.nRules = nRules
-
-        self.vl_names = self.candidate_rules[0].antecedents[0].linguistic_variable_names()
-        self.fuzzy_type = self.candidate_rules[0].antecedents[0].fuzzy_type()
-
-        self.min_bounds = np.min(self.X, axis=0)
-        self.max_bounds = np.max(self.X, axis=0)
-
-        nTotalRules = len(self.candidate_rules.get_rules())
-        # Each var is using or not a rule. 
-        vars = {ix: Integer(bounds=[0, nTotalRules - 1]) for ix in range(self.nRules)}
-        varbound = np.array([[0, nTotalRules- 1]] * self.nRules)
-
-        nVar = len(vars.keys())
-        if thread_runner is not None:
-            super().__init__(
-                vars=vars,
-                n_var=nVar,
-                n_obj=1,
-                elementwise=True,
-                vtype=int,
-                xl=varbound[:, 0],
-                xu=varbound[:, 1],
-                elementwise_runner=thread_runner)
-        else:
-            super().__init__(
-                vars=vars,
-                n_var=nVar,
-                n_obj=1,
-                elementwise=True,
-                vtype=int,
-                xl=varbound[:, 0],
-                xu=varbound[:, 1])
-
-
-    def _construct_ruleBase(self, x: np.array, fuzzy_type: fs.FUZZY_SETS) -> rules.MasterRuleBase:
-        '''
-        Creates a valid rulebase from the given subject and the candidate rules.
-
-        :param x: gen of a rulebase. type: dict.
-        
-        :return: a Master rulebase object.
-        '''
-        x = x.astype(int)
-        # Get all rules and their consequents
-        diff_consequents = np.arange(len(self.candidate_rules))
-        
-        # Choose the selected ones in the gen
-        total_rules = self.candidate_rules.get_rules()
-        chosen_rules = [total_rules[ix] for ix, val in enumerate(x)]
-        rule_consequents = sum([[ix] * len(rule) for ix, rule in enumerate(self.candidate_rules)], [])
-        chosen_rules_consequents = [rule_consequents[val] for ix, val in enumerate(x)]
-        # Create a rule base for each consequent with the selected rules
-        rule_list = [[] for _ in range(self.n_classes)]
-        rule_bases = []
-        for ix, consequent in enumerate(diff_consequents):
-            for rx, rule in enumerate(chosen_rules):
-                if chosen_rules_consequents[rx] == consequent:
-                    rule_list[ix].append(rule)
-
-            if len(rule_list[ix]) > 0:
-                if fuzzy_type == fs.FUZZY_SETS.t1:
-                    rule_base_cons = rules.RuleBaseT1(
-                        self.candidate_rules[0].antecedents, rule_list[ix])
-                elif fuzzy_type == fs.FUZZY_SETS.t2:
-                    rule_base_cons = rules.RuleBaseT2(
-                        self.candidate_rules[0].antecedents, rule_list[ix])
-                elif fuzzy_type == fs.FUZZY_SETS.gt2:
-                    rule_base_cons = rules.RuleBaseGT2(
-                        self.candidate_rules[0].antecedents, rule_list[ix])
-                    
-                rule_bases.append(rule_base_cons)
-            
-        # Create the Master Rule Base object with the individual rule bases
-        newMasterRuleBase = rules.MasterRuleBase(rule_bases, diff_consequents)    
-
-        return newMasterRuleBase
-
-
-    def _evaluate(self, x: np.array, out: dict, *args, **kwargs):
-        '''
-        :param x: array of train samples. x shape = features
-            those features are the parameters to optimize.
-
-        :param out: dict where the F field is the fitness. It is used from the outside.
-        '''
-        try:
-            ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
-
-            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance)
-            
-
-            out["F"] = 1 - score
-        except rules.RuleError:
-            out["F"] = 1
-
-    
-    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.95, beta:float=0.025, gamma:float=0.025) -> float:
-        '''
-        Fitness function for the optimization problem.
-        :param ruleBase: RuleBase object
-        :param X: array of train samples. X shape = (n_samples, n_features)
-        :param y: array of train labels. y shape = (n_samples,)
-        :param tolerance: float. Tolerance for the size evaluation.
-        :return: float. Fitness value.
-        '''
-        ev_object = evr.evalRuleBase(ruleBase, X, y)
-        ev_object.add_rule_weights()
-
-        score_acc = ev_object.classification_eval()
-        score_rules_size = ev_object.size_antecedents_eval(tolerance)
-        score_nrules = ev_object.effective_rulesize_eval(tolerance)
-
-        score = score_acc * alpha + (1 - alpha) * (score_rules_size * beta + score_nrules * gamma)
-
-        return score
-    
-
-
-class FitRuleBase(Problem):
-    '''
-    Class to model as pymoo problem the fitting of a rulebase for a classification problem using Evolutionary strategies. 
-    Supports type 1 and iv fs (iv-type 2)
-    '''
-
-    def _init_optimize_vl(self, fuzzy_type: fs.FUZZY_SETS, n_linguist_variables: int, domain: list[(float, float)] = None):
-        '''
-        Inits the corresponding fields if no linguistic partitions were given.
-
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param n_linguistic_variables: number of linguistic variables per antecedent.
-        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
-        '''
-        self.lvs = None
-        try:
-            self.vl_names = FitRuleBase.vl_names[n_linguist_variables]
-        except IndexError:
-            self.vl_names = [str(ix) for ix in range(n_linguist_variables)]
-
-        self.fuzzy_type = fuzzy_type
-        self.n_lv_possible = n_linguist_variables
-        self.domain = domain
-        
-
-    def _init_precomputed_vl(self, linguist_variables: list[fs.fuzzyVariable]):
-        '''
-        Inits the corresponding fields if linguistic partitions for each variable are given.
-
-        :param linguistic_variables: list of fuzzyVariables type.
-        '''
-        self.lvs = linguist_variables
-        self.vl_names = self.lvs[0].linguistic_variable_names()
-        self.n_lv_possible = len(self.lvs[0])
-        self.fuzzy_type = self.lvs[0].fs_type
-        self.domain = None
-
-    vl_names = [  # Linguistic variable names preestated for some specific cases.
-        [],
-        [],
-        ['Low', 'High'],
-        ['Low', 'Medium', 'High'],
-        ['Low', 'Medium', 'High', 'Very High'],
-        ['Very Low', 'Low', 'Medium', 'High', 'Very High']
-    ]
-
-    def __init__(self, X: np.array, y: np.array, nRules: int, nAnts: int, n_classes: int, thread_runner: StarmapParallelization=None, 
-                 linguistic_variables:list[fs.fuzzyVariable]=None, n_linguist_variables:int=3, fuzzy_type=fs.FUZZY_SETS.t1, domain:list=None,
-                 tolerance:float=0.01, alpha:float=0.950, beta:float=0.025, gamma:float=0.025) -> None:
-        '''
-        Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
-
-        :param X: np array or pandas dataframe samples x features.
-        :param y: np vector containing the target classes. vector sample
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param n_class: number of classes in the problem. If None (as default) it will be computed from the data.
-        :param linguistic_variables: list of linguistic variables precomputed. If given, the rest of conflicting arguments are ignored.
-        :param n_linguistic_variables: number of linguistic variables per antecedent.
-        :param fuzzy_type: Define the fuzzy set or fuzzy set extension used as linguistic variable.
-        :param domain: list with the upper and lower domains of each input variable. If None (as default) it will stablish the empirical min/max as the limits.
-        '''
-        try:
-            self.var_names = list(X.columns)
-            self.X = X.values
-        except AttributeError:
-            self.X = X
-            self.var_names = [str(ix) for ix in range(X.shape[1])]
-
-        try:
-            self.tolerance = tolerance
-        except KeyError:
-            self.tolerance = 0.001
-
-        self.y = y
-        self.nRules = nRules
-        self.nAnts = nAnts
-        self.nCons = 1  # This is fixed to MISO rules.
-
-        if n_classes is not None:
-            self.n_classes = n_classes
-        else:
-            self.n_classes = len(np.unique(y))
-
-        if linguistic_variables is not None:
-            self._init_precomputed_vl(linguistic_variables)
-        else:
-            self._init_optimize_vl(
-                fuzzy_type, n_linguist_variables)
-
-        if self.domain is None:
-            self.min_bounds = np.min(self.X, axis=0)
-            self.max_bounds = np.max(self.X, axis=0)
-        else:
-            self.min_bounds, self.max_bounds = self.domain
-
-        self.antecedents_referencial = [np.linspace(
-            self.min_bounds[ix], self.max_bounds[ix], 100) for ix in range(self.X.shape[1])]
-
-        possible_antecedent_bounds = np.array(
-            [[0, self.X.shape[1] - 1]] * self.nAnts * self.nRules)  
-        vl_antecedent_bounds = np.array(
-            [[-1, self.n_lv_possible - 1]] * self.nAnts * self.nRules) # -1 means not caring
-        antecedent_bounds = np.concatenate(
-            (possible_antecedent_bounds, vl_antecedent_bounds))
-        vars_antecedent = {ix: Integer(
-            bounds=antecedent_bounds[ix]) for ix in range(len(antecedent_bounds))}
-        aux_counter = len(vars_antecedent)
-
-        if self.lvs is None:
-            assert self.n_lv_possible >= 1, 'At least 1 possible value for a linguistic variable is required.'
-
-            self.feature_domain_bounds = np.array(
-                [[0, 99] for ix in range(self.X.shape[1])])
-            size_multiplier = 4 if self.fuzzy_type == fs.FUZZY_SETS.t1 else 8
-            membership_bounds = np.concatenate(
-                [self.feature_domain_bounds] * self.n_lv_possible * size_multiplier)
-            vars_memeberships = {
-                aux_counter + ix: Integer(bounds=membership_bounds[ix]) for ix in range(len(membership_bounds))}
-            aux_counter += len(vars_memeberships)
-
-        final_consequent_bounds = np.array(
-            [[-1, self.n_classes - 1]] * self.nRules)
-        vars_consequent = {aux_counter + ix: Integer(
-            bounds=final_consequent_bounds[ix]) for ix in range(len(final_consequent_bounds))}
-
-        if self.lvs is None:
-            vars = {key: val for d in [
-                vars_antecedent, vars_memeberships, vars_consequent] for key, val in d.items()}
-            varbound = np.concatenate(
-                (antecedent_bounds, membership_bounds, final_consequent_bounds), axis=0)
-        else:
-            vars = {key: val for d in [vars_antecedent,
-                                       vars_consequent] for key, val in d.items()}
-            varbound = np.concatenate(
-                (antecedent_bounds, final_consequent_bounds), axis=0)
-
-        nVar = len(varbound)
-        self.single_gen_size = nVar
-        self.alpha_ = alpha
-        self.beta_ = beta
-        self.gamma_ = gamma
-
-        if thread_runner is not None:
-            super().__init__(
-                vars=vars,
-                n_var=nVar,
-                n_obj=1,
-                elementwise=True,
-                vtype=int,
-                xl=varbound[:, 0],
-                xu=varbound[:, 1],
-                elementwise_runner=thread_runner)
-        else:
-            super().__init__(
-                vars=vars,
-                n_var=nVar,
-                n_obj=1,
-                elementwise=True,
-                vtype=int,
-                xl=varbound[:, 0],
-                xu=varbound[:, 1])
-
-
-    def encode_rulebase(self, rule_base: rules.MasterRuleBase, optimize_lv: bool) -> np.array:
-        '''
-        Given a rule base, constructs the corresponding gene associated with that rule base.
-
-        GENE STRUCTURE
-
-        First: antecedents chosen by each rule. Size: nAnts * nRules (index of the antecedent)
-        Second: Variable linguistics used. Size: nAnts * nRules
-        Third: Parameters for the fuzzy partitions of the chosen variables. Size: nAnts * self.n_linguistic_variables * 8|4 (2 trapezoidal memberships if t2)
-        Four: Consequent classes. Size: nRules
-
-        :param rule_base: rule base object.
-        :param optimize_lv: if True, the gene is prepared to optimize the membership functions.
-        :param antecedents_referencial: list of lists. Each list contains the referencial for each variable.  Required only if optimize_lv is True.
-        :return: np array of size self.single_gen_size.
-        '''
-        gene = np.zeros((self.single_gen_size,))
-
-        n_lv_possible = len(rule_base.rule_bases[0].antecedents[0].linguistic_variables)
-        fz_type = rule_base.fuzzy_type()
-        rule_consequents = rule_base.get_consequents()
-        nreal_rules = len(rule_consequents)
-        mf_size = 4 if fz_type == fs.FUZZY_SETS.t1 else 8
-
-        # Pointer to the fourth section of the gene: consequents
-        if optimize_lv:
-            # If lv memberships are optimized.
-            fourth_pointer = 2 * self.nAnts * self.nRules + \
-                len(rule_base.antecedents) * n_lv_possible * mf_size
-        else:
-            # If no memberships are optimized.
-            fourth_pointer = 2 * self.nAnts * self.nRules
-
-        # First and second sections of the gene: antecedents and linguistic variables
-        for i0, rule in enumerate(rule_base.get_rules()):  # Reconstruct the rules
-            first_pointer = i0 * self.nAnts
-            second_pointer = (self.nRules * self.nAnts) + i0 * self.nAnts
-
-            for ax, linguistic_variable in enumerate(rule.antecedents):
-                gene[first_pointer + ax] = ax
-                gene[second_pointer + ax] = linguistic_variable
-            
-            # Update the fourth section of the gene: consequents using the fourth pointer
-            gene[fourth_pointer + i0] = rule_consequents[i0]
-
-        # Fill the rest of the rules with don't care values
-        nvoid_rules = self.nRules - nreal_rules
-        for vx in range(nvoid_rules):
-            first_pointer = nreal_rules * self.nAnts + vx * self.nAnts
-            second_pointer = (self.nRules * self.nAnts) + nreal_rules * self.nAnts + vx * self.nAnts
-
-            for ax, linguistic_variable in enumerate(rule.antecedents):
-                gene[first_pointer + ax] = ax
-                gene[second_pointer + ax] = -1
-            
-            # Update the fourth section of the gene: consequents using the fourth pointer
-            gene[fourth_pointer + nreal_rules + vx] = -1
-
-        if optimize_lv:
-            # If lv memberships are optimized.
-            third_pointer = 2 * self.nAnts * self.nRules
-            aux_pointer = 0
-            for ix, fuzzy_variable in enumerate(rule_base.get_antecedents()):
-                for linguistic_variable in range(n_lv_possible):
-                    fz_parameters = fuzzy_variable[linguistic_variable].membership_parameters
-                    for jx, fz_parameter in enumerate(fz_parameters):
-                        closest_idx = (np.abs(np.asarray(self.antecedents_referencial[ix]) - fz_parameter)).argmin()
-                        gene[third_pointer + aux_pointer] = closest_idx
-                        aux_pointer += 1
-                    
-        return np.array(list(map(int, gene)))
-        
-
-
-    def _construct_ruleBase(self, x: np.array, fz_type: fs.FUZZY_SETS, **kwargs) -> rules.MasterRuleBase:
-        '''
-        Given a subject, it creates a rulebase according to its specification.
-
-        :param x: gen of a rulebase. type: dict.
-        :param fz_type: a enum type. Check fuzzy_sets for complete specification (two fields, t1 and t2, to mark which fs you want to use)
-        :return: a rulebase object.
-
-        kwargs:
-            - time_moment: if temporal fuzzy sets are used with different partitions for each time interval, 
-                            then this parameter is used to specify which time moment is being used.
-        '''
-
-        rule_list = [[] for _ in range(self.n_classes)]
-
-        mf_size = 4 if fz_type == fs.FUZZY_SETS.t1 else 8
-        '''
-        GEN STRUCTURE
-
-        First: antecedents chosen by each rule. Size: nAnts * nRules
-        Second: Variable linguistics used. Size: nAnts * nRules
-        Third: Parameters for the fuzzy partitions of the chosen variables. Size: X.shape[1] * self.n_linguistic_variables * 8|4 (2 trapezoidal memberships if t2)
-        Four: Consequent classes. Size: nRules (fixed to 4 right now)
-        '''
-        if self.lvs is None:
-            # If memberships are optimized.
-            fourth_pointer = 2 * self.nAnts * self.nRules + \
-                self.X.shape[1] * self.n_lv_possible * mf_size
-        else:
-            # If no memberships are optimized.
-            fourth_pointer = 2 * self.nAnts * self.nRules
-
-        aux_pointer = 0
-        min_domain = np.min(self.X, axis=0)
-        max_domain = np.max(self.X, axis=0)
-
-        # Integer sampling doesnt work fine in pymoo, so we do this (which is btw what pymoo is really doing if you just set integer optimization)
-        try:
-            # subject might come as a dict.
-            x = np.array(list(x.values())).astype(int)
-        except AttributeError:
-            x = x.astype(int)
-
-        for i0 in range(self.nRules):  # Reconstruct the rules
-            first_pointer = i0 * self.nAnts
-            chosen_ants = x[first_pointer:first_pointer + self.nAnts]
-
-            second_pointer = (i0 * self.nAnts) + (self.nAnts * self.nRules)
-            # Shape: self.nAnts + self.n_lv_possible  + 1
-            antecedent_parameters = x[second_pointer:second_pointer+self.nAnts]
-
-            init_rule_antecedents = np.zeros(
-                (self.X.shape[1],)) - 1  # -1 is dont care
-            for jx, ant in enumerate(chosen_ants):
-                antecedent_parameters[jx] = min(antecedent_parameters[jx], len(self.lvs[ant]) - 1)
-                init_rule_antecedents[ant] = antecedent_parameters[jx]
-
-            consequent_idx = x[fourth_pointer + aux_pointer]
-            assert consequent_idx < self.n_classes, "Consequent class is not valid. Something in the gene is wrong."
-            aux_pointer += 1
- 
-            if consequent_idx != -1:
-                rule_list[consequent_idx].append(
-                    rules.RuleSimple(init_rule_antecedents, 0))
-
-        # If we optimize the membership functions
-        if self.lvs is None:
-            third_pointer = 2 * self.nAnts * self.nRules
-            aux_pointer = 0
-            antecedents = []
-
-            for fuzzy_variable in range(self.X.shape[1]):
-                linguistic_variables = []
-
-                for linguistic_variable in range(self.n_lv_possible):
-                    parameter_pointer = third_pointer + aux_pointer
-                    fz_parameters_idx = x[parameter_pointer:parameter_pointer + mf_size]
-                    fz_parameters = self.antecedents_referencial[fuzzy_variable][fz_parameters_idx]
-                    aux_pointer += mf_size
-
-                    if fz_type == fs.FUZZY_SETS.t2:
-                        fz_parameters[0:6] = np.sort(fz_parameters[0:6])
-                        mu = [np.min(fz_parameters[0:2]), fz_parameters[2],
-                              fz_parameters[3], np.max(fz_parameters[4:6])]
-                        ml = [np.max(fz_parameters[0:2]), fz_parameters[2],
-                              fz_parameters[3], np.min(fz_parameters[4:6])]
-                        height = fz_parameters[6] / np.max(fz_parameters)
-
-                        ivfs = fs.IVFS(self.vl_names[linguistic_variable], ml, mu,
-                                       (min_domain[fuzzy_variable], max_domain[fuzzy_variable]), lower_height=height)
-                    else:
-                        ivfs = fs.FS(self.vl_names[linguistic_variable], np.sort(fz_parameters[0:4]),
-                                     (min_domain[fuzzy_variable], max_domain[fuzzy_variable]))
-                    linguistic_variables.append(ivfs)
-
-                antecedents.append(fs.fuzzyVariable(
-                    self.var_names[fuzzy_variable], linguistic_variables))
-        else:
-            try:
-                antecedents = self.lvs[kwargs['time_moment']]
-            except:
-                antecedents = self.lvs
-
-        for i in range(self.n_classes):
-            if fz_type == fs.FUZZY_SETS.temporal:
-                fz_type = self.lvs[0][0].inside_type()
-
-            if fz_type == fs.FUZZY_SETS.t1:
-                rule_base = rules.RuleBaseT1(antecedents, rule_list[i])
-            elif fz_type == fs.FUZZY_SETS.t2:
-                rule_base = rules.RuleBaseT2(antecedents, rule_list[i])
-            elif fz_type == fs.FUZZY_SETS.gt2:
-                rule_base = rules.RuleBaseGT2(antecedents, rule_list[i])
-            
-
-            if i == 0:
-                res = rules.MasterRuleBase([rule_base])
-            else:
-                res.add_rule_base(rule_base)
-
-        return res
-
-
-    def _evaluate(self, x: np.array, out: dict, *args, **kwargs):
-        '''
-        :param x: array of train samples. x shape = features
-            those features are the parameters to optimize.
-
-        :param out: dict where the F field is the fitness. It is used from the outside.
-        '''
-        ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
-
-        if len(ruleBase.get_rules()) > 0:
-            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self.alpha_, self.beta_, self.gamma_)
-        else:
-            score = 0.0
-        
-        out["F"] = 1 - score
-    
-
-    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.975, beta:float=0.0125, gamma:float=0.0125) -> float:
-        '''
-        Fitness function for the optimization problem.
-        :param ruleBase: RuleBase object
-        :param X: array of train samples. X shape = (n_samples, n_features)
-        :param y: array of train labels. y shape = (n_samples,)
-        :param tolerance: float. Tolerance for the size evaluation.
-        :return: float. Fitness value.
-        '''
-        ev_object = evr.evalRuleBase(ruleBase, X, y)
-        ev_object.add_full_evaluation()
-        ruleBase.purge_rules(tolerance)
-
-        if len(ruleBase.get_rules()) > 0: 
-            score_acc = ev_object.classification_eval()
-            score_rules_size = ev_object.size_antecedents_eval(tolerance)
-            score_nrules = ev_object.effective_rulesize_eval(tolerance)
-
-            score = score_acc * alpha + score_rules_size * beta + score_nrules * gamma
-        else:
-            score = 0.0
-            
-        return score
-    
-
+"""
+This is a the source file that contains the class to train/fit the rulebase using a genetic algorithm.
+
+"""
+import numpy as np
+import pandas as pd
+
+from sklearn.model_selection import StratifiedKFold
+from sklearn.metrics import matthews_corrcoef
+from sklearn.base import ClassifierMixin
+from pymoo.algorithms.soo.nonconvex.ga import GA
+from pymoo.core.problem import Problem
+from pymoo.optimize import minimize
+from pymoo.operators.sampling.rnd import IntegerRandomSampling
+from pymoo.operators.crossover.sbx import SBX
+from pymoo.operators.mutation.pm import PolynomialMutation
+from pymoo.core.variable import Integer
+from multiprocessing.pool import ThreadPool
+from pymoo.core.problem import StarmapParallelization
+
+try:
+    from . import fuzzy_sets as fs
+    from . import rules
+    from . import eval_rules as evr
+    from . import vis_rules
+    from . import maintenance as mnt
+except ImportError:
+    import fuzzy_sets as fs
+    import rules
+    import eval_rules as evr
+    import vis_rules
+    import maintenance as mnt
+
+
+
+class BaseFuzzyRulesClassifier(ClassifierMixin):
+    '''
+    Class that is used as a classifier for a fuzzy rule based system. Supports precomputed and optimization of the linguistic variables.
+    '''
+
+    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = fs.FUZZY_SETS.t1, tolerance: float = 0.0,
+                 n_linguist_variables: int = 3, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
+                 domain: list[float] = None, n_class: int=None, precomputed_rules: rules.MasterRuleBase =None, runner: int=1) -> None:
+        '''
+        Inits the optimizer with the corresponding parameters.
+
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param tolerance: tolerance for the dominance score of the rules.
+        :param n_linguist_variables: number of linguistic variables per antecedent.
+        :param verbose: if True, prints the progress of the optimization.
+        :param linguistic_variables: list of fuzzyVariables type. If None (default) the optimization process will init+optimize them.
+        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
+        :param n_class: names of the classes in the problem. If None (default) the classifier will compute it empirically.
+        :param precomputed_rules: MasterRuleBase object. If not None, the classifier will use the rules in the object and ignore the conflicting parameters.
+        :param runner: number of threads to use. If None (default) the classifier will use 1 thread.
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
+
+        if precomputed_rules is not None:
+            self.nRules = len(precomputed_rules.get_rules())
+            self.nAnts = len(precomputed_rules.get_rules()[0].antecedents)
+            self.n_class = len(precomputed_rules)
+            self.classes_ = precomputed_rules.consequent_names
+            self.rule_base = precomputed_rules
+        else:
+            self.nRules = nRules
+            self.nAnts = nAnts
+            self.classes_ = n_class
+
+        self.custom_loss = None
+        self.verbose = verbose
+        self.tolerance = tolerance
+        
+
+        if runner > 1:
+            pool = ThreadPool(runner)
+            self.thread_runner = StarmapParallelization(pool.starmap)
+        else:
+            self.thread_runner = None
+        
+        if linguistic_variables is not None:
+            if mnt.save_usage_flag:
+                mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
+            # If the linguistic variables are precomputed then we act accordingly
+            self.lvs = linguistic_variables
+            self.n_linguist_variables = len(
+                self.lvs[0].linguistic_variable_names())
+            self.domain = None
+            self.fuzzy_type = self.lvs[0].fuzzy_type()
+        else:
+            if mnt.save_usage_flag:
+                mnt.usage_data[mnt.usage_categories.Funcs]['opt_labels'] += 1
+
+            # If not, then we need the parameters sumistered by the user.
+            self.lvs = None
+            self.fuzzy_type = fuzzy_type
+            self.n_linguist_variables = n_linguist_variables
+            self.domain = domain
+
+        self.alpha_ = 0.950
+        self.beta_ = 0.025
+        self.gamma_ = 0.025
+
+    def customized_loss(self, loss_function):
+        '''
+        Function to customize the loss function used for the optimization.
+
+        :param loss_function: function that takes as input the true labels and the predicted labels and returns a float.
+        :return: None
+        '''
+        self.custom_loss = loss_function
+
+
+    def fit(self, X: np.array, y: np.array, n_gen:int=70, pop_size:int=30,
+            checkpoints:int=0, candidate_rules:rules.MasterRuleBase=None, initial_rules:rules.MasterRuleBase=None):
+        '''
+        Fits a fuzzy rule based classifier using a genetic algorithm to the given data.
+
+        :param X: numpy array samples x features
+        :param y: labels. integer array samples (x 1)
+        :param n_gen: integer. Number of generations to run the genetic algorithm.
+        :param pop_size: integer. Population size for each gneration.
+        :param checkpoints: integer. Number of checkpoints to save the best rulebase found so far.
+        :param candidate_rules: if these rules exist, the optimization process will choose the best rules from this set. If None (default) the rules will be generated from scratch.
+        :return: None. The classifier is fitted to the data.
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.Funcs]['fit'] += 1
+            
+        if self.classes_ is None:
+            if isinstance(y, pd.Series):
+                self.classes_ = [str(aux) for aux in y.unique()]
+                # Convert the names in the label vector to integer classes
+                y = np.array(y.replace(self.classes_, np.arange(len(self.classes_))))
+            else:
+                self.classes_ = [str(aux) for aux in np.unique(y)]
+            
+        if candidate_rules is None:
+            if initial_rules is not None:
+                self.fuzzy_type = initial_rules.fuzzy_type()
+                self.n_linguist_variables = initial_rules.n_linguist_variables()
+                self.domain = [fv.domain for fv in initial_rules[0].antecedents]
+                self.nRules = len(initial_rules.get_rules())
+                self.nAnts = len(initial_rules.get_rules()[0].antecedents)
+
+            if self.lvs is None:
+                # If Fuzzy variables need to be optimized.
+                problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, tolerance=self.tolerance, n_classes=len(np.unique(y)),
+                                    n_linguist_variables=self.n_linguist_variables, fuzzy_type=self.fuzzy_type, domain=self.domain, thread_runner=self.thread_runner,
+                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
+            else:
+                # If Fuzzy variables are already precomputed.
+                problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, n_classes=len(np.unique(y)),
+                                    linguistic_variables=self.lvs, domain=self.domain, tolerance=self.tolerance, thread_runner=self.thread_runner,
+                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
+        else:
+            self.fuzzy_type = candidate_rules.fuzzy_type()
+            self.n_linguist_variables = candidate_rules.n_linguist_variables()
+            problem = ExploreRuleBases(X, y, n_classes=len(np.unique(y)), cancidate_rules=candidate_rules, thread_runner=self.thread_runner, nRules=self.nRules)
+
+        if self.custom_loss is not None:
+            problem.fitness_func = self.custom_loss
+
+        if initial_rules is not None:
+            rules_gene = problem.encode_rulebase(initial_rules, self.lvs is None)
+            rules_gene = (np.ones((pop_size, len(rules_gene))) * rules_gene).astype(int)
+        else:
+            rules_gene = IntegerRandomSampling()
+
+        algorithm = GA(
+            pop_size=pop_size,
+            crossover=SBX(prob=.3, eta=3.0),
+            mutation=PolynomialMutation(eta=7.0),
+            sampling=rules_gene,
+            eliminate_duplicates=False)
+        
+
+        if checkpoints > 0:
+            if self.verbose:
+                print('=================================================')
+                print('n_gen  |  n_eval  |     f_avg     |     f_min    ')
+                print('=================================================')
+            algorithm.setup(problem, seed=33, termination=('n_gen', n_gen)) # 33? Soon...
+            for k in range(n_gen):
+                algorithm.next()
+                res = algorithm
+                if self.verbose:
+                    print('%-6s | %-8s | %-8s | %-8s' % (res.n_gen, res.evaluator.n_eval, res.pop.get('F').mean(), res.pop.get('F').min()))
+                if k % checkpoints == 0:
+                    with open("checkpoint_" + str(algorithm.n_gen), "w") as f:
+                        pop = algorithm.pop
+                        fitness_last_gen = pop.get('F')
+                        best_solution_arg = np.argmin(fitness_last_gen)
+                        best_individual = pop.get('X')[best_solution_arg, :]
+
+                        rule_base = problem._construct_ruleBase(
+                            best_individual, self.fuzzy_type)
+                        eval_performance = evr.evalRuleBase(
+                            rule_base, np.array(X), y)
+                        
+                        eval_performance.add_full_evaluation()  
+                        # self.rename_fuzzy_variables() This wont work on checkpoints!
+                        rule_base.purge_rules(self.tolerance)
+                        rule_base.rename_cons(self.classes_)
+                        checkpoint_rules = rule_base.print_rules(True)
+                        f.write(checkpoint_rules)     
+
+        else:
+            res = minimize(problem,
+                        algorithm,
+                        # termination,
+                        ("n_gen", n_gen),
+                        copy_algorithm=False,
+                        save_history=False,
+                        verbose=self.verbose)
+        
+        pop = res.pop
+        fitness_last_gen = pop.get('F')
+        best_solution = np.argmin(fitness_last_gen)
+        best_individual = pop.get('X')[best_solution, :]
+
+        
+        self.performance = 1 - fitness_last_gen[best_solution]
+
+        try:
+            self.var_names = list(X.columns)
+            self.X = X.values
+        except AttributeError:
+            self.X = X
+            self.var_names = [str(ix) for ix in range(X.shape[1])]
+
+        self.rule_base = problem._construct_ruleBase(
+        best_individual, self.fuzzy_type)
+
+        self.eval_performance = evr.evalRuleBase(
+        self.rule_base, np.array(X), y)
+
+        self.eval_performance.add_full_evaluation()  
+        if self.lvs is None:
+            self.rename_fuzzy_variables()
+        self.eval_performance.add_classification_metrics()
+        self.rule_base.purge_rules(self.tolerance)
+        
+
+    def load_master_rule_base(self, rule_base: rules.MasterRuleBase) -> None:
+        '''
+        Loads a master rule base to be used in the prediction process.
+
+        :param rule_base: ruleBase object.
+        :return: None
+        '''
+        self.rule_base = rule_base
+        self.nRules = len(rule_base.get_rules())
+        self.nAnts = len(rule_base.get_rules()[0].antecedents)
+        self.n_class = len(rule_base)
+        self.classes_ = rule_base.consequent_names
+        
+
+    def forward(self, X: np.array) -> np.array:
+        '''
+        Returns the predicted class for each sample.
+
+        :param X: np array samples x features.
+        :return: np array samples (x 1) with the predicted class.
+        '''
+        try:
+            X = X.values  # If X was a pandas dataframe
+        except AttributeError:
+            pass
+        
+        return self.rule_base.winning_rule_predict(X)
+        
+
+    def predict(self, X: np.array) -> np.array:
+        '''
+        Returns the predicted class for each sample.
+
+        :param X: np array samples x features.
+        :return: np array samples (x 1) with the predicted class.
+        '''
+        return self.forward(X)
+
+
+    def print_rules(self, return_rules:bool=False) -> None:
+        '''
+        Print the rules contained in the fitted rulebase.
+        '''
+        return self.rule_base.print_rules(return_rules)
+
+
+    def plot_fuzzy_variables(self) -> None:
+        '''
+        Plot the fuzzy partitions in each fuzzy variable.
+        '''
+        fuzzy_variables = self.rule_base.rule_bases[0].antecedents
+
+        for ix, fv in enumerate(fuzzy_variables):
+            vis_rules.plot_fuzzy_variable(fv)
+
+
+    def rename_fuzzy_variables(self) -> None:
+        '''
+        Renames the linguist labels so that high, low and so on are consistent. It does so usually after an optimization process.
+
+        :return: None. Names are sorted accorded to the central point of the fuzzy memberships.
+        '''
+
+        for ix in range(len(self.rule_base)):
+            fuzzy_variables = self.rule_base.rule_bases[ix].antecedents
+
+            for jx, fv in enumerate(fuzzy_variables):
+                # I feel so extraordinary, lifes got a hold on me...
+                new_order_values = []
+                possible_names = FitRuleBase.vl_names[self.n_linguist_variables]
+
+                for zx, fuzzy_set in enumerate(fv.linguistic_variables):
+                    studied_fz = fuzzy_set.type()
+                    
+                    if studied_fz == fs.FUZZY_SETS.temporal:
+                        studied_fz = fuzzy_set.inside_type()
+
+                    if studied_fz == fs.FUZZY_SETS.t1:
+                        f1 = np.mean(
+                            fuzzy_set.membership_parameters[0] + fuzzy_set.membership_parameters[1])
+                    elif (studied_fz == fs.FUZZY_SETS.t2):
+                        f1 = np.mean(
+                            fuzzy_set.secondMF_upper[0] + fuzzy_set.secondMF_upper[1])
+                    elif studied_fz == fs.FUZZY_SETS.gt2:
+                        sec_memberships = fuzzy_set.secondary_memberships.values()
+                        f1 = float(list(fuzzy_set.secondary_memberships.keys())[np.argmax(
+                            [fzm.membership_parameters[2] for ix, fzm in enumerate(sec_memberships)])])
+
+                    new_order_values.append(f1)
+
+                new_order = np.argsort(np.array(new_order_values))
+                fuzzy_sets_vl = fv.linguistic_variables
+
+                for jx, x in enumerate(new_order):
+                    fuzzy_sets_vl[x].name = possible_names[jx]
+
+
+    def get_rulebase(self) -> list[np.array]:
+        '''
+        Get the rulebase obtained after fitting the classifier to the data.
+
+        :return: a matrix format for the rulebase.
+        '''
+        return self.rule_base.get_rulebase_matrix()
+    
+
+    def reparametrice_loss(self, alpha:float, beta:float, gamma:float) -> None:
+        '''
+        Changes the parameters in the loss function. 
+
+        :note: Does not check for convexity preservation. The user can play with these parameters as it wills.
+        :param alpha: controls the MCC term.
+        :param beta: controls the average rule size loss.
+        :param gamma: controls the number of rules loss.
+        '''
+        self.alpha_ = alpha
+        self.beta_ = beta
+        self.gamma_ = gamma
+
+
+
+class ExploreRuleBases(Problem):
+    '''
+    Class to model as pymoo problem the fitting of a rulebase to a set of data given a series of candidate rules for a classification problem using Evolutionary strategies
+    Supports type 1 and t2.
+    '''
+
+    def __init__(self, X: np.array, y: np.array, nRules: int, n_classes: int, cancidate_rules: rules.MasterRuleBase, thread_runner: StarmapParallelization=None, tolerance:float = 0.01) -> None:
+        '''
+        Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
+
+        :param X: np array or pandas dataframe samples x features.
+        :param y: np vector containing the target classes. vector sample
+        :param n_class: number of classes in the problem. If None (as default) it will be computed from the data.
+        :param cancidate_rules: MasterRuleBase object. If not None, the classifier will use the rules in the object and ignore the conflicting parameters.
+        '''
+        try:
+            self.var_names = list(X.columns)
+            self.X = X.values
+        except AttributeError:
+            self.X = X
+            self.var_names = [str(ix) for ix in range(X.shape[1])]
+
+        self.tolerance = tolerance
+        self.fuzzy_type = cancidate_rules.fuzzy_type()
+        self.y = y
+        self.nCons = 1  # This is fixed to MISO rules.
+        self.n_classes = n_classes
+        self.candidate_rules = cancidate_rules
+        self.nRules = nRules
+
+        self.vl_names = self.candidate_rules[0].antecedents[0].linguistic_variable_names()
+        self.fuzzy_type = self.candidate_rules[0].antecedents[0].fuzzy_type()
+
+        self.min_bounds = np.min(self.X, axis=0)
+        self.max_bounds = np.max(self.X, axis=0)
+
+        nTotalRules = len(self.candidate_rules.get_rules())
+        # Each var is using or not a rule. 
+        vars = {ix: Integer(bounds=[0, nTotalRules - 1]) for ix in range(self.nRules)}
+        varbound = np.array([[0, nTotalRules- 1]] * self.nRules)
+
+        nVar = len(vars.keys())
+        if thread_runner is not None:
+            super().__init__(
+                vars=vars,
+                n_var=nVar,
+                n_obj=1,
+                elementwise=True,
+                vtype=int,
+                xl=varbound[:, 0],
+                xu=varbound[:, 1],
+                elementwise_runner=thread_runner)
+        else:
+            super().__init__(
+                vars=vars,
+                n_var=nVar,
+                n_obj=1,
+                elementwise=True,
+                vtype=int,
+                xl=varbound[:, 0],
+                xu=varbound[:, 1])
+
+
+    def _construct_ruleBase(self, x: np.array, fuzzy_type: fs.FUZZY_SETS) -> rules.MasterRuleBase:
+        '''
+        Creates a valid rulebase from the given subject and the candidate rules.
+
+        :param x: gen of a rulebase. type: dict.
+        
+        :return: a Master rulebase object.
+        '''
+        x = x.astype(int)
+        # Get all rules and their consequents
+        diff_consequents = np.arange(len(self.candidate_rules))
+        
+        # Choose the selected ones in the gen
+        total_rules = self.candidate_rules.get_rules()
+        chosen_rules = [total_rules[ix] for ix, val in enumerate(x)]
+        rule_consequents = sum([[ix] * len(rule) for ix, rule in enumerate(self.candidate_rules)], [])
+        chosen_rules_consequents = [rule_consequents[val] for ix, val in enumerate(x)]
+        # Create a rule base for each consequent with the selected rules
+        rule_list = [[] for _ in range(self.n_classes)]
+        rule_bases = []
+        for ix, consequent in enumerate(diff_consequents):
+            for rx, rule in enumerate(chosen_rules):
+                if chosen_rules_consequents[rx] == consequent:
+                    rule_list[ix].append(rule)
+
+            if len(rule_list[ix]) > 0:
+                if fuzzy_type == fs.FUZZY_SETS.t1:
+                    rule_base_cons = rules.RuleBaseT1(
+                        self.candidate_rules[0].antecedents, rule_list[ix])
+                elif fuzzy_type == fs.FUZZY_SETS.t2:
+                    rule_base_cons = rules.RuleBaseT2(
+                        self.candidate_rules[0].antecedents, rule_list[ix])
+                elif fuzzy_type == fs.FUZZY_SETS.gt2:
+                    rule_base_cons = rules.RuleBaseGT2(
+                        self.candidate_rules[0].antecedents, rule_list[ix])
+                    
+                rule_bases.append(rule_base_cons)
+            
+        # Create the Master Rule Base object with the individual rule bases
+        newMasterRuleBase = rules.MasterRuleBase(rule_bases, diff_consequents)    
+
+        return newMasterRuleBase
+
+
+    def _evaluate(self, x: np.array, out: dict, *args, **kwargs):
+        '''
+        :param x: array of train samples. x shape = features
+            those features are the parameters to optimize.
+
+        :param out: dict where the F field is the fitness. It is used from the outside.
+        '''
+        try:
+            ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
+
+            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self._precomputed_truth)
+            
+
+            out["F"] = 1 - score
+        except rules.RuleError:
+            out["F"] = 1
+
+    
+    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.95, beta:float=0.025, gamma:float=0.025) -> float:
+        '''
+        Fitness function for the optimization problem.
+        :param ruleBase: RuleBase object
+        :param X: array of train samples. X shape = (n_samples, n_features)
+        :param y: array of train labels. y shape = (n_samples,)
+        :param tolerance: float. Tolerance for the size evaluation.
+        :return: float. Fitness value.
+        '''
+        ev_object = evr.evalRuleBase(ruleBase, X, y)
+        ev_object.add_rule_weights()
+
+        score_acc = ev_object.classification_eval()
+        score_rules_size = ev_object.size_antecedents_eval(tolerance)
+        score_nrules = ev_object.effective_rulesize_eval(tolerance)
+
+        score = score_acc * alpha + (1 - alpha) * (score_rules_size * beta + score_nrules * gamma)
+
+        return score
+    
+
+
+class FitRuleBase(Problem):
+    '''
+    Class to model as pymoo problem the fitting of a rulebase for a classification problem using Evolutionary strategies. 
+    Supports type 1 and iv fs (iv-type 2)
+    '''
+
+    def _init_optimize_vl(self, fuzzy_type: fs.FUZZY_SETS, n_linguist_variables: int, domain: list[(float, float)] = None):
+        '''
+        Inits the corresponding fields if no linguistic partitions were given.
+
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param n_linguistic_variables: number of linguistic variables per antecedent.
+        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
+        '''
+        self.lvs = None
+        try:
+            self.vl_names = FitRuleBase.vl_names[n_linguist_variables]
+        except IndexError:
+            self.vl_names = [str(ix) for ix in range(n_linguist_variables)]
+
+        self.fuzzy_type = fuzzy_type
+        self.n_lv_possible = n_linguist_variables
+        self.domain = domain
+        self._precomputed_truth = None
+
+    def _init_precomputed_vl(self, linguist_variables: list[fs.fuzzyVariable], X: np.array):
+        '''
+        Inits the corresponding fields if linguistic partitions for each variable are given.
+
+        :param linguistic_variables: list of fuzzyVariables type.
+        :param X: np array samples x features.
+        '''
+        self.lvs = linguist_variables
+        self.vl_names = self.lvs[0].linguistic_variable_names()
+        self.n_lv_possible = len(self.lvs[0])
+        self.fuzzy_type = self.lvs[0].fs_type
+        self.domain = None
+        self._precomputed_truth = rules.compute_antecedents_memberships(linguist_variables, X)
+
+    vl_names = [  # Linguistic variable names preestated for some specific cases.
+        [],
+        [],
+        ['Low', 'High'],
+        ['Low', 'Medium', 'High'],
+        ['Low', 'Medium', 'High', 'Very High'],
+        ['Very Low', 'Low', 'Medium', 'High', 'Very High']
+    ]
+
+    def __init__(self, X: np.array, y: np.array, nRules: int, nAnts: int, n_classes: int, thread_runner: StarmapParallelization=None, 
+                 linguistic_variables:list[fs.fuzzyVariable]=None, n_linguist_variables:int=3, fuzzy_type=fs.FUZZY_SETS.t1, domain:list=None,
+                 tolerance:float=0.01, alpha:float=0.950, beta:float=0.025, gamma:float=0.025) -> None:
+        '''
+        Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
+
+        :param X: np array or pandas dataframe samples x features.
+        :param y: np vector containing the target classes. vector sample
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param n_class: number of classes in the problem. If None (as default) it will be computed from the data.
+        :param linguistic_variables: list of linguistic variables precomputed. If given, the rest of conflicting arguments are ignored.
+        :param n_linguistic_variables: number of linguistic variables per antecedent.
+        :param fuzzy_type: Define the fuzzy set or fuzzy set extension used as linguistic variable.
+        :param domain: list with the upper and lower domains of each input variable. If None (as default) it will stablish the empirical min/max as the limits.
+        '''
+        try:
+            self.var_names = list(X.columns)
+            self.X = X.values
+        except AttributeError:
+            self.X = X
+            self.var_names = [str(ix) for ix in range(X.shape[1])]
+
+        try:
+            self.tolerance = tolerance
+        except KeyError:
+            self.tolerance = 0.001
+
+        self.y = y
+        self.classes_names = np.unique(y)
+        self.nRules = nRules
+        self.nAnts = nAnts
+        self.nCons = 1  # This is fixed to MISO rules.
+
+        if n_classes is not None:
+            self.n_classes = n_classes
+        else:
+            self.n_classes = len(np.unique(y))
+
+        if linguistic_variables is not None:
+            self._init_precomputed_vl(linguistic_variables, X)
+        else:
+            self._init_optimize_vl(
+                fuzzy_type, n_linguist_variables)
+
+        if self.domain is None:
+            # If all the variables are numerical, then we can compute the min/max of the domain.
+            if np.all([np.issubdtype(self.X[:, ix].dtype, np.number) for ix in range(self.X.shape[1])]):
+                self.min_bounds = np.min(self.X, axis=0)
+                self.max_bounds = np.max(self.X, axis=0)
+            else:
+                self.min_bounds = np.zeros(self.X.shape[1])
+                self.max_bounds = np.zeros(self.X.shape[1])
+
+                for ix in range(self.X.shape[1]):
+                    if np.issubdtype(self.X[:, ix].dtype, np.number):
+                        self.min_bounds[ix] = np.min(self.X[:, ix])
+                        self.max_bounds[ix] = np.max(self.X[:, ix])
+                    else:
+                        self.min_bounds[ix] = 0
+                        self.max_bounds[ix] = len(np.unique(self.X[:, ix]))
+        else:
+            self.min_bounds, self.max_bounds = self.domain
+
+        self.antecedents_referencial = [np.linspace(
+            self.min_bounds[ix], self.max_bounds[ix], 100) for ix in range(self.X.shape[1])]
+
+        possible_antecedent_bounds = np.array(
+            [[0, self.X.shape[1] - 1]] * self.nAnts * self.nRules)  
+        vl_antecedent_bounds = np.array(
+            [[-1, self.n_lv_possible - 1]] * self.nAnts * self.nRules) # -1 means not caring
+        antecedent_bounds = np.concatenate(
+            (possible_antecedent_bounds, vl_antecedent_bounds))
+        vars_antecedent = {ix: Integer(
+            bounds=antecedent_bounds[ix]) for ix in range(len(antecedent_bounds))}
+        aux_counter = len(vars_antecedent)
+
+        if self.lvs is None:
+            assert self.n_lv_possible >= 1, 'At least 1 possible value for a linguistic variable is required.'
+
+            self.feature_domain_bounds = np.array(
+                [[0, 99] for ix in range(self.X.shape[1])])
+            size_multiplier = 4 if self.fuzzy_type == fs.FUZZY_SETS.t1 else 8
+            membership_bounds = np.concatenate(
+                [self.feature_domain_bounds] * self.n_lv_possible * size_multiplier)
+            vars_memeberships = {
+                aux_counter + ix: Integer(bounds=membership_bounds[ix]) for ix in range(len(membership_bounds))}
+            aux_counter += len(vars_memeberships)
+
+        final_consequent_bounds = np.array(
+            [[-1, self.n_classes - 1]] * self.nRules)
+        vars_consequent = {aux_counter + ix: Integer(
+            bounds=final_consequent_bounds[ix]) for ix in range(len(final_consequent_bounds))}
+
+        if self.lvs is None:
+            vars = {key: val for d in [
+                vars_antecedent, vars_memeberships, vars_consequent] for key, val in d.items()}
+            varbound = np.concatenate(
+                (antecedent_bounds, membership_bounds, final_consequent_bounds), axis=0)
+        else:
+            vars = {key: val for d in [vars_antecedent,
+                                       vars_consequent] for key, val in d.items()}
+            varbound = np.concatenate(
+                (antecedent_bounds, final_consequent_bounds), axis=0)
+
+        nVar = len(varbound)
+        self.single_gen_size = nVar
+        self.alpha_ = alpha
+        self.beta_ = beta
+        self.gamma_ = gamma
+
+        if thread_runner is not None:
+            super().__init__(
+                vars=vars,
+                n_var=nVar,
+                n_obj=1,
+                elementwise=True,
+                vtype=int,
+                xl=varbound[:, 0],
+                xu=varbound[:, 1],
+                elementwise_runner=thread_runner)
+        else:
+            super().__init__(
+                vars=vars,
+                n_var=nVar,
+                n_obj=1,
+                elementwise=True,
+                vtype=int,
+                xl=varbound[:, 0],
+                xu=varbound[:, 1])
+
+
+    def encode_rulebase(self, rule_base: rules.MasterRuleBase, optimize_lv: bool) -> np.array:
+        '''
+        Given a rule base, constructs the corresponding gene associated with that rule base.
+
+        GENE STRUCTURE
+
+        First: antecedents chosen by each rule. Size: nAnts * nRules (index of the antecedent)
+        Second: Variable linguistics used. Size: nAnts * nRules
+        Third: Parameters for the fuzzy partitions of the chosen variables. Size: nAnts * self.n_linguistic_variables * 8|4 (2 trapezoidal memberships if t2)
+        Four: Consequent classes. Size: nRules
+
+        :param rule_base: rule base object.
+        :param optimize_lv: if True, the gene is prepared to optimize the membership functions.
+        :param antecedents_referencial: list of lists. Each list contains the referencial for each variable.  Required only if optimize_lv is True.
+        :return: np array of size self.single_gen_size.
+        '''
+        gene = np.zeros((self.single_gen_size,))
+
+        n_lv_possible = len(rule_base.rule_bases[0].antecedents[0].linguistic_variables)
+        fz_type = rule_base.fuzzy_type()
+        rule_consequents = rule_base.get_consequents()
+        nreal_rules = len(rule_consequents)
+        mf_size = 4 if fz_type == fs.FUZZY_SETS.t1 else 8
+
+        # Pointer to the fourth section of the gene: consequents
+        if optimize_lv:
+            # If lv memberships are optimized.
+            fourth_pointer = 2 * self.nAnts * self.nRules + \
+                len(rule_base.antecedents) * n_lv_possible * mf_size
+        else:
+            # If no memberships are optimized.
+            fourth_pointer = 2 * self.nAnts * self.nRules
+
+        # First and second sections of the gene: antecedents and linguistic variables
+        for i0, rule in enumerate(rule_base.get_rules()):  # Reconstruct the rules
+            first_pointer = i0 * self.nAnts
+            second_pointer = (self.nRules * self.nAnts) + i0 * self.nAnts
+
+            for ax, linguistic_variable in enumerate(rule.antecedents):
+                gene[first_pointer + ax] = ax
+                gene[second_pointer + ax] = linguistic_variable
+            
+            # Update the fourth section of the gene: consequents using the fourth pointer
+            gene[fourth_pointer + i0] = rule_consequents[i0]
+
+        # Fill the rest of the rules with don't care values
+        nvoid_rules = self.nRules - nreal_rules
+        for vx in range(nvoid_rules):
+            first_pointer = nreal_rules * self.nAnts + vx * self.nAnts
+            second_pointer = (self.nRules * self.nAnts) + nreal_rules * self.nAnts + vx * self.nAnts
+
+            for ax, linguistic_variable in enumerate(rule.antecedents):
+                gene[first_pointer + ax] = ax
+                gene[second_pointer + ax] = -1
+            
+            # Update the fourth section of the gene: consequents using the fourth pointer
+            gene[fourth_pointer + nreal_rules + vx] = -1
+
+        if optimize_lv:
+            # If lv memberships are optimized.
+            third_pointer = 2 * self.nAnts * self.nRules
+            aux_pointer = 0
+            for ix, fuzzy_variable in enumerate(rule_base.get_antecedents()):
+                for linguistic_variable in range(n_lv_possible):
+                    fz_parameters = fuzzy_variable[linguistic_variable].membership_parameters
+                    for jx, fz_parameter in enumerate(fz_parameters):
+                        closest_idx = (np.abs(np.asarray(self.antecedents_referencial[ix]) - fz_parameter)).argmin()
+                        gene[third_pointer + aux_pointer] = closest_idx
+                        aux_pointer += 1
+                    
+        return np.array(list(map(int, gene)))
+        
+
+
+    def _construct_ruleBase(self, x: np.array, fz_type: fs.FUZZY_SETS, **kwargs) -> rules.MasterRuleBase:
+        '''
+        Given a subject, it creates a rulebase according to its specification.
+
+        :param x: gen of a rulebase. type: dict.
+        :param fz_type: a enum type. Check fuzzy_sets for complete specification (two fields, t1 and t2, to mark which fs you want to use)
+        :return: a rulebase object.
+
+        kwargs:
+            - time_moment: if temporal fuzzy sets are used with different partitions for each time interval, 
+                            then this parameter is used to specify which time moment is being used.
+        '''
+
+        rule_list = [[] for _ in range(self.n_classes)]
+
+        mf_size = 4 if fz_type == fs.FUZZY_SETS.t1 else 8
+        '''
+        GEN STRUCTURE
+
+        First: antecedents chosen by each rule. Size: nAnts * nRules
+        Second: Variable linguistics used. Size: nAnts * nRules
+        Third: Parameters for the fuzzy partitions of the chosen variables. Size: X.shape[1] * self.n_linguistic_variables * 8|4 (2 trapezoidal memberships if t2)
+        Four: Consequent classes. Size: nRules (fixed to 4 right now)
+        '''
+        if self.lvs is None:
+            # If memberships are optimized.
+            fourth_pointer = 2 * self.nAnts * self.nRules + \
+                self.X.shape[1] * self.n_lv_possible * mf_size
+        else:
+            # If no memberships are optimized.
+            fourth_pointer = 2 * self.nAnts * self.nRules
+
+        aux_pointer = 0
+        min_domain = np.min(self.X, axis=0)
+        max_domain = np.max(self.X, axis=0)
+
+        # Integer sampling doesnt work fine in pymoo, so we do this (which is btw what pymoo is really doing if you just set integer optimization)
+        try:
+            # subject might come as a dict.
+            x = np.array(list(x.values())).astype(int)
+        except AttributeError:
+            x = x.astype(int)
+
+        for i0 in range(self.nRules):  # Reconstruct the rules
+            first_pointer = i0 * self.nAnts
+            chosen_ants = x[first_pointer:first_pointer + self.nAnts]
+
+            second_pointer = (i0 * self.nAnts) + (self.nAnts * self.nRules)
+            # Shape: self.nAnts + self.n_lv_possible  + 1
+            antecedent_parameters = x[second_pointer:second_pointer+self.nAnts]
+
+            init_rule_antecedents = np.zeros(
+                (self.X.shape[1],)) - 1  # -1 is dont care
+            for jx, ant in enumerate(chosen_ants):
+                if self.lvs is not None:
+                    antecedent_parameters[jx] = min(antecedent_parameters[jx], len(self.lvs[ant]) - 1)
+                else:
+                    antecedent_parameters[jx] = min(antecedent_parameters[jx], self.n_lv_possible - 1)
+
+                init_rule_antecedents[ant] = antecedent_parameters[jx]
+
+            consequent_idx = x[fourth_pointer + aux_pointer]
+            assert consequent_idx < self.n_classes, "Consequent class is not valid. Something in the gene is wrong."
+            aux_pointer += 1
+ 
+            if consequent_idx != -1:
+                rule_list[consequent_idx].append(
+                    rules.RuleSimple(init_rule_antecedents, 0))
+
+        # If we optimize the membership functions
+        if self.lvs is None:
+            third_pointer = 2 * self.nAnts * self.nRules
+            aux_pointer = 0
+            antecedents = []
+
+            for fuzzy_variable in range(self.X.shape[1]):
+                linguistic_variables = []
+
+                for linguistic_variable in range(self.n_lv_possible):
+                    parameter_pointer = third_pointer + aux_pointer
+                    fz_parameters_idx = x[parameter_pointer:parameter_pointer + mf_size]
+                    fz_parameters = self.antecedents_referencial[fuzzy_variable][fz_parameters_idx]
+                    aux_pointer += mf_size
+
+                    if fz_type == fs.FUZZY_SETS.t2:
+                        fz_parameters[0:6] = np.sort(fz_parameters[0:6])
+                        mu = [np.min(fz_parameters[0:2]), fz_parameters[2],
+                              fz_parameters[3], np.max(fz_parameters[4:6])]
+                        ml = [np.max(fz_parameters[0:2]), fz_parameters[2],
+                              fz_parameters[3], np.min(fz_parameters[4:6])]
+                        height = fz_parameters[6] / np.max(fz_parameters)
+
+                        ivfs = fs.IVFS(self.vl_names[linguistic_variable], ml, mu,
+                                       (min_domain[fuzzy_variable], max_domain[fuzzy_variable]), lower_height=height)
+                    else:
+                        ivfs = fs.FS(self.vl_names[linguistic_variable], np.sort(fz_parameters[0:4]),
+                                     (min_domain[fuzzy_variable], max_domain[fuzzy_variable]))
+                    linguistic_variables.append(ivfs)
+
+                antecedents.append(fs.fuzzyVariable(
+                    self.var_names[fuzzy_variable], linguistic_variables))
+        else:
+            try:
+                antecedents = self.lvs[kwargs['time_moment']]
+            except:
+                antecedents = self.lvs
+
+        for i in range(self.n_classes):
+            if fz_type == fs.FUZZY_SETS.temporal:
+                fz_type = self.lvs[0][0].inside_type()
+
+            if fz_type == fs.FUZZY_SETS.t1:
+                rule_base = rules.RuleBaseT1(antecedents, rule_list[i])
+            elif fz_type == fs.FUZZY_SETS.t2:
+                rule_base = rules.RuleBaseT2(antecedents, rule_list[i])
+            elif fz_type == fs.FUZZY_SETS.gt2:
+                rule_base = rules.RuleBaseGT2(antecedents, rule_list[i])
+            
+
+            if i == 0:
+                res = rules.MasterRuleBase([rule_base], self.classes_names)
+            else:
+                res.add_rule_base(rule_base)
+
+        res.rename_cons(self.classes_names)
+
+        return res
+
+
+    def _evaluate(self, x: np.array, out: dict, *args, **kwargs):
+        '''
+        :param x: array of train samples. x shape = features
+            those features are the parameters to optimize.
+
+        :param out: dict where the F field is the fitness. It is used from the outside.
+        '''
+        ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
+
+        if len(ruleBase.get_rules()) > 0:
+            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self.alpha_, self.beta_, self.gamma_, self._precomputed_truth)
+        else:
+            score = 0.0
+        
+        out["F"] = 1 - score
+    
+
+    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.975, beta:float=0.0125, gamma:float=0.0125, precomputed_truth:np.array=None) -> float:
+        '''
+        Fitness function for the optimization problem.
+        :param ruleBase: RuleBase object
+        :param X: array of train samples. X shape = (n_samples, n_features)
+        :param y: array of train labels. y shape = (n_samples,)
+        :param tolerance: float. Tolerance for the size evaluation.
+        :param alpha: float. Weight for the accuracy term.
+        :param beta: float. Weight for the average rule size term.
+        :param gamma: float. Weight for the number of rules term.
+        :param precomputed_truth: np array. If given, it will be used as the truth values for the evaluation.
+        :return: float. Fitness value.
+        '''
+        if precomputed_truth is None:
+            precomputed_truth = rules.compute_antecedents_memberships(ruleBase.antecedents, X)
+
+        ev_object = evr.evalRuleBase(ruleBase, X, y, precomputed_truth=precomputed_truth)
+        ev_object.add_full_evaluation()
+        ruleBase.purge_rules(tolerance)
+
+        if len(ruleBase.get_rules()) > 0: 
+            score_acc = ev_object.classification_eval()
+            score_rules_size = ev_object.size_antecedents_eval(tolerance)
+            score_nrules = ev_object.effective_rulesize_eval(tolerance)
+
+            score = score_acc * alpha + score_rules_size * beta + score_nrules * gamma
+        else:
+            score = 0.0
+            
+        return score
+    
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-
-'''
-Module to keep track of the usage of the different features of the library. 
-Asks nicely for permission before saving anything.
-
-'''
-import os as _os
-import atexit
-
-from enum import Enum
-
-usage_categories = Enum('uses', ['FuzzySets', 'Funcs', 'Persistence', 'Visualization', 'FuzzyCognitiveMaps', 'RuleMining', 'Classification'])
-
-def instance_dict_usage():
-    # Inits the categories to track
-    return {usage_categories.FuzzySets: {'t1':0 , 't2': 0, 'gt2': 0, 'temporal': 0, 'temporal_t2': 0},
-                usage_categories.Funcs: {'fit': 0, 'precompute_labels': 0, 'opt_labels':0},
-                usage_categories.Persistence : {'persistence_write': 0,
-                    'persistence_read': 0},
-                usage_categories.FuzzyCognitiveMaps : {'fcm_create': 0, 'fcm_report': 0},
-                usage_categories.Visualization : {'plot_rules': 0, 'plot_graph': 0, 'print_rules': 0, 'plot_fuzzy_variable': 0},
-                usage_categories.RuleMining : {'mine_rulebase' : 0},
-                usage_categories.Classification : {'double_go': 0, 'data_mining': 0}
-    }
-
-
-def rename_dict_usage_categories():
-    global usage_data
-    str_names = ['Fuzzy sets', 'Utils and training', 'Persistence', 'Fuzzy Cognitive Maps', 'Visualization', 'Rule Mining', 'Classification']
-    new_usage = {}
-
-    for ix, (key, value) in enumerate(usage_data.items()):
-        new_usage[str_names[ix]] = value
-
-    usage_data = new_usage
-
-
-def send_data():
-    global path_usage_data_folder
-    # Send the data to the developers using a sfpt server (TODO)
-    import paramiko
-
-    host = "sftp.upv.es"
-    port = 22
-
-    files_to_send = _os.listdir(path_usage_data_folder)
-
-    # create ssh client 
-    ssh_client = paramiko.SSHClient()
-
-    # remote server credentials
-    host = "hostname"
-    # username = "username"
-    # password = "password"
-    port = port
-
-    ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-    ssh_client.connect(hostname=host,port=port)
-
-    # create an SFTP client object
-    ftp = ssh_client.open_sftp()
-
-    for file in files_to_send:
-        # send a file from the remote server
-        ftp.put(path_usage_data_folder + '/' + file, '/home/' + file)
-    
-    # Send also the logger file
-    ftp.put('ex_fuzzy.log', '/home/ex_fuzzy.log')
-    
-    # close the connection
-    ftp.close()
-    ssh_client.close()
-
-    # Clear the logger file
-    with open('ex_fuzzy.log', 'w') as f:
-        f.write('')
-
-
-def main():
-    global path_usage_data_folder
-    # Open the usage file from user
-    file_name = 'usage_data_permission.txt'
-    directory = _os.path.dirname(_os.path.realpath(__file__))
-
-    if file_name not in _os.listdir(directory):
-        # Get input from user
-        print('exFuzzy:')
-        print('Do you want to share your usage data with the developers?')
-        print('This data will be used to improve the library. It will also help us to acquire funding for the project.')
-        print('If you agree, we will store the number of times you use each functionality in a file called "usage_data.txt".')
-        print('This file will be stored in the same folder as the library.')
-        print('If you do not agree, we will not store any data.')
-        print('If you agree, type "[y]es". If you do not agree, type "no".')
-        user_input = None
-
-        while user_input not in ['no', 'yes', 'y']:
-            user_input = input()
-
-            if user_input not in ['no', 'yes', 'y']:
-                print('Answer not understood, please repeat: If you agree, type "[y]es". If you do not agree, type "no".')
-        
-        with open(_os.path.join(directory, file_name), 'w') as f:
-            f.write(user_input)
-
-    # Read the usage file
-    with open(_os.path.join(directory, file_name), 'r') as f:
-        user_input = f.read()
-
-    save_usage_flag = user_input == 'yes' or user_input == 'y'
-
-    if save_usage_flag:
-        import logging
-        logger = logging.getLogger(__name__)
-        logger.setLevel(logging.DEBUG)
-        # Create handlers
-        c_handler = logging.StreamHandler()
-        f_handler = logging.FileHandler(_os.path.join(directory, 'ex_fuzzy.log'))
-        c_handler.setLevel(logging.WARNING)
-        f_handler.setLevel(logging.DEBUG)
-        # Create formatters and add it to handlers
-        c_format = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
-        f_format = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        c_handler.setFormatter(c_format)
-        f_handler.setFormatter(f_format)
-        # Add handlers to the logger
-        logger.addHandler(c_handler)
-        logger.addHandler(f_handler)
-
-        # Create usage reports
-        @atexit.register
-        def save_usage():
-            # Saves the usage in the corresponding file
-            path_usage_data = _os.path.join(path_usage_data_folder, 'usage_data_' + str(number_files) + '.txt')
-            rename_dict_usage_categories()
-            import json
-            # Save the usage as a json
-            with open(_os.path.join(directory, path_usage_data), 'w') as f:
-                json.dump(usage_data, f)
-            
-            # Send the data to the developers
-            # send_data()
-        # Create usage data dictionary
-        usage_data = instance_dict_usage()
-
-        path_usage_data_folder = 'usage_data'
-        if path_usage_data_folder not in _os.listdir(directory):
-            _os.mkdir(_os.path.join(directory, path_usage_data_folder))
-        
-        number_files = len(_os.listdir(_os.path.join(directory, path_usage_data_folder)))
-
-        if number_files > 100:
-            # Avoid a large number of files
-            while number_files > 100:
-                _os.remove(_os.path.join(directory, path_usage_data_folder, 'usage_data_' + str(number_files-1) + '.txt'))
-                number_files = len(_os.listdir(path_usage_data_folder))
-
-
-        atexit.register(save_usage)
-
-save_usage_flag = False
-if __name__ == '__main__':
+
+'''
+Module to keep track of the usage of the different features of the library. 
+Asks nicely for permission before saving anything.
+
+'''
+import os as _os
+import atexit
+
+from enum import Enum
+
+usage_categories = Enum('uses', ['FuzzySets', 'Funcs', 'Persistence', 'Visualization', 'FuzzyCognitiveMaps', 'RuleMining', 'Classification'])
+
+def instance_dict_usage():
+    # Inits the categories to track
+    return {usage_categories.FuzzySets: {'t1':0 , 't2': 0, 'gt2': 0, 'temporal': 0, 'temporal_t2': 0, 'categorical': 0},
+                usage_categories.Funcs: {'fit': 0, 'precompute_labels': 0, 'opt_labels':0},
+                usage_categories.Persistence : {'persistence_write': 0,
+                    'persistence_read': 0},
+                usage_categories.FuzzyCognitiveMaps : {'fcm_create': 0, 'fcm_report': 0},
+                usage_categories.Visualization : {'plot_rules': 0, 'plot_graph': 0, 'print_rules': 0, 'plot_fuzzy_variable': 0},
+                usage_categories.RuleMining : {'mine_rulebase' : 0},
+                usage_categories.Classification : {'double_go': 0, 'data_mining': 0}
+    }
+
+
+def rename_dict_usage_categories():
+    global usage_data
+    str_names = ['Fuzzy sets', 'Utils and training', 'Persistence', 'Fuzzy Cognitive Maps', 'Visualization', 'Rule Mining', 'Classification']
+    new_usage = {}
+
+    for ix, (key, value) in enumerate(usage_data.items()):
+        new_usage[str_names[ix]] = value
+
+    usage_data = new_usage
+
+
+def send_data():
+    global path_usage_data_folder
+    # Send the data to the developers using a sfpt server (TODO)
+    import paramiko
+
+    host = "sftp.upv.es"
+    port = 22
+
+    files_to_send = _os.listdir(path_usage_data_folder)
+
+    # create ssh client 
+    ssh_client = paramiko.SSHClient()
+
+    # remote server credentials
+    host = "hostname"
+    # username = "username"
+    # password = "password"
+    port = port
+
+    ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+    ssh_client.connect(hostname=host,port=port)
+
+    # create an SFTP client object
+    ftp = ssh_client.open_sftp()
+
+    for file in files_to_send:
+        # send a file from the remote server
+        ftp.put(path_usage_data_folder + '/' + file, '/home/' + file)
+    
+    # Send also the logger file
+    ftp.put('ex_fuzzy.log', '/home/ex_fuzzy.log')
+    
+    # close the connection
+    ftp.close()
+    ssh_client.close()
+
+    # Clear the logger file
+    with open('ex_fuzzy.log', 'w') as f:
+        f.write('')
+
+
+def main():
+    global path_usage_data_folder
+    # Open the usage file from user
+    file_name = 'usage_data_permission.txt'
+    directory = _os.path.dirname(_os.path.realpath(__file__))
+
+    if file_name not in _os.listdir(directory):
+        # Get input from user
+        print('exFuzzy:')
+        print('Do you want to share your usage data with the developers?')
+        print('This data will be used to improve the library. It will also help us to acquire funding for the project.')
+        print('If you agree, we will store the number of times you use each functionality in a file called "usage_data.txt".')
+        print('This file will be stored in the same folder as the library.')
+        print('If you do not agree, we will not store any data.')
+        print('If you agree, type "[y]es". If you do not agree, type "no".')
+        user_input = None
+
+        while user_input not in ['no', 'yes', 'y']:
+            user_input = input()
+
+            if user_input not in ['no', 'yes', 'y']:
+                print('Answer not understood, please repeat: If you agree, type "[y]es". If you do not agree, type "no".')
+        
+        with open(_os.path.join(directory, file_name), 'w') as f:
+            f.write(user_input)
+
+    # Read the usage file
+    with open(_os.path.join(directory, file_name), 'r') as f:
+        user_input = f.read()
+
+    save_usage_flag = user_input == 'yes' or user_input == 'y'
+
+    if save_usage_flag:
+        import logging
+        logger = logging.getLogger(__name__)
+        logger.setLevel(logging.DEBUG)
+        # Create handlers
+        c_handler = logging.StreamHandler()
+        f_handler = logging.FileHandler(_os.path.join(directory, 'ex_fuzzy.log'))
+        c_handler.setLevel(logging.WARNING)
+        f_handler.setLevel(logging.DEBUG)
+        # Create formatters and add it to handlers
+        c_format = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
+        f_format = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        c_handler.setFormatter(c_format)
+        f_handler.setFormatter(f_format)
+        # Add handlers to the logger
+        logger.addHandler(c_handler)
+        logger.addHandler(f_handler)
+
+        # Create usage reports
+        @atexit.register
+        def save_usage():
+            # Saves the usage in the corresponding file
+            path_usage_data = _os.path.join(path_usage_data_folder, 'usage_data_' + str(number_files) + '.txt')
+            rename_dict_usage_categories()
+            import json
+            # Save the usage as a json
+            with open(_os.path.join(directory, path_usage_data), 'w') as f:
+                json.dump(usage_data, f)
+            
+            # Send the data to the developers
+            # send_data()
+        # Create usage data dictionary
+        usage_data = instance_dict_usage()
+
+        path_usage_data_folder = 'usage_data'
+        if path_usage_data_folder not in _os.listdir(directory):
+            _os.mkdir(_os.path.join(directory, path_usage_data_folder))
+        
+        number_files = len(_os.listdir(_os.path.join(directory, path_usage_data_folder)))
+
+        if number_files > 100:
+            # Avoid a large number of files
+            while number_files > 100:
+                _os.remove(_os.path.join(directory, path_usage_data_folder, 'usage_data_' + str(number_files-1) + '.txt'))
+                number_files = len(_os.listdir(path_usage_data_folder))
+
+
+        atexit.register(save_usage)
+
+save_usage_flag = False
+if __name__ == '__main__':
     pass
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-'''
-Load the rules of a fuzzy rules system using plain text format.
-
-'''
-import numpy as np
-
-try:
-    from . import fuzzy_sets as fs
-    from . import rules
-    from . import maintenance as mnt
-
-except ImportError:
-    import fuzzy_sets as fs
-    import rules
-    import maintenance as mnt
-
-
-def load_fuzzy_rules(rules_printed: str, fuzzy_variables: list) -> rules.MasterRuleBase:
-    '''
-    Load the rules from a string.
-    
-    :param rules_printed: string with the rules. Follows the specification given by the same printing method of rules.MasterRuleBase
-    :param fuzzy_variables: list with the linguistic variables. Objects of FuzzyVariable class.
-    
-    '''
-    if mnt.save_usage_flag:
-        mnt.usage_data[mnt.usage_categories.Persistence]['persistence_read'] += 1
-        
-    consequent = 0
-    linguistic_variables_names = [linguistic_variable.name for linguistic_variable in fuzzy_variables]
-    value_names = [x.name for x in fuzzy_variables[0]]
-    fz_type = fuzzy_variables[0].fuzzy_type()
-    consequent_names = []
-    for line in rules_printed.splitlines():
-        if line.startswith('IF'):
-            #Is a rule
-            antecedents , consequent_ds = line.split('WITH')
-            consequent_ds = consequent_ds.split(',')[0].strip()
-            init_rule_antecedents = np.zeros(
-                (len(fuzzy_variables),)) - 1  # -1 is dont care
-            
-            for antecedent in antecedents.split('AND'):
-                antecedent = antecedent.replace('IF', '').strip()
-                antecedent_name, antecedent_value = antecedent.split('IS')
-                antecedent_name = antecedent_name.strip()
-                antecedent_value = antecedent_value.strip()
-                antecedent_index = linguistic_variables_names.index(antecedent_name)
-                antecedent_value_index = value_names.index(antecedent_value)
-
-                init_rule_antecedents[antecedent_index] = antecedent_value_index
-                
-            rule_simple = rules.RuleSimple(init_rule_antecedents, 0)
-            rule_simple.score = float(consequent_ds[3:].strip()) # We remove the 'DS ' and the last space
-            reconstructed_rules.append(rule_simple)
-
-        elif line.startswith('Rules'):
-            #New consequent
-            consequent_name = line.split(':')[-1].strip()
-            consequent_names.append(consequent_name)
-            if consequent > 0:
-                if fz_type == fs.FUZZY_SETS.t1:
-                    rule_base = rules.RuleBaseT1(fuzzy_variables, reconstructed_rules)
-                elif fz_type == fs.FUZZY_SETS.t2:
-                    rule_base = rules.RuleBaseT2(fuzzy_variables, reconstructed_rules)
-                elif fz_type == fs.FUZZY_SETS.gt2:
-                    rule_base = rules.RuleBaseGT2(fuzzy_variables, reconstructed_rules)
-                                    
-            if consequent == 1:
-                mrule_base = rules.MasterRuleBase([rule_base])
-            elif consequent > 1:
-                mrule_base.add_rule_base(rule_base)
-
-            reconstructed_rules = []
-            consequent += 1
-    
-    # We add the last rule base
-    if fz_type == fs.FUZZY_SETS.t1:
-        rule_base = rules.RuleBaseT1(fuzzy_variables, reconstructed_rules)
-    elif fz_type == fs.FUZZY_SETS.t2:
-        rule_base = rules.RuleBaseT2(fuzzy_variables, reconstructed_rules)
-    elif fz_type == fs.FUZZY_SETS.gt2:
-        rule_base = rules.RuleBaseGT2(fuzzy_variables, reconstructed_rules)
-        
-    mrule_base.add_rule_base(rule_base) 
-    mrule_base.rename_cons(consequent_names)
-
-    return mrule_base
-
+'''
+Load the rules of a fuzzy rules system using plain text format.
+
+'''
+import numpy as np
+
+try:
+    from . import fuzzy_sets as fs
+    from . import rules
+    from . import maintenance as mnt
+
+except ImportError:
+    import fuzzy_sets as fs
+    import rules
+    import maintenance as mnt
+
+
+def load_fuzzy_rules(rules_printed: str, fuzzy_variables: list) -> rules.MasterRuleBase:
+    '''
+    Load the rules from a string.
+    
+    :param rules_printed: string with the rules. Follows the specification given by the same printing method of rules.MasterRuleBase
+    :param fuzzy_variables: list with the linguistic variables. Objects of FuzzyVariable class.
+    
+    '''
+    if mnt.save_usage_flag:
+        mnt.usage_data[mnt.usage_categories.Persistence]['persistence_read'] += 1
+        
+    consequent = 0
+    linguistic_variables_names = [linguistic_variable.name for linguistic_variable in fuzzy_variables]
+    value_names = [x.name for x in fuzzy_variables[0]]
+    fz_type = fuzzy_variables[0].fuzzy_type()
+    consequent_names = []
+    for line in rules_printed.splitlines():
+        if line.startswith('IF'):
+            #Is a rule
+            antecedents , consequent_ds = line.split('WITH')
+            consequent_ds = consequent_ds.split(',')[0].strip()
+            init_rule_antecedents = np.zeros(
+                (len(fuzzy_variables),)) - 1  # -1 is dont care
+            
+            for antecedent in antecedents.split('AND'):
+                antecedent = antecedent.replace('IF', '').strip()
+                antecedent_name, antecedent_value = antecedent.split('IS')
+                antecedent_name = antecedent_name.strip()
+                antecedent_value = antecedent_value.strip()
+                antecedent_index = linguistic_variables_names.index(antecedent_name)
+                antecedent_value_index = value_names.index(antecedent_value)
+
+                init_rule_antecedents[antecedent_index] = antecedent_value_index
+                
+            rule_simple = rules.RuleSimple(init_rule_antecedents, 0)
+            rule_simple.score = float(consequent_ds[3:].strip()) # We remove the 'DS ' and the last space
+            reconstructed_rules.append(rule_simple)
+
+        elif line.startswith('Rules'):
+            #New consequent
+            consequent_name = line.split(':')[-1].strip()
+            consequent_names.append(consequent_name)
+            if consequent > 0:
+                if fz_type == fs.FUZZY_SETS.t1:
+                    rule_base = rules.RuleBaseT1(fuzzy_variables, reconstructed_rules)
+                elif fz_type == fs.FUZZY_SETS.t2:
+                    rule_base = rules.RuleBaseT2(fuzzy_variables, reconstructed_rules)
+                elif fz_type == fs.FUZZY_SETS.gt2:
+                    rule_base = rules.RuleBaseGT2(fuzzy_variables, reconstructed_rules)
+                                    
+            if consequent == 1:
+                mrule_base = rules.MasterRuleBase([rule_base])
+            elif consequent > 1:
+                mrule_base.add_rule_base(rule_base)
+
+            reconstructed_rules = []
+            consequent += 1
+    
+    # We add the last rule base
+    if fz_type == fs.FUZZY_SETS.t1:
+        rule_base = rules.RuleBaseT1(fuzzy_variables, reconstructed_rules)
+    elif fz_type == fs.FUZZY_SETS.t2:
+        rule_base = rules.RuleBaseT2(fuzzy_variables, reconstructed_rules)
+    elif fz_type == fs.FUZZY_SETS.gt2:
+        rule_base = rules.RuleBaseGT2(fuzzy_variables, reconstructed_rules)
+        
+    mrule_base.add_rule_base(rule_base) 
+    mrule_base.rename_cons(consequent_names)
+
+    return mrule_base
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-"""
-Module to perform rule mining in a pandas dataframe or numpy array. The methods use the support of the different itemsets to look for good 
-rule candidates. It can be used then by a Genetic optimizator from evolutionary_fit module to search the optimal combination of them.
-
-"""
-import typing
-from itertools import product, combinations
-
-import pandas as pd
-import numpy as np
-
-try:
-    from . import rules as rl
-    from . import fuzzy_sets as fs
-    from . import maintenance as mnt
-    from . import utils
-except ImportError:
-    import utils
-    import rules as rl
-    import fuzzy_sets as fs
-    import maintenance as mnt
-
-
-def _generate_combinations(lists: list, k: int) -> typing.Iterator:
-    '''
-    Generate all the combinations between elements of different lists of length k without repeting elements of the same list.
-
-    :param lists: list of lists.
-    :param k: integer with the length of the combinations.
-    :return: a list with all the combinations.
-    '''
-    # Get all combinations of elements for k
-    all_combs = combinations(np.arange(len(lists)), k)
-    
-    # For those elements, get the cartesian product between them
-    for comb in all_combs:
-        selected_lists = [lists[x] for x in comb]
-        all_combinations = product(*selected_lists)
-
-        # Add them to the global combination list
-        yield all_combinations
-
-
-def rule_search(data: pd.DataFrame, fuzzy_variables: dict[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=None) -> list:
-    '''
-    Computes the apriori algorithm for the given dataframe and threshold the support.
-    
-    :param data: Dataframe of shape: samples x features
-    :param fuzzy variables: dict that maps each feature name with a fuzzy variable.
-    :param support_threshold: minimum support to consider frequent an itemset.
-    :return: all the frequent itemsets as a list.
-    '''
-    n_linguist_variables = len(fuzzy_variables[0])
-    list_possible_vars = []
-    for ix in range(len(fuzzy_variables)):
-        list_possible_vars.append([(ix, ax) for ax in range(n_linguist_variables)])
-
-    memberships = [fuzzy_variables[ix](data.iloc[:, ix].values) for ix in range(data.shape[1])]
-    freq_itemsets = []
-
-    if max_depth is None:
-        max_depth = data.shape[1]
-    
-    # For all possible lengths
-    for r in range(max_depth):
-        all_r_combs = _generate_combinations(list_possible_vars, r+1)
-
-        # Iterate through the possible itemsets
-        for itemsets in all_r_combs:
-            for ix, itemset in enumerate(itemsets):
-                relevant_memberships = []
-                for item in itemset:
-                    item_var, item_vl = item
-                    relevant_memberships.append([memberships[item_var][item_vl]])
-                
-                array_membership = np.array(relevant_memberships).T[:,0,:]
-                support = np.mean(np.min(array_membership, axis=1))
-                if fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.t2 or fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.gt2:
-                    support = np.mean(support, axis=1)
-
-                if support > support_threshold:
-                    freq_itemsets.append(itemset) 
-
-    return freq_itemsets
-
-
-def generate_rules_from_itemsets(itemsets:list, nAnts:int) -> list[rl.RuleSimple]:
-    '''
-    Given a list of itemsets, it creates the rules for each one and returns a list of rules containing them.
-
-    :param itemsets: list of tuple (antecedent, linguistic variable value) 
-    :param nAnts: number of possible antecedents.
-    :return: the rules for ech itemset.
-    '''
-    rules = []
-    for itemset in itemsets:
-        template = np.ones((nAnts, )) * -1
-        for ant, vl in itemset:
-            template[ant] = vl
-        
-        rule = rl.RuleSimple(list(template))
-        rules.append(rule)
-
-    return rules
-
-
-def mine_rulebase_support(x: pd.DataFrame, fuzzy_variables:list[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=3) -> rl.RuleBase:
-    '''
-    Search the data for associations that are frequent given a list of fuzzy variables for each antecedent.
-
-    :param x: the data to mine. Dims: samples x features.
-    :param fuzzy_variables: list of the fuzzy variables for each of the input variables.
-    :param support_threshold: minimum threshold to decide if prune or not the rule.
-    :param max_depth: maximum number of antecedents per rule.
-    :return: a rulebase object with the rules denoted as good.
-    '''
-    
-    if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.RuleMining]['mine_rulebase'] += 1
-            
-    freq_itemsets = rule_search(x, fuzzy_variables, support_threshold, max_depth)
-    rule_list = generate_rules_from_itemsets(freq_itemsets, len(fuzzy_variables))
-
-    fuzzy_type = fuzzy_variables[0].fs_type
-
-    if fuzzy_type == fs.FUZZY_SETS.t1:
-        rule_base = rl.RuleBaseT1(fuzzy_variables, rule_list)
-    elif fuzzy_type == fs.FUZZY_SETS.t2:
-        rule_base = rl.RuleBaseT2(fuzzy_variables, rule_list)
-    elif fuzzy_type == fs.FUZZY_SETS.gt2:
-        rule_base = rl.RuleBaseGT2(fuzzy_variables, rule_list)
-    
-    return rule_base
-
-
-def prune_rules_confidence_lift(x: pd.DataFrame, y:np.array, rules: rl.MasterRuleBase, fuzzy_variables: list[fs.fuzzyVariable], confidence_threshold:float=0.5, 
-                                lift_threshold:float=1.05):
-    '''
-    Removes the rules from the rule base that do not meet a minimum value for confidence and lift measures.
-
-    Confidence is the ratio of rules that have a particular antecedent and consequent, and those that only have the antecedent.
-    Lift is ratio between confidence and expected confidence, which is the percentage of class samples in the original data.
-
-    :param x: data to mine. samples x features.
-    :param y: class vector.
-    :param rules: MasterRuleBase object with the rules to prune.
-    :param fuzzy_variables: a list of the fuzzy variables per antecedent.
-    :param confidence_threshold: minimum confidence required to the rules.
-    :param lift_threshold: minimum lift required to the rules.
-    '''
-    for ix, rule_base in enumerate(rules):
-        delete_list = []
-        relevant_class = ix
-        relevant_class_samples = x.loc[np.equal(y, relevant_class), :]
-
-        for jx, rule in enumerate(rule_base):
-            real_nAnts = sum([ant != -1 for ant in rule])
-            global_membership_array = np.zeros((x.shape[0], real_nAnts))
-            class_samples_membership_array = np.zeros((relevant_class_samples.shape[0], real_nAnts))
-            ant_counter = 0
-            for zx, antecedent in enumerate(rule):
-                if antecedent != -1:
-                    global_membership_array[:, ant_counter] = fuzzy_variables[zx](x[fuzzy_variables[zx].name])[antecedent]
-                    class_samples_membership_array[:, ant_counter] = fuzzy_variables[zx](relevant_class_samples[fuzzy_variables[zx].name])[antecedent]
-                    ant_counter += 1
-
-            # Compute rule confidence
-            global_support = np.mean(np.min(global_membership_array, axis=1), axis=0)
-            class_support = np.mean(np.min(class_samples_membership_array, axis=1), axis=0)
-            if fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.t2 or fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.gt2:
-                    global_support = np.mean(global_support, axis=1)
-                    class_support = np.mean(class_support, axis=1)
-
-            rule_confidence = class_support / global_support
-            rule_lift = rule_confidence / np.mean(np.equal(relevant_class, y))
-
-            if rule_confidence < confidence_threshold or rule_lift < lift_threshold:
-                delete_list.append(jx)
-
-        rule_base.remove_rules(delete_list)
-
-
-def simple_mine_rulebase(x: pd.DataFrame, fuzzy_type:fs.FUZZY_SETS=fs.FUZZY_SETS.t1, support_threshold:float=0.05, max_depth:int=3) -> rl.RuleBase:
-    '''
-    Search the data for associations that are frequent. Computes the fuzzy variables using a 3 label partition (low, medium, high).
-
-    :param x: the data to mine. Dims: samples x features.
-    :param fuzzy_type: fuzzy type to use.
-    :param support_threshold: minimum threshold to decide if prune or not the rule.
-    :param max_depth: maximum number of antecedents per rule.
-    :return: a rulebase object with the rules denoted as good.
-    '''
-    
-    precomputed_partitions = utils.construct_partitions(x, fuzzy_type)
-    return mine_rulebase_support(x, precomputed_partitions, support_threshold, max_depth)
-
-
-def multiclass_mine_rulebase(x: pd.DataFrame, y: np.array, fuzzy_variables:list[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=3,
-                             confidence_threshold:float=0.05, lift_threshold:float=1.05) -> rl.MasterRuleBase:
-    '''
-    Search the data for associations that are frequent and have good confidence/lift values given a list of fuzzy variables for each antecedent. Computes a different ruleBase for each 
-    class and then uses them to form a MasterRuleBase.
-
-    :param x: the data to mine. Dims: samples x features.
-    :param fuzzy_variables: list of the fuzzy variables for each of the input variables.
-    :param support_threshold: minimum threshold to decide if prune or not the rule.
-    :param max_depth: maximum number of antecedents per rule.
-    :param confidence_threshold: minimum confidence value.
-    :param lift_threshold: 
-    :return: a rulebase object with the rules denoted as good.
-    '''
-    unique_classes = np.unique(y)
-    rulebases = []
-    for yclass in unique_classes:
-        selected_samples = np.equal(yclass, y) 
-        selected_x = x.loc[selected_samples, :]
-
-        rulebase = mine_rulebase_support(selected_x, fuzzy_variables, support_threshold, max_depth)
-        rulebases.append(rulebase)
-
-    master_rulebase = rl.MasterRuleBase(rulebases, list(map(str, unique_classes)))
-    prune_rules_confidence_lift(x, y, master_rulebase, fuzzy_variables, confidence_threshold, lift_threshold)
-    return master_rulebase
-
-
-def simple_multiclass_mine_rulebase(x: pd.DataFrame, y: np.array, fuzzy_type:fs.FUZZY_SETS, support_threshold:float=0.05, max_depth:int=3,
-                                    confidence_threshold:float=0.5, lift_threshold:float=1.1) -> rl.MasterRuleBase:
-    '''
-    Search the data for associations that are frequent and have good confidence/lift values given a list of fuzzy variables for each antecedent. 
-    Computes a different ruleBase for each class and then uses them to form a MasterRuleBase.
-
-    Computes the fuzzy variables using a 3 label partition (low, medium, high).
-
-    :param x: the data to mine. Dims: samples x features.
-    :param fuzzy_type: fuzzy type to use.
-    :param support_threshold: minimum threshold to decide if prune or not the rule.
-    :param max_depth: maximum number of antecedents per rule.
-    :return: a rulebase object with the rules denoted as good.
-    '''
-    precomputed_partitions = utils.construct_partitions(x, fuzzy_type)
-    return multiclass_mine_rulebase(x, y, precomputed_partitions, support_threshold, max_depth, 
-                                    confidence_threshold=confidence_threshold, lift_threshold=lift_threshold)
-
-
-
-
-
+"""
+Module to perform rule mining in a pandas dataframe or numpy array. The methods use the support of the different itemsets to look for good 
+rule candidates. It can be used then by a Genetic optimizator from evolutionary_fit module to search the optimal combination of them.
+
+"""
+import typing
+from itertools import product, combinations
+
+import pandas as pd
+import numpy as np
+
+try:
+    from . import rules as rl
+    from . import fuzzy_sets as fs
+    from . import maintenance as mnt
+    from . import utils
+except ImportError:
+    import utils
+    import rules as rl
+    import fuzzy_sets as fs
+    import maintenance as mnt
+
+
+def _generate_combinations(lists: list, k: int) -> typing.Iterator:
+    '''
+    Generate all the combinations between elements of different lists of length k without repeting elements of the same list.
+
+    :param lists: list of lists.
+    :param k: integer with the length of the combinations.
+    :return: a list with all the combinations.
+    '''
+    # Get all combinations of elements for k
+    all_combs = combinations(np.arange(len(lists)), k)
+    
+    # For those elements, get the cartesian product between them
+    for comb in all_combs:
+        selected_lists = [lists[x] for x in comb]
+        all_combinations = product(*selected_lists)
+
+        # Add them to the global combination list
+        yield all_combinations
+
+
+def rule_search(data: pd.DataFrame, fuzzy_variables: dict[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=None) -> list:
+    '''
+    Computes the apriori algorithm for the given dataframe and threshold the support.
+    
+    :param data: Dataframe of shape: samples x features
+    :param fuzzy variables: dict that maps each feature name with a fuzzy variable.
+    :param support_threshold: minimum support to consider frequent an itemset.
+    :return: all the frequent itemsets as a list.
+    '''
+    n_linguist_variables = len(fuzzy_variables[0])
+    list_possible_vars = []
+    for ix in range(len(fuzzy_variables)):
+        list_possible_vars.append([(ix, ax) for ax in range(n_linguist_variables)])
+
+    memberships = [fuzzy_variables[ix](data.iloc[:, ix].values) for ix in range(data.shape[1])]
+    freq_itemsets = []
+
+    if max_depth is None:
+        max_depth = data.shape[1]
+    
+    # For all possible lengths
+    for r in range(max_depth):
+        all_r_combs = _generate_combinations(list_possible_vars, r+1)
+
+        # Iterate through the possible itemsets
+        for itemsets in all_r_combs:
+            for ix, itemset in enumerate(itemsets):
+                relevant_memberships = []
+                for item in itemset:
+                    item_var, item_vl = item
+                    relevant_memberships.append([memberships[item_var][item_vl]])
+                
+                array_membership = np.array(relevant_memberships).T[:,0,:]
+                support = np.mean(np.min(array_membership, axis=1))
+                if fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.t2 or fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.gt2:
+                    support = np.mean(support, axis=1)
+
+                if support > support_threshold:
+                    freq_itemsets.append(itemset) 
+
+    return freq_itemsets
+
+
+def generate_rules_from_itemsets(itemsets:list, nAnts:int) -> list[rl.RuleSimple]:
+    '''
+    Given a list of itemsets, it creates the rules for each one and returns a list of rules containing them.
+
+    :param itemsets: list of tuple (antecedent, linguistic variable value) 
+    :param nAnts: number of possible antecedents.
+    :return: the rules for ech itemset.
+    '''
+    rules = []
+    for itemset in itemsets:
+        template = np.ones((nAnts, )) * -1
+        for ant, vl in itemset:
+            template[ant] = vl
+        
+        rule = rl.RuleSimple(list(template))
+        rules.append(rule)
+
+    return rules
+
+
+def mine_rulebase_support(x: pd.DataFrame, fuzzy_variables:list[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=3) -> rl.RuleBase:
+    '''
+    Search the data for associations that are frequent given a list of fuzzy variables for each antecedent.
+
+    :param x: the data to mine. Dims: samples x features.
+    :param fuzzy_variables: list of the fuzzy variables for each of the input variables.
+    :param support_threshold: minimum threshold to decide if prune or not the rule.
+    :param max_depth: maximum number of antecedents per rule.
+    :return: a rulebase object with the rules denoted as good.
+    '''
+    
+    if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.RuleMining]['mine_rulebase'] += 1
+            
+    freq_itemsets = rule_search(x, fuzzy_variables, support_threshold, max_depth)
+    rule_list = generate_rules_from_itemsets(freq_itemsets, len(fuzzy_variables))
+
+    fuzzy_type = fuzzy_variables[0].fs_type
+
+    if fuzzy_type == fs.FUZZY_SETS.t1:
+        rule_base = rl.RuleBaseT1(fuzzy_variables, rule_list)
+    elif fuzzy_type == fs.FUZZY_SETS.t2:
+        rule_base = rl.RuleBaseT2(fuzzy_variables, rule_list)
+    elif fuzzy_type == fs.FUZZY_SETS.gt2:
+        rule_base = rl.RuleBaseGT2(fuzzy_variables, rule_list)
+    
+    return rule_base
+
+
+def prune_rules_confidence_lift(x: pd.DataFrame, y:np.array, rules: rl.MasterRuleBase, fuzzy_variables: list[fs.fuzzyVariable], confidence_threshold:float=0.5, 
+                                lift_threshold:float=1.05):
+    '''
+    Removes the rules from the rule base that do not meet a minimum value for confidence and lift measures.
+
+    Confidence is the ratio of rules that have a particular antecedent and consequent, and those that only have the antecedent.
+    Lift is ratio between confidence and expected confidence, which is the percentage of class samples in the original data.
+
+    :param x: data to mine. samples x features.
+    :param y: class vector.
+    :param rules: MasterRuleBase object with the rules to prune.
+    :param fuzzy_variables: a list of the fuzzy variables per antecedent.
+    :param confidence_threshold: minimum confidence required to the rules.
+    :param lift_threshold: minimum lift required to the rules.
+    '''
+    for ix, rule_base in enumerate(rules):
+        delete_list = []
+        relevant_class = ix
+        relevant_class_samples = x.loc[np.equal(y, relevant_class), :]
+
+        for jx, rule in enumerate(rule_base):
+            real_nAnts = sum([ant != -1 for ant in rule])
+            global_membership_array = np.zeros((x.shape[0], real_nAnts))
+            class_samples_membership_array = np.zeros((relevant_class_samples.shape[0], real_nAnts))
+            ant_counter = 0
+            for zx, antecedent in enumerate(rule):
+                if antecedent != -1:
+                    global_membership_array[:, ant_counter] = fuzzy_variables[zx](x[fuzzy_variables[zx].name])[antecedent]
+                    class_samples_membership_array[:, ant_counter] = fuzzy_variables[zx](relevant_class_samples[fuzzy_variables[zx].name])[antecedent]
+                    ant_counter += 1
+
+            # Compute rule confidence
+            global_support = np.mean(np.min(global_membership_array, axis=1), axis=0)
+            class_support = np.mean(np.min(class_samples_membership_array, axis=1), axis=0)
+            if fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.t2 or fuzzy_variables[0].fuzzy_type == fs.FUZZY_SETS.gt2:
+                    global_support = np.mean(global_support, axis=1)
+                    class_support = np.mean(class_support, axis=1)
+
+            rule_confidence = class_support / global_support
+            rule_lift = rule_confidence / np.mean(np.equal(relevant_class, y))
+
+            if rule_confidence < confidence_threshold or rule_lift < lift_threshold:
+                delete_list.append(jx)
+
+        rule_base.remove_rules(delete_list)
+
+
+def simple_mine_rulebase(x: pd.DataFrame, fuzzy_type:fs.FUZZY_SETS=fs.FUZZY_SETS.t1, support_threshold:float=0.05, max_depth:int=3) -> rl.RuleBase:
+    '''
+    Search the data for associations that are frequent. Computes the fuzzy variables using a 3 label partition (low, medium, high).
+
+    :param x: the data to mine. Dims: samples x features.
+    :param fuzzy_type: fuzzy type to use.
+    :param support_threshold: minimum threshold to decide if prune or not the rule.
+    :param max_depth: maximum number of antecedents per rule.
+    :return: a rulebase object with the rules denoted as good.
+    '''
+    
+    precomputed_partitions = utils.construct_partitions(x, fuzzy_type)
+    return mine_rulebase_support(x, precomputed_partitions, support_threshold, max_depth)
+
+
+def multiclass_mine_rulebase(x: pd.DataFrame, y: np.array, fuzzy_variables:list[fs.fuzzyVariable], support_threshold:float=0.05, max_depth:int=3,
+                             confidence_threshold:float=0.05, lift_threshold:float=1.05) -> rl.MasterRuleBase:
+    '''
+    Search the data for associations that are frequent and have good confidence/lift values given a list of fuzzy variables for each antecedent. Computes a different ruleBase for each 
+    class and then uses them to form a MasterRuleBase.
+
+    :param x: the data to mine. Dims: samples x features.
+    :param fuzzy_variables: list of the fuzzy variables for each of the input variables.
+    :param support_threshold: minimum threshold to decide if prune or not the rule.
+    :param max_depth: maximum number of antecedents per rule.
+    :param confidence_threshold: minimum confidence value.
+    :param lift_threshold: 
+    :return: a rulebase object with the rules denoted as good.
+    '''
+    unique_classes = np.unique(y)
+    rulebases = []
+    for yclass in unique_classes:
+        selected_samples = np.equal(yclass, y) 
+        selected_x = x.loc[selected_samples, :]
+
+        rulebase = mine_rulebase_support(selected_x, fuzzy_variables, support_threshold, max_depth)
+        rulebases.append(rulebase)
+
+    master_rulebase = rl.MasterRuleBase(rulebases, list(map(str, unique_classes)))
+    prune_rules_confidence_lift(x, y, master_rulebase, fuzzy_variables, confidence_threshold, lift_threshold)
+    return master_rulebase
+
+
+def simple_multiclass_mine_rulebase(x: pd.DataFrame, y: np.array, fuzzy_type:fs.FUZZY_SETS, support_threshold:float=0.05, max_depth:int=3,
+                                    confidence_threshold:float=0.5, lift_threshold:float=1.1) -> rl.MasterRuleBase:
+    '''
+    Search the data for associations that are frequent and have good confidence/lift values given a list of fuzzy variables for each antecedent. 
+    Computes a different ruleBase for each class and then uses them to form a MasterRuleBase.
+
+    Computes the fuzzy variables using a 3 label partition (low, medium, high).
+
+    :param x: the data to mine. Dims: samples x features.
+    :param fuzzy_type: fuzzy type to use.
+    :param support_threshold: minimum threshold to decide if prune or not the rule.
+    :param max_depth: maximum number of antecedents per rule.
+    :return: a rulebase object with the rules denoted as good.
+    '''
+    precomputed_partitions = utils.construct_partitions(x, fuzzy_type)
+    return multiclass_mine_rulebase(x, y, precomputed_partitions, support_threshold, max_depth, 
+                                    confidence_threshold=confidence_threshold, lift_threshold=lift_threshold)
+
+
+
+
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,684 +1,684 @@
-'''
-Expansion of the base fuzzy sets, adding temporal fuzzy sets.
-
-Contains functions to model the temporal fuzzy sets, temporal fuzzy variables and temporal rule bases.
-It also contains functions to evaluate the fuzzy rulebases obtained.
-
-'''
-import enum
-
-import numpy as np
-import pandas as pd
-
-from sklearn.metrics import accuracy_score, f1_score, precision_score, recall_score, confusion_matrix, matthews_corrcoef
-from pymoo.algorithms.soo.nonconvex.ga import GA
-from pymoo.core.problem import Problem
-from pymoo.optimize import minimize
-from pymoo.operators.sampling.rnd import IntegerRandomSampling
-from pymoo.operators.crossover.sbx import SBX
-from pymoo.operators.mutation.pm import PolynomialMutation
-from pymoo.core.variable import Integer
-from multiprocessing.pool import ThreadPool
-from pymoo.core.problem import StarmapParallelization
-
-try:
-    from . import fuzzy_sets as fs
-    from . import maintenance as mnt
-    from . import rules as rl
-    from . import evolutionary_fit as evf
-    from . import vis_rules
-    from . import eval_rules as evr
-except:
-    import fuzzy_sets as fs
-    import maintenance as mnt
-    import rules as rl
-    import evolutionary_fit as evf
-    import vis_rules
-    import eval_rules as evr
-
-
-TMP_FUZZY_SETS = enum.Enum(
-    "NEW_FUZZY_SETS",
-    ['temporal', 'temporal_t2', 'temporal_gt2']
-)
-NEW_FUZZY_SETS = enum.Enum(
-    "FUZZY_SETS",
-    [(es.name, es.value) for es in fs.FUZZY_SETS] + [(es.name, es.name) for es in TMP_FUZZY_SETS]
-)
-
-fs.FUZZY_SETS = NEW_FUZZY_SETS
-### DEFINE THE FUZZY SET ####
-class temporalFS(fs.FS):
-    '''
-    Class to implement temporal fuzzy sets.
-    '''
-
-    def __init__(self, std_fuzzy_set: fs.FS, conditional_variable: np.array) -> None:
-        '''
-        Creates a temporal fuzzy set.
-
-        :param std_fuzzy_set: FS. Standard fuzzy set that contains the non-temporal aware memberhsip function.
-        :param conditional_variable: np.array. The variable that expresses the different temporal moments. Shape (time discrete moments, ).
-        '''
-        if mnt.save_usage_flag:
-            mnt.usage_data[mnt.usage_categories.FuzzySets][self.type().name] += 1
-            
-        self.std_set = std_fuzzy_set
-        self.tmp_function = conditional_variable
-        self.time = None
-        self.name = std_fuzzy_set.name
-
-        if std_fuzzy_set.type() == fs.FUZZY_SETS.t1:
-            self.membership_parameters = std_fuzzy_set.membership_parameters
-        elif std_fuzzy_set.type() == fs.FUZZY_SETS.t2:
-            self.secondMF_upper = std_fuzzy_set.secondMF_upper
-            self.secondMF_lower = std_fuzzy_set.secondMF_lower
-        elif std_fuzzy_set.type() == fs.FUZZY_SETS.gt2:
-            self.secondary_memberships = std_fuzzy_set.secondary_memberships
-            self.alpha_cuts = std_fuzzy_set.alpha_cuts
-
-
-    def membership(self, input: np.array, time: int=None) -> np.array:
-        '''
-        Computes the membership of each sample and in each time for the fs.
-
-        :param input: array temporal_time x samples.
-        :time: int. Time moment to compute the membership. If none, looks for a fixed time
-        :return: array temporal_time x samples.
-        '''
-        if time is None:
-            assert self.time is not None, 'Temporal fuzzy set has no fixed time. Please, fix a time or provide a time to compute the membership.'
-            time = self.time
-
-        return self.std_set.membership(input) * self.tmp_function[time]
-
-
-    def type(self) -> fs.FUZZY_SETS:
-        '''
-        Returns the type of the fuzzy set. (temporal)
-        '''
-        return fs.FUZZY_SETS.temporal
-    
-
-    def inside_type(self) -> fs.FUZZY_SETS:
-        '''
-        Returns the type of the og fuzzy set computed before the time dependency.
-        '''
-        return self.std_set.type()
-    
-
-    def fix_time(self, time: int) -> None:
-        '''
-        Fixes the time of the temporal fuzzy set.
-
-        :param time: int. Time moment to fix.
-        :return: FS. Fuzzy set with the fixed time.
-        '''
-        self.time = time
-
-
-
-#### DEFINE THE FUZZY VARIABLE ####
-class temporalFuzzyVariable(fs.fuzzyVariable):
-    '''
-    Class to implement a temporal fuzzy variable.
-    '''
-
-    def __init__(self, name: str, fuzzy_sets: list[temporalFS]) -> None:
-        '''
-        Creates a temporal fuzzy variable.
-
-        :param str: name of the variable.
-        :param fuzzy_sets: list of the fuzzy sets pre-time dependencies.
-        '''
-        self.linguistic_variables = []
-        self.name = name
-        self.time = None
-        for ix, fs in enumerate(fuzzy_sets):
-            self.linguistic_variables.append(fs)
-
-        self.fs_type = self.linguistic_variables[0].type()
-
-
-    def fix_time(self, time: int) -> None:
-        '''
-        Fixes the time of the temporal fuzzy variable.
-
-        :param time: int. Time moment to fix.
-        '''
-        self.time = time
-
-
-    def compute_memberships(self, x: np.array, time: int=None) -> dict:
-        '''
-        Computes the membership to each of the FS in the fuzzy variables.
-
-        :param x: numeric value or array. Computes the membership to each of the IVFS in the fuzzy variables.
-        :param time: int. Time moment to compute the membership.
-        :return: list of floats. Membership to each of the FS in the fuzzy variables.
-        '''
-        if time is None:
-            assert self.time is not None, 'Temporal fuzzy variable has no fixed time. Please, fix a time or provide a time to compute the membership.'
-            time = self.time
-
-        res = []
-
-        for fuzzy_set in self.linguistic_variables:
-            res.append(fuzzy_set.membership(x, time))
-
-        return res
-    
-
-    def n_time_moments(self) -> int:
-        '''
-        Returns the number of time moments of the temporal fuzzy variable.
-
-        :return: int. Number of time moments of the temporal fuzzy variable.
-        '''
-        return self.linguistic_variables[0].tmp_function.shape[0]
-
-
-#### DEFINE THE RULE BASE WITH TEMPORAL DEPENDENCIES ####
-class temporalMasterRuleBase(rl.MasterRuleBase):
-    '''
-    This class is a temporal extension of the MasterRuleBase class. It includes a list of
-    rule bases for each time step.
-    '''
-    def __init__(self, rule_base: list[rl.MasterRuleBase], time_step_names: list[str]=None):
-        '''
-        Constructor of the temporalMasterRuleBase class.
-
-        :param rule_base: list of rule bases.
-        :param time_steps: number of time steps.
-        '''
-        super().__init__(rule_base)
-        self.time_steps = np.arange(len(rule_base))
-        self.time_mrule_bases = rule_base
-
-        if time_step_names is None:
-            self.time_step_names = [str(x) for x in self.time_steps]
-        else:
-            self.time_step_names = time_step_names
-        
-        for ix, mrb in enumerate(rule_base):
-            for jx, rb in enumerate(mrb):
-                for antecedent in rb.antecedents:
-                    antecedent.fix_time(ix)
-        
-        self.antecedents = rule_base[0].antecedents
-                     
-
-    def add_rule(self, rule: rl.RuleSimple, consequent: int, time_step: int) -> None:
-        '''
-        Adds a rule to the rule base of the given consequent.
-
-        :param rule: rule to add.
-        :param consequent: index of the rule base to add the rule.
-        :param time_step: time step of the rule base to add the rule.
-        '''
-        self.time_mrule_bases[time_step][consequent].add_rule(rule)
-
-
-    def get_rulebase_matrix(self) -> list[np.array]:
-        '''
-        Returns a list with the rulebases for each antecedent in matrix format.
-
-        :return: list with the rulebases for each antecedent in matrix format.
-        '''
-        return [a.get_rulebase_matrix() for x in self.time_mrule_bases for a in x]
-
-
-    def get_scores(self) -> np.array:
-        '''
-        Returns the dominance score for each rule in all the rulebases.
-
-        :return: array with the dominance score for each rule in all the rulebases.
-        '''
-        res = []
-        for rule_bases in self.time_mrule_bases:    
-            for rb in rule_bases:
-                res.append(rb.scores())
-
-        res = [x for x in res if len(x) > 0]
-
-        return np.concatenate(res, axis=0)
-
-
-    def compute_firing_strenghts(self, X: np.array, time_moments: list[int]) -> np.array:
-        '''
-        Computes the firing strength of each rule for each sample.
-
-        :param X: array with the values of the inputs.
-        :return: array with the firing strength of each rule for each sample.
-        '''
-        aux = []
-        time_moments = np.array(time_moments)
-
-        for time_moment, rule_bases in enumerate(self.time_mrule_bases):
-            actual_moment = np.equal(time_moments, time_moment)
-            for ix in range(len(rule_bases)):
-                if rule_bases.fuzzy_type() == fs.FUZZY_SETS.t2:
-                    aux.append(np.mean(rule_bases[ix].compute_rule_antecedent_memberships(X), axis=2) * np.expand_dims(actual_moment, axis=1))
-                elif rule_bases.fuzzy_type() == fs.FUZZY_SETS.gt2:
-                    aux.append(np.mean(rule_bases[ix].compute_rule_antecedent_memberships(X), axis=2) * np.expand_dims(actual_moment, axis=1))
-                else:
-                    aux.append(rule_bases[ix].compute_rule_antecedent_memberships(X) * np.expand_dims(actual_moment, axis=1))
-
-        # Firing strengths shape: samples x rules
-        return np.concatenate(aux, axis=1)
-
-
-    def winning_rule_predict(self, X: np.array, time_moments: int) -> np.array:
-        '''
-        Returns the winning rule for each sample. Takes into account dominance scores if already computed.
-
-        :param X: array with the values of the inputs.
-        :return: array with the winning rule for each sample.
-        '''
-        consequents = []
-        for ix, mrb in enumerate(self.time_mrule_bases):
-            for jx, rb in enumerate(mrb):
-                for rule in rb:
-                    consequents.append(jx)
-
-        # consequents = sum([[ix]*len(self[ix].get_rules())
-        #                  for ix in range(len(self.rule_bases))], [])  # The sum is for flatenning
-        firing_strengths = self.compute_firing_strenghts(X, time_moments)
-
-        if self.time_mrule_bases[0].fuzzy_type() == fs.FUZZY_SETS.t2 or self.time_mrule_bases[0].fuzzy_type() == fs.FUZZY_SETS.gt2:
-            association_degrees = np.mean(self.get_scores(), axis=1) * firing_strengths
-        else:
-            association_degrees = self.get_scores() * firing_strengths
-
-
-        winning_rules = np.argmax(association_degrees, axis=1)
-
-        return np.array([consequents[ix] for ix in winning_rules])
-
-
-    def add_rule_base(self, rule_base: rl.RuleBase, time: int) -> None:
-        '''
-        Adds a rule base to the list of rule bases.
-
-        :param rule_base: rule base to add.
-        '''
-        self.time_mrule_bases[time].add_rule_base(rule_base)
-
-
-    def print_rules(self, return_rules=False) -> None:
-        '''
-        Print all the rules for all the consequents.
-        '''
-        res = ''
-        for zx, time in enumerate(self.time_mrule_bases):
-            res += 'Rules for time step: ' + self.time_step_names[zx] + '\n'
-            res += '----------------\n' 
-            for ix, ruleBase in enumerate(time):
-                res += 'Consequent: ' + time.consequent_names[ix] + '\n'
-                res += ruleBase.print_rules(True)
-                res += '\n'
-            res += '----------------\n'
-
-        if return_rules:
-            return res
-        else:
-            print(res)
-
-
-    def get_rules(self) -> list[rl.RuleSimple]:
-        '''
-        Returns a list with all the rules.
-
-        :return: list with all the rules.
-        '''
-        return [rule for mruleBase in self.rule_bases for rule in mruleBase.get_rules()]
-
-
-    def fuzzy_type(self) -> fs.FUZZY_SETS:
-        '''
-        Returns the correspoing type of the RuleBase using the enum type in the fuzzy_sets module.
-
-        :return: the corresponding fuzzy set type of the RuleBase.
-        '''
-        return self.time_mrule_bases[0].rule_bases[0].fuzzy_type()
-
-
-    def purge_rules(self, tolerance=0.001) -> None:
-        '''
-        Delete the roles with a dominance score lower than the tolerance.
-
-        :param tolerance: tolerance to delete the rules.
-        '''
-        for mruleBase in self.time_mrule_bases:
-            mruleBase.purge_rules(tolerance)
-
-
-    def __getitem__(self, item: int) -> rl.RuleBase:
-        '''
-        Returns the corresponding time rulebase.
-
-        :param item: index of the rulebase.
-        :return: the corresponding rulebase.
-        '''
-        return self.time_mrule_bases[item]
-
-
-    def __len__(self) -> int:
-        '''
-        Returns the number of rule bases.
-        '''
-        return len(self.time_mrule_bases)
-
-
-    def get_consequents(self) -> list[int]:
-        '''
-        Returns a list with the consequents of each rule base.
-
-        :return: list with the consequents of each rule base.
-        '''
-        return sum([x.get_consequents() for ix, x in enumerate(self.time_mrule_bases)], [])
-    
-
-    def get_rulebases(self) -> list[rl.RuleBase]:
-        '''
-        Returns a list with all the rules.
-
-        :return: list
-        '''
-        rule_bases = []
-
-        for ruleBase in self.time_mrule_bases:
-            for rule in ruleBase:
-                rule_bases.append(rule)
-        
-        return rule_bases
-    
-
-    def _winning_rules(self, X: np.array, temporal_moments: list[int]) -> np.array:
-        '''
-        Returns the winning rule for each sample. Takes into account dominance scores if already computed.
-
-        :param X: array with the values of the inputs.
-        :return: array with the winning rule for each sample.
-        '''
-        
-        firing_strengths = self.compute_firing_strenghts(X, temporal_moments)
-
-        association_degrees = self.get_scores() * firing_strengths
-
-        if (self[0].fuzzy_type() == fs.FUZZY_SETS.t2) or (self[0].fuzzy_type() == fs.FUZZY_SETS.gt2):
-            association_degrees = np.mean(association_degrees, axis=2)
-        elif self[0].fuzzy_type() == fs.FUZZY_SETS.gt2:
-            association_degrees = np.mean(association_degrees, axis=3)
-
-        winning_rules = np.argmax(association_degrees, axis=1)
-
-        return winning_rules
-        
-
-#### DEFINE THE FUZZY CLASSIFIER USING TEMPORAL FUZZY SETS ####
-class TemporalFuzzyRulesClassifier(evf.BaseFuzzyRulesClassifier):
-    '''
-    Class that is used as a classifier for a fuzzy rule based system with time dependencies. Supports precomputed and optimization of the linguistic variables.
-    '''
-
-    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0,
-                 n_linguist_variables: int = 0, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
-                 domain: list[float] = None, n_class: int=None, precomputed_rules: rl.MasterRuleBase =None, runner: int=1) -> None:
-        '''
-        Inits the optimizer with the corresponding parameters.
-
-        :param nRules: number of rules to optimize.
-        :param nAnts: max number of antecedents to use.
-        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
-        :param tolerance: tolerance for the dominance score of the rules.
-        :param n_linguist_variables: number of linguistic variables per antecedent.
-        :param verbose: if True, prints the progress of the optimization.
-        :param linguistic_variables: list of fuzzyVariables type. If None (default) the optimization process will init+optimize them.
-        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
-
-        kwargs:
-            - n_classes: number of classes to predict. Default deduces from data.
-        '''
-        super().__init__(nRules=nRules, nAnts=nAnts, fuzzy_type=fuzzy_type, tolerance=tolerance, 
-                         n_linguist_variables=n_linguist_variables, verbose=verbose, linguistic_variables=linguistic_variables, 
-                         domain=domain, n_class=n_class, precomputed_rules=precomputed_rules, runner=runner)
-    
-
-    def _contruct_tempRuleBase(self, problems, best_individuals):
-        ruleBase_temp = []
-
-        for problem, subject in zip(problems, best_individuals):
-            ruleBase_time_moment = problem._construct_ruleBase(subject, 
-                                                                self.fuzzy_type)
-            ruleBase_temp.append(ruleBase_time_moment)
-
-        return ruleBase_temp
-
-
-    def _fix_time(self, lvs: list[temporalFuzzyVariable], time: int) -> None:
-        '''
-        Fixes the time of the temporal fuzzy variables.
-
-        :param lvs: list of temporal fuzzy variables.
-        :param time: integer. Time moment to fix.
-        :return: None. The time is fixed.
-        '''
-        for lv in lvs:
-            lv.fix_time(time)
-
-
-    def fit(self, X: np.array, y: np.array, n_gen:int=50, pop_size:int=10, time_moments: np.array=None, checkpoints:int=0):
-        '''
-        Fits a fuzzy rule based classifier using a genetic algorithm to the given data.
-
-        :param X: numpy array samples x features
-        :param y: labels. integer array samples (x 1)
-        :param n_gen: integer. Number of generations to run the genetic algorithm.
-        :param pop_size: integer. Population size for each gneration.
-        :param time_moments: array of integers. Time moments associated to each sample (when temporal dependencies are present)
-        :return: None. The classifier is fitted to the data.
-        '''
-        problems = []
-        for ix in range(len(np.unique(time_moments))):
-            X_problem = X[time_moments == ix]
-            y_problem = y[time_moments == ix]
-            
-            if self.lvs is None:
-                # If Fuzzy variables need to be optimized.
-                problem = evf.FitRuleBase(X_problem, y_problem, nRules=self.nRules, nAnts=self.nAnts, tolerance=self.tolerance,
-                                    n_linguist_variables=self.n_linguist_variables, fuzzy_type=self.fuzzy_type, domain=self.domain, 
-                                    n_classes=self.n_class, thread_runner=self.thread_runner)
-            else:
-                import copy
-                time_lvs = [copy.deepcopy(aux) for aux in self.lvs]
-                self._fix_time(time_lvs, ix)
-                # If Fuzzy variables are already precomputed.       
-                problem = evf.FitRuleBase(X_problem, y_problem, nRules=self.nRules, nAnts=self.nAnts,
-                                    linguistic_variables=time_lvs, domain=self.domain, tolerance=self.tolerance, 
-                                    n_classes=self.classes_, thread_runner=self.thread_runner)
-            
-            problems.append(problem)
-
-        
-
-        best_individuals = []
-        self.performance = {}
-        for time, problem in enumerate(problems):
-            algorithm = GA(
-            pop_size=pop_size,
-            sampling=IntegerRandomSampling(),
-            crossover=SBX(prob=.3, eta=3.0),
-            mutation=PolynomialMutation(eta=7.0),
-            eliminate_duplicates=True)
-
-            if checkpoints > 0:
-                if self.verbose:
-                    print('=================================================')
-                    print('n_gen  |  n_eval  |     f_avg     |     f_min    ')
-                    print('=================================================')
-                algorithm.setup(problem, seed=33, termination=('n_gen', n_gen)) # 33? Soon...
-                for k in range(n_gen):
-                    algorithm.next()
-                    res = algorithm
-                    if self.verbose:
-                        print('%-6s | %-8s | %-8s | %-8s' % (res.n_gen, res.evaluator.n_eval, round(res.pop.get('F').mean(), 8), round(res.pop.get('F').min(), 8)))
-                    if k % checkpoints == 0:
-                        with open("checkpoint_" + str(time) + '_' + str(algorithm.n_gen), "w") as f:
-                            pop = algorithm.pop
-                            fitness_last_gen = pop.get('F')
-                            best_solution_arg = np.argmin(fitness_last_gen)
-                            best_individual = pop.get('X')[best_solution_arg, :]
-
-                            rule_base = problem._construct_ruleBase(
-                                best_individual, self.fuzzy_type)
-                            eval_performance = evr.evalRuleBase(
-                                rule_base, np.array(X), y)
-                            
-                            eval_performance.add_full_evaluation()  
-                            # self.rename_fuzzy_variables() This wont work on checkpoints!
-                            rule_base.purge_rules(self.tolerance)
-                            checkpoint_rules = rule_base.print_rules(True)
-                            f.write(checkpoint_rules)     
-
-            else:
-                res = minimize(problem,
-                            algorithm,
-                            # termination,
-                            ("n_gen", n_gen),
-                            copy_algorithm=False,
-                            save_history=False,
-                            verbose=self.verbose)
-
-            pop = res.pop
-            fitness_last_gen = pop.get('F')
-            best_solution = np.argmin(fitness_last_gen)
-            best_individual = pop.get('X')[best_solution, :]
-            best_individuals.append(best_individual)
-
-            if self.verbose:
-                print('Rule based fit for time ' + str(time) + ' completed.')
-
-        
-            self.performance[time] = 1 - fitness_last_gen[best_solution]
-
-        try:
-            self.var_names = list(X.columns)
-            self.X = X.values
-        except AttributeError:
-            self.X = X
-            self.var_names = [str(ix) for ix in range(X.shape[1])]
-
-        
-        ruleBase_temp = self._contruct_tempRuleBase(problems, best_individuals)
-
-        self.rule_base = temporalMasterRuleBase(ruleBase_temp)
-
-        self.eval_performance = evr.evalRuleBase(self.rule_base, np.array(X), y, time_moments)
-
-        self.eval_performance.add_full_evaluation()  
-        self.rename_fuzzy_variables()
-        self.rule_base.purge_rules(self.tolerance)
-
-
-    def forward(self, X: np.array, time_moments: list[int] = None) -> np.array:
-        '''
-        Returns the predicted class for each sample.
-
-        :param X: np array samples x features.
-        :param time_moments: list of integers. Time moments associated to each sample (when temporal dependencies are present)
-        :return: np array samples (x 1) with the predicted class.
-        '''
-        try:
-            X = X.values  # If X was a numpy array
-        except AttributeError:
-            pass
-        
-        return self.rule_base.winning_rule_predict(X, time_moments)
-
-
-
-    def plot_fuzzy_variables(self) -> None:
-        '''
-        Plot the fuzzy partitions in each fuzzy variable.
-        '''
-        fuzzy_variables = self.rule_base.rule_bases[0].antecedents
-
-        for ix, fv in enumerate(fuzzy_variables):
-            vis_rules.plot_fuzzy_variable(fv)
-
-
-    def get_rulebase(self) -> list[np.array]:
-        '''
-        Get the rulebase obtained after fitting the classifier to the data.
-
-        :return: a matrix format for the rulebase.
-        '''
-        return self.rule_base.get_rulebase_matrix()
-
-
-def eval_temporal_fuzzy_model(fl_classifier: evf.BaseFuzzyRulesClassifier, X_train: np.array, y_train: np.array,
-                     X_test: np.array, y_test: np.array, time_moments: list[int] = None, test_time_moments: list[int] = None,
-                     plot_rules=True, print_rules=True, plot_partitions=True, return_rules=False, print_accuracy=True, print_matthew=True) -> None:
-    '''
-    Function that evaluates a fuzzy rule based model. It also plots the rules and the fuzzy partitions.
-
-    :param fl_classifier: Fuzzy rule based model.
-    :param X_train: Training data.
-    :param y_train: Training labels.
-    :param X_test: Test data.
-    :param y_test: Test labels.
-    :param plot_rules: If True, it plots the rules.
-    :param print_rules: If True, it prints the rules.
-    :param plot_partitions: If True, it plots the fuzzy partitions.
-    :return: None
-    '''
-
-    if print_accuracy:
-      print('ACCURACY')
-      print('Train performance: ' +
-            str(np.mean(np.equal(y_train, fl_classifier.forward(X_train, time_moments)))))
-      print('Test performance: ' +
-            str(np.mean(np.equal(y_test, fl_classifier.forward(X_test, test_time_moments)))))
-      print('------------')
-    if print_matthew:
-      print('MATTHEW CORRCOEF')
-      print('Train performance: ' +
-            str(matthews_corrcoef(y_train, fl_classifier.forward(X_train, time_moments))))
-      print('Test performance: ' +
-            str(matthews_corrcoef(y_test, fl_classifier.forward(X_test, test_time_moments))))
-      print('------------')
-
-    for ix in np.unique(time_moments):
-      try:
-            X_aux = X_train[time_moments == ix, :]
-            X_aux_test = X_test[time_moments == ix, :]
-      except pd.core.indexing.InvalidIndexError:
-            X_aux = X_train.iloc[time_moments == ix, :]
-            X_aux_test = X_test.iloc[test_time_moments == ix, :]
-
-      y_aux = y_train[time_moments == ix]
-      y_aux_test = y_test[test_time_moments == ix]
-
-      if print_matthew:
-            print('MOMENT ' + str(ix))
-            print('------------')
-            print('MATTHEW CORRCOEF')
-            print('Train performance: ' +
-                  str(matthews_corrcoef(y_aux, fl_classifier.forward(X_aux, np.array([ix] * X_aux.shape[0])))))
-            print('Test performance: ' +
-                  str(matthews_corrcoef(y_aux_test, fl_classifier.forward(X_aux_test, np.array([ix] * X_aux_test.shape[0])))))
-            print('------------')
-
-    if plot_rules:
-        vis_rules.visualize_rulebase(fl_classifier)
-    if print_rules or return_rules:
-        res = fl_classifier.print_rules(return_rules)
-    if plot_partitions:
-        fl_classifier.plot_fuzzy_variables()
-      
-    if return_rules:
-        return res
-    else:
-        print(res)
-
+'''
+Expansion of the base fuzzy sets, adding temporal fuzzy sets.
+
+Contains functions to model the temporal fuzzy sets, temporal fuzzy variables and temporal rule bases.
+It also contains functions to evaluate the fuzzy rulebases obtained.
+
+'''
+import enum
+
+import numpy as np
+import pandas as pd
+
+from sklearn.metrics import accuracy_score, f1_score, precision_score, recall_score, confusion_matrix, matthews_corrcoef
+from pymoo.algorithms.soo.nonconvex.ga import GA
+from pymoo.core.problem import Problem
+from pymoo.optimize import minimize
+from pymoo.operators.sampling.rnd import IntegerRandomSampling
+from pymoo.operators.crossover.sbx import SBX
+from pymoo.operators.mutation.pm import PolynomialMutation
+from pymoo.core.variable import Integer
+from multiprocessing.pool import ThreadPool
+from pymoo.core.problem import StarmapParallelization
+
+try:
+    from . import fuzzy_sets as fs
+    from . import maintenance as mnt
+    from . import rules as rl
+    from . import evolutionary_fit as evf
+    from . import vis_rules
+    from . import eval_rules as evr
+except:
+    import fuzzy_sets as fs
+    import maintenance as mnt
+    import rules as rl
+    import evolutionary_fit as evf
+    import vis_rules
+    import eval_rules as evr
+
+
+TMP_FUZZY_SETS = enum.Enum(
+    "NEW_FUZZY_SETS",
+    ['temporal', 'temporal_t2', 'temporal_gt2']
+)
+NEW_FUZZY_SETS = enum.Enum(
+    "FUZZY_SETS",
+    [(es.name, es.value) for es in fs.FUZZY_SETS] + [(es.name, es.name) for es in TMP_FUZZY_SETS]
+)
+
+fs.FUZZY_SETS = NEW_FUZZY_SETS
+### DEFINE THE FUZZY SET ####
+class temporalFS(fs.FS):
+    '''
+    Class to implement temporal fuzzy sets.
+    '''
+
+    def __init__(self, std_fuzzy_set: fs.FS, conditional_variable: np.array) -> None:
+        '''
+        Creates a temporal fuzzy set.
+
+        :param std_fuzzy_set: FS. Standard fuzzy set that contains the non-temporal aware memberhsip function.
+        :param conditional_variable: np.array. The variable that expresses the different temporal moments. Shape (time discrete moments, ).
+        '''
+        if mnt.save_usage_flag:
+            mnt.usage_data[mnt.usage_categories.FuzzySets][self.type().name] += 1
+            
+        self.std_set = std_fuzzy_set
+        self.tmp_function = conditional_variable
+        self.time = None
+        self.name = std_fuzzy_set.name
+
+        if std_fuzzy_set.type() == fs.FUZZY_SETS.t1:
+            self.membership_parameters = std_fuzzy_set.membership_parameters
+        elif std_fuzzy_set.type() == fs.FUZZY_SETS.t2:
+            self.secondMF_upper = std_fuzzy_set.secondMF_upper
+            self.secondMF_lower = std_fuzzy_set.secondMF_lower
+        elif std_fuzzy_set.type() == fs.FUZZY_SETS.gt2:
+            self.secondary_memberships = std_fuzzy_set.secondary_memberships
+            self.alpha_cuts = std_fuzzy_set.alpha_cuts
+
+
+    def membership(self, input: np.array, time: int=None) -> np.array:
+        '''
+        Computes the membership of each sample and in each time for the fs.
+
+        :param input: array temporal_time x samples.
+        :time: int. Time moment to compute the membership. If none, looks for a fixed time
+        :return: array temporal_time x samples.
+        '''
+        if time is None:
+            assert self.time is not None, 'Temporal fuzzy set has no fixed time. Please, fix a time or provide a time to compute the membership.'
+            time = self.time
+
+        return self.std_set.membership(input) * self.tmp_function[time]
+
+
+    def type(self) -> fs.FUZZY_SETS:
+        '''
+        Returns the type of the fuzzy set. (temporal)
+        '''
+        return fs.FUZZY_SETS.temporal
+    
+
+    def inside_type(self) -> fs.FUZZY_SETS:
+        '''
+        Returns the type of the og fuzzy set computed before the time dependency.
+        '''
+        return self.std_set.type()
+    
+
+    def fix_time(self, time: int) -> None:
+        '''
+        Fixes the time of the temporal fuzzy set.
+
+        :param time: int. Time moment to fix.
+        :return: FS. Fuzzy set with the fixed time.
+        '''
+        self.time = time
+
+
+
+#### DEFINE THE FUZZY VARIABLE ####
+class temporalFuzzyVariable(fs.fuzzyVariable):
+    '''
+    Class to implement a temporal fuzzy variable.
+    '''
+
+    def __init__(self, name: str, fuzzy_sets: list[temporalFS]) -> None:
+        '''
+        Creates a temporal fuzzy variable.
+
+        :param str: name of the variable.
+        :param fuzzy_sets: list of the fuzzy sets pre-time dependencies.
+        '''
+        self.linguistic_variables = []
+        self.name = name
+        self.time = None
+        for ix, fs in enumerate(fuzzy_sets):
+            self.linguistic_variables.append(fs)
+
+        self.fs_type = self.linguistic_variables[0].type()
+
+
+    def fix_time(self, time: int) -> None:
+        '''
+        Fixes the time of the temporal fuzzy variable.
+
+        :param time: int. Time moment to fix.
+        '''
+        self.time = time
+
+
+    def compute_memberships(self, x: np.array, time: int=None) -> dict:
+        '''
+        Computes the membership to each of the FS in the fuzzy variables.
+
+        :param x: numeric value or array. Computes the membership to each of the IVFS in the fuzzy variables.
+        :param time: int. Time moment to compute the membership.
+        :return: list of floats. Membership to each of the FS in the fuzzy variables.
+        '''
+        if time is None:
+            assert self.time is not None, 'Temporal fuzzy variable has no fixed time. Please, fix a time or provide a time to compute the membership.'
+            time = self.time
+
+        res = []
+
+        for fuzzy_set in self.linguistic_variables:
+            res.append(fuzzy_set.membership(x, time))
+
+        return res
+    
+
+    def n_time_moments(self) -> int:
+        '''
+        Returns the number of time moments of the temporal fuzzy variable.
+
+        :return: int. Number of time moments of the temporal fuzzy variable.
+        '''
+        return self.linguistic_variables[0].tmp_function.shape[0]
+
+
+#### DEFINE THE RULE BASE WITH TEMPORAL DEPENDENCIES ####
+class temporalMasterRuleBase(rl.MasterRuleBase):
+    '''
+    This class is a temporal extension of the MasterRuleBase class. It includes a list of
+    rule bases for each time step.
+    '''
+    def __init__(self, rule_base: list[rl.MasterRuleBase], time_step_names: list[str]=None):
+        '''
+        Constructor of the temporalMasterRuleBase class.
+
+        :param rule_base: list of rule bases.
+        :param time_steps: number of time steps.
+        '''
+        super().__init__(rule_base)
+        self.time_steps = np.arange(len(rule_base))
+        self.time_mrule_bases = rule_base
+
+        if time_step_names is None:
+            self.time_step_names = [str(x) for x in self.time_steps]
+        else:
+            self.time_step_names = time_step_names
+        
+        for ix, mrb in enumerate(rule_base):
+            for jx, rb in enumerate(mrb):
+                for antecedent in rb.antecedents:
+                    antecedent.fix_time(ix)
+        
+        self.antecedents = rule_base[0].antecedents
+                     
+
+    def add_rule(self, rule: rl.RuleSimple, consequent: int, time_step: int) -> None:
+        '''
+        Adds a rule to the rule base of the given consequent.
+
+        :param rule: rule to add.
+        :param consequent: index of the rule base to add the rule.
+        :param time_step: time step of the rule base to add the rule.
+        '''
+        self.time_mrule_bases[time_step][consequent].add_rule(rule)
+
+
+    def get_rulebase_matrix(self) -> list[np.array]:
+        '''
+        Returns a list with the rulebases for each antecedent in matrix format.
+
+        :return: list with the rulebases for each antecedent in matrix format.
+        '''
+        return [a.get_rulebase_matrix() for x in self.time_mrule_bases for a in x]
+
+
+    def get_scores(self) -> np.array:
+        '''
+        Returns the dominance score for each rule in all the rulebases.
+
+        :return: array with the dominance score for each rule in all the rulebases.
+        '''
+        res = []
+        for rule_bases in self.time_mrule_bases:    
+            for rb in rule_bases:
+                res.append(rb.scores())
+
+        res = [x for x in res if len(x) > 0]
+
+        return np.concatenate(res, axis=0)
+
+
+    def compute_firing_strenghts(self, X: np.array, time_moments: list[int]) -> np.array:
+        '''
+        Computes the firing strength of each rule for each sample.
+
+        :param X: array with the values of the inputs.
+        :return: array with the firing strength of each rule for each sample.
+        '''
+        aux = []
+        time_moments = np.array(time_moments)
+
+        for time_moment, rule_bases in enumerate(self.time_mrule_bases):
+            actual_moment = np.equal(time_moments, time_moment)
+            for ix in range(len(rule_bases)):
+                if rule_bases.fuzzy_type() == fs.FUZZY_SETS.t2:
+                    aux.append(np.mean(rule_bases[ix].compute_rule_antecedent_memberships(X), axis=2) * np.expand_dims(actual_moment, axis=1))
+                elif rule_bases.fuzzy_type() == fs.FUZZY_SETS.gt2:
+                    aux.append(np.mean(rule_bases[ix].compute_rule_antecedent_memberships(X), axis=2) * np.expand_dims(actual_moment, axis=1))
+                else:
+                    aux.append(rule_bases[ix].compute_rule_antecedent_memberships(X) * np.expand_dims(actual_moment, axis=1))
+
+        # Firing strengths shape: samples x rules
+        return np.concatenate(aux, axis=1)
+
+
+    def winning_rule_predict(self, X: np.array, time_moments: int) -> np.array:
+        '''
+        Returns the winning rule for each sample. Takes into account dominance scores if already computed.
+
+        :param X: array with the values of the inputs.
+        :return: array with the winning rule for each sample.
+        '''
+        consequents = []
+        for ix, mrb in enumerate(self.time_mrule_bases):
+            for jx, rb in enumerate(mrb):
+                for rule in rb:
+                    consequents.append(jx)
+
+        # consequents = sum([[ix]*len(self[ix].get_rules())
+        #                  for ix in range(len(self.rule_bases))], [])  # The sum is for flatenning
+        firing_strengths = self.compute_firing_strenghts(X, time_moments)
+
+        if self.time_mrule_bases[0].fuzzy_type() == fs.FUZZY_SETS.t2 or self.time_mrule_bases[0].fuzzy_type() == fs.FUZZY_SETS.gt2:
+            association_degrees = np.mean(self.get_scores(), axis=1) * firing_strengths
+        else:
+            association_degrees = self.get_scores() * firing_strengths
+
+
+        winning_rules = np.argmax(association_degrees, axis=1)
+
+        return np.array([consequents[ix] for ix in winning_rules])
+
+
+    def add_rule_base(self, rule_base: rl.RuleBase, time: int) -> None:
+        '''
+        Adds a rule base to the list of rule bases.
+
+        :param rule_base: rule base to add.
+        '''
+        self.time_mrule_bases[time].add_rule_base(rule_base)
+
+
+    def print_rules(self, return_rules=False) -> None:
+        '''
+        Print all the rules for all the consequents.
+        '''
+        res = ''
+        for zx, time in enumerate(self.time_mrule_bases):
+            res += 'Rules for time step: ' + self.time_step_names[zx] + '\n'
+            res += '----------------\n' 
+            for ix, ruleBase in enumerate(time):
+                res += 'Consequent: ' + time.consequent_names[ix] + '\n'
+                res += ruleBase.print_rules(True)
+                res += '\n'
+            res += '----------------\n'
+
+        if return_rules:
+            return res
+        else:
+            print(res)
+
+
+    def get_rules(self) -> list[rl.RuleSimple]:
+        '''
+        Returns a list with all the rules.
+
+        :return: list with all the rules.
+        '''
+        return [rule for mruleBase in self.rule_bases for rule in mruleBase.get_rules()]
+
+
+    def fuzzy_type(self) -> fs.FUZZY_SETS:
+        '''
+        Returns the correspoing type of the RuleBase using the enum type in the fuzzy_sets module.
+
+        :return: the corresponding fuzzy set type of the RuleBase.
+        '''
+        return self.time_mrule_bases[0].rule_bases[0].fuzzy_type()
+
+
+    def purge_rules(self, tolerance=0.001) -> None:
+        '''
+        Delete the roles with a dominance score lower than the tolerance.
+
+        :param tolerance: tolerance to delete the rules.
+        '''
+        for mruleBase in self.time_mrule_bases:
+            mruleBase.purge_rules(tolerance)
+
+
+    def __getitem__(self, item: int) -> rl.RuleBase:
+        '''
+        Returns the corresponding time rulebase.
+
+        :param item: index of the rulebase.
+        :return: the corresponding rulebase.
+        '''
+        return self.time_mrule_bases[item]
+
+
+    def __len__(self) -> int:
+        '''
+        Returns the number of rule bases.
+        '''
+        return len(self.time_mrule_bases)
+
+
+    def get_consequents(self) -> list[int]:
+        '''
+        Returns a list with the consequents of each rule base.
+
+        :return: list with the consequents of each rule base.
+        '''
+        return sum([x.get_consequents() for ix, x in enumerate(self.time_mrule_bases)], [])
+    
+
+    def get_rulebases(self) -> list[rl.RuleBase]:
+        '''
+        Returns a list with all the rules.
+
+        :return: list
+        '''
+        rule_bases = []
+
+        for ruleBase in self.time_mrule_bases:
+            for rule in ruleBase:
+                rule_bases.append(rule)
+        
+        return rule_bases
+    
+
+    def _winning_rules(self, X: np.array, temporal_moments: list[int]) -> np.array:
+        '''
+        Returns the winning rule for each sample. Takes into account dominance scores if already computed.
+
+        :param X: array with the values of the inputs.
+        :return: array with the winning rule for each sample.
+        '''
+        
+        firing_strengths = self.compute_firing_strenghts(X, temporal_moments)
+
+        association_degrees = self.get_scores() * firing_strengths
+
+        if (self[0].fuzzy_type() == fs.FUZZY_SETS.t2) or (self[0].fuzzy_type() == fs.FUZZY_SETS.gt2):
+            association_degrees = np.mean(association_degrees, axis=2)
+        elif self[0].fuzzy_type() == fs.FUZZY_SETS.gt2:
+            association_degrees = np.mean(association_degrees, axis=3)
+
+        winning_rules = np.argmax(association_degrees, axis=1)
+
+        return winning_rules
+        
+
+#### DEFINE THE FUZZY CLASSIFIER USING TEMPORAL FUZZY SETS ####
+class TemporalFuzzyRulesClassifier(evf.BaseFuzzyRulesClassifier):
+    '''
+    Class that is used as a classifier for a fuzzy rule based system with time dependencies. Supports precomputed and optimization of the linguistic variables.
+    '''
+
+    def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = None, tolerance: float = 0.0,
+                 n_linguist_variables: int = 0, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
+                 domain: list[float] = None, n_class: int=None, precomputed_rules: rl.MasterRuleBase =None, runner: int=1) -> None:
+        '''
+        Inits the optimizer with the corresponding parameters.
+
+        :param nRules: number of rules to optimize.
+        :param nAnts: max number of antecedents to use.
+        :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
+        :param tolerance: tolerance for the dominance score of the rules.
+        :param n_linguist_variables: number of linguistic variables per antecedent.
+        :param verbose: if True, prints the progress of the optimization.
+        :param linguistic_variables: list of fuzzyVariables type. If None (default) the optimization process will init+optimize them.
+        :param domain: list of the limits for each variable. If None (default) the classifier will compute them empirically.
+
+        kwargs:
+            - n_classes: number of classes to predict. Default deduces from data.
+        '''
+        super().__init__(nRules=nRules, nAnts=nAnts, fuzzy_type=fuzzy_type, tolerance=tolerance, 
+                         n_linguist_variables=n_linguist_variables, verbose=verbose, linguistic_variables=linguistic_variables, 
+                         domain=domain, n_class=n_class, precomputed_rules=precomputed_rules, runner=runner)
+    
+
+    def _contruct_tempRuleBase(self, problems, best_individuals):
+        ruleBase_temp = []
+
+        for problem, subject in zip(problems, best_individuals):
+            ruleBase_time_moment = problem._construct_ruleBase(subject, 
+                                                                self.fuzzy_type)
+            ruleBase_temp.append(ruleBase_time_moment)
+
+        return ruleBase_temp
+
+
+    def _fix_time(self, lvs: list[temporalFuzzyVariable], time: int) -> None:
+        '''
+        Fixes the time of the temporal fuzzy variables.
+
+        :param lvs: list of temporal fuzzy variables.
+        :param time: integer. Time moment to fix.
+        :return: None. The time is fixed.
+        '''
+        for lv in lvs:
+            lv.fix_time(time)
+
+
+    def fit(self, X: np.array, y: np.array, n_gen:int=50, pop_size:int=10, time_moments: np.array=None, checkpoints:int=0):
+        '''
+        Fits a fuzzy rule based classifier using a genetic algorithm to the given data.
+
+        :param X: numpy array samples x features
+        :param y: labels. integer array samples (x 1)
+        :param n_gen: integer. Number of generations to run the genetic algorithm.
+        :param pop_size: integer. Population size for each gneration.
+        :param time_moments: array of integers. Time moments associated to each sample (when temporal dependencies are present)
+        :return: None. The classifier is fitted to the data.
+        '''
+        problems = []
+        for ix in range(len(np.unique(time_moments))):
+            X_problem = X[time_moments == ix]
+            y_problem = y[time_moments == ix]
+            
+            if self.lvs is None:
+                # If Fuzzy variables need to be optimized.
+                problem = evf.FitRuleBase(X_problem, y_problem, nRules=self.nRules, nAnts=self.nAnts, tolerance=self.tolerance,
+                                    n_linguist_variables=self.n_linguist_variables, fuzzy_type=self.fuzzy_type, domain=self.domain, 
+                                    n_classes=self.n_class, thread_runner=self.thread_runner)
+            else:
+                import copy
+                time_lvs = [copy.deepcopy(aux) for aux in self.lvs]
+                self._fix_time(time_lvs, ix)
+                # If Fuzzy variables are already precomputed.       
+                problem = evf.FitRuleBase(X_problem, y_problem, nRules=self.nRules, nAnts=self.nAnts,
+                                    linguistic_variables=time_lvs, domain=self.domain, tolerance=self.tolerance, 
+                                    n_classes=self.classes_, thread_runner=self.thread_runner)
+            
+            problems.append(problem)
+
+        
+
+        best_individuals = []
+        self.performance = {}
+        for time, problem in enumerate(problems):
+            algorithm = GA(
+            pop_size=pop_size,
+            sampling=IntegerRandomSampling(),
+            crossover=SBX(prob=.3, eta=3.0),
+            mutation=PolynomialMutation(eta=7.0),
+            eliminate_duplicates=True)
+
+            if checkpoints > 0:
+                if self.verbose:
+                    print('=================================================')
+                    print('n_gen  |  n_eval  |     f_avg     |     f_min    ')
+                    print('=================================================')
+                algorithm.setup(problem, seed=33, termination=('n_gen', n_gen)) # 33? Soon...
+                for k in range(n_gen):
+                    algorithm.next()
+                    res = algorithm
+                    if self.verbose:
+                        print('%-6s | %-8s | %-8s | %-8s' % (res.n_gen, res.evaluator.n_eval, round(res.pop.get('F').mean(), 8), round(res.pop.get('F').min(), 8)))
+                    if k % checkpoints == 0:
+                        with open("checkpoint_" + str(time) + '_' + str(algorithm.n_gen), "w") as f:
+                            pop = algorithm.pop
+                            fitness_last_gen = pop.get('F')
+                            best_solution_arg = np.argmin(fitness_last_gen)
+                            best_individual = pop.get('X')[best_solution_arg, :]
+
+                            rule_base = problem._construct_ruleBase(
+                                best_individual, self.fuzzy_type)
+                            eval_performance = evr.evalRuleBase(
+                                rule_base, np.array(X), y)
+                            
+                            eval_performance.add_full_evaluation()  
+                            # self.rename_fuzzy_variables() This wont work on checkpoints!
+                            rule_base.purge_rules(self.tolerance)
+                            checkpoint_rules = rule_base.print_rules(True)
+                            f.write(checkpoint_rules)     
+
+            else:
+                res = minimize(problem,
+                            algorithm,
+                            # termination,
+                            ("n_gen", n_gen),
+                            copy_algorithm=False,
+                            save_history=False,
+                            verbose=self.verbose)
+
+            pop = res.pop
+            fitness_last_gen = pop.get('F')
+            best_solution = np.argmin(fitness_last_gen)
+            best_individual = pop.get('X')[best_solution, :]
+            best_individuals.append(best_individual)
+
+            if self.verbose:
+                print('Rule based fit for time ' + str(time) + ' completed.')
+
+        
+            self.performance[time] = 1 - fitness_last_gen[best_solution]
+
+        try:
+            self.var_names = list(X.columns)
+            self.X = X.values
+        except AttributeError:
+            self.X = X
+            self.var_names = [str(ix) for ix in range(X.shape[1])]
+
+        
+        ruleBase_temp = self._contruct_tempRuleBase(problems, best_individuals)
+
+        self.rule_base = temporalMasterRuleBase(ruleBase_temp)
+
+        self.eval_performance = evr.evalRuleBase(self.rule_base, np.array(X), y, time_moments)
+
+        self.eval_performance.add_full_evaluation()  
+        self.rename_fuzzy_variables()
+        self.rule_base.purge_rules(self.tolerance)
+
+
+    def forward(self, X: np.array, time_moments: list[int] = None) -> np.array:
+        '''
+        Returns the predicted class for each sample.
+
+        :param X: np array samples x features.
+        :param time_moments: list of integers. Time moments associated to each sample (when temporal dependencies are present)
+        :return: np array samples (x 1) with the predicted class.
+        '''
+        try:
+            X = X.values  # If X was a numpy array
+        except AttributeError:
+            pass
+        
+        return self.rule_base.winning_rule_predict(X, time_moments)
+
+
+
+    def plot_fuzzy_variables(self) -> None:
+        '''
+        Plot the fuzzy partitions in each fuzzy variable.
+        '''
+        fuzzy_variables = self.rule_base.rule_bases[0].antecedents
+
+        for ix, fv in enumerate(fuzzy_variables):
+            vis_rules.plot_fuzzy_variable(fv)
+
+
+    def get_rulebase(self) -> list[np.array]:
+        '''
+        Get the rulebase obtained after fitting the classifier to the data.
+
+        :return: a matrix format for the rulebase.
+        '''
+        return self.rule_base.get_rulebase_matrix()
+
+
+def eval_temporal_fuzzy_model(fl_classifier: evf.BaseFuzzyRulesClassifier, X_train: np.array, y_train: np.array,
+                     X_test: np.array, y_test: np.array, time_moments: list[int] = None, test_time_moments: list[int] = None,
+                     plot_rules=True, print_rules=True, plot_partitions=True, return_rules=False, print_accuracy=True, print_matthew=True) -> None:
+    '''
+    Function that evaluates a fuzzy rule based model. It also plots the rules and the fuzzy partitions.
+
+    :param fl_classifier: Fuzzy rule based model.
+    :param X_train: Training data.
+    :param y_train: Training labels.
+    :param X_test: Test data.
+    :param y_test: Test labels.
+    :param plot_rules: If True, it plots the rules.
+    :param print_rules: If True, it prints the rules.
+    :param plot_partitions: If True, it plots the fuzzy partitions.
+    :return: None
+    '''
+
+    if print_accuracy:
+      print('ACCURACY')
+      print('Train performance: ' +
+            str(np.mean(np.equal(y_train, fl_classifier.forward(X_train, time_moments)))))
+      print('Test performance: ' +
+            str(np.mean(np.equal(y_test, fl_classifier.forward(X_test, test_time_moments)))))
+      print('------------')
+    if print_matthew:
+      print('MATTHEW CORRCOEF')
+      print('Train performance: ' +
+            str(matthews_corrcoef(y_train, fl_classifier.forward(X_train, time_moments))))
+      print('Test performance: ' +
+            str(matthews_corrcoef(y_test, fl_classifier.forward(X_test, test_time_moments))))
+      print('------------')
+
+    for ix in np.unique(time_moments):
+      try:
+            X_aux = X_train[time_moments == ix, :]
+            X_aux_test = X_test[time_moments == ix, :]
+      except pd.core.indexing.InvalidIndexError:
+            X_aux = X_train.iloc[time_moments == ix, :]
+            X_aux_test = X_test.iloc[test_time_moments == ix, :]
+
+      y_aux = y_train[time_moments == ix]
+      y_aux_test = y_test[test_time_moments == ix]
+
+      if print_matthew:
+            print('MOMENT ' + str(ix))
+            print('------------')
+            print('MATTHEW CORRCOEF')
+            print('Train performance: ' +
+                  str(matthews_corrcoef(y_aux, fl_classifier.forward(X_aux, np.array([ix] * X_aux.shape[0])))))
+            print('Test performance: ' +
+                  str(matthews_corrcoef(y_aux_test, fl_classifier.forward(X_aux_test, np.array([ix] * X_aux_test.shape[0])))))
+            print('------------')
+
+    if plot_rules:
+        vis_rules.visualize_rulebase(fl_classifier)
+    if print_rules or return_rules:
+        res = fl_classifier.print_rules(return_rules)
+    if plot_partitions:
+        fl_classifier.plot_fuzzy_variables()
+      
+    if return_rules:
+        return res
+    else:
+        print(res)
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,579 +1,595 @@
-# -*- coding: utf-8 -*-
-"""
-Functions that are not fuzzy-specific, but util for some computations. 
-Dedicated mostly to compute quantiles for fuzzy partitions.
-
-"""
-import numpy as np
-import pandas as pd
-
-try:
-    from . import fuzzy_sets as fs
-    from . import maintenance as mnt
-    from . import temporal
-    from . import rules
-    from . import eval_rules as evr
-except ImportError:
-    import fuzzy_sets as fs
-    import maintenance as mnt
-    import temporal
-    import rules
-    import eval_rules as evr
-
-
-from sklearn.model_selection import train_test_split
-
-
-def quartile_compute(x: np.array) -> list[float]:
-    '''
-    Computes the quartiles for each feature.
-
-    :param x: array samples x features
-    :return: list of quartiles for each feature
-    '''
-    return np.quantile(x, [0, 0.25, 0.5, 1], axis=0)
-
-
-def fixed_quantile_compute(x: np.array) -> list[float]:
-    '''
-    Computes a series of quantiles for each feature in numpy array.
-    Quantiles: [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1]
-
-    :param x: array samples x features
-    :return: list of quantiles for each feature
-    '''
-    return np.quantile(x, [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1], axis=0)
-
-
-def partition3_quantile_compute(x: np.array) -> list[float]:
-    '''
-    Computes a series of quantiles partitioning the variable in 3 cases.
-
-    Quantiles: [0.00, 0.20, 0.50, 0.80, 1.00]
-
-    :param x: array samples x features
-    :return: list of quantiles for each feature
-    '''
-    return np.quantile(x, [0, 0.20, 0.50, 0.80, 1.00], axis=0)
-
-
-def t1_simple_partition(x: np.array) -> np.array:
-    '''
-    Partitions the fuzzy variable in four trapezoidal memberships.
-
-    :param x: numpy array, vector of shape (samples, ).
-    :return: numpy array, vector of shape (variables, 4, 4).
-    '''
-    
-
-    n_partitions = 4
-    trap_memberships_size = 4
-    quantile_numbers = fixed_quantile_compute(x)
-
-    partition_parameters = np.zeros(
-        (x.shape[1], n_partitions, trap_memberships_size))
-    for partition in range(n_partitions):
-        if partition == 0:
-            partition_parameters[:, partition, 0] = quantile_numbers[0]
-            partition_parameters[:, partition, 1] = quantile_numbers[0]
-            partition_parameters[:, partition, 2] = quantile_numbers[1]
-            partition_parameters[:, partition, 3] = quantile_numbers[2]
-        elif partition == n_partitions - 1:
-            partition_parameters[:, partition, 0] = quantile_numbers[-3]
-            partition_parameters[:, partition, 1] = quantile_numbers[-2]
-            partition_parameters[:, partition, 2] = quantile_numbers[-1]
-            partition_parameters[:, partition, 3] = quantile_numbers[-1]
-        else:
-            pointer = 1 if partition == 1 else 4
-            partition_parameters[:, partition, 0] = quantile_numbers[pointer]
-            partition_parameters[:, partition,
-                                 1] = quantile_numbers[pointer + 1]
-            partition_parameters[:, partition,
-                                 2] = quantile_numbers[pointer + 2]
-            partition_parameters[:, partition,
-                                 3] = quantile_numbers[pointer + 3]
-
-    return partition_parameters
-
-
-def t1_three_partition(x: np.array) -> np.array:
-    '''
-    Partitions the fuzzy variable in three trapezoidal memberships.
-
-    :param x: numpy array, vector of shape (samples, ).
-    :return: numpy array, vector of shape (variables, 3, 4).
-    '''
-    n_partitions = 3
-    trap_memberships_size = 4
-    quantile_numbers = partition3_quantile_compute(x)
-
-    partition_parameters = np.zeros(
-        (x.shape[1], n_partitions, trap_memberships_size))
-    for partition in range(n_partitions):
-        if partition == 0:
-            partition_parameters[:, partition, 0] = quantile_numbers[0]
-            partition_parameters[:, partition, 1] = quantile_numbers[0]
-            partition_parameters[:, partition, 2] = quantile_numbers[1]
-            partition_parameters[:, partition, 3] = quantile_numbers[2]
-        elif partition == 1:
-            partition_parameters[:, partition, 0] = quantile_numbers[1]
-            partition_parameters[:, partition, 1] = (
-                quantile_numbers[1] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 2] = (
-                quantile_numbers[3] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 3] = quantile_numbers[3]
-        else:
-            partition_parameters[:, partition, 0] = quantile_numbers[2]
-            partition_parameters[:, partition, 1] = quantile_numbers[3]
-            partition_parameters[:, partition, 2] = quantile_numbers[4]
-            partition_parameters[:, partition, 3] = quantile_numbers[4]
-
-    return partition_parameters
-
-
-def t2_simple_partition(x: np.array) -> np.array:
-    '''
-    Partitions the fuzzy variable in three trapezoidal memberships.
-
-    :param x: numpy array, vector of shape (samples, ).
-    :return: numpy array, vector of shape (variables, 3, 4, 2).
-    '''
-    n_partitions = 3
-    trap_memberships_size = 4
-    quantile_numbers = partition3_quantile_compute(x)
-
-    partition_parameters = np.zeros(
-        (x.shape[1], n_partitions, trap_memberships_size, 2))
-    for partition in range(n_partitions):
-        if partition == 0:
-            partition_parameters[:, partition, 0, 1] = quantile_numbers[0]
-            partition_parameters[:, partition, 1, 1] = quantile_numbers[0]
-            partition_parameters[:, partition, 2, 1] = quantile_numbers[1]
-            partition_parameters[:, partition, 3, 1] = quantile_numbers[2]
-
-            partition_parameters[:, partition, 0, 0] = quantile_numbers[0]
-            partition_parameters[:, partition, 1, 0] = quantile_numbers[0]
-            partition_parameters[:, partition, 2, 0] = quantile_numbers[1]
-            partition_parameters[:, partition, 3, 0] = quantile_numbers[1] + \
-                0.9 * (quantile_numbers[2] - quantile_numbers[1])
-
-        elif partition == 1:
-            partition_parameters[:, partition, 0, 1] = quantile_numbers[1]
-            partition_parameters[:, partition, 1, 1] = (
-                quantile_numbers[1] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 2, 1] = (
-                quantile_numbers[2] + quantile_numbers[3]) / 2
-            partition_parameters[:, partition, 3, 1] = quantile_numbers[3]
-
-            partition_parameters[:, partition, 0, 0] = quantile_numbers[1] + \
-                0.1 * (quantile_numbers[2] - quantile_numbers[1])
-            partition_parameters[:, partition, 1, 0] = (
-                quantile_numbers[1] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 2, 0] = (
-                quantile_numbers[3] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 3, 0] = quantile_numbers[2] + \
-                0.9 * (quantile_numbers[3] - quantile_numbers[2])
-
-        else:
-            partition_parameters[:, partition, 0, 1] = quantile_numbers[2]
-            partition_parameters[:, partition, 1, 1] = quantile_numbers[3]
-            partition_parameters[:, partition, 2, 1] = quantile_numbers[4]
-            partition_parameters[:, partition, 3, 1] = quantile_numbers[4]
-
-            partition_parameters[:, partition, 0, 0] = quantile_numbers[2] + \
-                0.1 * (quantile_numbers[3] - quantile_numbers[2])
-            partition_parameters[:, partition, 1, 0] = quantile_numbers[3]
-            partition_parameters[:, partition, 2, 0] = quantile_numbers[4]
-            partition_parameters[:, partition, 3, 0] = quantile_numbers[4]
-
-    return partition_parameters
-
-
-def t1_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
-    '''
-    Partitions the dataset features into different fuzzy variables. Parameters are prefixed.
-    Use it for simple testing and initial solution.
-
-    :param x: numpy array|pandas dataframe, shape samples x features.
-    :return: list of fuzzy variables.
-    '''
-    tripartition_names = ['Low', 'Medium', 'High']
-    try:
-        fv_names = x0.columns
-        x = x0.values
-    except AttributeError:
-        fv_names = [str(ix) for ix in range(x0.shape[1])]
-        x = x0
-
-    mins = np.min(x, axis=0)
-    maxs = np.max(x, axis=0)
-    fz_memberships = t1_three_partition(x)
-    res = []
-    for fz_parameter in range(fz_memberships.shape[0]):
-        fzs = [fs.FS(tripartition_names[ix], fz_memberships[fz_parameter, ix, :], [
-                     mins[fz_parameter], maxs[fz_parameter]]) for ix in range(fz_memberships.shape[1])]
-        res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
-
-    return res
-
-
-def t2_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
-    '''
-    Partitions the dataset features into different fuzzy variables using iv fuzzy sets. Parameters are prefixed.
-    Use it for simple testing and initial solution.
-
-    :param x: numpy array|pandas dataframe, shape samples x features.
-    :return: list of fuzzy variables.
-    '''
-    try:
-        fv_names = x0.columns
-        x = x0.values
-    except AttributeError:
-        fv_names = [str(ix) for ix in range(x0.shape[1])]
-        x = x0
-
-    mins = np.min(x, axis=0)
-    maxs = np.max(x, axis=0)
-    fz_memberships = t2_simple_partition(x)
-    res = []
-    for fz_parameter in range(fz_memberships.shape[0]):
-        fzs = [fs.IVFS(str(ix), fz_memberships[fz_parameter, ix, :, 0], fz_memberships[fz_parameter, ix, :, 1], [
-                       mins[fz_parameter], maxs[fz_parameter]], lower_height=0.8) for ix in range(fz_memberships.shape[1])]
-        res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
-
-    return res
-
-
-def gt2_fuzzy_partitions_dataset(x0: np.array, resolution_exp:int=1) -> list[fs.fuzzyVariable]:
-    '''
-    Partitions the dataset features into different fuzzy variables using gt2 fuzzy sets. Parameters are prefixed.
-    Use it for simple testing and initial solution.
-
-    :param x: numpy array|pandas dataframe, shape samples x features.
-    :param resolution_exp: exponent of the resolution of the partition. Default is -2, which means 0.01. (Number of significant decimals)
-    :return: list of fuzzy variables.
-    '''
-    try:
-        fv_names = x0.columns
-        x = x0.values
-    except AttributeError:
-        fv_names = [str(ix) for ix in range(x0.shape[1])]
-        x = x0
-
-    mins = np.min(x, axis=0)
-    maxs = np.max(x, axis=0)
-    iv_simple_partition = t2_fuzzy_partitions_dataset(x)
-    resolution = 10.0**-np.abs(resolution_exp)
-    res = []
-    # We iterate through all possible variables
-    for ix_var, fz_var in enumerate(iv_simple_partition):
-        domain_resolution = np.arange(
-            mins[ix_var], maxs[ix_var] + resolution, resolution)
-        fzs = []
-        for ix_lv, fz_lv in enumerate(fz_var.get_linguistic_variables()):
-            memberships = fz_lv.membership(domain_resolution)
-            fs_domain = {}
-            for ix_z, x in enumerate(domain_resolution):
-                membership_z = memberships[ix_z]
-                fs_domain[x] = fs.FS(str(x), [membership_z[0], np.mean(
-                   membership_z), np.mean(membership_z), membership_z[1]], [0.0, 1.0])
-
-            fzs.append(fs.GT2(fz_lv.name, fs_domain, [
-                       mins[ix_var], maxs[ix_var]], significant_decimals=np.abs(resolution_exp), unit_resolution=0.01))
-
-        res.append(fs.fuzzyVariable(fv_names[ix_var], fzs))
-
-    return res
-
-
-def construct_partitions(X : np.array, fz_type_studied:fs.FUZZY_SETS, categorical_mask: np.array=None) -> list[fs.fuzzyVariable]:
-    '''
-    Returns a list of linguistic variables according to the kind of fuzzy specified.
-
-    :param X: numpy array|pandas dataframe, shape samples x features.
-    :param fz_type_studied: fuzzy set type studied.
-    :param categorial_mask: a boolean mask vector that indicates for each variables if its categorical or not.
-    '''
-    if mnt.save_usage_flag:
-        mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
-        mnt.usage_data[mnt.usage_categories.FuzzySets][fz_type_studied.name] += 1
-
-    if fz_type_studied == fs.FUZZY_SETS.t1:
-        precomputed_partitions = t1_fuzzy_partitions_dataset(X)
-    elif fz_type_studied == fs.FUZZY_SETS.t2:
-        precomputed_partitions = t2_fuzzy_partitions_dataset(X)
-    elif fz_type_studied == fs.FUZZY_SETS.gt2:
-        precomputed_partitions = gt2_fuzzy_partitions_dataset(X)
-
-    if categorical_mask is not None:
-        for ix, elem in enumerate(categorical_mask):
-            if elem:
-                if isinstance(X, pd.DataFrame):
-                    name = X.columns[ix]
-                else:
-                    name = str(ix)
-                cat_var = construct_crisp_categorical_partition(np.array(X)[:, ix], name, fz_type_studied)
-
-                precomputed_partitions[ix] = cat_var
-
-    return precomputed_partitions
-
-
-def construct_crisp_categorical_partition(x: np.array, name: str, fz_type_studied: fs.FUZZY_SETS):
-    '''
-    Creates a fuzzy variable for a categorical feature. 
-
-    :param x: array with values of the categorical variable.
-    :param name of the fuzzy variable.
-    :return: a fuzzy variable that works as a categorical crips variable (each fuzzy set is 1 exactly on each class value, and 0 on the rest)
-    '''
-    possible_values = np.unique(x)
-    possible_fuzzy_values = np.arange(len(possible_values))
-
-    epsilon = 1e-5
-    fuzzy_sets = []
-
-    # Create a fuzzy sets for each possible value
-    for ix, value in enumerate(possible_values):
-        mem_function = [possible_fuzzy_values[ix] - epsilon, possible_fuzzy_values[ix], possible_fuzzy_values[ix], possible_fuzzy_values[ix] + epsilon]
-
-        if fz_type_studied == fs.FUZZY_SETS.t1:
-            aux = fs.FS(str(value), mem_function, [0, len(possible_fuzzy_values)])
-        elif fz_type_studied == fs.FUZZY_SETS.t2 or fz_type_studied == fs.FUZZY_SETS.gt2:
-            aux = fs.IVFS(str(value), mem_function, mem_function, [0, len(possible_fuzzy_values)])
-
-        fuzzy_sets.append(aux)
-
-    return fs.fuzzyVariable(name, fuzzy_sets)
-    
-
-def construct_conditional_frequencies(X: np.array, discrete_time_labels: list[int], initial_ffss: list[fs.FS]):
-    '''
-    Computes the conditional temporal function for a set of fuzzy sets according to their variation in time.
-
-    :param X: numpy array, shape samples x features.
-    :param discrete_time_labels: discrete time labels.
-    :param initial_fs: initial fuzzy set list.
-    :return: conditional frequencies. Array shape (time steps, initial fuzzy sets)
-    '''
-    obs = X.shape[0]
-    discrete_time_labels = np.array(discrete_time_labels)
-    memberships = np.zeros((obs, len(initial_ffss)))
-    for ix, fset in enumerate(initial_ffss):
-        if fset.type() == fs.FUZZY_SETS.t2:
-            memberships[:, ix] = np.mean(fset.membership(X), axis=1)
-        elif fset.type() == fs.FUZZY_SETS.gt2:
-            memberships[:, ix] = np.mean(np.squeeze(fset._alpha_reduction(fset.membership(X))), axis=1)
-        else:
-            memberships[:, ix] = fset.membership(X)
-    
-    max_memberships = np.argmax(memberships, axis=1)
-    res = np.zeros((len(np.unique(discrete_time_labels)), len(initial_ffss)))
-
-    for time in range(len(np.unique(discrete_time_labels))):
-
-        relevant_memberships = max_memberships[time == discrete_time_labels]
-        fs_winner_counter = np.zeros(len(initial_ffss))
-        for ix, fset in enumerate(initial_ffss):
-            fs_winner_counter[ix] = np.sum(relevant_memberships == ix)
-        
-        res[time, :] = fs_winner_counter
-    
-    return res / (np.max(res, axis=0) + 1e-6)
-
-
-def classify_temp(dates: pd.DataFrame, cutpoints: tuple[str, str], time: str) -> np.array:
-    '''
-    Classifies a set of dates according to the temporal cutpoints. Uses {time} as a the time resolution.
-    Returns an array where true values are those values contained between those two date points.
-
-    :param dates: data observations to cut. 
-    :param cutpoints: points to check.
-    :param time: time field to use as the criteria.
-    :return: boolean array. True values are those contained between the cutpoints.
-    '''
-
-    def extract_hour(row):
-        return row.__getattribute__(time)
-    
-    hours = pd.to_datetime(dates['date']).apply(extract_hour)
-
-    cutpoint_series_0 =  pd.to_datetime(pd.Series([cutpoints[0]] * len(dates)))
-    cutpoint_series_0.index = dates.index
-    hours0 = cutpoint_series_0.apply(extract_hour)
-
-    cutpoint_series_1 =  pd.to_datetime(pd.Series([cutpoints[1]] * len(dates)))
-    cutpoint_series_1.index = dates.index
-    hours1 = cutpoint_series_1.apply(extract_hour)
-
-    condicion1 = hours >= hours0
-    condicion2 = hours <= hours1
-
-    return np.array(np.logical_and(condicion1, condicion2))
-
-
-def assign_time(a: np.array, observations: list[np.array]) -> int:
-    '''
-    Assigns a temporal moment to a set of observations.
-    
-    :param a: array of boolean values.
-    :param observations: list of boolean arrays with the corresponding timestamps.
-    :return: the index of the correspondent time moment for the a-th observation.
-    :raises: ValueError if a is not timestamped in any of the observation arrays.'''
-    for ix, obs in enumerate(observations):
-        if obs[a]:
-            return ix
-    
-    raise ValueError('No temporal moment assigned')
-        
-
-def create_tempVariables(X_train: np.array, time_moments: np.array, precomputed_partitions: list[fs.fuzzyVariable]) -> list[temporal.temporalFS]:
-    '''
-    Creates a list of temporal fuzzy variables.
-
-    :param X_train: numpy array, shape samples x features.
-    :param time_moments: time moments. Array shape (samples,). Each value is an integer denoting the n-th time moment of that observation.
-    :param precomputed_partitions: precomputed partitions for each feature.
-    :return: list of temporal fuzzy variables.
-    '''
-    temp_partitions = []
-    for ix in range(X_train.shape[1]):
-        feat_conditional = construct_conditional_frequencies(X_train[:, ix], time_moments, initial_ffss=precomputed_partitions[ix])
-        temp_fs_list = []
-        for vl in range(feat_conditional.shape[1]):
-            vl_temp_fs = temporal.temporalFS(precomputed_partitions[ix][vl], feat_conditional[:, vl])
-            temp_fs_list.append(vl_temp_fs)
-
-        temp_fs_variable = temporal.temporalFuzzyVariable(precomputed_partitions[ix].name, temp_fs_list)
-        temp_partitions.append(temp_fs_variable)
-
-    return temp_partitions
-
-
-def create_multi_tempVariables(X_train: np.array, time_moments: np.array, fuzzy_type: fs.FUZZY_SETS) -> list[list[temporal.temporalFS]]:
-    '''
-    Creates a of list of lists of temporal fuzzy variables. Each corresponds to a fuzzy partition in a different moment in time.
-    (So, instead of having one vl for all time moments, you have one different for each time moment that represents the same idea)
-
-    :param X_train: numpy array, shape samples x features.
-    :param time_moments: time moments. Array shape (samples,). Each value is an integer denoting the n-th time moment of that observation.
-    :param precomputed_partitions: precomputed partitions for each feature.
-    :return: list of lists of temporal fuzzy variables.
-    '''
-    temp_partitions = []
-
-    unique_time_moments = np.unique(time_moments)
-    for time in unique_time_moments:
-        X_obs = X_train[time_moments == time, :]
-        precomputed_partitions = construct_partitions(X_obs, fuzzy_type)
-
-        temp_partitions.append(create_tempVariables(X_obs, time_moments[time_moments == time], precomputed_partitions))
-    
-    return temp_partitions
-
-
-def temporal_cuts(X: pd.DataFrame, cutpoints: list[tuple[str, str]], time_resolution: str='hour') -> list[np.array]:
-    '''
-    Returns a list of boolean indexes for each temporal moment. Performs the cuts between time steps using the cutpoints list.
-
-    :param X: data observations to cut in temrporal moments.
-    :param temporal_moments: list of temporal moments to cut.
-    :param cutpoints: list of tuples with the cutpoints for each temporal moment.
-    :param time_resolution: time field to use as the criteria.
-    :return: list of boolean arrays. True values are those contained between the cutpoints in each moment.
-    '''
-
-    res = []
-    for ix, cutpoint in enumerate(cutpoints):
-        observations = classify_temp(X, cutpoint, time=time_resolution)
-        res.append(observations)
-    
-    return res
-
-
-def temporal_assemble(X: np.array, y:np.array, temporal_moments: list[np.array]):
-    '''
-    Assembles the data in the temporal moments in order to have partitions with balanced time moments in each one.
-    
-    :param X: data observations.
-    :param y: labels.
-    :param temporal_moments: list of boolean arrays. True values are those contained between the cutpoints in each moment.
-    :return: tuple of lists of data and labels for each temporal moment.
-        First tuple is: X_train, X_test, y_train, y_test
-        Second tuple is: train temporal moments, test temporal moments.
-    '''
-    moments_partitions = []
-    train_temporal_boolean_markers = []
-    test_temporal_boolean_markers = []
-    train_counter = 0
-    test_counter = 0
-
-    for ix, temporal_moment in enumerate(temporal_moments):
-        X_train, X_test, y_train, y_test = train_test_split(X[temporal_moment], y[temporal_moment], test_size=0.33, random_state=0)
-        moments_partitions.append((X_train, X_test, y_train, y_test))
-    
-    if isinstance(X_train,(pd.core.series.Series,pd.DataFrame)):
-        X_train = pd.concat([moments_partitions[ix][0] for ix in range(len(moments_partitions))])
-        X_test =  pd.concat([moments_partitions[ix][1] for ix in range(len(moments_partitions))])
-        y_train = np.concatenate([moments_partitions[ix][2] for ix in range(len(moments_partitions))])
-        y_test = np.concatenate([moments_partitions[ix][3] for ix in range(len(moments_partitions))])
-    else:
-        X_train = np.concatenate([moments_partitions[ix][0] for ix in range(len(moments_partitions))])
-        X_test =  np.concatenate([moments_partitions[ix][1] for ix in range(len(moments_partitions))])
-        y_train = np.concatenate([moments_partitions[ix][2] for ix in range(len(moments_partitions))])
-        y_test = np.concatenate([moments_partitions[ix][3] for ix in range(len(moments_partitions))])
-
-    for ix, temporal_moment in enumerate(temporal_moments):
-        # Believe, this makes sense to avoid rounding errrors in the size of the final vector
-        _, _, y_train0, y_test0 = train_test_split(X[temporal_moment], y[temporal_moment], test_size=0.33, random_state=0)
-
-        train_moment_observations = np.zeros((X_train.shape[0]))
-        train_moment_observations[train_counter:train_counter+len(y_train0)] = 1
-        train_counter += len(y_train0)
-        train_temporal_boolean_markers.append(train_moment_observations)
-
-        test_moment_observations = np.zeros((X_test.shape[0]))
-        test_moment_observations[test_counter:test_counter+len(y_test0)] = 1
-        test_counter += len(y_test0)
-        test_temporal_boolean_markers.append(test_moment_observations)
-
-    
-    return [X_train, X_test, y_train, y_test], [train_temporal_boolean_markers, test_temporal_boolean_markers]
-
-
-def extend_fuzzy_sets_enum(new_fuzzy_sets_enum: fs.FUZZY_SETS) -> list[fs.FUZZY_SETS]:
-    '''
-    Extends the fuzzy sets enum with additional types.
-
-    :param fuzzy_sets_enum: fuzzy sets enum.
-    :return: extended fuzzy sets enum.
-    '''
-    import enum
-    NEW_FUZZY_SETS = enum.Enum(
-        "FUZZY_SETS",
-        [(es.name, es.value) for es in fs.FUZZY_SETS] + [(es.name, es.value) for es in new_fuzzy_sets_enum]
-        )
-    fs.FUZZY_SETS = NEW_FUZZY_SETS
-
-
-def mcc_loss(ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.99, beta:float=0.0125, gamma:float=0.0125) -> float:
-
-        '''
-        Fitness function for the optimization problem. Uses only the MCC, ignores the size penalization terms.
-
-
-        :param ruleBase: RuleBase object
-        :param X: array of train samples. X shape = (n_samples, n_features)
-        :param y: array of train labels. y shape = (n_samples,)
-        :param tolerance: float. Tolerance for the size evaluation.
-        :param alpha: ignored.
-        :param beta: ignored.
-        :param gamma: ignored.
-        :return: float. Fitness value.
-        '''
-        ev_object = evr.evalRuleBase(ruleBase, X, y)
-        ev_object.add_rule_weights()
-
-        score_acc = ev_object.classification_eval()
-        
+# -*- coding: utf-8 -*-
+"""
+Functions that are not fuzzy-specific, but util for some computations. 
+Dedicated mostly to compute quantiles for fuzzy partitions.
+
+"""
+import numpy as np
+import pandas as pd
+
+try:
+    from . import fuzzy_sets as fs
+    from . import maintenance as mnt
+    from . import temporal
+    from . import rules
+    from . import eval_rules as evr
+except ImportError:
+    import fuzzy_sets as fs
+    import maintenance as mnt
+    import temporal
+    import rules
+    import eval_rules as evr
+
+
+from sklearn.model_selection import train_test_split
+
+
+def quartile_compute(x: np.array) -> list[float]:
+    '''
+    Computes the quartiles for each feature.
+
+    :param x: array samples x features
+    :return: list of quartiles for each feature
+    '''
+    return np.quantile(x, [0, 0.25, 0.5, 1], axis=0)
+
+
+def fixed_quantile_compute(x: np.array) -> list[float]:
+    '''
+    Computes a series of quantiles for each feature in numpy array.
+    Quantiles: [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1]
+
+    :param x: array samples x features
+    :return: list of quantiles for each feature
+    '''
+    return np.quantile(x, [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1], axis=0)
+
+
+def partition3_quantile_compute(x: np.array) -> list[float]:
+    '''
+    Computes a series of quantiles partitioning the variable in 3 cases.
+
+    Quantiles: [0.00, 0.20, 0.50, 0.80, 1.00]
+
+    :param x: array samples x features
+    :return: list of quantiles for each feature
+    '''
+    return np.quantile(x, [0, 0.20, 0.50, 0.80, 1.00], axis=0)
+
+
+def t1_simple_partition(x: np.array) -> np.array:
+    '''
+    Partitions the fuzzy variable in four trapezoidal memberships.
+
+    :param x: numpy array, vector of shape (samples, ).
+    :return: numpy array, vector of shape (variables, 4, 4).
+    '''
+    
+
+    n_partitions = 4
+    trap_memberships_size = 4
+    quantile_numbers = fixed_quantile_compute(x)
+
+    partition_parameters = np.zeros(
+        (x.shape[1], n_partitions, trap_memberships_size))
+    for partition in range(n_partitions):
+        if partition == 0:
+            partition_parameters[:, partition, 0] = quantile_numbers[0]
+            partition_parameters[:, partition, 1] = quantile_numbers[0]
+            partition_parameters[:, partition, 2] = quantile_numbers[1]
+            partition_parameters[:, partition, 3] = quantile_numbers[2]
+        elif partition == n_partitions - 1:
+            partition_parameters[:, partition, 0] = quantile_numbers[-3]
+            partition_parameters[:, partition, 1] = quantile_numbers[-2]
+            partition_parameters[:, partition, 2] = quantile_numbers[-1]
+            partition_parameters[:, partition, 3] = quantile_numbers[-1]
+        else:
+            pointer = 1 if partition == 1 else 4
+            partition_parameters[:, partition, 0] = quantile_numbers[pointer]
+            partition_parameters[:, partition,
+                                 1] = quantile_numbers[pointer + 1]
+            partition_parameters[:, partition,
+                                 2] = quantile_numbers[pointer + 2]
+            partition_parameters[:, partition,
+                                 3] = quantile_numbers[pointer + 3]
+
+    return partition_parameters
+
+
+def t1_three_partition(x: np.array) -> np.array:
+    '''
+    Partitions the fuzzy variable in three trapezoidal memberships.
+
+    :param x: numpy array, vector of shape (samples, ).
+    :return: numpy array, vector of shape (variables, 3, 4).
+    '''
+    n_partitions = 3
+    trap_memberships_size = 4
+    quantile_numbers = partition3_quantile_compute(x)
+
+    partition_parameters = np.zeros(
+        (x.shape[1], n_partitions, trap_memberships_size))
+    for partition in range(n_partitions):
+        if partition == 0:
+            partition_parameters[:, partition, 0] = quantile_numbers[0]
+            partition_parameters[:, partition, 1] = quantile_numbers[0]
+            partition_parameters[:, partition, 2] = quantile_numbers[1]
+            partition_parameters[:, partition, 3] = quantile_numbers[2]
+        elif partition == 1:
+            partition_parameters[:, partition, 0] = quantile_numbers[1]
+            partition_parameters[:, partition, 1] = (
+                quantile_numbers[1] + quantile_numbers[2]) / 2
+            partition_parameters[:, partition, 2] = (
+                quantile_numbers[3] + quantile_numbers[2]) / 2
+            partition_parameters[:, partition, 3] = quantile_numbers[3]
+        else:
+            partition_parameters[:, partition, 0] = quantile_numbers[2]
+            partition_parameters[:, partition, 1] = quantile_numbers[3]
+            partition_parameters[:, partition, 2] = quantile_numbers[4]
+            partition_parameters[:, partition, 3] = quantile_numbers[4]
+
+    return partition_parameters
+
+
+def t2_simple_partition(x: np.array) -> np.array:
+    '''
+    Partitions the fuzzy variable in three trapezoidal memberships.
+
+    :param x: numpy array, vector of shape (samples, ).
+    :return: numpy array, vector of shape (variables, 3, 4, 2).
+    '''
+    n_partitions = 3
+    trap_memberships_size = 4
+    quantile_numbers = partition3_quantile_compute(x)
+
+    partition_parameters = np.zeros(
+        (x.shape[1], n_partitions, trap_memberships_size, 2))
+    for partition in range(n_partitions):
+        if partition == 0:
+            partition_parameters[:, partition, 0, 1] = quantile_numbers[0]
+            partition_parameters[:, partition, 1, 1] = quantile_numbers[0]
+            partition_parameters[:, partition, 2, 1] = quantile_numbers[1]
+            partition_parameters[:, partition, 3, 1] = quantile_numbers[2]
+
+            partition_parameters[:, partition, 0, 0] = quantile_numbers[0]
+            partition_parameters[:, partition, 1, 0] = quantile_numbers[0]
+            partition_parameters[:, partition, 2, 0] = quantile_numbers[1]
+            partition_parameters[:, partition, 3, 0] = quantile_numbers[1] + \
+                0.9 * (quantile_numbers[2] - quantile_numbers[1])
+
+        elif partition == 1:
+            partition_parameters[:, partition, 0, 1] = quantile_numbers[1]
+            partition_parameters[:, partition, 1, 1] = (
+                quantile_numbers[1] + quantile_numbers[2]) / 2
+            partition_parameters[:, partition, 2, 1] = (
+                quantile_numbers[2] + quantile_numbers[3]) / 2
+            partition_parameters[:, partition, 3, 1] = quantile_numbers[3]
+
+            partition_parameters[:, partition, 0, 0] = quantile_numbers[1] + \
+                0.1 * (quantile_numbers[2] - quantile_numbers[1])
+            partition_parameters[:, partition, 1, 0] = (
+                quantile_numbers[1] + quantile_numbers[2]) / 2
+            partition_parameters[:, partition, 2, 0] = (
+                quantile_numbers[3] + quantile_numbers[2]) / 2
+            partition_parameters[:, partition, 3, 0] = quantile_numbers[2] + \
+                0.9 * (quantile_numbers[3] - quantile_numbers[2])
+
+        else:
+            partition_parameters[:, partition, 0, 1] = quantile_numbers[2]
+            partition_parameters[:, partition, 1, 1] = quantile_numbers[3]
+            partition_parameters[:, partition, 2, 1] = quantile_numbers[4]
+            partition_parameters[:, partition, 3, 1] = quantile_numbers[4]
+
+            partition_parameters[:, partition, 0, 0] = quantile_numbers[2] + \
+                0.1 * (quantile_numbers[3] - quantile_numbers[2])
+            partition_parameters[:, partition, 1, 0] = quantile_numbers[3]
+            partition_parameters[:, partition, 2, 0] = quantile_numbers[4]
+            partition_parameters[:, partition, 3, 0] = quantile_numbers[4]
+
+    return partition_parameters
+
+
+def t1_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
+    '''
+    Partitions the dataset features into different fuzzy variables. Parameters are prefixed.
+    Use it for simple testing and initial solution.
+
+    :param x: numpy array|pandas dataframe, shape samples x features.
+    :return: list of fuzzy variables.
+    '''
+    tripartition_names = ['Low', 'Medium', 'High']
+    try:
+        fv_names = x0.columns
+        x = x0.values
+    except AttributeError:
+        fv_names = [str(ix) for ix in range(x0.shape[1])]
+        x = x0
+
+    mins = np.min(x, axis=0)
+    maxs = np.max(x, axis=0)
+    fz_memberships = t1_three_partition(x)
+    res = []
+    for fz_parameter in range(fz_memberships.shape[0]):
+        fzs = [fs.FS(tripartition_names[ix], fz_memberships[fz_parameter, ix, :], [
+                     mins[fz_parameter], maxs[fz_parameter]]) for ix in range(fz_memberships.shape[1])]
+        res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
+
+    return res
+
+
+def t2_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
+    '''
+    Partitions the dataset features into different fuzzy variables using iv fuzzy sets. Parameters are prefixed.
+    Use it for simple testing and initial solution.
+
+    :param x: numpy array|pandas dataframe, shape samples x features.
+    :return: list of fuzzy variables.
+    '''
+    tripartition_names = ['Low', 'Medium', 'High']
+    try:
+        fv_names = x0.columns
+        x = x0.values
+    except AttributeError:
+        fv_names = [str(ix) for ix in range(x0.shape[1])]
+        x = x0
+
+    mins = np.min(x, axis=0)
+    maxs = np.max(x, axis=0)
+    fz_memberships = t2_simple_partition(x)
+    res = []
+    for fz_parameter in range(fz_memberships.shape[0]):
+        fzs = [fs.IVFS(tripartition_names[ix], fz_memberships[fz_parameter, ix, :, 0], fz_memberships[fz_parameter, ix, :, 1], [
+                       mins[fz_parameter], maxs[fz_parameter]], lower_height=0.8) for ix in range(fz_memberships.shape[1])]
+        res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
+
+    return res
+
+
+def gt2_fuzzy_partitions_dataset(x0: np.array, resolution_exp:int=1) -> list[fs.fuzzyVariable]:
+    '''
+    Partitions the dataset features into different fuzzy variables using gt2 fuzzy sets. Parameters are prefixed.
+    Use it for simple testing and initial solution.
+
+    :param x: numpy array|pandas dataframe, shape samples x features.
+    :param resolution_exp: exponent of the resolution of the partition. Default is -2, which means 0.01. (Number of significant decimals)
+    :return: list of fuzzy variables.
+    '''
+    try:
+        fv_names = x0.columns
+        x = x0.values
+    except AttributeError:
+        fv_names = [str(ix) for ix in range(x0.shape[1])]
+        x = x0
+
+    mins = np.min(x, axis=0)
+    maxs = np.max(x, axis=0)
+    iv_simple_partition = t2_fuzzy_partitions_dataset(x)
+    resolution = 10.0**-np.abs(resolution_exp)
+    res = []
+    # We iterate through all possible variables
+    for ix_var, fz_var in enumerate(iv_simple_partition):
+        domain_resolution = np.arange(
+            mins[ix_var], maxs[ix_var] + resolution, resolution)
+        fzs = []
+        for ix_lv, fz_lv in enumerate(fz_var.get_linguistic_variables()):
+            memberships = fz_lv.membership(domain_resolution)
+            fs_domain = {}
+            for ix_z, x in enumerate(domain_resolution):
+                membership_z = memberships[ix_z]
+                fs_domain[x] = fs.FS(str(x), [membership_z[0], np.mean(
+                   membership_z), np.mean(membership_z), membership_z[1]], [0.0, 1.0])
+
+            fzs.append(fs.GT2(fz_lv.name, fs_domain, [
+                       mins[ix_var], maxs[ix_var]], significant_decimals=np.abs(resolution_exp), unit_resolution=0.01))
+
+        res.append(fs.fuzzyVariable(fv_names[ix_var], fzs))
+
+    return res
+
+
+def construct_partitions(X : np.array, fz_type_studied:fs.FUZZY_SETS, categorical_mask: np.array=None) -> list[fs.fuzzyVariable]:
+    '''
+    Returns a list of linguistic variables according to the kind of fuzzy specified.
+
+    :param X: numpy array|pandas dataframe, shape samples x features.
+    :param fz_type_studied: fuzzy set type studied.
+    :param categorial_mask: a boolean mask vector that indicates for each variables if its categorical or not.
+    '''
+    if mnt.save_usage_flag:
+        mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
+        mnt.usage_data[mnt.usage_categories.FuzzySets][fz_type_studied.name] += 1
+
+    # Get the X dataframe without the categorical variables
+    if categorical_mask is not None:
+        X_numerical = X.loc[:, np.array(~categorical_mask)]
+    else:
+        X_numerical = X
+
+    if fz_type_studied == fs.FUZZY_SETS.t1:
+        precomputed_partitions = t1_fuzzy_partitions_dataset(X_numerical)
+    elif fz_type_studied == fs.FUZZY_SETS.t2:
+        precomputed_partitions = t2_fuzzy_partitions_dataset(X_numerical)
+    elif fz_type_studied == fs.FUZZY_SETS.gt2:
+        precomputed_partitions = gt2_fuzzy_partitions_dataset(X_numerical)
+
+
+    if categorical_mask is not None:
+        categorical_partition = {}
+        for ix, elem in enumerate(categorical_mask):
+            if elem:
+                if isinstance(X, pd.DataFrame):
+                    name = X.columns[ix]
+                else:
+                    name = str(ix)
+                cat_var = construct_crisp_categorical_partition(np.array(X)[:, ix], name, fz_type_studied)
+
+                categorical_partition[X.columns[ix]] = cat_var
+
+        # Reorder the partitions so that they follow the same order as in the original X
+        precomputed_partitions_aux = []
+        for ix, elem in enumerate(categorical_mask):
+            if elem:
+                precomputed_partitions_aux.append(categorical_partition[X.columns[ix]])
+            else:
+                precomputed_partitions_aux.append(precomputed_partitions.pop(0))
+
+        precomputed_partitions = precomputed_partitions_aux
+
+    return precomputed_partitions
+
+
+def construct_crisp_categorical_partition(x: np.array, name: str, fz_type_studied: fs.FUZZY_SETS) -> fs.fuzzyVariable:
+    '''
+    Creates a fuzzy variable for a categorical feature. 
+
+    :param x: array with values of the categorical variable.
+    :param name of the fuzzy variable.
+    :param fz_type_studied: fuzzy set type studied.
+    :return: a fuzzy variable that works as a categorical crips variable (each fuzzy set is 1 exactly on each class value, and 0 on the rest)
+    '''
+    possible_values = np.unique(x)
+    fuzzy_sets = []
+
+    # Create a fuzzy sets for each possible value
+    for ix, value in enumerate(possible_values):
+
+        if fz_type_studied == fs.FUZZY_SETS.t1:
+            aux = fs.categoricalFS(str(value), value)
+        elif fz_type_studied == fs.FUZZY_SETS.t2 or fz_type_studied == fs.FUZZY_SETS.gt2:
+            aux = fs.categoricalIVFS(str(value), np.unique(x))
+
+        fuzzy_sets.append(aux)
+
+    return fs.fuzzyVariable(name, fuzzy_sets)
+    
+
+def construct_conditional_frequencies(X: np.array, discrete_time_labels: list[int], initial_ffss: list[fs.FS]):
+    '''
+    Computes the conditional temporal function for a set of fuzzy sets according to their variation in time.
+
+    :param X: numpy array, shape samples x features.
+    :param discrete_time_labels: discrete time labels.
+    :param initial_fs: initial fuzzy set list.
+    :return: conditional frequencies. Array shape (time steps, initial fuzzy sets)
+    '''
+    obs = X.shape[0]
+    discrete_time_labels = np.array(discrete_time_labels)
+    memberships = np.zeros((obs, len(initial_ffss)))
+    for ix, fset in enumerate(initial_ffss):
+        if fset.type() == fs.FUZZY_SETS.t2:
+            memberships[:, ix] = np.mean(fset.membership(X), axis=1)
+        elif fset.type() == fs.FUZZY_SETS.gt2:
+            memberships[:, ix] = np.mean(np.squeeze(fset._alpha_reduction(fset.membership(X))), axis=1)
+        else:
+            memberships[:, ix] = fset.membership(X)
+    
+    max_memberships = np.argmax(memberships, axis=1)
+    res = np.zeros((len(np.unique(discrete_time_labels)), len(initial_ffss)))
+
+    for time in range(len(np.unique(discrete_time_labels))):
+
+        relevant_memberships = max_memberships[time == discrete_time_labels]
+        fs_winner_counter = np.zeros(len(initial_ffss))
+        for ix, fset in enumerate(initial_ffss):
+            fs_winner_counter[ix] = np.sum(relevant_memberships == ix)
+        
+        res[time, :] = fs_winner_counter
+    
+    return res / (np.max(res, axis=0) + 1e-6)
+
+
+def classify_temp(dates: pd.DataFrame, cutpoints: tuple[str, str], time: str) -> np.array:
+    '''
+    Classifies a set of dates according to the temporal cutpoints. Uses {time} as a the time resolution.
+    Returns an array where true values are those values contained between those two date points.
+
+    :param dates: data observations to cut. 
+    :param cutpoints: points to check.
+    :param time: time field to use as the criteria.
+    :return: boolean array. True values are those contained between the cutpoints.
+    '''
+
+    def extract_hour(row):
+        return row.__getattribute__(time)
+    
+    hours = pd.to_datetime(dates['date']).apply(extract_hour)
+
+    cutpoint_series_0 =  pd.to_datetime(pd.Series([cutpoints[0]] * len(dates)))
+    cutpoint_series_0.index = dates.index
+    hours0 = cutpoint_series_0.apply(extract_hour)
+
+    cutpoint_series_1 =  pd.to_datetime(pd.Series([cutpoints[1]] * len(dates)))
+    cutpoint_series_1.index = dates.index
+    hours1 = cutpoint_series_1.apply(extract_hour)
+
+    condicion1 = hours >= hours0
+    condicion2 = hours <= hours1
+
+    return np.array(np.logical_and(condicion1, condicion2))
+
+
+def assign_time(a: np.array, observations: list[np.array]) -> int:
+    '''
+    Assigns a temporal moment to a set of observations.
+    
+    :param a: array of boolean values.
+    :param observations: list of boolean arrays with the corresponding timestamps.
+    :return: the index of the correspondent time moment for the a-th observation.
+    :raises: ValueError if a is not timestamped in any of the observation arrays.'''
+    for ix, obs in enumerate(observations):
+        if obs[a]:
+            return ix
+    
+    raise ValueError('No temporal moment assigned')
+        
+
+def create_tempVariables(X_train: np.array, time_moments: np.array, precomputed_partitions: list[fs.fuzzyVariable]) -> list[temporal.temporalFS]:
+    '''
+    Creates a list of temporal fuzzy variables.
+
+    :param X_train: numpy array, shape samples x features.
+    :param time_moments: time moments. Array shape (samples,). Each value is an integer denoting the n-th time moment of that observation.
+    :param precomputed_partitions: precomputed partitions for each feature.
+    :return: list of temporal fuzzy variables.
+    '''
+    temp_partitions = []
+    for ix in range(X_train.shape[1]):
+        feat_conditional = construct_conditional_frequencies(X_train[:, ix], time_moments, initial_ffss=precomputed_partitions[ix])
+        temp_fs_list = []
+        for vl in range(feat_conditional.shape[1]):
+            vl_temp_fs = temporal.temporalFS(precomputed_partitions[ix][vl], feat_conditional[:, vl])
+            temp_fs_list.append(vl_temp_fs)
+
+        temp_fs_variable = temporal.temporalFuzzyVariable(precomputed_partitions[ix].name, temp_fs_list)
+        temp_partitions.append(temp_fs_variable)
+
+    return temp_partitions
+
+
+def create_multi_tempVariables(X_train: np.array, time_moments: np.array, fuzzy_type: fs.FUZZY_SETS) -> list[list[temporal.temporalFS]]:
+    '''
+    Creates a of list of lists of temporal fuzzy variables. Each corresponds to a fuzzy partition in a different moment in time.
+    (So, instead of having one vl for all time moments, you have one different for each time moment that represents the same idea)
+
+    :param X_train: numpy array, shape samples x features.
+    :param time_moments: time moments. Array shape (samples,). Each value is an integer denoting the n-th time moment of that observation.
+    :param precomputed_partitions: precomputed partitions for each feature.
+    :return: list of lists of temporal fuzzy variables.
+    '''
+    temp_partitions = []
+
+    unique_time_moments = np.unique(time_moments)
+    for time in unique_time_moments:
+        X_obs = X_train[time_moments == time, :]
+        precomputed_partitions = construct_partitions(X_obs, fuzzy_type)
+
+        temp_partitions.append(create_tempVariables(X_obs, time_moments[time_moments == time], precomputed_partitions))
+    
+    return temp_partitions
+
+
+def temporal_cuts(X: pd.DataFrame, cutpoints: list[tuple[str, str]], time_resolution: str='hour') -> list[np.array]:
+    '''
+    Returns a list of boolean indexes for each temporal moment. Performs the cuts between time steps using the cutpoints list.
+
+    :param X: data observations to cut in temrporal moments.
+    :param temporal_moments: list of temporal moments to cut.
+    :param cutpoints: list of tuples with the cutpoints for each temporal moment.
+    :param time_resolution: time field to use as the criteria.
+    :return: list of boolean arrays. True values are those contained between the cutpoints in each moment.
+    '''
+
+    res = []
+    for ix, cutpoint in enumerate(cutpoints):
+        observations = classify_temp(X, cutpoint, time=time_resolution)
+        res.append(observations)
+    
+    return res
+
+
+def temporal_assemble(X: np.array, y:np.array, temporal_moments: list[np.array]):
+    '''
+    Assembles the data in the temporal moments in order to have partitions with balanced time moments in each one.
+    
+    :param X: data observations.
+    :param y: labels.
+    :param temporal_moments: list of boolean arrays. True values are those contained between the cutpoints in each moment.
+    :return: tuple of lists of data and labels for each temporal moment.
+        First tuple is: X_train, X_test, y_train, y_test
+        Second tuple is: train temporal moments, test temporal moments.
+    '''
+    moments_partitions = []
+    train_temporal_boolean_markers = []
+    test_temporal_boolean_markers = []
+    train_counter = 0
+    test_counter = 0
+
+    for ix, temporal_moment in enumerate(temporal_moments):
+        X_train, X_test, y_train, y_test = train_test_split(X[temporal_moment], y[temporal_moment], test_size=0.33, random_state=0)
+        moments_partitions.append((X_train, X_test, y_train, y_test))
+    
+    if isinstance(X_train,(pd.core.series.Series,pd.DataFrame)):
+        X_train = pd.concat([moments_partitions[ix][0] for ix in range(len(moments_partitions))])
+        X_test =  pd.concat([moments_partitions[ix][1] for ix in range(len(moments_partitions))])
+        y_train = np.concatenate([moments_partitions[ix][2] for ix in range(len(moments_partitions))])
+        y_test = np.concatenate([moments_partitions[ix][3] for ix in range(len(moments_partitions))])
+    else:
+        X_train = np.concatenate([moments_partitions[ix][0] for ix in range(len(moments_partitions))])
+        X_test =  np.concatenate([moments_partitions[ix][1] for ix in range(len(moments_partitions))])
+        y_train = np.concatenate([moments_partitions[ix][2] for ix in range(len(moments_partitions))])
+        y_test = np.concatenate([moments_partitions[ix][3] for ix in range(len(moments_partitions))])
+
+    for ix, temporal_moment in enumerate(temporal_moments):
+        # Believe, this makes sense to avoid rounding errrors in the size of the final vector
+        _, _, y_train0, y_test0 = train_test_split(X[temporal_moment], y[temporal_moment], test_size=0.33, random_state=0)
+
+        train_moment_observations = np.zeros((X_train.shape[0]))
+        train_moment_observations[train_counter:train_counter+len(y_train0)] = 1
+        train_counter += len(y_train0)
+        train_temporal_boolean_markers.append(train_moment_observations)
+
+        test_moment_observations = np.zeros((X_test.shape[0]))
+        test_moment_observations[test_counter:test_counter+len(y_test0)] = 1
+        test_counter += len(y_test0)
+        test_temporal_boolean_markers.append(test_moment_observations)
+
+    
+    return [X_train, X_test, y_train, y_test], [train_temporal_boolean_markers, test_temporal_boolean_markers]
+
+
+def extend_fuzzy_sets_enum(new_fuzzy_sets_enum: fs.FUZZY_SETS) -> list[fs.FUZZY_SETS]:
+    '''
+    Extends the fuzzy sets enum with additional types.
+
+    :param fuzzy_sets_enum: fuzzy sets enum.
+    :return: extended fuzzy sets enum.
+    '''
+    import enum
+    NEW_FUZZY_SETS = enum.Enum(
+        "FUZZY_SETS",
+        [(es.name, es.value) for es in fs.FUZZY_SETS] + [(es.name, es.value) for es in new_fuzzy_sets_enum]
+        )
+    fs.FUZZY_SETS = NEW_FUZZY_SETS
+
+
+def mcc_loss(ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.99, beta:float=0.0125, gamma:float=0.0125) -> float:
+
+        '''
+        Fitness function for the optimization problem. Uses only the MCC, ignores the size penalization terms.
+
+
+        :param ruleBase: RuleBase object
+        :param X: array of train samples. X shape = (n_samples, n_features)
+        :param y: array of train labels. y shape = (n_samples,)
+        :param tolerance: float. Tolerance for the size evaluation.
+        :param alpha: ignored.
+        :param beta: ignored.
+        :param gamma: ignored.
+        :return: float. Fitness value.
+        '''
+        ev_object = evr.evalRuleBase(ruleBase, X, y)
+        ev_object.add_rule_weights()
+
+        score_acc = ev_object.classification_eval()
+        
         return score_acc
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.0/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,405 +1,408 @@
-# -*- coding: utf-8 -*-
-"""
-This is a the source file that contains the functions necessary to visualize the set of rules.
-"""
-import os
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import networkx as nx
-
-try:
-    from . import rules
-    from . import evolutionary_fit as evf
-    from . import fuzzy_sets as fs
-    from . import maintenance as mnt
-except ImportError:
-    import rules
-    import evolutionary_fit as evf
-    import fuzzy_sets as fs
-    import maintenance as mnt
-
-
-def _column_histogram(rule_matrix: np.array) -> dict:
-    '''
-    Computes the histogram for all the unique values in a column.
-
-    :param rule_matrix: vector with the numerical values.
-    :return: dictionary with the histogram.
-    '''
-    res = {}
-    for x in np.unique(rule_matrix):
-        if x != -1:
-            res[x] = np.sum(rule_matrix == x)
-
-    return res
-
-
-def _histogram(rule_matrix: np.array) -> list[dict]:
-    '''
-    Returns a list with the histogram for each antecedent according to linguist variables.
-
-    :param rule_matrix: matrix with the rules.
-    :return: list with the histogram in dictionary format for each antecedent.
-    '''
-    res = []
-
-    for column_ix in range(rule_matrix.shape[1]):
-        res.append(_column_histogram(rule_matrix[:, column_ix]))
-
-    return res
-
-
-def _max_values(appearances: list) -> tuple[int, int]:
-    '''
-    Returns the antecedent and its linguistic value most repeated.
-
-    :param appearances: list with the histogram for each antecedent.
-    :return: tuple with the antecedent and its linguistic value most repeated.
-    '''
-    res = 0
-    antecedent = None
-    vl = None
-
-    for ix, apperances_an in enumerate(appearances):
-        for key, value in apperances_an.items():
-            if value > res:
-                res = value
-                antecedent = ix
-                vl = key
-
-    return antecedent, vl
-
-
-def create_graph_connection(rules, possible_vl):
-    '''
-    Returns a square matrix where each number indicates if two nodes are connected.
-    Connectes by checking if both are in the same rule.
-
-    :param rules: list with the rules.
-    :param possible_vl: number of linguistic variables.
-    :return: square matrix where each number indicates if two nodes are connected.
-    '''
-    def generate_index(ant, vl0): return int(possible_vl * ant + vl0)
-    res = np.zeros(
-        (possible_vl * rules.shape[1], possible_vl * rules.shape[1]))
-
-    for rule in rules:
-        for antecedent, vl in enumerate(rule):
-            if vl > -1:
-                for antecedent2, vl2 in enumerate(rule):
-                    if vl2 > -1:
-                        res_index1 = generate_index(antecedent, vl)
-                        res_index2 = generate_index(antecedent2, vl2)
-
-                        res[res_index1, res_index2] += 1
-
-    return res / 2
-
-
-def choose_popular_rules(rule_matrix: np.array) -> np.array:
-    '''
-    Returns the index of the rules that contain the most popular antecedent in the dataset.
-
-    :param rule_matrix: matrix with the rules.
-    :return: numpy array with the rules that contain the most popular antecedent in the dataset.
-    '''
-    appearances = _histogram(rule_matrix)
-    antecedent, vl = _max_values(appearances)
-
-    chosen_rules = rule_matrix[:, antecedent] == vl
-
-    return chosen_rules
-
-
-def connect_rulebase(rulebase: rules.RuleBase) -> list[np.array]:
-    '''
-    Connects antecedents connected by checking if both are in the same rule.
-
-    :param rulebase: Rule base to connect.
-    :return: List of pandas dataframes with the connections in adjacency matrix format.
-    '''
-
-    # We choose those rules to explain, as those who have the most common antecedent.
-    rule_matrix = rules.list_rules_to_matrix(rulebase.rules)
-    res = []
-    antecedents_names = [
-        x.name + ' ' + y for x in rulebase.antecedents for y in rulebase.antecedents[0].linguistic_variable_names()]
-
-    while rule_matrix.shape[0] > 0:
-        rules_to_viz = rule_matrix[choose_popular_rules(rule_matrix), :]
-        rule_matrix = rule_matrix[(
-            1 - choose_popular_rules(rule_matrix)).astype(bool), :]
-
-        graph_rule = create_graph_connection(rules_to_viz, len(
-            rulebase.antecedents[0].linguistic_variable_names()))
-        res.append(pd.DataFrame(
-            graph_rule, columns=antecedents_names, index=antecedents_names))
-
-    return res
-
-
-def connect_master_rulebase(mrule_base: rules.MasterRuleBase) -> list[list[np.array]]:
-    '''
-    Connects antecedents connected by checking if both are in the same rule.
-
-    :param mrule_base: Master rule base to connect.
-    :return: List of list of pandas dataframes with the connections in adjacency matrix format.
-    '''
-    res = []
-    for rule_base in mrule_base.rule_bases:
-        res.append(connect_rulebase(rule_base))
-
-    return res
-
-
-def visualize_rulebase(mrule_base: rules.MasterRuleBase, export_path: str=None) -> None:
-    '''
-    Visualize a rule base using low, medium and high partitions with 1 rule in common -> 1 edge connections.
-
-    :param mrule_base: Master rule base to visualize.
-    :param export_path: Path to export the graph.
-    '''
-
-    if mnt.save_usage_flag:
-        mnt.usage_data[mnt.usage_categories.Visualization]['plot_graph'] += 1
-
-    def color_func(a):
-        '''
-        Returns the color of the node according to the linguistic variable.
-
-        :param a: Node name.
-        :return: Color of the node.
-        '''
-        node_colors = ['blue', 'yellow', 'red']
-
-        if ' L' in a:
-            return node_colors[0]
-        elif ' M' in a:
-            return node_colors[1]
-        else:
-            return node_colors[2]
-
-    def vl_prune(a): return a.replace('High', 'H').replace(
-        'Medium', 'M').replace('Low', 'L').strip()
-
-    if isinstance(mrule_base, evf.BaseFuzzyRulesClassifier):
-        mrule_base = mrule_base.rule_base
-
-    connected_mrule_base = connect_master_rulebase(mrule_base)
-
-    for ix, connected_rule_base in enumerate(connected_mrule_base):
-        for jx, rule in enumerate(connected_rule_base):
-            G = nx.from_pandas_adjacency(rule)
-            isolated_nodes = [
-                node for node in G.nodes() if G.degree(node) == 0]
-            G.remove_nodes_from(isolated_nodes)
-            auto_edges = nx.selfloop_edges(G)
-            G.remove_edges_from(auto_edges)
-
-            new_node_names = [vl_prune(node) for node in G.nodes()]
-            mapping = dict(zip(G, new_node_names))
-            G = nx.relabel_nodes(G, mapping)
-
-            if jx == 0:
-                G_final = G
-            else:
-                G_final = nx.compose(G_final, G)
-
-        fig, ax = plt.subplots()
-        try:
-            os = nx.nx_agraph.graphviz_layout(G_final, prog='sfdp')
-        except ImportError:
-            os = nx.kamada_kawai_layout(G_final)
-
-        node_colors = [color_func(node) for node in G_final.nodes()]
-        nx.draw(G_final, with_labels=True, ax=ax,
-                pos=os, node_color=node_colors)
-        plt.title('Consequent: ' + str(ix))
-        fig.show()
-
-        if export_path is not None:
-            nx.write_gexf(G_final, os.path.join(export_path,
-                          'consequent_' + str(ix) + '.gexf'))
-
-
-def plot_fuzzy_variable(fuzzy_variable: fs.fuzzyVariable) -> None:
-    '''
-    Plots a fuzzy variable using trapezoidal membership functions.
-
-    :param fuzzy_variable: a fuzzy variable from the fuzzyVariable class in fuzzy_set module.
-    :return: None
-    '''
-    if mnt.save_usage_flag:
-        mnt.usage_data[mnt.usage_categories.Visualization]['plot_fuzzy_variable'] += 1
-
-    if fuzzy_variable.linguistic_variables[0].type() != fs.FUZZY_SETS.gt2:
-        fig, ax = plt.subplots()
-    else:
-        fig = plt.figure()
-        ax = plt.axes(projection='3d')
-
-    memberships = [0, 1, 1, 0]
-
-    colors = ['b', 'r', 'g', 'orange', 'y']
-    for ix, fuzzy_set in enumerate(fuzzy_variable.linguistic_variables):
-        name = fuzzy_set.name
-        initiated = False
-        fz_studied =  fuzzy_set.type()
-
-        if  fz_studied == fs.FUZZY_SETS.t1:
-            ax.plot(fuzzy_set.membership_parameters,
-                    memberships, colors[ix], label=name)
-        elif fz_studied == fs.FUZZY_SETS.t2:
-            ax.plot(fuzzy_set.secondMF_lower, np.array(memberships) * fuzzy_set.lower_height, 'black')
-            ax.plot(fuzzy_set.secondMF_upper, np.array(memberships), 'black')
-
-            # Compute the memberships for the lower/upper membership points. We do it in this way because non-exact 0/1s give problems.
-            x_lower = fuzzy_set.secondMF_lower
-            x_lower_lmemberships = [0.0 ,fuzzy_set.lower_height ,fuzzy_set.lower_height, 0.0] 
-            x_lower_umemberships = [fuzzy_set(x_lower[0])[1] , 1.0, 1.0 , fuzzy_set(x_lower[3])[1]]
-
-            x_upper = fuzzy_set.secondMF_upper
-            x_upper_lmemberships  = [0.0 , fuzzy_set(x_upper[1])[0], fuzzy_set(x_upper[2])[0], 0.0] 
-            x_upper_umemberships  = [0.0 ,1.0 ,1.0, 0.0] 
-
-            x_values = list(x_lower) + list(x_upper)
-            lmembership_values = list(x_lower_lmemberships) + list(x_upper_lmemberships)
-            umembership_values = list(x_lower_umemberships) + list(x_upper_umemberships)
-            aux_df = pd.DataFrame(zip(x_values, lmembership_values, umembership_values),  columns=['x', 'l', 'u'])
-            
-
-            if len(aux_df['x']) != len(set(aux_df['x'])): # There are repeated elements, so we use an order that should work in this case
-                # u0 l0 u1 l1 l2 u2 l3 u3
-                x = list((x_upper[0], x_lower[0], x_upper[1], x_lower[1], x_lower[2], x_upper[2], x_lower[3], x_upper[3]))
-                l_memberships = list((x_upper_lmemberships[0], x_lower_lmemberships[0], x_upper_lmemberships[1], x_lower_lmemberships[1], x_lower_lmemberships[2], x_upper_lmemberships[2], x_lower_lmemberships[3], x_upper_lmemberships[3]))
-                u_memberships = list((x_upper_umemberships[0], x_lower_umemberships[0], x_upper_umemberships[1], x_lower_umemberships[1], x_lower_umemberships[2], x_upper_umemberships[2], x_lower_umemberships[3], x_upper_umemberships[3]))
-
-                ax.fill_between(x, l_memberships, u_memberships, color=colors[ix], alpha=0.5, label=name)
-            else:
-                aux_df.sort_values('x', inplace=True)
-                ax.fill_between(aux_df['x'], aux_df['l'], aux_df['u'], color=colors[ix], alpha=0.5, label=name)
-
-        elif fz_studied == fs.FUZZY_SETS.gt2:
-            for key, value in fuzzy_set.secondary_memberships.items():
-                
-                gt2_memberships = value(fuzzy_set.sample_unit_domain)
-                key_plot = [float(key)]*sum(gt2_memberships > 0)
-                if initiated:
-                    ax.plot(key_plot, fuzzy_set.sample_unit_domain[gt2_memberships > 0], gt2_memberships[gt2_memberships > 0], color=colors[ix])
-                else:
-                    ax.plot(key_plot,  fuzzy_set.sample_unit_domain[gt2_memberships > 0], gt2_memberships[gt2_memberships > 0], color=colors[ix], label=name)
-                    initiated = True
-
-    ax.legend(loc='upper right', shadow=True)
-    plt.title(fuzzy_variable.name)
-    fig.show()
-
-
-def matrix_rule_base_form(rule_base: rules.Rule) -> pd.DataFrame:
-    '''
-    Returns a matrix with the rule base in the form of a matrix to visualize.
-
-    :param mrule_base: Rule base to transform.
-    :return: Matrix with the rule base in the form of a matrix.
-    '''
-
-    n_rules = len(rule_base.rules)
-    antecedents = len(rule_base.antecedents)
-
-    res = pd.DataFrame(np.zeros((n_rules, antecedents)), columns=[jx.name for jx in rule_base.antecedents])
-
-    for ix, rule in enumerate(rule_base):
-        for jx, antecedent in enumerate(rule_base.antecedents):
-            res.loc[ix, antecedent.name] = rule.antecedents[jx]
-    
-    return res
-
-
-def filter_useless_columns(df: pd.DataFrame) -> pd.DataFrame:
-    '''
-    Filter columns with only one value.
-
-    :param df: Dataframe to filter.
-    :return: Filtered dataframe.
-    '''
-    for column in df.columns:
-        if df[column].unique()[0] == -1:
-            df.drop(column, axis=1, inplace=True)
-
-    return df
-
-
-def rules_to_latex(rule_base:rules.MasterRuleBase) -> str:
-    '''
-    Prints the rule base in a latex format. It prints
-
-    :note: if the rule base has three different linguistic labels, it will use custom commands for the partitions. You can define these commands (\low, \mid, \hig, \dc) to show colors, figures, etc. Be sure to recheck the DS, ACC values in this case, because 1.0 values of them are also converted to these commands.
-    
-    :param rule_base: the master rule base to print.
-    :returns: the String as a latex tabular.
-    '''
-    class proxy_dict():
-
-        def __init__(self) -> None:
-            self.cell_colors = {
-                -1: '\\dc',
-                0: '\\low',
-                1: '\\med',
-                2: '\\hig'
-            }
-        
-        def __getitem__(self, value) -> str:
-            if value in self.cell_colors.keys():
-                return self.cell_colors[value]
-            else:
-                return "{:.2f}".format(value)
-
-
-    # Define the mapping for cell colors
-    rules_matrix = rule_base.get_rulebase_matrix()
-
-    # Add the consequent to the rules
-    cons_rules_matrix = []
-    for ix_cons, ruls in enumerate(rules_matrix):
-        for rule_list in ruls:
-            if len(rule_list.shape) == 2:
-                cons_rules_matrix.append(np.append(np.ones((rule_list.shape[0])) * ix_cons, rule_list, axis=1))
-            else:
-                cons_rules_matrix.append(np.append(np.ones((1, )) * ix_cons, rule_list))
-                     
-    dominance_scores = np.array([x.score for x in rule_base.get_rules()])
-    if len(dominance_scores.shape) == 2:
-        dominance_scores = np.mean(dominance_scores, axis=1, keepdims=True)
-    else:
-        dominance_scores = np.expand_dims(dominance_scores, axis=1)
-
-    accs = np.array([x.accuracy for x in rule_base.get_rules()])
-    accs = np.expand_dims(accs, axis=1)
-    cons_rules_matrix = np.append(np.append(np.array(cons_rules_matrix), dominance_scores, axis=1), accs, axis=1)
-    column_order = ['Consequent'] + [a.name for a in rule_base.antecedents] + ['DS', 'Acc']
-    df = pd.DataFrame(cons_rules_matrix, columns=column_order)
-    cell_colors = proxy_dict()
-
-    # Create the LaTeX table
-    latex_table = "\\begin{tabular}{" + "c" * (len(column_order)-2) + "|cc}\n"
-    latex_table += "\t\\toprule\n"
-    latex_table += "\t" + " & ".join(column_order) + " \\\\\n"
-    latex_table += "\t\\midrule\n"
-
-    i = 0
-    for cluster, group in df.groupby('Consequent'):
-            latex_table += f"\t\\multirow{{{len(group)}}}{{*}}{{{cluster}}}"
-            for _, row in group.iterrows():
-                if i % 2 == 0: # Add a shade of grey
-                    latex_table += " & \cellcolor{gray!25}" + " & \cellcolor{gray!25}".join([cell_colors[val] for val in row[column_order[1:]]]) + " \\\\\n"
-                else:
-                    latex_table += " & " + " & ".join([cell_colors[val] for val in row[column_order[1:]]]) + " \\\\\n"
-                i += 1
-            if cluster != len(rules_matrix) - 1:
-                latex_table += "\t\\midrule\n"            
-                
-    latex_table += "\t\\bottomrule\n"
-    latex_table += "\\end{tabular}"
-
+# -*- coding: utf-8 -*-
+"""
+This is a the source file that contains the functions necessary to visualize the set of rules.
+"""
+import os
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import networkx as nx
+
+try:
+    from . import rules
+    from . import evolutionary_fit as evf
+    from . import fuzzy_sets as fs
+    from . import maintenance as mnt
+except ImportError:
+    import rules
+    import evolutionary_fit as evf
+    import fuzzy_sets as fs
+    import maintenance as mnt
+
+
+def _column_histogram(rule_matrix: np.array) -> dict:
+    '''
+    Computes the histogram for all the unique values in a column.
+
+    :param rule_matrix: vector with the numerical values.
+    :return: dictionary with the histogram.
+    '''
+    res = {}
+    for x in np.unique(rule_matrix):
+        if x != -1:
+            res[x] = np.sum(rule_matrix == x)
+
+    return res
+
+
+def _histogram(rule_matrix: np.array) -> list[dict]:
+    '''
+    Returns a list with the histogram for each antecedent according to linguist variables.
+
+    :param rule_matrix: matrix with the rules.
+    :return: list with the histogram in dictionary format for each antecedent.
+    '''
+    res = []
+
+    for column_ix in range(rule_matrix.shape[1]):
+        res.append(_column_histogram(rule_matrix[:, column_ix]))
+
+    return res
+
+
+def _max_values(appearances: list) -> tuple[int, int]:
+    '''
+    Returns the antecedent and its linguistic value most repeated.
+
+    :param appearances: list with the histogram for each antecedent.
+    :return: tuple with the antecedent and its linguistic value most repeated.
+    '''
+    res = 0
+    antecedent = None
+    vl = None
+
+    for ix, apperances_an in enumerate(appearances):
+        for key, value in apperances_an.items():
+            if value > res:
+                res = value
+                antecedent = ix
+                vl = key
+
+    return antecedent, vl
+
+
+def create_graph_connection(rules, possible_vl):
+    '''
+    Returns a square matrix where each number indicates if two nodes are connected.
+    Connectes by checking if both are in the same rule.
+
+    :param rules: list with the rules.
+    :param possible_vl: number of linguistic variables.
+    :return: square matrix where each number indicates if two nodes are connected.
+    '''
+    def generate_index(ant, vl0): return int(possible_vl * ant + vl0)
+    res = np.zeros(
+        (possible_vl * rules.shape[1], possible_vl * rules.shape[1]))
+
+    for rule in rules:
+        for antecedent, vl in enumerate(rule):
+            if vl > -1:
+                for antecedent2, vl2 in enumerate(rule):
+                    if vl2 > -1:
+                        res_index1 = generate_index(antecedent, vl)
+                        res_index2 = generate_index(antecedent2, vl2)
+
+                        res[res_index1, res_index2] += 1
+
+    return res / 2
+
+
+def choose_popular_rules(rule_matrix: np.array) -> np.array:
+    '''
+    Returns the index of the rules that contain the most popular antecedent in the dataset.
+
+    :param rule_matrix: matrix with the rules.
+    :return: numpy array with the rules that contain the most popular antecedent in the dataset.
+    '''
+    appearances = _histogram(rule_matrix)
+    antecedent, vl = _max_values(appearances)
+
+    chosen_rules = rule_matrix[:, antecedent] == vl
+
+    return chosen_rules
+
+
+def connect_rulebase(rulebase: rules.RuleBase) -> list[np.array]:
+    '''
+    Connects antecedents connected by checking if both are in the same rule.
+
+    :param rulebase: Rule base to connect.
+    :return: List of pandas dataframes with the connections in adjacency matrix format.
+    '''
+
+    # We choose those rules to explain, as those who have the most common antecedent.
+    rule_matrix = rules.list_rules_to_matrix(rulebase.rules)
+    res = []
+    antecedents_names = [
+        x.name + ' ' + y for x in rulebase.antecedents for y in rulebase.antecedents[0].linguistic_variable_names()]
+
+    try:
+        while rule_matrix.shape[0] > 0:
+            rules_to_viz = rule_matrix[choose_popular_rules(rule_matrix), :]
+            rule_matrix = rule_matrix[(
+                1 - choose_popular_rules(rule_matrix)).astype(bool), :]
+
+            graph_rule = create_graph_connection(rules_to_viz, len(
+                rulebase.antecedents[0].linguistic_variable_names()))
+            res.append(pd.DataFrame(
+                graph_rule, columns=antecedents_names, index=antecedents_names))
+    except:
+        print('Error in the visualization of the rule base, probably because the rulebase is too small')
+
+    return res
+
+
+def connect_master_rulebase(mrule_base: rules.MasterRuleBase) -> list[list[np.array]]:
+    '''
+    Connects antecedents connected by checking if both are in the same rule.
+
+    :param mrule_base: Master rule base to connect.
+    :return: List of list of pandas dataframes with the connections in adjacency matrix format.
+    '''
+    res = []
+    for rule_base in mrule_base.rule_bases:
+        res.append(connect_rulebase(rule_base))
+
+    return res
+
+
+def visualize_rulebase(mrule_base: rules.MasterRuleBase, export_path: str=None) -> None:
+    '''
+    Visualize a rule base using low, medium and high partitions with 1 rule in common -> 1 edge connections.
+
+    :param mrule_base: Master rule base to visualize.
+    :param export_path: Path to export the graph.
+    '''
+
+    if mnt.save_usage_flag:
+        mnt.usage_data[mnt.usage_categories.Visualization]['plot_graph'] += 1
+
+    def color_func(a):
+        '''
+        Returns the color of the node according to the linguistic variable.
+
+        :param a: Node name.
+        :return: Color of the node.
+        '''
+        node_colors = ['blue', 'yellow', 'red']
+
+        if ' L' in a:
+            return node_colors[0]
+        elif ' M' in a:
+            return node_colors[1]
+        else:
+            return node_colors[2]
+
+    def vl_prune(a): return a.replace('High', 'H').replace(
+        'Medium', 'M').replace('Low', 'L').strip()
+
+    if isinstance(mrule_base, evf.BaseFuzzyRulesClassifier):
+        mrule_base = mrule_base.rule_base
+
+    connected_mrule_base = connect_master_rulebase(mrule_base)
+
+    for ix, connected_rule_base in enumerate(connected_mrule_base):
+        for jx, rule in enumerate(connected_rule_base):
+            G = nx.from_pandas_adjacency(rule)
+            isolated_nodes = [
+                node for node in G.nodes() if G.degree(node) == 0]
+            G.remove_nodes_from(isolated_nodes)
+            auto_edges = nx.selfloop_edges(G)
+            G.remove_edges_from(auto_edges)
+
+            new_node_names = [vl_prune(node) for node in G.nodes()]
+            mapping = dict(zip(G, new_node_names))
+            G = nx.relabel_nodes(G, mapping)
+
+            if jx == 0:
+                G_final = G
+            else:
+                G_final = nx.compose(G_final, G)
+
+        fig, ax = plt.subplots()
+        try:
+            os = nx.nx_agraph.graphviz_layout(G_final, prog='sfdp')
+        except ImportError:
+            os = nx.kamada_kawai_layout(G_final)
+
+        node_colors = [color_func(node) for node in G_final.nodes()]
+        nx.draw(G_final, with_labels=True, ax=ax,
+                pos=os, node_color=node_colors)
+        plt.title('Consequent: ' + str(ix))
+        fig.show()
+
+        if export_path is not None:
+            nx.write_gexf(G_final, os.path.join(export_path,
+                          'consequent_' + str(ix) + '.gexf'))
+
+
+def plot_fuzzy_variable(fuzzy_variable: fs.fuzzyVariable) -> None:
+    '''
+    Plots a fuzzy variable using trapezoidal membership functions.
+
+    :param fuzzy_variable: a fuzzy variable from the fuzzyVariable class in fuzzy_set module.
+    :return: None
+    '''
+    if mnt.save_usage_flag:
+        mnt.usage_data[mnt.usage_categories.Visualization]['plot_fuzzy_variable'] += 1
+
+    if fuzzy_variable.linguistic_variables[0].type() != fs.FUZZY_SETS.gt2:
+        fig, ax = plt.subplots()
+    else:
+        fig = plt.figure()
+        ax = plt.axes(projection='3d')
+
+    memberships = [0, 1, 1, 0]
+
+    colors = ['b', 'r', 'g', 'orange', 'y']
+    for ix, fuzzy_set in enumerate(fuzzy_variable.linguistic_variables):
+        name = fuzzy_set.name
+        initiated = False
+        fz_studied =  fuzzy_set.type()
+
+        if  fz_studied == fs.FUZZY_SETS.t1:
+            ax.plot(fuzzy_set.membership_parameters,
+                    memberships, colors[ix], label=name)
+        elif fz_studied == fs.FUZZY_SETS.t2:
+            ax.plot(fuzzy_set.secondMF_lower, np.array(memberships) * fuzzy_set.lower_height, 'black')
+            ax.plot(fuzzy_set.secondMF_upper, np.array(memberships), 'black')
+
+            # Compute the memberships for the lower/upper membership points. We do it in this way because non-exact 0/1s give problems.
+            x_lower = fuzzy_set.secondMF_lower
+            x_lower_lmemberships = [0.0 ,fuzzy_set.lower_height ,fuzzy_set.lower_height, 0.0] 
+            x_lower_umemberships = [fuzzy_set(x_lower[0])[1] , 1.0, 1.0 , fuzzy_set(x_lower[3])[1]]
+
+            x_upper = fuzzy_set.secondMF_upper
+            x_upper_lmemberships  = [0.0 , fuzzy_set(x_upper[1])[0], fuzzy_set(x_upper[2])[0], 0.0] 
+            x_upper_umemberships  = [0.0 ,1.0 ,1.0, 0.0] 
+
+            x_values = list(x_lower) + list(x_upper)
+            lmembership_values = list(x_lower_lmemberships) + list(x_upper_lmemberships)
+            umembership_values = list(x_lower_umemberships) + list(x_upper_umemberships)
+            aux_df = pd.DataFrame(zip(x_values, lmembership_values, umembership_values),  columns=['x', 'l', 'u'])
+            
+
+            if len(aux_df['x']) != len(set(aux_df['x'])): # There are repeated elements, so we use an order that should work in this case
+                # u0 l0 u1 l1 l2 u2 l3 u3
+                x = list((x_upper[0], x_lower[0], x_upper[1], x_lower[1], x_lower[2], x_upper[2], x_lower[3], x_upper[3]))
+                l_memberships = list((x_upper_lmemberships[0], x_lower_lmemberships[0], x_upper_lmemberships[1], x_lower_lmemberships[1], x_lower_lmemberships[2], x_upper_lmemberships[2], x_lower_lmemberships[3], x_upper_lmemberships[3]))
+                u_memberships = list((x_upper_umemberships[0], x_lower_umemberships[0], x_upper_umemberships[1], x_lower_umemberships[1], x_lower_umemberships[2], x_upper_umemberships[2], x_lower_umemberships[3], x_upper_umemberships[3]))
+
+                ax.fill_between(x, l_memberships, u_memberships, color=colors[ix], alpha=0.5, label=name)
+            else:
+                aux_df.sort_values('x', inplace=True)
+                ax.fill_between(aux_df['x'], aux_df['l'], aux_df['u'], color=colors[ix], alpha=0.5, label=name)
+
+        elif fz_studied == fs.FUZZY_SETS.gt2:
+            for key, value in fuzzy_set.secondary_memberships.items():
+                
+                gt2_memberships = value(fuzzy_set.sample_unit_domain)
+                key_plot = [float(key)]*sum(gt2_memberships > 0)
+                if initiated:
+                    ax.plot(key_plot, fuzzy_set.sample_unit_domain[gt2_memberships > 0], gt2_memberships[gt2_memberships > 0], color=colors[ix])
+                else:
+                    ax.plot(key_plot,  fuzzy_set.sample_unit_domain[gt2_memberships > 0], gt2_memberships[gt2_memberships > 0], color=colors[ix], label=name)
+                    initiated = True
+
+    ax.legend(loc='upper right', shadow=True)
+    plt.title(fuzzy_variable.name)
+    fig.show()
+
+
+def matrix_rule_base_form(rule_base: rules.Rule) -> pd.DataFrame:
+    '''
+    Returns a matrix with the rule base in the form of a matrix to visualize.
+
+    :param mrule_base: Rule base to transform.
+    :return: Matrix with the rule base in the form of a matrix.
+    '''
+
+    n_rules = len(rule_base.rules)
+    antecedents = len(rule_base.antecedents)
+
+    res = pd.DataFrame(np.zeros((n_rules, antecedents)), columns=[jx.name for jx in rule_base.antecedents])
+
+    for ix, rule in enumerate(rule_base):
+        for jx, antecedent in enumerate(rule_base.antecedents):
+            res.loc[ix, antecedent.name] = rule.antecedents[jx]
+    
+    return res
+
+
+def filter_useless_columns(df: pd.DataFrame) -> pd.DataFrame:
+    '''
+    Filter columns with only one value.
+
+    :param df: Dataframe to filter.
+    :return: Filtered dataframe.
+    '''
+    for column in df.columns:
+        if df[column].unique()[0] == -1:
+            df.drop(column, axis=1, inplace=True)
+
+    return df
+
+
+def rules_to_latex(rule_base:rules.MasterRuleBase) -> str:
+    '''
+    Prints the rule base in a latex format. It prints
+
+    :note: if the rule base has three different linguistic labels, it will use custom commands for the partitions. You can define these commands (\low, \mid, \hig, \dc) to show colors, figures, etc. Be sure to recheck the DS, ACC values in this case, because 1.0 values of them are also converted to these commands.
+    
+    :param rule_base: the master rule base to print.
+    :returns: the String as a latex tabular.
+    '''
+    class proxy_dict():
+
+        def __init__(self) -> None:
+            self.cell_colors = {
+                -1: '\\dc',
+                0: '\\low',
+                1: '\\med',
+                2: '\\hig'
+            }
+        
+        def __getitem__(self, value) -> str:
+            if value in self.cell_colors.keys():
+                return self.cell_colors[value]
+            else:
+                return "{:.2f}".format(value)
+
+
+    # Define the mapping for cell colors
+    rules_matrix = rule_base.get_rulebase_matrix()
+
+    # Add the consequent to the rules
+    cons_rules_matrix = []
+    for ix_cons, ruls in enumerate(rules_matrix):
+        for rule_list in ruls:
+            if len(rule_list.shape) == 2:
+                cons_rules_matrix.append(np.append(np.ones((rule_list.shape[0])) * ix_cons, rule_list, axis=1))
+            else:
+                cons_rules_matrix.append(np.append(np.ones((1, )) * ix_cons, rule_list))
+                     
+    dominance_scores = np.array([x.score for x in rule_base.get_rules()])
+    if len(dominance_scores.shape) == 2:
+        dominance_scores = np.mean(dominance_scores, axis=1, keepdims=True)
+    else:
+        dominance_scores = np.expand_dims(dominance_scores, axis=1)
+
+    accs = np.array([x.accuracy for x in rule_base.get_rules()])
+    accs = np.expand_dims(accs, axis=1)
+    cons_rules_matrix = np.append(np.append(np.array(cons_rules_matrix), dominance_scores, axis=1), accs, axis=1)
+    column_order = ['Consequent'] + [a.name for a in rule_base.antecedents] + ['DS', 'Acc']
+    df = pd.DataFrame(cons_rules_matrix, columns=column_order)
+    cell_colors = proxy_dict()
+
+    # Create the LaTeX table
+    latex_table = "\\begin{tabular}{" + "c" * (len(column_order)-2) + "|cc}\n"
+    latex_table += "\t\\toprule\n"
+    latex_table += "\t" + " & ".join(column_order) + " \\\\\n"
+    latex_table += "\t\\midrule\n"
+
+    i = 0
+    for cluster, group in df.groupby('Consequent'):
+            latex_table += f"\t\\multirow{{{len(group)}}}{{*}}{{{cluster}}}"
+            for _, row in group.iterrows():
+                if i % 2 == 0: # Add a shade of grey
+                    latex_table += " & \cellcolor{gray!25}" + " & \cellcolor{gray!25}".join([cell_colors[val] for val in row[column_order[1:]]]) + " \\\\\n"
+                else:
+                    latex_table += " & " + " & ".join([cell_colors[val] for val in row[column_order[1:]]]) + " \\\\\n"
+                i += 1
+            if cluster != len(rules_matrix) - 1:
+                latex_table += "\t\\midrule\n"            
+                
+    latex_table += "\t\\bottomrule\n"
+    latex_table += "\\end{tabular}"
+
     print(latex_table)
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.0/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,78 @@
-Metadata-Version: 2.1
-Name: ex_fuzzy
-Version: 1.0.7
-Summary: Library to perform explainable AI using fuzzy logic.
-Home-page: https://github.com/Fuminides/ex-fuzzy
-Download-URL: https://pypi.org/project/ex-fuzzy/
-Maintainer: Javier Fumanal Idocin
-Maintainer-email: javierfumanalidocin@gmail.com
-License: GPL-3.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: matplotlib
-Requires-Dist: pymoo
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
-
-# Ex-Fuzzy
-ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
-
-Some of the tools available in this library include:
-
-- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
-- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
-- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
-- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
-
-## Main Characteristics
-
-### Easy to use
-
-ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
-
-### Reusable code
-
-Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
-
-### Sci-py like interface
-
-ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
-
-### Visualization
-
-Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
-
-
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
-  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
-  
-</p>
-
-## Dependencies
-
-- Numpy
-- Pandas
-- Matplotlib
-- Networkx
-- Pymoo
-
-## Installation
-
-You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
-
-`pip install ex-fuzzy`
-
-
-## Contributors
-Javier Fumanal Idocin, Javier Andreu-Perez
-
-All rights reserved, 2021-2024
-
-
+Metadata-Version: 2.1
+Name: ex-fuzzy
+Version: 1.1.0
+Summary: Library to perform explainable AI using fuzzy logic.
+Home-page: https://github.com/Fuminides/ex-fuzzy
+Download-URL: https://pypi.org/project/ex-fuzzy/
+Maintainer: Javier Fumanal Idocin
+Maintainer-email: javierfumanalidocin@gmail.com
+License: GPL-3.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+
+# Ex-Fuzzy
+ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
+
+Some of the tools available in this library include:
+
+- Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
+- Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
+- Support for various kinds of fuzzy sets, including classic fuzzy sets, IV-fuzzy sets and General Type 2 fuzzy sets.
+- Rule mining using support, confidence and lift measures. Customizable genetic optimization of the rule bases parameters.
+
+## Main Characteristics
+
+### Easy to use
+
+ex-Fuzzy is designed to be easy to use. Linguistic variables can be precomputed and optimized without any understading of its implementation. Choosing one kind of fuzzy set only requires to set one flag. 
+
+### Reusable code
+
+Code is designed so that some parts can be easily extendable so that some use cases, like research, can be also supported. The rule base optimization is done using a Genetic Algorithm, but almost any other pymoo search algorithm will do. Fuzzy sets can be extended with ease, just as the kind of partitions, membership functions, etc.
+
+### Sci-py like interface
+
+ex-Fuzzy is built taking into account the actual machine-learing frameworks used in Python. Training amd sing a rule base classifier works exactly as sci-kit learn classifier. Parameters such as the number of rules or antecedents are also built 
+
+### Visualization
+
+Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
+
+
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
+  <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
+  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
+  
+</p>
+
+## Dependencies
+
+- Numpy
+- Pandas
+- Matplotlib
+- Networkx
+- Pymoo
+
+## Installation
+
+You can install ex-Fuzzy using pip, from the PyPi repository, with the following command:
+
+`pip install ex-fuzzy`
+
+
+## Contributors
+Javier Fumanal Idocin, Javier Andreu-Perez
+
+All rights reserved, 2021-2024
+
+
```

### Comparing `ex_fuzzy-1.0.7/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.0/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.0.7/tests/test_centroids.py` & `ex_fuzzy-1.1.0/tests/test_centroids.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import numpy as np
-import math
-
-import sys
-sys.path.append('../ex_fuzzy/')
-
-import ex_fuzzy as ex_fuzzy
-
-def test_t2_centroid():
-    '''
-    Tests that fuzzy t2 (iv) centroids compute correctly.
-    '''
-    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0.35, 0.4, 0.6, 0.65], [0.25 ,0.4, 0.6, 0.75], [0,1], lower_height=0.8)
-    z = np.arange(0, 1, 0.001)
-    assert math.isclose(ex_fuzzy.centroid.compute_centroid_iv(z, trial_fs(z))[0], 0.5, abs_tol=0.01), 'T2 centroid right not correctly computed'
-    assert math.isclose(ex_fuzzy.centroid.compute_centroid_iv(z, trial_fs(z))[1], 0.5, abs_tol=0.01), 'T2 centroid left not correctly computed'
-
-
-def test_t2_centroid_centroids():
-    '''
-    Tests that fuzzy t2 (iv) centroid computed from previous centroids is computed correctly.
-    '''
-    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0.35, 0.4, 0.6, 0.65], [0.25 ,0.4, 0.6, 0.75], [0,1], lower_height=0.8)
-    z = np.arange(0, 1, 0.001)
-    assert math.isclose(ex_fuzzy.centroid.compute_centroid_t2_r(z, trial_fs(z)), 0.5, abs_tol=0.01), 'T2 centroid right not correctly computed'
-    assert math.isclose(ex_fuzzy.centroid.compute_centroid_t2_l(z, trial_fs(z)), 0.5, abs_tol=0.01), 'T2 centroid left not correctly computed'
-
-
+import numpy as np
+import math
+
+import sys
+sys.path.append('../ex_fuzzy/')
+
+import ex_fuzzy as ex_fuzzy
+
+def test_t2_centroid():
+    '''
+    Tests that fuzzy t2 (iv) centroids compute correctly.
+    '''
+    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0.35, 0.4, 0.6, 0.65], [0.25 ,0.4, 0.6, 0.75], [0,1], lower_height=0.8)
+    z = np.arange(0, 1, 0.001)
+    assert math.isclose(ex_fuzzy.centroid.compute_centroid_iv(z, trial_fs(z))[0], 0.5, abs_tol=0.01), 'T2 centroid right not correctly computed'
+    assert math.isclose(ex_fuzzy.centroid.compute_centroid_iv(z, trial_fs(z))[1], 0.5, abs_tol=0.01), 'T2 centroid left not correctly computed'
+
+
+def test_t2_centroid_centroids():
+    '''
+    Tests that fuzzy t2 (iv) centroid computed from previous centroids is computed correctly.
+    '''
+    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0.35, 0.4, 0.6, 0.65], [0.25 ,0.4, 0.6, 0.75], [0,1], lower_height=0.8)
+    z = np.arange(0, 1, 0.001)
+    assert math.isclose(ex_fuzzy.centroid.compute_centroid_t2_r(z, trial_fs(z)), 0.5, abs_tol=0.01), 'T2 centroid right not correctly computed'
+    assert math.isclose(ex_fuzzy.centroid.compute_centroid_t2_l(z, trial_fs(z)), 0.5, abs_tol=0.01), 'T2 centroid left not correctly computed'
+
+
```

### Comparing `ex_fuzzy-1.0.7/tests/test_classification.py` & `ex_fuzzy-1.1.0/tests/test_classification.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-
-import numpy as np
-import pandas as pd
-import math
-import sys
-sys.path.append('../ex_fuzzy/')
-sys.path.append('./ex_fuzzy/')
-
-import ex_fuzzy
-
-sample_size = 1000
-
-def test_random_classification(fs_type=ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1):
-    global sample_size
-
-    sample = np.random.random_sample((sample_size, 5))
-    targets = np.random.randint(0, 2, sample_size)
-
-    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, fs_type, verbose=False, tolerance=0.0, n_linguist_variables=3)
-    model.fit(sample, targets)
-    predictions = model.predict(sample)
-    assert math.isclose(np.mean(np.equal(predictions, targets)), 0.5, abs_tol=0.1)
-
-
-def test_random_classification_precomputed(fs_type=ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1):
-    global sample_size
-
-    sample = np.random.random_sample((sample_size, 5))
-    targets = np.random.randint(0, 2, sample_size)
-    vl_partitions = ex_fuzzy.utils.construct_partitions(sample, fs_type)
-    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, verbose=False, tolerance=0.0, linguistic_variables=vl_partitions)
-    model.fit(sample, targets)
-    predictions = model.predict(sample)
-    assert math.isclose(np.mean(np.equal(predictions, targets)), 0.5, abs_tol=0.1)
-
-
-def test_random_classification_t2():
-    test_random_classification(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
-
-
-def test_random_classification_t2_precomputed():
-    test_random_classification_precomputed(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
-
-
-def test_random_classification_gt2():
-    test_random_classification(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
-
-
-def test_random_classification_gt2_precomputed():
-    test_random_classification_precomputed(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
-
-if __name__ == '__main__':
-    test_random_classification_t2()
-    test_random_classification_t2_precomputed()
-    test_random_classification_gt2()
-    test_random_classification_gt2_precomputed()
+
+import numpy as np
+import pandas as pd
+import math
+import sys
+sys.path.append('../ex_fuzzy/')
+sys.path.append('./ex_fuzzy/')
+
+import ex_fuzzy
+
+sample_size = 1000
+
+def test_random_classification(fs_type=ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1):
+    global sample_size
+
+    sample = np.random.random_sample((sample_size, 5))
+    targets = np.random.randint(0, 2, sample_size)
+
+    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, fs_type, verbose=False, tolerance=0.0, n_linguist_variables=3)
+    model.fit(sample, targets)
+    predictions = model.predict(sample)
+    assert math.isclose(np.mean(np.equal(predictions, targets)), 0.5, abs_tol=0.1)
+
+
+def test_random_classification_precomputed(fs_type=ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1):
+    global sample_size
+
+    sample = np.random.random_sample((sample_size, 5))
+    targets = np.random.randint(0, 2, sample_size)
+    vl_partitions = ex_fuzzy.utils.construct_partitions(sample, fs_type)
+    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, verbose=False, tolerance=0.0, linguistic_variables=vl_partitions)
+    model.fit(sample, targets)
+    predictions = model.predict(sample)
+    assert math.isclose(np.mean(np.equal(predictions, targets)), 0.5, abs_tol=0.1)
+
+
+def test_random_classification_t2():
+    test_random_classification(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
+
+
+def test_random_classification_t2_precomputed():
+    test_random_classification_precomputed(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
+
+
+def test_random_classification_gt2():
+    test_random_classification(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
+
+
+def test_random_classification_gt2_precomputed():
+    test_random_classification_precomputed(ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
+
+if __name__ == '__main__':
+    test_random_classification_t2()
+    test_random_classification_t2_precomputed()
+    test_random_classification_gt2()
+    test_random_classification_gt2_precomputed()
```

### Comparing `ex_fuzzy-1.0.7/tests/test_eval_tools.py` & `ex_fuzzy-1.1.0/tests/test_eval_tools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import numpy as np
-import ex_fuzzy
-import sys
-sys.path.append('../ex_fuzzy/')
-
-def test_eval_fuzzy_model():
-    '''
-    Test the eval_fuzzy_model function.
-
-    If it works, it should print the following:
-    Accuracy: 0.5 aprox
-    Matthews correlation coefficient: 0.0 aprox
-    '''
-    sample_size = 1000
-    sample = np.random.random_sample((sample_size, 5))
-    targets = np.random.randint(0, 2, sample_size)
-
-    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1, verbose=False, tolerance=0.0, n_linguist_variables=3)
-    model.fit(sample, targets)
-
-    ex_fuzzy.eval_tools.eval_fuzzy_model(model, sample, targets, sample, targets, 
-                        plot_rules=False, print_rules=False, plot_partitions=False)
-
+import numpy as np
+import ex_fuzzy
+import sys
+sys.path.append('../ex_fuzzy/')
+
+def test_eval_fuzzy_model():
+    '''
+    Test the eval_fuzzy_model function.
+
+    If it works, it should print the following:
+    Accuracy: 0.5 aprox
+    Matthews correlation coefficient: 0.0 aprox
+    '''
+    sample_size = 1000
+    sample = np.random.random_sample((sample_size, 5))
+    targets = np.random.randint(0, 2, sample_size)
+
+    model = ex_fuzzy.evolutionary_fit.BaseFuzzyRulesClassifier(10, 3, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1, verbose=False, tolerance=0.0, n_linguist_variables=3)
+    model.fit(sample, targets)
+
+    ex_fuzzy.eval_tools.eval_fuzzy_model(model, sample, targets, sample, targets, 
+                        plot_rules=False, print_rules=False, plot_partitions=False)
+
```

### Comparing `ex_fuzzy-1.0.7/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.0/tests/test_fuzzy_sets.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import numpy as np
-import math
-
-import sys
-sys.path.append('./ex_fuzzy/')
-sys.path.append('../ex_fuzzy/')
-import ex_fuzzy as ex_fuzzy
-
-
-def test_fuzzy_t1_memberships():
-    '''
-    Tests that fuzzy t1 memberships compute correctly.
-    '''
-    trial_fs = ex_fuzzy.fuzzy_sets.FS('trial', [0,0.1, 0.25, 0.5], [0,1])
-
-    assert trial_fs.name == 'trial', 'Name not correctly set'
-    assert trial_fs(0.1) == 1, 'Trapezoidal membership fails in first term'
-    assert trial_fs(1) == 0, 'Trapezoidal membership fails in last term'
-    assert trial_fs(0.51) == 0, 'Trapezoidal memberships does not stop where it shoud'
-    assert trial_fs(0.05) == 0.5, 'Trapeziodal membership increasining in non linear way' 
-
-
-def test_fuzzy_t2_memberships():
-    '''
-    Tests that fuzzy t2 (iv) memberships compute correctly.
-    '''
-    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0,0.1, 0.25, 0.4], [0, 0.15, 0.25, 0.5], [0,1], lower_height=0.8)
-
-    assert trial_fs.name == 'trial', 'Name not correctly set'
-    trial_mfs = trial_fs(0.2)
-    assert trial_mfs[0] <= trial_mfs[1], 'Incoherent lower and upper membership behaviour'
-
-
-def test_fuzzy_gt2_memberships():
-    '''
-    Tests that fuzzy gt2 memberships compute correctly.
-    '''
-    trial_fs = {}
-    for x in [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 1]:
-        trial_fs[x] = ex_fuzzy.fuzzy_sets.FS('trial', [0.25,0.5, 0.5, 0.75], [0,1])
-
-    trial_fs = ex_fuzzy.fuzzy_sets.GT2('trial', trial_fs, [0, 1], significant_decimals=1, unit_resolution=0.001)
-    res = trial_fs(0.3)
-    assert math.isclose(np.mean(trial_fs.alpha_reduction(res)), 0.5, abs_tol=0.1), 'GT2 memberships not correctly reduced'
-
-
-
-    
-if __name__ == '__main__':
-    test_fuzzy_t1_memberships()
-    test_fuzzy_t2_memberships()
+import numpy as np
+import math
+
+import sys
+sys.path.append('./ex_fuzzy/')
+sys.path.append('../ex_fuzzy/')
+import ex_fuzzy as ex_fuzzy
+
+
+def test_fuzzy_t1_memberships():
+    '''
+    Tests that fuzzy t1 memberships compute correctly.
+    '''
+    trial_fs = ex_fuzzy.fuzzy_sets.FS('trial', [0,0.1, 0.25, 0.5], [0,1])
+
+    assert trial_fs.name == 'trial', 'Name not correctly set'
+    assert trial_fs(0.1) == 1, 'Trapezoidal membership fails in first term'
+    assert trial_fs(1) == 0, 'Trapezoidal membership fails in last term'
+    assert trial_fs(0.51) == 0, 'Trapezoidal memberships does not stop where it shoud'
+    assert trial_fs(0.05) == 0.5, 'Trapeziodal membership increasining in non linear way' 
+
+
+def test_fuzzy_t2_memberships():
+    '''
+    Tests that fuzzy t2 (iv) memberships compute correctly.
+    '''
+    trial_fs = ex_fuzzy.fuzzy_sets.IVFS('trial', [0,0.1, 0.25, 0.4], [0, 0.15, 0.25, 0.5], [0,1], lower_height=0.8)
+
+    assert trial_fs.name == 'trial', 'Name not correctly set'
+    trial_mfs = trial_fs(0.2)
+    assert trial_mfs[0] <= trial_mfs[1], 'Incoherent lower and upper membership behaviour'
+
+
+def test_fuzzy_gt2_memberships():
+    '''
+    Tests that fuzzy gt2 memberships compute correctly.
+    '''
+    trial_fs = {}
+    for x in [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 1]:
+        trial_fs[x] = ex_fuzzy.fuzzy_sets.FS('trial', [0.25,0.5, 0.5, 0.75], [0,1])
+
+    trial_fs = ex_fuzzy.fuzzy_sets.GT2('trial', trial_fs, [0, 1], significant_decimals=1, unit_resolution=0.001)
+    res = trial_fs(0.3)
+    assert math.isclose(np.mean(trial_fs.alpha_reduction(res)), 0.5, abs_tol=0.1), 'GT2 memberships not correctly reduced'
+
+
+
+    
+if __name__ == '__main__':
+    test_fuzzy_t1_memberships()
+    test_fuzzy_t2_memberships()
     test_fuzzy_gt2_memberships()
```

### Comparing `ex_fuzzy-1.0.7/tests/test_utils.py` & `ex_fuzzy-1.1.0/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import numpy as np
-import math
-import sys
-
-sys.path.append('./ex_fuzzy/')
-sys.path.append('../ex_fuzzy/')
-import ex_fuzzy as ex_fuzzy
-
-sample_size = 10000
-tolerate = 0.05
-def test_quartiles():
-    sample = np.random.random_sample(sample_size)
-    targets = [0, 0.25, 0.5, 1]
-    quartiles = ex_fuzzy.utils.quartile_compute(sample)
-    for ix, target in enumerate(targets):
-        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
-
-def test_quantiles():
-    sample = np.random.random_sample(sample_size)
-    targets = [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1]
-    quartiles = ex_fuzzy.utils.fixed_quantile_compute(sample)
-    for ix, target in enumerate(targets):
-        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
-
-def test_3_partitions():
-    sample = np.random.random_sample(sample_size)
-    targets = [0, 0.20, 0.50, 0.80, 1.00]
-    quartiles = ex_fuzzy.utils.partition3_quantile_compute(sample)
-    for ix, target in enumerate(targets):
-        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
-
-
-def test_construct_partitions_t1():
-    sample = np.random.random_sample((sample_size, 1))
-    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1)
-    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
-    assert math.isclose(partitions[0](0.01)[0], 1, abs_tol=tolerate), 'Not the correct partition'
-
-
-def test_construct_partitions_t2():
-    sample = np.random.random_sample((sample_size, 1))
-    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
-    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
-    assert math.isclose(partitions[0](0.01)[0][0], 0.8, abs_tol=tolerate), 'Not the correct partition'
-    assert math.isclose(partitions[0](0.01)[0][1], 1, abs_tol=tolerate), 'Not the correct partition'
-
-
-def test_construct_partitions_gt2():
-    sample = np.random.random_sample((sample_size, 1))
-    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.gt2)
-    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
-    assert math.isclose(np.mean(partitions[0][0].alpha_reduction(partitions[0](0.1)[0])), 0.9, abs_tol=tolerate), 'Not the correct partition'
-
-
-def test_temporal_conditional():
-    sample_size = 10
-    sample = np.random.random_sample((sample_size, ))
-
-    first_temp = int(sample_size / 2)
-
-    sample[:first_temp] = sample[:first_temp] * 0.5
-    time_labels = [0] * sample_size
-    time_labels[first_temp:] = [1] * first_temp
-
-    vl1 = ex_fuzzy.fuzzy_sets.FS('',[0, 0.20, 0.30, 0.5], [0, 1])
-    vl2 = ex_fuzzy.fuzzy_sets.FS('',[0.5, 0.70, 0.80, 1], [0, 1])
-
-    conditional_frequencies = ex_fuzzy.utils.construct_conditional_frequencies(sample, time_labels, [vl1, vl2])
-
-    assert conditional_frequencies[0, 0] > conditional_frequencies[0, 1]
-    assert conditional_frequencies[1, 0] < conditional_frequencies[1, 1]
-
-
-def test_temporal_assemble():
-    sample_size = 1000
-    sample = np.random.random_sample((sample_size, 5))
-    y = np.random.randint(0, 2, sample_size)
-
-    temp_moments1 = np.random.randint(0, 2, sample_size)
-    temp_moments2 = 1 - temp_moments1
-    temp_moments = [temp_moments1, temp_moments2]
-
-    [X_train, X_test, y_train, y_test], [train_temporal_boolean_markers, test_temporal_boolean_markers] = ex_fuzzy.utils.temporal_assemble(sample, y, temp_moments)
-
-    t1test = [y_test[jx] for jx, aux in enumerate(test_temporal_boolean_markers[0]) if aux]
-    t2test = [y_test[jx] for jx, aux in enumerate(test_temporal_boolean_markers[1]) if aux]
-
-    assert len(t1test) == len(t2test)
-
-    
-
-
-if __name__ == '__main__':
-    test_quartiles()
-    test_quantiles()
-    test_3_partitions()
-    test_construct_partitions_t1()
-    test_construct_partitions_t2()
-    test_construct_partitions_gt2()
-    test_temporal_conditional()
-    test_temporal_assemble()
+import numpy as np
+import math
+import sys
+
+sys.path.append('./ex_fuzzy/')
+sys.path.append('../ex_fuzzy/')
+import ex_fuzzy as ex_fuzzy
+
+sample_size = 10000
+tolerate = 0.05
+def test_quartiles():
+    sample = np.random.random_sample(sample_size)
+    targets = [0, 0.25, 0.5, 1]
+    quartiles = ex_fuzzy.utils.quartile_compute(sample)
+    for ix, target in enumerate(targets):
+        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
+
+def test_quantiles():
+    sample = np.random.random_sample(sample_size)
+    targets = [0, 0.20, 0.30, 0.45, 0.55, 0.7, 0.8, 1]
+    quartiles = ex_fuzzy.utils.fixed_quantile_compute(sample)
+    for ix, target in enumerate(targets):
+        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
+
+def test_3_partitions():
+    sample = np.random.random_sample(sample_size)
+    targets = [0, 0.20, 0.50, 0.80, 1.00]
+    quartiles = ex_fuzzy.utils.partition3_quantile_compute(sample)
+    for ix, target in enumerate(targets):
+        assert math.isclose(quartiles[ix], target, abs_tol=tolerate), 'Not the correct ' +str(target) + ' quartile.'
+
+
+def test_construct_partitions_t1():
+    sample = np.random.random_sample((sample_size, 1))
+    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t1)
+    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
+    assert math.isclose(partitions[0](0.01)[0], 1, abs_tol=tolerate), 'Not the correct partition'
+
+
+def test_construct_partitions_t2():
+    sample = np.random.random_sample((sample_size, 1))
+    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.t2)
+    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
+    assert math.isclose(partitions[0](0.01)[0][0], 0.8, abs_tol=tolerate), 'Not the correct partition'
+    assert math.isclose(partitions[0](0.01)[0][1], 1, abs_tol=tolerate), 'Not the correct partition'
+
+
+def test_construct_partitions_gt2():
+    sample = np.random.random_sample((sample_size, 1))
+    partitions = ex_fuzzy.utils.construct_partitions(sample, ex_fuzzy.fuzzy_sets.FUZZY_SETS.gt2)
+    assert len(partitions[0]) == 3, 'Not the correct number of partitions'
+    assert math.isclose(np.mean(partitions[0][0].alpha_reduction(partitions[0](0.1)[0])), 0.9, abs_tol=tolerate), 'Not the correct partition'
+
+
+def test_temporal_conditional():
+    sample_size = 10
+    sample = np.random.random_sample((sample_size, ))
+
+    first_temp = int(sample_size / 2)
+
+    sample[:first_temp] = sample[:first_temp] * 0.5
+    time_labels = [0] * sample_size
+    time_labels[first_temp:] = [1] * first_temp
+
+    vl1 = ex_fuzzy.fuzzy_sets.FS('',[0, 0.20, 0.30, 0.5], [0, 1])
+    vl2 = ex_fuzzy.fuzzy_sets.FS('',[0.5, 0.70, 0.80, 1], [0, 1])
+
+    conditional_frequencies = ex_fuzzy.utils.construct_conditional_frequencies(sample, time_labels, [vl1, vl2])
+
+    assert conditional_frequencies[0, 0] > conditional_frequencies[0, 1]
+    assert conditional_frequencies[1, 0] < conditional_frequencies[1, 1]
+
+
+def test_temporal_assemble():
+    sample_size = 1000
+    sample = np.random.random_sample((sample_size, 5))
+    y = np.random.randint(0, 2, sample_size)
+
+    temp_moments1 = np.random.randint(0, 2, sample_size)
+    temp_moments2 = 1 - temp_moments1
+    temp_moments = [temp_moments1, temp_moments2]
+
+    [X_train, X_test, y_train, y_test], [train_temporal_boolean_markers, test_temporal_boolean_markers] = ex_fuzzy.utils.temporal_assemble(sample, y, temp_moments)
+
+    t1test = [y_test[jx] for jx, aux in enumerate(test_temporal_boolean_markers[0]) if aux]
+    t2test = [y_test[jx] for jx, aux in enumerate(test_temporal_boolean_markers[1]) if aux]
+
+    assert len(t1test) == len(t2test)
+
+    
+
+
+if __name__ == '__main__':
+    test_quartiles()
+    test_quantiles()
+    test_3_partitions()
+    test_construct_partitions_t1()
+    test_construct_partitions_t2()
+    test_construct_partitions_gt2()
+    test_temporal_conditional()
+    test_temporal_assemble()
     print('All tests passed.')
```

