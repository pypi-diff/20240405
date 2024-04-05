# Comparing `tmp/causal-playground-0.1.0.tar.gz` & `tmp/causal-playground-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal-playground-0.1.0.tar", last modified: Thu Feb 29 15:45:14 2024, max compression
+gzip compressed data, was "causal-playground-0.1.1.tar", last modified: Fri Apr  5 07:50:41 2024, max compression
```

## Comparing `causal-playground-0.1.0.tar` & `causal-playground-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:14.867174 causal-playground-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:14.863174 causal-playground-0.1.0/CausalPlayground/
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-02-29 15:45:06.000000 causal-playground-0.1.0/CausalPlayground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-02-29 15:45:06.000000 causal-playground-0.1.0/CausalPlayground/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-02-29 15:45:06.000000 causal-playground-0.1.0/CausalPlayground/scm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-02-29 15:45:06.000000 causal-playground-0.1.0/CausalPlayground/scm_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-29 15:45:06.000000 causal-playground-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-29 15:45:14.867174 causal-playground-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-29 15:45:06.000000 causal-playground-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:14.867174 causal-playground-0.1.0/causal_playground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-29 15:45:14.000000 causal-playground-0.1.0/causal_playground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-29 15:45:14.000000 causal-playground-0.1.0/causal_playground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 15:45:14.000000 causal-playground-0.1.0/causal_playground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-29 15:45:14.000000 causal-playground-0.1.0/causal_playground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 15:45:14.000000 causal-playground-0.1.0/causal_playground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-29 15:45:06.000000 causal-playground-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 15:45:14.867174 causal-playground-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:14.863174 causal-playground-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-29 15:45:06.000000 causal-playground-0.1.0/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-02-29 15:45:06.000000 causal-playground-0.1.0/tests/test_graph_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-02-29 15:45:06.000000 causal-playground-0.1.0/tests/test_scm_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/CausalPlayground/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/scm_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 07:50:37.000000 causal-playground-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-05 07:50:41.582765 causal-playground-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-05 07:50:37.000000 causal-playground-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/causal_playground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 07:50:37.000000 causal-playground-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:50:41.582765 causal-playground-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_graph_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_scm_gen.py
```

### Comparing `causal-playground-0.1.0/CausalPlayground/generators.py` & `causal-playground-0.1.1/CausalPlayground/generators.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.0/CausalPlayground/scm.py` & `causal-playground-0.1.1/CausalPlayground/scm.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 This file defines all functionality for Structural Causal Models.
 """
 
 from typing import Tuple, Any, Callable, Dict, List
 import networkx as nx
 import matplotlib.pyplot as plt
 import random
+import dill
 
 
 class StructuralCausalModel:
     """
     Class defining a Structural Causal Model. We define an SCM as a tuple
     .. math::
         \mathcal{M} = (\mathcal{X}, \mathcal{F}, \mathcal{U}, \mathcal{P})
     where :math:`\mathcal{X}` is the set of endogenous variables, :math:`\mathcal{F}` is the set of assignment
     functions, :math:`\mathcal{U}` the set of exogenous variables, and :math:`\mathcal{P}` is the set of probability
     distributions associated with the exogenous variables.
     """
 
     endogenous_vars: Dict[str, Any]
-    """Dictionary storing the value of each endogenoous variable."""
+    """Dictionary storing the value of each endogenous variable."""
     functions: Dict[str, Tuple[Callable, dict]]
     """Functional assignments of the endogenous variables. for each endogenous variables, the functional assignments are
     stored as well as a dictionary mapping the parameters of the callable (key) to the name of the causes (values)."""
     exogenous_vars: Dict[str, Any]
     """Dictionary storing the values of the exogenous variables."""
     exogenous_distributions: Dict[str, Tuple[Callable, dict]]
     """Dictionary storing the distribution for each exogenous variable. The values of the dict contain the callable 
