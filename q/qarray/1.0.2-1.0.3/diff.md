# Comparing `tmp/qarray-1.0.2.tar.gz` & `tmp/qarray-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-1.0.2.tar` & `qarray-1.0.3.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0      850 2024-04-05 07:47:47.854266 qarray-1.0.2/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0     1317 2024-04-05 07:47:47.854266 qarray-1.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3079 2024-04-05 07:47:47.854266 qarray-1.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2024-04-05 07:47:47.854266 qarray-1.0.2/LICENSE
--rw-r--r--   0        0        0     3044 2024-04-05 07:47:47.854266 qarray-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-05 07:47:47.854266 qarray-1.0.2/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-05 07:47:47.854266 qarray-1.0.2/docs/installation.rst
--rw-r--r--   0        0        0     1652 2024-04-05 07:47:47.854266 qarray-1.0.2/docs/simulating_double_dot.rst
--rw-r--r--   0        0        0     2507 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/charge_sensing.py
--rw-r--r--   0        0        0     2632 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/double_dot.py
--rw-r--r--   0        0        0      589 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/gate_voltage_composer_tricks.py
--rw-r--r--   0        0        0     1933 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/gradient.py
--rw-r--r--   0        0        0     2747 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/linear_quadruple_dot.py
--rw-r--r--   0        0        0     2520 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/linear_triple_dot.py
--rw-r--r--   0        0        0      694 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/paper_examples.py
--rw-r--r--   0        0        0     2650 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/quadruple_dot_all_gates.py
--rw-r--r--   0        0        0     3229 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/simulating_closed_five_dot_array_.py
--rw-r--r--   0        0        0     1684 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/simulating_open_four_dot_array.py
--rw-r--r--   0        0        0     2888 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/triple_dot.py
--rw-r--r--   0        0        0    27960 2024-04-05 07:47:47.854266 qarray-1.0.2/misc/recreations.jpg
--rw-r--r--   0        0        0    17300 2024-04-05 07:47:47.854266 qarray-1.0.2/misc/structure.jpg
--rw-r--r--   0        0        0      669 2024-04-05 07:47:47.858266 qarray-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      506 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/__init__.py
--rw-r--r--   0        0        0      108 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/__init__.py
--rw-r--r--   0        0        0       80 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      640 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2649 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/closed.py
--rw-r--r--   0        0        0     2429 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/open.py
--rw-r--r--   0        0        0      114 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/__init__.py
--rw-r--r--   0        0        0       83 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      634 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2372 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/closed.py
--rw-r--r--   0        0        0     2094 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/open.py
--rw-r--r--   0        0        0     6570 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/BaseDataClass.py
--rw-r--r--   0        0        0     5629 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/ChargeSensedDotArray.py
--rw-r--r--   0        0        0     7092 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/DotArray.py
--rw-r--r--   0        0        0    10321 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/GateVoltageComposer.py
--rw-r--r--   0        0        0      139 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/__init__.py
--rw-r--r--   0        0        0     8001 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/_helper_functions.py
--rw-r--r--   0        0        0     5334 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/functions.py
--rw-r--r--   0        0        0       84 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/__init__.py
--rw-r--r--   0        0        0       68 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      726 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     6227 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/closed.py
--rw-r--r--   0        0        0      275 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/helper_functions.py
--rw-r--r--   0        0        0     4819 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/open.py
--rw-r--r--   0        0        0       80 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/__init__.py
--rw-r--r--   0        0        0      132 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
--rw-r--r--   0        0        0      947 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     7025 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/core_python.py
--rw-r--r--   0        0        0      258 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/qarray_types/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/qarray_types/typing_classes.py
--rw-r--r--   0        0        0      109 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/rust_core/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/rust_core/core_rust.py
--rw-r--r--   0        0        0      133 2024-04-05 07:47:47.858266 qarray-1.0.2/requirements.txt
--rw-r--r--   0        0        0      338 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/GLOBAL_OPTIONS.py
--rw-r--r--   0        0        0        0 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3357 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/helper_functions.py
--rw-r--r--   0        0        0      939 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/pydantic_validation_tests.py
--rw-r--r--   0        0        0     6190 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_against_brute_force.py
--rw-r--r--   0        0        0    17563 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_charge_combinations.py
--rw-r--r--   0        0        0     6110 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_double_dot.py
--rw-r--r--   0        0        0     3978 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_gate_voltage_composer.py
--rw-r--r--   0        0        0     5939 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_quadruple_dot.py
--rw-r--r--   0        0        0     4579 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_solver.py
--rw-r--r--   0        0        0     9900 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_threshold.py
--rw-r--r--   0        0        0     5938 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_triple_dot.py
--rw-r--r--   0        0        0     1724 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_user_interaction.py
--rw-r--r--   0        0        0      109 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/tests.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 qarray-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      850 2024-04-05 08:17:17.184964 qarray-1.0.3/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0     1317 2024-04-05 08:17:17.188964 qarray-1.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3079 2024-04-05 08:17:17.188964 qarray-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-05 08:17:17.188964 qarray-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3038 2024-04-05 08:17:17.188964 qarray-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 08:17:17.188964 qarray-1.0.3/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-05 08:17:17.188964 qarray-1.0.3/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-05 08:17:17.188964 qarray-1.0.3/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/charge_sensing.py
+-rw-r--r--   0        0        0     2632 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/paper_examples.py
+-rw-r--r--   0        0        0     2650 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/simulating_closed_five_dot_array_.py
+-rw-r--r--   0        0        0     1684 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/simulating_open_four_dot_array.py
+-rw-r--r--   0        0        0     2888 2024-04-05 08:17:17.188964 qarray-1.0.3/examples/triple_dot.py
+-rw-r--r--   0        0        0    27960 2024-04-05 08:17:17.188964 qarray-1.0.3/misc/recreations.jpg
+-rw-r--r--   0        0        0    17300 2024-04-05 08:17:17.188964 qarray-1.0.3/misc/structure.jpg
+-rw-r--r--   0        0        0     2875 2024-04-05 08:17:17.188964 qarray-1.0.3/pypi_README.md
+-rw-r--r--   0        0        0      674 2024-04-05 08:17:17.188964 qarray-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      649 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     8001 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-05 08:17:17.188964 qarray-1.0.3/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-05 08:17:17.192964 qarray-1.0.3/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      133 2024-04-05 08:17:17.192964 qarray-1.0.3/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6190 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6110 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5939 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1724 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-05 08:17:17.192964 qarray-1.0.3/tests/tests.py
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 qarray-1.0.3/PKG-INFO
```

### Comparing `qarray-1.0.2/.github/workflows/pypi.yaml` & `qarray-1.0.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/.github/workflows/test.yaml` & `qarray-1.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/.gitignore` & `qarray-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/LICENSE` & `qarray-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/README.md` & `qarray-1.0.3/pypi_README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # Qarray
 
 ![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/qarray)
 
