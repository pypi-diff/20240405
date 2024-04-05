# Comparing `tmp/qarray-1.0.8.tar.gz` & `tmp/qarray-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-1.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-1.0.8.tar` & `qarray-1.0.9.tar`

### file list

```diff
@@ -1,73 +1,76 @@
--rw-r--r--   0        0        0      724 2024-04-05 09:39:11.838844 qarray-1.0.8/.github/workflows/linux_tests.yaml
--rw-r--r--   0        0        0      725 2024-04-05 09:39:11.838844 qarray-1.0.8/.github/workflows/macos_tests.yaml
--rw-r--r--   0        0        0      850 2024-04-05 09:39:11.838844 qarray-1.0.8/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0      729 2024-04-05 09:39:11.838844 qarray-1.0.8/.github/workflows/windows_tests.yaml
--rw-r--r--   0        0        0     3079 2024-04-05 09:39:11.838844 qarray-1.0.8/.gitignore
--rw-r--r--   0        0        0     1087 2024-04-05 09:39:11.838844 qarray-1.0.8/LICENSE
--rw-r--r--   0        0        0     4773 2024-04-05 09:39:11.838844 qarray-1.0.8/README.md
--rw-r--r--   0        0        0     1024 2024-04-05 09:39:11.838844 qarray-1.0.8/docs/installation.rst
--rw-r--r--   0        0        0     1652 2024-04-05 09:39:11.838844 qarray-1.0.8/docs/simulating_double_dot.rst
--rw-r--r--   0        0        0     2507 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/charge_sensing.py
--rw-r--r--   0        0        0     2632 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/double_dot.py
--rw-r--r--   0        0        0      589 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/gate_voltage_composer_tricks.py
--rw-r--r--   0        0        0     1933 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/gradient.py
--rw-r--r--   0        0        0     2747 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/linear_quadruple_dot.py
--rw-r--r--   0        0        0     2520 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/linear_triple_dot.py
--rw-r--r--   0        0        0      694 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/paper_examples.py
--rw-r--r--   0        0        0     2650 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/quadruple_dot_all_gates.py
--rw-r--r--   0        0        0     3229 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/simulating_closed_five_dot_array_.py
--rw-r--r--   0        0        0     1684 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/simulating_open_four_dot_array.py
--rw-r--r--   0        0        0     2888 2024-04-05 09:39:11.838844 qarray-1.0.8/examples/triple_dot.py
--rw-r--r--   0        0        0   520772 2024-04-05 09:39:11.842844 qarray-1.0.8/misc/recreations.jpg
--rw-r--r--   0        0        0   181957 2024-04-05 09:39:11.842844 qarray-1.0.8/misc/structure.jpg
--rw-r--r--   0        0        0     3781 2024-04-05 09:39:11.842844 qarray-1.0.8/pypi_README.md
--rw-r--r--   0        0        0     1280 2024-04-05 09:39:11.842844 qarray-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      644 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/__init__.py
--rw-r--r--   0        0        0      108 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_jax/__init__.py
--rw-r--r--   0        0        0       80 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_jax/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      640 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2649 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_jax/closed.py
--rw-r--r--   0        0        0     2429 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_jax/open.py
--rw-r--r--   0        0        0      114 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_python/__init__.py
--rw-r--r--   0        0        0       83 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_python/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      634 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2372 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_python/closed.py
--rw-r--r--   0        0        0     2094 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/brute_force_python/open.py
--rw-r--r--   0        0        0     6570 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/BaseDataClass.py
--rw-r--r--   0        0        0     5629 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/ChargeSensedDotArray.py
--rw-r--r--   0        0        0     7092 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/DotArray.py
--rw-r--r--   0        0        0    10321 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/GateVoltageComposer.py
--rw-r--r--   0        0        0      139 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/__init__.py
--rw-r--r--   0        0        0     8001 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/classes/_helper_functions.py
--rw-r--r--   0        0        0     5334 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/functions.py
--rw-r--r--   0        0        0       84 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/__init__.py
--rw-r--r--   0        0        0       68 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      726 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     6227 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/closed.py
--rw-r--r--   0        0        0      275 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/helper_functions.py
--rw-r--r--   0        0        0     4819 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/jax_core/open.py
--rw-r--r--   0        0        0       80 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/python_core/__init__.py
--rw-r--r--   0        0        0      132 2024-04-05 09:39:11.842844 qarray-1.0.8/qarray/python_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
--rw-r--r--   0        0        0      947 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     7025 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/python_core/core_python.py
--rw-r--r--   0        0        0      258 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/qarray_types/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/qarray_types/typing_classes.py
--rw-r--r--   0        0        0      109 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/rust_core/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-05 09:39:11.846844 qarray-1.0.8/qarray/rust_core/core_rust.py
--rw-r--r--   0        0        0      133 2024-04-05 09:39:11.846844 qarray-1.0.8/requirements.txt
--rw-r--r--   0        0        0      338 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/GLOBAL_OPTIONS.py
--rw-r--r--   0        0        0        0 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3357 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/helper_functions.py
--rw-r--r--   0        0        0      939 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/pydantic_validation_tests.py
--rw-r--r--   0        0        0     6190 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_against_brute_force.py
--rw-r--r--   0        0        0    17563 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_charge_combinations.py
--rw-r--r--   0        0        0     6110 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_double_dot.py
--rw-r--r--   0        0        0     3978 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_gate_voltage_composer.py
--rw-r--r--   0        0        0     5939 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_quadruple_dot.py
--rw-r--r--   0        0        0     4579 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_solver.py
--rw-r--r--   0        0        0     9900 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_threshold.py
--rw-r--r--   0        0        0     5938 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_triple_dot.py
--rw-r--r--   0        0        0     1724 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/test_user_interaction.py
--rw-r--r--   0        0        0      109 2024-04-05 09:39:11.846844 qarray-1.0.8/tests/tests.py
--rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 qarray-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      724 2024-04-05 11:10:31.352584 qarray-1.0.9/.github/workflows/linux_tests.yaml
+-rw-r--r--   0        0        0     1314 2024-04-05 11:10:31.352584 qarray-1.0.9/.github/workflows/macos_tests.yaml
+-rw-r--r--   0        0        0      850 2024-04-05 11:10:31.352584 qarray-1.0.9/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0      729 2024-04-05 11:10:31.352584 qarray-1.0.9/.github/workflows/windows_tests.yaml
+-rw-r--r--   0        0        0     3079 2024-04-05 11:10:31.352584 qarray-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-05 11:10:31.352584 qarray-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4768 2024-04-05 11:10:31.352584 qarray-1.0.9/README.md
+-rw-r--r--   0        0        0     1024 2024-04-05 11:10:31.352584 qarray-1.0.9/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-05 11:10:31.352584 qarray-1.0.9/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-05 11:10:31.352584 qarray-1.0.9/examples/charge_sensing.py
+-rw-r--r--   0        0        0   135928 2024-04-05 11:10:31.352584 qarray-1.0.9/examples/double_dot.ipynb
+-rw-r--r--   0        0        0     2632 2024-04-05 11:10:31.352584 qarray-1.0.9/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-05 11:10:31.352584 qarray-1.0.9/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/paper_examples.py
+-rw-r--r--   0        0        0   108774 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/quadruple_dot.ipynb
+-rw-r--r--   0        0        0     2650 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/simulating_closed_five_dot_array_.py
+-rw-r--r--   0        0        0     1684 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/simulating_open_four_dot_array.py
+-rw-r--r--   0        0        0   116282 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/triple_dot.ipynb
+-rw-r--r--   0        0        0     2888 2024-04-05 11:10:31.356584 qarray-1.0.9/examples/triple_dot.py
+-rw-r--r--   0        0        0   520772 2024-04-05 11:10:31.360584 qarray-1.0.9/misc/recreations.jpg
+-rw-r--r--   0        0        0   181957 2024-04-05 11:10:31.360584 qarray-1.0.9/misc/structure.jpg
+-rw-r--r--   0        0        0     3813 2024-04-05 11:10:31.360584 qarray-1.0.9/pypi_README.md
+-rw-r--r--   0        0        0     1280 2024-04-05 11:10:31.360584 qarray-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      644 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     8001 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-05 11:10:31.360584 qarray-1.0.9/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-05 11:10:31.364584 qarray-1.0.9/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      133 2024-04-05 11:10:31.364584 qarray-1.0.9/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6190 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6110 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5939 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1724 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-05 11:10:31.364584 qarray-1.0.9/tests/tests.py
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 qarray-1.0.9/PKG-INFO
```

