# Comparing `tmp/qarray-1.0.1.tar.gz` & `tmp/qarray-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-1.0.1.tar` & `qarray-1.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      850 2024-04-04 18:54:29.129871 qarray-1.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0     1317 2024-04-04 18:54:29.129871 qarray-1.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3079 2024-04-04 18:54:29.129871 qarray-1.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2024-04-04 18:54:29.129871 qarray-1.0.1/LICENSE
--rw-r--r--   0        0        0     2958 2024-04-04 18:54:29.129871 qarray-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-04 18:54:29.129871 qarray-1.0.1/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-04 18:54:29.129871 qarray-1.0.1/docs/installation.rst
--rw-r--r--   0        0        0     1652 2024-04-04 18:54:29.129871 qarray-1.0.1/docs/simulating_double_dot.rst
--rw-r--r--   0        0        0     2507 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/charge_sensing.py
--rw-r--r--   0        0        0     2632 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/double_dot.py
--rw-r--r--   0        0        0      589 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/gate_voltage_composer_tricks.py
--rw-r--r--   0        0        0     1933 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/gradient.py
--rw-r--r--   0        0        0     2747 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/linear_quadruple_dot.py
--rw-r--r--   0        0        0     2520 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/linear_triple_dot.py
--rw-r--r--   0        0        0      694 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/paper_examples.py
--rw-r--r--   0        0        0     2650 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/quadruple_dot_all_gates.py
--rw-r--r--   0        0        0     3229 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/simulating_closed_five_dot_array_.py
--rw-r--r--   0        0        0     1597 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/simulating_open_four_dot_array.py
--rw-r--r--   0        0        0     2888 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/triple_dot.py
--rw-r--r--   0        0        0    27960 2024-04-04 18:54:29.133871 qarray-1.0.1/misc/recreations.jpg
--rw-r--r--   0        0        0    17300 2024-04-04 18:54:29.133871 qarray-1.0.1/misc/structure.jpg
--rw-r--r--   0        0        0      669 2024-04-04 18:54:29.133871 qarray-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      506 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/__init__.py
--rw-r--r--   0        0        0      108 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/__init__.py
--rw-r--r--   0        0        0       80 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      640 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2649 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/closed.py
--rw-r--r--   0        0        0     2429 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/open.py
--rw-r--r--   0        0        0      114 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/__init__.py
--rw-r--r--   0        0        0       83 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      634 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2372 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/closed.py
--rw-r--r--   0        0        0     2094 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/open.py
--rw-r--r--   0        0        0     6570 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/BaseDataClass.py
--rw-r--r--   0        0        0     5629 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/ChargeSensedDotArray.py
--rw-r--r--   0        0        0     7092 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/DotArray.py
--rw-r--r--   0        0        0    10321 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/GateVoltageComposer.py
--rw-r--r--   0        0        0      139 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/__init__.py
--rw-r--r--   0        0        0     7884 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/_helper_functions.py
--rw-r--r--   0        0        0     5334 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/functions.py
--rw-r--r--   0        0        0       84 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/__init__.py
--rw-r--r--   0        0        0       68 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      726 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     6227 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/closed.py
--rw-r--r--   0        0        0      275 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/helper_functions.py
--rw-r--r--   0        0        0     4819 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/open.py
--rw-r--r--   0        0        0       80 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/__init__.py
--rw-r--r--   0        0        0      132 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
--rw-r--r--   0        0        0      947 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     7025 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/core_python.py
--rw-r--r--   0        0        0      258 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/qarray_types/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/qarray_types/typing_classes.py
--rw-r--r--   0        0        0      109 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/rust_core/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/rust_core/core_rust.py
--rw-r--r--   0        0        0      133 2024-04-04 18:54:29.133871 qarray-1.0.1/requirements.txt
--rw-r--r--   0        0        0      338 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/GLOBAL_OPTIONS.py
--rw-r--r--   0        0        0        0 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3357 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/helper_functions.py
--rw-r--r--   0        0        0      939 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/pydantic_validation_tests.py
--rw-r--r--   0        0        0     6190 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_against_brute_force.py
--rw-r--r--   0        0        0    17563 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_charge_combinations.py
--rw-r--r--   0        0        0     6110 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_double_dot.py
--rw-r--r--   0        0        0     3978 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_gate_voltage_composer.py
--rw-r--r--   0        0        0     5939 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_quadruple_dot.py
--rw-r--r--   0        0        0     4579 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_solver.py
--rw-r--r--   0        0        0     9900 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_threshold.py
--rw-r--r--   0        0        0     5938 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_triple_dot.py
--rw-r--r--   0        0        0     1724 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_user_interaction.py
--rw-r--r--   0        0        0      109 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/tests.py
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 qarray-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      850 2024-04-05 07:47:47.854266 qarray-1.0.2/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0     1317 2024-04-05 07:47:47.854266 qarray-1.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3079 2024-04-05 07:47:47.854266 qarray-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-05 07:47:47.854266 qarray-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3044 2024-04-05 07:47:47.854266 qarray-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 07:47:47.854266 qarray-1.0.2/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-05 07:47:47.854266 qarray-1.0.2/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-05 07:47:47.854266 qarray-1.0.2/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/charge_sensing.py
+-rw-r--r--   0        0        0     2632 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/paper_examples.py
+-rw-r--r--   0        0        0     2650 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/simulating_closed_five_dot_array_.py
+-rw-r--r--   0        0        0     1684 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/simulating_open_four_dot_array.py
+-rw-r--r--   0        0        0     2888 2024-04-05 07:47:47.854266 qarray-1.0.2/examples/triple_dot.py
+-rw-r--r--   0        0        0    27960 2024-04-05 07:47:47.854266 qarray-1.0.2/misc/recreations.jpg
+-rw-r--r--   0        0        0    17300 2024-04-05 07:47:47.854266 qarray-1.0.2/misc/structure.jpg
+-rw-r--r--   0        0        0      669 2024-04-05 07:47:47.858266 qarray-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      506 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     8001 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-05 07:47:47.858266 qarray-1.0.2/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      133 2024-04-05 07:47:47.858266 qarray-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6190 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6110 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5939 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-05 07:47:47.858266 qarray-1.0.2/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1724 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-05 07:47:47.862266 qarray-1.0.2/tests/tests.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 qarray-1.0.2/PKG-INFO
```

### Comparing `qarray-1.0.1/.github/workflows/pypi.yaml` & `qarray-1.0.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/.github/workflows/test.yaml` & `qarray-1.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/.gitignore` & `qarray-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/LICENSE` & `qarray-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/README.md` & `qarray-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Qarray
 
 ![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/qarray)
 
