# Comparing `tmp/qarray-1.0.3.tar.gz` & `tmp/qarray-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-1.0.3.tar` & `qarray-1.0.6.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0      850 2024-04-05 08:17:17.184964 qarray-1.0.3/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0     1317 2024-04-05 08:17:17.188964 qarray-1.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3079 2024-04-05 08:17:17.188964 qarray-1.0.3/.gitignore
--rw-r--r--   0        0        0     1087 2024-04-05 08:17:17.188964 qarray-1.0.3/LICENSE
--rw-r--r--   0        0        0     3038 2024-04-05 08:17:17.188964 qarray-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-05 08:17:17.188964 qarray-1.0.3/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-05 08:17:17.188964 qarray-1.0.3/docs/installation.rst
--rw-r--r--   0        0        0     1652 2024-04-05 08:17:17.188964 qarray-1.0.3/docs/simulating_double_dot.rst
--rw-r--r--   0        0        0     2507 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/charge_sensing.py
--rw-r--r--   0        0        0     2632 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/double_dot.py
--rw-r--r--   0        0        0      589 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/gate_voltage_composer_tricks.py
--rw-r--r--   0        0        0     1933 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/gradient.py
--rw-r--r--   0        0        0     2747 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/linear_quadruple_dot.py
--rw-r--r--   0        0        0     2520 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/linear_triple_dot.py
--rw-r--r--   0        0        0      694 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/paper_examples.py
--rw-r--r--   0        0        0     2650 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/quadruple_dot_all_gates.py
--rw-r--r--   0        0        0     3229 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/simulating_closed_five_dot_array_.py
--rw-r--r--   0        0        0     1684 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/simulating_open_four_dot_array.py
--rw-r--r--   0        0        0     2888 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/triple_dot.py
--rw-r--r--   0        0        0    27960 2024-04-05 08:17:17.188964 qarray-1.0.3/misc/recreations.jpg
--rw-r--r--   0        0        0    17300 2024-04-05 08:17:17.188964 qarray-1.0.3/misc/structure.jpg
--rw-r--r--   0        0        0     2875 2024-04-05 08:17:17.188964 qarray-1.0.3/pypi_README.md
--rw-r--r--   0        0        0      674 2024-04-05 08:17:17.188964 qarray-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      649 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/__init__.py
--rw-r--r--   0        0        0      108 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/__init__.py
--rw-r--r--   0        0        0       80 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      640 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2649 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/closed.py
--rw-r--r--   0        0        0     2429 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/open.py
--rw-r--r--   0        0        0      114 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/__init__.py
--rw-r--r--   0        0        0       83 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      634 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2372 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/closed.py
--rw-r--r--   0        0        0     2094 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/open.py
--rw-r--r--   0        0        0     6570 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/BaseDataClass.py
--rw-r--r--   0        0        0     5629 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/ChargeSensedDotArray.py
--rw-r--r--   0        0        0     7092 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/DotArray.py
--rw-r--r--   0        0        0    10321 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/GateVoltageComposer.py
--rw-r--r--   0        0        0      139 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/__init__.py
--rw-r--r--   0        0        0     8001 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/_helper_functions.py
--rw-r--r--   0        0        0     5334 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/functions.py
--rw-r--r--   0        0        0       84 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/__init__.py
--rw-r--r--   0        0        0       68 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      726 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     6227 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/closed.py
--rw-r--r--   0        0        0      275 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/helper_functions.py
--rw-r--r--   0        0        0     4819 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/jax_core/open.py
--rw-r--r--   0        0        0       80 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/__init__.py
--rw-r--r--   0        0        0      132 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
--rw-r--r--   0        0        0      947 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     7025 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/core_python.py
--rw-r--r--   0        0        0      258 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/qarray_types/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/qarray_types/typing_classes.py
--rw-r--r--   0        0        0      109 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/rust_core/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/rust_core/core_rust.py
--rw-r--r--   0        0        0      133 2024-04-05 08:17:17.192964 qarray-1.0.3/requirements.txt
--rw-r--r--   0        0        0      338 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/GLOBAL_OPTIONS.py
--rw-r--r--   0        0        0        0 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3357 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/helper_functions.py
--rw-r--r--   0        0        0      939 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/pydantic_validation_tests.py
--rw-r--r--   0        0        0     6190 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_against_brute_force.py
--rw-r--r--   0        0        0    17563 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_charge_combinations.py
--rw-r--r--   0        0        0     6110 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_double_dot.py
--rw-r--r--   0        0        0     3978 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_gate_voltage_composer.py
--rw-r--r--   0        0        0     5939 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_quadruple_dot.py
--rw-r--r--   0        0        0     4579 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_solver.py
--rw-r--r--   0        0        0     9900 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_threshold.py
--rw-r--r--   0        0        0     5938 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_triple_dot.py
--rw-r--r--   0        0        0     1724 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_user_interaction.py
--rw-r--r--   0        0        0      109 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/tests.py
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 qarray-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      850 2024-04-05 08:57:44.286948 qarray-1.0.6/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0     1317 2024-04-05 08:57:44.286948 qarray-1.0.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3079 2024-04-05 08:57:44.286948 qarray-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-05 08:57:44.286948 qarray-1.0.6/LICENSE
+-rw-r--r--   0        0        0     4468 2024-04-05 08:57:44.286948 qarray-1.0.6/README.md
+-rw-r--r--   0        0        0     1024 2024-04-05 08:57:44.290948 qarray-1.0.6/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-05 08:57:44.290948 qarray-1.0.6/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/charge_sensing.py
+-rw-r--r--   0        0        0     2632 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/paper_examples.py
+-rw-r--r--   0        0        0     2650 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/simulating_closed_five_dot_array_.py
+-rw-r--r--   0        0        0     1684 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/simulating_open_four_dot_array.py
+-rw-r--r--   0        0        0     2888 2024-04-05 08:57:44.290948 qarray-1.0.6/examples/triple_dot.py
+-rw-r--r--   0        0        0   520772 2024-04-05 08:57:44.290948 qarray-1.0.6/misc/recreations.jpg
+-rw-r--r--   0        0        0   181957 2024-04-05 08:57:44.294947 qarray-1.0.6/misc/structure.jpg
+-rw-r--r--   0        0        0     4469 2024-04-05 08:57:44.294947 qarray-1.0.6/pypi_README.md
+-rw-r--r--   0        0        0      674 2024-04-05 08:57:44.294947 qarray-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      644 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     8001 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-05 08:57:44.294947 qarray-1.0.6/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      133 2024-04-05 08:57:44.294947 qarray-1.0.6/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-05 08:57:44.294947 qarray-1.0.6/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:57:44.294947 qarray-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6190 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6110 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5939 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1724 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-05 08:57:44.298947 qarray-1.0.6/tests/tests.py
+-rw-r--r--   0        0        0     5171 1970-01-01 00:00:00.000000 qarray-1.0.6/PKG-INFO
```

### Comparing `qarray-1.0.3/.github/workflows/pypi.yaml` & `qarray-1.0.6/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/.github/workflows/test.yaml` & `qarray-1.0.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/.gitignore` & `qarray-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/LICENSE` & `qarray-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/docs/installation.rst` & `qarray-1.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/docs/simulating_double_dot.rst` & `qarray-1.0.6/docs/simulating_double_dot.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/charge_sensing.py` & `qarray-1.0.6/examples/charge_sensing.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/double_dot.py` & `qarray-1.0.6/examples/double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/gate_voltage_composer_tricks.py` & `qarray-1.0.6/examples/gate_voltage_composer_tricks.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/gradient.py` & `qarray-1.0.6/examples/gradient.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/linear_quadruple_dot.py` & `qarray-1.0.6/examples/linear_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/linear_triple_dot.py` & `qarray-1.0.6/examples/linear_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/paper_examples.py` & `qarray-1.0.6/examples/paper_examples.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/quadruple_dot_all_gates.py` & `qarray-1.0.6/examples/quadruple_dot_all_gates.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/simulating_closed_five_dot_array_.py` & `qarray-1.0.6/examples/simulating_closed_five_dot_array_.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/simulating_open_four_dot_array.py` & `qarray-1.0.6/examples/simulating_open_four_dot_array.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/examples/triple_dot.py` & `qarray-1.0.6/examples/triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/pyproject.toml` & `qarray-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/__init__.py` & `qarray-1.0.6/qarray/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and just in time compiled JAX
+Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and JAX XLA acceleration
 to compute charge stability diagrams of large both open and closed arrays in milliseconds.
 """
-__version__ = "1.0.3"
+__version__ = "1.0.6"
 
 from .classes import (DotArray, GateVoltageComposer, ChargeSensedDotArray)
 from .functions import (optimal_Vg, compute_threshold, convert_to_maxwell, dot_occupation_changes, lorentzian,
                         dot_gradient)
 from .python_core import (ground_state_open_python, ground_state_closed_python)
 from .rust_core import (ground_state_open_rust, ground_state_closed_rust, closed_charge_configurations_rust)
```

### Comparing `qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.6/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/brute_force_jax/closed.py` & `qarray-1.0.6/qarray/brute_force_jax/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/brute_force_jax/open.py` & `qarray-1.0.6/qarray/brute_force_jax/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.6/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/brute_force_python/closed.py` & `qarray-1.0.6/qarray/brute_force_python/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/brute_force_python/open.py` & `qarray-1.0.6/qarray/brute_force_python/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/classes/BaseDataClass.py` & `qarray-1.0.6/qarray/classes/BaseDataClass.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/classes/ChargeSensedDotArray.py` & `qarray-1.0.6/qarray/classes/ChargeSensedDotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/classes/DotArray.py` & `qarray-1.0.6/qarray/classes/DotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/classes/GateVoltageComposer.py` & `qarray-1.0.6/qarray/classes/GateVoltageComposer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/classes/_helper_functions.py` & `qarray-1.0.6/qarray/classes/_helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/functions.py` & `qarray-1.0.6/qarray/functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.6/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/jax_core/closed.py` & `qarray-1.0.6/qarray/jax_core/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/jax_core/open.py` & `qarray-1.0.6/qarray/jax_core/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py` & `qarray-1.0.6/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/python_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.6/qarray/python_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/python_core/core_python.py` & `qarray-1.0.6/qarray/python_core/core_python.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/qarray_types/typing_classes.py` & `qarray-1.0.6/qarray/qarray_types/typing_classes.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/qarray/rust_core/core_rust.py` & `qarray-1.0.6/qarray/rust_core/core_rust.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/helper_functions.py` & `qarray-1.0.6/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/pydantic_validation_tests.py` & `qarray-1.0.6/tests/pydantic_validation_tests.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_against_brute_force.py` & `qarray-1.0.6/tests/test_against_brute_force.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_charge_combinations.py` & `qarray-1.0.6/tests/test_charge_combinations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_double_dot.py` & `qarray-1.0.6/tests/test_double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_gate_voltage_composer.py` & `qarray-1.0.6/tests/test_gate_voltage_composer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_quadruple_dot.py` & `qarray-1.0.6/tests/test_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_solver.py` & `qarray-1.0.6/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_threshold.py` & `qarray-1.0.6/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_triple_dot.py` & `qarray-1.0.6/tests/test_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/tests/test_user_interaction.py` & `qarray-1.0.6/tests/test_user_interaction.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.3/PKG-INFO` & `qarray-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1
-Name: qarray
-Version: 1.0.3
-Summary: Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and just in time compiled JAX
-Author-email: Barnaby van Straaten <barnaby.vanstraaten@kellogg.ox.ac.uk>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: qarray-rust-core==1.2.0
-Requires-Dist: osqp==0.6.3
-Requires-Dist: numpy>=1.26
-Requires-Dist: pydantic>=2.3
-Requires-Dist: scipy>=1.11
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: loguru>=0.5
-Requires-Dist: jax>=0.2
-Requires-Dist: jaxopt>=0.4
-Requires-Dist: tqdm>=4.62
-Project-URL: Home, https://github.com/b-vanstraaten/qarray
-
-# Qarray
+# QArray
 
 ![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/qarray)
 
-**QArray** is a high-performance Python package that leverages the power of Rust and JAX to provide a fully parallelised
-and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
-and is designed to be easy to use and integrate into your existing workflow.
+<img src="https://github.com/b-vanstraaten/qarray/blob/main/misc/structure.jpg" alt="structure" width="600">
+
+**QArray** harnesses the speed of the systems programming language Rust or the compute power of GPUs using JAX XLA
+to deliver constant capacitance model charge stability diagrams in seconds or millisecond. It couples
+highly optimised and parrelised code with two new algorithms to compute the ground state charge configuration. These
+algorithms scale better than the traditional brute-force approach and do not require the user to maxmimum specify
+the maxmimum number of charge carrier a priori.
+
+QArray runs on both CPUs and GPUs, and is designed to be easy to use and integrate into your existing workflow.
+It was developed on MacOS running on Apple Silicon and is continuously tested, Linux and Windows.
+
+Finally, QArray captures physical effects such as measuring the charge stability diagram
+of with a SET and thermal broadening of charge transitions. The combination of these effects
+permits the simulation of charge stability diagrams which are visually similar to those measured experimentally.
+The plots on the right below are measured experimentally, and the plots on the left are simulated using QArray.
+
+<img src="https://github.com/b-vanstraaten/qarray/blob/main/misc/recreations.jpg" alt="structure" width="400">
 
-Harnesses the speed of Rust or the compute power of GPUs using JAX to deliver charge stability diagrams in seconds or
-millisecond
+Figure (a) shows the charge stability diagram of an open quadruple quantum dot array. (a) is a recreation
+of the charge stability diagram recreated with permission from [1] while (b) is a simulated using QArray.
 
+Figure (c) shows the charge stability diagram of closed five dot quantum recreated with permission from [2] and (d) is
+simulated using QArray.
+
+[1] [Full control of quadruple quantum dot circuit charge states in the single electron regime](https://pubs.aip.org/aip/apl/article/104/18/183111/24127/Full-control-of-quadruple-quantum-dot-circuit)
+
+[2] [Coherent control of individual electron spins in a two-dimensional quantum dot array](https://www.nature.com/articles/s41565-020-00816-w)
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
 ```
@@ -74,19 +74,17 @@
 # run the simulation with the quantum dot array open such that the number of charge carriers is not fixed
 n_open = model.ground_state_open(vg)  # n_open is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 # run the simulation with the quantum dot array closed such that the number of charge carriers is fixed to 2
 n_closed = model.ground_state_closed(vg, n_charge_carriers=2)  # n_closed is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 ```
-
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
 1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
 2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
 3. [Linear Quadruple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_quadruple_dot.py)
 4. [Charge sensed double quantum dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/charge_sensing.py)
 
-
```

