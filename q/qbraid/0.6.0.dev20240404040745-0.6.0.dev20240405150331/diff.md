# Comparing `tmp/qbraid-0.6.0.dev20240404040745.tar.gz` & `tmp/qbraid-0.6.0.dev20240405150331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.6.0.dev20240404040745.tar", last modified: Thu Apr  4 04:07:47 2024, max compression
+gzip compressed data, was "qbraid-0.6.0.dev20240405150331.tar", last modified: Fri Apr  5 15:03:34 2024, max compression
```

## Comparing `qbraid-0.6.0.dev20240404040745.tar` & `qbraid-0.6.0.dev20240405150331.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55239 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.752930 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.752930 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.compiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 04:07:45.000000 qbraid-0.6.0.dev20240404040745/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/custom_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/convert_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21875 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55239 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tools/set_provider_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55271 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.863107 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.compiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.867107 qbraid-0.6.0.dev20240405150331/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 15:03:31.000000 qbraid-0.6.0.dev20240405150331/qbraid/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/compiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.871107 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.875107 qbraid-0.6.0.dev20240405150331/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/abc_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.875107 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/providers/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.879107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/custom_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/convert_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/transpiler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55271 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 15:03:34.000000 qbraid-0.6.0.dev20240405150331/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:03:34.887107 qbraid-0.6.0.dev20240405150331/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:03:34.883107 qbraid-0.6.0.dev20240405150331/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tools/set_provider_configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-05 15:03:23.000000 qbraid-0.6.0.dev20240405150331/tox.ini
```

### Comparing `qbraid-0.6.0.dev20240404040745/CODE_OF_CONDUCT.md` & `qbraid-0.6.0.dev20240405150331/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/CONTRIBUTING.md` & `qbraid-0.6.0.dev20240405150331/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/LICENSE` & `qbraid-0.6.0.dev20240405150331/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/PKG-INFO` & `qbraid-0.6.0.dev20240405150331/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.0.dev20240404040745
+Version: 0.6.0.dev20240405150331
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core==0.1.0.dev3
+Requires-Dist: qbraid-core>=0.1.0.dev4
 Provides-Extra: braket
 Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
@@ -790,19 +790,15 @@
 <img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-environment).
 
-Using the SDK on qBraid Lab means direct, pre-configured access to all
-[Amazon Braket supported devices](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)
-with no additional access keys or API tokens required. See
-[qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html)
-for more.
+Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
 ```bash
 pip install qbraid
@@ -898,20 +894,32 @@
 Behind the scenes, the qBraid-SDK uses ``networkx`` to create a directional graph that maps all possible conversions between supported program types:
 
 ```python
 from qbraid.transpiler import ConversionGraph
 from qbraid.visualization import plot_conversion_graph
 
 graph = ConversionGraph()
-plot_conversion_graph(graph)
+
+graph.plot()
 ```
 
 <img align="middle" width="full" alt="conversion_graph" src="https://qbraid-static.s3.amazonaws.com/conversion_graph.png">
 
-You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. See [example](https://github.com/qBraid/qbraid-lab-demo/blob/main/qbraid_sdk/qbraid_sdk_transpiler_braket_qiskit.ipynb).
+You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-node-to-qbraid-conversion-graph):
+
+```python
+from qbraid_qir.qasm3 import qasm3_to_qir
+from qbraid.transpiler import Conversion
+
+conversion = Conversion("qasm3", "qir", qasm3_to_qir)
+
+graph.add_conversion(conversion)
+
+graph.plot()
+```
 
 ### Devices & Jobs
 
 Search for quantum backend(s) on which to execute your program.
 
 ```python
 >>> from qbraid import get_devices