-![structure.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/structure)
-
-**Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
+**QArray** is a high-performance Python package that leverages the power of Rust and JAX to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
 Harnesses the speed of Rust or the compute power of GPUs using JAX to deliver charge stability diagrams in seconds or
 millisecond
 
-![recreations.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/recreations)
-
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
 ```
@@ -58,14 +54,15 @@
 # run the simulation with the quantum dot array open such that the number of charge carriers is not fixed
 n_open = model.ground_state_open(vg)  # n_open is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 # run the simulation with the quantum dot array closed such that the number of charge carriers is fixed to 2
 n_closed = model.ground_state_closed(vg, n_charge_carriers=2)  # n_closed is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 ```
+
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
 1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
 2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
```

### Comparing `qarray-1.0.2/docs/installation.rst` & `qarray-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/docs/simulating_double_dot.rst` & `qarray-1.0.3/docs/simulating_double_dot.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/charge_sensing.py` & `qarray-1.0.3/examples/charge_sensing.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/double_dot.py` & `qarray-1.0.3/examples/double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/gate_voltage_composer_tricks.py` & `qarray-1.0.3/examples/gate_voltage_composer_tricks.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/gradient.py` & `qarray-1.0.3/examples/gradient.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/linear_quadruple_dot.py` & `qarray-1.0.3/examples/linear_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/linear_triple_dot.py` & `qarray-1.0.3/examples/linear_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/paper_examples.py` & `qarray-1.0.3/examples/paper_examples.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/quadruple_dot_all_gates.py` & `qarray-1.0.3/examples/quadruple_dot_all_gates.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/simulating_closed_five_dot_array_.py` & `qarray-1.0.3/examples/simulating_closed_five_dot_array_.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/simulating_open_four_dot_array.py` & `qarray-1.0.3/examples/simulating_open_four_dot_array.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/examples/triple_dot.py` & `qarray-1.0.3/examples/triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/misc/recreations.jpg` & `qarray-1.0.3/misc/recreations.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/misc/structure.jpg` & `qarray-1.0.3/misc/structure.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/pyproject.toml` & `qarray-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "qarray"
 authors = [{ name = "Barnaby van Straaten", email = "barnaby.vanstraaten@kellogg.ox.ac.uk" }]