-![structure.jpg](./misc/structure.jpg)
+![structure.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/structure)
 
 **Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
-Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver charge stability diagrams in seconds or
+Harnesses the speed of Rust or the compute power of GPUs using JAX to deliver charge stability diagrams in seconds or
 millisecond
 
-![recreations.jpg](./misc/recreations.jpg)
+![recreations.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/recreations)
 
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
```

### Comparing `qarray-1.0.1/docs/installation.rst` & `qarray-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/docs/simulating_double_dot.rst` & `qarray-1.0.2/docs/simulating_double_dot.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/charge_sensing.py` & `qarray-1.0.2/examples/charge_sensing.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/double_dot.py` & `qarray-1.0.2/examples/double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/gate_voltage_composer_tricks.py` & `qarray-1.0.2/examples/gate_voltage_composer_tricks.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/gradient.py` & `qarray-1.0.2/examples/gradient.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/linear_quadruple_dot.py` & `qarray-1.0.2/examples/linear_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/linear_triple_dot.py` & `qarray-1.0.2/examples/linear_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/paper_examples.py` & `qarray-1.0.2/examples/paper_examples.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/quadruple_dot_all_gates.py` & `qarray-1.0.2/examples/quadruple_dot_all_gates.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/simulating_closed_five_dot_array_.py` & `qarray-1.0.2/examples/simulating_closed_five_dot_array_.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/examples/simulating_open_four_dot_array.py` & `qarray-1.0.2/examples/simulating_open_four_dot_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 
 import numpy as np