### Comparing `qarray-1.0.8/.github/workflows/linux_tests.yaml` & `qarray-1.0.9/.github/workflows/linux_tests.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/.github/workflows/macos_tests.yaml` & `qarray-1.0.9/.github/workflows/macos_tests.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,37 @@
 on:
     push:
         branches:
             - main  # Change this to your main branch name if different
 
 jobs:
 
-    windows:
-        runs-on: macos-latest
+    macos14:
+        runs-on: macos-14
+        strategy:
+            matrix:
+                python-version: [ '3.10', '3.11' ]
+        steps:
+            -   name: Checkout code
+                uses: actions/checkout@v2
+
+            -   name: Set up Python
+                uses: actions/setup-python@v2
+                with:
+                    python-version: ${{ matrix.python-version }}
+
+            -   name: Install dependencies
+                run: pip install -r requirements.txt
+
+            -   name: Run unit tests
+                run: python -m unittest discover -s ./tests -t .
+
+
+    macos13:
+        runs-on: macos-13
         strategy:
             matrix:
                 python-version: [ '3.10', '3.11' ]
         steps:
             -   name: Checkout code
                 uses: actions/checkout@v2
```

### Comparing `qarray-1.0.8/.github/workflows/pypi.yaml` & `qarray-1.0.9/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/.github/workflows/windows_tests.yaml` & `qarray-1.0.9/.github/workflows/windows_tests.yaml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/.gitignore` & `qarray-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/LICENSE` & `qarray-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/README.md` & `qarray-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 # number of charge carriers in each dot for each gate voltage
 ```
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
-1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
-2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
-3. [Linear Quadruple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_quadruple_dot.py)
+1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.ipynb)
+2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/triple_dot.ipynb)
+3. [Linear Quadruple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/quadruple_dot.ipynb)
 4. [Charge sensed double quantum dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/charge_sensing.py)
 
 ## References
 
 <a name="[1]"></a>
 [1] [Full control of quadruple quantum dot circuit charge states in the single electron regime](https://pubs.aip.org/aip/apl/article/104/18/183111/24127/Full-control-of-quadruple-quantum-dot-circuit)
```

