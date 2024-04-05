# Comparing `tmp/qibo-0.2.6.tar.gz` & `tmp/qibo-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo-0.2.6.tar", max compression
+gzip compressed data, was "qibo-0.2.7.tar", max compression
```

## Comparing `qibo-0.2.6.tar` & `qibo-0.2.7.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0    11342 2024-03-13 23:08:22.576926 qibo-0.2.6/LICENSE
--rw-r--r--   0        0        0     3277 2024-03-13 23:08:22.576926 qibo-0.2.6/README.md
--rw-r--r--   0        0        0     3044 2024-03-13 23:08:22.756928 qibo-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      569 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/__init__.py
--rw-r--r--   0        0        0     6201 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/__init__.py
--rw-r--r--   0        0        0    17580 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/_clifford_operations.py
--rw-r--r--   0        0        0    14561 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/abstract.py
--rw-r--r--   0        0        0    12514 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/clifford.py
--rw-r--r--   0        0        0     2780 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/einsum_utils.py
--rw-r--r--   0        0        0    14244 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/npmatrices.py
--rw-r--r--   0        0        0    34052 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/numpy.py
--rw-r--r--   0        0        0     8600 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/backends/tensorflow.py
--rw-r--r--   0        0        0    11847 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/callbacks.py
--rw-r--r--   0        0        0     3097 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/config.py
--rw-r--r--   0        0        0     8513 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/derivative.py
--rw-r--r--   0        0        0      136 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/__init__.py
--rw-r--r--   0        0        0    16739 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/abstract.py
--rw-r--r--   0        0        0    30848 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/channels.py
--rw-r--r--   0        0        0    69440 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/gates.py
--rw-r--r--   0        0        0     9721 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/measurements.py
--rw-r--r--   0        0        0     6004 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/gates/special.py
--rw-r--r--   0        0        0      109 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/__init__.py
--rw-r--r--   0        0        0     4466 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/abstract.py
--rw-r--r--   0        0        0     6009 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/adiabatic.py
--rw-r--r--   0        0        0    31839 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/hamiltonians.py
--rw-r--r--   0        0        0     6695 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/models.py
--rw-r--r--   0        0        0    13154 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/hamiltonians/terms.py
--rw-r--r--   0        0        0     6883 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/measurements.py
--rw-r--r--   0        0        0      422 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/__init__.py
--rw-r--r--   0        0        0    11877 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/_openqasm.py
--rw-r--r--   0        0        0    52982 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/circuit.py
--rw-r--r--   0        0        0        0 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/dbi/__init__.py
--rw-r--r--   0        0        0     6182 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/dbi/double_bracket.py
--rw-r--r--   0        0        0     6023 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/dbi/utils.py
--rw-r--r--   0        0        0    13651 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/distcircuit.py
--rw-r--r--   0        0        0    12269 2024-03-13 23:08:22.756928 qibo-0.2.6/src/qibo/models/encodings.py
--rw-r--r--   0        0        0    39577 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/error_mitigation.py
--rw-r--r--   0        0        0    13526 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/evolution.py
--rw-r--r--   0        0        0    11600 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/grover.py
--rw-r--r--   0        0        0     9065 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/hep.py
--rw-r--r--   0        0        0    14786 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/iqae.py
--rw-r--r--   0        0        0    15629 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/qcnn.py
--rw-r--r--   0        0        0     2868 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/qft.py
--rw-r--r--   0        0        0    16345 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/qgan.py
--rw-r--r--   0        0        0     6922 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/tsp.py
--rw-r--r--   0        0        0     8166 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/utils.py
--rw-r--r--   0        0        0    26896 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/models/variational.py
--rw-r--r--   0        0        0    21207 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/noise.py
--rw-r--r--   0        0        0    19616 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/noise_model.py
--rw-r--r--   0        0        0    13516 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/optimizers.py
--rw-r--r--   0        0        0     6786 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/parallel.py
--rw-r--r--   0        0        0     4652 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/parameter.py
--rw-r--r--   0        0        0      404 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/__init__.py
--rw-r--r--   0        0        0    18833 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/_clifford_utils.py
--rw-r--r--   0        0        0     9587 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/basis.py
--rw-r--r--   0        0        0    17742 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/clifford.py
--rw-r--r--   0        0        0    10188 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/entanglement.py
--rw-r--r--   0        0        0    32335 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/entropies.py
--rw-r--r--   0        0        0    29696 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/metrics.py
--rw-r--r--   0        0        0    27161 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/quantum_networks.py
--rw-r--r--   0        0        0    47444 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/random_ensembles.py
--rw-r--r--   0        0        0    88497 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/superoperator_transformations.py
--rw-r--r--   0        0        0    17634 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/quantum_info/utils.py
--rw-r--r--   0        0        0    21438 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/result.py
--rw-r--r--   0        0        0     5088 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/solvers.py
--rw-r--r--   0        0        0     5001 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/symbols.py
--rw-r--r--   0        0        0      376 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/__init__.py
--rw-r--r--   0        0        0      604 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/_exceptions.py
--rw-r--r--   0        0        0     1787 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/abstract.py
--rw-r--r--   0        0        0    12514 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/blocks.py
--rw-r--r--   0        0        0    13310 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/decompositions.py
--rw-r--r--   0        0        0     1874 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/optimizer.py
--rw-r--r--   0        0        0    10588 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/pipeline.py
--rw-r--r--   0        0        0    16809 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/placer.py
--rw-r--r--   0        0        0    35659 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/router.py
--rw-r--r--   0        0        0    10104 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/unitary_decompositions.py
--rw-r--r--   0        0        0     8127 2024-03-13 23:08:22.760928 qibo-0.2.6/src/qibo/transpiler/unroller.py
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 qibo-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-04-05 12:05:25.084715 qibo-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3277 2024-04-05 12:05:25.084715 qibo-0.2.7/README.md
+-rw-r--r--   0        0        0     3119 2024-04-05 12:05:25.264717 qibo-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      569 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/__init__.py
+-rw-r--r--   0        0        0     6346 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/__init__.py
+-rw-r--r--   0        0        0    17580 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/_clifford_operations.py
+-rw-r--r--   0        0        0    14561 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/abstract.py
+-rw-r--r--   0        0        0    12600 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/clifford.py
+-rw-r--r--   0        0        0     2780 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/einsum_utils.py
+-rw-r--r--   0        0        0    14381 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/npmatrices.py
+-rw-r--r--   0        0        0    34067 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/numpy.py
+-rw-r--r--   0        0        0     6453 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/pytorch.py
+-rw-r--r--   0        0        0     8588 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/tensorflow.py
+-rw-r--r--   0        0        0    11718 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/callbacks.py
+-rw-r--r--   0        0        0     3097 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/config.py
+-rw-r--r--   0        0        0     8794 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/derivative.py
+-rw-r--r--   0        0        0      136 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/__init__.py
+-rw-r--r--   0        0        0    16946 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/abstract.py
+-rw-r--r--   0        0        0    30848 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/channels.py
+-rw-r--r--   0        0        0    70885 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/gates.py
+-rw-r--r--   0        0        0     9713 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/measurements.py
+-rw-r--r--   0        0        0     6004 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/special.py
+-rw-r--r--   0        0        0      109 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/__init__.py
+-rw-r--r--   0        0        0     4384 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/abstract.py
+-rw-r--r--   0        0        0     5941 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/adiabatic.py
+-rw-r--r--   0        0        0    32100 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/hamiltonians.py
+-rw-r--r--   0        0        0     6695 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/models.py
+-rw-r--r--   0        0        0    13024 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/terms.py
+-rw-r--r--   0        0        0     6875 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/measurements.py
+-rw-r--r--   0        0        0      531 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/__init__.py
+-rw-r--r--   0        0        0    12344 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/_openqasm.py
+-rw-r--r--   0        0        0    52843 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/circuit.py
+-rw-r--r--   0        0        0        0 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/double_bracket.py
+-rw-r--r--   0        0        0     6023 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/utils.py
+-rw-r--r--   0        0        0    13651 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/distcircuit.py
+-rw-r--r--   0        0        0    15947 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/encodings.py
+-rw-r--r--   0        0        0    39662 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/error_mitigation.py
+-rw-r--r--   0        0        0    13481 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/evolution.py
+-rw-r--r--   0        0        0    11600 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/grover.py
+-rw-r--r--   0        0        0     9065 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/hep.py
+-rw-r--r--   0        0        0    14786 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/iqae.py
+-rw-r--r--   0        0        0    16497 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qcnn.py
+-rw-r--r--   0        0        0     2842 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qft.py
+-rw-r--r--   0        0        0    16345 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qgan.py
+-rw-r--r--   0        0        0     6922 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/tsp.py
+-rw-r--r--   0        0        0     8166 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/utils.py
+-rw-r--r--   0        0        0    26669 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/models/variational.py
+-rw-r--r--   0        0        0    21207 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/noise.py
+-rw-r--r--   0        0        0    19616 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/noise_model.py
+-rw-r--r--   0        0        0    13516 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/optimizers.py
+-rw-r--r--   0        0        0     6786 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/parallel.py
+-rw-r--r--   0        0        0     4652 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/parameter.py
+-rw-r--r--   0        0        0      404 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/__init__.py
+-rw-r--r--   0        0        0    18833 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/_clifford_utils.py
+-rw-r--r--   0        0        0     9608 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/basis.py
+-rw-r--r--   0        0        0    17742 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/clifford.py
+-rw-r--r--   0        0        0    10188 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/entanglement.py
+-rw-r--r--   0        0        0    32812 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/entropies.py
+-rw-r--r--   0        0        0    29696 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/metrics.py
+-rw-r--r--   0        0        0    27251 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/quantum_networks.py
+-rw-r--r--   0        0        0    48165 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/random_ensembles.py
+-rw-r--r--   0        0        0    88591 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/superoperator_transformations.py
+-rw-r--r--   0        0        0    17674 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/utils.py
+-rw-r--r--   0        0        0    21454 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/result.py
+-rw-r--r--   0        0        0     5069 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/solvers.py
+-rw-r--r--   0        0        0     4950 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/symbols.py
+-rw-r--r--   0        0        0      376 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/_exceptions.py
+-rw-r--r--   0        0        0     1787 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/abstract.py
+-rw-r--r--   0        0        0    12514 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/blocks.py
+-rw-r--r--   0        0        0    13310 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/decompositions.py
+-rw-r--r--   0        0        0     1874 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/optimizer.py
+-rw-r--r--   0        0        0    10588 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/pipeline.py
+-rw-r--r--   0        0        0    16809 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/placer.py
+-rw-r--r--   0        0        0    35659 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/router.py
+-rw-r--r--   0        0        0    11816 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/unitary_decompositions.py
+-rw-r--r--   0        0        0     8127 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/unroller.py
+-rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 qibo-0.2.7/PKG-INFO
```

### Comparing `qibo-0.2.6/LICENSE` & `qibo-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/README.md` & `qibo-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/pyproject.toml` & `qibo-0.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibo"
-version = "0.2.6"
+version = "0.2.7"
 description = "A framework for quantum computing with hardware acceleration."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibo/"
 documentation = "https://qibo.science/docs/qibo/stable"