+import scipy
 from matplotlib import pyplot as plt
 
 from qarray import DotArray, GateVoltageComposer, dot_occupation_changes
 
 cdd = [
     [1., -0., -0.004, -0.0],
     [-0., 1, -0.04, -0.01],
@@ -17,18 +18,18 @@
     [0.05, 0.4, 1., 0.4],
     [0.04, 0.1, 0.4, 1.1]
 ])
 
 model = DotArray(
     cdd=cdd,
     cgd=cgd,
-    core='python',
+    core='rust',
     charge_carrier='electron',
-    T=0.02,
-    threshold=0.5
+    T=0.01 / 8.617333262145e-5,
+    threshold=1.
 )
 model.max_charge_carriers = 2
 
 voltage_composer = GateVoltageComposer(n_gate=model.n_gate)
 
 vx_min, vx_max = -1.4, 0.6
 vy_min, vy_max = -1, 1
@@ -50,15 +51,18 @@
 
 def lorentzian(x, x0, gamma):
     return np.reciprocal((((x - x0) / gamma) ** 2 + 1))
 
 
 z = lorentzian(v_sensor, 0.5, 0.1)
 
+n = scipy.ndimage.gaussian_filter(np.random.randn(z.size), 1).reshape(z.shape)
+z += n * 0.00015
+
+
 z = -np.gradient(z, axis=0)
 z = (z - z.min()) / (z.max() - z.min())
-z = z + np.random.randn(*z.shape) * 0.05
 
 fig, ax = plt.subplots()
 ax.imshow(z.T, extent=[vx_min, vx_max, vy_min, vy_max], origin='lower', interpolation='None',
           aspect='equal', cmap='YlGnBu')
 plt.savefig('quadruple_dot.pdf', bbox_inches='tight')
```

### Comparing `qarray-1.0.1/examples/triple_dot.py` & `qarray-1.0.2/examples/triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/misc/recreations.jpg` & `qarray-1.0.2/misc/recreations.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/misc/structure.jpg` & `qarray-1.0.2/misc/structure.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/pyproject.toml` & `qarray-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.2/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_jax/closed.py` & `qarray-1.0.2/qarray/brute_force_jax/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_jax/open.py` & `qarray-1.0.2/qarray/brute_force_jax/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.2/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_python/closed.py` & `qarray-1.0.2/qarray/brute_force_python/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/brute_force_python/open.py` & `qarray-1.0.2/qarray/brute_force_python/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/classes/BaseDataClass.py` & `qarray-1.0.2/qarray/classes/BaseDataClass.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/classes/ChargeSensedDotArray.py` & `qarray-1.0.2/qarray/classes/ChargeSensedDotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/classes/DotArray.py` & `qarray-1.0.2/qarray/classes/DotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/classes/GateVoltageComposer.py` & `qarray-1.0.2/qarray/classes/GateVoltageComposer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/classes/_helper_functions.py` & `qarray-1.0.2/qarray/classes/_helper_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from ..brute_force_jax import ground_state_open_brute_force_jax, ground_state_closed_brute_force_jax
 from ..brute_force_python import ground_state_open_brute_force_python, ground_state_closed_brute_force_python
 from ..jax_core import ground_state_open_jax, ground_state_closed_jax
 from ..python_core import ground_state_open_python, ground_state_closed_python
 from ..qarray_types import VectorList
 from ..rust_core import ground_state_open_rust, ground_state_closed_rust
 
+# Boltzmann constant in eV/K
+k_B = 8.617333262145e-5  # eV/K
 
 def _validate_vg(vg: VectorList, n_gate: NonNegativeInt):
     """
     This function is used to validate the shape of the dot voltage array.
     :param vg: the dot voltage array
     """
     if vg.shape[-1] != n_gate:
@@ -34,30 +36,32 @@
     # reshaping the dot voltage array to be of shape (n_points, n_gate)
     vg = vg.reshape(-1, model.n_gate)
 
     # performing the type conversion if necessary
     if not isinstance(vg, VectorList):
         vg = VectorList(vg)
 
