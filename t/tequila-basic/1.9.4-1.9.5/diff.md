# Comparing `tmp/tequila-basic-1.9.4.tar.gz` & `tmp/tequila-basic-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tequila-basic-1.9.4.tar", last modified: Thu Feb 29 10:11:07 2024, max compression
+gzip compressed data, was "tequila-basic-1.9.5.tar", last modified: Fri Apr  5 11:50:58 2024, max compression
```

## Comparing `tequila-basic-1.9.4.tar` & `tequila-basic-1.9.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.204724 tequila-basic-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-02-29 10:11:07.200724 tequila-basic-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18764 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-29 10:11:06.000000 tequila-basic-1.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 10:11:07.204724 tequila-basic-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.180724 tequila-basic-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21757 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/_unary_state_prep_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/apps/adapt/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19529 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/adapt/adapt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/apps/krylov/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/krylov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/krylov/krylov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/apps/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/robustness/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/robustness/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/apps/unary_state_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/autograd_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.184724 tequila-basic-1.9.4/src/tequila/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/_gates_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    32044 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    32685 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    35906 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/pyzx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/circuit/qpic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.188724 tequila-basic-1.9.4/src/tequila/grouping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19406 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/binary_rep.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    66415 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/compile_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/ev_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34109 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/fermionic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27807 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/fermionic_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/grouping/overlapping_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.188724 tequila-basic-1.9.4/src/tequila/hamiltonian/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/hamiltonian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/hamiltonian/paulis.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/hamiltonian/paulistring.py
--rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/hamiltonian/qubit_hamiltonian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.188724 tequila-basic-1.9.4/src/tequila/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/ml/interface_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/ml/ml_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/ml/utils_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.188724 tequila-basic-1.9.4/src/tequila/objective/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/objective/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    31763 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/objective/qtensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.192724 tequila-basic-1.9.4/src/tequila/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32272 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/optimizer_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    39059 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/optimizer_gd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/optimizer_gpyopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18949 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/optimizers/optimizer_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.192724 tequila-basic-1.9.4/src/tequila/quantumchemistry/
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40960 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/chemistry_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/madness_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/orbital_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29953 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/psi4_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/pyscf_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    92908 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/quantumchemistry/qc_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.192724 tequila-basic-1.9.4/src/tequila/simulators/
--rwxr-xr-x   0 runner    (1001) docker     (127)        4 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24172 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33174 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16535 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_cirq.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24240 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_pyquil.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25095 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_qibo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23429 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_qlm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19728 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_qulacs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      659 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_qulacs_gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5220 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/simulators/simulator_symbolic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.196724 tequila-basic-1.9.4/src/tequila/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/tools/convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/tools/qng.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/tools/random_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.196724 tequila-basic-1.9.4/src/tequila/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/joined_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/keymap.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.196724 tequila-basic-1.9.4/src/tequila/wavefunction/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/wavefunction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/src/tequila/wavefunction/qubit_wavefunction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.200724 tequila-basic-1.9.4/src/tequila_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-02-29 10:11:07.000000 tequila-basic-1.9.4/src/tequila_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-29 10:11:07.000000 tequila-basic-1.9.4/src/tequila_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:11:07.000000 tequila-basic-1.9.4/src/tequila_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-29 10:11:07.000000 tequila-basic-1.9.4/src/tequila_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 10:11:07.000000 tequila-basic-1.9.4/src/tequila_basic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:11:07.200724 tequila-basic-1.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_TrotErr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_adapt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_binary_pauli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_chemistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_chemistry_f12.py
--rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_chemistry_madness.py
--rw-r--r--   0 runner    (1001) docker     (127)    14538 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_circuits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_fermionic_meas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_gd_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_gpyopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_hamiltonian_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_krylov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_noise_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    32601 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_pyzx.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_qtensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_recompilation_routines.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_simulator_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_symbolic_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_torch_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_unary_state_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-29 10:10:55.000000 tequila-basic-1.9.4/tests/test_zzz_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.850885 tequila-basic-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19691 2024-04-05 11:50:58.846885 tequila-basic-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19165 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:50:58.850885 tequila-basic-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.822885 tequila-basic-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.822885 tequila-basic-1.9.5/src/tequila/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.826885 tequila-basic-1.9.5/src/tequila/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21757 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/_unary_state_prep_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.826885 tequila-basic-1.9.5/src/tequila/apps/adapt/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19529 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/adapt/adapt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.826885 tequila-basic-1.9.5/src/tequila/apps/krylov/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/krylov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/krylov/krylov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.826885 tequila-basic-1.9.5/src/tequila/apps/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/robustness/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24735 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/robustness/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/apps/unary_state_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/autograd_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.826885 tequila-basic-1.9.5/src/tequila/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/_gates_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32044 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32685 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35906 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/pyzx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15418 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/circuit/qpic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.830885 tequila-basic-1.9.5/src/tequila/grouping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19406 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/binary_rep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66415 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/compile_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/ev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34109 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/fermionic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27807 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/fermionic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/grouping/overlapping_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.830885 tequila-basic-1.9.5/src/tequila/hamiltonian/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/hamiltonian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/hamiltonian/paulis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/hamiltonian/paulistring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/hamiltonian/qubit_hamiltonian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.830885 tequila-basic-1.9.5/src/tequila/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/ml/interface_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/ml/ml_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/ml/utils_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.834885 tequila-basic-1.9.5/src/tequila/objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/objective/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31763 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/objective/qtensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.834885 tequila-basic-1.9.5/src/tequila/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32272 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/optimizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39059 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/optimizer_gd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/optimizer_gpyopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18949 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/optimizers/optimizer_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.834885 tequila-basic-1.9.5/src/tequila/quantumchemistry/
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41353 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/chemistry_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/madness_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/orbital_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29953 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/psi4_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/pyscf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96531 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/quantumchemistry/qc_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.838885 tequila-basic-1.9.5/src/tequila/simulators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        4 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24172 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33174 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16535 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_cirq.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24240 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_pyquil.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25095 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_qibo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23429 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_qlm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19728 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_qulacs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      659 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_qulacs_gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5220 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/simulators/simulator_symbolic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.838885 tequila-basic-1.9.5/src/tequila/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/tools/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/tools/qng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/tools/random_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.838885 tequila-basic-1.9.5/src/tequila/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/joined_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.842885 tequila-basic-1.9.5/src/tequila/wavefunction/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/wavefunction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/src/tequila/wavefunction/qubit_wavefunction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.846885 tequila-basic-1.9.5/src/tequila_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19691 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/src/tequila_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/src/tequila_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/src/tequila_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/src/tequila_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 11:50:58.000000 tequila-basic-1.9.5/src/tequila_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:50:58.846885 tequila-basic-1.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_TrotErr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_binary_pauli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_chemistry_f12.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_chemistry_madness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14538 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_circuits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_fermionic_meas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_gd_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_gpyopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_hamiltonian_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_krylov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_noise_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32601 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_pyzx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_qtensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_recompilation_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_simulator_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_symbolic_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_torch_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_unary_state_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 11:50:50.000000 tequila-basic-1.9.5/tests/test_zzz_cleanup.py
```

### Comparing `tequila-basic-1.9.4/LICENSE` & `tequila-basic-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/PKG-INFO` & `tequila-basic-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tequila-basic
-Version: 1.9.4
+Version: 1.9.5
 Summary: A High-Level Abstraction Framework for Quantum Algorithms
 Home-page: https://github.com/tequilahub/tequila
 Author: Tequila Developers 
 Author-email: jakob.kottmann@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -28,15 +28,15 @@
 - [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
 - [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
 - [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
 - [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
 - [talks and slides](https://kottmanj.github.io/talks_and_material/)  
 
 # Installation
-Recommended Python version is 3.8-3.9.   
+Recommended Python version is 3.9 - 3.10.   
 Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.  
 
 ## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
 You can install tequila from PyPi as:
@@ -254,14 +254,22 @@
 Boosting quantum amplitude exponentially in variational quantum algorithms  
 [10.1088/2058-9565/acf4ba](doi.org/10.1088/2058-9565/acf4ba)  
 
 A.G. Cadavid, I. Montalban, A. Dalal, E. Solano, N.N. Hegade  
 Efficient DCQO Algorithm within the Impulse Regime for Portfolio Optimization  
 [arxiv:2308.15475](https://arxiv.org/abs/2308.15475)  
 
+A. Anand, K. Brown  
+Hamiltonians, groups, graphs and ansätze  
+[arxiv:2312.17146](https://arxiv.org/abs/2312.17146)  
+
+P.W.K. Jensen, E.R. Kjellgren, P. Reinholdt, K.M. Ziems, S. Coriani, J. Kongsted, S. Sauer  
+Quantum Equation of Motion with Orbital Optimization for Computing Molecular Properties in Near-Term Quantum Computing  
+[arxiv:2312.12386](https://arxiv.org/abs/2312.12386)  
+
 Let us know, if you want your research project and/or tutorial to be included in this list!
 
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
@@ -281,15 +289,15 @@
 For best performance it is recommended to have `qulacs` installed.
 
 ## QuantumChemistry:
 Currently supported
 ### [Psi4](https://github.com/psi4/psi4).
 In a conda environment this can be installed with
 ```bash
-conda install psi4 -c psi4
+conda install psi4 -c conda-forge
 ```
 Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
 
 ### [Madness](https://github.com/kottmanj/madness)  
 In a conda environment this can be installed with  
 ```bash
 conda install madtequila -c kottmann
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tequila-basic-1.9.4/README.md` & `tequila-basic-1.9.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
 - [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
 - [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
 - [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
 - [talks and slides](https://kottmanj.github.io/talks_and_material/)  
 
 # Installation
-Recommended Python version is 3.8-3.9.   
+Recommended Python version is 3.9 - 3.10.   
 Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.  
 
 ## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
 You can install tequila from PyPi as:
@@ -236,14 +236,22 @@
 Boosting quantum amplitude exponentially in variational quantum algorithms  
 [10.1088/2058-9565/acf4ba](doi.org/10.1088/2058-9565/acf4ba)  
 
 A.G. Cadavid, I. Montalban, A. Dalal, E. Solano, N.N. Hegade  
 Efficient DCQO Algorithm within the Impulse Regime for Portfolio Optimization  
 [arxiv:2308.15475](https://arxiv.org/abs/2308.15475)  
 
+A. Anand, K. Brown  
+Hamiltonians, groups, graphs and ansätze  
+[arxiv:2312.17146](https://arxiv.org/abs/2312.17146)  
+
+P.W.K. Jensen, E.R. Kjellgren, P. Reinholdt, K.M. Ziems, S. Coriani, J. Kongsted, S. Sauer  
+Quantum Equation of Motion with Orbital Optimization for Computing Molecular Properties in Near-Term Quantum Computing  
+[arxiv:2312.12386](https://arxiv.org/abs/2312.12386)  
+
 Let us know, if you want your research project and/or tutorial to be included in this list!
 
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
@@ -263,15 +271,15 @@
 For best performance it is recommended to have `qulacs` installed.
 
 ## QuantumChemistry:
 Currently supported
 ### [Psi4](https://github.com/psi4/psi4).
 In a conda environment this can be installed with
 ```bash
-conda install psi4 -c psi4
+conda install psi4 -c conda-forge
 ```
 Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
 
 ### [Madness](https://github.com/kottmanj/madness)  
 In a conda environment this can be installed with  
 ```bash
 conda install madtequila -c kottmann
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tequila-basic-1.9.4/requirements.txt` & `tequila-basic-1.9.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/setup.py` & `tequila-basic-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/__init__.py` & `tequila-basic-1.9.5/src/tequila/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/__init__.py` & `tequila-basic-1.9.5/src/tequila/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/_unary_state_prep_impl.py` & `tequila-basic-1.9.5/src/tequila/apps/_unary_state_prep_impl.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/adapt/adapt.py` & `tequila-basic-1.9.5/src/tequila/apps/adapt/adapt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/krylov/krylov.py` & `tequila-basic-1.9.5/src/tequila/apps/krylov/krylov.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/robustness/helpers.py` & `tequila-basic-1.9.5/src/tequila/apps/robustness/helpers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/robustness/interval.py` & `tequila-basic-1.9.5/src/tequila/apps/robustness/interval.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/apps/unary_state_prep.py` & `tequila-basic-1.9.5/src/tequila/apps/unary_state_prep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/autograd_imports.py` & `tequila-basic-1.9.5/src/tequila/autograd_imports.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/_gates_impl.py` & `tequila-basic-1.9.5/src/tequila/circuit/_gates_impl.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/circuit.py` & `tequila-basic-1.9.5/src/tequila/circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/compiler.py` & `tequila-basic-1.9.5/src/tequila/circuit/compiler.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/gates.py` & `tequila-basic-1.9.5/src/tequila/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/gradient.py` & `tequila-basic-1.9.5/src/tequila/circuit/gradient.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/noise.py` & `tequila-basic-1.9.5/src/tequila/circuit/noise.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/pyzx.py` & `tequila-basic-1.9.5/src/tequila/circuit/pyzx.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/qasm.py` & `tequila-basic-1.9.5/src/tequila/circuit/qasm.py`

 * *Files 3% similar despite different names*

```diff
@@ -309,27 +309,41 @@
         custom_circuit = custom_gates_map[name]
         qregisters_values = []
         for a in args:
             qregisters_values.append(get_qregister(a, qregisters))
         return apply_custom_gate(custom_circuit=custom_circuit, qregisters_values=qregisters_values)
 
     if name in ("x", "y", "z", "h", "cx", "cy", "cz", "ch"):
-        return QCircuit.wrap_gate(gates.impl.QGateImpl(name=(name[1] if name[0] == 'c' else name).upper(),
-                                            control=get_qregister(args[0], qregisters) if name[0] == 'c' else None,
-                                            target=get_qregister(args[1 if name[0] == 'c' else 0], qregisters)))
+        target = get_qregister(args[0], qregisters)
+        control = None
+        if name[0].lower() == 'c':
+            control = get_qregister(args[0], qregisters)
+            target = get_qregister(args[1], qregisters)
+            name = name[1]
+        G = getattr(gates, name.upper())
+        return G(control=control, target=target)
+
     if name in ("ccx", "ccy", "ccz"):
-        return QCircuit.wrap_gate(gates.impl.QGateImpl(name=name.upper()[2],
-                                            control=[get_qregister(args[0], qregisters), get_qregister(args[1], qregisters)],
-                                            target=get_qregister(args[2], qregisters)))
+        G = getattr(gates, name[2].upper())
+        control = [get_qregister(args[0], qregisters), get_qregister(args[1], qregisters)]
+        target = get_qregister(args[2], qregisters)
+        return G(control=control, target=target)
+
     if name.startswith("rx(") or name.startswith("ry(") or name.startswith("rz(") or \
         name.startswith("crx(") or name.startswith("cry(") or name.startswith("crz("):
-        return QCircuit.wrap_gate(gates.impl.RotationGateImpl(axis=name[2 if name[0] == 'c' else 1],
-                                                   angle=get_angle(name)[0],
-                                                   control=get_qregister(args[0], qregisters) if name[0] == 'c' else None,
-                                                   target=get_qregister(args[1 if name[0] == 'c' else 0], qregisters)))
+        angle = get_angle(name)[0]
+        i = name.find('(')
+        name = name[0:i]
+        name = name.upper()
+        name = [x for x in name]
+        name[-1] = name[-1].lower()
+        name = "".join(name)
+        G = getattr(gates, name)
+        return G(angle=angle,control=get_qregister(args[0], qregisters) if name[0] == 'C' else None,target=get_qregister(args[1 if name[0] == 'C' else 0], qregisters))
+            
     if name.startswith("U("):
         angles = get_angle(name)
         return gates.U(theta=angles[0], phi=angles[1], lambd=angles[2],
                  control=None,
                  target=get_qregister(args[0], qregisters))
     if name.startswith("u1("):
         angles = get_angle(name)
@@ -358,15 +372,15 @@
                   target=get_qregister(args[1], qregisters))
     if name.startswith("cu3("):
         angles = get_angle(name)
         return gates.u3(theta=angles[0], phi=angles[1], lambd=angles[2],
                   control=get_qregister(args[0], qregisters),
                   target=get_qregister(args[1], qregisters))
     if name in ("s", "t", "sdg", "tdg"):
-        g = gates.Phase(pi / (2 if name.startswith("s") else 4),
+        g = gates.Phase(angle=pi / (2 if name.startswith("s") else 4),
                      control=None,
                      target=get_qregister(args[0], qregisters))
         if name.find("dg") != -1:
             g = g.dagger()
         return g
```

### Comparing `tequila-basic-1.9.4/src/tequila/circuit/qpic.py` & `tequila-basic-1.9.5/src/tequila/circuit/qpic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/binary_rep.py` & `tequila-basic-1.9.5/src/tequila/grouping/binary_rep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/binary_utils.py` & `tequila-basic-1.9.5/src/tequila/grouping/binary_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/compile_groups.py` & `tequila-basic-1.9.5/src/tequila/grouping/compile_groups.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/ev_utils.py` & `tequila-basic-1.9.5/src/tequila/grouping/ev_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/fermionic_functions.py` & `tequila-basic-1.9.5/src/tequila/grouping/fermionic_functions.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/fermionic_methods.py` & `tequila-basic-1.9.5/src/tequila/grouping/fermionic_methods.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/grouping/overlapping_methods.py` & `tequila-basic-1.9.5/src/tequila/grouping/overlapping_methods.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/hamiltonian/paulis.py` & `tequila-basic-1.9.5/src/tequila/hamiltonian/paulis.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/hamiltonian/qubit_hamiltonian.py` & `tequila-basic-1.9.5/src/tequila/hamiltonian/qubit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/ml/interface_torch.py` & `tequila-basic-1.9.5/src/tequila/ml/interface_torch.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/ml/ml_api.py` & `tequila-basic-1.9.5/src/tequila/ml/ml_api.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/ml/utils_ml.py` & `tequila-basic-1.9.5/src/tequila/ml/utils_ml.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/objective/braket.py` & `tequila-basic-1.9.5/src/tequila/objective/braket.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/objective/objective.py` & `tequila-basic-1.9.5/src/tequila/objective/objective.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/objective/qtensor.py` & `tequila-basic-1.9.5/src/tequila/objective/qtensor.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/__init__.py` & `tequila-basic-1.9.5/src/tequila/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/_containers.py` & `tequila-basic-1.9.5/src/tequila/optimizers/_containers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/optimizer_base.py` & `tequila-basic-1.9.5/src/tequila/optimizers/optimizer_base.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/optimizer_gd.py` & `tequila-basic-1.9.5/src/tequila/optimizers/optimizer_gd.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/optimizer_gpyopt.py` & `tequila-basic-1.9.5/src/tequila/optimizers/optimizer_gpyopt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/optimizers/optimizer_scipy.py` & `tequila-basic-1.9.5/src/tequila/optimizers/optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/__init__.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     integrals_provided = all([key in kwargs for key in ["one_body_integrals", "two_body_integrals"]])
     if integrals_provided and backend is None:
         backend = "base"
 
     if backend is None:
         if basis_set is None or basis_set.lower() in ["madness", "mra", "pno"]:
             backend = "madness"
+            basis_set = "mra"
+            parameters.basis_set = basis_set
             if orbital_type is not None and orbital_type.lower() not in ["pno", "mra-pno"]:
                 warnings.warn("only PNOs supported as orbital_type without basis set. Setting to pno - You gave={}".format(orbital_type), TequilaWarning)
             orbital_type = "pno"
         else:
             if orbital_type is not None and orbital_type.lower() not in ["hf", "native"]:
                 warnings.warn("only hf and native supported as orbital_type with basis-set. Setting to hf - You gave={}".format(orbital_type), TequilaWarning)
                 orbital_type = "hf"
```

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/chemistry_tools.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/chemistry_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -800,28 +800,26 @@
     All integrals are held in their original basis, the corresponding mo-coefficients have to be passed down
     and are usually held by the QuantumChemistryBaseClass
     """
     _overlap_integrals: numpy.ndarray = None
     _one_body_integrals: numpy.ndarray = None
     _two_body_integrals: NBodyTensor = None
     _constant_term: float = None
-    _basis_type: str = "unknown"
     _basis_name: str = "unknown"
     _orbital_type: str = "unknown" # e.g. "HF", "PNO", "native"
     _orbital_coefficients: numpy.ndarray = None
     _active_space: ActiveSpaceData = None
     _orbitals: typing.List[OrbitalData] = None
 
-    def __init__(self, one_body_integrals, two_body_integrals, basis_type="custom",
+    def __init__(self, one_body_integrals, two_body_integrals,
                  basis_name="unknown", orbital_type="unknown",
                  constant_term=0.0, orbital_coefficients=None, active_space=None, overlap_integrals=None, orbitals=None, *args, **kwargs):
         self._one_body_integrals = one_body_integrals
         self._two_body_integrals = two_body_integrals
         self._constant_term = constant_term
-        self._basis_type = basis_type
         self._basis_name = basis_name
         self._orbital_type = orbital_type
 
         assert len(self._one_body_integrals.shape) == 2
         assert len(self._two_body_integrals.shape) == 4
         try:
             two_body_integrals = two_body_integrals.reorder(to="chem")
@@ -952,31 +950,40 @@
     
     def transform_to_native_orbitals(self):
         """
         Transform orbitals to orthonormal functions closest to the native basis
         """
         c = self.get_orthonormalized_orbital_coefficients()
         self.orbital_coefficients=c
-        self._orbital_type="orthonormalized-{}-basis".format(self._orbital_type)
+        self._orbital_type="orthonormalized-{}-basis".format(self._basis_name)
 
-    def transform_orbitals(self, U):
+    def is_unitary(self, U):
+        if len(U.shape) != 2: return False
+        if U.shape[0] != U.shape[1]: return False
+        test = (U.conj().T).dot(U) - numpy.eye(U.shape[0])
+        if not numpy.isclose(numpy.linalg.norm(test), 0.0): return False
+        return True
+
+    def transform_orbitals(self, U, name=None):
         """
         Transform orbitals
         Parameters
         ----------
         U: second index is new orbital indes, first is old orbital index (summed over)
 
         Returns
         -------
         updates the structure with new orbitals: c = cU
         """
-        c = self.orbital_coefficients
-        c = numpy.einsum("ix, xj -> ij", c, U, optimize="greedy")
-        self.orbital_coefficients = c
-        self._orbital_type += "-transformed"
+        assert self.is_unitary(U)
+        self.orbital_coefficients = numpy.einsum("ix, xj -> ij", self.orbital_coefficients, U, optimize="greedy")
+        if name is None:
+            self._orbital_type += "-transformed"
+        else:
+            self._orbital_type = name
 
     def get_integrals(self, orbital_coefficients=None, ordering="openfermion", ignore_active_space=False, *args, **kwargs):
         """
         Get all molecular integrals in given orbital basis (determined by orbital_coefficients in self or the ones passed here)
         active space is considered if not explicitly ignored
         Parameters
         ----------
@@ -997,15 +1004,17 @@
         if not ignore_active_space and self._active_space is not None:
 
             g = g.reorder(to="openfermion").elems
 
             active_integrals = get_active_space_integrals(one_body_integrals=h, two_body_integrals=g,
                                                           occupied_indices=self._active_space.frozen_reference_orbitals,
                                                           active_indices=self._active_space.active_orbitals)
+
             c = active_integrals[0] + c
+
             h = active_integrals[1]
             g = NBodyTensor(elems=active_integrals[2], ordering="openfermion")
         g.reorder(to=ordering)
         return c, h, g
 
     def _get_transformed_one_body_integrals(self, orbital_coefficients=None, verify=True):
         if orbital_coefficients is None:
@@ -1065,19 +1074,21 @@
         result+= "ActiveSpace:\n"
         result+= str(self.active_space)
         result+= "Orbitals:\n"
         for x in self.orbitals:
             result += str(x) + "\n"
         return result
 
-    def print_basis_info(self, *args, **kwargs) -> None:
-        print("{:15} : {}".format("basis_type", self._basis_type), *args, **kwargs)
+    def print_basis_info(self, print_coefficients=True, *args, **kwargs) -> None:
         print("{:15} : {}".format("basis_name", self._basis_name), *args, **kwargs)
         print("{:15} : {}".format("orbital_type", self._orbital_type), *args, **kwargs)
-        print("{:15} : {}".format("orthogonal", self.basis_is_orthogonal()), *args, **kwargs)
-        print("{:15} : {}".format("functions", self.one_body_integrals.shape[0]), *args, **kwargs)
+        print("{:15} : {}".format("orthogonal basis", self.basis_is_orthogonal()), *args, **kwargs)
+        print("{:15} : {}".format("basis functions", self.one_body_integrals.shape[0]), *args, **kwargs)
+        print("{:15} : {}".format("active orbitals", [o.idx_total for o in self.active_orbitals]), *args, **kwargs)
         print("{:15} : {}".format("reference", [x.idx_total for x in self.reference_orbitals]), *args, **kwargs)
 
+        if not print_coefficients: return
+
         print("Current Orbitals", *args, **kwargs)
         for i,x in enumerate(self.orbitals):
             print(x, *args, **kwargs)
             print("coefficients: ", self.orbital_coefficients[:,i], *args, **kwargs)
```

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/encodings.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/encodings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/madness_interface.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/madness_interface.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/orbital_optimizer.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/orbital_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         # use as callback
         if "u" in local_data:
             self.rotation_matrix = copy.deepcopy(local_data["u"])
         self.mcscf_local_data=local_data
         self.iterations += 1
 
 def optimize_orbitals(molecule, circuit=None, vqe_solver=None, pyscf_arguments=None, silent=False,
-                      vqe_solver_arguments=None, initial_guess=None, return_mcscf=False, use_hcb=False, molecule_factory=None, molecule_arguments=None, *args, **kwargs):
+                      vqe_solver_arguments=None, initial_guess=None, return_mcscf=False, use_hcb=False, molecule_factory=None, molecule_arguments=None, restrict_to_active_space=True, *args, **kwargs):
     """
 
     Parameters
     ----------
     molecule: The tequila molecule whose orbitals are to be optimized
     circuit: The circuit that defines the ansatz to the wavefunction in the VQE
              can be None, if a customized vqe_solver is passed that can construct a circuit
@@ -74,15 +74,20 @@
         from . import QuantumChemistryPySCF
     except Exception as exception:
         raise Exception("{}\noptimize_orbitals: Need pyscf to run (pip install pyscf)".format(str(exception)))
 
     if pyscf_arguments is None:
         pyscf_arguments = {"max_cycle_macro": 10, "max_cycle_micro": 3}
     no = molecule.n_orbitals
-    pyscf_molecule = QuantumChemistryPySCF.from_tequila(molecule=molecule, transformation=molecule.transformation)
+
+    if not isinstance(molecule, QuantumChemistryPySCF):
+        pyscf_molecule = QuantumChemistryPySCF.from_tequila(molecule=molecule, transformation=molecule.transformation)
+    else:
+        pyscf_molecule = molecule
+
     mf = pyscf_molecule._get_hf()
     result=OptimizeOrbitalsResult()
     mc = mcscf.CASSCF(mf, pyscf_molecule.n_orbitals, pyscf_molecule.n_electrons)
     mc.callback=result
     c = pyscf_molecule.compute_constant_part()
 
     if circuit is None and vqe_solver is None:
@@ -136,18 +141,19 @@
         assert initial_guess.shape[1] == no
         initial_guess = mcscf.project_init_guess(mc, initial_guess)
         mc.kernel(mo_coeff=initial_guess)
     else:
         mc.kernel()
     # make new molecule
 
-    transformed_molecule = pyscf_molecule.transform_orbitals(orbital_coefficients=mc.mo_coeff)
+    mo_coeff = mc.mo_coeff
+    transformed_molecule = pyscf_molecule.transform_orbitals(orbital_coefficients=mo_coeff, name="optimized")
     result.molecule=transformed_molecule
     result.old_molecule=molecule
-    result.mo_coeff=mc.mo_coeff
+    result.mo_coeff=mo_coeff
     result.energy=mc.e_tot
     
     if return_mcscf:
         result.mcscf_object = mc
     
     return result
```

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/psi4_interface.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/psi4_interface.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/pyscf_interface.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/pyscf_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             self.pyscf_molecule = mol
             self.point_group = mol.symmetry_subgroup
 
             kwargs["overlap_integrals"] = S
             kwargs["two_body_integrals"] = g_ao
             kwargs["one_body_integrals"] = h_ao
             kwargs["orbital_coefficients"] = mo_coeff
+            kwargs["orbital_type"] = "hf"
 
             if "nuclear_repulsion" not in kwargs:
                 kwargs["nuclear_repulsion"] = mol.energy_nuc()
 
         super().__init__(parameters=parameters, transformation=transformation, *args, **kwargs)
 
     def compute_fci(self, *args, **kwargs):
```

### Comparing `tequila-basic-1.9.4/src/tequila/quantumchemistry/qc_base.py` & `tequila-basic-1.9.5/src/tequila/quantumchemistry/qc_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,38 +90,46 @@
 
         # initialize integral manager
         if "integral_manager" in kwargs:
             self.integral_manager = kwargs["integral_manager"]
         else:
             self.integral_manager = self.initialize_integral_manager(active_orbitals=active_orbitals,
                                                                      reference_orbitals=reference_orbitals,
-                                                                     orbitals=orbitals, frozen_orbitals=frozen_orbitals, orbital_type=orbital_type, *args,
+                                                                     orbitals=orbitals, frozen_orbitals=frozen_orbitals, orbital_type=orbital_type, basis_name=self.parameters.basis_set, *args,
                                                                      **kwargs)
         
         if orbital_type is not None and orbital_type.lower() == "native":
             self.integral_manager.transform_to_native_orbitals()
 
 
         self.transformation = self._initialize_transformation(transformation=transformation, *args, **kwargs)
 
         self._rdm1 = None
         self._rdm2 = None
 
 
     @classmethod
     def from_tequila(cls, molecule, transformation=None, *args, **kwargs):
-        c, h1, h2 = molecule.get_integrals()
+        c = molecule.integral_manager.constant_term
+        h1 = molecule.integral_manager.one_body_integrals
+        h2 = molecule.integral_manager.two_body_integrals
+        S = molecule.integral_manager.overlap_integrals
+        active_orbitals = [o.idx_total for o in molecule.integral_manager.active_orbitals]
         if transformation is None:
             transformation = molecule.transformation
+        parameters = molecule.parameters
         return cls(nuclear_repulsion=c,
                    one_body_integrals=h1,
                    two_body_integrals=h2,
-                   n_electrons=molecule.n_electrons,
+                   overlap_integrals = S,
+                   orbital_coefficients = molecule.integral_manager.orbital_coefficients,
+                   active_orbitals= active_orbitals,
                    transformation=transformation,
-                   parameters=molecule.parameters, *args, **kwargs)
+                   orbital_type=molecule.integral_manager._orbital_type,
+                   parameters=parameters, *args, **kwargs)
 
     def supports_ucc(self):
         """
         check if the current molecule supports UCC operations
         (e.g. mol.make_excitation_gate)
         """
         return self.transformation.supports_ucc
@@ -539,30 +547,43 @@
             kwargs["basis_name"] = self.parameters.basis_set
 
         manager = IntegralManager(one_body_integrals=one_body_integrals, two_body_integrals=two_body_integrals,
                                   constant_term=constant_part, *args, **kwargs)
 
         return manager
 
-    def transform_orbitals(self, orbital_coefficients, *args, **kwargs):
+    def transform_orbitals(self, orbital_coefficients, ignore_active_space=False, name=None, *args, **kwargs):
         """
         Parameters
         ----------
-        orbital_coefficients: second index is new orbital indes, first is old orbital index (summed over)
+        orbital_coefficients: second index is new orbital indes, first is old orbital index (summed over), indices are assumed to be defined on the active space
+        ignore_active_space: if true orbital_coefficients are not assumed to be given in the active space
+        name: str, name the new orbitals
         args
         kwargs
 
         Returns
         -------
         New molecule with transformed orbitals
         """
 
+        U = numpy.eye(self.integral_manager.orbital_coefficients.shape[0])
+        # mo_coeff by default only acts on the active space
+        active_indices = [o.idx_total for o in self.integral_manager.active_orbitals]
+
+        if ignore_active_space:
+            U = orbital_coefficients
+        else:
+            for kk,k in enumerate(active_indices):
+                for ll,l in enumerate(active_indices):
+                    U[k][l] = orbital_coefficients[kk][ll]
+
         # can not be an instance of a specific backend (otherwise we get inconsistencies with classical methods in the backend)
         integral_manager = copy.deepcopy(self.integral_manager)
-        integral_manager.transform_orbitals(U=orbital_coefficients)
+        integral_manager.transform_orbitals(U=U, name=name)
         result = QuantumChemistryBase(parameters=self.parameters, integral_manager=integral_manager, transformation=self.transformation)
         return result
     
     def orthonormalize_basis_orbitals(self):
         # backward compatibility
         return self.use_native_orbitals()
     
@@ -579,15 +600,15 @@
         # can not be an instance of a specific backend (otherwise we get inconsistencies with classical methods in the backend)
         if inplace:
             self.integral_manager.transform_to_native_orbitals()
             return self
         else:
             integral_manager = copy.deepcopy(self.integral_manager)
             integral_manager.transform_to_native_orbitals()
-            result = QuantumChemistryBase(parameters=self.parameters, integral_manager=integral_manager, orbital_type="native", transformation=self.transformation)
+            result = QuantumChemistryBase(parameters=self.parameters, integral_manager=integral_manager, transformation=self.transformation)
             return result
 
 
     def do_make_molecule(self, *args, **kwargs):
         """
         Called by self.make_molecule with args and kwargs passed through
         Override this in derived class if needed
@@ -641,14 +662,76 @@
         """
         Returns
         -------
         The number of active electrons in this molecule
         """
         return 2 * len(self.integral_manager.active_reference_orbitals)
 
+    def make_annihilation_op(self, orbital, coefficient=1.0):
+        """
+        Compute annihilation operator on spin-orbital in qubit representation
+        Spin-orbital order is always (up,down,up,down,...)
+        """
+        assert orbital<=self.n_orbitals*2
+        aop = openfermion.ops.FermionOperator(f'{orbital}', coefficient)
+        return self.transformation(aop)
+
+    def make_creation_op(self, orbital, coefficient=1.0):
+        """
+        Compute creation operator on spin-orbital in qubit representation
+        Spin-orbital order is always (up,down,up,down,...)
+        """
+        assert orbital<=self.n_orbitals*2
+        cop = openfermion.ops.FermionOperator(f'{orbital}^', coefficient)
+        return self.transformation(cop)
+
+    def make_number_op(self, orbital):
+        """
+        Compute number operator on spin-orbital in qubit representation
+        Spin-orbital order is always (up,down,up,down,...)
+        """
+        num_op = self.make_creation_op(orbital) * self.make_annihilation_op(orbital)
+        return num_op
+    
+    def make_sz_op(self):
+        """
+        Compute the spin_z operator of the molecule in qubit representation
+        """
+        sz = QubitHamiltonian()
+        for i in range(0, self.n_orbitals * 2, 2):
+            one = 0.5 * self.make_creation_op(i) * self.make_annihilation_op(i)
+            two = 0.5 * self.make_creation_op(i+1) * self.make_annihilation_op(i+1)
+            sz += (one - two)
+        return sz
+
+    def make_sp_op(self):
+        """
+        Compute the spin+ operator of the molecule in qubit representation
+        """
+        sp = QubitHamiltonian()
+        for i in range(self.n_orbitals):
+            sp += self.make_creation_op(i*2) * self.make_annihilation_op(i*2 + 1)
+        return sp
+
+    def make_sm_op(self):
+        """
+        Compute the spin- operator of the molecule in qubit representation
+        """
+        sm = QubitHamiltonian()
+        for i in range(self.n_orbitals):
+            sm += self.make_creation_op(i*2 + 1) * self.make_annihilation_op(i*2)
+        return sm
+
+    def make_s2_op(self):
+        """
+        Compute the spin^2 operator of the molecule in qubit representation
+        """
+        s2_op = self.make_sm_op() * self.make_sp_op() + self.make_sz_op() * (self.make_sz_op() + 1)
+        return s2_op
+
     def make_hamiltonian(self, *args, **kwargs) -> QubitHamiltonian:
         """
         Parameters
         ----------
         occupied_indices: will be auto-assigned according to specified active space. Can be overridden by passing specific lists (same as in open fermion)
         active_indices: will be auto-assigned according to specified active space. Can be overridden by passing specific lists (same as in open fermion)
 
@@ -801,21 +884,21 @@
         condensed: assume that incoming U is condensed (HCB on the first n_orbitals; and not, as for example in JW on the first n even orbitals)
         Returns
         -------
 
         """
         if U is None:
             U = QCircuit()
-
-        # consistency
-        consistency = [x < self.n_orbitals for x in U.qubits]
-        if not all(consistency):
-            warnings.warn(
-                "hcb_to_me: given circuit is not defined on the first {} qubits. Is this a HCB circuit?".format(
-                    self.n_orbitals))
+        else:
+            ups = [self.transformation.up(i.idx) for i in self.orbitals]
+            consistency = [x in ups for x in U.qubits]
+            if not all(consistency):
+                warnings.warn(
+                    "hcb_to_me: given circuit is not defined on all first {} qubits. Is this a HCB circuit?".format(
+                        self.n_orbitals))
 
         # map to alpha qubits
         if condensed:
             alpha_map = {k: self.transformation.up(k) for k in range(self.n_orbitals)}
             alpha_U = U.map_qubits(qubit_map=alpha_map)
         else:
             alpha_U = U
```

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_api.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_api.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_base.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_base.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_cirq.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_cirq.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_pyquil.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_pyquil.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_qibo.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_qibo.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_qiskit.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_qiskit.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_qlm.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_qlm.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_qulacs.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_qulacs.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_qulacs_gpu.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_qulacs_gpu.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/simulators/simulator_symbolic.py` & `tequila-basic-1.9.5/src/tequila/simulators/simulator_symbolic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/tools/convenience.py` & `tequila-basic-1.9.5/src/tequila/tools/convenience.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/tools/qng.py` & `tequila-basic-1.9.5/src/tequila/tools/qng.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/tools/random_generators.py` & `tequila-basic-1.9.5/src/tequila/tools/random_generators.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/utils/bitstrings.py` & `tequila-basic-1.9.5/src/tequila/utils/bitstrings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/utils/exceptions.py` & `tequila-basic-1.9.5/src/tequila/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/utils/joined_transformation.py` & `tequila-basic-1.9.5/src/tequila/utils/joined_transformation.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/utils/keymap.py` & `tequila-basic-1.9.5/src/tequila/utils/keymap.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/utils/misc.py` & `tequila-basic-1.9.5/src/tequila/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila/wavefunction/qubit_wavefunction.py` & `tequila-basic-1.9.5/src/tequila/wavefunction/qubit_wavefunction.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/src/tequila_basic.egg-info/PKG-INFO` & `tequila-basic-1.9.5/src/tequila_basic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tequila-basic
-Version: 1.9.4
+Version: 1.9.5
 Summary: A High-Level Abstraction Framework for Quantum Algorithms
 Home-page: https://github.com/tequilahub/tequila
 Author: Tequila Developers 
 Author-email: jakob.kottmann@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -28,15 +28,15 @@
 - [tequila in a nutshell](https://kottmanj.github.io/tequila-in-a-nutshell/#/)  
 - [getting started](https://jakobkottmann.com/posts/tq-get-started/)    
 - [circuits in tequila](https://jakobkottmann.com/posts/tq-circuits/)  
 - [notebook collection](https://github.com/tequilahub/tequila-tutorials)  
 - [talks and slides](https://kottmanj.github.io/talks_and_material/)  
 
 # Installation
-Recommended Python version is 3.8-3.9.   
+Recommended Python version is 3.9 - 3.10.   
 Tequila supports linux, osx and windows. However, not all optional dependencies are supported on windows.  
 
 ## Install from PyPi
 **Do not** install like this: (Minecraft lovers excluded)
 <strike>`pip install tequila`</strike>
 
 You can install tequila from PyPi as:
@@ -254,14 +254,22 @@
 Boosting quantum amplitude exponentially in variational quantum algorithms  
 [10.1088/2058-9565/acf4ba](doi.org/10.1088/2058-9565/acf4ba)  
 
 A.G. Cadavid, I. Montalban, A. Dalal, E. Solano, N.N. Hegade  
 Efficient DCQO Algorithm within the Impulse Regime for Portfolio Optimization  
 [arxiv:2308.15475](https://arxiv.org/abs/2308.15475)  
 
+A. Anand, K. Brown  
+Hamiltonians, groups, graphs and ansätze  
+[arxiv:2312.17146](https://arxiv.org/abs/2312.17146)  
+
+P.W.K. Jensen, E.R. Kjellgren, P. Reinholdt, K.M. Ziems, S. Coriani, J. Kongsted, S. Sauer  
+Quantum Equation of Motion with Orbital Optimization for Computing Molecular Properties in Near-Term Quantum Computing  
+[arxiv:2312.12386](https://arxiv.org/abs/2312.12386)  
+
 Let us know, if you want your research project and/or tutorial to be included in this list!
 
 # Dependencies
 Support for additional optimizers or quantum backends can be activated by intalling them in your environment.
 Tequila will then detect them automatically.
 Currently those are: [Phoenics](https://github.com/aspuru-guzik-group/phoenics)
  and [GPyOpt](https://sheffieldml.github.io/GPyOpt/).
@@ -281,15 +289,15 @@
 For best performance it is recommended to have `qulacs` installed.
 
 ## QuantumChemistry:
 Currently supported
 ### [Psi4](https://github.com/psi4/psi4).
 In a conda environment this can be installed with
 ```bash
-conda install psi4 -c psi4
+conda install psi4 -c conda-forge
 ```
 Here is a small [tutorial](https://nbviewer.org/github/tequilahub/tequila-tutorials/blob/main/chemistry/ChemistryModule.ipynb) that illustrates the usage.
 
 ### [Madness](https://github.com/kottmanj/madness)  
 In a conda environment this can be installed with  
 ```bash
 conda install madtequila -c kottmann
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tequila-basic-1.9.4/src/tequila_basic.egg-info/SOURCES.txt` & `tequila-basic-1.9.5/src/tequila_basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_TrotErr.py` & `tequila-basic-1.9.5/tests/test_TrotErr.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_adapt.py` & `tequila-basic-1.9.5/tests/test_adapt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_array.py` & `tequila-basic-1.9.5/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_binary_pauli.py` & `tequila-basic-1.9.5/tests/test_binary_pauli.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_binary_utils.py` & `tequila-basic-1.9.5/tests/test_binary_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_bitstrings.py` & `tequila-basic-1.9.5/tests/test_bitstrings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_braket.py` & `tequila-basic-1.9.5/tests/test_braket.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_chemistry.py` & `tequila-basic-1.9.5/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_chemistry_f12.py` & `tequila-basic-1.9.5/tests/test_chemistry_f12.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_chemistry_madness.py` & `tequila-basic-1.9.5/tests/test_chemistry_madness.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_circuits.py` & `tequila-basic-1.9.5/tests/test_circuits.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_fermionic_meas.py` & `tequila-basic-1.9.5/tests/test_fermionic_meas.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_gd_optimizer.py` & `tequila-basic-1.9.5/tests/test_gd_optimizer.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_gpyopt.py` & `tequila-basic-1.9.5/tests/test_gpyopt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_gradient.py` & `tequila-basic-1.9.5/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_hamiltonian_arithmetic.py` & `tequila-basic-1.9.5/tests/test_hamiltonian_arithmetic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_krylov.py` & `tequila-basic-1.9.5/tests/test_krylov.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_mappings.py` & `tequila-basic-1.9.5/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_noise.py` & `tequila-basic-1.9.5/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_noise_opt.py` & `tequila-basic-1.9.5/tests/test_noise_opt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_objectives.py` & `tequila-basic-1.9.5/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_pyzx.py` & `tequila-basic-1.9.5/tests/test_pyzx.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_qasm.py` & `tequila-basic-1.9.5/tests/test_qasm.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_qtensor.py` & `tequila-basic-1.9.5/tests/test_qtensor.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_recompilation_routines.py` & `tequila-basic-1.9.5/tests/test_recompilation_routines.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_scipy.py` & `tequila-basic-1.9.5/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_simulator_backends.py` & `tequila-basic-1.9.5/tests/test_simulator_backends.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_symbolic_simulator.py` & `tequila-basic-1.9.5/tests/test_symbolic_simulator.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_torch_interface.py` & `tequila-basic-1.9.5/tests/test_torch_interface.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_unary_state_prep.py` & `tequila-basic-1.9.5/tests/test_unary_state_prep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.9.4/tests/test_variable.py` & `tequila-basic-1.9.5/tests/test_variable.py`

 * *Files identical despite different names*