@@ -29,14 +29,15 @@
 hyperopt = "^0.2.7"
 tabulate = "^0.9.0"
 openqasm3 = { version = ">=0.5.0", extras = ["parser"] }
 numpy = "^1.26.4"
 networkx = "^3.2.1"
 cvxpy = { version = "^1.4.2", optional = true }
 tensorflow = { version = "^2.14.1,<2.16", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", optional = true }
+torch = { version = "^2.1.1", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
 ipython = "^8.12.0"
@@ -59,20 +60,20 @@
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.2.1"
 cirq = "^1.1.0"
 cvxpy = "^1.3.1"
 ply = "^3.11"
 scikit-learn = "^1.2.1"
-dill = "^0.3.6"
 pytest-cov = "^4.0.0"
 pylint = "^3.0.3"
 matplotlib = "^3.7.0"
-qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
 tensorflow = { version = "^2.14.1,<2.16", markers = "sys_platform == 'linux'" }
+torch = "^2.1.1"
+qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
 qibotn = { git = "https://github.com/qiboteam/qibotn.git" }
 stim = "^1.12.0"
 
 [tool.poe.tasks]
 test = "pytest"
 lint = "pylint src --errors-only"
 lint-warnings = "pylint src --exit-zero"
@@ -96,15 +97,16 @@
 cupy-cuda12x = "^12.0.0"
 cuquantum-python-cu12 = "^23.3.0"
 qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
 qibotn = { git = "https://github.com/qiboteam/qibotn.git" }
 
 [tool.poetry.extras]
 tensorflow = ["tensorflow"]
-qinfo = ["cvxpy"]
+torch = ["torch"]
+qinfo = ["cvxpy", "stim"]
 
 [tool.pylint.reports]
 output-format = "colorized"
 
 [tool.coverage.run]
 omit = ["src/qibo/noise_model.py"]
```

### Comparing `qibo-0.2.6/src/qibo/__init__.py` & `qibo-0.2.7/src/qibo/__init__.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/backends/__init__.py` & `qibo-0.2.7/src/qibo/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 from qibo.backends.abstract import Backend
 from qibo.backends.clifford import CliffordBackend
 from qibo.backends.npmatrices import NumpyMatrices
 from qibo.backends.numpy import NumpyBackend
+from qibo.backends.pytorch import PyTorchBackend
 from qibo.backends.tensorflow import TensorflowBackend
 from qibo.config import log, raise_error
 
 
 def construct_backend(backend, **kwargs):
     if backend == "qibojit":
         from qibojit.backends import CupyBackend, CuQuantumBackend, NumbaBackend
@@ -24,14 +25,17 @@
                 return CupyBackend()
             except (ModuleNotFoundError, ImportError):
                 return NumbaBackend()
 
     elif backend == "tensorflow":
         return TensorflowBackend()
 
+    elif backend == "pytorch":
+        return PyTorchBackend()
+
     elif backend == "numpy":
         return NumpyBackend()
 
     elif backend == "qibolab":  # pragma: no cover
         from qibolab.backends import QibolabBackend  # pylint: disable=E0401
 
         return QibolabBackend(**kwargs)
@@ -72,14 +76,15 @@
     _instance = None
     _dtypes = {"double": "complex128", "single": "complex64"}
     _default_order = [
         {"backend": "qibojit", "platform": "cupy"},
         {"backend": "qibojit", "platform": "numba"},
         {"backend": "tensorflow"},
         {"backend": "numpy"},
+        {"backend": "pytorch"},
     ]
 
     def __new__(cls):
         if cls._instance is not None:
             return cls._instance
 
         backend = os.environ.get("QIBO_BACKEND")
```

### Comparing `qibo-0.2.6/src/qibo/backends/_clifford_operations.py` & `qibo-0.2.7/src/qibo/backends/_clifford_operations.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/backends/abstract.py` & `qibo-0.2.7/src/qibo/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/backends/clifford.py` & `qibo-0.2.7/src/qibo/backends/clifford.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,17 @@
             {"theta": gate.init_kwargs["theta"]} if "theta" in gate.init_kwargs else {}
         )
 
         return operation(symplectic_matrix, *gate.init_args, nqubits, **kwargs)
 
     def apply_channel(self, channel, state, nqubits):
         probabilities = channel.coefficients + (1 - np.sum(channel.coefficients),)
-        index = np.random.choice(range(len(probabilities)), size=1, p=probabilities)[0]
+        index = self.np.random.choice(
+            range(len(probabilities)), size=1, p=probabilities
+        )[0]
         if index != len(channel.gates):
             gate = channel.gates[index]
             state = gate.apply_clifford(self, state, nqubits)
         return state
 
     def execute_circuit(  # pylint: disable=R1710
         self, circuit, initial_state=None, nshots: int = 1000
@@ -325,15 +327,17 @@
         phases = (-1) ** symplectic_matrix[:-1, -1]
         tmp = 1 * symplectic_matrix[:-1, :-1]
         X, Z = tmp[:, :nqubits], tmp[:, nqubits:]
         generators = []
         for x, z in zip(X, Z):
             paulis = [bits_to_gate[f"{zz}{xx}"] for xx, zz in zip(x, z)]
             if return_array:
-                paulis = [self.cast(getattr(gates, p)(0).matrix()) for p in paulis]
+                from qibo import matrices  # pylint: disable=C0415
+
+                paulis = [self.cast(getattr(matrices, p)) for p in paulis]
                 matrix = reduce(self.np.kron, paulis)
                 generators.append(matrix)
             else:
                 generators.append("".join(paulis))
 
         if return_array:
             generators = self.cast(generators)
```

### Comparing `qibo-0.2.6/src/qibo/backends/einsum_utils.py` & `qibo-0.2.7/src/qibo/backends/einsum_utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/backends/npmatrices.py` & `qibo-0.2.7/src/qibo/backends/npmatrices.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,17 @@
     @cached_property
     def TDG(self):
         return self._cast(
             [[1, 0], [0, self.np.exp(-1j * self.np.pi / 4.0)]], dtype=self.dtype
         )
 
     def I(self, n=2):
-        return self._cast(self.np.eye(n, dtype=self.dtype), dtype=self.dtype)
+        # dtype=complex is necessary for pytorch backend,
+        # _cast will take care of casting in the right dtype for all the backends
+        return self._cast(self.np.eye(n, dtype=complex), dtype=self.dtype)
 
     def Align(self, n=2):
         return self._cast(self.I(n), dtype=self.dtype)
 
     def M(self):  # pragma: no cover
         raise_error(NotImplementedError)
```

### Comparing `qibo-0.2.6/src/qibo/backends/numpy.py` & `qibo-0.2.7/src/qibo/backends/numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import collections
+import math
 
 import numpy as np
 
 from qibo import __version__
 from qibo.backends import einsum_utils
 from qibo.backends.abstract import Backend
 from qibo.backends.npmatrices import NumpyMatrices
@@ -89,59 +90,63 @@
         state = self.np.eye(2**nqubits, dtype=self.dtype)
         if normalize is True:
             state /= 2**nqubits
         return state
 
     def plus_state(self, nqubits):
         state = self.np.ones(2**nqubits, dtype=self.dtype)
-        state /= self.np.sqrt(2**nqubits)
+        state /= math.sqrt(2**nqubits)
         return state
 
     def plus_density_matrix(self, nqubits):
         state = self.np.ones(2 * (2**nqubits,), dtype=self.dtype)
         state /= 2**nqubits
         return state
 
     def matrix(self, gate):
         """Convert a gate to its matrix representation in the computational basis."""
         name = gate.__class__.__name__
         _matrix = getattr(self.matrices, name)
-        return _matrix(2 ** len(gate.target_qubits)) if callable(_matrix) else _matrix
+        if callable(_matrix):
+            _matrix = _matrix(2 ** len(gate.target_qubits))
+
+        return self.cast(_matrix, dtype=_matrix.dtype)
 
     def matrix_parametrized(self, gate):
         """Convert a parametrized gate to its matrix representation in the computational basis."""
         name = gate.__class__.__name__
-        return getattr(self.matrices, name)(*gate.parameters)
+        matrix = getattr(self.matrices, name)(*gate.parameters)
+        return self.cast(matrix, dtype=matrix.dtype)
 
     def matrix_fused(self, fgate):
         rank = len(fgate.target_qubits)
-        matrix = np.eye(2**rank, dtype=self.dtype)
+        matrix = np.eye(2**rank)
         for gate in fgate.gates:
             # transfer gate matrix to numpy as it is more efficient for
             # small tensor calculations
             # explicit to_numpy see https://github.com/qiboteam/qibo/issues/928
             gmatrix = self.to_numpy(gate.matrix(self))
             # Kronecker product with identity is needed to make the
             # original matrix have shape (2**rank x 2**rank)
-            eye = np.eye(2 ** (rank - len(gate.qubits)), dtype=self.dtype)
+            eye = np.eye(2 ** (rank - len(gate.qubits)))
             gmatrix = np.kron(gmatrix, eye)
             # Transpose the new matrix indices so that it targets the
             # target qubits of the original gate
             original_shape = gmatrix.shape
             gmatrix = np.reshape(gmatrix, 2 * rank * (2,))
             qubits = list(gate.qubits)
             indices = qubits + [q for q in fgate.target_qubits if q not in qubits]
             indices = np.argsort(indices)
             transpose_indices = list(indices)
             transpose_indices.extend(indices + rank)
             gmatrix = np.transpose(gmatrix, transpose_indices)
             gmatrix = np.reshape(gmatrix, original_shape)
             # fuse the individual gate matrix to the total ``FusedGate`` matrix
             matrix = gmatrix @ matrix
-        return matrix
+        return self.cast(matrix)
 
     def control_matrix(self, gate):
         if len(gate.control_qubits) > 1:
             raise_error(
                 NotImplementedError,
                 "Cannot calculate controlled "
                 "unitary for more than two "
@@ -149,18 +154,21 @@
             )
         matrix = gate.matrix(self)
         shape = matrix.shape
         if shape != (2, 2):
             raise_error(
                 ValueError,
                 "Cannot use ``control_unitary`` method on "
-                "gate matrix of shape {}.".format(shape),
+                + f"gate matrix of shape {shape}.",
             )
         zeros = self.np.zeros((2, 2), dtype=self.dtype)
-        part1 = self.np.concatenate([self.np.eye(2, dtype=self.dtype), zeros], axis=0)
+        zeros = self.cast(zeros, dtype=zeros.dtype)
+        identity = self.np.eye(2, dtype=self.dtype)
+        identity = self.cast(identity, dtype=identity.dtype)
+        part1 = self.np.concatenate([identity, zeros], axis=0)
         part2 = self.np.concatenate([zeros, matrix], axis=0)
         return self.np.concatenate([part1, part2], axis=1)
 
     def apply_gate(self, gate, state, nqubits):
         state = self.cast(state)
         state = self.np.reshape(state, nqubits * (2,))
         matrix = gate.matrix(self)
@@ -173,15 +181,15 @@
             # Apply `einsum` only to the part of the state where all controls
             # are active. This should be `state[-1]`
             state = self.np.reshape(state, (2**ncontrol,) + nactive * (2,))
             opstring = einsum_utils.apply_gate_string(targets, nactive)
             updates = self.np.einsum(opstring, state[-1], matrix)
             # Concatenate the updated part of the state `updates` with the
             # part of of the state that remained unaffected `state[:-1]`.
-            state = self.np.concatenate([state[:-1], updates[self.np.newaxis]], axis=0)
+            state = self.np.concatenate([state[:-1], updates[None]], axis=0)
             state = self.np.reshape(state, nqubits * (2,))
             # Put qubit indices back to their proper places
             state = self.np.transpose(state, einsum_utils.reverse_order(order))
         else:
             matrix = self.np.reshape(matrix, 2 * len(gate.qubits) * (2,))
             opstring = einsum_utils.apply_gate_string(gate.qubits, nqubits)
             state = self.np.einsum(opstring, state, matrix)
@@ -215,49 +223,47 @@
             )
             state11 = state[n - 1, n - 1]
             state11 = self.np.einsum(right, state11, matrixc)
             state11 = self.np.einsum(left, state11, matrix)
 
             state00 = state[range(n - 1)]
             state00 = state00[:, range(n - 1)]
-            state01 = self.np.concatenate(
-                [state00, state01[:, self.np.newaxis]], axis=1
-            )
-            state10 = self.np.concatenate([state10, state11[self.np.newaxis]], axis=0)
-            state = self.np.concatenate([state01, state10[self.np.newaxis]], axis=0)
+            state01 = self.np.concatenate([state00, state01[:, None]], axis=1)
+            state10 = self.np.concatenate([state10, state11[None]], axis=0)
+            state = self.np.concatenate([state01, state10[None]], axis=0)
             state = self.np.reshape(state, 2 * nqubits * (2,))
             state = self.np.transpose(state, einsum_utils.reverse_order(order))
         else:
             matrix = self.np.reshape(matrix, 2 * len(gate.qubits) * (2,))
             matrixc = self.np.conj(matrix)
             left, right = einsum_utils.apply_gate_density_matrix_string(
                 gate.qubits, nqubits
             )
             state = self.np.einsum(right, state, matrixc)
             state = self.np.einsum(left, state, matrix)
         return self.np.reshape(state, 2 * (2**nqubits,))
 
     def apply_gate_half_density_matrix(self, gate, state, nqubits):
         state = self.cast(state)
-        state = np.reshape(state, 2 * nqubits * (2,))
+        state = self.np.reshape(state, 2 * nqubits * (2,))
         matrix = gate.matrix(self)
         if gate.is_controlled_by:  # pragma: no cover
             raise_error(
                 NotImplementedError,
                 "Gate density matrix half call is "
                 "not implemented for ``controlled_by``"
                 "gates.",
             )
         else:
-            matrix = np.reshape(matrix, 2 * len(gate.qubits) * (2,))
+            matrix = self.np.reshape(matrix, 2 * len(gate.qubits) * (2,))
             left, _ = einsum_utils.apply_gate_density_matrix_string(
                 gate.qubits, nqubits
             )
-            state = np.einsum(left, state, matrix)
-        return np.reshape(state, 2 * (2**nqubits,))
+            state = self.np.einsum(left, state, matrix)
+        return self.np.reshape(state, 2 * (2**nqubits,))
 
     def apply_channel(self, channel, state, nqubits):
         probabilities = channel.coefficients + (1 - np.sum(channel.coefficients),)
         index = self.sample_shots(probabilities, 1)[0]
         if index != len(channel.gates):
             gate = channel.gates[index]
             state = self.apply_gate(gate, state, nqubits)
@@ -269,19 +275,20 @@
         for coeff, gate in zip(channel.coefficients, channel.gates):
             new_state += coeff * self.apply_gate_density_matrix(gate, state, nqubits)
         return new_state
 
     def _append_zeros(self, state, qubits, results):
         """Helper method for collapse."""
         for q, r in zip(qubits, results):
-            state = self.np.expand_dims(state, axis=q)
-            if r:
-                state = self.np.concatenate([self.np.zeros_like(state), state], axis=q)
-            else:
-                state = self.np.concatenate([state, self.np.zeros_like(state)], axis=q)
+            state = self.np.expand_dims(state, q)
+            state = (
+                self.np.concatenate([self.np.zeros_like(state), state], q)
+                if r == 1
+                else self.np.concatenate([state, self.np.zeros_like(state)], q)
+            )
         return state
 
     def collapse_state(self, state, qubits, shot, nqubits, normalize=True):
         state = self.cast(state)
         shape = state.shape
         binshot = self.samples_to_binary(shot, len(qubits))[0]
         state = self.np.reshape(state, nqubits * (2,))
@@ -320,15 +327,15 @@
         state = self.cast(state)
         shape = state.shape
         q = gate.target_qubits[0]
         p_0, p_1 = gate.init_kwargs["p_0"], gate.init_kwargs["p_1"]
         trace = self.partial_trace_density_matrix(state, (q,), nqubits)
         trace = self.np.reshape(trace, 2 * (nqubits - 1) * (2,))
         zero = self.zero_density_matrix(1)
-        zero = self.np.tensordot(trace, zero, axes=0)
+        zero = self.np.tensordot(trace, zero, 0)
         order = list(range(2 * nqubits - 2))
         order.insert(q, 2 * nqubits - 2)
         order.insert(q + nqubits, 2 * nqubits - 1)
         zero = self.np.reshape(self.np.transpose(zero, order), shape)
         state = (1 - p_0 - p_1) * state + p_0 * zero
         return state + p_1 * self.apply_gate_density_matrix(X(q), zero, nqubits)
 
@@ -343,15 +350,15 @@
         shape = state.shape
         q = gate.target_qubits
         lam = gate.init_kwargs["lam"]
         trace = self.partial_trace_density_matrix(state, q, nqubits)
         trace = self.np.reshape(trace, 2 * (nqubits - len(q)) * (2,))
         identity = self.identity_density_matrix(len(q))
         identity = self.np.reshape(identity, 2 * len(q) * (2,))
-        identity = self.np.tensordot(trace, identity, axes=0)
+        identity = self.np.tensordot(trace, identity, 0)
         qubits = list(range(nqubits))
         for j in q:
             qubits.pop(qubits.index(j))
         qubits.sort()
         qubits += list(q)
         qubit_1 = list(range(nqubits - len(q))) + list(
             range(2 * (nqubits - len(q)), 2 * nqubits - len(q))
@@ -365,14 +372,15 @@
             qj = [qj[qubits.index(i)] for i in range(len(qubits))]
             order += qj
         identity = self.np.reshape(self.np.transpose(identity, order), shape)
         state = (1 - lam) * state + lam * identity
         return state
 
     def execute_circuit(self, circuit, initial_state=None, nshots=1000):
+
         if isinstance(initial_state, type(circuit)):
             if not initial_state.density_matrix == circuit.density_matrix:
                 raise_error(
                     ValueError,
                     f"""Cannot set circuit with density_matrix {initial_state.density_matrix} as
                       initial state for circuit with density_matrix {circuit.density_matrix}.""",
                 )
@@ -382,14 +390,16 @@
                 raise_error(
                     ValueError,
                     f"""Cannot set circuit with accelerators {initial_state.density_matrix} as
                       initial state for circuit with accelerators {circuit.density_matrix}.""",
                 )
             else:
                 return self.execute_circuit(initial_state + circuit, None, nshots)
+        elif initial_state is not None:
+            initial_state = self.cast(initial_state)
 
         if circuit.repeated_execution:
             if circuit.measurements or circuit.has_collapse:
                 return self.execute_circuit_repeated(circuit, nshots, initial_state)
             else:
                 raise RuntimeError(
                     "Attempting to perform noisy simulation with `density_matrix=False` and no Measurement gate in the Circuit. If you wish to retrieve the statistics of the outcomes please include measurements in the circuit, otherwise set `density_matrix=True` to recover the final state."
@@ -461,15 +471,15 @@
         )
 
     def execute_circuit_repeated(self, circuit, nshots, initial_state=None):
         """
         Execute the circuit `nshots` times to retrieve probabilities, frequencies
         and samples. Note that this method is called only if a unitary channel
         is present in the circuit (i.e. noisy simulation) and `density_matrix=False`, or
-        if some collapsing measuremnt is performed.
+        if some collapsing measurement is performed.
         """
 
         if (
             circuit.has_collapse
             and not circuit.measurements
             and not circuit.density_matrix
         ):
@@ -518,23 +528,22 @@
             if circuit.measurements:
                 result = CircuitResult(
                     state, circuit.measurements, backend=self, nshots=1
                 )
                 sample = result.samples()[0]
                 results.append(sample)
                 if not circuit.density_matrix:
-                    samples.append("".join([str(s) for s in sample]))
+                    samples.append("".join([str(int(s)) for s in sample]))
                 for gate in circuit.measurements:
                     gate.result.reset()
 
         if circuit.density_matrix:  # this implies also it has_collapse
             assert circuit.has_collapse
-            final_state = np.mean(self.to_numpy(final_states), 0)
+            final_state = self.cast(np.mean(self.to_numpy(final_states), 0))
             if circuit.measurements:
-                qubits = [q for m in circuit.measurements for q in m.target_qubits]
                 final_result = CircuitResult(
                     final_state,
                     circuit.measurements,
                     backend=self,
                     samples=self.aggregate_shots(results),
                     nshots=nshots,
                 )
@@ -602,15 +611,15 @@
                 unmeasured.append(i)
         return self.np.transpose(probs, [reduced.get(i) for i in qubits])
 
     def calculate_probabilities(self, state, qubits, nqubits):
         rtype = self.np.real(state).dtype
         unmeasured_qubits = tuple(i for i in range(nqubits) if i not in qubits)
         state = self.np.reshape(self.np.abs(state) ** 2, nqubits * (2,))
-        probs = self.np.sum(state.astype(rtype), axis=unmeasured_qubits)
+        probs = self.np.sum(self.cast(state, dtype=rtype), axis=unmeasured_qubits)
         return self._order_probabilities(probs, qubits, nqubits).ravel()
 
     def calculate_probabilities_density_matrix(self, state, qubits, nqubits):
         order = tuple(sorted(qubits))
         order += tuple(i for i in range(nqubits) if i not in qubits)
         order = order + tuple(i + nqubits for i in order)
         shape = 2 * (2 ** len(qubits), 2 ** (nqubits - len(qubits)))
@@ -625,62 +634,66 @@
 
     def sample_shots(self, probabilities, nshots):
         return self.np.random.choice(
             range(len(probabilities)), size=nshots, p=probabilities
         )
 
     def aggregate_shots(self, shots):
-        return self.np.array(shots, dtype=shots[0].dtype)
+        return self.cast(shots, dtype=shots[0].dtype)
 
     def samples_to_binary(self, samples, nqubits):
-        qrange = self.np.arange(nqubits - 1, -1, -1, dtype="int32")
-        return self.np.mod(self.np.right_shift(samples[:, self.np.newaxis], qrange), 2)
+        qrange = self.np.arange(nqubits - 1, -1, -1, dtype=self.np.int32)
+        return self.np.mod(
+            self.np.right_shift(self.cast(samples[:, None], dtype="int32"), qrange), 2
+        )
 
     def samples_to_decimal(self, samples, nqubits):
-        qrange = self.np.arange(nqubits - 1, -1, -1, dtype="int32")
-        qrange = (2**qrange)[:, self.np.newaxis]
-        return self.np.matmul(self.to_numpy(samples), qrange)[:, 0]
+        qrange = self.np.arange(nqubits - 1, -1, -1, dtype=self.np.int32)
+        qrange = (2**qrange)[:, None]
+        return self.np.matmul(samples, qrange)[:, 0]
 
     def calculate_frequencies(self, samples):
-        res, counts = self.np.unique(samples, return_counts=True)
-        res, counts = self.np.array(res), self.np.array(counts)
-        return collections.Counter({k: v for k, v in zip(res, counts)})
+        # Samples are a list of strings so there is no advantage in using other backends
+        res, counts = np.unique(samples, return_counts=True)
+        return collections.Counter(dict(zip(res, counts)))
 
     def update_frequencies(self, frequencies, probabilities, nsamples):
         samples = self.sample_shots(probabilities, nsamples)
         res, counts = self.np.unique(samples, return_counts=True)
         frequencies[res] += counts
         return frequencies
 
     def sample_frequencies(self, probabilities, nshots):
         from qibo.config import SHOT_BATCH_SIZE
 
         nprobs = probabilities / self.np.sum(probabilities)
-        frequencies = self.np.zeros(len(nprobs), dtype="int64")
+        frequencies = self.np.zeros(len(nprobs), dtype=self.np.int64)
         for _ in range(nshots // SHOT_BATCH_SIZE):
             frequencies = self.update_frequencies(frequencies, nprobs, SHOT_BATCH_SIZE)
         frequencies = self.update_frequencies(
             frequencies, nprobs, nshots % SHOT_BATCH_SIZE
         )
-        return collections.Counter({i: f for i, f in enumerate(frequencies) if f > 0})
+        return collections.Counter(
+            {i: int(f) for i, f in enumerate(frequencies) if f > 0}
+        )
 
     def apply_bitflips(self, noiseless_samples, bitflip_probabilities):
-        fprobs = self.np.array(bitflip_probabilities, dtype="float64")
-        sprobs = self.np.random.random(noiseless_samples.shape)
-        flip_0 = self.np.array(sprobs < fprobs[0], dtype=noiseless_samples.dtype)
-        flip_1 = self.np.array(sprobs < fprobs[1], dtype=noiseless_samples.dtype)
+        fprobs = self.cast(bitflip_probabilities, dtype="float64")
+        sprobs = self.cast(np.random.random(noiseless_samples.shape), dtype="float64")
+        flip_0 = self.cast(sprobs < fprobs[0], dtype=noiseless_samples.dtype)
+        flip_1 = self.cast(sprobs < fprobs[1], dtype=noiseless_samples.dtype)
         noisy_samples = noiseless_samples + (1 - noiseless_samples) * flip_0
         noisy_samples = noisy_samples - noiseless_samples * flip_1
         return noisy_samples
 
     def partial_trace(self, state, qubits, nqubits):
         state = self.cast(state)
         state = self.np.reshape(state, nqubits * (2,))
         axes = 2 * [list(qubits)]
-        rho = self.np.tensordot(state, self.np.conj(state), axes=axes)
+        rho = self.np.tensordot(state, self.np.conj(state), axes)
         shape = 2 * (2 ** (nqubits - len(qubits)),)
         return self.np.reshape(rho, shape)
 
     def partial_trace_density_matrix(self, state, qubits, nqubits):
         state = self.cast(state)
         state = self.np.reshape(state, 2 * nqubits * (2,))
 
@@ -691,29 +704,27 @@
 
         state = self.np.transpose(state, order)
         state = self.np.reshape(state, shape)
         return self.np.einsum("abac->bc", state)
 
     def calculate_norm(self, state, order=2):
         state = self.cast(state)
-        return self.np.linalg.norm(state, ord=order)
+        return self.np.linalg.norm(state, order)
 
     def calculate_norm_density_matrix(self, state, order="nuc"):
         state = self.cast(state)
         return self.np.linalg.norm(state, ord=order)
 
     def calculate_overlap(self, state1, state2):
-        state1 = self.cast(state1)
-        state2 = self.cast(state2)
-        return self.np.abs(self.np.sum(self.np.conj(state1) * state2))
+        return self.np.abs(self.np.sum(np.conj(self.cast(state1)) * self.cast(state2)))
 
     def calculate_overlap_density_matrix(self, state1, state2):
-        state1 = self.cast(state1)
-        state2 = self.cast(state2)
-        return self.np.trace(self.np.transpose(self.np.conj(state1)) @ state2)
+        return self.np.trace(
+            self.np.matmul(self.np.conj(self.cast(state1)).T, self.cast(state2))
+        )
 
     def calculate_eigenvalues(self, matrix, k=6):
         if self.issparse(matrix):
             log.warning(
                 "Calculating sparse matrix eigenvectors because "
                 "sparse modules do not provide ``eigvals`` method."
             )
@@ -733,50 +744,45 @@
     def calculate_matrix_exp(self, a, matrix, eigenvectors=None, eigenvalues=None):
         if eigenvectors is None or self.issparse(matrix):
             if self.issparse(matrix):
                 from scipy.sparse.linalg import expm
             else:
                 from scipy.linalg import expm
             return expm(-1j * a * matrix)
-        else:
-            expd = self.np.diag(self.np.exp(-1j * a * eigenvalues))
-            ud = self.np.transpose(self.np.conj(eigenvectors))
-            return self.np.matmul(eigenvectors, self.np.matmul(expd, ud))
+        expd = self.np.diag(self.np.exp(-1j * a * eigenvalues))
+        ud = self.np.transpose(np.conj(eigenvectors))
+        return self.np.matmul(eigenvectors, self.np.matmul(expd, ud))
 
     def calculate_expectation_state(self, hamiltonian, state, normalize):
         statec = self.np.conj(state)
         hstate = hamiltonian @ state
         ev = self.np.real(self.np.sum(statec * hstate))
         if normalize:
-            norm = self.np.sum(self.np.square(self.np.abs(state)))
-            ev = ev / norm
+            ev /= self.np.sum(self.np.square(self.np.abs(state)))
         return ev
 
     def calculate_expectation_density_matrix(self, hamiltonian, state, normalize):
-        ev = self.np.real(self.np.trace(hamiltonian @ state))
+        ev = self.np.real(self.np.trace(self.cast(hamiltonian @ state)))
         if normalize:
             norm = self.np.real(self.np.trace(state))
-            ev = ev / norm
+            ev /= norm
         return ev
 
+    # TODO: remove this method
     def calculate_hamiltonian_matrix_product(self, matrix1, matrix2):
-        return self.np.dot(matrix1, matrix2)
+        return matrix1 @ matrix2
 
+    # TODO: remove this method
     def calculate_hamiltonian_state_product(self, matrix, state):
-        rank = len(tuple(state.shape))
-        state = self.cast(state)
-        if rank == 1:  # vector
-            return matrix.dot(state[:, np.newaxis])[:, 0]
-        elif rank == 2:  # matrix
-            return matrix.dot(state)
-        else:
+        if len(tuple(state.shape)) > 2:
             raise_error(
                 ValueError,
-                "Cannot multiply Hamiltonian with " "rank-{} tensor.".format(rank),
+                f"Cannot multiply Hamiltonian with rank-{len(tuple(state.shape))} tensor.",
             )
+        return matrix @ state
 
     def assert_allclose(self, value, target, rtol=1e-7, atol=0.0):
         if isinstance(value, CircuitResult) or isinstance(value, QuantumState):
             value = value.state()
         if isinstance(target, CircuitResult) or isinstance(target, QuantumState):
             target = target.state()
         value = self.to_numpy(value)
```

### Comparing `qibo-0.2.6/src/qibo/backends/tensorflow.py` & `qibo-0.2.7/src/qibo/backends/tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,34 +195,34 @@
         if rank == 1:  # vector
             return self.np.matmul(matrix, state[:, self.np.newaxis])[:, 0]
         elif rank == 2:  # matrix
             return self.np.matmul(matrix, state)
         else:
             raise_error(
                 ValueError,
-                "Cannot multiply Hamiltonian with " "rank-{} tensor.".format(rank),
+                f"Cannot multiply Hamiltonian with rank-{rank} tensor.",
             )
 
     def test_regressions(self, name):
         if name == "test_measurementresult_apply_bitflips":
             return [
-                [4, 0, 0, 1, 0, 2, 2, 4, 4, 0],
-                [4, 0, 0, 1, 0, 2, 2, 4, 4, 0],
-                [4, 0, 0, 1, 0, 0, 0, 4, 4, 0],
-                [4, 0, 0, 0, 0, 0, 0, 4, 4, 0],
+                [4, 0, 0, 1, 0, 0, 1, 0, 0, 0],
+                [0, 1, 1, 2, 1, 1, 4, 0, 0, 4],
+                [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0, 4, 0, 0, 0, 4],
             ]
         elif name == "test_probabilistic_measurement":
             if "GPU" in self.device:  # pragma: no cover
                 return {0: 273, 1: 233, 2: 242, 3: 252}
             else:
                 return {0: 271, 1: 239, 2: 242, 3: 248}
         elif name == "test_unbalanced_probabilistic_measurement":
             if "GPU" in self.device:  # pragma: no cover
                 return {0: 196, 1: 153, 2: 156, 3: 495}
             else:
                 return {0: 168, 1: 188, 2: 154, 3: 490}
         elif name == "test_post_measurement_bitflips_on_circuit":
             return [
                 {5: 30},
-                {5: 16, 7: 10, 6: 2, 3: 1, 4: 1},
-                {3: 6, 5: 6, 7: 5, 2: 4, 4: 3, 0: 2, 1: 2, 6: 2},
+                {5: 12, 7: 6, 4: 6, 1: 5, 6: 1},
+                {3: 7, 6: 4, 2: 4, 7: 4, 0: 4, 5: 3, 4: 2, 1: 2},
             ]
```

### Comparing `qibo-0.2.6/src/qibo/callbacks.py` & `qibo-0.2.7/src/qibo/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,21 @@
         self._results.append(x)
 
     def extend(self, x):
         self._results.extend(x)
 
     def __getitem__(self, k):
         if not isinstance(k, (int, slice, list, tuple)):
-            raise_error(IndexError, "Unrecognized type for index {}.".format(k))
+            raise_error(IndexError, f"Unrecognized type for index {k}.")
 
         if isinstance(k, int) and k >= len(self._results):
             raise_error(
                 IndexError,
-                "Attempting to access callbacks {} run but "
-                "the callback has been used in {} executions."
-                "".format(k, len(self._results)),
+                f"Attempting to access callbacks {k} run but "
+                + f"the callback has been used in {len(self._results)} executions.",
             )
 
         return self._results[k]
 
     def apply(self, backend, state):  # pragma: no cover
         pass
 
@@ -304,21 +303,18 @@
     """
 
     def __init__(self, mode: Union[str, int] = "gap", check_degenerate: bool = True):
         super().__init__()
         if not isinstance(mode, (int, str)):
             raise_error(
                 TypeError,
-                "Gap callback mode should be integer or "
-                "string but is {}.".format(type(mode)),
+                f"Gap callback mode should be integer or string but is {type(mode)}.",
             )
         elif isinstance(mode, str) and mode != "gap":
-            raise_error(
-                ValueError, "Unsupported mode {} for gap callback." "".format(mode)
-            )
+            raise_error(ValueError, f"Unsupported mode {mode} for gap callback.")
         self.mode = mode
         self.check_degenerate = check_degenerate
         self.evolution = None
 
     def apply(self, backend, state):
         from qibo.config import EIGVAL_CUTOFF, log
 
@@ -346,16 +342,15 @@
             return gap
 
         while backend.np.less(gap, EIGVAL_CUTOFF):
             gap = backend.np.real(eigvals[excited] - eigvals[0])
             excited += 1
         if excited > 1:
             log.warning(
-                "The Hamiltonian is degenerate. Using eigenvalue {} "
-                "to calculate gap.".format(excited)
+                f"The Hamiltonian is degenerate. Using eigenvalue {excited} to calculate gap."
             )
         self.append(gap)
         return gap
 
     def apply_density_matrix(self, backend, state):
         raise_error(
             NotImplementedError,
```

### Comparing `qibo-0.2.6/src/qibo/config.py` & `qibo-0.2.7/src/qibo/config.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/derivative.py` & `qibo-0.2.7/src/qibo/derivative.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+from qibo.backends.pytorch import PyTorchBackend
 from qibo.config import raise_error
 from qibo.hamiltonians.abstract import AbstractHamiltonian
 
 
 def parameter_shift(
     circuit,
     hamiltonian,
@@ -98,14 +99,20 @@
         raise_error(
             TypeError,
             "hamiltonian must be a qibo.hamiltonians.Hamiltonian or qibo.hamiltonians.SymbolicHamiltonian object",
         )
 
     # inheriting hamiltonian's backend
     backend = hamiltonian.backend
+    # TODO: make this work wih pytorch backend
+    if isinstance(backend, PyTorchBackend):
+        raise_error(
+            NotImplementedError,
+            "PyTorchBackend for the parameter shift rule is not supported.",
+        )
 
     # getting the gate's type
     gate = circuit.associate_gates_with_parameters()[parameter_index]
 
     # getting the generator_eigenvalue
     generator_eigenval = gate.generator_eigenvalue()
```

### Comparing `qibo-0.2.6/src/qibo/gates/abstract.py` & `qibo-0.2.7/src/qibo/gates/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,32 @@
         self.name = None
         self.draw_label = None
         self.is_controlled_by = False
         # args for creating gate
         self.init_args = []
         self.init_kwargs = {}
 
-        self.clifford = False
         self.unitary = False
-        self._target_qubits = tuple()
-        self._control_qubits = set()
-        self._parameters = tuple()
+        self._target_qubits = ()
+        self._control_qubits = ()
+        self._parameters = ()
         config.ALLOW_SWITCHERS = False
 
         self.symbolic_parameters = {}
 
         # for distributed circuits
         self.device_gates = set()
         self.original_gate = None
 
     @property
+    def clifford(self):
+        """Return boolean value representing if a Gate is Clifford or not."""
+        return False
+
+    @property
     def raw(self) -> dict:
         """Serialize to dictionary.
 
         The values used in the serialization should be compatible with a
         JSON dump (or any other one supporting a minimal set of scalar
         types). Though the specific implementation is up to the specific
         gate.
@@ -154,21 +158,21 @@
             raise_error(
                 ValueError,
                 f"Target qubit {repeated} was given twice for gate {self.__class__.__name__}.",
             )
 
     def _set_control_qubits(self, qubits: Sequence[int]):
         """Helper method for setting control qubits."""
-        self._control_qubits = set(qubits)
-        if len(self._control_qubits) != len(qubits):
+        if len(set(qubits)) != len(qubits):
             repeated = self._find_repeated(qubits)
             raise_error(
                 ValueError,
                 f"Control qubit {repeated} was given twice for gate {self.__class__.__name__}.",
             )
+        self._control_qubits = qubits
 
     @target_qubits.setter
     def target_qubits(self, qubits: Sequence[int]):
         """Sets target qubits tuple."""
         self._set_target_qubits(qubits)
         self._check_control_target_overlap()
 
@@ -200,19 +204,20 @@
             if qubit in temp_set:
                 return qubit
             temp_set.add(qubit)
 
     def _check_control_target_overlap(self):
         """Checks that there are no qubits that are both target and
         controls."""
-        common = set(self._target_qubits) & self._control_qubits
+        control_and_target = self._control_qubits + self._target_qubits
+        common = len(set(control_and_target)) != len(control_and_target)
         if common:
             raise_error(
                 ValueError,
-                f"{common} qubits are both targets and controls "
+                f"{set(self._target_qubits) & set(self._control_qubits)} qubits are both targets and controls "
                 + f"for gate {self.__class__.__name__}.",
             )
 
     @property
     def parameters(self):
         """Returns a tuple containing the current value of gate's
         parameters."""
```

### Comparing `qibo-0.2.6/src/qibo/gates/channels.py` & `qibo-0.2.7/src/qibo/gates/channels.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/gates/gates.py` & `qibo-0.2.7/src/qibo/gates/gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "h"
         self.draw_label = "H"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "h"
 
 
 class X(Gate):
     """The Pauli-:math:`X` gate.
 
@@ -54,18 +57,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "x"
         self.draw_label = "X"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "x"
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CNOT and Toffoli if there is one or two controls."""
         if len(q) == 1:
@@ -167,18 +173,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "y"
         self.draw_label = "Y"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "y"
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CY if there is only one control."""
         if len(q) == 1:
@@ -211,18 +220,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "z"
         self.draw_label = "Z"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "z"
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CZ if there is only one control."""
         if len(q) == 1:
@@ -252,18 +264,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "sx"
         self.draw_label = "SX"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "sx"
 
     def decompose(self):
         """Decomposition of :math:`\\sqrt{X}` up to global phase.
 
         A global phase difference exists between the definitions of
@@ -299,18 +314,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "sxdg"
         self.draw_label = "SXDG"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "sxdg"
 
     def decompose(self):
         """Decomposition of :math:`(\\sqrt{X})^{\\dagger}` up to global phase.
 
         A global phase difference exists between the definitions of
@@ -346,18 +364,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "s"
         self.draw_label = "S"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "s"
 
     def _dagger(self):
         return SDG(*self.init_args)
 
 
@@ -378,18 +399,21 @@
 
     def __init__(self, q):
         super().__init__()
         self.name = "sdg"
         self.draw_label = "SDG"
         self.target_qubits = (q,)
         self.init_args = [q]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "sdg"
 
     def _dagger(self):
         return S(*self.init_args)
 
 
@@ -464,18 +488,21 @@
 
     def __init__(self, *q):
         super().__init__()
         self.name = "id"
         self.draw_label = "I"
         self.target_qubits = tuple(q)
         self.init_args = q
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "id"
 
 
 class Align(Gate):
     """Aligns proceeding qubit operations and (optionally) waits ``delay`` amount of time.
 
@@ -498,14 +525,19 @@
         self.delay = delay
         self.draw_label = f"A({delay})"
         self.init_args = q
         self.init_kwargs = {"delay": delay}
         self.target_qubits = tuple(q)
 
 
+def _is_clifford_given_angle(angle):
+    """Helper function to update Clifford boolean condition according to the given angle ``angle``."""
+    return isinstance(angle, (float, int)) and (angle % (np.pi / 2)).is_integer()
+
+
 class _Rn_(ParametrizedGate):
     """Abstract class for defining the RX, RY and RZ rotations.
 
     Args:
         q (int): the qubit id number.
         theta (float): the rotation angle.
         trainable (bool): whether gate parameters can be updated using
@@ -520,21 +552,22 @@
         self.target_qubits = (q,)
         self.unitary = True
 
         self.initparams = theta
         if isinstance(theta, Parameter):
             theta = theta()
 
-        if isinstance(theta, (float, int)) and (theta % (np.pi / 2)).is_integer():
-            self.clifford = True
-
         self.parameters = theta
         self.init_args = [q]
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
+    @property
+    def clifford(self):
+        return _is_clifford_given_angle(self.parameters[0])
+
     def _dagger(self) -> "Gate":
         """"""
         return self.__class__(
             self.target_qubits[0], -self.parameters[0]
         )  # pylint: disable=E1130
 
     @Gate.check_controls
@@ -970,18 +1003,21 @@
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "cx"
         self.draw_label = "X"
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "cx"
 
     def decompose(self, *free, use_toffolis: bool = True) -> List[Gate]:
         q0, q1 = self.control_qubits[0], self.target_qubits[0]
         return [self.__class__(q0, q1)]
 
@@ -1007,18 +1043,21 @@
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "cy"
         self.draw_label = "Y"
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "cy"
 
     def decompose(self) -> List[Gate]:
         """Decomposition of :math:`\\text{CY}` gate.
 
         Decompose :math:`\\text{CY}` gate into :class:`qibo.gates.SDG` in
@@ -1053,18 +1092,21 @@
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "cz"
         self.draw_label = "Z"
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "cz"
 
     def decompose(self) -> List[Gate]:
         """Decomposition of :math:`\\text{CZ}` gate.
 
         Decompose :math:`\\text{CZ}` gate into :class:`qibo.gates.H` in
@@ -1182,20 +1224,21 @@
         super().__init__(trainable)
         self.name = None
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.parameters = theta
         self.unitary = True
 
-        if isinstance(theta, (float, int)) and (theta % np.pi).is_integer():
-            self.clifford = True
-
         self.init_args = [q0, q1]
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
+    @property
+    def clifford(self):
+        return _is_clifford_given_angle(self.parameters[0])
+
     def _dagger(self) -> "Gate":
         """"""
         q0 = self.control_qubits[0]
         q1 = self.target_qubits[0]
         theta = -self.parameters[0]
         return self.__class__(q0, q1, theta)  # pylint: disable=E1130
 
@@ -1480,18 +1523,21 @@
 
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "swap"
         self.draw_label = "x"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "swap"
 
 
 class iSWAP(Gate):
     """The iSWAP gate.
 
@@ -1512,18 +1558,21 @@
 
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "iswap"
         self.draw_label = "i"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "iswap"
 
 
 class SiSWAP(Gate):
     """The :math:`\\sqrt{\\text{iSWAP}}` gate.
 
@@ -1604,18 +1653,21 @@
 
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "fswap"
         self.draw_label = "fx"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
     @property
+    def clifford(self):
+        return True
+
+    @property
     def qasm_label(self):
         return "fswap"
 
     def decompose(self, *free, use_toffolis: bool = True) -> List[Gate]:
         """"""
         q0, q1 = self.target_qubits
         return [X(q1)] + GIVENS(q0, q1, np.pi / 2).decompose() + [X(q0)]
@@ -1750,15 +1802,15 @@
 
     @Gate.parameters.setter
     def parameters(self, x):
         shape = tuple(x[0].shape)
         if shape != (2, 2):
             raise_error(
                 ValueError,
-                "Invalid rotation shape {} for generalized " "fSim gate".format(shape),
+                f"Invalid rotation shape {shape} for generalized fSim gate",
             )
         ParametrizedGate.parameters.fset(self, x)  # pylint: disable=no-member
 
 
 class _Rnn_(ParametrizedGate):
     """Abstract class for defining the RXX, RYY, RZZ, and RZX rotations.
 
@@ -2154,17 +2206,20 @@
 
     def __init__(self, q0, q1):
         super().__init__()
         self.name = "ecr"
         self.draw_label = "ECR"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
-        self.clifford = True
         self.unitary = True
 
+    @property
+    def clifford(self):
+        return True
+
     def decompose(self, *free, use_toffolis: bool = True) -> List[Gate]:
         """Decomposition of :math:`\\textup{ECR}` gate up to global phase.
 
         A global phase difference exists between the definitions of
         :math:`\\textup{ECR}` and this decomposition. More precisely,
 
         .. math::
@@ -2311,43 +2366,69 @@
     def __init__(
         self, unitary, *q, trainable=True, name: str = None, check_unitary: bool = True
     ):
         super().__init__(trainable)
         self.name = "Unitary" if name is None else name
         self.draw_label = "U"
         self.target_qubits = tuple(q)
+        self._clifford = False
 
         # TODO: Check that given ``unitary`` has proper shape?
         self.parameter_names = "u"
         self._parameters = (unitary,)
         self.nparams = 4 ** len(self.target_qubits)
 
         self.init_args = [unitary] + list(q)
         self.init_kwargs = {
             "name": name,
             "check_unitary": check_unitary,
             "trainable": trainable,
         }
 
-        # checking unitarity without invoking any backend
         if check_unitary:
-            product = np.transpose(np.conj(unitary)) @ unitary
-            sums = all(np.abs(1 - np.sum(product, axis=1)) < PRECISION_TOL)
-            diagonal = all(np.abs(1 - np.diag(product)) < PRECISION_TOL)
+            if unitary.__class__.__name__ == "Tensor":
+                import torch  # pylint: disable=C0145
 
-            self.unitary = True if sums and diagonal else False
-            del sums, diagonal, product
+                diag_function = torch.diag
+                all_function = torch.all
+                conj_function = torch.conj
+                transpose_function = torch.transpose
+            else:
+                diag_function = np.diag
+                all_function = np.all
+                conj_function = np.conj
+                transpose_function = np.transpose
+
+            product = transpose_function(conj_function(unitary), (1, 0)) @ unitary
+            diagonals = all(np.abs(1 - diag_function(product)) < PRECISION_TOL)
+            off_diagonals = bool(
+                all_function(
+                    np.abs(product - diag_function(diag_function(product)))
+                    < PRECISION_TOL
+                )
+            )
+
+            self.unitary = True if diagonals and off_diagonals else False
+            del diagonals, off_diagonals, product
 
     @Gate.parameters.setter
     def parameters(self, x):
         shape = self.parameters[0].shape
         self._parameters = (np.reshape(x, shape),)
         for gate in self.device_gates:  # pragma: no cover
             gate.parameters = x
 
+    @property
+    def clifford(self):
+        return self._clifford
+
+    @clifford.setter
+    def clifford(self, value):
+        self._clifford = value
+
     def on_qubits(self, qubit_map):
         args = [self.init_args[0]]
         args.extend(qubit_map.get(i) for i in self.target_qubits)
         gate = self.__class__(*args, **self.init_kwargs)
         if self.is_controlled_by:
             controls = (qubit_map.get(i) for i in self.control_qubits)
             gate = gate.controlled_by(*controls)
```

### Comparing `qibo-0.2.6/src/qibo/gates/measurements.py` & `qibo-0.2.7/src/qibo/gates/measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             if diff:
                 raise_error(
                     KeyError,
                     f"Bitflip map contains {diff} qubits that are not measured.",
                 )
             return tuple(probs[q] if q in probs else 0.0 for q in qubits)
 
-        raise_error(TypeError, "Invalid type {} of bitflip map.".format(probs))
+        raise_error(TypeError, f"Invalid type {probs} of bitflip map.")
 
     def _get_bitflip_map(self, p: Optional["ProbsType"] = None) -> Dict[int, float]:
         """Creates dictionary with bitflip probabilities."""
         if p is None:
             return {q: 0 for q in self.qubits}
         pt = self._get_bitflip_tuple(self.qubits, p)
         return dict(zip(self.qubits, pt))
```

### Comparing `qibo-0.2.6/src/qibo/gates/special.py` & `qibo-0.2.7/src/qibo/gates/special.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/hamiltonians/abstract.py` & `qibo-0.2.7/src/qibo/hamiltonians/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,17 @@
     @property
     def nqubits(self):
         return self._nqubits
 
     @nqubits.setter
     def nqubits(self, n):
         if not isinstance(n, int):
-            raise_error(
-                RuntimeError, "nqubits must be an integer but is " "{}.".format(type(n))
-            )
+            raise_error(RuntimeError, f"nqubits must be an integer but is {type(n)}.")
         if n < 1:
-            raise_error(
-                ValueError, "nqubits must be a positive integer but is " "{}".format(n)
-            )
+            raise_error(ValueError, f"nqubits must be a positive integer but is {n}")
         self._nqubits = n
 
     @abstractmethod
     def eigenvalues(self, k=6):  # pragma: no cover
         """Computes the eigenvalues for the Hamiltonian.
 
         Args:
```

### Comparing `qibo-0.2.6/src/qibo/hamiltonians/adiabatic.py` & `qibo-0.2.7/src/qibo/hamiltonians/adiabatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,24 @@
     form ``(1 - s) * H0 + s * H1`` efficiently.
     """
 
     def __new__(cls, h0, h1):
         if type(h1) != type(h0):
             raise_error(
                 TypeError,
-                "h1 should be of the same type {} of h0 but "
-                "is {}.".format(type(h0), type(h1)),
+                f"h1 should be of the same type {type(h0)} of h0 but is {type(h1)}.",
             )
         if isinstance(h0, hamiltonians.Hamiltonian):
             return BaseAdiabaticHamiltonian(h0, h1)
         elif isinstance(h0, hamiltonians.SymbolicHamiltonian):
             return SymbolicAdiabaticHamiltonian(h0, h1)
         else:
             raise_error(
                 TypeError,
-                "h0 should be a hamiltonians.Hamiltonian "
-                "object but is {}.".format(type(h0)),
+                f"h0 should be a hamiltonians.Hamiltonian object but is {type(h0)}.",
             )
 
     def __init__(self, h0, h1):  # pragma: no cover
         self.h0, self.h1 = h0, h1
         self.schedule = None
         self.total_time = None
 
@@ -59,19 +57,19 @@
 class BaseAdiabaticHamiltonian:
     """Adiabatic Hamiltonian that is a sum of :class:`qibo.hamiltonians.hamiltonians.Hamiltonian`."""
 
     def __init__(self, h0, h1):
         if h0.nqubits != h1.nqubits:
             raise_error(
                 ValueError,
-                "H0 has {} qubits while H1 has {}." "".format(h0.nqubits, h1.nqubits),
+                f"H0 has {h0.nqubits} qubits while H1 has {h1.nqubits}.",
             )
         self.nqubits = h0.nqubits
         if h0.backend != h1.backend:  # pragma: no cover
-            raise_error(ValueError, "H0 and H1 have different backend.")
+            raise_error(ValueError, "H0 and H1 have different backends.")
         self.backend = h0.backend
         self.h0, self.h1 = h0, h1
         self.schedule = None
         self.total_time = None
 
     def ground_state(self):
         return self.h0.ground_state()
```

### Comparing `qibo-0.2.6/src/qibo/hamiltonians/hamiltonians.py` & `qibo-0.2.7/src/qibo/hamiltonians/hamiltonians.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from itertools import chain
 from typing import Optional
 
 import numpy as np
 import sympy
 
+from qibo.backends import PyTorchBackend
 from qibo.config import EINSUM_CHARS, log, raise_error
 from qibo.hamiltonians.abstract import AbstractHamiltonian
 from qibo.symbols import Z
 
 
 class Hamiltonian(AbstractHamiltonian):
     """Hamiltonian based on a dense or sparse matrix representation.
@@ -111,14 +112,15 @@
             self._exp["result"] = self.backend.calculate_matrix_exp(
                 a, self.matrix, self._eigenvectors, self._eigenvalues
             )
         return self._exp.get("result")
 
     def expectation(self, state, normalize=False):
         if isinstance(state, self.backend.tensor_types):
+            state = self.backend.cast(state)
             shape = tuple(state.shape)
             if len(shape) == 1:  # state vector
                 return self.backend.calculate_expectation_state(self, state, normalize)
 
             if len(shape) == 2:  # density matrix
                 return self.backend.calculate_expectation_density_matrix(
                     self, state, normalize
@@ -170,14 +172,15 @@
 
         Args:
             state (np.ndarray): quantum state to be used to compute the energy fluctuation.
 
         Return:
             Energy fluctuation value (float).
         """
+        state = self.backend.cast(state)
         energy = self.expectation(state)
         h = self.matrix
         h2 = Hamiltonian(nqubits=self.nqubits, matrix=h @ h, backend=self.backend)
         average_h2 = self.backend.calculate_expectation_state(h2, state, normalize=True)
         return np.sqrt(np.abs(average_h2 - energy**2))
 
     def __add__(self, o):
@@ -238,19 +241,21 @@
         elif not isinstance(o, self.backend.numeric_types):
             raise_error(
                 NotImplementedError,
                 f"Hamiltonian multiplication to {type(o)} not implemented.",
             )
         new_matrix = self.matrix * o
         r = self.__class__(self.nqubits, new_matrix, backend=self.backend)
+        o = self.backend.cast(o)
         if self._eigenvalues is not None:
             if self.backend.np.real(o) >= 0:  # TODO: check for side effects K.qnp
                 r._eigenvalues = o * self._eigenvalues
             elif not self.backend.issparse(self.matrix):
-                r._eigenvalues = o * self._eigenvalues[::-1]
+                axis = (0,) if isinstance(self.backend, PyTorchBackend) else 0
+                r._eigenvalues = o * self.backend.np.flip(self._eigenvalues, axis)
         if self._eigenvectors is not None:
             if self.backend.np.real(o) > 0:  # TODO: see above
                 r._eigenvectors = self._eigenvectors
             elif o == 0:
                 r._eigenvectors = self.eye(int(self._eigenvectors.shape[0]))
         return r
```

### Comparing `qibo-0.2.6/src/qibo/hamiltonians/models.py` & `qibo-0.2.7/src/qibo/hamiltonians/models.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/hamiltonians/terms.py` & `qibo-0.2.7/src/qibo/hamiltonians/terms.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,25 @@
     """
 
     def __init__(self, matrix, *q):
         for qi in q:
             if qi < 0:
                 raise_error(
                     ValueError,
-                    "Invalid qubit id {} < 0 was given "
-                    "in Hamiltonian term".format(qi),
+                    f"Invalid qubit id {qi} < 0 was given in Hamiltonian term.",
                 )
         if not isinstance(matrix, np.ndarray):
-            raise_error(
-                TypeError, "Invalid type {} of symbol matrix." "".format(type(matrix))
-            )
+            raise_error(TypeError, f"Invalid type {type(matrix)} of symbol matrix.")
         dim = int(matrix.shape[0])
         if 2 ** len(q) != dim:
             raise_error(
                 ValueError,
-                "Matrix dimension {} given in Hamiltonian "
-                "term is not compatible with the number "
-                "of target qubits {}."
-                "".format(dim, len(q)),
+                f"Matrix dimension {dim} given in Hamiltonian "
+                + "term is not compatible with the number "
+                + f"of target qubits {len(q)}.",
             )
         self.target_qubits = tuple(q)
         self._gate = None
         self.hamiltonian = None
         self._matrix = matrix
 
     @property
@@ -75,16 +71,15 @@
         The target qubits of the given term should be a subset of the target
         qubits of the current term.
         """
         if not set(term.target_qubits).issubset(set(self.target_qubits)):
             raise_error(
                 ValueError,
                 "Cannot merge HamiltonianTerm acting on "
-                "qubits {} to term on qubits {}."
-                "".format(term.target_qubits, self.target_qubits),
+                + f"qubits {term.target_qubits} to term on qubits {self.target_qubits}.",
             )
         matrix = np.kron(term.matrix, np.eye(2 ** (len(self) - len(term))))
         matrix = np.reshape(matrix, 2 * len(self) * (2,))
         order = []
         i = len(term)
         for qubit in self.target_qubits:
             if qubit in term.target_qubits:
@@ -186,15 +181,15 @@
                     else:
                         self.coefficient *= factor.matrix
                 elif factor == sympy.I:
                     self.coefficient *= 1j
                 elif factor.is_number:
                     self.coefficient *= complex(factor)
                 else:  # pragma: no cover
-                    raise_error(TypeError, "Cannot parse factor {}.".format(factor))
+                    raise_error(TypeError, f"Cannot parse factor {factor}.")
 
         self.target_qubits = tuple(sorted(self.matrix_map.keys()))
 
     @property
     def matrix(self):
         """Calculates the full matrix corresponding to this term.
```

### Comparing `qibo-0.2.6/src/qibo/measurements.py` & `qibo-0.2.7/src/qibo/measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Used by :class:`qibo.gates.measurements.M` with ``collapse=True`` to allow
     controlling subsequent gates from the measurement results.
     """
 
     _counter = 0
 
     def __new__(cls, *args, **kwargs):
-        name = "m{}".format(cls._counter)
+        name = f"m{cls._counter}"
         cls._counter += 1
         return super().__new__(cls=cls, name=name)
 
     def __init__(self, index, result):
         self.index = index
         self.result = result
```

### Comparing `qibo-0.2.6/src/qibo/models/_openqasm.py` & `qibo-0.2.7/src/qibo/models/_openqasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,15 @@
                 raise_error(RuntimeError, f"Unsupported {type(statement)} statement.")
         circ = qibo.Circuit(
             nqubits,
             accelerators,
             density_matrix,
             wire_names=self._construct_wire_names(),
         )
-        for gate in gates:
-            circ.add(gate)
-        self._reorder_registers(circ.measurements)
+        circ.add(self._merge_measurements(gates))
         return circ
 
     def _get_measurement(self, measurement):
         """Converts a :class:`openqasm3.ast.QuantumMeasurementStatement` statement
         into :class:`qibo.gates.measurements.M`."""
         qubit = self._get_qubit(measurement.measure.qubit)
         register = measurement.target.name.name
@@ -263,19 +261,35 @@
         into :class:`qibo.parser.CustomQASMGate` object."""
         name = definition.name.name
         qubits = [self._get_qubit(q) for q in definition.qubits]
         args = [self._unroll_expression(expr) for expr in definition.arguments]
         gates = [self._get_gate(gate) for gate in definition.body]
         self.defined_gates.update({name: CustomQASMGate(name, gates, qubits, args)})
 
-    def _reorder_registers(self, measurements):
-        """Reorders the registers of the provided :class:`qibo.gates.measurements.M`
-        gates according to the classical registers order defined in the QASM program."""
-        for meas in measurements:
-            meas.target_qubits = [self.c_registers[meas.register_name].pop(0)]
+    def _merge_measurements(self, gates):
+        """Merges separated measurements of a same register into a single one.
+        This is needed because qibo doesn't allow to separetely define two measurements in a same register:
+
+        # not allowed
+        c.add(gates.M(0, register="m0"))
+        c.add(gates.M(1, register="m0"))
+        """
+        updated_queue = []
+        for gate in gates:
+            if isinstance(gate, qibo.gates.M):
+                if gate.register_name in self.c_registers:
+                    updated_queue.append(
+                        qibo.gates.M(
+                            *self.c_registers.pop(gate.register_name),
+                            register_name=gate.register_name,
+                        )
+                    )
+            else:
+                updated_queue.append(gate)
+        return updated_queue
 
     def _construct_wire_names(self):
         """Builds the wires names from the declared quantum registers."""
         wire_names = []
         for reg_name, reg_qubits in self.q_registers.items():
             wires = sorted(
                 zip(repeat(reg_name, len(reg_qubits)), reg_qubits), key=lambda x: x[1]
```

### Comparing `qibo-0.2.6/src/qibo/models/circuit.py` & `qibo-0.2.7/src/qibo/models/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,15 +434,18 @@
             for gate in self.queue:
                 if isinstance(gate, gates.FusedGate):  # pragma: no cover
                     # impractical case
                     raise_error(
                         NotImplementedError,
                         "Cannot create deep copy of fused circuit.",
                     )
-                new_circuit.add(copy.copy(gate))
+                if isinstance(gate, gates.M):
+                    new_circuit.add(gate.__class__(*gate.init_args, **gate.init_kwargs))
+                else:
+                    new_circuit.add(copy.copy(gate))
         else:
             if self.accelerators:  # pragma: no cover
                 raise_error(
                     ValueError,
                     "Non-deep copy is not allowed for distributed "
                     "circuits because they modify gate objects.",
                 )
@@ -660,21 +663,19 @@
 
                 self.queue.append(gate)
                 if gate.register_name is None:
                     # add default register name
                     nreg = self.queue.nmeasurements - 1
                     gate.register_name = f"register{nreg}"
                 else:
-                    registers = self.measurement_tuples
-                    for register, qubits in registers.items():
-                        intersection = set(qubits).intersection(set(gate.target_qubits))
-                        if len(intersection) > 0:
+                    name = gate.register_name
+                    for mgate in self.measurements:
+                        if name == mgate.register_name:
                             raise_error(
-                                KeyError,
-                                f"Qubits {tuple(intersection)} already measured in register `{register}`.",
+                                KeyError, f"Register {name} already exists in circuit."
                             )
 
                 gate.result.circuit = self
                 if gate.collapse:
                     self.has_collapse = True
                 else:
                     self.measurements.append(gate)
@@ -1149,24 +1150,22 @@
 
         code = [f"// Generated by QIBO {__version__}"]
         code += ["OPENQASM 2.0;"]
         code += ['include "qelib1.inc";']
         code += [f"qreg q[{self.nqubits}];"]
 
         # Set measurements
-        for measurement in self.measurements:
-            reg_name = measurement.register_name
-            reg_qubits = measurement.target_qubits
-            if not reg_name.islower():
+        for register, qubits in self.measurement_tuples.items():
+            if not register.islower():
                 raise_error(
                     NameError,
                     "OpenQASM does not support capital letters in "
-                    + f"register names but {reg_name} was used",
+                    + f"register names but {register} was used",
                 )
-            code.append(f"creg {reg_name}[{len(reg_qubits)}];")
+            code.append(f"creg {register}[{len(qubits)}];")
 
         # Add gates
         for gate in self.queue:
             if isinstance(gate, gates.M):
                 continue
 
             if gate.is_controlled_by:
@@ -1179,18 +1178,17 @@
                 params = (str(x) for x in gate.parameters)
                 name = f"{gate.qasm_label}({', '.join(params)})"
             else:
                 name = gate.qasm_label
             code.append(f"{name} {qubits};")
 
         # Add measurements
-        for measurement in self.measurements:
-            reg_name = measurement.register_name
-            for i, q in enumerate(measurement.target_qubits):
-                code.append(f"measure q[{q}] -> {reg_name}[{i}];")
+        for register, qubits in self.measurement_tuples.items():
+            for i, q in enumerate(qubits):
+                code.append(f"measure q[{q}] -> {register}[{i}];")
 
         return "\n".join(code)
 
     @classmethod
     def from_qasm(cls, qasm_code, accelerators=None, density_matrix=False):
         """Constructs a circuit from QASM code.
```

### Comparing `qibo-0.2.6/src/qibo/models/dbi/double_bracket.py` & `qibo-0.2.7/src/qibo/models/dbi/double_bracket.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/dbi/utils.py` & `qibo-0.2.7/src/qibo/models/dbi/utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/distcircuit.py` & `qibo-0.2.7/src/qibo/models/distcircuit.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/encodings.py` & `qibo-0.2.7/src/qibo/models/encodings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module with functions that encode classical data into quantum circuits."""
 
 import math
+from inspect import signature
 from typing import Optional, Union
 
 import numpy as np
-from scipy.stats import rv_continuous
 
 from qibo import gates
 from qibo.config import raise_error
 from qibo.models.circuit import Circuit
 
 
 def comp_basis_encoder(
@@ -223,14 +223,18 @@
         and not isinstance(seed, int)
         and not isinstance(seed, np.random.Generator)
     ):
         raise_error(
             TypeError, "seed must be either type int or numpy.random.Generator."
         )
 
+    from qibo.quantum_info.random_ensembles import (  # pylint: disable=C0415
+        _ProbabilityDistributionGaussianLoader,
+    )
+
     local_state = (
         np.random.default_rng(seed) if seed is None or isinstance(seed, int) else seed
     )
 
     sampler = _ProbabilityDistributionGaussianLoader(
         a=0, b=2 * math.pi, seed=local_state
     )
@@ -245,14 +249,123 @@
         phases.extend(sampler.rvs(depth=depth, size=len(row)))
 
     circuit.set_parameters(phases)
 
     return circuit
 
 
+def entangling_layer(
+    nqubits: int,
+    architecture: str = "diagonal",
+    entangling_gate: Union[str, gates.Gate] = "CNOT",
+    closed_boundary: bool = False,
+):
+    """Creates a layer of two-qubit, entangling gates.
+
+    If the chosen gate is a parametrized gate, all phases are set to :math:`0.0`.
+
+    Args:
+        nqubits (int): Total number of qubits in the circuit.
+        architecture (str, optional): Architecture of the entangling layer.
+            Options are ``diagonal``, ``shifted``, ``even-layer``, and ``odd-layer``.
+            Defaults to ``"diagonal"``.
+        entangling_gate (str or :class:`qibo.gates.Gate`, optional): Two-qubit gate to be used
+            in the entangling layer. If ``entangling_gate`` is a parametrized gate,
+            all phases are initialized as :math:`0.0`. Defaults to  ``"CNOT"``.
+        closed_boundary (bool, optional): If ``True`` adds a closed-boundary condition
+            to the entangling layer. Defaults to ``False``.
+
+    Returns:
+        :class:`qibo.models.circuit.Circuit`: Circuit containing layer of two-qubit gates.
+    """
+
+    if not isinstance(nqubits, int):
+        raise_error(
+            TypeError, f"nqubits must be type int, but it is type {type(nqubits)}."
+        )
+
+    if nqubits <= 0.0:
+        raise_error(
+            ValueError, f"nqubits must be a positive integer, but it is {nqubits}."
+        )
+
+    if not isinstance(architecture, str):
+        raise_error(
+            TypeError,
+            f"``architecture`` must be type str, but it is type {type(architecture)}.",
+        )
+
+    if architecture not in ["diagonal", "shifted", "even-layer", "odd-layer"]:
+        raise_error(
+            NotImplementedError,
+            f"``architecture`` {architecture} not found.",
+        )
+
+    if not isinstance(closed_boundary, bool):
+        raise_error(
+            TypeError,
+            f"closed_boundary must be type bool, but it is type {type(closed_boundary)}.",
+        )
+
+    gate = (
+        getattr(gates, entangling_gate)
+        if isinstance(entangling_gate, str)
+        else entangling_gate
+    )
+
+    if gate.__name__ == "GeneralizedfSim":
+        raise_error(
+            NotImplementedError,
+            "This function does not support the ``GeneralizedfSim`` gate.",
+        )
+
+    # Finds the number of correct number of parameters to initialize the gate class.
+    parameters = list(signature(gate).parameters)
+
+    if "q2" in parameters:
+        raise_error(
+            NotImplementedError, f"This function does not accept three-qubit gates."
+        )
+
+    # If gate is parametrized, sets all angles to 0.0
+    parameters = (0.0,) * (len(parameters) - 3) if len(parameters) > 2 else None
+
+    circuit = Circuit(nqubits)
+
+    if architecture == "diagonal":
+        circuit.add(
+            _parametrized_two_qubit_gate(gate, qubit, qubit + 1, parameters)
+            for qubit in range(nqubits - 1)
+        )
+    elif architecture == "even-layer":
+        circuit.add(
+            _parametrized_two_qubit_gate(gate, qubit, qubit + 1, parameters)
+            for qubit in range(0, nqubits - 1, 2)
+        )
+    elif architecture == "odd-layer":
+        circuit.add(
+            _parametrized_two_qubit_gate(gate, qubit, qubit + 1, parameters)
+            for qubit in range(1, nqubits - 1, 2)
+        )
+    else:
+        circuit.add(
+            _parametrized_two_qubit_gate(gate, qubit, qubit + 1, parameters)
+            for qubit in range(0, nqubits - 1, 2)
+        )
+        circuit.add(
+            _parametrized_two_qubit_gate(gate, qubit, qubit + 1, parameters)
+            for qubit in range(1, nqubits - 1, 2)
+        )
+
+    if closed_boundary:
+        circuit.add(_parametrized_two_qubit_gate(gate, nqubits - 1, 0, parameters))
+
+    return circuit
+
+
 def _generate_rbs_pairs(nqubits: int, architecture: str):
     """Generating list of indexes representing the RBS connections
 
     Creates circuit with all RBS initialised with 0.0 phase.
 
     Args:
         nqubits (int): number of qubits.
@@ -330,17 +443,13 @@
         for j in range(j_max - 1, 0, -1):
             r_array[j - 1] = math.sqrt(r_array[2 * j] ** 2 + r_array[2 * j - 1] ** 2)
             phases[j - 1] = math.acos(r_array[2 * j - 1] / r_array[j - 1])
 
     return phases
 
 
-class _ProbabilityDistributionGaussianLoader(rv_continuous):
-    """Probability density function for sampling phases of
-    the RBS gates as a function of circuit depth."""
-
-    def _pdf(self, theta: float, depth: int):
-        amplitude = 2 * math.gamma(2 ** (depth - 1)) / math.gamma(2 ** (depth - 2)) ** 2
-
-        probability = abs(math.sin(theta) * math.cos(theta)) ** (2 ** (depth - 1) - 1)
+def _parametrized_two_qubit_gate(gate, q0, q1, params=None):
+    """Returns two-qubit gate initialized with or without phases."""
+    if params is not None:
+        return gate(q0, q1, *params)
 
-        return amplitude * probability / 4
+    return gate(q0, q1)
```

### Comparing `qibo-0.2.6/src/qibo/models/error_mitigation.py` & `qibo-0.2.7/src/qibo/models/error_mitigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     if replacement_gates is None:
         replacement_gates = [(gates.RZ, {"theta": n * np.pi / 2}) for n in range(4)]
 
     gates_to_replace = []
     for i, gate in enumerate(circuit.queue):
         if isinstance(gate, gates.RZ):
-            if gate.init_kwargs["theta"] % (np.pi / 2) != 0.0:
+            if not gate.clifford:
                 gates_to_replace.append((i, gate))
 
     if not gates_to_replace:
         raise_error(ValueError, "No non-Clifford RZ gate found, no circuit sampled.")
 
     replacement, distance = [], []
     for _, gate in gates_to_replace:
@@ -784,41 +784,45 @@
     sampled_circuit = sample_clifford_training_circuit(circuit, backend=backend)
     unitary_matrix = sampled_circuit.unitary(backend=backend)
     num_qubits = sampled_circuit.nqubits
 
     comp_to_pauli = comp_basis_to_pauli(num_qubits, backend=backend)
     observable.nqubits = num_qubits
     observable_liouville = vectorization(
-        np.transpose(np.conjugate(unitary_matrix)) @ observable.matrix @ unitary_matrix,
+        backend.np.transpose(backend.np.conj(unitary_matrix), (1, 0))
+        @ observable.matrix
+        @ unitary_matrix,
         order="row",
         backend=backend,
     )
     observable_pauli_liouville = comp_to_pauli @ observable_liouville
 
-    index = int(np.where(abs(observable_pauli_liouville) >= 1e-5)[0][0])
+    index = int(
+        backend.np.where(backend.np.abs(observable_pauli_liouville) >= 1e-5)[0][0]
+    )
 
     observable_pauli = list(product(["I", "X", "Y", "Z"], repeat=num_qubits))[index]
 
     pauli_gates = {
         "I": backend.cast(gates.I(0).matrix(backend=backend)),
         "X": backend.cast(gates.X(0).matrix(backend=backend)),
         "Y": backend.cast(gates.Y(0).matrix(backend=backend)),
         "Z": backend.cast(gates.Z(0).matrix(backend=backend)),
     }
 
     adjustment_gates = []
     for i in range(num_qubits):
         observable_i = pauli_gates[observable_pauli[i]]
         random_init = pauli_gates["I"]
-        while np.any(abs(observable_i - pauli_gates["Z"]) > 1e-5) and np.any(
-            abs(observable_i - pauli_gates["I"]) > 1e-5
-        ):
+        while backend.np.any(
+            backend.np.abs(observable_i - pauli_gates["Z"]) > 1e-5
+        ) and backend.np.any(abs(observable_i - pauli_gates["I"]) > 1e-5):
             random_init = random_clifford(1, backend=backend, return_circuit=False)
             observable_i = (
-                np.conjugate(np.transpose(random_init))
+                backend.np.conj(backend.np.transpose(random_init, (1, 0)))
                 @ pauli_gates[observable_pauli[i]]
                 @ random_init
             )
 
         adjustment_gate = gates.Unitary(random_init, i)
         adjustment_gate.clifford = True
         adjustment_gates.append(adjustment_gate)
```

### Comparing `qibo-0.2.6/src/qibo/models/evolution.py` & `qibo-0.2.7/src/qibo/models/evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,31 +51,29 @@
     def __init__(self, hamiltonian, dt, solver="exp", callbacks=[], accelerators=None):
         hamtypes = (AbstractHamiltonian, BaseAdiabaticHamiltonian)
         if isinstance(hamiltonian, hamtypes):
             ham = hamiltonian
         else:
             ham = hamiltonian(0)
             if not isinstance(ham, AbstractHamiltonian):
-                raise TypeError(
-                    "Hamiltonian type {} not understood." "".format(type(ham))
-                )
+                raise TypeError(f"Hamiltonian type {type(ham)} not understood.")
         self.nqubits = ham.nqubits
         self.backend = ham.backend
         if dt <= 0:
             raise_error(ValueError, f"Time step dt should be positive but is {dt}.")
         self.dt = dt
 
         disthamtypes = (SymbolicHamiltonian, BaseAdiabaticHamiltonian)
         if accelerators is not None:  # pragma: no cover
             if not isinstance(ham, disthamtypes) or solver != "exp":
                 raise_error(
                     NotImplementedError,
                     "Distributed evolution is only "
-                    "implemented using the Trotter "
-                    "exponential solver.",
+                    + "implemented using the Trotter "
+                    + "exponential solver.",
                 )
             ham.circuit(dt, accelerators)
         self.solver = solvers.get_solver(solver, self.dt, hamiltonian)
         self.callbacks = callbacks
         self.accelerators = accelerators
         self.normalize_state = self._create_normalize_state(solver)
         self.calculate_callbacks = self._create_calculate_callbacks(accelerators)
```

### Comparing `qibo-0.2.6/src/qibo/models/grover.py` & `qibo-0.2.7/src/qibo/models/grover.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/hep.py` & `qibo-0.2.7/src/qibo/models/hep.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/iqae.py` & `qibo-0.2.7/src/qibo/models/iqae.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/qcnn.py` & `qibo-0.2.7/src/qibo/models/qcnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+""" This module implements a Quantum Convolutional Neural Network (QCNN) for classification tasks. The QCNN model was originally proposed in: arXiv:1810.03787 <https://arxiv.org/abs/1810.03787>_ for the identification of quantum phases.
+
+The QuantumCNN class in this module provides methods to construct the QCNN.
+"""
+
 import numpy as np
 
 from qibo import gates, get_backend
 from qibo.models import Circuit
 
 
 class QuantumCNN:
@@ -50,14 +55,29 @@
         nqubits,
         nlayers,
         nclasses=2,
         params=None,
         twoqubitansatz=None,
         copy_init_state=None,
     ):
+        """
+        Initializes the QuantumCNN object.
+
+        Args:
+            nqubits (int): The number of qubits in the QCNN.
+            nlayers (int): The number of layers in the QCNN.
+            nclasses (int, optional): The number of classes for the classification task. Defaults to 2.
+            params (np.ndarray, optional): The initial parameters for the QCNN. If None, random parameters are generated. Defaults to None.
+            twoqubitansatz (qibo.models.circuit.Circuit, optional): A two-qubit ansatz for the convolutional layers. If None, a default ansatz is used. Defaults to None.
+            copy_init_state (bool, optional): Whether to copy the initial state for each shot in the simulation. If None, the behavior depends on the backend. Defaults to None.
+
+        Raises:
+            ValueError: If nqubits is not larger than 1.
+        """
+
         self.nclasses = nclasses
         self.nqubits = nqubits
         self.nlayers = nlayers
         self.twoqubitansatz = twoqubitansatz
 
         if copy_init_state is None:
             if "qibojit" in get_backend():
@@ -253,17 +273,14 @@
 
         self._circuit.set_parameters(expanded_params)
 
     def Classifier_circuit(self, theta):
         """
         Args:
             theta: list or numpy.array with the biases and the angles to be used in the circuit.
-            nlayers: int number of layers of the varitional circuit ansatz.
-            RY: if True, parameterized Rx,Rz,Rx gates are used in the circuit.
-                if False, parameterized Ry gates are used in the circuit (default=False).
         Returns:
             Circuit implementing the variational ansatz for angles "theta".
         """
         bias = np.array(theta[0 : self.measured_qubits])
         angles = theta[self.measured_qubits :]
 
         self.set_circuit_params(angles)
@@ -309,15 +326,14 @@
 
         return loss / len(labels)
 
     def Cost_function(self, theta, data=None, labels=None, nshots=10000):
         """
         Args:
             theta: list or numpy.array with the biases and the angles to be used in the circuit.
-            nlayers: int number of layers of the varitional circuit ansatz.
             data: numpy.array data[page][word]  (this is an array of kets).
             labels: list or numpy.array with the labels of the quantum states to be classified.
             nshots: int number of runs of the circuit during the sampling process (default=10000).
         Returns:
             numpy.float32 with the value of the square-loss function.
         """
         circ = self.Classifier_circuit(theta)
```

### Comparing `qibo-0.2.6/src/qibo/models/qft.py` & `qibo-0.2.7/src/qibo/models/qft.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,16 @@
     circuit = Circuit(nqubits, accelerators)
     icrit = nqubits // 2 + nqubits % 2
     if accelerators is not None:
         circuit.global_qubits = range(circuit.nlocal, nqubits)  # pylint: disable=E1101
         if icrit < circuit.nglobal:  # pylint: disable=E1101
             raise_error(
                 NotImplementedError,
-                "Cannot implement QFT for {} qubits "
-                "using {} global qubits."
-                "".format(nqubits, circuit.nglobal),
+                f"Cannot implement QFT for {nqubits} qubits "
+                + f"using {circuit.nglobal} global qubits.",
             )  # pylint: disable=E1101
 
     for i1 in range(nqubits):
         if i1 < icrit:
             i1eff = i1
         else:
             i1eff = nqubits - i1 - 1
```

### Comparing `qibo-0.2.6/src/qibo/models/qgan.py` & `qibo-0.2.7/src/qibo/models/qgan.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/tsp.py` & `qibo-0.2.7/src/qibo/models/tsp.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/utils.py` & `qibo-0.2.7/src/qibo/models/utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/models/variational.py` & `qibo-0.2.7/src/qibo/models/variational.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,27 +184,26 @@
         t_max=1,
         bounds_tolerance=1e-7,
         time_tolerance=1e-7,
     ):
         if nsteps <= 0:  # pragma: no cover
             raise_error(
                 ValueError,
-                "Number of steps nsteps should be positive but is {}."
-                "".format(nsteps),
+                f"Number of steps nsteps should be positive but is {nsteps}.",
             )
         if t_max <= 0:  # pragma: no cover
             raise_error(
                 ValueError,
-                "Maximum time t_max should be positive but is {}." "".format(t_max),
+                f"Maximum time t_max should be positive but is {t_max}.",
             )
         if easy_hamiltonian.nqubits != problem_hamiltonian.nqubits:  # pragma: no cover
             raise_error(
                 ValueError,
-                "The easy Hamiltonian has {} qubits while problem Hamiltonian has {}."
-                "".format(easy_hamiltonian.nqubits, problem_hamiltonian.nqubits),
+                f"The easy Hamiltonian has {easy_hamiltonian.nqubits} qubits "
+                + f"while problem Hamiltonian has {problem_hamiltonian.nqubits}.",
             )
 
         self.ATOL = bounds_tolerance
         self.ATOL_TIME = time_tolerance
 
         self._circuit = circuit
         self._h0 = easy_hamiltonian
@@ -215,52 +214,50 @@
 
         self._schedule = None
         nparams = s.__code__.co_argcount
         if not nparams == 1:  # pragma: no cover
             raise_error(
                 ValueError,
                 "Scheduling function must take only one argument,"
-                "but the function proposed takes {}.".format(nparams),
+                + f"but the function proposed takes {nparams}.",
             )
         self.set_schedule(s)
 
     def set_schedule(self, func):
         """Set scheduling function s(t) as func."""
         # check boundary conditions
         s0 = func(0)
         if abs(s0) > self.ATOL:  # pragma: no cover
-            raise_error(ValueError, "s(0) should be 0 but it is {}.".format(s0))
+            raise_error(ValueError, f"s(0) should be 0 but it is {s0}.")
         s1 = func(1)
         if abs(s1 - 1) > self.ATOL:  # pragma: no cover
-            raise_error(ValueError, "s(1) should be 1 but it is {}.".format(s1))
+            raise_error(ValueError, f"s(1) should be 1 but it is {s1}.")
         self._schedule = func
 
     def schedule(self, t):
         """Returns scheduling function evaluated at time t: s(t/Tmax)."""
         if self._schedule is None:  # pragma: no cover
             raise_error(ValueError, "Cannot access scheduling before it is set.")
         if (t - self._t_max) > self.ATOL_TIME:  # pragma: no cover
             raise_error(
                 ValueError,
-                "t cannot be greater than {}, but it is {}.".format(self._t_max, t),
+                f"t cannot be greater than {self._t_max}, but it is {t}.",
             )
 
         s = self._schedule(t / self._t_max)
         if (abs(s) - 1) > self.ATOL:  # pragma: no cover
-            raise_error(
-                ValueError, "s cannot be greater than 1 but it is {}.".format(s)
-            )
+            raise_error(ValueError, f"s cannot be greater than 1 but it is {s}.")
         return s
 
     def hamiltonian(self, t):
         """Returns the adiabatic evolution Hamiltonian at a given time."""
         if (t - self._t_max) > self.ATOL:  # pragma: no cover
             raise_error(
                 ValueError,
-                "t cannot be greater than {}, but it is {}.".format(self._t_max, t),
+                f"t cannot be greater than {self._t_max}, but it is {t}.",
             )
         # boundary conditions  s(0)=0, s(total_time)=1
         st = self.schedule(t)
         return self._h0 * (1 - st) + self._h1 * st
 
     def minimize(
         self,
@@ -356,54 +353,50 @@
     ):
         from qibo.hamiltonians.abstract import AbstractHamiltonian
 
         # list of QAOA variational parameters (angles)
         self.params = None
         # problem hamiltonian
         if not isinstance(hamiltonian, AbstractHamiltonian):
-            raise_error(
-                TypeError, "Invalid Hamiltonian type {}." "".format(type(hamiltonian))
-            )
+            raise_error(TypeError, f"Invalid Hamiltonian type {type(hamiltonian)}.")
         self.hamiltonian = hamiltonian
         self.nqubits = hamiltonian.nqubits
         # mixer hamiltonian (default = -sum(sigma_x))
         if mixer is None:
             trotter = isinstance(
                 self.hamiltonian, self.hamiltonians.SymbolicHamiltonian
             )
             self.mixer = self.hamiltonians.X(
                 self.nqubits, dense=not trotter, backend=self.hamiltonian.backend
             )
         else:
             if type(mixer) != type(hamiltonian):
                 raise_error(
                     TypeError,
-                    "Given Hamiltonian is of type {} "
-                    "while mixer is of type {}."
-                    "".format(type(hamiltonian), type(mixer)),
+                    f"Given Hamiltonian is of type {type(hamiltonian)} "
+                    + f"while mixer is of type {type(mixer)}.",
                 )
             if mixer.nqubits != hamiltonian.nqubits:
                 raise_error(
                     ValueError,
-                    "Given Hamiltonian acts on {} qubits "
-                    "while mixer acts on {}."
-                    "".format(hamiltonian.nqubits, mixer.nqubits),
+                    f"Given Hamiltonian acts on {hamiltonian.nqubits} qubits "
+                    + f"while mixer acts on {mixer.nqubits}.",
                 )
             self.mixer = mixer
 
         # create circuits for Trotter Hamiltonians
         if accelerators is not None and (
             not isinstance(self.hamiltonian, self.hamiltonians.SymbolicHamiltonian)
             or solver != "exp"
         ):
             raise_error(
                 NotImplementedError,
                 "Distributed QAOA is implemented "
-                "only with SymbolicHamiltonian and "
-                "exponential solver.",
+                + "only with SymbolicHamiltonian and "
+                + "exponential solver.",
             )
         if isinstance(self.hamiltonian, self.hamiltonians.SymbolicHamiltonian):
             self.hamiltonian.circuit(1e-2, accelerators)
             self.mixer.circuit(1e-2, accelerators)
 
         # evolution solvers
         from qibo.solvers import get_solver
@@ -530,16 +523,16 @@
                 best, params, _ = qaoa.minimize(initial_p, loss_func=gibbs, loss_func_param={'eta':0.1})
 
         """
         if len(initial_p) % 2 != 0:
             raise_error(
                 ValueError,
                 "Initial guess for the parameters must "
-                "contain an even number of values but "
-                "contains {}.".format(len(initial_p)),
+                + "contain an even number of values but "
+                + "contains {len(initial_p)}.",
             )
 
         def _loss(params, qaoa, hamiltonian, state):
             if state is not None:
                 state = hamiltonian.backend.cast(state, copy=True)
             qaoa.set_parameters(params)
             state = qaoa(state)
```

### Comparing `qibo-0.2.6/src/qibo/noise.py` & `qibo-0.2.7/src/qibo/noise.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/noise_model.py` & `qibo-0.2.7/src/qibo/noise_model.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/optimizers.py` & `qibo-0.2.7/src/qibo/optimizers.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/parallel.py` & `qibo-0.2.7/src/qibo/parallel.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/parameter.py` & `qibo-0.2.7/src/qibo/parameter.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/quantum_info/_clifford_utils.py` & `qibo-0.2.7/src/qibo/quantum_info/_clifford_utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/quantum_info/basis.py` & `qibo-0.2.7/src/qibo/quantum_info/basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     elif vectorize and not sparse:
         basis = [
             vectorization(matrix, order=order, backend=backend) for matrix in basis_full
         ]
     else:
         basis = basis_full
 
-    basis = backend.cast(basis)
+    basis = backend.cast(basis, dtype=backend.dtype)
 
     if normalize:
         basis /= np.sqrt(2**nqubits)
 
     if vectorize and sparse:
         indexes = backend.cast(indexes)
```

### Comparing `qibo-0.2.6/src/qibo/quantum_info/clifford.py` & `qibo-0.2.7/src/qibo/quantum_info/clifford.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/quantum_info/entanglement.py` & `qibo-0.2.7/src/qibo/quantum_info/entanglement.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/quantum_info/entropies.py` & `qibo-0.2.7/src/qibo/quantum_info/entropies.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,20 +50,22 @@
 
     if any(prob_dist < 0) or any(prob_dist > 1.0):
         raise_error(
             ValueError,
             "All elements of the probability array must be between 0. and 1..",
         )
 
-    if np.abs(np.sum(prob_dist) - 1.0) > PRECISION_TOL:
+    total_sum = backend.np.sum(prob_dist)
+
+    if np.abs(total_sum - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "Probability array must sum to 1.")
 
     log_prob = np.where(prob_dist != 0, np.log2(prob_dist) / np.log2(base), 0.0)
 
-    shan_entropy = -np.sum(prob_dist * log_prob)
+    shan_entropy = -backend.np.sum(prob_dist * log_prob)
 
     # absolute value if entropy == 0.0 to avoid returning -0.0
     shan_entropy = np.abs(shan_entropy) if shan_entropy == 0.0 else shan_entropy
 
     return complex(shan_entropy).real
 
 
@@ -115,29 +117,33 @@
     if (any(prob_dist_p < 0) or any(prob_dist_p > 1.0)) or (
         any(prob_dist_q < 0) or any(prob_dist_q > 1.0)
     ):
         raise_error(
             ValueError,
             "All elements of the probability array must be between 0. and 1..",
         )
-    if np.abs(np.sum(prob_dist_p) - 1.0) > PRECISION_TOL:
+    total_sum_p = backend.np.sum(prob_dist_p)
+
+    total_sum_q = backend.np.sum(prob_dist_q)
+
+    if np.abs(total_sum_p - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "First probability array must sum to 1.")
 
-    if np.abs(np.sum(prob_dist_q) - 1.0) > PRECISION_TOL:
+    if np.abs(total_sum_q - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "Second probability array must sum to 1.")
 
     entropy_p = -1 * shannon_entropy(prob_dist_p, base=base, backend=backend)
 
     log_prob_q = np.where(
         prob_dist_q != 0.0, np.log2(prob_dist_q) / np.log2(base), -np.inf
     )
 
     log_prob = np.where(prob_dist_p != 0.0, log_prob_q, 0.0)
 
-    relative = np.sum(prob_dist_p * log_prob)
+    relative = backend.np.sum(prob_dist_p * log_prob)
 
     return entropy_p - relative
 
 
 def classical_renyi_entropy(
     prob_dist, alpha: Union[float, int], base: float = 2, backend=None
 ):
@@ -202,27 +208,31 @@
 
     if any(prob_dist < 0) or any(prob_dist > 1.0):
         raise_error(
             ValueError,
             "All elements of the probability array must be between 0. and 1..",
         )
 
-    if np.abs(np.sum(prob_dist) - 1.0) > PRECISION_TOL:
+    total_sum = backend.np.sum(prob_dist)
+
+    if np.abs(total_sum - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "Probability array must sum to 1.")
 
     if alpha == 0.0:
         return np.log2(len(prob_dist)) / np.log2(base)
 
     if alpha == 1.0:
         return shannon_entropy(prob_dist, base=base, backend=backend)
 
     if alpha == np.inf:
         return -1 * np.log2(max(prob_dist)) / np.log2(base)
 
-    renyi_ent = (1 / (1 - alpha)) * np.log2(np.sum(prob_dist**alpha)) / np.log2(base)
+    total_sum = backend.np.sum(prob_dist**alpha)
+
+    renyi_ent = (1 / (1 - alpha)) * np.log2(total_sum) / np.log2(base)
 
     return renyi_ent
 
 
 def classical_relative_renyi_entropy(
     prob_dist_p, prob_dist_q, alpha: Union[float, int], base: float = 2, backend=None
 ):
@@ -295,35 +305,44 @@
     if (any(prob_dist_p < 0) or any(prob_dist_p > 1.0)) or (
         any(prob_dist_q < 0) or any(prob_dist_q > 1.0)
     ):
         raise_error(
             ValueError,
             "All elements of the probability array must be between 0. and 1..",
         )
-    if np.abs(np.sum(prob_dist_p) - 1.0) > PRECISION_TOL:
+
+    total_sum_p = backend.np.sum(prob_dist_p)
+    total_sum_q = backend.np.sum(prob_dist_q)
+
+    if np.abs(total_sum_p - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "First probability array must sum to 1.")
 
-    if np.abs(np.sum(prob_dist_q) - 1.0) > PRECISION_TOL:
+    if np.abs(total_sum_q - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "Second probability array must sum to 1.")
 
     if alpha == 0.5:
-        return -2 * np.log2(np.sum(np.sqrt(prob_dist_p * prob_dist_q))) / np.log2(base)
+        total_sum = np.sqrt(prob_dist_p * prob_dist_q)
+        total_sum = backend.np.sum(total_sum)
+
+        return -2 * np.log2(total_sum) / np.log2(base)
 
     if alpha == 1.0:
         return classical_relative_entropy(
             prob_dist_p, prob_dist_q, base=base, backend=backend
         )
 
     if alpha == np.inf:
         return np.log2(max(prob_dist_p / prob_dist_q)) / np.log2(base)
 
     prob_p = prob_dist_p**alpha
     prob_q = prob_dist_q ** (1 - alpha)
 
-    return (1 / (alpha - 1)) * np.log2(np.sum(prob_p * prob_q)) / np.log2(base)
+    total_sum = backend.np.sum(prob_p * prob_q)
+
+    return (1 / (alpha - 1)) * np.log2(total_sum) / np.log2(base)
 
 
 def classical_tsallis_entropy(prob_dist, alpha: float, base: float = 2, backend=None):
     """Calculates the classical Tsallis entropy for a discrete probability distribution.
 
     This is defined as
 
@@ -371,21 +390,26 @@
 
     if any(prob_dist < 0) or any(prob_dist > 1.0):
         raise_error(
             ValueError,
             "All elements of the probability array must be between 0. and 1..",
         )
 
-    if np.abs(np.sum(prob_dist) - 1.0) > PRECISION_TOL:
+    total_sum = backend.np.sum(prob_dist)
+
+    if np.abs(total_sum - 1.0) > PRECISION_TOL:
         raise_error(ValueError, "Probability array must sum to 1.")
 
     if alpha == 1.0:
         return shannon_entropy(prob_dist, base=base, backend=backend)
 
-    return (1 / (1 - alpha)) * (np.sum(prob_dist**alpha) - 1)
+    total_sum = prob_dist**alpha
+    total_sum = backend.np.sum(total_sum)
+
+    return (1 / (1 - alpha)) * (total_sum - 1)
 
 
 def von_neumann_entropy(
     state,
     base: float = 2,
     check_hermitian: bool = False,
     return_spectrum: bool = False,
```

### Comparing `qibo-0.2.6/src/qibo/quantum_info/metrics.py` & `qibo-0.2.7/src/qibo/quantum_info/metrics.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/quantum_info/quantum_networks.py` & `qibo-0.2.7/src/qibo/quantum_info/quantum_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         if order is None and self._backend.__class__.__name__ == "TensorflowBackend":
             order = "euclidean"
 
         self._matrix = self._full()
         self._pure = False
 
-        partial_trace = np.einsum("jkjl -> kl", self._matrix)
+        partial_trace = self._einsum("jkjl -> kl", self._matrix)
         identity = self._backend.cast(
             np.eye(partial_trace.shape[0]), dtype=partial_trace.dtype
         )
 
         norm = self._backend.calculate_norm_density_matrix(
             partial_trace - identity,
             order=order,
@@ -208,15 +208,15 @@
 
         if order is None and self._backend.__class__.__name__ == "TensorflowBackend":
             order = "euclidean"
 
         self._matrix = self._full()
         self._pure = False
 
-        partial_trace = np.einsum("jklk -> jl", self._matrix)
+        partial_trace = self._einsum("jklk -> jl", self._matrix)
         identity = self._backend.cast(
             np.eye(partial_trace.shape[0]), dtype=partial_trace.dtype
         )
 
         norm = self._backend.calculate_norm_density_matrix(
             partial_trace - identity,
             order=order,
@@ -288,20 +288,20 @@
 
         Args:
             state (ndarray): density matrix of a ``state``.
 
         Returns:
             ndarray: Resulting state :math:`\\mathcal{E}(\\varrho)`.
         """
-        matrix = np.copy(self._matrix)
+        matrix = self._backend.cast(self._matrix, copy=True)
 
         if self.is_pure():
-            return np.einsum("kj,ml,jl -> km", matrix, np.conj(matrix), state)
+            return self._einsum("kj,ml,jl -> km", matrix, np.conj(matrix), state)
 
-        return np.einsum("jklm,km -> jl", matrix, state)
+        return self._einsum("jklm,km -> jl", matrix, state)
 
     def link_product(self, second_network, subscripts: str = "ij,jk -> ik"):
         """Link product between two quantum networks.
 
         The link product is not commutative. Here, we assume that
         :math:`A.\\textup{link_product}(B)` means "applying :math:`B` to :math:`A`".
         However, the ``link_product`` is associative, so we override the `@` operation
@@ -349,28 +349,28 @@
 
         first_matrix = self._full()
         second_matrix = second_network._full()  # pylint: disable=W0212
 
         if super_subscripts:
             cexpr = "jklmnopq,klop->jmnq"
             return QuantumNetwork(
-                np.einsum(cexpr, first_matrix, second_matrix),
+                self._einsum(cexpr, first_matrix, second_matrix),
                 [self.partition[0] + self.partition[-1]],
             )
 
         cexpr = "jkab,klbc->jlac"
 
         if inv_subscripts:
             return QuantumNetwork(
-                np.einsum(cexpr, second_matrix, first_matrix),
+                self._einsum(cexpr, second_matrix, first_matrix),
                 [second_network.partition[0], self.partition[1]],
             )
 
         return QuantumNetwork(
-            np.einsum(cexpr, first_matrix, second_matrix),
+            self._einsum(cexpr, first_matrix, second_matrix),
             [self.partition[0], second_network.partition[1]],
         )
 
     def copy(self):
         """Returns a copy of the :class:`qibo.quantum_info.quantum_networks.QuantumNetwork` object."""
         return self.__class__(
             np.copy(self._matrix),
@@ -629,14 +629,16 @@
                 f"``pure`` must be type ``bool``, but it is type ``{type(pure)}``.",
             )
 
     def _set_tensor_and_parameters(self):
         """Sets tensor based on inputs."""
         self._backend = _check_backend(self._backend)
 
+        self._einsum = self._backend.np.einsum
+
         if isinstance(self.partition, list):
             self.partition = tuple(self.partition)
 
         try:
             if self._pure:
                 self._matrix = np.reshape(self._matrix, self.partition)
             else:
@@ -657,19 +659,18 @@
                 self.system_output[k * 2] = False
             self.system_output = tuple(self.system_output)
         else:
             self.system_output = tuple(self.system_output)
 
     def _full(self):
         """Reshapes input matrix based on purity."""
-        matrix = np.copy(self._matrix)
-        if self.is_pure():
-            matrix = np.einsum("jk,lm -> kjml", matrix, np.conj(matrix))
+        matrix = self._backend.cast(self._matrix, copy=True)
 
-            return matrix
+        if self.is_pure():
+            matrix = self._einsum("jk,lm -> kjml", matrix, np.conj(matrix))
 
         return matrix
 
     def _check_subscript_pattern(self, subscripts: str):
         """Checks if input subscript match any implemented pattern."""
         braket = "[a-z]"
         pattern_two = re.compile(braket * 2 + "," + braket * 2 + "->" + braket * 2)
```

### Comparing `qibo-0.2.6/src/qibo/quantum_info/random_ensembles.py` & `qibo-0.2.7/src/qibo/quantum_info/random_ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Module with functions that create random quantum and classical objects."""
 
+import math
 import warnings
+from functools import cache
 from typing import Optional, Union
 
 import numpy as np
 from scipy.stats import rv_continuous
 
 from qibo import Circuit, gates
 from qibo.backends import NumpyBackend, _check_backend
@@ -16,14 +18,26 @@
     choi_to_liouville,
     choi_to_pauli,
     choi_to_stinespring,
     vectorization,
 )
 
 
+class _ProbabilityDistributionGaussianLoader(rv_continuous):
+    """Probability density function for sampling phases of
+    the RBS gates as a function of circuit depth."""
+
+    def _pdf(self, theta: float, depth: int):
+        amplitude = 2 * math.gamma(2 ** (depth - 1)) / math.gamma(2 ** (depth - 2)) ** 2
+
+        probability = abs(math.sin(theta) * math.cos(theta)) ** (2 ** (depth - 1) - 1)
+
+        return amplitude * probability / 4
+
+
 class _probability_distribution_sin(rv_continuous):  # pragma: no cover
     def _pdf(self, theta: float):
         return 0.5 * np.sin(theta)
 
     def _cdf(self, theta: float):
         return np.sin(theta / 2) ** 2
 
@@ -222,15 +236,16 @@
         R = np.diag(D)
         unitary = np.dot(Q, R)
     elif measure is None:
         from scipy.linalg import expm
 
         H = random_hermitian(dims, seed=seed, backend=NumpyBackend())
         unitary = expm(-1.0j * H / 2)
-        unitary = backend.cast(unitary, dtype=unitary.dtype)
+
+    unitary = backend.cast(unitary, dtype=unitary.dtype)
 
     return unitary
 
 
 def random_quantum_channel(
     dims: int,
     representation: str = "liouville",
@@ -1083,14 +1098,29 @@
         k = int(k)
         permutations[l] = mute_index[k]
         del mute_index[k]
 
     return hadamards, permutations
 
 
+@cache
+def _create_S(q):
+    return gates.S(q)
+
+
+@cache
+def _create_CZ(cq, tq):
+    return gates.CZ(cq, tq)
+
+
+@cache
+def _create_CNOT(cq, tq):
+    return gates.CNOT(cq, tq)
+
+
 def _operator_from_hadamard_free_group(
     gamma_matrix, delta_matrix, density_matrix: bool = False, pauli_operator=None
 ):
     """Calculates an element :math:`F` of the Hadamard-free group :math:`\\mathcal{F}_{n}`,
     where :math:`n` is the number of qubits ``nqubits``. For more details,
     see Reference [1].
 
@@ -1120,27 +1150,27 @@
 
     nqubits = len(gamma_matrix)
     circuit = Circuit(nqubits, density_matrix=density_matrix)
 
     if pauli_operator is not None:
         circuit += pauli_operator
 
-    for qubit, gamma in enumerate(np.diag(gamma_matrix)):
-        if gamma == 1:
-            circuit.add(gates.S(qubit))
-
-    for j in range(nqubits):
-        for k in range(j + 1, nqubits):
-            if gamma_matrix[k, j] == 1:
-                circuit.add(gates.CZ(j, k))
+    idx = np.tril_indices(nqubits, k=-1)
+    gamma_ones = gamma_matrix[idx].nonzero()[0]
+    delta_ones = delta_matrix[idx].nonzero()[0]
+
+    S_gates = [_create_S(q) for q in np.diag(gamma_matrix).nonzero()[0]]
+    CZ_gates = [
+        _create_CZ(cq, tq) for cq, tq in zip(idx[1][gamma_ones], idx[0][gamma_ones])
+    ]
+    CNOT_gates = [
+        _create_CNOT(cq, tq) for cq, tq in zip(idx[1][delta_ones], idx[0][delta_ones])
+    ]
 
-    for j in range(nqubits):
-        for k in range(j + 1, nqubits):
-            if delta_matrix[k, j] == 1:
-                circuit.add(gates.CNOT(j, k))
+    circuit.add(S_gates + CZ_gates + CNOT_gates)
 
     return circuit
 
 
 def _super_op_from_bcsz_measure(dims: int, rank: int, order: str, seed, backend):
     """Helper function for :func:qibo.quantum_info.random_ensembles.random_quantum_channel.
     Generates a channel from the BCSZ measure.
@@ -1174,19 +1204,19 @@
 
     operator = np.zeros((dims, dims), dtype=complex)
     operator = backend.cast(operator, dtype=operator.dtype)
     for eigenvalue, eigenvector in zip(eigenvalues, np.transpose(eigenvectors)):
         operator += eigenvalue * np.outer(eigenvector, np.conj(eigenvector))
 
     if order == "row":
-        operator = np.kron(
+        operator = backend.np.kron(
             backend.identity_density_matrix(nqubits, normalize=False), operator
         )
     if order == "column":
-        operator = np.kron(
+        operator = backend.np.kron(
             operator, backend.identity_density_matrix(nqubits, normalize=False)
         )
 
     super_op = operator @ super_op @ operator
 
     return super_op
```

### Comparing `qibo-0.2.6/src/qibo/quantum_info/superoperator_transformations.py` & `qibo-0.2.7/src/qibo/quantum_info/superoperator_transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,16 @@
         for coeff, eigenvector_left, eigenvector_right in zip(coefficients, U, V):
             kraus_left.append(
                 coeff * unvectorization(eigenvector_left, order=order, backend=backend)
             )
             kraus_right.append(
                 coeff * unvectorization(eigenvector_right, order=order, backend=backend)
             )
+        kraus_left = backend.cast(kraus_left)
+        kraus_right = backend.cast(kraus_right)
         kraus_ops = backend.cast([kraus_left, kraus_right])
     else:
         # when choi_super_op is CP
         kraus_ops, coefficients = [], []
         for eig, kraus in zip(eigenvalues, eigenvectors):
             if np.abs(eig) > precision_tol:
                 eig = np.sqrt(eig)
```

### Comparing `qibo-0.2.6/src/qibo/quantum_info/utils.py` & `qibo-0.2.7/src/qibo/quantum_info/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,18 +233,18 @@
         if (any(prob_dist_p < 0) or any(prob_dist_p > 1.0)) or (
             any(prob_dist_q < 0) or any(prob_dist_q > 1.0)
         ):
             raise_error(
                 ValueError,
                 "All elements of the probability array must be between 0. and 1..",
             )
-        if np.abs(np.sum(prob_dist_p) - 1.0) > PRECISION_TOL:
+        if backend.np.abs(backend.np.sum(prob_dist_p) - 1.0) > PRECISION_TOL:
             raise_error(ValueError, "First probability array must sum to 1.")
 
-        if np.abs(np.sum(prob_dist_q) - 1.0) > PRECISION_TOL:
+        if backend.np.abs(backend.np.sum(prob_dist_q) - 1.0) > PRECISION_TOL:
             raise_error(ValueError, "Second probability array must sum to 1.")
 
     distance = float(
         backend.calculate_norm(np.sqrt(prob_dist_p) - np.sqrt(prob_dist_q)) / np.sqrt(2)
     )
 
     return distance
@@ -317,15 +317,15 @@
 
     if isinstance(prob_dist_q, list):
         prob_dist_q = backend.cast(prob_dist_q, dtype=np.float64)
 
     hellinger_error = hellinger_fidelity(
         prob_dist_p, prob_dist_q, validate=validate, backend=backend
     )
-    hellinger_error = np.sqrt(hellinger_error / nshots) * np.sum(
+    hellinger_error = np.sqrt(hellinger_error / nshots) * backend.np.sum(
         np.sqrt(prob_dist_q * (1 - prob_dist_p))
         + np.sqrt(prob_dist_p * (1 - prob_dist_q))
     )
 
     return hellinger_error
```

### Comparing `qibo-0.2.6/src/qibo/result.py` & `qibo-0.2.7/src/qibo/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             If ``registers`` is ``False``
                 a single tensor is returned which contains samples from all the
                 measured qubits, independently of their registers.
         """
         qubits = self.measurement_gate.target_qubits
         if self._samples is None:
             if self.measurements[0].result.has_samples():
-                self._samples = np.concatenate(
+                self._samples = self.backend.np.concatenate(
                     [gate.result.samples() for gate in self.measurements], axis=1
                 )
             else:
                 if self._frequencies is not None:
                     # generate samples that respect the existing frequencies
                     frequencies = self.frequencies(binary=False)
                     samples = np.concatenate(
@@ -349,15 +349,15 @@
                     samples = self.backend.apply_bitflips(
                         samples, bitflip_probabilities
                     )
                 # register samples to individual gate ``MeasurementResult``
                 qubit_map = {
                     q: i for i, q in enumerate(self.measurement_gate.target_qubits)
                 }
-                self._samples = np.array(samples, dtype="int32")
+                self._samples = self.backend.cast(samples, "int32")
                 for gate in self.measurements:
                     rqubits = tuple(qubit_map.get(q) for q in gate.target_qubits)
                     gate.result.register_samples(
                         self._samples[:, rqubits], self.backend
                     )
 
         if registers:
```

### Comparing `qibo-0.2.6/src/qibo/solvers.py` & `qibo-0.2.7/src/qibo/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     Calculates the evolution operator in every step and thus is compatible with
     time-dependent Hamiltonians.
     """
 
     def __call__(self, state):
         propagator = self.current_hamiltonian.exp(self.dt)
         self.t += self.dt
-        return (propagator @ state[:, self.backend.np.newaxis])[:, 0]
+        return (propagator @ state[:, None])[:, 0]
 
 
 class RungeKutta4(BaseSolver):
     """Solver based on the 4th order Runge-Kutta method."""
 
     def __call__(self, state):
         ham1 = self.current_hamiltonian
```

### Comparing `qibo-0.2.6/src/qibo/symbols.py` & `qibo-0.2.7/src/qibo/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             may lead to wrong results. It is useful for improving performance
             in symbolic calculations in cases where the user is sure that
             the operators participating in the Hamiltonian form are commuting
             (for example when the Hamiltonian consists of Z terms only).
     """
 
     def __new__(cls, q, matrix=None, name="Symbol", commutative=False, **assumptions):
-        name = "{}{}".format(name, q)
+        name = f"{name}{q}"
         assumptions["commutative"] = commutative
         return super().__new__(cls=cls, name=name, **assumptions)
 
     def __init__(self, q, matrix=None, name="Symbol", commutative=False):
         self.target_qubit = q
         self._gate = None
         if not (
@@ -59,17 +59,15 @@
                     np.float32,
                     np.float64,
                     np.complex64,
                     np.complex128,
                 ),
             )
         ):
-            raise_error(
-                TypeError, "Invalid type {} of symbol matrix." "".format(type(matrix))
-            )
+            raise_error(TypeError, f"Invalid type {type(matrix)} of symbol matrix.")
         self.matrix = matrix
 
     def __getstate__(self):
         return {
             "target_qubit": self.target_qubit,
             "matrix": self.matrix,
             "name": self.name,
```

### Comparing `qibo-0.2.6/src/qibo/transpiler/_exceptions.py` & `qibo-0.2.7/src/qibo/transpiler/_exceptions.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/abstract.py` & `qibo-0.2.7/src/qibo/transpiler/abstract.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/blocks.py` & `qibo-0.2.7/src/qibo/transpiler/blocks.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/decompositions.py` & `qibo-0.2.7/src/qibo/transpiler/decompositions.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/optimizer.py` & `qibo-0.2.7/src/qibo/transpiler/optimizer.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/pipeline.py` & `qibo-0.2.7/src/qibo/transpiler/pipeline.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/placer.py` & `qibo-0.2.7/src/qibo/transpiler/placer.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/router.py` & `qibo-0.2.7/src/qibo/transpiler/router.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/src/qibo/transpiler/unroller.py` & `qibo-0.2.7/src/qibo/transpiler/unroller.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.6/PKG-INFO` & `qibo-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: qibo
-Version: 0.2.6
+Version: 0.2.7
 Summary: A framework for quantum computing with hardware acceleration.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: qinfo
 Provides-Extra: tensorflow
+Provides-Extra: torch
 Requires-Dist: cma (>=3.3.0,<4.0.0)
 Requires-Dist: cvxpy (>=1.4.2,<2.0.0) ; extra == "qinfo"
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openqasm3[parser] (>=0.5.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tensorflow (>=2.14.1,<2.16) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "tensorflow")
+Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "torch"
 Project-URL: Documentation, https://qibo.science/docs/qibo/stable
 Project-URL: Repository, https://github.com/qiboteam/qibo/
 Description-Content-Type: text/markdown
 
 ![Logo](https://github.com/qiboteam/qibo/blob/master/doc/source/_static/qibo_logo_dark.svg)
 
 [![codecov](https://codecov.io/gh/qiboteam/qibo/branch/master/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibo)
```