+    kB_T = 8.617333262145e-5 * model.T
+
     # calling the appropriate core function to compute the ground state
     match model.core:
         case 'rust' | 'Rust' | 'RUST' | 'r':
             result = ground_state_open_rust(
                 vg=vg, cgd=model.cgd,
                 cdd_inv=model.cdd_inv,
                 threshold=model.threshold,
-                polish=model.polish, T=model.T
+                polish=model.polish, T=kB_T
             )
         case 'jax' | 'Jax' | 'JAX' | 'j':
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using threshold of 1.0')
 
             result = ground_state_open_jax(
                 vg=vg, cgd=model.cgd,
-                cdd_inv=model.cdd_inv, T=model.T, batch_size=model.batch_size
+                cdd_inv=model.cdd_inv, T=kB_T, batch_size=model.batch_size
             )
 
         case 'brute_force_jax' | 'jax_brute_force' | 'Jax_brute_force' | 'JAX_BRUTE_FORCE' | 'b':
 
             if model.max_charge_carriers is None:
                 message = ('The max_charge_carriers must be specified for the jax_brute_force core use:'
                            '\nmodel.max_charge_carriers = #')
@@ -65,15 +69,15 @@
 
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using threshold of 1.0')
             result = ground_state_open_brute_force_jax(
                 vg=vg, cgd=model.cgd,
                 cdd_inv=model.cdd_inv,
                 max_number_of_charge_carriers=model.max_charge_carriers,
-                T=model.T,
+                T=kB_T,
                 batch_size=model.batch_size
             )
 
         case 'python_brute_force' | 'Python_brute_force' | 'PYTHON_BRUTE_FORCE' | 'bp' | 'brute_force_python' | 'Brute_force_python' | 'BRUTE_FORCE_PYTHON' | 'bpy':
             if model.max_charge_carriers is None:
                 message = ('The max_charge_carriers must be specified for the jax_brute_force core use:'
                            '\nmodel.max_charge_carriers = #')