@@ -193,7 +194,43 @@
         graph = self.create_graph()
         values = dict(self.endogenous_vars), dict(self.exogenous_vars)
         values = dict(values[0], **values[1])
         nx.draw(graph, arrowsize=20, with_labels=True, node_size=3000, font_size=10,
                 labels={key: str(key) + ':\n' + str(values[key]) for key in values}, pos=nx.planar_layout(graph))
         plt.show()
 
+    def save(self, filepath: str, verbose: int = 0) -> None:
+        """
+        Save the structural causal model to a file
+
+        :param filepath: path to file for saving the SCM
+        :param verbose: verbosity level, 0=silent, 1=print to console
+        """
+        try:
+            with open(filepath, 'wb') as file:
+                dill.dump(self, file)
+            message = f"SCM successfully saved to {filepath}"
+        except IOError as e:
+            message = f"Error saving object to file: {str(e)}"
+        if verbose == 1:
+            print(message)
+
+    @staticmethod
+    def load(filepath: str, verbose: int = 0) -> "StructuralCausalModel":
+        """
+        Load an object from a file using dill deserialization.
+
+        :param filepath: The path and filename of the file to load the object from.
+        :param verbose: verbosity level, 0=silent, 1=print to console
+
+        :return: the loaded SCM
+        """
+        try:
+            with open(filepath, 'rb') as file:
+                obj = dill.load(file)
+            return obj
+        except IOError as e:
+            if verbose == 1:
+                print(f"Error loading object from file: {str(e)}")
+        except dill.UnpicklingError as e:
+            if verbose == 1:
+                print(f"Error deserializing object: {str(e)}")
```

### Comparing `causal-playground-0.1.0/CausalPlayground/scm_environment.py` & `causal-playground-0.1.1/CausalPlayground/scm_environment.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.0/LICENSE` & `causal-playground-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.0/PKG-INFO` & `causal-playground-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-playground
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interactively generating causal data from structural causal models.
 Author-email: Andreas Sauter <a.sauter@vu.nl>
 License: MIT License
 Project-URL: Homepage, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Documentation, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Repository, https://github.com/sa-and/CausalPlayground
 Keywords: causality,reinforcement learning,structural causal model,data generation,RL,SCM