### Comparing `qarray-1.0.8/docs/installation.rst` & `qarray-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/docs/simulating_double_dot.rst` & `qarray-1.0.9/docs/simulating_double_dot.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/charge_sensing.py` & `qarray-1.0.9/examples/charge_sensing.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/double_dot.py` & `qarray-1.0.9/examples/double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/gate_voltage_composer_tricks.py` & `qarray-1.0.9/examples/gate_voltage_composer_tricks.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/gradient.py` & `qarray-1.0.9/examples/gradient.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/linear_quadruple_dot.py` & `qarray-1.0.9/examples/linear_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/linear_triple_dot.py` & `qarray-1.0.9/examples/linear_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/paper_examples.py` & `qarray-1.0.9/examples/paper_examples.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/quadruple_dot_all_gates.py` & `qarray-1.0.9/examples/quadruple_dot_all_gates.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/simulating_closed_five_dot_array_.py` & `qarray-1.0.9/examples/simulating_closed_five_dot_array_.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/simulating_open_four_dot_array.py` & `qarray-1.0.9/examples/simulating_open_four_dot_array.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/examples/triple_dot.py` & `qarray-1.0.9/examples/triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/misc/recreations.jpg` & `qarray-1.0.9/misc/recreations.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/misc/structure.jpg` & `qarray-1.0.9/misc/structure.jpg`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/pypi_README.md` & `qarray-1.0.9/pypi_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 **QArray** harnesses the speed of the systems programming language Rust or the compute power of GPUs using JAX XLA
 to deliver constant capacitance model charge stability diagrams in seconds or millisecond. It couples
 highly optimised and parrelised code with two new algorithms to compute the ground state charge configuration. These
 algorithms scale better than the traditional brute-force approach and do not require the user to maxmimum specify
 the maxmimum number of charge carrier a priori.
 
 QArray runs on both CPUs and GPUs, and is designed to be easy to use and integrate into your existing workflow.
-It was developed on macOS running on Apple Silicon and is continuously tested, Linux and Windows.
+It was developed on macOS running on Apple Silicon and is continuously tested on Ubuntu-latest, macOS13, macos14,
+Windows-latest.
 
 Finally, QArray captures physical effects such as measuring the charge stability diagram
 of with a SET and thermal broadening of charge transitions. The combination of these effects
 permits the simulation of charge stability diagrams which are visually similar to those measured experimentally.
 The plots on the right below are measured experimentally, and the plots on the left are simulated using QArray.
 
 ## Installation