-readme = "README.md"
+readme = "pypi_README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">=3.10"
 dependencies = [
     'qarray-rust-core==1.2.0',
     'osqp==0.6.3',
```

### Comparing `qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.3/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/brute_force_jax/closed.py` & `qarray-1.0.3/qarray/brute_force_jax/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/brute_force_jax/open.py` & `qarray-1.0.3/qarray/brute_force_jax/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.3/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/brute_force_python/closed.py` & `qarray-1.0.3/qarray/brute_force_python/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/brute_force_python/open.py` & `qarray-1.0.3/qarray/brute_force_python/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/classes/BaseDataClass.py` & `qarray-1.0.3/qarray/classes/BaseDataClass.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/classes/ChargeSensedDotArray.py` & `qarray-1.0.3/qarray/classes/ChargeSensedDotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/classes/DotArray.py` & `qarray-1.0.3/qarray/classes/DotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/classes/GateVoltageComposer.py` & `qarray-1.0.3/qarray/classes/GateVoltageComposer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/classes/_helper_functions.py` & `qarray-1.0.3/qarray/classes/_helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/functions.py` & `qarray-1.0.3/qarray/functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.3/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/jax_core/closed.py` & `qarray-1.0.3/qarray/jax_core/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/jax_core/open.py` & `qarray-1.0.3/qarray/jax_core/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py` & `qarray-1.0.3/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/python_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.3/qarray/python_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/python_core/core_python.py` & `qarray-1.0.3/qarray/python_core/core_python.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/qarray_types/typing_classes.py` & `qarray-1.0.3/qarray/qarray_types/typing_classes.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/qarray/rust_core/core_rust.py` & `qarray-1.0.3/qarray/rust_core/core_rust.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/helper_functions.py` & `qarray-1.0.3/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/pydantic_validation_tests.py` & `qarray-1.0.3/tests/pydantic_validation_tests.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_against_brute_force.py` & `qarray-1.0.3/tests/test_against_brute_force.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_charge_combinations.py` & `qarray-1.0.3/tests/test_charge_combinations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_double_dot.py` & `qarray-1.0.3/tests/test_double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_gate_voltage_composer.py` & `qarray-1.0.3/tests/test_gate_voltage_composer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_quadruple_dot.py` & `qarray-1.0.3/tests/test_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_solver.py` & `qarray-1.0.3/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_threshold.py` & `qarray-1.0.3/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_triple_dot.py` & `qarray-1.0.3/tests/test_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/tests/test_user_interaction.py` & `qarray-1.0.3/tests/test_user_interaction.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.2/PKG-INFO` & `qarray-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qarray
-Version: 1.0.2
-Summary: Qarray is a Python package for simulating quantum dot arrays.
+Version: 1.0.3
+Summary: Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and just in time compiled JAX
 Author-email: Barnaby van Straaten <barnaby.vanstraaten@kellogg.ox.ac.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: qarray-rust-core==1.2.0
 Requires-Dist: osqp==0.6.3
 Requires-Dist: numpy>=1.26
@@ -19,25 +19,21 @@
 Project-URL: Home, https://github.com/b-vanstraaten/qarray
 
 # Qarray
 
 ![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/qarray)
 
-![structure.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/structure)
-
-**Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
+**QArray** is a high-performance Python package that leverages the power of Rust and JAX to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
 Harnesses the speed of Rust or the compute power of GPUs using JAX to deliver charge stability diagrams in seconds or
 millisecond
 
-![recreations.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/recreations)
-
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
 ```
@@ -78,14 +74,15 @@
 # run the simulation with the quantum dot array open such that the number of charge carriers is not fixed
 n_open = model.ground_state_open(vg)  # n_open is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 # run the simulation with the quantum dot array closed such that the number of charge carriers is fixed to 2
 n_closed = model.ground_state_closed(vg, n_charge_carriers=2)  # n_closed is a (100, 100, 2) array encoding the 
 # number of charge carriers in each dot for each gate voltage
 ```
+
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
 1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
 2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
```