@@ -25,27 +25,27 @@
 
 # Overview
 The [CausalPlayground](https://github.com/sa-and/CausalPlayground) library serves as a tool for causality research, focusing on the interactive exploration of structural 
 causal models (SCMs). It provides extensive functionality for creating, manipulating and sampling SCMs, seamlessly 
 integrating them with the Gymnasium framework. Users have complete control over SCMs, enabling precise manipulation and
 interaction with causal mechanisms. Additionally, CausalPlayground offers a range of useful helper functions for generating 
 diverse instances of SCMs and DAGs, facilitating quantitative experimentation and evaluation. Notably, the library is 
-designed for easy integration with reinforcement learning methods, enhancing its utility in active inference and 
+optimized for (but not limited to) easy integration with reinforcement learning methods, enhancing its utility in active inference and 
 learning settings. Find the complete API documentation and a quickstart guide [here](https://sa-and.github.io/CausalPlayground/).
 
-# Installation guide (TODO)
+# Installation guide
 In your python environment `pip install causal-playground`.
 
 # Contributing
 Contributions are highly welcomed and encouraged! To contribute to the project, please follow the following steps:
 
 - Fork the project.
 - Create a local branch `my-awesome-new-feature`.
 - Implement your new feature in the newly created branch.
 - Make sure you provide sufficient documentation and test-cases.
 - Open a pull request.
 
 Alternatively, you can open a well-described issue.
 
-# Citing this work (TODO)
+# Citing this work
 If you are using this library, please consider citing us:
 TODO
```

### Comparing `causal-playground-0.1.0/README.md` & `causal-playground-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Overview
 The [CausalPlayground](https://github.com/sa-and/CausalPlayground) library serves as a tool for causality research, focusing on the interactive exploration of structural 
 causal models (SCMs). It provides extensive functionality for creating, manipulating and sampling SCMs, seamlessly 
 integrating them with the Gymnasium framework. Users have complete control over SCMs, enabling precise manipulation and
 interaction with causal mechanisms. Additionally, CausalPlayground offers a range of useful helper functions for generating 
 diverse instances of SCMs and DAGs, facilitating quantitative experimentation and evaluation. Notably, the library is 
-designed for easy integration with reinforcement learning methods, enhancing its utility in active inference and 
+optimized for (but not limited to) easy integration with reinforcement learning methods, enhancing its utility in active inference and 
 learning settings. Find the complete API documentation and a quickstart guide [here](https://sa-and.github.io/CausalPlayground/).
 
-# Installation guide (TODO)
+# Installation guide
 In your python environment `pip install causal-playground`.
 
 # Contributing
 Contributions are highly welcomed and encouraged! To contribute to the project, please follow the following steps:
 
 - Fork the project.
 - Create a local branch `my-awesome-new-feature`.
 - Implement your new feature in the newly created branch.
 - Make sure you provide sufficient documentation and test-cases.
 - Open a pull request.
 
 Alternatively, you can open a well-described issue.
 
-# Citing this work (TODO)
+# Citing this work
 If you are using this library, please consider citing us:
 TODO
```

### Comparing `causal-playground-0.1.0/causal_playground.egg-info/PKG-INFO` & `causal-playground-0.1.1/causal_playground.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-playground
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interactively generating causal data from structural causal models.
 Author-email: Andreas Sauter <a.sauter@vu.nl>
 License: MIT License
 Project-URL: Homepage, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Documentation, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Repository, https://github.com/sa-and/CausalPlayground
 Keywords: causality,reinforcement learning,structural causal model,data generation,RL,SCM
@@ -25,27 +25,27 @@
 
 # Overview
 The [CausalPlayground](https://github.com/sa-and/CausalPlayground) library serves as a tool for causality research, focusing on the interactive exploration of structural 
 causal models (SCMs). It provides extensive functionality for creating, manipulating and sampling SCMs, seamlessly 
 integrating them with the Gymnasium framework. Users have complete control over SCMs, enabling precise manipulation and
 interaction with causal mechanisms. Additionally, CausalPlayground offers a range of useful helper functions for generating 
 diverse instances of SCMs and DAGs, facilitating quantitative experimentation and evaluation. Notably, the library is 
-designed for easy integration with reinforcement learning methods, enhancing its utility in active inference and 
+optimized for (but not limited to) easy integration with reinforcement learning methods, enhancing its utility in active inference and 
 learning settings. Find the complete API documentation and a quickstart guide [here](https://sa-and.github.io/CausalPlayground/).
 
-# Installation guide (TODO)
+# Installation guide
 In your python environment `pip install causal-playground`.
 
 # Contributing
 Contributions are highly welcomed and encouraged! To contribute to the project, please follow the following steps:
 
 - Fork the project.
 - Create a local branch `my-awesome-new-feature`.
 - Implement your new feature in the newly created branch.
 - Make sure you provide sufficient documentation and test-cases.
 - Open a pull request.
 
 Alternatively, you can open a well-described issue.
 
-# Citing this work (TODO)
+# Citing this work
 If you are using this library, please consider citing us:
 TODO
```

### Comparing `causal-playground-0.1.0/pyproject.toml` & `causal-playground-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causal-playground"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">= 3.10"
 authors = [{name = "Andreas Sauter", email = "a.sauter@vu.nl"}]
 readme = "README.md"
 description = "Interactively generating causal data from structural causal models."
 license = {text = "MIT License"}
 keywords = ["causality", "reinforcement learning", "structural causal model", "data generation", "RL", "SCM"]
 dependencies = [
```

### Comparing `causal-playground-0.1.0/tests/test_envs.py` & `causal-playground-0.1.1/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.0/tests/test_graph_gen.py` & `causal-playground-0.1.1/tests/test_graph_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,35 +59,31 @@
         
         for i in range(49):
             self.assertTrue(nx.is_isomorphic(set_generator1.graphs[i], set_generator3.graphs[i]))
             self.assertFalse(nx.is_isomorphic(set_generator1.graphs[i], set_generator2.graphs[i]))  # holds just for
             # these specific seeds and 50 samples
 
     def test_graphset_save_load(self):
+        if os.path.exists("./delme.pkl"):
+            os.remove("./delme.pkl")
         graph_set = CausalGraphSetGenerator(n_endo=5, n_exo=10, allow_exo_confounders=False)
         graph_set.generate(20)
-        graph_set.save('delme.pkl')
-        graph_set.load('delme.pkl')
+        graph_set.save('./delme.pkl')
+        graph_set.load('./delme.pkl')
         self.assertTrue(len(graph_set.graphs), 20)
-        os.remove('delme.pkl')
+        np.array([1, 2]).dump('delme.pkl')
+        with self.assertRaises(TypeError):
+            graph_set.load('delme.pkl')
+        os.remove('./delme.pkl')
         
     def test_unique_graph_set(self):
         graph_set = CausalGraphSetGenerator(n_endo=4, n_exo=0, allow_exo_confounders=False)
         graph_set.generate(300)
         edges = [list(g.edges()) for g in graph_set.graphs]
         self.assertTrue(all([len(e) == len(set(e)) for e in edges]))
         graph_set.generate(300, method='ER', p=0.3)
         edges = [list(g.edges()) for g in graph_set.graphs]
         self.assertTrue(all([len(e) == len(set(e)) for e in edges]))
 
-    def test_save_load_graph_set(self):
-        graph_set = CausalGraphSetGenerator(n_endo=4, n_exo=0, allow_exo_confounders=False)
-        graph_set.generate(300)
-        graph_set.save('delme.pkl')
-        graph_set.load('delme.pkl')
-        np.array([1, 2]).dump('delme.pkl')
-        with self.assertRaises(TypeError):
-            graph_set.load('delme.pkl')
-        
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `causal-playground-0.1.0/tests/test_scm_gen.py` & `causal-playground-0.1.1/tests/test_scm_gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import CausalPlayground
 from CausalPlayground import StructuralCausalModel
 from CausalPlayground import SCMGenerator
 import unittest
 from functions import *
 import random
+import os
 
 
 class TestSCM(unittest.TestCase):
     def __init__(self, *args,  **kwargs):
         super(TestSCM, self).__init__(*args, **kwargs)
         self.scm = SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"], n_endo=20, n_exo=0)[0]
         self.test_scm = StructuralCausalModel()
@@ -68,14 +69,31 @@
     def test_intervention_targets(self):
         """Are the correct intervention targets returned"""
         self.scm.do_interventions([("X0", (lambda: 5, {})), ("X1", (lambda x0: x0 + 1, {'x0': 'X0'}))])
         self.assertTrue(self.scm.get_intervention_targets() == ["X0", "X1"])
         self.scm.undo_interventions()
         self.assertTrue(self.scm.get_intervention_targets() == [])
 
+    def test_save_and_load(self):
+        if os.path.exists("./delme.pkl"):
+            os.remove("./delme.pkl")
+        # Test saving the object to a file
+        self.test_scm.save("./delme.pkl")
+        self.assertTrue(os.path.exists("./delme.pkl"))
+
+        # Test loading the object from the file
+        loaded_scm = StructuralCausalModel.load("./delme.pkl")
+        self.assertIsInstance(loaded_scm, StructuralCausalModel)
+        self.assertEqual(list(loaded_scm.endogenous_vars.keys()), ['A', 'EFFECT'])
+        self.assertEqual(list(loaded_scm.exogenous_vars.keys()), ['U'])
+        self.assertEqual(loaded_scm.create_graph().edges, self.test_scm.create_graph().edges)
+
+        if os.path.exists("./delme.pkl"):
+            os.remove("./delme.pkl")
+
 
 class TestRandNN(unittest.TestCase):
     def __init__(self, *args,  **kwargs):
         super(TestRandNN, self).__init__(*args, **kwargs)
         self.scm1 = SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"], n_endo=10, n_exo=0)[0]
         # self.scm2 = SCMGenerator(seed=42).create_random(possible_functions=["NN"], n_endo=6, n_exo=8,
         #                                                 exo_distribution=random.random, exo_distribution_kwargs={})[0]
```