```

### Comparing `qarray-1.0.8/pyproject.toml` & `qarray-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "quantum simulation",
     "quantum optimization"
 ]
 
 dynamic = ["version", "description"]
 requires-python = ">=3.10"
 dependencies = [
-    'qarray-rust-core==1.2.0',
+    'qarray-rust-core==1.2.3',
     'osqp==0.6.3',
     'numpy>=1.26',
     'pydantic>=2.3',
     'scipy>=1.11',
     'matplotlib>=3.8',
     'loguru>=0.5',
     'jax>=0.2',
```

### Comparing `qarray-1.0.8/qarray/__init__.py` & `qarray-1.0.9/qarray/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and JAX XLA acceleration
 to compute charge stability diagrams of large both open and closed arrays in milliseconds.
 """
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 from .classes import (DotArray, GateVoltageComposer, ChargeSensedDotArray)
 from .functions import (optimal_Vg, compute_threshold, convert_to_maxwell, dot_occupation_changes, lorentzian,
                         dot_gradient)
 from .python_core import (ground_state_open_python, ground_state_closed_python)
 from .rust_core import (ground_state_open_rust, ground_state_closed_rust, closed_charge_configurations_rust)
```

### Comparing `qarray-1.0.8/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.9/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/brute_force_jax/closed.py` & `qarray-1.0.9/qarray/brute_force_jax/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/brute_force_jax/open.py` & `qarray-1.0.9/qarray/brute_force_jax/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.9/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/brute_force_python/closed.py` & `qarray-1.0.9/qarray/brute_force_python/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/brute_force_python/open.py` & `qarray-1.0.9/qarray/brute_force_python/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/classes/BaseDataClass.py` & `qarray-1.0.9/qarray/classes/BaseDataClass.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/classes/ChargeSensedDotArray.py` & `qarray-1.0.9/qarray/classes/ChargeSensedDotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/classes/DotArray.py` & `qarray-1.0.9/qarray/classes/DotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/classes/GateVoltageComposer.py` & `qarray-1.0.9/qarray/classes/GateVoltageComposer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/classes/_helper_functions.py` & `qarray-1.0.9/qarray/classes/_helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/functions.py` & `qarray-1.0.9/qarray/functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.9/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/jax_core/closed.py` & `qarray-1.0.9/qarray/jax_core/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/jax_core/open.py` & `qarray-1.0.9/qarray/jax_core/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py` & `qarray-1.0.9/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/python_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.9/qarray/python_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/python_core/core_python.py` & `qarray-1.0.9/qarray/python_core/core_python.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/qarray_types/typing_classes.py` & `qarray-1.0.9/qarray/qarray_types/typing_classes.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/qarray/rust_core/core_rust.py` & `qarray-1.0.9/qarray/rust_core/core_rust.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/helper_functions.py` & `qarray-1.0.9/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/pydantic_validation_tests.py` & `qarray-1.0.9/tests/pydantic_validation_tests.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_against_brute_force.py` & `qarray-1.0.9/tests/test_against_brute_force.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_charge_combinations.py` & `qarray-1.0.9/tests/test_charge_combinations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_double_dot.py` & `qarray-1.0.9/tests/test_double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_gate_voltage_composer.py` & `qarray-1.0.9/tests/test_gate_voltage_composer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_quadruple_dot.py` & `qarray-1.0.9/tests/test_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_solver.py` & `qarray-1.0.9/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_threshold.py` & `qarray-1.0.9/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_triple_dot.py` & `qarray-1.0.9/tests/test_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/tests/test_user_interaction.py` & `qarray-1.0.9/tests/test_user_interaction.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.8/PKG-INFO` & `qarray-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qarray
-Version: 1.0.8
+Version: 1.0.9
 Summary: Qarray, a GPU accelerated quantum dot array simulator, leveraging parallelised Rust and JAX XLA acceleration
 Keywords: semiconducting,quantum dots,quantum,simulation,GPU,rust,jax,quantum computing,quantum programming,quantum simulation,quantum optimization
 Author-email: Barnaby van Straaten <barnaby.vanstraaten@kellogg.ox.ac.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: qarray-rust-core==1.2.0
+Requires-Dist: qarray-rust-core==1.2.3
 Requires-Dist: osqp==0.6.3
 Requires-Dist: numpy>=1.26
 Requires-Dist: pydantic>=2.3
 Requires-Dist: scipy>=1.11
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: loguru>=0.5
 Requires-Dist: jax>=0.2
@@ -38,15 +38,16 @@
 **QArray** harnesses the speed of the systems programming language Rust or the compute power of GPUs using JAX XLA
 to deliver constant capacitance model charge stability diagrams in seconds or millisecond. It couples
 highly optimised and parrelised code with two new algorithms to compute the ground state charge configuration. These
 algorithms scale better than the traditional brute-force approach and do not require the user to maxmimum specify
 the maxmimum number of charge carrier a priori.
 
 QArray runs on both CPUs and GPUs, and is designed to be easy to use and integrate into your existing workflow.
-It was developed on macOS running on Apple Silicon and is continuously tested, Linux and Windows.
+It was developed on macOS running on Apple Silicon and is continuously tested on Ubuntu-latest, macOS13, macos14,
+Windows-latest.
 
 Finally, QArray captures physical effects such as measuring the charge stability diagram
 of with a SET and thermal broadening of charge transitions. The combination of these effects
 permits the simulation of charge stability diagrams which are visually similar to those measured experimentally.
 The plots on the right below are measured experimentally, and the plots on the left are simulated using QArray.
 
 ## Installation
```