@@ -1037,19 +1045,15 @@
 
 ## Contributing
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
-- For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
-  other topics, [join our discord community](https://discord.gg/TPBU2sa8Et)
+- For discussions, and specific questions about the qBraid-SDK [join our discord community](https://discord.gg/TPBU2sa8Et)
 - For questions that are more suited for a forum, post to
   [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
   with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
-- Want your open-source project featured as its own runtime environment on
-  qBraid Lab? Fill out our
-  [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.6.0.dev20240404040745/README.md` & `qbraid-0.6.0.dev20240405150331/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,15 @@
 <img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-environment).
 
-Using the SDK on qBraid Lab means direct, pre-configured access to all
-[Amazon Braket supported devices](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)
-with no additional access keys or API tokens required. See
-[qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html)
-for more.
+Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
 ```bash
 pip install qbraid
@@ -153,20 +149,32 @@
 Behind the scenes, the qBraid-SDK uses ``networkx`` to create a directional graph that maps all possible conversions between supported program types:
 
 ```python
 from qbraid.transpiler import ConversionGraph
 from qbraid.visualization import plot_conversion_graph
 
 graph = ConversionGraph()
-plot_conversion_graph(graph)
+
+graph.plot()
 ```
 
 <img align="middle" width="full" alt="conversion_graph" src="https://qbraid-static.s3.amazonaws.com/conversion_graph.png">
 
-You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. See [example](https://github.com/qBraid/qbraid-lab-demo/blob/main/qbraid_sdk/qbraid_sdk_transpiler_braket_qiskit.ipynb).
+You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-node-to-qbraid-conversion-graph):
+
+```python
+from qbraid_qir.qasm3 import qasm3_to_qir
+from qbraid.transpiler import Conversion
+
+conversion = Conversion("qasm3", "qir", qasm3_to_qir)
+
+graph.add_conversion(conversion)
+
+graph.plot()
+```
 
 ### Devices & Jobs
 
 Search for quantum backend(s) on which to execute your program.
 
 ```python
 >>> from qbraid import get_devices
@@ -292,19 +300,15 @@
 
 ## Contributing
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
-- For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
-  other topics, [join our discord community](https://discord.gg/TPBU2sa8Et)
+- For discussions, and specific questions about the qBraid-SDK [join our discord community](https://discord.gg/TPBU2sa8Et)
 - For questions that are more suited for a forum, post to
   [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
   with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
-- Want your open-source project featured as its own runtime environment on
-  qBraid Lab? Fill out our
-  [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

#### html2text {}

```diff
@@ -11,44 +11,44 @@
 backend that interfaces with a supported frontend. - Benchmark, compare,
 interpret results. Built-in **compatible** post-processing enables comparing
 results between runs and **across backends**. ## Installation & Setup [qbraid-
 sdk-env]For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or [create an account](https:/
 /account.qbraid.com)) and follow the steps to [install an environment](https://
 docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-
-environment). Using the SDK on qBraid Lab means direct, pre-configured access
-to all [Amazon Braket supported devices](https://docs.aws.amazon.com/braket/
-latest/developerguide/braket-devices.html) with no additional access keys or
-API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/
-projects/lab/en/latest/lab/quantum_jobs.html) for more. ### Local install The
-qBraid-SDK, and all of its dependencies, can also be installed using pip:
-```bash pip install qbraid ``` You can also [install from source]
-(CONTRIBUTING.md#installing-from-source) by cloning this repository and running
-a pip install command in the root directory of the repository: ```bash git
-clone https://github.com/qBraid/qBraid.git cd qBraid pip install . ``` *Note*:
-The qBraid-SDK requires Python 3.9 or greater. If using locally, follow linked
-instructions to configure your [qBraid](#local-account-setup), [AWS](https://
-github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
-and [IBMQ](https://github.com/Qiskit/qiskit-ibm-provider#provider-setup)
-credentials. ### Check version You can view the version of the qBraid-SDK you
-have installed within Python using the following: ```python In [1]: import
-qbraid In [2]: qbraid.__version__ ``` ## Documentation & Tutorials qBraid
-documentation is available at [docs.qbraid.com](https://docs.qbraid.com/en/
-stable/). See also: - [API Reference](https://docs.qbraid.com/en/stable/api/
-qbraid.html) - [User Guide](https://docs.qbraid.com/en/stable/sdk/
-overview.html) - [Example Notebooks](https://github.com/qBraid/qbraid-lab-demo)
-## Quickstart ### Transpiler Construct a quantum program of any supported
-program type. Below, `SUPPORTED_QPROGRAMS` maps shorthand identifiers for
-supported quantum programs, each corresponding to a type in the typed
-`QPROGRAM` Union. For example, 'qiskit' maps to `qiskit.QuantumCircuit` in
-`QPROGRAM`. Notably, 'qasm2' and 'qasm3' both represent raw OpenQASM strings.
-This arrangement simplifies targeting and transpiling between different quantum
-programming frameworks. ```python >>> from qbraid.programs import
-SUPPORTED_QPROGRAMS >>> SUPPORTED_QPROGRAMS {'cirq':
-'cirq.circuits.circuit.Circuit', 'qiskit':
+environment). Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/
+lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs
+from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand
+simulators from AWS, all with no additional access keys or API tokens required.
+See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/
+quantum_jobs.html) for more. ### Local install The qBraid-SDK, and all of its
+dependencies, can also be installed using pip: ```bash pip install qbraid ```
+You can also [install from source](CONTRIBUTING.md#installing-from-source) by
+cloning this repository and running a pip install command in the root directory
+of the repository: ```bash git clone https://github.com/qBraid/qBraid.git cd
+qBraid pip install . ``` *Note*: The qBraid-SDK requires Python 3.9 or greater.
+If using locally, follow linked instructions to configure your [qBraid](#local-
+account-setup), [AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-
+and-setting-up-aws-credentials), and [IBMQ](https://github.com/Qiskit/qiskit-
+ibm-provider#provider-setup) credentials. ### Check version You can view the
+version of the qBraid-SDK you have installed within Python using the following:
+```python In [1]: import qbraid In [2]: qbraid.__version__ ``` ## Documentation
+& Tutorials qBraid documentation is available at [docs.qbraid.com](https://
+docs.qbraid.com/en/stable/). See also: - [API Reference](https://
+docs.qbraid.com/en/stable/api/qbraid.html) - [User Guide](https://
+docs.qbraid.com/en/stable/sdk/overview.html) - [Example Notebooks](https://
+github.com/qBraid/qbraid-lab-demo) ## Quickstart ### Transpiler Construct a
+quantum program of any supported program type. Below, `SUPPORTED_QPROGRAMS`
+maps shorthand identifiers for supported quantum programs, each corresponding
+to a type in the typed `QPROGRAM` Union. For example, 'qiskit' maps to
+`qiskit.QuantumCircuit` in `QPROGRAM`. Notably, 'qasm2' and 'qasm3' both
+represent raw OpenQASM strings. This arrangement simplifies targeting and
+transpiling between different quantum programming frameworks. ```python >>>
+from qbraid.programs import SUPPORTED_QPROGRAMS >>> SUPPORTED_QPROGRAMS
+{'cirq': 'cirq.circuits.circuit.Circuit', 'qiskit':
 'qiskit.circuit.quantumcircuit.QuantumCircuit', 'pyquil':
 'pyquil.quil.Program', 'pytket': 'pytket._tket.circuit.Circuit', 'braket':
 'braket.circuits.circuit.Circuit', 'openqasm3': 'openqasm3.ast.Program',
 'qasm2': 'str', 'qasm3': 'str'} ``` Pass any quantum program of type
 `qbraid.programs.QPROGRAM` to the `load_program()` and specify a target package
 from `SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
 ```python >>> from qbraid.interface import random_circuit >>> from
@@ -62,23 +62,25 @@
 âââHâââX^0.5ââââââââ ``` The same functionality can
 be achieved using the underlying `transpile()` function directly: ```python >>>
 from qbraid.transpiler import transpile >>> cirq_circuit = transpile
 (qiskit_circuit, "cirq") ``` Behind the scenes, the qBraid-SDK uses
 ``networkx`` to create a directional graph that maps all possible conversions
 between supported program types: ```python from qbraid.transpiler import
 ConversionGraph from qbraid.visualization import plot_conversion_graph graph =
-ConversionGraph() plot_conversion_graph(graph) ``` [conversion_graph]You can
-use the native conversions supported by qBraid, or define your own custom nodes
-and/or edges. See [example](https://github.com/qBraid/qbraid-lab-demo/blob/
-main/qbraid_sdk/qbraid_sdk_transpiler_braket_qiskit.ipynb). ### Devices & Jobs
-Search for quantum backend(s) on which to execute your program. ```python >>>
-from qbraid import get_devices >>> get_devices() Device status updated 0
-minutes ago Device ID Status --------- ------ aws_oqc_lucy ONLINE
-aws_ionq_aria2 OFFLINE aws_rigetti_aspen_m3 ONLINE ibm_q_brisbane ONLINE ...
-``` You can get a Python list of device objects using: ```python from
+ConversionGraph() graph.plot() ``` [conversion_graph]You can use the native
+conversions supported by qBraid, or define your own custom nodes and/or edges.
+For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-
+node-to-qbraid-conversion-graph): ```python from qbraid_qir.qasm3 import
+qasm3_to_qir from qbraid.transpiler import Conversion conversion = Conversion
+("qasm3", "qir", qasm3_to_qir) graph.add_conversion(conversion) graph.plot()
+``` ### Devices & Jobs Search for quantum backend(s) on which to execute your
+program. ```python >>> from qbraid import get_devices >>> get_devices() Device
+status updated 0 minutes ago Device ID Status --------- ------ aws_oqc_lucy
+ONLINE aws_ionq_aria2 OFFLINE aws_rigetti_aspen_m3 ONLINE ibm_q_brisbane ONLINE
+... ``` You can get a Python list of device objects using: ```python from
 qbraid.providers import QbraidProvider provider = QbraidProvider() qdevices =
 provider.get_devices() ``` Or, instantiate a known device by ID via the
 `QbraidProvider.get_device()` method, and submit quantum jobs from any
 supported program type: ```python >>> from qbraid import get_jobs >>> from
 qbraid.providers import QbraidProvider >>> provider = QbraidProvider() >>>
 aws_device = provider.get_device("aws_oqc_lucy") >>> ibm_device =
 provider.get_device("ibm_q_brisbane") >>> aws_job = aws_device.run
@@ -117,15 +119,13 @@
 github.com/YOUR-USERNAME/YOUR-REPOSITORY.git) ``` Use the badge in your
 project's `README.rst`: ```rst .. image:: https://qbraid-
 static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png :target: https://
 account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-
 REPOSITORY.git :width: 150px ``` ## Contributing - Interested in contributing
 code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For feature
 requests and bug reports: [Submit an issue](https://github.com/qBraid/qBraid/
-issues) - For discussions, and specific questions about the qBraid SDK, qBraid
-Lab, or other topics, [join our discord community](https://discord.gg/
-TPBU2sa8Et) - For questions that are more suited for a forum, post to [Quantum
-Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) with the
-[`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid)
-tag. - Want your open-source project featured as its own runtime environment on
-qBraid Lab? Fill out our [New Environment Request Form](https://forms.gle/
-a4v7Kdn7G7bs9jYD8) ## License [GNU General Public License v3.0](LICENSE)
+issues) - For discussions, and specific questions about the qBraid-SDK [join
+our discord community](https://discord.gg/TPBU2sa8Et) - For questions that are
+more suited for a forum, post to [Quantum Computing Stack Exchange](https://
+quantumcomputing.stackexchange.com/) with the [`qbraid`](https://
+quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag. ## License
+[GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/cards/jupyter.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/cards/python.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/cards/terminal.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/favicon.ico` & `qbraid-0.6.0.dev20240405150331/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/logo.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/braket.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/cirq.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qasm.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qir.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/get_devices.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.6.0.dev20240405150331/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/conf.py` & `qbraid-0.6.0.dev20240405150331/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/index.rst` & `qbraid-0.6.0.dev20240405150331/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/devices.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/jobs.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/overview.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/programs.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/programs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/results.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/docs/sdk/transpiler.rst` & `qbraid-0.6.0.dev20240405150331/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/pyproject.toml` & `qbraid-0.6.0.dev20240405150331/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "networkx>=2.5,<4.0",
     "numpy>=1.17,<1.27",
     "openqasm3[parser]>=0.4.0,<0.6.0",
     "ply>=3.6",
-    "qbraid-core==0.1.0.dev3"
+    "qbraid-core>=0.1.0.dev4"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/en/stable/"
 "Source Code" = "https://github.com/qBraid/qBraid"
@@ -96,15 +96,16 @@
 
 [tool.coverage.run]
 parallel = true
 source = ["qbraid"]
 omit = [
   "**/qbraid/transpiler/conversions/cirq/cirq_gates.py",
   "**/qbraid/visualization/plot_conversions.py",
-  "**/qbraid/visualization/draw_circuit.py.py"
+  "**/qbraid/visualization/draw_circuit.py.py",
+  "**/qbraid/_compat.py",
 ]
 
 [tool.coverage.paths]
 source = ["qbraid", ".tox/*/lib/python*/site-packages/qbraid"]
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    about
    get_devices
-   refresh_devices
    get_jobs
 
 
 Classes
 --------
 
 .. autosummary::
@@ -41,20 +40,19 @@
    :toctree: ../stubs/
 
    QbraidError
 
 """
 import sys
 
-from . import _warnings
 from ._about import about
 from ._import import LazyLoader
 from ._version import __version__
 from .exceptions import QbraidError
-from .get_devices import get_devices, refresh_devices
+from .get_devices import get_devices
 from .get_jobs import get_jobs
 
 if "sphinx" in sys.modules:
     from . import compiler, interface, programs, providers, transpiler, visualization
 else:
     compiler = LazyLoader("compiler", globals(), "qbraid.compiler")
     interface = LazyLoader("interface", globals(), "qbraid.interface")
@@ -70,11 +68,10 @@
     "get_devices",
     "get_jobs",
     "interface",
     "LazyLoader",
     "programs",
     "providers",
     "QbraidError",
-    "refresh_devices",
     "transpiler",
     "visualization",
 ]
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/_about.py` & `qbraid-0.6.0.dev20240405150331/qbraid/_about.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # pylint: disable=import-outside-toplevel
     import platform
 
     from networkx import __version__ as networkx_version
     from numpy import __version__ as numpy_version
     from openqasm3 import __version__ as openqasm3_version
     from ply import __version__ as ply_version
-    from qbraid_core._version import __version__ as qbraid_core_version
+    from qbraid_core import __version__ as qbraid_core_version
 
     from ._version import __version__ as qbraid_version
 
     # Core dependencies
     core_dependencies = {
         "qbraid_core": qbraid_core_version,
         "networkx": networkx_version,
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/_display.py` & `qbraid-0.6.0.dev20240405150331/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/_import.py` & `qbraid-0.6.0.dev20240405150331/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/_warnings.py` & `qbraid-0.6.0.dev20240405150331/qbraid/_compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for emitting and disabling warnings at top level.
+Module for emitting and configuring warnings and logging at top level.
 
 """
 import logging
+import os
 import warnings
 
-from qbraid_core._warnings import _check_version
+from qbraid_core._compat import check_version
 
-# Set up logging configuration to suppress INFO messages
-logging.basicConfig(level=logging.WARNING)
-logging.getLogger("qiskit").setLevel(logging.WARNING)
+
+def configure_logging():
+    """Configure logging to show warnings and errors."""
+    level = os.getenv("LOG_LEVEL", "INFO").upper()  # Default to INFO if not set
+    logging.basicConfig(
+        level=getattr(logging, level, logging.INFO),
+        format="%(levelname)s - %(module)s - %(message)s",
+    )
 
 
-def _filterwarnings():
+def filterwarnings():
     """Filter out warnings that are not relevant to the user."""
     warnings.filterwarnings("ignore", category=SyntaxWarning)
     warnings.filterwarnings(
         "ignore", category=UserWarning, message="Setuptools is replacing distutils"
     )
     warnings.filterwarnings("ignore", category=DeprecationWarning)
-    # warnings.filterwarnings("ignore", category=PendingDeprecationWarning)
     warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy")
 
 
-def _warn_version():
-    """Emit a warning."""
-    _check_version("qbraid")
-
-
-_warn_version()
-_filterwarnings()
+def check_warn_version_update():
+    """Emit a warning if updated package version exists."""
+    check_version("qbraid")
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/compiler/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/ionq.py` & `qbraid-0.6.0.dev20240405150331/qbraid/compiler/braket/ionq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/compiler/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/compiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/get_devices.py` & `qbraid-0.6.0.dev20240405150331/qbraid/get_devices.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,76 +11,28 @@
 # pylint: disable=consider-using-f-string
 
 """
 Module to retrieve, update, and display information about devices
 supported by the qBraid SDK.
 
 """
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
-
-from qbraid_core import QbraidSession
-from qbraid_core.services.quantum import QuantumClient, process_device_data
+from typing import Any, Dict, List, Optional
 
 try:
     from IPython.display import HTML, clear_output, display
 except ImportError:
     pass
 
-from ._display import running_in_jupyter, update_progress_bar
-
-if TYPE_CHECKING:
-    from IPython.display import DisplayHandle
-
-
-def refresh_devices() -> None:
-    """Refreshes status for all qbraid supported devices. Requires credential for each vendor."""
-    # pylint: disable-next=import-outside-toplevel
-    from qbraid.providers import QbraidProvider
-
-    client = QuantumClient()
-    provider = QbraidProvider(client=client)
-    devices = client.search_devices()
-    count = 0
-    num_devices = len(devices)  # i.e. number of iterations
-    for document in devices:
-        progress = count / num_devices
-        update_progress_bar(progress)
-        if document["statusRefresh"] is not None:  # None => internally not available at moment
-            qbraid_id = document["qbraid_id"]
-            try:
-                device = provider.get_device(qbraid_id)
-                status = device.status().name
-                client.update_device(data={"qbraid_id": qbraid_id, "status": status})
-            except Exception:  # pylint: disable=broad-except
-                pass
-
-        count += 1
-    update_progress_bar(1)
-    print()
-
-
-def _get_device_data(query: Dict[str, Any]) -> Tuple[List[List[str]], int]:
-    """Get devices helper function that queries the qBraid API for all supported devices
-    and returns a list of devices that match the query filters. Each device is
-    represented by its own length-4 list containing the [provider, name, qbraid_id, status].
-    """
-    session = QbraidSession()
-
-    # forward compatibility for casing transition
-    if query.get("type") == "SIMULATOR":
-        query["type"] = "Simulator"
+from qbraid_core import QbraidSession
+from qbraid_core.services.quantum import QuantumClient, process_device_data
 
-    # get-devices must be a POST request with kwarg `json` (not `data`) to
-    # encode the query. This is because certain queries contain regular
-    # expressions which cannot be encoded in GET request `params`.
-    devices = session.post("/public/lab/get-devices", json=query).json()
-    return process_device_data(devices)
+from ._display import running_in_jupyter, update_progress_bar
 
 
-def _display_basic(data: List[str], message: str) -> None:
+def _display_basic(data: List[str], message: str):
     if len(data) == 0:
         print(message)
     else:
         print(f"{message}\n")
         print("{:<35} {:<15}".format("Device ID", "Status"))
         print("{:<35} {:<15}".format("-" * 9, "-" * 6))
         for _, _, device_id, status in data:
@@ -130,17 +82,42 @@
         html += f"<tr><td colspan='4'; style='text-align:{align}'>{message}</td></tr>"
 
     html += "</table>"
 
     return display(HTML(html))
 
 
-def get_devices(
-    filters: Optional[Dict[str, Any]] = None, refresh: bool = False
-) -> "Optional[Union[DisplayHandle, Any]]":
+def _refresh_devices() -> None:
+    """Refreshes status for all qbraid supported devices. Requires credential for each vendor."""
+    # pylint: disable-next=import-outside-toplevel
+    from qbraid.providers import QbraidProvider
+
+    client = QuantumClient()
+    provider = QbraidProvider(client=client)
+    devices = client.search_devices()
+    count = 0
+    num_devices = len(devices)  # i.e. number of iterations
+    for document in devices:
+        progress = count / num_devices
+        update_progress_bar(progress)
+        if document["statusRefresh"] is not None:  # None => internally not available at moment
+            qbraid_id = document["qbraid_id"]
+            try:
+                device = provider.get_device(qbraid_id)
+                status = device.status().name
+                client.update_device(data={"qbraid_id": qbraid_id, "status": status})
+            except Exception:  # pylint: disable=broad-except
+                pass
+
+        count += 1
+    update_progress_bar(1)
+    print()
+
+
+def get_devices(filters: Optional[Dict[str, Any]] = None, refresh: bool = False):
     """Displays a list of all supported devices matching given filters, tabulated by provider,
     name, and qBraid ID. Each device also has a status given by a solid green bubble or a hollow
     red bubble, indicating that the device is online or offline, respectively. You can narrow your
     device search by supplying a dictionary containing the desired criteria.
 
     **Request Syntax:**
 
@@ -197,15 +174,31 @@
 
     Args:
         filters: A dictionary containing any filters to be applied.
         refresh: If True, calls :func:`~qbraid.refresh_devices` before execution.
 
     """
     if refresh:
-        refresh_devices()
+        _refresh_devices()
+
+    session = QbraidSession()
     query = {} if filters is None else filters
-    device_data, msg = _get_device_data(query)
+
+    # forward compatibility for casing transition
+    if query.get("type") == "SIMULATOR":
+        query["type"] = "Simulator"
+
+    if len(query) == 0:
+        client = QuantumClient(session=session)
+        devices = client.search_devices()
+    else:
+        # get-devices must be a POST request with kwarg `json` (not `data`) to
+        # encode the query. This is because certain queries contain regular
+        # expressions which cannot be encoded in GET request `params`.
+        devices = session.post("/public/lab/get-devices", json=query).json()
+
+    device_data, msg = process_device_data(devices)
     align = "center" if len(device_data) == 0 else "right"
 
     if running_in_jupyter():
         return _display_jupyter(device_data, msg, align=align)
     return _display_basic(device_data, msg)
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/get_jobs.py` & `qbraid-0.6.0.dev20240405150331/qbraid/get_jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,51 +13,51 @@
 """
 Module to retrieve, update, and display information about quantum
 jobs submitted through the qBraid SDK.
 
 """
 
 import warnings
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 try:
     from IPython.display import HTML, clear_output, display
 except ImportError:
     pass
 
 from qbraid_core import QbraidSession
-from qbraid_core.services.quantum.adapter import _job_status_msg
+from qbraid_core.services.quantum import QuantumClient, process_job_data
 
-from qbraid._display import running_in_jupyter, update_progress_bar
+from ._display import running_in_jupyter, update_progress_bar
 
 
-def _display_jobs_basic(data, msg):
+def _display_basic(data: List[str], message: str) -> None:
     if len(data) == 0:
-        print(msg)
+        print(message)
     else:
         headers = ["Job ID", "Submitted", "Status"]
 
         max_job_id_length = max(len(str(job_id)) for job_id, _, _ in data)
         max_job_id_length = max(max_job_id_length, len(headers[0]))
 
         header_format = "{:<" + str(max_job_id_length) + "} {:<25} {:<15}"
         separator_format = "{:<" + str(max_job_id_length) + "} {:<25} {:<15}"
         row_format = "{:<" + str(max_job_id_length) + "} {:<25} {:<15}"
 
-        print(f"{msg}:\n")
+        print(f"{message}:\n")
         print(header_format.format(*headers))
 
         separators = ["-" * len(header) for header in headers]
         print(separator_format.format(*separators))
 
         for job_id, timestamp, status in data:
             print(row_format.format(job_id, timestamp, status))
 
 
-def _display_jobs_jupyter(data, msg):
+def _display_jupyter(data: List[str], message: Optional[str] = None, align: str = "right"):
     clear_output(wait=True)
 
     html = """<h3>Quantum Jobs</h3><table><tr>
     <th style='text-align:left'>qBraid ID</th>
     <th style='text-align:left'>Submitted</th>
     <th style='text-align:left'>Status</th></tr>
     """
@@ -83,72 +83,51 @@
 
         html += f"""<tr>
         <td style='text-align:left'>{job_id}</td>
         <td style='text-align:left'>{timestamp}</td>
         <td style='text-align:left'>{status}</td></tr>
         """
 
-    html += f"<tr><td colspan='4'; style='text-align:right'>{msg}</td></tr>"
+    html += f"<tr><td colspan='4'; style='text-align:{align}'>{message}</td></tr>"
 
     html += "</table>"
 
     return display(HTML(html))
 
 
-def _get_jobs_data(
-    query: Dict[str, Any],
-    refresh: bool = False,
-    session: Optional[QbraidSession] = None,
-) -> Tuple[List[List[str]], str]:
+def _refresh_jobs(job_data: List[str]) -> List[str]:
+    """Refreshes the status of all quantum jobs in the list."""
     from qbraid.providers import QuantumJob  # pylint: disable=import-outside-toplevel
 
-    session = QbraidSession() if not session else session
-    jobs = session.post("/get-user-jobs", json=query).json()
     count = 0
-    num_jobs = len(jobs)
-    job_data = []
-    for document in jobs:
+    num_jobs = len(job_data)
+    job_data_refresh = []
+    for job_id, created_at, status in job_data:
         count += 1
         progress = count / num_jobs
-        if refresh:
-            update_progress_bar(progress)
-        job_id = document.get("qbraidJobId", document.get("_id"))
-        if job_id is None:
-            continue
-        created_at = document.get("createdAt")
-        if created_at is None:
-            timestamps = document.get("timestamps", {})
-            created_at = timestamps.get("createdAt", timestamps.get("jobStarted"))
-        status = document.get("qbraidStatus", document.get("status", "UNKNOWN"))
+        update_progress_bar(progress)
         try:
             status_final = QuantumJob.status_final(status)
         except Exception:  # pylint: disable=broad-except
             status_final = True
-        if refresh and not status_final:
+        if not status_final:
             try:
                 qbraid_job = QuantumJob.retrieve(job_id)
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     status_obj = qbraid_job.status()
                 status = status_obj.name
             except Exception:  # pylint: disable=broad-except
                 pass
-        job_data.append([job_id, created_at, status])
+        job_data_refresh.append([job_id, created_at, status])
 
-    msg = _job_status_msg(num_jobs, query)
+    return job_data_refresh
 
-    return job_data, msg
 
-
-def get_jobs(
-    filters: Optional[dict] = None,
-    refresh: bool = False,
-    raw: bool = False,
-    session: Optional[QbraidSession] = None,
-):  # pylint: disable=too-many-statements
+def get_jobs(filters: Optional[Dict[str, Any]] = None, refresh: bool = False, raw: bool = False):
     """Displays a list of quantum jobs submitted by user, tabulated by job ID,
     the date/time it was submitted, and status. You can specify filters to
     narrow the search by supplying a dictionary containing the desired criteria.
 
     **Request Syntax:**
 
     .. code-block:: python
@@ -178,21 +157,32 @@
         * **status** (str): The status of the job
         * **numResults** (int): Maximum number of results to display. Defaults to 10 if not specified.
 
     Args:
         filters (dict): A dictionary containing any filters to be applied.
         refresh (bool): If True, refreshes the status of all jobs before displaying them.
         raw (bool): If True, returns a list of job IDs instead of displaying the jobs.
-        session (QbraidSession): A qBraid session object. If not provided, a new session will be created.
 
     """
     filters = filters or {}
 
-    job_data, msg = _get_jobs_data(filters, refresh, session)
+    session = QbraidSession()
+
+    if len(filters) == 0:
+        client = QuantumClient(session=session)
+        jobs = client.search_jobs()
+    else:
+        jobs = session.post("/get-user-jobs", json=filters).json()
+
+    job_data, msg = process_job_data(jobs, filters)
+
+    if refresh:
+        job_data = _refresh_jobs(job_data)
 
     if raw:
-        job_ids = [job[0] for job in job_data]
-        return job_ids
+        return [job[0] for job in job_data]
+
+    align = "center" if len(job_data) == 0 else "right"
 
     if running_in_jupyter():
-        return _display_jobs_jupyter(job_data, msg)
-    return _display_jobs_basic(job_data, msg)
+        return _display_jupyter(job_data, msg, align=align)
+    return _display_basic(job_data, msg)
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/circuit_equality.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/circuit_equality.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/cirq_random.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qasm3_random.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qiskit_random.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/random.py` & `qbraid-0.6.0.dev20240405150331/qbraid/interface/random/random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
 .. autosummary::
    :toctree: ../stubs/
 
    get_qasm_version
    get_program_type
    load_program
+   remove_qasm_barriers
+   unfold_qasm_gate_defs
+   flatten_qasm_program
+   decompose_qasm_qelib1
 
 Classes
 --------
 
 .. autosummary::
    :toctree: ../stubs/
 
@@ -52,7 +56,9 @@
 
 """
 from ._import import QPROGRAM, QPROGRAM_LIBS, QPROGRAM_TYPES, SUPPORTED_QPROGRAMS
 from .abc_program import QuantumProgram
 from .exceptions import PackageValueError, ProgramTypeError, QasmError
 from .inspector import get_program_type, get_qasm_version
 from .loader import load_program
+from .qasm_passes import flatten_qasm_program, remove_qasm_barriers, unfold_qasm_gate_defs
+from .qasm_qelib1 import decompose_qasm_qelib1
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/_import.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/abc_program.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/abc_program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/inspector.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/inspector.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/braket.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/cirq.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pennylane.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pyquil.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pytket.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm2.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm3.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qiskit.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/programs/loader.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/loader.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/_import.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/device.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/job.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from qbraid.providers.enums import JOB_FINAL
 from qbraid.providers.exceptions import JobStateError
 from qbraid.providers.job import QuantumJob
 
 from .result import BraketGateModelResult
 from .tracker import get_quantum_task_cost
 
+logger = logging.getLogger(__name__)
+
 
 class AmazonBraketVersionError(Exception):
     """Exception raised for Amazon Braket SDK errors due to versioning."""
 
 
 class BraketQuantumTask(QuantumJob):
     """Wrapper class for Amazon Braket ``QuantumTask`` objects."""
@@ -59,15 +61,15 @@
             raise AmazonBraketVersionError(
                 "Queue visibility is only available for amazon-braket-sdk>=1.56.0"
             ) from err
 
     def result(self) -> BraketGateModelResult:
         """Return the results of the job."""
         if self.status() not in JOB_FINAL:
-            logging.info("Result will be available when job has reached final state.")
+            logger.info("Result will be available when job has reached final state.")
         return BraketGateModelResult(self._job.result())
 
     def cancel(self) -> None:
         """Cancel the quantum task."""
         task = self._job
         status = self.status()
         if status in JOB_FINAL:
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/provider.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/result.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/tracker.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/aws/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/device.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 import warnings
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from qbraid_core.services.quantum import QuantumClient, quantum_lib_proxy_state
 
 from qbraid.programs import get_program_type, load_program
-from qbraid.providers.enums import DeviceType
-from qbraid.transpiler import transpile
-from qbraid.transpiler.exceptions import CircuitConversionError
+from qbraid.transpiler import CircuitConversionError, transpile
 
+from .enums import DeviceType
 from .exceptions import ProgramValidationError, QbraidRuntimeError
 from .job import QuantumJob
 
 if TYPE_CHECKING:
     import qbraid.programs
     import qbraid.providers
     import qbraid.transpiler
 
 
+logger = logging.getLogger(__name__)
+
+
 class QuantumDevice(ABC):
     """Abstract interface for device-like classes."""
 
     def __init__(self, device: "qbraid.providers.QDEVICE"):
         """Create a ``QuantumDevice`` object.
 
         Args:
@@ -63,15 +65,15 @@
         """Return the device ID."""
         if self._id is None and self._vendor_id is not None:
             try:
                 client = QuantumClient()
                 device = client.get_device(vendor_id=self._vendor_id)
                 self._id = device["qbraid_id"]
             except Exception as err:  # pylint: disable=broad-exception-caught
-                logging.info(
+                logger.info(
                     "Error retrieving device ID from qBraid API: %s. "
                     "Field will be ommited in job metadata",
                     err,
                 )
         return self._id
 
     @property
@@ -190,15 +192,15 @@
                     f"Number of qubits in circuit ({qbraid_circuit.num_qubits}) exceeds "
                     f"the device's capacity ({self.num_qubits})."
                 )
             return qbraid_circuit
         except Exception as err:  # pylint: disable=broad-exception-caught
             if not safe_mode:
                 raise
-            logging.info("Error verifying run input: %s.", err)
+            logger.info("Error verifying run input: %s.", err)
             return None
 
     def transpile(
         self,
         run_input: "qbraid.programs.QPROGRAM",
         conversion_graph: "Optional[qbraid.transpiler.ConversionGraph]" = None,
     ) -> "qbraid.programs.QPROGRAM":
@@ -236,15 +238,14 @@
         return self._compile(run_input)
 
     def process_run_input(
         self,
         run_input: "qbraid.programs.QPROGRAM",
         auto_compile: bool = False,
         conversion_graph: "Optional[qbraid.transpiler.ConversionGraph]" = None,
-        log_level=logging.INFO,
     ) -> Tuple[Any, Dict[str, Any]]:
         """Process quantum program before passing to device run method.
 
         Returns:
             Tupe of run input and job data dictionary (num_qubits, depth, openqasm string)
 
         Raises:
@@ -260,21 +261,21 @@
 
         if qprogram is None:
             try:
                 qprogram = load_program(run_input)
             except Exception as err:  # pylint: disable=broad-exception-caught
                 if not safe_mode:
                     raise
-                logging.log(log_level, "Error loading run input: %s", err)
+                logger.info("Error loading run input: %s", err)
 
         def try_extracting_info(lambda_expression, error_message):
             try:
                 return lambda_expression()
-            except Exception as err:  # pylint: disable=broad-exception-caught
-                logging.log(log_level, error_message, err)
+            except Exception:  # pylint: disable=broad-exception-caught
+                logger.info(error_message)
                 return None
 
         num_qubits = try_extracting_info(
             lambda: qprogram.num_qubits,
             "Error calculating circuit num_qubits: %s. Field will be omitted in job metadata",
         )
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/enums.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/device.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/job.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 from qbraid.providers.enums import JOB_FINAL
 from qbraid.providers.exceptions import JobError, JobStateError
 from qbraid.providers.job import QuantumJob
 
 from .result import QiskitResult
 
+logger = logging.getLogger(__name__)
+
 
 class QiskitJob(QuantumJob):
     """Wrapper class for IBM Qiskit ``Job`` objects."""
 
     def __init__(self, job_id: str, **kwargs):
         """Create a ``QiskitJob`` object."""
         super().__init__(job_id, **kwargs)
@@ -46,15 +48,15 @@
     def _get_status(self):
         """Returns status from Qiskit Job object."""
         return str(self._job.status())
 
     def result(self):
         """Return the results of the job."""
         if self.status() not in JOB_FINAL:
-            logging.info("Result will be available when job has reached final state.")
+            logger.info("Result will be available when job has reached final state.")
         return QiskitResult(self._job.result())
 
     def cancel(self):
         """Attempt to cancel the job."""
         status = self.status()
         if status in JOB_FINAL:
             raise JobStateError(f"Cannot cancel quantum job in the {status} state.")
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/provider.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
 
 class QiskitProvider(QiskitRemoteService):
     """Wrapper for qiskit_ibm_provider.IBMProvider class"""
 
     def save_config(self):
         """Save the current configuration."""
-        raise NotImplementedError
+        provider = self._get_ibm_provider()
+        provider.save_account(token=self.qiskit_ibm_token, overwrite=True)
 
     def _get_ibm_provider(self, **kwargs) -> "qiskit_ibm_provider.IBMProvider":
         """Returns the IBM Quantum provider."""
         from qiskit_ibm_provider import IBMProvider  # pylint: disable=import-outside-toplevel
 
         return IBMProvider(token=self.qiskit_ibm_token, **kwargs)
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/result.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/job.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from .exceptions import JobError, ResourceNotFoundError
 from .provider import QbraidProvider
 from .status_maps import STATUS_MAP
 
 if TYPE_CHECKING:
     import qbraid
 
+logger = logging.getLogger(__name__)
+
 
 class QuantumJob(ABC):
     """Abstract interface for job-like classes."""
 
     @classmethod
     def retrieve(cls, job_id: str, **kwargs) -> "qbraid.providers.QuantumJob":
         """Create a QuantumJob object from a job_id."""
@@ -169,15 +171,15 @@
         )
 
     def _status(self) -> Tuple[JobStatus, str]:
         vendor_status = self._get_status()
         try:
             return self._status_map[vendor_status], vendor_status
         except KeyError:
-            logging.warning(
+            logger.warning(
                 "Expected %s job status matching one of %s but instead got '%s'.",
                 self._device.vendor,
                 str(list(self._status_map.keys())),
                 vendor_status,
             )
             return JobStatus.UNKNOWN, vendor_status
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/provider.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from qbraid_core.exceptions import AuthError
 from qbraid_core.services.quantum import QuantumClient, QuantumServiceRequestError
 
 from qbraid._import import _load_entrypoint
-from qbraid.providers._import import QDEVICE_TYPES
 
+from ._import import QDEVICE_TYPES
 from .exceptions import ResourceNotFoundError
 
 if TYPE_CHECKING:
     import qbraid.providers
 
 
 class QuantumProvider(ABC):
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/result.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/providers/status_maps.py` & `qbraid-0.6.0.dev20240405150331/qbraid/providers/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,14 @@
 
 """
 Module containing one-step functions for converting between supported
 quantum software program types.
 
 .. currentmodule:: qbraid.transpiler.conversions
 
-Functions
-----------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-    remove_qasm_barriers
-    unfold_qasm_gate_defs
-    flatten_qasm_program
-    decompose_qasm_qelib1
-
 Submodules
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    braket
@@ -39,17 +28,14 @@
    pytket
    qiskit
 
 """
 import importlib
 import inspect
 
-from .qasm_passes import flatten_qasm_program, remove_qasm_barriers, unfold_qasm_gate_defs
-from .qasm_qelib1 import decompose_qasm_qelib1
-
 # Dynamically import QPROGRAM_LIBS when needed
 _qbraid = importlib.import_module("qbraid.programs._import")
 _PROGRAM_LIBS = getattr(_qbraid, "_PROGRAM_LIBS", [])
 
 # List to store the names of the imported functions
 conversion_functions = []
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/cirq_to_braket.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 from braket.circuits import gates as braket_gates
 from braket.circuits import noises as braket_noise_gate
 from cirq import Circuit
 from cirq import ops as cirq_ops
 from cirq import protocols
 from cirq.linalg.decompositions import kak_decomposition
 
-import qbraid.programs.libs.cirq
-
 try:
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
-from qbraid.transpiler.conversions.braket.custom_gates import C as BKControl
+import qbraid.programs.libs.cirq
 from qbraid.transpiler.exceptions import CircuitConversionError
 
+from .custom_gates import C as BKControl
+
 
 def cirq_to_braket(circuit: Circuit) -> BKCircuit:
     """Returns a Braket circuit equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a Braket circuit.
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/conversions_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/custom_gates.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/braket/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_gates.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/cirq/conversions_qasm.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 """
 from typing import Optional
 
 import cirq
 from cirq import ops
 from cirq.contrib.qasm_import.exception import QasmException as CirqQasmException
 
-import qbraid
+from qbraid._version import __version__ as qbraid_version
 from qbraid.programs.exceptions import QasmError as QbraidQasmError
-from qbraid.transpiler.conversions.cirq.cirq_gates import _map_zpow_and_unroll
-from qbraid.transpiler.conversions.cirq.cirq_qasm_parser import QasmParser
-from qbraid.transpiler.conversions.qasm_passes import flatten_qasm_program
+from qbraid.programs.qasm_passes import flatten_qasm_program
+
+from .cirq_gates import _map_zpow_and_unroll
+from .cirq_qasm_parser import QasmParser
 
 QASMType = str
 
 
 def _to_qasm_output(
     circuit: cirq.Circuit,
     header: Optional[str] = None,
@@ -39,15 +40,15 @@
         header: A multi-line string that is placed in a comment at the top
             of the QASM. Defaults to a cirq version specifier.
         precision: Number of digits to use when representing numbers.
         qubit_order: Determines how qubits are ordered in the QASM
             register.
     """
     if header is None:
-        header = f"Generated from qBraid v{qbraid._version.__version__}"
+        header = f"Generated from qBraid v{qbraid_version}"
     qubits = ops.QubitOrder.as_qubit_order(qubit_order).order_for(circuit.all_qubits())
     return cirq.QasmOutput(
         operations=circuit.all_operations(),
         qubits=qubits,
         header=header,
         precision=precision,
         version="2.0",
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/convert_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/openqasm3/convert_qasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 import os
 
 import openqasm3
 
 from qbraid.programs.inspector import get_qasm_version
-from qbraid.transpiler.conversions.qasm_qelib1 import _decompose_rxx_instr
+from qbraid.programs.qasm_qelib1 import _decompose_rxx_instr
 
 QASMType = str
 
 
 def _get_qasm3_gate_defs() -> str:
     """Helper function to get openqasm 3 gate defs from .qasm file"""
     current_dir = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pennylane/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/conversions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 representation and pyQuil's circuit representation (Quil programs).
 
 """
 from cirq import Circuit, LineQubit
 from cirq.ops import QubitOrder
 from pyquil import Program
 
-from qbraid.transpiler.conversions.pyquil.quil_input import circuit_from_quil
-from qbraid.transpiler.conversions.pyquil.quil_output import QuilOutput
 from qbraid.transpiler.exceptions import CircuitConversionError
 
+from .quil_input import circuit_from_quil
+from .quil_output import QuilOutput
+
 
 def cirq_to_pyquil(circuit: Circuit) -> Program:
     """Returns a pyQuil Program equivalent to the input Cirq circuit.
 
     Args:
         circuit: Cirq circuit to convert to a pyQuil Program.
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_input.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_output.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pyquil/quil_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 from fractions import Fraction
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
 import cirq
 import numpy as np
 from cirq import ops, protocols, value
 
-import qbraid
-
 
 def exponent_to_pi_string(exp: float) -> str:
     """A function for outputting a float exponent to a string in QUIL format."""
 
     exp_div_pi = exp / np.pi
     exponent_fraction = Fraction(exp_div_pi).limit_denominator(12)
 
@@ -403,15 +401,15 @@
         self.qubits = qubits
         self.operations = tuple(cirq.ops.flatten_to_ops(operations))
         self.measurements = tuple(
             op for op in self.operations if isinstance(op.gate, ops.MeasurementGate)
         )
         self.qubit_id_map = self._generate_qubit_ids()
         self.measurement_id_map = self._generate_measurement_ids()
-        self.formatter = qbraid.transpiler.conversions.pyquil.quil_output.QuilFormatter(
+        self.formatter = QuilFormatter(
             qubit_id_map=self.qubit_id_map, measurement_id_map=self.measurement_id_map
         )
 
     def _generate_qubit_ids(self) -> Dict["cirq.Qid", str]:
         return {qubit: str(i) for i, qubit in enumerate(self.qubits)}
 
     def _generate_measurement_ids(self) -> Dict[str, str]:
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/pytket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_passes.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_passes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 """
 Module for preprocessing qasm string to before it is passed to parser.
 
 """
 import re
 
-from qbraid.transpiler.conversions.qasm_qelib1 import decompose_qasm_qelib1
+from .qasm_qelib1 import decompose_qasm_qelib1
 
 
 def remove_qasm_barriers(qasm_str: str) -> str:
     """Returns a copy of the input QASM with all barriers removed.
 
     Args:
         qasm_str: QASM to remove barriers from.
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_qelib1.py` & `qbraid-0.6.0.dev20240405150331/qbraid/programs/qasm_qelib1.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 Module that implements qelib1.inc qasm gate definitions as python functions
 
 """
 import re
 from typing import Optional
 
-from qbraid.programs.exceptions import QasmError
+from .exceptions import QasmError
 
 
 def _get_param(instr: str) -> Optional[str]:
     try:
         return instr[instr.index("(") + 1 : instr.index(")")]
     except ValueError:
         return None
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/conversions_qasm.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/conversions/qiskit/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/converter.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 """
 import logging
 import warnings
 from copy import deepcopy
 from typing import TYPE_CHECKING, Callable, List, Optional
 
 from qbraid.programs import QPROGRAM_LIBS, get_program_type
-from qbraid.transpiler.exceptions import (
-    CircuitConversionError,
-    ConversionPathNotFoundError,
-    NodeNotFoundError,
-)
-from qbraid.transpiler.graph import ConversionGraph
+
+from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
+from .graph import ConversionGraph
 
 if TYPE_CHECKING:
     import cirq
 
     import qbraid.programs
 
 
+logger = logging.getLogger(__name__)
+
+
 def _warn_if_unsupported(program_type, program_direction):
     if program_type not in QPROGRAM_LIBS:
         warnings.warn(
             f"Converting {program_direction} unsupported program type '{program_type}'.",
             UserWarning,
         )
 
@@ -164,20 +164,20 @@
                     temp_program = convert_func(temp_program)
                 except Exception:  # pylint: disable=broad-exception-caught
                     if get_program_type(temp_program) == "cirq":
                         temp_program = _flatten_cirq(temp_program)
                         temp_program = convert_func(temp_program)  # Retry conversion
                     else:
                         raise
-            logging.info(
+            logger.info(
                 "\nSuccessfully transpiled using conversions: %s",
                 _get_path_from_bound_methods(path),
             )
             return temp_program
         except Exception:  # pylint: disable=broad-exception-caught
-            logging.info(
+            logger.info(
                 "\nFailed to transpile using conversions: %s",
                 _get_path_from_bound_methods(path),
             )
             continue
 
     raise CircuitConversionError(f"Failed to convert program from '{source}' to '{target}'.")
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/edge.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/edge.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/graph.py` & `qbraid-0.6.0.dev20240405150331/qbraid/transpiler/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 """
 from importlib import import_module
 from typing import List, Optional
 
 import networkx as nx
 
-from qbraid.transpiler.conversions import conversion_functions
-from qbraid.transpiler.edge import Conversion
-from qbraid.transpiler.exceptions import ConversionPathNotFoundError
+from .conversions import conversion_functions
+from .edge import Conversion
+from .exceptions import ConversionPathNotFoundError
 
 
 class ConversionGraph(nx.DiGraph):
     """
     Class for coordinating conversions between different quantum software programs
 
     """
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/__init__.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_circuit.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_qasm3.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/exceptions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_conversions.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_counts.py` & `qbraid-0.6.0.dev20240405150331/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/PKG-INFO` & `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.0.dev20240404040745
+Version: 0.6.0.dev20240405150331
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core==0.1.0.dev3
+Requires-Dist: qbraid-core>=0.1.0.dev4
 Provides-Extra: braket
 Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
@@ -790,19 +790,15 @@
 <img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/c82d61b4-2518-4c7e-8f48-05106afa708e">
 
 For the best experience, install the qBraid-SDK environment on
 [lab.qbraid.com](https://lab.qbraid.com). Login (or
 [create an account](https://account.qbraid.com)) and follow the steps to
 [install an environment](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-environment).
 
-Using the SDK on qBraid Lab means direct, pre-configured access to all
-[Amazon Braket supported devices](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)
-with no additional access keys or API tokens required. See
-[qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html)
-for more.
+Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
 ```bash
 pip install qbraid
@@ -898,20 +894,32 @@
 Behind the scenes, the qBraid-SDK uses ``networkx`` to create a directional graph that maps all possible conversions between supported program types:
 
 ```python
 from qbraid.transpiler import ConversionGraph
 from qbraid.visualization import plot_conversion_graph
 
 graph = ConversionGraph()
-plot_conversion_graph(graph)
+
+graph.plot()
 ```
 
 <img align="middle" width="full" alt="conversion_graph" src="https://qbraid-static.s3.amazonaws.com/conversion_graph.png">
 
-You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. See [example](https://github.com/qBraid/qbraid-lab-demo/blob/main/qbraid_sdk/qbraid_sdk_transpiler_braket_qiskit.ipynb).
+You can use the native conversions supported by qBraid, or define your own custom nodes and/or edges. For [example](https://github.com/qBraid/qbraid-qir?tab=readme-ov-file#add-qir-node-to-qbraid-conversion-graph):
+
+```python
+from qbraid_qir.qasm3 import qasm3_to_qir
+from qbraid.transpiler import Conversion
+
+conversion = Conversion("qasm3", "qir", qasm3_to_qir)
+
+graph.add_conversion(conversion)
+
+graph.plot()
+```
 
 ### Devices & Jobs
 
 Search for quantum backend(s) on which to execute your program.
 
 ```python
 >>> from qbraid import get_devices
@@ -1037,19 +1045,15 @@
 
 ## Contributing
 
 - Interested in contributing code, or making a PR? See
   [CONTRIBUTING.md](CONTRIBUTING.md)
 - For feature requests and bug reports:
   [Submit an issue](https://github.com/qBraid/qBraid/issues)
-- For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
-  other topics, [join our discord community](https://discord.gg/TPBU2sa8Et)
+- For discussions, and specific questions about the qBraid-SDK [join our discord community](https://discord.gg/TPBU2sa8Et)
 - For questions that are more suited for a forum, post to
   [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/)
   with the [`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag.
-- Want your open-source project featured as its own runtime environment on
-  qBraid Lab? Fill out our
-  [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/SOURCES.txt` & `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 docs/sdk/overview.rst
 docs/sdk/programs.rst
 docs/sdk/providers.rst
 docs/sdk/results.rst
 docs/sdk/transpiler.rst
 qbraid/__init__.py
 qbraid/_about.py
+qbraid/_compat.py
 qbraid/_display.py
 qbraid/_import.py
 qbraid/_version.py
-qbraid/_warnings.py
 qbraid/exceptions.py
 qbraid/get_devices.py
 qbraid/get_jobs.py
 qbraid.egg-info/PKG-INFO
 qbraid.egg-info/SOURCES.txt
 qbraid.egg-info/dependency_links.txt
 qbraid.egg-info/entry_points.txt
@@ -70,14 +70,16 @@
 qbraid/interface/random/random.py
 qbraid/programs/__init__.py
 qbraid/programs/_import.py
 qbraid/programs/abc_program.py
 qbraid/programs/exceptions.py
 qbraid/programs/inspector.py
 qbraid/programs/loader.py
+qbraid/programs/qasm_passes.py
+qbraid/programs/qasm_qelib1.py
 qbraid/programs/libs/__init__.py
 qbraid/programs/libs/braket.py
 qbraid/programs/libs/cirq.py
 qbraid/programs/libs/pennylane.py
 qbraid/programs/libs/pyquil.py
 qbraid/programs/libs/pytket.py
 qbraid/programs/libs/qasm2.py
@@ -105,16 +107,14 @@
 qbraid/providers/ibm/result.py
 qbraid/transpiler/__init__.py
 qbraid/transpiler/converter.py
 qbraid/transpiler/edge.py
 qbraid/transpiler/exceptions.py
 qbraid/transpiler/graph.py
 qbraid/transpiler/conversions/__init__.py
-qbraid/transpiler/conversions/qasm_passes.py
-qbraid/transpiler/conversions/qasm_qelib1.py
 qbraid/transpiler/conversions/braket/__init__.py
 qbraid/transpiler/conversions/braket/cirq_from_braket.py
 qbraid/transpiler/conversions/braket/cirq_to_braket.py
 qbraid/transpiler/conversions/braket/conversions_qasm.py
 qbraid/transpiler/conversions/braket/custom_gates.py
 qbraid/transpiler/conversions/cirq/__init__.py
 qbraid/transpiler/conversions/cirq/cirq_gates.py
```

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/entry_points.txt` & `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/requires.txt` & `qbraid-0.6.0.dev20240405150331/qbraid.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 networkx<4.0,>=2.5
 numpy<1.27,>=1.17
 openqasm3[parser]<0.6.0,>=0.4.0
 ply>=3.6
-qbraid-core==0.1.0.dev3
+qbraid-core>=0.1.0.dev4
 
 [braket]
 amazon-braket-sdk<1.77.0,>=1.42.1
 
 [cirq]
 cirq-core<1.4.0,>=1.3.0
```

### Comparing `qbraid-0.6.0.dev20240404040745/tools/verify_headers.py` & `qbraid-0.6.0.dev20240405150331/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.0.dev20240404040745/tox.ini` & `qbraid-0.6.0.dev20240405150331/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,18 @@
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/transpiler/conversions/cirq/cirq_gates.py,qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py
+    coverage report --omit=qbraid/transpiler/conversions/cirq/cirq_gates.py, \
+                           qbraid/visualization/draw_circuit.py, \
+                           qbraid/visualization/plot_conversions.py, \
+                           qbraid/_compat.py
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
     docs
```