@@ -82,15 +86,15 @@
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using threshold of 1.0')
 
             result = ground_state_open_brute_force_python(
                 vg=vg, cgd=model.cgd,
                 cdd_inv=model.cdd_inv,
                 max_number_of_charge_carriers=model.max_charge_carriers,
-                T=model.T
+                T=kB_T
             )
 
         case 'python' | 'Python' | 'PYTHON' | 'p':
             result = ground_state_open_python(
                 vg=vg, cgd=model.cgd,
                 cdd_inv=model.cdd_inv,
                 threshold=model.threshold,
@@ -118,52 +122,54 @@
     # reshaping the dot voltage array to be of shape (n_points, n_gate)
     vg = vg.reshape(-1, model.n_gate)
 
     # performing the type conversion if necessary
     if not isinstance(vg, VectorList):
         vg = VectorList(vg)
 
+    kB_T = 8.617333262145e-5 * model.T
+
     # calling the appropriate core function to compute the ground state
     match model.core:
         case 'rust' | 'Rust' | 'RUST' | 'r':
             result = ground_state_closed_rust(
                 vg=vg, n_charge=n_charge, cgd=model.cgd,
                 cdd=model.cdd, cdd_inv=model.cdd_inv,
-                threshold=model.threshold, polish=model.polish, T=model.T
+                threshold=model.threshold, polish=model.polish, T=kB_T
             )
 
         case 'jax' | 'Jax' | 'JAX' | 'j':
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using of 1.0')
             result = ground_state_closed_jax(
                 vg=vg, n_charge=n_charge, cgd=model.cgd,
-                cdd=model.cdd, cdd_inv=model.cdd_inv, T=model.T, batch_size=model.batch_size
+                cdd=model.cdd, cdd_inv=model.cdd_inv, T=kB_T, batch_size=model.batch_size
             )
 
         case 'brute_force_jax' | 'jax_brute_force' | 'Jax_brute_force' | 'JAX_BRUTE_FORCE' | 'b':
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using threshold of 1.0')
 
             result = ground_state_closed_brute_force_jax(
                 vg=vg, n_charge=n_charge, cgd=model.cgd,
-                cdd=model.cdd, cdd_inv=model.cdd_inv, T=model.T, batch_size=model.batch_size
+                cdd=model.cdd, cdd_inv=model.cdd_inv, T=kB_T, batch_size=model.batch_size
             )
 
         case 'python_brute_force' | 'Python_brute_force' | 'PYTHON_BRUTE_FORCE' | 'bp' | 'brute_force_python' | 'Brute_force_python' | 'BRUTE_FORCE_PYTHON' | 'bpy':
             if model.max_charge_carriers is None:
                 message = ('The max_charge_carriers must be specified for the jax_brute_force core use:'
                            '\nmodel.max_charge_carriers = #')
                 raise ValueError(message)
 
             if model.threshold < 1.:
                 print('Warning: JAX core does not support threshold < 1.0, using threshold of 1.0')
 
             result = ground_state_closed_brute_force_python(
                 vg=vg, n_charge=n_charge, cgd=model.cgd,
-                cdd=model.cdd, cdd_inv=model.cdd_inv, T=model.T
+                cdd=model.cdd, cdd_inv=model.cdd_inv, T=kB_T
             )
 
         case 'python' | 'Python' | 'PYTHON' | 'p':
             result = ground_state_closed_python(
                 vg=vg, n_charge=n_charge, cgd=model.cgd,
                 cdd=model.cdd, cdd_inv=model.cdd_inv,
                 threshold=model.threshold, polish=model.polish
```

### Comparing `qarray-1.0.1/qarray/functions.py` & `qarray-1.0.2/qarray/functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.2/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/jax_core/closed.py` & `qarray-1.0.2/qarray/jax_core/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/jax_core/open.py` & `qarray-1.0.2/qarray/jax_core/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py` & `qarray-1.0.2/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/python_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.2/qarray/python_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/python_core/core_python.py` & `qarray-1.0.2/qarray/python_core/core_python.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/qarray_types/typing_classes.py` & `qarray-1.0.2/qarray/qarray_types/typing_classes.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/qarray/rust_core/core_rust.py` & `qarray-1.0.2/qarray/rust_core/core_rust.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/helper_functions.py` & `qarray-1.0.2/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/pydantic_validation_tests.py` & `qarray-1.0.2/tests/pydantic_validation_tests.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_against_brute_force.py` & `qarray-1.0.2/tests/test_against_brute_force.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_charge_combinations.py` & `qarray-1.0.2/tests/test_charge_combinations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_double_dot.py` & `qarray-1.0.2/tests/test_double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_gate_voltage_composer.py` & `qarray-1.0.2/tests/test_gate_voltage_composer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_quadruple_dot.py` & `qarray-1.0.2/tests/test_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_solver.py` & `qarray-1.0.2/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_threshold.py` & `qarray-1.0.2/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_triple_dot.py` & `qarray-1.0.2/tests/test_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/tests/test_user_interaction.py` & `qarray-1.0.2/tests/test_user_interaction.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.1/PKG-INFO` & `qarray-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qarray
-Version: 1.0.1
+Version: 1.0.2
 Summary: Qarray is a Python package for simulating quantum dot arrays.
 Author-email: Barnaby van Straaten <barnaby.vanstraaten@kellogg.ox.ac.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: qarray-rust-core==1.2.0
 Requires-Dist: osqp==0.6.3
@@ -19,24 +19,24 @@
 Project-URL: Home, https://github.com/b-vanstraaten/qarray
 
 # Qarray
 
 ![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/qarray)
 
-![structure.jpg](./misc/structure.jpg)
+![structure.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/structure)
 
 **Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
-Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver charge stability diagrams in seconds or
+Harnesses the speed of Rust or the compute power of GPUs using JAX to deliver charge stability diagrams in seconds or
 millisecond
 
-![recreations.jpg](./misc/recreations.jpg)
+![recreations.jpg](https://github.com/b-vanstraaten/qarray/raw/main/misc/recreations)
 
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
```

