# Comparing `tmp/FLORIS-3.5.tar.gz` & `tmp/FLORIS-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLORIS-3.5.tar", last modified: Thu Oct 26 22:31:35 2023, max compression
+gzip compressed data, was "FLORIS-3.6.tar", last modified: Fri Apr  5 20:18:15 2024, max compression
```

## Comparing `FLORIS-3.5.tar` & `FLORIS-3.6.tar`

### file list

```diff
@@ -1,123 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.039687 FLORIS-3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.987684 FLORIS-3.5/FLORIS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-26 22:31:34.000000 FLORIS-3.5/FLORIS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2023-10-26 22:31:34.000000 FLORIS-3.5/FLORIS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 22:31:34.000000 FLORIS-3.5/FLORIS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-26 22:31:34.000000 FLORIS-3.5/FLORIS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-26 22:31:34.000000 FLORIS-3.5/FLORIS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-10-26 22:31:15.000000 FLORIS-3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-26 22:31:35.039687 FLORIS-3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2023-10-26 22:31:15.000000 FLORIS-3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.987684 FLORIS-3.5/floris/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.991684 FLORIS-3.5/floris/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19168 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/floris.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/flow_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    36978 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    67026 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    30881 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)    20922 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/turbine_multi_dim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.995684 FLORIS-3.5/floris/simulation/wake_combination/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_combination/fls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_combination/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_combination/sosfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.995684 FLORIS-3.5/floris/simulation/wake_deflection/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_deflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_deflection/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18506 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_deflection/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_deflection/jimenez.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_deflection/none.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:34.999685 FLORIS-3.5/floris/simulation/wake_turbulence/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_turbulence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_turbulence/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_turbulence/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_turbulence/wake_induced_mixing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.003685 FLORIS-3.5/floris/simulation/wake_velocity/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/cumulative_gauss_curl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/turbopark.py
--rw-r--r--   0 runner    (1001) docker     (127)  9163212 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/simulation/wake_velocity/turbopark_lookup_table.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.019686 FLORIS-3.5/floris/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/cc_blade_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/cut_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)    41803 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/floris_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/floris_interface_legacy_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/flow_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/interface_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/layout_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.019686 FLORIS-3.5/floris/tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.023687 FLORIS-3.5/floris/tools/optimization/layout_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24314 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.023687 FLORIS-3.5/floris/tools/optimization/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.023687 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.031687 FLORIS-3.5/floris/tools/optimization/legacy/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/base_COE.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/cluster_turbines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/layout_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/power_density_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    30497 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw.py
--rw-r--r--   0 runner    (1001) docker     (127)    14439 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_clustered.py
--rw-r--r--   0 runner    (1001) docker     (127)    46052 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
--rw-r--r--   0 runner    (1001) docker     (127)    21991 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
--rw-r--r--   0 runner    (1001) docker     (127)    26817 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    30220 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.031687 FLORIS-3.5/floris/tools/optimization/other/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/other/boundary_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.035687 FLORIS-3.5/floris/tools/optimization/yaw_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34636 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24159 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/parallel_computing_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/power_rose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/rews.py
--rw-r--r--   0 runner    (1001) docker     (127)    21079 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/sowfa_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    30200 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/uncertainty_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    25011 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    61719 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/tools/wind_rose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 22:31:35.035687 FLORIS-3.5/floris/turbine_library/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/iea_10MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/iea_15MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/nrel_5MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    33041 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/turbine_previewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/turbine_library/x_20MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/type_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-26 22:31:15.000000 FLORIS-3.5/floris/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-10-26 22:31:15.000000 FLORIS-3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 22:31:35.039687 FLORIS-3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-10-26 22:31:15.000000 FLORIS-3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/FLORIS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-05 20:18:03.000000 FLORIS-3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-05 20:18:15.529142 FLORIS-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-05 20:18:03.000000 FLORIS-3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.501142 FLORIS-3.6/floris/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21042 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17324 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/floris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/flow_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37599 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66932 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27618 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/turbine_multi_dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_combination/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/fls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/sosfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_deflection/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/jimenez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/none.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_turbulence/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/wake_induced_mixing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.509142 FLORIS-3.6/floris/simulation/wake_velocity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/cumulative_gauss_curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/turbopark.py
+-rw-r--r--   0 runner    (1001) docker     (127)  9163212 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/turbopark_lookup_table.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/cut_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48328 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/floris_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/floris_interface_legacy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/interface_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/layout_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/layout_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.525142 FLORIS-3.6/floris/tools/optimization/legacy/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/base_COE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/cluster_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30497 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46052 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22003 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26829 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30232 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.525142 FLORIS-3.6/floris/tools/optimization/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/other/boundary_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/floris/tools/optimization/yaw_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34644 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24167 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/parallel_computing_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/power_rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/rews.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30208 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/uncertainty_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61719 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/wind_rose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/floris/turbine_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_10MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/nrel_5MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34777 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/turbine_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/turbine_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/x_20MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/type_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-05 20:18:03.000000 FLORIS-3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:18:15.533142 FLORIS-3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 20:18:03.000000 FLORIS-3.6/setup.py
```

### Comparing `FLORIS-3.5/FLORIS.egg-info/PKG-INFO` & `FLORIS-3.6/FLORIS.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.5
+Version: 3.6
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -14,29 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: attrs
-Requires-Dist: pyyaml
-Requires-Dist: numexpr
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.1
-Requires-Dist: matplotlib>=3
-Requires-Dist: pandas
-Requires-Dist: shapely
-Requires-Dist: coloredlogs>=10.0
-Requires-Dist: flatten_dict
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: numexpr~=2.0
+Requires-Dist: numpy~=1.20
+Requires-Dist: scipy~=1.1
+Requires-Dist: matplotlib~=3.0
+Requires-Dist: pandas~=2.0
+Requires-Dist: shapely~=2.0
+Requires-Dist: coloredlogs~=10.0
+Requires-Dist: flatten_dict~=0.0
 Provides-Extra: docs
+Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
-Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
+Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: jupyter-book<=0.13.3; extra == "docs"
 Provides-Extra: develop
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
-Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
+Requires-Dist: pre-commit; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-3.5/FLORIS.egg-info/SOURCES.txt` & `FLORIS-3.6/FLORIS.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,22 @@
 floris/simulation/wake_velocity/empirical_gauss.py
 floris/simulation/wake_velocity/gauss.py
 floris/simulation/wake_velocity/jensen.py
 floris/simulation/wake_velocity/none.py
 floris/simulation/wake_velocity/turbopark.py
 floris/simulation/wake_velocity/turbopark_lookup_table.mat
 floris/tools/__init__.py
-floris/tools/cc_blade_utilities.py
 floris/tools/cut_plane.py
 floris/tools/floris_interface.py
 floris/tools/floris_interface_legacy_reader.py
-floris/tools/flow_data.py
 floris/tools/interface_utilities.py
 floris/tools/layout_functions.py
 floris/tools/parallel_computing_interface.py
 floris/tools/power_rose.py
 floris/tools/rews.py
-floris/tools/sowfa_utilities.py
 floris/tools/uncertainty_interface.py
 floris/tools/visualization.py
 floris/tools/wind_rose.py
 floris/tools/optimization/__init__.py
 floris/tools/optimization/layout_optimization/__init__.py
 floris/tools/optimization/layout_optimization/layout_optimization_base.py
 floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
@@ -97,8 +94,9 @@
 floris/turbine_library/__init__.py
 floris/turbine_library/iea_10MW.yaml
 floris/turbine_library/iea_15MW.yaml
 floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
 floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
 floris/turbine_library/nrel_5MW.yaml
 floris/turbine_library/turbine_previewer.py
+floris/turbine_library/turbine_utilities.py
 floris/turbine_library/x_20MW.yaml
```

### Comparing `FLORIS-3.5/LICENSE.txt` & `FLORIS-3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/PKG-INFO` & `FLORIS-3.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.5
+Version: 3.6
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -14,29 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: attrs
-Requires-Dist: pyyaml
-Requires-Dist: numexpr
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.1
-Requires-Dist: matplotlib>=3
-Requires-Dist: pandas
-Requires-Dist: shapely
-Requires-Dist: coloredlogs>=10.0
-Requires-Dist: flatten_dict
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: numexpr~=2.0
+Requires-Dist: numpy~=1.20
+Requires-Dist: scipy~=1.1
+Requires-Dist: matplotlib~=3.0
+Requires-Dist: pandas~=2.0
+Requires-Dist: shapely~=2.0
+Requires-Dist: coloredlogs~=10.0
+Requires-Dist: flatten_dict~=0.0
 Provides-Extra: docs
+Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
-Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
+Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: jupyter-book<=0.13.3; extra == "docs"
 Provides-Extra: develop
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
-Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
+Requires-Dist: pre-commit; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-3.5/README.md` & `FLORIS-3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FLORIS Wake Modeling and Wind Farm Controls Software
 
 FLORIS is a controls-focused wind farm simulation software incorporating
 steady-state engineering wake models into a performance-focused Python
 framework. It has been in active development at NREL since 2013 and the latest
-release is [FLORIS v3.5](https://github.com/NREL/floris/releases/latest).
+release is [FLORIS v3.6](https://github.com/NREL/floris/releases/latest).
 Online documentation is available at https://nrel.github.io/floris.
 
 The software is in active development and engagement with the development team
 is highly encouraged. If you are interested in using FLORIS to conduct studies
 of a wind farm or extending FLORIS to include your own wake model, please join
 the conversation in [GitHub Discussions](https://github.com/NREL/floris/discussions/)!
 
@@ -67,15 +67,15 @@
         tools (package)
         turbine_library (package)
         type_dec
         utilities
         version
 
     VERSION
-        3.5
+        3.6
 
     FILE
         ~/floris/floris/__init__.py
 ```
 
 It is important to regularly check for new updates and releases as new
 features, improvements, and bug fixes will be issued on an ongoing basis.
```

### Comparing `FLORIS-3.5/floris/__init__.py` & `FLORIS-3.6/floris/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/logging_manager.py` & `FLORIS-3.6/floris/logging_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -139,18 +139,18 @@
             record._stack_info_hidden, record.stack_info = record.stack_info, None
         elif hasattr(record, "_stack_info_hidden"):
             record.stack_info = record._stack_info_hidden
             del record._stack_info_hidden
         return True
 
 
-class LoggerBase:
+class LoggingManager:
     """
-    Convenience super-class to any class requiring access to the logging
-    module. The virtual property here allows a simple and dynamic method
+    This class provide an easy access to the global logger.
+    The virtual property here allows a simple and dynamic method
     for obtaining the correct logger for the calling class.
     """
 
     @property
     def logger(self):
         return logging.getLogger(
             "{}.{}".format(type(self).__module__, type(self).__name__)
```

### Comparing `FLORIS-3.5/floris/simulation/__init__.py` & `FLORIS-3.6/floris/simulation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from .turbine import (
     average_velocity,
     axial_induction,
     compute_tilt_angles_for_floating_turbines,
     Ct,
     power,
     rotor_effective_velocity,
-    TiltTable,
     Turbine
 )
 from .turbine_multi_dim import (
     axial_induction_multidim,
     Ct_multidim,
     TurbineMultiDimensional
 )
```

### Comparing `FLORIS-3.5/floris/simulation/farm.py` & `FLORIS-3.6/floris/simulation/farm.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 from __future__ import annotations
 
 import copy
 from pathlib import Path
-from typing import Any, List
+from typing import (
+    Any,
+    Dict,
+    List,
+)
 
 import attrs
 import numpy as np
 from attrs import define, field
+from scipy.interpolate import interp1d
 
 from floris.simulation import (
     BaseClass,
     State,
     Turbine,
     TurbineMultiDimensional,
 )
@@ -30,15 +35,15 @@
 from floris.type_dec import (
     convert_to_path,
     floris_array_converter,
     iter_validator,
     NDArrayFloat,
     NDArrayObject,
 )
-from floris.utilities import load_yaml, Vec3
+from floris.utilities import load_yaml
 
 
 default_turbine_library_path = Path(__file__).parents[1] / "turbine_library"
 
 
 @define
 class Farm(BaseClass):
@@ -48,58 +53,82 @@
     data.
 
     Farm is the container class of the FLORIS package. It brings
     together all of the component objects after input (i.e., Turbine,
     Wake, FlowField) and packages everything into the appropriate data
     type. Farm should also be used as an entry point to probe objects
     for generating output.
+
+    Args:
+        layout_x (NDArrayFloat): A sequence of x-axis locations for the turbines that can be
+            converted to a 1-D :py:obj:`numpy.ndarray`.
+        layout_y (NDArrayFloat): A sequence of y-axis locations for the turbines that can be
+            converted to a 1-D :py:obj:`numpy.ndarray`.
+        turbine_type (list[dict | str]): A list of turbine definition dictionaries, or string
+            references to the filename of the turbine type in either the FLORIS-provided turbine
+            library (.../floris/turbine_library/), or a user-provided
+            :py:attr:`turbine_library_path`.
+        turbine_library_path (:obj:`str`): Either an absolute file path to the turbine library, or a
+            path relative to the file that is running the analysis.
     """
 
     layout_x: NDArrayFloat = field(converter=floris_array_converter)
     layout_y: NDArrayFloat = field(converter=floris_array_converter)
     # TODO: turbine_type should be immutable
     turbine_type: List = field(validator=iter_validator(list, (dict, str)))
     turbine_library_path: Path = field(
         default=default_turbine_library_path, converter=convert_to_path
     )
 
     turbine_definitions: list = field(init=False, validator=iter_validator(list, dict))
-    coordinates: List[Vec3] = field(init=False)
-    turbine_fCts: tuple = field(init=False, default=[])
-    turbine_fTilts: list = field(init=False, default=[])
+
+    turbine_fCts: Dict[str, interp1d] | List[interp1d] = field(init=False, factory=list)
+    turbine_fCts_sorted: NDArrayFloat = field(init=False, factory=list)
+
+    turbine_tilt_interps: dict[str, interp1d] = field(init=False, factory=dict)
 
     yaw_angles: NDArrayFloat = field(init=False)
     yaw_angles_sorted: NDArrayFloat = field(init=False)
 
     tilt_angles: NDArrayFloat = field(init=False)
     tilt_angles_sorted: NDArrayFloat = field(init=False)
 
     hub_heights: NDArrayFloat = field(init=False)
-    hub_heights_sorted: NDArrayFloat = field(init=False, default=[])
+    hub_heights_sorted: NDArrayFloat = field(init=False, factory=list)
+
+    turbine_map: List[Turbine | TurbineMultiDimensional] = field(init=False, factory=list)
 
-    turbine_type_map: NDArrayObject = field(init=False, default=[])
-    turbine_type_map_sorted: NDArrayObject = field(init=False, default=[])
+    turbine_type_map: NDArrayObject = field(init=False, factory=list)
+    turbine_type_map_sorted: NDArrayObject = field(init=False, factory=list)
 
-    rotor_diameters: NDArrayFloat = field(init=False, default=[])
-    rotor_diameters_sorted: NDArrayFloat = field(init=False, default=[])
+    turbine_power_interps: Dict[str, interp1d] | List[interp1d] = field(init=False, factory=list)
+    turbine_power_interps_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    TSRs: NDArrayFloat = field(init=False, default=[])
-    TSRs_sorted: NDArrayFloat = field(init=False, default=[])
+    rotor_diameters: NDArrayFloat = field(init=False, factory=list)
+    rotor_diameters_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    pPs: NDArrayFloat = field(init=False, default=[])
-    pPs_sorted: NDArrayFloat = field(init=False, default=[])
+    TSRs: NDArrayFloat = field(init=False, factory=list)
+    TSRs_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    pTs: NDArrayFloat = field(init=False, default=[])
-    pTs_sorted: NDArrayFloat = field(init=False, default=[])
+    pPs: NDArrayFloat = field(init=False, factory=list)
+    pPs_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    ref_tilt_cp_cts: NDArrayFloat = field(init=False, default=[])
-    ref_tilt_cp_cts_sorted: NDArrayFloat = field(init=False, default=[])
+    pTs: NDArrayFloat = field(init=False, factory=list)
+    pTs_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    correct_cp_ct_for_tilt: NDArrayFloat = field(init=False, default=[])
-    correct_cp_ct_for_tilt_sorted: NDArrayFloat = field(init=False, default=[])
+    ref_density_cp_cts: NDArrayFloat = field(init=False, factory=list)
+    ref_density_cp_cts_sorted: NDArrayFloat = field(init=False, factory=list)
+
+    ref_tilt_cp_cts: NDArrayFloat = field(init=False, factory=list)
+    ref_tilt_cp_cts_sorted: NDArrayFloat = field(init=False, factory=list)
+
+    correct_cp_ct_for_tilt: NDArrayFloat = field(init=False, factory=list)
+    correct_cp_ct_for_tilt_sorted: NDArrayFloat = field(init=False, factory=list)
+
+    internal_turbine_library: Path = field(init=False, default=default_turbine_library_path)
 
     def __attrs_post_init__(self) -> None:
         # Turbine definitions can be supplied in three ways:
         # - A string selecting a turbine in the floris turbine library
         # - A Python dict representation of a turbine definition
         #   - There's an option to use the yaml keyword "!include" which results in the yaml
         #     library preprocessing the inputs and loading the specified file directly into
@@ -124,15 +153,15 @@
             # If a turbine type is a string, then it is expected in the internal or external
             # turbine library
             if isinstance(t, str):
                 if t in turbine_definition_cache:
                     continue
 
                 # Check if the file exists in the internal and/or external library
-                internal_fn = (default_turbine_library_path / t).with_suffix(".yaml")
+                internal_fn = (self.internal_turbine_library / t).with_suffix(".yaml")
                 external_fn = (self.turbine_library_path / t).with_suffix(".yaml")
                 in_internal = internal_fn.exists()
                 in_external = external_fn.exists()
 
                 # If an external library is used and there's a duplicate of an internal
                 # definition, then raise an error
                 is_unique_path = self.turbine_library_path != default_turbine_library_path
@@ -244,46 +273,48 @@
 
     def construct_turbine_correct_cp_ct_for_tilt(self):
         self.correct_cp_ct_for_tilt = np.array(
             [turb.correct_cp_ct_for_tilt for turb in self.turbine_map]
         )
 
     def construct_turbine_map(self):
-        if 'multi_dimensional_cp_ct' in self.turbine_definitions[0].keys() \
-            and self.turbine_definitions[0]['multi_dimensional_cp_ct'] is True:
-            self.turbine_map = [
-                TurbineMultiDimensional.from_dict(turb) for turb in self.turbine_definitions
-            ]
+        multi_key = "multi_dimensional_cp_ct"
+        if multi_key in self.turbine_definitions[0] and self.turbine_definitions[0][multi_key]:
+            self.turbine_map = []
+            for turb in self.turbine_definitions:
+                _turb = {**turb, **{"turbine_library_path": self.internal_turbine_library}}
+                try:
+                    self.turbine_map.append(TurbineMultiDimensional.from_dict(_turb))
+                except FileNotFoundError:
+                    _turb["turbine_library_path"] = self.turbine_library_path
+                    self.turbine_map.append(TurbineMultiDimensional.from_dict(_turb))
         else:
             self.turbine_map = [Turbine.from_dict(turb) for turb in self.turbine_definitions]
 
     def construct_turbine_fCts(self):
         self.turbine_fCts = {
             turb.turbine_type: turb.fCt_interp for turb in self.turbine_map
         }
 
     def construct_multidim_turbine_fCts(self):
         self.turbine_fCts = [turb.fCt_interp for turb in self.turbine_map]
 
-    def construct_turbine_fTilts(self):
-        self.turbine_fTilts = [(turb.turbine_type, turb.fTilt_interp) for turb in self.turbine_map]
+    def construct_turbine_tilt_interps(self):
+        self.turbine_tilt_interps = {
+            turb.turbine_type: turb.tilt_interp for turb in self.turbine_map
+        }
 
     def construct_turbine_power_interps(self):
         self.turbine_power_interps = {
             turb.turbine_type: turb.power_interp for turb in self.turbine_map
         }
 
     def construct_multidim_turbine_power_interps(self):
         self.turbine_power_interps = [turb.power_interp for turb in self.turbine_map]
 
-    def construct_coordinates(self):
-        self.coordinates = np.array([
-            Vec3([x, y, z]) for x, y, z in zip(self.layout_x, self.layout_y, self.hub_heights)
-        ])
-
     def expand_farm_properties(
         self,
         n_wind_directions: int,
         n_wind_speeds: int,
         sorted_coord_indices
     ):
         template_shape = np.ones_like(sorted_coord_indices)
@@ -390,15 +421,15 @@
             * self.ref_tilt_cp_cts
         )
 
     def calculate_tilt_for_eff_velocities(self, rotor_effective_velocities):
         tilt_angles = compute_tilt_angles_for_floating_turbines(
             self.turbine_type_map_sorted,
             self.tilt_angles_sorted,
-            self.turbine_fTilts,
+            self.turbine_tilt_interps,
             rotor_effective_velocities,
         )
         return tilt_angles
 
     def finalize(self, unsorted_indices):
         if 'multi_dimensional_cp_ct' in self.turbine_definitions[0].keys() \
             and self.turbine_definitions[0]['multi_dimensional_cp_ct'] is True:
@@ -433,15 +464,14 @@
             axis=2
         )
         self.TSRs = np.take_along_axis(
             self.TSRs_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
-        # TODO: do these need to be unsorted? Maybe we should just for completeness...
         self.ref_density_cp_cts = np.take_along_axis(
             self.ref_density_cp_cts_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
         self.ref_tilt_cp_cts = np.take_along_axis(
             self.ref_tilt_cp_cts_sorted,
@@ -467,9 +497,19 @@
             self.turbine_type_map_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
         self.state.USED
 
     @property
+    def coordinates(self):
+        return np.array([
+            np.array([x, y, z]) for x, y, z in zip(
+                self.layout_x,
+                self.layout_y,
+                self.hub_heights if len(self.hub_heights.shape) == 1 else self.hub_heights[0,0]
+            )
+        ])
+
+    @property
     def n_turbines(self):
         return len(self.layout_x)
```

### Comparing `FLORIS-3.5/floris/simulation/floris.py` & `FLORIS-3.6/floris/simulation/floris.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 from pathlib import Path
 
+import numpy as np
+import pandas as pd
 import yaml
 from attrs import define, field
 
 from floris import logging_manager
 from floris.simulation import (
     BaseClass,
     cc_solver,
@@ -38,15 +40,19 @@
     sequential_solver,
     State,
     TurbineCubatureGrid,
     TurbineGrid,
     turbopark_solver,
     WakeModelManager,
 )
-from floris.utilities import load_yaml
+from floris.type_dec import NDArrayFloat
+from floris.utilities import (
+    load_yaml,
+    reverse_rotate_coordinates_rel_west,
+)
 
 
 @define
 class Floris(BaseClass):
     """
     Top-level class that describes a Floris model and initializes the
     simulation. Use the :py:class:`~.simulation.farm.Farm` attribute to
@@ -77,69 +83,68 @@
         logging_manager.configure_file_log(
             self.logging["file"]["enable"],
             self.logging["file"]["level"],
         )
 
         self.check_deprecated_inputs()
 
-        # Initialize farm quanitities that depend on other objects
+        # Initialize farm quantities that depend on other objects
         self.farm.construct_turbine_map()
         if self.wake.model_strings['velocity_model'] == 'multidim_cp_ct':
             self.farm.construct_multidim_turbine_fCts()
             self.farm.construct_multidim_turbine_power_interps()
         else:
             self.farm.construct_turbine_fCts()
             self.farm.construct_turbine_power_interps()
         self.farm.construct_hub_heights()
         self.farm.construct_rotor_diameters()
         self.farm.construct_turbine_TSRs()
         self.farm.construct_turbine_pPs()
         self.farm.construct_turbine_pTs()
         self.farm.construct_turbine_ref_density_cp_cts()
         self.farm.construct_turbine_ref_tilt_cp_cts()
-        self.farm.construct_turbine_fTilts()
+        self.farm.construct_turbine_tilt_interps()
         self.farm.construct_turbine_correct_cp_ct_for_tilt()
-        self.farm.construct_coordinates()
         self.farm.set_yaw_angles(self.flow_field.n_wind_directions, self.flow_field.n_wind_speeds)
         self.farm.set_tilt_to_ref_tilt(
             self.flow_field.n_wind_directions,
             self.flow_field.n_wind_speeds,
         )
 
         if self.solver["type"] == "turbine_grid":
             self.grid = TurbineGrid(
                 turbine_coordinates=self.farm.coordinates,
-                reference_turbine_diameter=self.farm.rotor_diameters,
+                turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["turbine_grid_points"],
                 time_series=self.flow_field.time_series,
             )
         elif self.solver["type"] == "turbine_cubature_grid":
             self.grid = TurbineCubatureGrid(
                 turbine_coordinates=self.farm.coordinates,
-                reference_turbine_diameter=self.farm.rotor_diameters,
+                turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 time_series=self.flow_field.time_series,
                 grid_resolution=self.solver["turbine_grid_points"],
             )
         elif self.solver["type"] == "flow_field_grid":
             self.grid = FlowFieldGrid(
                 turbine_coordinates=self.farm.coordinates,
-                reference_turbine_diameter=self.farm.rotor_diameters,
+                turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["flow_field_grid_points"],
                 time_series=self.flow_field.time_series,
             )
         elif self.solver["type"] == "flow_field_planar_grid":
             self.grid = FlowFieldPlanarGrid(
                 turbine_coordinates=self.farm.coordinates,
-                reference_turbine_diameter=self.farm.rotor_diameters,
+                turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 normal_vector=self.solver["normal_vector"],
                 planar_coordinate=self.solver["planar_coordinate"],
                 grid_resolution=self.solver["flow_field_grid_points"],
                 time_series=self.flow_field.time_series,
                 x1_bounds=self.solver["flow_field_bounds"][0],
@@ -192,19 +197,18 @@
 
             if len(error_messages) > 0:
                 raise ValueError(
                     f"{turbine['turbine_type']} turbine model\n" +
                     "\n\n".join(error_messages)
                 )
 
-    # @profile
     def initialize_domain(self):
         """Initialize solution space prior to wake calculations"""
 
-        # Initialize field quanitities; doing this immediately prior to doing
+        # Initialize field quantities; doing this immediately prior to doing
         # the calculation step allows for manipulating inputs in a script
         # without changing the data structures
         self.flow_field.initialize_velocity_field(self.grid)
 
         # Initialize farm quantities
         self.farm.initialize(self.grid.sorted_indices)
 
@@ -212,20 +216,17 @@
 
     def steady_state_atmospheric_condition(self):
         """Perform the steady-state wind farm wake calculations. Note that
         initialize_domain() is required to be called before this function."""
 
         vel_model = self.wake.model_strings["velocity_model"]
 
-        # <<interface>>
-        # start = time.time()
-
         if vel_model in ["gauss", "cc", "turbopark", "jensen"] and \
             self.farm.correct_cp_ct_for_tilt.any():
-            self.logger.warn(
+            self.logger.warning(
                 "The current model does not account for vertical wake deflection due to " +
                 "tilt. Corrections to Cp and Ct can be included, but no vertical wake " +
                 "deflection will occur."
             )
 
         if vel_model=="cc":
             cc_solver(
@@ -258,19 +259,16 @@
         else:
             sequential_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
-        # end = time.time()
-        # elapsed_time = end - start
 
         self.finalize()
-        # return elapsed_time
 
     def solve_for_viz(self):
         # Do the calculation with the TurbineGrid for a single wind speed
         # and wind direction and 1 point on the grid. Then, use the result
         # to construct the full flow field grid.
         # This function call should be for a single wind direction and wind speed
         # since the memory consumption is very large.
@@ -297,15 +295,15 @@
 
         # Instantiate the flow_grid
         field_grid = PointsGrid(
             points_x=x,
             points_y=y,
             points_z=z,
             turbine_coordinates=self.farm.coordinates,
-            reference_turbine_diameter=self.farm.rotor_diameters,
+            turbine_diameters=self.farm.rotor_diameters,
             wind_directions=self.flow_field.wind_directions,
             wind_speeds=self.flow_field.wind_speeds,
             grid_resolution=1,
             time_series=self.flow_field.time_series,
             x_center_of_rotation=self.grid.x_center_of_rotation,
             y_center_of_rotation=self.grid.y_center_of_rotation
         )
@@ -322,14 +320,89 @@
         elif vel_model == "empirical_gauss":
             full_flow_empirical_gauss_solver(self.farm, self.flow_field, field_grid, self.wake)
         else:
             full_flow_sequential_solver(self.farm, self.flow_field, field_grid, self.wake)
 
         return self.flow_field.u_sorted[:,:,:,0,0] # Remove turbine grid dimensions
 
+    def solve_for_velocity_deficit_profiles(
+        self,
+        direction: str,
+        downstream_dists: NDArrayFloat | list,
+        profile_range: NDArrayFloat | list,
+        resolution: int,
+        homogeneous_wind_speed: float,
+        ref_rotor_diameter: float,
+        x_start: float,
+        y_start: float,
+        reference_height: float,
+    ) -> list[pd.DataFrame]:
+        """
+        Extract velocity deficit profiles. See
+        :py:meth:`~floris.tools.floris_interface.FlorisInterface.sample_velocity_deficit_profiles`
+        for more details.
+        """
+
+        # Create a grid that contains coordinates for all the sample points in all profiles.
+        # Effectively, this is a grid of parallel lines.
+        n_lines = len(downstream_dists)
+
+        # Coordinate system (x1, x2, x3) is used to define the sample points. The origin is at
+        # (x_start, y_start, reference_height) and x1 is in the streamwise direction.
+        # The x1-coordinate is fixed for every line (every row in  `x1`).
+        x1 = np.atleast_2d(downstream_dists).T * np.ones((n_lines, resolution))
+
+        if resolution == 1:
+            single_line = [0.0]
+        else:
+            single_line = np.linspace(profile_range[0], profile_range[1], resolution)
+
+        if direction == 'cross-stream':
+            x2 = single_line * np.ones((n_lines, resolution))
+            x3 = np.zeros((n_lines, resolution))
+        elif direction == 'vertical':
+            x3 = single_line * np.ones((n_lines, resolution))
+            x2 = np.zeros((n_lines, resolution))
+
+        # Find the coordinates of the sample points in the inertial frame (x, y, z). This is done
+        # through one rotation and one translation.
+        x, y, z = reverse_rotate_coordinates_rel_west(
+            self.flow_field.wind_directions,
+            x1[None, :, :],
+            x2[None, :, :],
+            x3[None, :, :],
+            x_center_of_rotation=0.0,
+            y_center_of_rotation=0.0,
+        )
+        x = np.squeeze(x, axis=0) + x_start
+        y = np.squeeze(y, axis=0) + y_start
+        z = np.squeeze(z, axis=0) + reference_height
+
+        u = self.solve_for_points(x.flatten(), y.flatten(), z.flatten())
+        u = np.reshape(u[0, 0, :], (n_lines, resolution))
+        velocity_deficit = (homogeneous_wind_speed - u) / homogeneous_wind_speed
+
+        velocity_deficit_profiles = []
+
+        for i in range(n_lines):
+            df = pd.DataFrame(
+                {
+                    'x': x[i],
+                    'y': y[i],
+                    'z': z[i],
+                    'x1/D': x1[i]/ref_rotor_diameter,
+                    'x2/D': x2[i]/ref_rotor_diameter,
+                    'x3/D': x3[i]/ref_rotor_diameter,
+                    'velocity_deficit': velocity_deficit[i],
+                }
+            )
+            velocity_deficit_profiles.append(df)
+
+        return velocity_deficit_profiles
+
     def finalize(self):
         # Once the wake calculation is finished, unsort the values to match
         # the user-supplied order of things.
         self.flow_field.finalize(self.grid.unsorted_indices)
         self.farm.finalize(self.grid.unsorted_indices)
         self.state = State.USED
```

### Comparing `FLORIS-3.5/floris/simulation/flow_field.py` & `FLORIS-3.6/floris/simulation/flow_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,29 +44,33 @@
     time_series: bool = field(default=False)
     heterogenous_inflow_config: dict = field(default=None)
     multidim_conditions: dict = field(default=None)
 
     n_wind_speeds: int = field(init=False)
     n_wind_directions: int = field(init=False)
 
-    u_initial_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    v_initial_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    w_initial_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    u_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    v_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    w_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    u: NDArrayFloat = field(init=False, default=np.array([]))
-    v: NDArrayFloat = field(init=False, default=np.array([]))
-    w: NDArrayFloat = field(init=False, default=np.array([]))
+    u_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    v_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    w_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    u_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    v_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    w_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    u: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    v: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    w: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     het_map: list = field(init=False, default=None)
-    dudz_initial_sorted: NDArrayFloat = field(init=False, default=np.array([]))
+    dudz_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
 
-    turbulence_intensity_field: NDArrayFloat = field(init=False, default=np.array([]))
-    turbulence_intensity_field_sorted: NDArrayFloat = field(init=False, default=np.array([]))
-    turbulence_intensity_field_sorted_avg: NDArrayFloat = field(init=False, default=np.array([]))
+    turbulence_intensity_field: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
+    turbulence_intensity_field_sorted: NDArrayFloat = field(
+        init=False, factory=lambda: np.array([])
+    )
+    turbulence_intensity_field_sorted_avg: NDArrayFloat = field(
+        init=False, factory=lambda: np.array([])
+    )
 
     @wind_speeds.validator
     def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
         """Using the validator method to keep the `n_wind_speeds` attribute up to date."""
         if self.time_series:
             self.n_wind_speeds = 1
         else:
@@ -127,18 +131,21 @@
         # determined by this line. Since the right-most dimension on grid.z is storing the values
         # for height, using it here to apply the shear law makes that dimension store the vertical
         # wind profile.
         wind_profile_plane = (grid.z_sorted / self.reference_wind_height) ** self.wind_shear
         dwind_profile_plane = (
             self.wind_shear
             * (1 / self.reference_wind_height) ** self.wind_shear
-            * (grid.z_sorted) ** (self.wind_shear - 1)
+            * np.power(
+                grid.z_sorted,
+                (self.wind_shear - 1),
+                where=grid.z_sorted != 0.0
+            )
         )
-
-        # If no hetergeneous inflow defined, then set all speeds ups to 1.0
+        # If no heterogeneous inflow defined, then set all speeds ups to 1.0
         if self.het_map is None:
             speed_ups = 1.0
 
         # If heterogeneous flow data is given, the speed ups at the defined
         # grid locations are determined in either 2 or 3 dimensions.
         else:
             bounds = np.array(list(zip(
```

### Comparing `FLORIS-3.5/floris/simulation/grid.py` & `FLORIS-3.6/floris/simulation/grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,89 +18,87 @@
 from abc import ABC, abstractmethod
 from typing import Iterable
 
 import attrs
 import numpy as np
 from attrs import define, field
 
+from floris.simulation import BaseClass
 from floris.type_dec import (
     floris_array_converter,
     floris_float_type,
     NDArrayFloat,
     NDArrayInt,
 )
 from floris.utilities import (
     reverse_rotate_coordinates_rel_west,
     rotate_coordinates_rel_west,
-    Vec3,
 )
 
 
 @define
-class Grid(ABC):
+class Grid(ABC, BaseClass):
     """
     Grid should establish domain bounds based on given criteria,
     and develop three arrays to contain components of the grid
-    locations in space.
-
-    This could be generalized to any number of dimensions to be
-    used by perhaps a turbulence field.
+    locations in space. This could be generalized to any number
+    of dimensions to be used by perhaps a turbulence field.
 
     The grid will have to be reestablished for each wind direction since the planform
     area of the farm will be different.
 
     x are the locations in space in the primary direction (typically the direction of the wind)
     y are the locations in space in the lateral direction
     z are the locations in space in the vertical direction
     u are the velocity components at each point in space
     v are the velocity components at each point in space
     w are the velocity components at each point in space
     all of these arrays are the same size
 
     Args:
-        turbine_coordinates (`list[Vec3]`): The series of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): A reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Grid resolution with values
-            specific to each grid type.
+        turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
+            arrays with shape (N coordinates, 3).
+        turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
         wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
         time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
             series.
+        grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Grid resolution with values
+            specific to each grid type.
     """
-    turbine_coordinates: list[Vec3] = field()
-    reference_turbine_diameter: float
-    grid_resolution: int | Iterable = field()
+    turbine_coordinates: NDArrayFloat = field(converter=floris_array_converter)
+    turbine_diameters: NDArrayFloat = field(converter=floris_array_converter)
     wind_directions: NDArrayFloat = field(converter=floris_array_converter)
     wind_speeds: NDArrayFloat = field(converter=floris_array_converter)
     time_series: bool = field()
+    grid_resolution: int | Iterable = field()
 
     n_turbines: int = field(init=False)
     n_wind_speeds: int = field(init=False)
     n_wind_directions: int = field(init=False)
-    turbine_coordinates_array: NDArrayFloat = field(init=False)
     x_sorted: NDArrayFloat = field(init=False)
     y_sorted: NDArrayFloat = field(init=False)
     z_sorted: NDArrayFloat = field(init=False)
     x_sorted_inertial_frame: NDArrayFloat = field(init=False)
     y_sorted_inertial_frame: NDArrayFloat = field(init=False)
     z_sorted_inertial_frame: NDArrayFloat = field(init=False)
     cubature_weights: NDArrayFloat = field(init=False, default=None)
 
-    def __attrs_post_init__(self) -> None:
-        self.turbine_coordinates_array = np.array([c.elements for c in self.turbine_coordinates])
-
     @turbine_coordinates.validator
-    def check_coordinates(self, instance: attrs.Attribute, value: list[Vec3]) -> None:
+    def check_coordinates(self, instance: attrs.Attribute, value: np.ndarray) -> None:
         """
-        Ensures all elements are `Vec3` objects and keeps the `n_turbines`
+        Ensures all elements are Numpy arrays and keeps the `n_turbines`
         attribute up to date.
         """
-        types = np.unique([isinstance(c, Vec3) for c in value])
+        types = np.unique([isinstance(c, np.ndarray) for c in value])
         if not all(types):
-            raise TypeError("'turbine_coordinates' must be `Vec3` objects.")
+            raise TypeError(
+                "'turbine_coordinates' must be `np.array` objects "
+                "with three components of type `float`."
+            )
 
         self.n_turbines = len(value)
 
     @wind_speeds.validator
     def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
         """Using the validator method to keep the `n_wind_speeds` attribute up to date."""
         if self.time_series:
@@ -112,15 +110,15 @@
     def wind_directions_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
         """Using the validator method to keep the `n_wind_directions` attribute up to date."""
         self.n_wind_directions = value.size
 
     @grid_resolution.validator
     def grid_resolution_validator(self, instance: attrs.Attribute, value: int | Iterable) -> None:
         # TODO move this to the grid types and off of the base class
-        """Check that grid resolution is given as int or Vec3 with int components."""
+        """Check that grid resolution is given as appropriate for the chosen Grid-type."""
         if isinstance(value, int) and \
             isinstance(self, (TurbineGrid, TurbineCubatureGrid, PointsGrid)):
             return
         elif isinstance(value, Iterable) and isinstance(self, FlowFieldPlanarGrid):
             assert type(value[0]) is int
             assert type(value[1]) is int
         elif isinstance(value, Iterable) and isinstance(self, FlowFieldGrid):
@@ -135,34 +133,34 @@
         raise NotImplementedError("Grid.set_grid")
 
 @define
 class TurbineGrid(Grid):
     """See `Grid` for more details.
 
     Args:
-        turbine_coordinates (`list[Vec3]`): The series of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): A reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): The number of points in each
-            direction of the square grid on the rotor plane. For example, grid_resolution=3
-            creates a 3x3 grid within the rotor swept area.
+        turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
+            arrays with shape (N coordinates, 3).
+        turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
         wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
         time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
             series.
+        grid_resolution (:py:obj:`int`): The number of points in each
+            direction of the square grid on the rotor plane. For example, grid_resolution=3
+            creates a 3x3 grid within the rotor swept area.
     """
     # TODO: describe these and the differences between `sorted_indices` and `sorted_coord_indices`
     sorted_indices: NDArrayInt = field(init=False)
     sorted_coord_indices: NDArrayInt = field(init=False)
     unsorted_indices: NDArrayInt = field(init=False)
     x_center_of_rotation: NDArrayFloat = field(init=False)
     y_center_of_rotation: NDArrayFloat = field(init=False)
     average_method = "cubic-mean"
 
     def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
         self.set_grid()
 
     def set_grid(self) -> None:
         """
         Create grid points at each turbine for each wind direction and wind speed in the simulation.
         This creates the underlying data structure for the calculation.
 
@@ -213,25 +211,25 @@
         """
         # TODO: Where should we locate the coordinate system? Currently, its at
         # the foot of the turbine where the tower meets the ground.
 
         # These are the rotated coordinates of the wind turbines based on the wind direction
         x, y, z, self.x_center_of_rotation, self.y_center_of_rotation = rotate_coordinates_rel_west(
             self.wind_directions,
-            self.turbine_coordinates_array,
+            self.turbine_coordinates,
         )
 
         # -   **rloc** (*float, optional): A value, from 0 to 1, that determines
         #         the width/height of the grid of points on the rotor as a ratio of
         #         the rotor radius.
         #         Defaults to 0.5.
 
         # Create the data for the turbine grids
         radius_ratio = 0.5
-        disc_area_radius = radius_ratio * self.reference_turbine_diameter / 2
+        disc_area_radius = radius_ratio * self.turbine_diameters / 2
         template_grid = np.ones(
             (
                 self.n_wind_directions,
                 self.n_wind_speeds,
                 self.n_turbines,
                 self.grid_resolution,
                 self.grid_resolution,
@@ -296,42 +294,42 @@
     This grid type arranges points throughout the swept area of the rotor based on the cubature
     of a unit circle. The number of points is set by the user, and then the location of the
     points and their weighting in integration is automatically set. This type of grid
     enables a better approximation of the total incoming velocities on the rotor and therefore
     a more accurate average velocity, thrust coefficient, and axial induction.
 
     Args:
-        turbine_coordinates (`list[Vec3]`): The list of turbine coordinates as `Vec3` objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
+        turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
+            arrays with shape (N coordinates, 3).
+        turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
         wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): The number of points to
-            include in the cubature method. This value must be in the range [1, 10], and the
-            corresponding cubature weights are set automatically.
         time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
             series.
+        grid_resolution (:py:obj:`int`): The number of points to
+            include in the cubature method. This value must be in the range [1, 10], and the
+            corresponding cubature weights are set automatically.
     """
     sorted_indices: NDArrayInt = field(init=False)
     sorted_coord_indices: NDArrayInt = field(init=False)
     unsorted_indices: NDArrayInt = field(init=False)
     x_center_of_rotation: NDArrayFloat = field(init=False)
     y_center_of_rotation: NDArrayFloat = field(init=False)
     average_method = "simple-cubature"
 
     def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
         self.set_grid()
 
     def set_grid(self) -> None:
         """
         """
         # These are the rotated coordinates of the wind turbines based on the wind direction
         x, y, z, self.x_center_of_rotation, self.y_center_of_rotation = rotate_coordinates_rel_west(
             self.wind_directions,
-            self.turbine_coordinates_array
+            self.turbine_coordinates
         )
 
         # Coefficients
         cubature_coefficients = TurbineCubatureGrid.get_cubature_coefficients(self.grid_resolution)
 
         # Generate grid points
         yv = np.kron(cubature_coefficients["r"], cubature_coefficients["q"])
@@ -355,16 +353,16 @@
             ),
             dtype=floris_float_type
         )
         _x = x[:, :, :, None, None] * template_grid
         _y = y[:, :, :, None, None] * template_grid
         _z = z[:, :, :, None, None] * template_grid
         for ti in range(self.n_turbines):
-            _y[:, :, ti, :, :] += yv[None, None, :, None]*self.reference_turbine_diameter[ti] / 2.0
-            _z[:, :, ti, :, :] += zv[None, None, :, None]*self.reference_turbine_diameter[ti] / 2.0
+            _y[:, :, ti, :, :] += yv[None, None, :, None]*self.turbine_diameters[ti] / 2.0
+            _z[:, :, ti, :, :] += zv[None, None, :, None]*self.turbine_diameters[ti] / 2.0
 
         # Sort the turbines at each wind direction
 
         # Get the sorted indices for the x coordinates. These are the indices
         # to sort the turbines from upstream to downstream for all wind directions.
         # Also, store the indices to sort them back for when the calculation finishes.
         self.sorted_indices = _x.argsort(axis=2)
@@ -461,30 +459,33 @@
             "B": np.pi/N,
         }
 
 @define
 class FlowFieldGrid(Grid):
     """
     Args:
-        grid_resolution (`Vec3`): The number of grid points to be created in each direction.
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int`): The number of points on each turbine
+        turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
+            arrays with shape (N coordinates, 3).
+        turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
+        wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
+        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
+        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
+            series.
+        grid_resolution (:py:obj:`Iterable(int,)`): The number of grid points to create in each
+            planar direction. Must be 3 components for resolution in the x, y, and z directions.
     """
     x_center_of_rotation: NDArrayFloat = field(init=False)
     y_center_of_rotation: NDArrayFloat = field(init=False)
 
     def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
         self.set_grid()
 
     def set_grid(self) -> None:
         """
         Create a structured grid for the entire flow field domain.
-        resolution: Vec3
 
         Calculates the domain bounds for the current wake model. The bounds
         are calculated based on preset extents from the
         given layout. The bounds consist of the minimum and maximum values
         in the x-, y-, and z-directions.
 
         If the Curl model is used, the predefined bounds are always set.
@@ -492,23 +493,23 @@
         First, sort the turbines so that we know the bounds in the correct orientation.
         Then, create the grid based on this wind-from-left orientation
         """
 
         # These are the rotated coordinates of the wind turbines based on the wind direction
         x, y, z, self.x_center_of_rotation, self.y_center_of_rotation = rotate_coordinates_rel_west(
             self.wind_directions,
-            self.turbine_coordinates_array
+            self.turbine_coordinates
         )
 
         # Construct the arrays storing the grid points
         eps = 0.01
-        xmin = min(x[0,0]) - 2 * self.reference_turbine_diameter
-        xmax = max(x[0,0]) + 10 * self.reference_turbine_diameter
-        ymin = min(y[0,0]) - 2 * self.reference_turbine_diameter
-        ymax = max(y[0,0]) + 2 * self.reference_turbine_diameter
+        xmin = min(x[0,0]) - 2 * self.turbine_diameters
+        xmax = max(x[0,0]) + 10 * self.turbine_diameters
+        ymin = min(y[0,0]) - 2 * self.turbine_diameters
+        ymax = max(y[0,0]) + 2 * self.turbine_diameters
         zmin = 0 + eps
         zmax = 6 * max(z[0,0])
 
         x_points, y_points, z_points = np.meshgrid(
             np.linspace(xmin, xmax, int(self.grid_resolution[0])),
             np.linspace(ymin, ymax, int(self.grid_resolution[1])),
             np.linspace(zmin, zmax, int(self.grid_resolution[2])),
@@ -530,53 +531,56 @@
                 y_center_of_rotation=self.y_center_of_rotation,
             )
 
 @define
 class FlowFieldPlanarGrid(Grid):
     """
     Args:
-        grid_resolution (`Vec3`): The number of grid points to be created in each direction.
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int`): The number of points on each turbine
+        turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
+            arrays with shape (N coordinates, 3).
+        turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
+        wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
+        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
+        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
+            series.
+        grid_resolution (:py:obj:`Iterable(int,)`): The number of grid points to create in each
+            planar direction. Must be 2 components for resolution in the x and y directions.
+            The z direction is set to 3 planes at -10.0, 0.0, and +10.0 relative to the
+            `planar_coordinate`.
     """
     normal_vector: str = field()
     planar_coordinate: float = field()
     x1_bounds: tuple = field(default=None)
     x2_bounds: tuple = field(default=None)
     x_center_of_rotation: NDArrayFloat = field(init=False)
     y_center_of_rotation: NDArrayFloat = field(init=False)
     sorted_indices: NDArrayInt = field(init=False)
     unsorted_indices: NDArrayInt = field(init=False)
 
     def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
         self.set_grid()
 
     def set_grid(self) -> None:
         """
         Create a structured grid for the entire flow field domain.
-        resolution: Vec3
 
         Calculates the domain bounds for the current wake model. The bounds
         are calculated based on preset extents from the
         given layout. The bounds consist of the minimum and maximum values
         in the x-, y-, and z-directions.
 
-        If the Curl model is used, the predefined bounds are always set.
-
         First, sort the turbines so that we know the bounds in the correct orientation.
         Then, create the grid based on this wind-from-left orientation
         """
         # These are the rotated coordinates of the wind turbines based on the wind direction
         x, y, z, self.x_center_of_rotation, self.y_center_of_rotation = rotate_coordinates_rel_west(
             self.wind_directions,
-            self.turbine_coordinates_array
+            self.turbine_coordinates
         )
-        max_diameter = np.max(self.reference_turbine_diameter)
+        max_diameter = np.max(self.turbine_diameters)
 
         if self.normal_vector == "z":  # Rules of thumb for horizontal plane
             if self.x1_bounds is None:
                 self.x1_bounds = (np.min(x) - 2 * max_diameter, np.max(x) + 10 * max_diameter)
 
             if self.x2_bounds is None:
                 self.x2_bounds = (np.min(y) - 2 * max_diameter, np.max(y) + 2 * max_diameter)
@@ -644,22 +648,26 @@
                 y_center_of_rotation=self.y_center_of_rotation,
             )
 
 @define
 class PointsGrid(Grid):
     """
     Args:
-        turbine_coordinates (`list[Vec3]`): The list of turbine coordinates as `Vec3` objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
+        turbine_coordinates (:py:obj:`NDArrayFloat`): Not used for PointsGrid, but
+            required for the `Grid` super-class.
+        turbine_diameters (:py:obj:`NDArrayFloat`):  Not used for PointsGrid, but
+            required for the `Grid` super-class.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
+        wind_speeds (:py:obj:`NDArrayFloat`):  Not used for PointsGrid, but
+            required for the `Grid` super-class.
+        time_series (:py:obj:`bool`):  Not used for PointsGrid, but
+            required for the `Grid` super-class.
         grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Not used for PointsGrid, but
             required for the `Grid` super-class.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
+
         points_x (:py:obj:`NDArrayFloat`): Array of x-components for the points in the grid.
         points_y (:py:obj:`NDArrayFloat`): Array of y-components for the points in the grid.
         points_z (:py:obj:`NDArrayFloat`): Array of z-components for the points in the grid.
         x_center_of_rotation (:py:obj:`float`, optional): Component of the centroid of the
             farm or area of interest. The PointsGrid will be rotated around this center
             of rotation to account for wind direction changes. If not supplied, the center
             of rotation will be the centroid of the points in the PointsGrid.
@@ -671,15 +679,14 @@
     points_x: NDArrayFloat = field(converter=floris_array_converter)
     points_y: NDArrayFloat = field(converter=floris_array_converter)
     points_z: NDArrayFloat = field(converter=floris_array_converter)
     x_center_of_rotation: float | None = field(default=None)
     y_center_of_rotation: float | None = field(default=None)
 
     def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
         self.set_grid()
 
     def set_grid(self) -> None:
         """
         Set points for calculation based on a series of user-supplied coordinates.
         """
         point_coordinates = np.array(list(zip(self.points_x, self.points_y, self.points_z)))
```

### Comparing `FLORIS-3.5/floris/simulation/solver.py` & `FLORIS-3.6/floris/simulation/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         ct_i = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
@@ -119,15 +119,15 @@
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
@@ -278,22 +278,21 @@
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
     turbine_grid_farm.construct_turbine_pPs()
     turbine_grid_farm.construct_turbine_pTs()
     turbine_grid_farm.construct_turbine_ref_density_cp_cts()
     turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
-    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.construct_coordinates()
     turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
-        reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
+        turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
         wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
         time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
         turbine_grid_flow_field.n_wind_directions,
@@ -336,29 +335,29 @@
 
         ct_i = Ct(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the Ct function,
         # get the first index here (0:1)
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
         axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
@@ -498,28 +497,28 @@
         turb_avg_vels = average_velocity(turb_inflow_field)
         turb_Cts = Ct(
             turb_avg_vels,
             farm.yaw_angles_sorted,
             farm.tilt_angles_sorted,
             farm.ref_tilt_cp_cts_sorted,
             farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         turb_Cts = turb_Cts[:, :, :, None, None]
         turb_aIs = axial_induction(
             turb_avg_vels,
             farm.yaw_angles_sorted,
             farm.tilt_angles_sorted,
             farm.ref_tilt_cp_cts_sorted,
             farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         turb_aIs = turb_aIs[:, :, :, None, None]
@@ -529,15 +528,15 @@
 
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
 
@@ -684,22 +683,21 @@
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
     turbine_grid_farm.construct_turbine_pPs()
     turbine_grid_farm.construct_turbine_pTs()
     turbine_grid_farm.construct_turbine_ref_density_cp_cts()
     turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
-    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.construct_coordinates()
     turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
-        reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
+        turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
         wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
         time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
         turbine_grid_flow_field.n_wind_directions,
@@ -746,29 +744,29 @@
         turb_avg_vels = average_velocity(turbine_grid_flow_field.u_sorted)
         turb_Cts = Ct(
             velocities=turb_avg_vels,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             average_method=turbine_grid.average_method,
             cubature_weights=turbine_grid.cubature_weights
         )
         turb_Cts = turb_Cts[:, :, :, None, None]
 
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=turbine_grid.average_method,
             cubature_weights=turbine_grid.cubature_weights
         )
         axial_induction_i = axial_induction_i[:, :, :, None, None]
@@ -897,28 +895,28 @@
 
         Cts = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
 
         ct_i = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
@@ -926,15 +924,15 @@
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
@@ -963,15 +961,15 @@
                 axial_induction_i,
                 flow_field.wind_shear,
             )
             effective_yaw_i += added_yaw
 
         # Model calculations
         # NOTE: exponential
-        if not np.all(farm.yaw_angles_sorted):
+        if np.any(farm.yaw_angles_sorted):
             model_manager.deflection_model.logger.warning(
                 "WARNING: Deflection with the TurbOPark model has not been fully validated."
                 "This is an initial implementation, and we advise you use at your own risk"
                 "and perform a thorough examination of the results."
             )
             for ii in range(i):
                 x_ii = np.mean(grid.x_sorted[:, :, ii:ii+1], axis=(3, 4))
@@ -983,15 +981,15 @@
                 turbulence_intensity_ii = turbine_turbulence_intensity[:, :, ii:ii+1]
                 ct_ii = Ct(
                     velocities=flow_field.u_sorted,
                     yaw_angle=farm.yaw_angles_sorted,
                     tilt_angle=farm.tilt_angles_sorted,
                     ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
                     fCt=farm.turbine_fCts,
-                    tilt_interp=farm.turbine_fTilts,
+                    tilt_interp=farm.turbine_tilt_interps,
                     correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
                     turbine_type_map=farm.turbine_type_map_sorted,
                     ix_filter=[ii],
                     average_method=grid.average_method,
                     cubature_weights=grid.cubature_weights
                 )
                 ct_ii = ct_ii[:, :, 0:1, None, None]
@@ -1121,19 +1119,18 @@
     # turbine_grid_farm.construct_turbine_map()
     # turbine_grid_farm.construct_turbine_fCts()
     # turbine_grid_farm.construct_turbine_power_interps()
     # turbine_grid_farm.construct_hub_heights()
     # turbine_grid_farm.construct_rotor_diameters()
     # turbine_grid_farm.construct_turbine_TSRs()
     # turbine_grid_farm.construc_turbine_pPs()
-    # turbine_grid_farm.construct_coordinates()
 
     # turbine_grid = TurbineGrid(
     #     turbine_coordinates=turbine_grid_farm.coordinates,
-    #     reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
+    #     turbine_diameters=turbine_grid_farm.rotor_diameters,
     #     wind_directions=turbine_grid_flow_field.wind_directions,
     #     wind_speeds=turbine_grid_flow_field.wind_speeds,
     #     grid_resolution=11,
     # )
     # turbine_grid_farm.expand_farm_properties(
     #     turbine_grid_flow_field.n_wind_directions,
     #     turbine_grid_flow_field.n_wind_speeds,
@@ -1216,15 +1213,15 @@
 
         ct_i = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
@@ -1232,15 +1229,15 @@
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
@@ -1362,22 +1359,21 @@
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
     turbine_grid_farm.construct_turbine_pPs()
     turbine_grid_farm.construct_turbine_pTs()
     turbine_grid_farm.construct_turbine_ref_density_cp_cts()
     turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
-    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.construct_coordinates()
     turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
-        reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
+        turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
         wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
         time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
         turbine_grid_flow_field.n_wind_directions,
@@ -1421,29 +1417,29 @@
 
         ct_i = Ct(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the Ct function,
         # get the first index here (0:1)
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
             tilt_angle=turbine_grid_farm.tilt_angles_sorted,
             ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
         axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
@@ -1558,15 +1554,15 @@
 
         ct_i = Ct_multidim(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=downselect_turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
@@ -1574,15 +1570,15 @@
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction_multidim(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
             tilt_angle=farm.tilt_angles_sorted,
             ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=downselect_turbine_fCts,
-            tilt_interp=farm.turbine_fTilts,
+            tilt_interp=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
             average_method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
```

### Comparing `FLORIS-3.5/floris/simulation/turbine.py` & `FLORIS-3.6/floris/simulation/turbine.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,79 +12,32 @@
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import copy
 from collections.abc import Iterable
-from typing import Any
 
 import attrs
 import numpy as np
 from attrs import define, field
 from scipy.interpolate import interp1d
 
 from floris.simulation import BaseClass
 from floris.type_dec import (
-    floris_array_converter,
-    FromDictMixin,
+    floris_numeric_dict_converter,
     NDArrayBool,
     NDArrayFilter,
     NDArrayFloat,
     NDArrayInt,
     NDArrayObject,
 )
 from floris.utilities import cosd
 
 
-def _filter_convert(
-    ix_filter: NDArrayFilter | Iterable[int] | None, sample_arg: NDArrayFloat | NDArrayInt
-) -> NDArrayFloat | None:
-    """This function selects turbine indeces from the given array of turbine properties
-    over the simulation's atmospheric conditions (wind directions / wind speeds).
-    It converts the ix_filter to a standard format of `np.ndarray`s for filtering
-    certain arguments.
-
-    Args:
-        ix_filter (NDArrayFilter | Iterable[int] | None): The indices, or truth
-            array-like object to use for filtering. None implies that all indeces in the
-            sample_arg should be selected.
-        sample_arg (NDArrayFloat | NDArrayInt): Any argument that will be filtered, to be used for
-            creating the shape. This should be of shape:
-            (n wind directions, n wind speeds, n turbines)
-
-    Returns:
-        NDArrayFloat | None: Returns an array of a truth or index list if a list is
-            passed, a truth array if ix_filter is None, or None if ix_filter is None
-            and the `sample_arg` is a single value.
-    """
-    # Check that the ix_filter is either None or an Iterable. Otherwise,
-    # there's nothing we can do with it.
-    if not isinstance(ix_filter, Iterable) and ix_filter is not None:
-        raise TypeError("Expected ix_filter to be an Iterable or None")
-
-    # Check that the sample_arg is a Numpy array. If it isn't, we
-    # can't get its shape.
-    if not isinstance(sample_arg, np.ndarray):
-        raise TypeError("Expected sample_arg to be a float or integer np.ndarray")
-
-    # At this point, the arguments have this type:
-    # ix_filter: Union[Iterable, None]
-    # sample_arg: np.ndarray
-
-    # Return all values in the turbine-dimension
-    # if the index filter is None
-    if ix_filter is None:
-        return np.ones(sample_arg.shape[-1], dtype=bool)
-
-    # Finally, we should have an index filter list of type Iterable,
-    # so cast it to Numpy array and return
-    return np.array(ix_filter)
-
-
 def _rotor_velocity_yaw_correction(
     pP: float,
     yaw_angle: NDArrayFloat,
     rotor_effective_velocities: NDArrayFloat,
 ) -> NDArrayFloat:
     # Compute the rotor effective velocity adjusting for yaw settings
     pW = pP / 3.0  # Convert from pP to w
@@ -110,30 +63,27 @@
         tilt_interp,
         rotor_effective_velocities,
     )
     # Only update tilt angle if requested (if the tilt isn't accounted for in the Cp curve)
     tilt_angle = np.where(correct_cp_ct_for_tilt, tilt_angle, old_tilt_angle)
 
     # Compute the rotor effective velocity adjusting for tilt
-    rotor_effective_velocities = (
-        rotor_effective_velocities
-        * cosd(tilt_angle - ref_tilt_cp_ct) ** (pT / 3.0)
-    )
+    relative_tilt = tilt_angle - ref_tilt_cp_ct
+    rotor_effective_velocities = rotor_effective_velocities * cosd(relative_tilt) ** (pT / 3.0)
     return rotor_effective_velocities
 
 
 def compute_tilt_angles_for_floating_turbines(
     turbine_type_map: NDArrayObject,
     tilt_angle: NDArrayFloat,
-    tilt_interp: NDArrayObject,
+    tilt_interp: dict[str, interp1d],
     rotor_effective_velocities: NDArrayFloat,
 ) -> NDArrayFloat:
     # Loop over each turbine type given to get tilt angles for all turbines
     tilt_angles = np.zeros(np.shape(rotor_effective_velocities))
-    tilt_interp = dict(tilt_interp)
     turb_types = np.unique(turbine_type_map)
     for turb_type in turb_types:
         # If no tilt interpolation is specified, assume no modification to tilt
         if tilt_interp[turb_type] is None:
             # TODO should this be break? Should it be continue? Do we want to support mixed
             # fixed-bottom and floating? Or non-tilting floating?
             pass
@@ -144,15 +94,15 @@
                 tilt_interp[turb_type](rotor_effective_velocities)
                 * (turbine_type_map == turb_type)
             )
 
     # TODO: Not sure if this is the best way to do this? Basically replaces the initialized
     # tilt_angles if there are non-zero tilt angles calculated above (meaning that the turbine
     # definition contained  a wind_speed/tilt table definition)
-    if not tilt_angles.all() == 0.:
+    if not tilt_angles.all() == 0.0:
         tilt_angle = tilt_angles
 
     return tilt_angle
 
 
 def rotor_effective_velocity(
     air_density: float,
@@ -174,15 +124,14 @@
     if isinstance(yaw_angle, list):
         yaw_angle = np.array(yaw_angle)
     if isinstance(tilt_angle, list):
         tilt_angle = np.array(tilt_angle)
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        ix_filter = _filter_convert(ix_filter, yaw_angle)
         velocities = velocities[:, :, ix_filter]
         yaw_angle = yaw_angle[:, :, ix_filter]
         tilt_angle = tilt_angle[:, :, ix_filter]
         ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
         pP = pP[:, :, ix_filter]
         pT = pT[:, :, ix_filter]
         turbine_type_map = turbine_type_map[:, :, ix_filter]
@@ -215,27 +164,27 @@
 
     return rotor_effective_velocities
 
 
 def power(
     ref_density_cp_ct: float,
     rotor_effective_velocities: NDArrayFloat,
-    power_interp: NDArrayObject,
+    power_interp: dict[str, interp1d],
     turbine_type_map: NDArrayObject,
     ix_filter: NDArrayInt | Iterable[int] | None = None,
 ) -> NDArrayFloat:
     """Power produced by a turbine adjusted for yaw and tilt. Value
     given in Watts.
 
     Args:
         ref_density_cp_cts (NDArrayFloat[wd, ws, turbines]): The reference density for each turbine
-        rotor_effective_velocities (NDArrayFloat[wd, ws, turbines, grid1, grid2]): The rotor
+        rotor_effective_velocities (NDArrayFloat[wd, ws, turbines]): The rotor
             effective velocities at a turbine.
-        power_interp (NDArrayObject[wd, ws, turbines]): The power interpolation function
-            for each turbine.
+        power_interp (dict[str, interp1d]): A dictionary of power interpolation functions for
+            each turbine type.
         turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition for
             each turbine.
         ix_filter (NDArrayInt, optional): The boolean array, or
             integer indices to filter out before calculation. Defaults to None.
 
     Returns:
         NDArrayFloat: The power, in Watts, for each turbine after adjusting for yaw and tilt.
@@ -251,28 +200,24 @@
     # Ervin Bossanyi
 
     # TODO: check this - where is it?
     # P = 1/2 rho A V^3 Cp
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        ix_filter = _filter_convert(ix_filter, rotor_effective_velocities)
         rotor_effective_velocities = rotor_effective_velocities[:, :, ix_filter]
         turbine_type_map = turbine_type_map[:, :, ix_filter]
 
     # Loop over each turbine type given to get power for all turbines
     p = np.zeros(np.shape(rotor_effective_velocities))
     turb_types = np.unique(turbine_type_map)
     for turb_type in turb_types:
         # Using a masked array, apply the thrust coefficient for all turbines of the current
         # type to the main thrust coefficient array
-        p += (
-            power_interp[turb_type](rotor_effective_velocities)
-            * (turbine_type_map == turb_type)
-        )
+        p += power_interp[turb_type](rotor_effective_velocities) * (turbine_type_map == turb_type)
 
     return p * ref_density_cp_ct
 
 
 def Ct(
     velocities: NDArrayFloat,
     yaw_angle: NDArrayFloat,
@@ -318,15 +263,14 @@
         yaw_angle = np.array(yaw_angle)
 
     if isinstance(tilt_angle, list):
         tilt_angle = np.array(tilt_angle)
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        ix_filter = _filter_convert(ix_filter, yaw_angle)
         velocities = velocities[:, :, ix_filter]
         yaw_angle = yaw_angle[:, :, ix_filter]
         tilt_angle = tilt_angle[:, :, ix_filter]
         ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
         turbine_type_map = turbine_type_map[:, :, ix_filter]
         correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, :, ix_filter]
 
@@ -390,15 +334,15 @@
         tilt_interp (Iterable[tuple]): The tilt interpolation functions for each
             turbine.
         correct_cp_ct_for_tilt (NDArrayBool[wd, ws, turbines]): Boolean for determining if the
             turbines Cp and Ct should be corrected for tilt.
         turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition
             for each turbine.
         ix_filter (NDArrayFilter | Iterable[int] | None, optional): The boolean array, or
-            integer indices (as an aray or iterable) to filter out before calculation.
+            integer indices (as an array or iterable) to filter out before calculation.
             Defaults to None.
 
     Returns:
         Union[float, NDArrayFloat]: [description]
     """
 
     if isinstance(yaw_angle, list):
@@ -421,15 +365,14 @@
         turbine_type_map,
         ix_filter,
         average_method,
         cubature_weights
     )
 
     # Then, process the input arguments as needed for this function
-    ix_filter = _filter_convert(ix_filter, yaw_angle)
     if ix_filter is not None:
         yaw_angle = yaw_angle[:, :, ix_filter]
         tilt_angle = tilt_angle[:, :, ix_filter]
         ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
 
     return (
         0.5
@@ -505,174 +448,109 @@
             raise ValueError("cubature_weights is required for 'cubic-cubature' method.")
         return cubic_cubature(velocities, cubature_weights, axis)
 
     else:
         raise ValueError("Incorrect method given.")
 
 @define
-class PowerThrustTable(FromDictMixin):
-    """Helper class to convert the dictionary and list-based inputs to a object of arrays.
-
-    Args:
-        power (NDArrayFloat): The power produced at a given wind speed.
-        thrust (NDArrayFloat): The thrust at a given wind speed.
-        wind_speed (NDArrayFloat): Wind speed values, m/s.
-
-    Raises:
-        ValueError: Raised if the power, thrust, and wind_speed are not all 1-d array-like shapes.
-        ValueError: Raised if power, thrust, and wind_speed don't have the same number of values.
-    """
-    power: NDArrayFloat = field(default=[], converter=floris_array_converter)
-    thrust: NDArrayFloat = field(default=[], converter=floris_array_converter)
-    wind_speed: NDArrayFloat = field(default=[], converter=floris_array_converter)
-
-    def __attrs_post_init__(self) -> None:
-        # Validate the power, thrust, and wind speed inputs.
-
-        inputs = (self.power, self.thrust, self.wind_speed)
-
-        if any(el.ndim > 1 for el in inputs):
-            raise ValueError("power, thrust, and wind_speed inputs must be 1-D.")
-
-        if len( {self.power.size, self.thrust.size, self.wind_speed.size} ) > 1:
-            raise ValueError("power, thrust, and wind_speed tables must be the same size.")
-
-        # Remove any duplicate wind speed entries
-        _, duplicate_filter = np.unique(self.wind_speed, return_index=True)
-        self.power = self.power[duplicate_filter]
-        self.thrust = self.thrust[duplicate_filter]
-        self.wind_speed = self.wind_speed[duplicate_filter]
-
-
-@define
-class TiltTable(FromDictMixin):
-    """Helper class to convert the dictionary and list-based inputs to a object of arrays.
-
-    Args:
-        tilt (NDArrayFloat): The tilt angle at a given wind speed.
-        wind_speeds (NDArrayFloat): Wind speed values, m/s.
-
-    Raises:
-        ValueError: Raised if tilt and wind_speeds are not all 1-d array-like shapes.
-        ValueError: Raised if tilt and wind_speeds don't have the same number of values.
-    """
-    tilt: NDArrayFloat = field(converter=floris_array_converter)
-    wind_speeds: NDArrayFloat = field(converter=floris_array_converter)
-
-    def __attrs_post_init__(self) -> None:
-        # Validate the power, thrust, and wind speed inputs.
-
-        inputs = (self.tilt, self.wind_speeds)
-
-        if any(el.ndim > 1 for el in inputs):
-            raise ValueError("tilt and wind_speed inputs must be 1-D.")
-
-        if len({self.tilt.size, self.wind_speeds.size}) > 1:
-            raise ValueError("tilt and wind_speed tables must be the same size.")
-
-        # Remove any duplicate wind speed entries
-        _, duplicate_filter = np.unique(self.wind_speeds, return_index=True)
-        self.tilt = self.tilt[duplicate_filter]
-        self.wind_speeds = self.wind_speeds[duplicate_filter]
-
-
-@define
 class Turbine(BaseClass):
     """
-    Turbine is a class containing objects pertaining to the individual
-    turbines.
+    A class containing the parameters and infrastructure to model a wind turbine's performance
+    for a particular atmospheric condition.
 
-    Turbine is a model class representing a particular wind turbine. It
-    is largely a container of data and parameters, but also contains
-    methods to probe properties for output.
-
-    Parameters:
-        rotor_diameter (:py:obj: float): The rotor diameter (m).
-        hub_height (:py:obj: float): The hub height (m).
-        pP (:py:obj: float): The cosine exponent relating the yaw
-            misalignment angle to power.
-        pT (:py:obj: float): The cosine exponent relating the rotor
-            tilt angle to power.
-        generator_efficiency (:py:obj: float): The generator
-            efficiency factor used to scale the power production.
-        ref_density_cp_ct (:py:obj: float): The density at which the provided
-            cp and ct is defined
-        power_thrust_table (PowerThrustTable): A dictionary containing the
-            following key-value pairs:
-
-            power (:py:obj: List[float]): The coefficient of power at
-                different wind speeds.
-            thrust (:py:obj: List[float]): The coefficient of thrust
-                at different wind speeds.
-            wind_speed (:py:obj: List[float]): The wind speeds for
-                which the power and thrust values are provided (m/s).
-        ngrid (*int*, optional): The square root of the number
-            of points to use on the turbine grid. This number will be
-            squared so that the points can be evenly distributed.
-            Defaults to 5.
-        rloc (:py:obj: float, optional): A value, from 0 to 1, that determines
-            the width/height of the grid of points on the rotor as a ratio of
-            the rotor radius.
-            Defaults to 0.5.
+    Args:
+        turbine_type (str): An identifier for this type of turbine such as "NREL_5MW".
+        rotor_diameter (float): The rotor diameter in meters.
+        hub_height (float): The hub height in meters.
+        pP (float): The cosine exponent relating the yaw misalignment angle to turbine power.
+        pT (float): The cosine exponent relating the rotor tilt angle to turbine power.
+        TSR (float): The Tip Speed Ratio of the turbine.
+        generator_efficiency (float): The efficiency of the generator used to scale
+            power production.
+        ref_density_cp_ct (float): The density at which the provided Cp and Ct curves are defined.
+        ref_tilt_cp_ct (float): The implicit tilt of the turbine for which the Cp and Ct
+            curves are defined. This is typically the nacelle tilt.
+        power_thrust_table (dict[str, float]): Contains power coefficient and thrust coefficient
+            values at a series of wind speeds to define the turbine performance.
+            The dictionary must have the following three keys with equal length values:
+                {
+                    "wind_speeds": List[float],
+                    "power": List[float],
+                    "thrust": List[float],
+                }
+        correct_cp_ct_for_tilt (bool): A flag to indicate whether to correct Cp and Ct for tilt
+            usually for a floating turbine.
+            Optional, defaults to False.
+        floating_tilt_table (dict[str, float]): Look up table of tilt angles at a series of
+            wind speeds. The dictionary must have the following keys with equal length values:
+                {
+                    "wind_speeds": List[float],
+                    "tilt": List[float],
+                }
+            Required if `correct_cp_ct_for_tilt = True`. Defaults to None.
     """
-
     turbine_type: str = field()
     rotor_diameter: float = field()
     hub_height: float = field()
     pP: float = field()
     pT: float = field()
     TSR: float = field()
     generator_efficiency: float = field()
     ref_density_cp_ct: float = field()
     ref_tilt_cp_ct: float = field()
-    power_thrust_table: PowerThrustTable = field(default=None)
-    floating_tilt_table: TiltTable = field(default=None)
-    floating_correct_cp_ct_for_tilt: bool = field(default=None)
-    power_thrust_data_file: str = field(default=None)
-    multi_dimensional_cp_ct: bool = field(default=False)
+    power_thrust_table: dict[str, NDArrayFloat] = field(converter=floris_numeric_dict_converter)
 
-    # rloc: float = float_attrib()  # TODO: goes here or on the Grid?
-    # use_points_on_perimeter: bool = bool_attrib()
+    correct_cp_ct_for_tilt: bool = field(default=False)
+    floating_tilt_table: dict[str, NDArrayFloat] | None = field(default=None)
+
+    # Even though this Turbine class does not support the multidimensional features as they
+    # are implemented in TurbineMultiDim, providing the following two attributes here allows
+    # the turbine data inputs to keep the multidimensional Cp and Ct curve but switch them off
+    # with multi_dimensional_cp_ct = False
+    multi_dimensional_cp_ct: bool = field(default=False)
+    power_thrust_data_file: str = field(default=None)
 
     # Initialized in the post_init function
     rotor_radius: float = field(init=False)
     rotor_area: float = field(init=False)
-    fCp_interp: interp1d = field(init=False)
     fCt_interp: interp1d = field(init=False)
     power_interp: interp1d = field(init=False)
-    tilt_interp: interp1d = field(init=False)
+    tilt_interp: interp1d = field(init=False, default=None)
 
+    def __attrs_post_init__(self) -> None:
+        self._initialize_power_thrust_interpolation()
+        self.__post_init__()
 
-    # For the following parameters, use default values if not user-specified
-    # self.rloc = float(input_dictionary["rloc"]) if "rloc" in input_dictionary else 0.5
-    # if "use_points_on_perimeter" in input_dictionary:
-    #     self.use_points_on_perimeter = bool(input_dictionary["use_points_on_perimeter"])
-    # else:
-    #     self.use_points_on_perimeter = False
+    def __post_init__(self) -> None:
+        self._initialize_tilt_interpolation()
 
-    def __attrs_post_init__(self) -> None:
+    def _initialize_power_thrust_interpolation(self) -> None:
+        # TODO This validation for the power thrust tables should go in the turbine library
+        # since it's preprocessing
+        # Remove any duplicate wind speed entries
+        # _, duplicate_filter = np.unique(self.wind_speed, return_index=True)
+        # self.power = self.power[duplicate_filter]
+        # self.thrust = self.thrust[duplicate_filter]
+        # self.wind_speed = self.wind_speed[duplicate_filter]
 
-        # Post-init initialization for the power curve interpolation functions
-        self.power_thrust_table = PowerThrustTable.from_dict(self.power_thrust_table)
-        wind_speeds = self.power_thrust_table.wind_speed
-        self.fCp_interp = interp1d(
+        wind_speeds = self.power_thrust_table["wind_speed"]
+        cp_interp = interp1d(
             wind_speeds,
-            self.power_thrust_table.power,
+            self.power_thrust_table["power"],
             fill_value=(0.0, 1.0),
             bounds_error=False,
         )
-        inner_power = (
-            0.5 * self.rotor_area
-            * self.fCp_interp(wind_speeds)
-            * self.generator_efficiency
-            * wind_speeds ** 3
-        )
         self.power_interp = interp1d(
             wind_speeds,
-            inner_power,
+            (
+                0.5 * self.rotor_area
+                * cp_interp(wind_speeds)
+                * self.generator_efficiency
+                * wind_speeds ** 3
+            ),
             bounds_error=False,
             fill_value=0
         )
 
         """
         Given an array of wind speeds, this function returns an array of the
         interpolated thrust coefficients from the power / thrust table used
@@ -681,36 +559,63 @@
         speeds are assigned Ct of 0.0001 or 0.9999.
 
         The fill_value arguments sets (upper, lower) bounds for any values
         outside of the input range.
         """
         self.fCt_interp = interp1d(
             wind_speeds,
-            self.power_thrust_table.thrust,
+            self.power_thrust_table["thrust"],
             fill_value=(0.0001, 0.9999),
             bounds_error=False,
         )
 
+    def _initialize_tilt_interpolation(self) -> None:
+        # TODO:
+        # Remove any duplicate wind speed entries
+        # _, duplicate_filter = np.unique(self.wind_speeds, return_index=True)
+        # self.tilt = self.tilt[duplicate_filter]
+        # self.wind_speeds = self.wind_speeds[duplicate_filter]
+
+        if self.floating_tilt_table is not None:
+            self.floating_tilt_table = floris_numeric_dict_converter(self.floating_tilt_table)
+
         # If defined, create a tilt interpolation function for floating turbines.
         # fill_value currently set to apply the min or max tilt angles if outside
         # of the interpolation range.
-        if self.floating_tilt_table is not None:
-            self.floating_tilt_table = TiltTable.from_dict(self.floating_tilt_table)
-            self.fTilt_interp = interp1d(
-                self.floating_tilt_table.wind_speeds,
-                self.floating_tilt_table.tilt,
-                fill_value=(0.0, self.floating_tilt_table.tilt[-1]),
+        if self.correct_cp_ct_for_tilt:
+            self.tilt_interp = interp1d(
+                self.floating_tilt_table["wind_speed"],
+                self.floating_tilt_table["tilt"],
+                fill_value=(0.0, self.floating_tilt_table["tilt"][-1]),
                 bounds_error=False,
             )
-            self.tilt_interp = self.fTilt_interp
-            self.correct_cp_ct_for_tilt = self.floating_correct_cp_ct_for_tilt
-        else:
-            self.fTilt_interp = None
-            self.tilt_interp = None
-            self.correct_cp_ct_for_tilt = False
+
+    @power_thrust_table.validator
+    def check_power_thrust_table(self, instance: attrs.Attribute, value: dict) -> None:
+        """
+        Verify that the power and thrust tables are given with arrays of equal length
+        to the wind speed array.
+        """
+        if len(value.keys()) != 3 or set(value.keys()) != {"wind_speed", "power", "thrust"}:
+            raise ValueError(
+                """
+                power_thrust_table dictionary must have the form:
+                    {
+                        "wind_speed": List[float],
+                        "power": List[float],
+                        "thrust": List[float],
+                    }
+                """
+            )
+
+        if any(e.ndim > 1 for e in (value["power"], value["thrust"], value["wind_speed"])):
+            raise ValueError("power, thrust, and wind_speed inputs must be 1-D.")
+
+        if len( {value["power"].size, value["thrust"].size, value["wind_speed"].size} ) > 1:
+            raise ValueError("power, thrust, and wind_speed tables must be the same size.")
 
     @rotor_diameter.validator
     def reset_rotor_diameter_dependencies(self, instance: attrs.Attribute, value: float) -> None:
         """Resets the `rotor_radius` and `rotor_area` attributes."""
         # Temporarily turn off validators to avoid infinite recursion
         with attrs.validators.disabled():
             # Reset the values
@@ -730,37 +635,46 @@
         """
         Resets the `rotor_radius` value to trigger the recalculation of
         `rotor_diameter`, `rotor_radius` and `rotor_area`.
         """
         self.rotor_radius = (value / np.pi) ** 0.5
 
     @floating_tilt_table.validator
-    def check_floating_tilt_table(self, instance: attrs.Attribute, value: Any) -> None:
+    def check_floating_tilt_table(self, instance: attrs.Attribute, value: dict | None) -> None:
         """
-        Check that if the tile/wind_speed table is defined, that the tilt and
-        wind_speed arrays are the same length so that the interpolation will work.
+        If the tilt / wind_speed table is defined, verify that the tilt and
+        wind_speed arrays are the same length.
         """
-        if self.floating_tilt_table is not None:
-            if (
-                len(self.floating_tilt_table["tilt"])
-                != len(self.floating_tilt_table["wind_speeds"])
-            ):
-                raise ValueError(
-                    "tilt and wind_speeds must be the same length for the interpolation to work."
-                )
+        if value is None:
+            return
 
-    @floating_correct_cp_ct_for_tilt.validator
+        if len(value.keys()) != 2 or set(value.keys()) != {"wind_speed", "tilt"}:
+            raise ValueError(
+                """
+                floating_tilt_table dictionary must have the form:
+                    {
+                        "wind_speed": List[float],
+                        "tilt": List[float],
+                    }
+                """
+            )
+
+        if any(len(np.shape(e)) > 1 for e in (value["tilt"], value["wind_speed"])):
+            raise ValueError("tilt and wind_speed inputs must be 1-D.")
+
+        if len( {len(value["tilt"]), len(value["wind_speed"])} ) > 1:
+            raise ValueError("tilt and wind_speed inputs must be the same size.")
+
+    @correct_cp_ct_for_tilt.validator
     def check_for_cp_ct_correct_flag_if_floating(
         self,
         instance: attrs.Attribute,
-        value: Any
+        value: bool
     ) -> None:
         """
         Check that the boolean flag exists for correcting Cp/Ct for tilt
         if a tile/wind_speed table is also defined.
         """
-        if self.floating_tilt_table is not None:
-            if self.floating_correct_cp_ct_for_tilt is None:
-                raise ValueError(
-                    "If a floating tilt/wind_speed table is defined, the boolean flag"
-                    "floating_correct_cp_ct_for_tilt must also be defined."
-                )
+        if self.correct_cp_ct_for_tilt and self.floating_tilt_table is None:
+            raise ValueError(
+                "To enable the Cp and Ct tilt correction, a tilt table must be given."
+            )
```

### Comparing `FLORIS-3.5/floris/simulation/turbine_multi_dim.py` & `FLORIS-3.6/floris/simulation/turbine_multi_dim.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import copy
 from collections.abc import Iterable
+from pathlib import Path
 
+import attrs
 import numpy as np
 import pandas as pd
 from attrs import define, field
 from flatten_dict import flatten
 from scipy.interpolate import interp1d
 
-# import floris.simulation.turbine as turbine
 from floris.simulation import (
     average_velocity,
     compute_tilt_angles_for_floating_turbines,
-    TiltTable,
     Turbine,
 )
-from floris.simulation.turbine import _filter_convert
 from floris.type_dec import (
+    convert_to_path,
     NDArrayBool,
     NDArrayFilter,
     NDArrayFloat,
     NDArrayInt,
     NDArrayObject,
 )
 from floris.utilities import cosd
@@ -73,15 +73,14 @@
     # Ervin Bossanyi
 
     # TODO: check this - where is it?
     # P = 1/2 rho A V^3 Cp
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        ix_filter = _filter_convert(ix_filter, rotor_effective_velocities)
         power_interp = power_interp[:, :, ix_filter]
         rotor_effective_velocities = rotor_effective_velocities[:, :, ix_filter]
     # Loop over each turbine to get power for all turbines
     p = np.zeros(np.shape(rotor_effective_velocities))
     for i, wd in enumerate(power_interp):
         for j, ws in enumerate(wd):
             for k, turb in enumerate(ws):
@@ -135,15 +134,14 @@
         yaw_angle = np.array(yaw_angle)
 
     if isinstance(tilt_angle, list):
         tilt_angle = np.array(tilt_angle)
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        ix_filter = _filter_convert(ix_filter, yaw_angle)
         velocities = velocities[:, :, ix_filter]
         yaw_angle = yaw_angle[:, :, ix_filter]
         tilt_angle = tilt_angle[:, :, ix_filter]
         ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
         fCt = fCt[:, :, ix_filter]
         turbine_type_map = turbine_type_map[:, :, ix_filter]
         correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, :, ix_filter]
@@ -203,15 +201,15 @@
         tilt_interp (Iterable[tuple]): The tilt interpolation functions for each
             turbine.
         correct_cp_ct_for_tilt (NDArrayBool[wd, ws, turbines]): Boolean for determining if the
             turbines Cp and Ct should be corrected for tilt.
         turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition
             for each turbine.
         ix_filter (NDArrayFilter | Iterable[int] | None, optional): The boolean array, or
-            integer indices (as an aray or iterable) to filter out before calculation.
+            integer indices (as an array or iterable) to filter out before calculation.
             Defaults to None.
 
     Returns:
         Union[float, NDArrayFloat]: [description]
     """
 
     if isinstance(yaw_angle, list):
@@ -234,15 +232,14 @@
         turbine_type_map,
         ix_filter,
         average_method,
         cubature_weights
     )
 
     # Then, process the input arguments as needed for this function
-    ix_filter = _filter_convert(ix_filter, yaw_angle)
     if ix_filter is not None:
         yaw_angle = yaw_angle[:, :, ix_filter]
         tilt_angle = tilt_angle[:, :, ix_filter]
         ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
 
     return (
         0.5
@@ -266,15 +263,15 @@
 
     Args:
         turbine_fCts (NDArray[wd, ws, turbines]): The Ct interpolants generated from the
             multi-dimensional Ct turbine data for all specified conditions.
         conditions (dict): The conditions at which to determine which Ct interpolant to use.
 
     Returns:
-        NDArray: The downselected Ct interpolants for the selected conditions.
+        NDArray: The down selected Ct interpolants for the selected conditions.
     """
     downselect_turbine_fCts = np.empty_like(turbine_fCts)
     # Loop over the wind directions, wind speeds, and turbines, finding the Ct interpolant
     # that is closest to the specified multi-dimensional condition.
     for i, wd in enumerate(turbine_fCts):
         for j, ws in enumerate(wd):
             for k, turb in enumerate(ws):
@@ -303,15 +300,15 @@
 
     Args:
         power_interps (NDArray[wd, ws, turbines]): The power interpolants generated from the
             multi-dimensional Cp turbine data for all specified conditions.
         conditions (dict): The conditions at which to determine which Ct interpolant to use.
 
     Returns:
-        NDArray: The downselected power interpolants for the selected conditions.
+        NDArray: The down selected power interpolants for the selected conditions.
     """
     downselect_power_interps = np.empty_like(power_interps)
     # Loop over the wind directions, wind speeds, and turbines, finding the power interpolant
     # that is closest to the specified multi-dimensional condition.
     for i, wd in enumerate(power_interps):
         for j, ws in enumerate(wd):
             for k, turb in enumerate(ws):
@@ -418,101 +415,88 @@
             of points to use on the turbine grid. This number will be
             squared so that the points can be evenly distributed.
             Defaults to 5.
         rloc (:py:obj: float, optional): A value, from 0 to 1, that determines
             the width/height of the grid of points on the rotor as a ratio of
             the rotor radius.
             Defaults to 0.5.
+        power_thrust_data_file (:py:obj:`str`): The path and name of the file containing the
+            multidimensional power thrust curve. The path may be an absolute location or a relative
+            path to where FLORIS is being run.
+        multi_dimensional_cp_ct (:py:obj:`bool`, optional): Indicates if the turbine definition is
+            single dimensional (False) or multidimensional (True).
+        turbine_library_path (:py:obj:`pathlib.Path`, optional): The
+            :py:attr:`Farm.turbine_library_path` or :py:attr:`Farm.internal_turbine_library_path`,
+            whichever is being used to load turbine definitions.
+            Defaults to the internal turbine library.
     """
-
-    power_thrust_data_file: str = field(default=None)
     multi_dimensional_cp_ct: bool = field(default=False)
+    power_thrust_table: dict = field(default={})
+    # TODO power_thrust_data_file is actually required and should not default to None.
+    # However, the super class has optional attributes so a required attribute here breaks
+    power_thrust_data_file: str = field(default=None)
+    power_thrust_data: MultiDimensionalPowerThrustTable = field(default=None)
+    turbine_library_path: Path = field(
+        default=Path(__file__).parents[1] / "turbine_library",
+        converter=convert_to_path,
+        validator=attrs.validators.instance_of(Path)
+    )
 
-    # rloc: float = float_attrib()  # TODO: goes here or on the Grid?
-    # use_points_on_perimeter: bool = bool_attrib()
-
-    # Initialized in the post_init function
-    # rotor_radius: float = field(init=False)
-    # rotor_area: float = field(init=False)
-    # fCp_interp: interp1d = field(init=False)
-    # fCt_interp: interp1d = field(init=False)
-    # power_interp: interp1d = field(init=False)
-    # tilt_interp: interp1d = field(init=False)
-
-
-    # For the following parameters, use default values if not user-specified
-    # self.rloc = float(input_dictionary["rloc"]) if "rloc" in input_dictionary else 0.5
-    # if "use_points_on_perimeter" in input_dictionary:
-    #     self.use_points_on_perimeter = bool(input_dictionary["use_points_on_perimeter"])
-    # else:
-    #     self.use_points_on_perimeter = False
+    # Not to be provided by the user
+    condition_keys: list[str] = field(init=False, factory=list)
 
     def __attrs_post_init__(self) -> None:
+        super().__post_init__()
+
+        # Solidify the data file path and name
+        self.power_thrust_data_file = self.turbine_library_path / self.power_thrust_data_file
 
         # Read in the multi-dimensional data supplied by the user.
         df = pd.read_csv(self.power_thrust_data_file)
 
         # Build the multi-dimensional power/thrust table
         self.power_thrust_data = MultiDimensionalPowerThrustTable.from_dataframe(df)
 
         # Create placeholders for the interpolation functions
         self.fCt_interp = {}
         self.power_interp = {}
 
         # Down-select the DataFrame to have just the ws, Cp, and Ct values
         index_col = df.columns.values[:-3]
+        self.condition_keys = index_col.tolist()
         df2 = df.set_index(index_col.tolist())
 
         # Loop over the multi-dimensional keys to get the correct ws/Cp/Ct data to make
         # the Ct and power interpolants.
         for key in df2.index.unique():
             # Select the correct ws/Cp/Ct data
             data = df2.loc[key]
 
             # Build the interpolants
             wind_speeds = data['ws'].values
-            self.fCp_interp = interp1d(
+            cp_interp = interp1d(
                 wind_speeds,
                 data['Cp'].values,
                 fill_value=(0.0, 1.0),
                 bounds_error=False,
             )
-            inner_power = (
-                0.5 * self.rotor_area
-                * self.fCp_interp(wind_speeds)
-                * self.generator_efficiency
-                * wind_speeds ** 3
-            )
             self.power_interp.update({
                 key: interp1d(
                     wind_speeds,
-                    inner_power,
+                    (
+                        0.5 * self.rotor_area
+                        * cp_interp(wind_speeds)
+                        * self.generator_efficiency
+                        * wind_speeds ** 3
+                    ),
                     bounds_error=False,
                     fill_value=0
                 )
             })
             self.fCt_interp.update({
                 key: interp1d(
                     wind_speeds,
                     data['Ct'].values,
                     fill_value=(0.0001, 0.9999),
                     bounds_error=False,
                 )
             })
-
-        # If defined, create a tilt interpolation function for floating turbines.
-        # fill_value currently set to apply the min or max tilt angles if outside
-        # of the interpolation range.
-        if self.floating_tilt_table is not None:
-            self.floating_tilt_table = TiltTable.from_dict(self.floating_tilt_table)
-            self.fTilt_interp = interp1d(
-                self.floating_tilt_table.wind_speeds,
-                self.floating_tilt_table.tilt,
-                fill_value=(0.0, self.floating_tilt_table.tilt[-1]),
-                bounds_error=False,
-            )
-            self.tilt_interp = self.fTilt_interp
-            self.correct_cp_ct_for_tilt = self.floating_correct_cp_ct_for_tilt
-        else:
-            self.fTilt_interp = None
-            self.tilt_interp = None
-            self.correct_cp_ct_for_tilt = False
```

### Comparing `FLORIS-3.5/floris/simulation/wake.py` & `FLORIS-3.6/floris/simulation/wake.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     model_strings: dict = field(converter=dict)
     enable_secondary_steering: bool = field(converter=bool)
     enable_yaw_added_recovery: bool = field(converter=bool)
     enable_transverse_velocities: bool = field(converter=bool)
 
     wake_deflection_parameters: dict = field(converter=dict)
     wake_turbulence_parameters: dict = field(converter=dict)
-    wake_velocity_parameters: dict = field(converter=dict, default={})
+    wake_velocity_parameters: dict = field(converter=dict, factory=dict)
 
     combination_model: BaseModel = field(init=False)
     deflection_model: BaseModel = field(init=False)
     turbulence_model: BaseModel = field(init=False)
     velocity_model: BaseModel = field(init=False)
 
     def __attrs_post_init__(self) -> None:
```

### Comparing `FLORIS-3.5/floris/simulation/wake_combination/__init__.py` & `FLORIS-3.6/floris/simulation/wake_combination/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_combination/fls.py` & `FLORIS-3.6/floris/simulation/wake_combination/fls.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def prepare_function(self) -> dict:
         pass
 
     def function(self, wake_field: np.ndarray, velocity_field: np.ndarray):
         """
         Combines the base flow field with the velocity deficits
-        using freestream linear superpostion. In other words, the wake
+        using freestream linear superposition. In other words, the wake
         field and base fields are simply added together.
 
         Args:
             u_field (np.array): The base flow field.
             u_wake (np.array): The wake to apply to the base flow field.
 
         Returns:
```

### Comparing `FLORIS-3.5/floris/simulation/wake_combination/max.py` & `FLORIS-3.6/floris/simulation/wake_combination/max.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     def prepare_function(self) -> dict:
         pass
 
     def function(self, wake_field: np.ndarray, velocity_field: np.ndarray):
         """
-        Incorporates the velicty deficits into the base flow field by
+        Incorporates the velocity deficits into the base flow field by
         selecting the maximum of the two for each point.
 
         Args:
             u_field (np.array): The base flow field.
             u_wake (np.array): The wake to apply to the base flow field.
 
         Returns:
```

### Comparing `FLORIS-3.5/floris/simulation/wake_combination/sosfs.py` & `FLORIS-3.6/floris/simulation/wake_combination/sosfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
 
     def prepare_function(self) -> dict:
         pass
 
     def function(self, wake_field: np.ndarray, velocity_field: np.ndarray):
         """
-        Combines the base flow field with the velocity defecits
+        Combines the base flow field with the velocity deficits
         using sum of squares.
 
         Args:
             u_field (np.array): The base flow field.
             u_wake (np.array): The wake to apply to the base flow field.
 
         Returns:
```

### Comparing `FLORIS-3.5/floris/simulation/wake_deflection/__init__.py` & `FLORIS-3.6/floris/simulation/wake_deflection/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_deflection/empirical_gauss.py` & `FLORIS-3.6/floris/simulation/wake_deflection/empirical_gauss.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 from floris.utilities import cosd, sind
 
 
 @define
 class EmpiricalGaussVelocityDeflection(BaseModel):
     """
     The Empirical Gauss deflection model is based on the form of previous the
-    Guass deflection model (see :cite:`bastankhah2016experimental` and
+    Gauss deflection model (see :cite:`bastankhah2016experimental` and
     :cite:`King2019Controls`) but simplifies the formulation for simpler
     tuning and more independence from the velocity deficit model.
 
     parameter_dictionary (dict): Model-specific parameters.
         Default values are used when a parameter is not included
         in `parameter_dictionary`. Possible key-value pairs include:
 
             -   **horizontal_deflection_gain_D** (*float*): Gain for the
-                maximum (y-direction) deflection acheived far downstream
+                maximum (y-direction) deflection achieved far downstream
                 of a yawed turbine.
             -   **vertical_deflection_gain_D** (*float*): Gain for the
-                maximum vertical (z-direction) deflection acheived at a
+                maximum vertical (z-direction) deflection achieved at a
                 far downstream location due to rotor tilt. Specifying as
                 -1 will mean that vertical deflections due to tilt match
                 horizontal deflections due to yaw.
             -   **deflection_rate** (*float*): Rate at which the
                 deflected wake center approaches its maximum deflection.
             -   **mixing_gain_deflection** (*float*): Gain to set the
                 reduction in deflection due to wake-induced mixing.
@@ -97,15 +97,15 @@
             y_i (np.array): Cross stream direction grid coordinates of
                 the ith turbine (m) [not used].
             yaw_i (np.array): Yaw angle of the ith turbine (deg).
             tilt_i (np.array): Tilt angle of the ith turbine (deg).
             mixing_i (np.array): The wake-induced mixing term for the
                 ith turbine.
             ct_i (np.array): Thrust coefficient for the ith turbine (-).
-            rotor_diameter_i (np.array): Rotor diamter for the ith
+            rotor_diameter_i (np.array): Rotor diameter for the ith
                 turbine (m).
 
             x (np.array): Streamwise direction grid coordinates of the
                 flow field domain (m).
 
         Returns:
             np.array: Deflection field for the wake.
```

### Comparing `FLORIS-3.5/floris/simulation/wake_deflection/gauss.py` & `FLORIS-3.6/floris/simulation/wake_deflection/gauss.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,33 @@
 
 from __future__ import annotations
 
 from typing import Any
 
 import numexpr as ne
 import numpy as np
-from attrs import define, field
+from attrs import (
+    define,
+    field,
+    fields,
+)
 from numpy import pi
 
 from floris.simulation import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import cosd, sind
 
 
+NUM_EPS = fields(BaseModel).NUM_EPS.default
+
 @define
 class GaussVelocityDeflection(BaseModel):
     """
     The Gauss deflection model is a blend of the models described in
     :cite:`gdm-bastankhah2016experimental` and :cite:`gdm-King2019Controls` for
     calculating the deflection field in turbine wakes.
 
@@ -120,29 +126,15 @@
     ):
         """
         Calculates the deflection field of the wake. See
         :cite:`gdm-bastankhah2016experimental` and :cite:`gdm-King2019Controls`
         for details on the methods used.
 
         Args:
-            x_locations (np.array): An array of floats that contains the
-                streamwise direction grid coordinates of the flow field
-                domain (m).
-            y_locations (np.array): An array of floats that contains the grid
-                coordinates of the flow field domain in the direction normal to
-                x and parallel to the ground (m).
-            z_locations (np.array): An array of floats that contains the grid
-                coordinates of the flow field domain in the vertical
-                direction (m).
-            turbine (:py:obj:`floris.simulation.turbine`): Object that
-                represents the turbine creating the wake.
-            coord (:py:obj:`floris.utilities.Vec3`): Object containing
-                the coordinate of the turbine creating the wake (m).
-            flow_field (:py:class:`floris.simulation.flow_field`): Object
-                containing the flow field information for the wind farm.
+            # TODO
 
         Returns:
             np.array: Deflection field for the wake.
         """
         # ==============================================================
 
         # Opposite sign convention in this model
@@ -305,37 +297,37 @@
 
     turbine_average_velocity = np.cbrt(np.mean(u_i ** 3, axis=(3, 4)))[:, :, :, None, None]
     Gamma_wake_rotation = 0.25 * 2 * pi * D * (aI - aI ** 2) * turbine_average_velocity / TSR
 
     ### compute the spanwise and vertical velocities induced by yaw
 
     # decay = eps ** 2 / (4 * nu * delta_x / Uinf + eps ** 2)   # This is the decay downstream
-    yLocs = delta_y + BaseModel.NUM_EPS
+    yLocs = delta_y + NUM_EPS
 
     # top vortex
     # NOTE: this is the top of the grid, not the top of the rotor
-    zT = z_i - (HH + D / 2) + BaseModel.NUM_EPS  # distance from the top of the grid
+    zT = z_i - (HH + D / 2) + NUM_EPS  # distance from the top of the grid
     rT = ne.evaluate("yLocs ** 2 + zT ** 2")  # TODO: This is (-) in the paper
     # This looks like spanwise decay;
     # it defines the vortex profile in the spanwise directions
     core_shape = ne.evaluate("1 - exp(-rT / (eps ** 2))")
     v_top = ne.evaluate("(Gamma_top * zT) / (2 * pi * rT) * core_shape")
     v_top = np.mean( v_top, axis=(3,4) )
     # w_top = (-1 * Gamma_top * yLocs) / (2 * pi * rT) * core_shape * decay
 
     # bottom vortex
-    zB = z_i - (HH - D / 2) + BaseModel.NUM_EPS
+    zB = z_i - (HH - D / 2) + NUM_EPS
     rB = ne.evaluate("yLocs ** 2 + zB ** 2")
     core_shape = ne.evaluate("1 - exp(-rB / (eps ** 2))")
     v_bottom = ne.evaluate("(Gamma_bottom * zB) / (2 * pi * rB) * core_shape")
     v_bottom = np.mean( v_bottom, axis=(3,4) )
     # w_bottom = (-1 * Gamma_bottom * yLocs) / (2 * pi * rB) * core_shape * decay
 
     # wake rotation vortex
-    zC = z_i - HH + BaseModel.NUM_EPS
+    zC = z_i - HH + NUM_EPS
     rC = ne.evaluate("yLocs ** 2 + zC ** 2")
     core_shape = ne.evaluate("1 - exp(-rC / (eps ** 2))")
     v_core = ne.evaluate("(Gamma_wake_rotation * zC) / (2 * pi * rC) * core_shape")
     v_core = np.mean( v_core, axis=(3,4) )
     # w_core = (-1 * Gamma_wake_rotation * yLocs) / (2 * pi * rC) * core_shape * decay
 
     # Cap the effective yaw values between -45 and 45 degrees
@@ -407,59 +399,59 @@
     lmda = D / 8
     kappa = 0.41
     lm = kappa * z / (1 + kappa * z / lmda)
     nu = lm ** 2 * np.abs(dudz_initial)
 
     # This is the decay downstream
     decay = ne.evaluate("eps ** 2 / (4 * nu * delta_x / Uinf + eps ** 2)")
-    yLocs = delta_y + BaseModel.NUM_EPS
+    yLocs = delta_y + NUM_EPS
 
     # top vortex
-    zT = z - (HH + D / 2) + BaseModel.NUM_EPS
+    zT = z - (HH + D / 2) + NUM_EPS
     rT = ne.evaluate("yLocs ** 2 + zT ** 2")  # TODO: This is - in the paper
     # This looks like spanwise decay;
     # it defines the vortex profile in the spanwise directions
     core_shape = ne.evaluate("1 - exp(-rT / (eps ** 2))")
     V1 = ne.evaluate("(Gamma_top * zT) / (2 * pi * rT) * core_shape * decay")
     W1 = ne.evaluate("(-1 * Gamma_top * yLocs) / (2 * pi * rT) * core_shape * decay")
 
     # bottom vortex
-    zB = z - (HH - D / 2) + BaseModel.NUM_EPS
+    zB = z - (HH - D / 2) + NUM_EPS
     rB = ne.evaluate("yLocs ** 2 + zB ** 2")
     core_shape = ne.evaluate("1 - exp(-rB / (eps ** 2))")
     V2 = ne.evaluate("(Gamma_bottom * zB) / (2 * pi * rB) * core_shape * decay")
     W2 = ne.evaluate("(-1 * Gamma_bottom * yLocs) / (2 * pi * rB) * core_shape * decay")
 
     # wake rotation vortex
-    zC = z - HH + BaseModel.NUM_EPS
+    zC = z - HH + NUM_EPS
     rC = ne.evaluate("yLocs ** 2 + zC ** 2")
     core_shape = ne.evaluate("1 - exp(-rC / (eps ** 2))")
     V5 = ne.evaluate("(Gamma_wake_rotation * zC) / (2 * pi * rC) * core_shape * decay")
     W5 = ne.evaluate("(-1 * Gamma_wake_rotation * yLocs) / (2 * pi * rC) * core_shape * decay")
 
     ### Boundary condition - ground mirror vortex
 
     # top vortex - ground
-    zTb = z + (HH + D / 2) + BaseModel.NUM_EPS
+    zTb = z + (HH + D / 2) + NUM_EPS
     rTb = ne.evaluate("yLocs ** 2 + zTb ** 2")
     # This looks like spanwise decay;
     # it defines the vortex profile in the spanwise directions
     core_shape = ne.evaluate("1 - exp(-rTb / (eps ** 2))")
     V3 = ne.evaluate("(-1 * Gamma_top * zTb) / (2 * pi * rTb) * core_shape * decay")
     W3 = ne.evaluate("(Gamma_top * yLocs) / (2 * pi * rTb) * core_shape * decay")
 
     # bottom vortex - ground
-    zBb = z + (HH - D / 2) + BaseModel.NUM_EPS
+    zBb = z + (HH - D / 2) + NUM_EPS
     rBb = ne.evaluate("yLocs ** 2 + zBb ** 2")
     core_shape = ne.evaluate("1 - exp(-rBb / (eps ** 2))")
     V4 = ne.evaluate("(-1 * Gamma_bottom * zBb) / (2 * pi * rBb) * core_shape * decay")
     W4 = ne.evaluate("(Gamma_bottom * yLocs) / (2 * pi * rBb) * core_shape * decay")
 
     # wake rotation vortex - ground effect
-    zCb = z + HH + BaseModel.NUM_EPS
+    zCb = z + HH + NUM_EPS
     rCb = ne.evaluate("yLocs ** 2 + zCb ** 2")
     core_shape = ne.evaluate("1 - exp(-rCb / (eps ** 2))")
     V6 = ne.evaluate("(-1 * Gamma_wake_rotation * zCb) / (2 * pi * rCb) * core_shape * decay")
     W6 = ne.evaluate("(Gamma_wake_rotation * yLocs) / (2 * pi * rCb) * core_shape * decay")
 
     # total spanwise velocity
     V = V1 + V2 + V3 + V4 + V5 + V6
```

### Comparing `FLORIS-3.5/floris/simulation/wake_deflection/jimenez.py` & `FLORIS-3.6/floris/simulation/wake_deflection/jimenez.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 from floris.utilities import cosd, sind
 
 
 @define
 class JimenezVelocityDeflection(BaseModel):
     """
-    Jiménez wake deflection model, dervied from
+    Jiménez wake deflection model, derived from
     :cite:`jdm-jimenez2010application`.
 
     References:
         .. bibliography:: /references.bib
             :style: unsrt
             :filter: docname in docnames
             :keyprefix: jdm-
@@ -63,15 +63,15 @@
         turbulence_intensity_i: np.ndarray,
         ct_i: np.ndarray,
         rotor_diameter_i: np.ndarray,
         *,
         x: np.ndarray,
     ):
         """
-        Calcualtes the deflection field of the wake in relation to the yaw of
+        Calculates the deflection field of the wake in relation to the yaw of
         the turbine. This is coded as defined in [1].
 
         Args:
             x_locations (np.array): streamwise locations in wake
             y_locations (np.array): spanwise locations in wake
             z_locations (np.array): vertical locations in wake
                 (not used in Jiménez)
```

### Comparing `FLORIS-3.5/floris/simulation/wake_deflection/none.py` & `FLORIS-3.6/floris/simulation/wake_deflection/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_turbulence/__init__.py` & `FLORIS-3.6/floris/simulation/wake_turbulence/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_turbulence/crespo_hernandez.py` & `FLORIS-3.6/floris/simulation/wake_turbulence/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_turbulence/none.py` & `FLORIS-3.6/floris/simulation/wake_turbulence/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_turbulence/wake_induced_mixing.py` & `FLORIS-3.6/floris/simulation/wake_turbulence/wake_induced_mixing.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/__init__.py` & `FLORIS-3.6/floris/simulation/wake_velocity/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/cumulative_gauss_curl.py` & `FLORIS-3.6/floris/simulation/wake_velocity/cumulative_gauss_curl.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 )
 
 
 @define
 class CumulativeGaussCurlVelocityDeficit(BaseModel):
     """
     The cumulative curl model is an implementation of the model described in
-    :cite:`gdm-bay_2022`, which itself is based on the cumulative model of
-    :cite:`bastankhah_2021`
+    :cite:`cc-bay_2022`, which itself is based on the cumulative model of
+    :cite:`cc-bastankhah_2021`.
 
     References:
-    .. bibliography:: /references.bib
-        :style: unsrt
-        :filter: docname in docnames
-        :keyprefix: gdm-
+        .. bibliography:: /references.bib
+            :style: unsrt
+            :filter: docname in docnames
+            :keyprefix: cc-
     """
 
     a_s: float = field(default=0.179367259)
     b_s: float = field(default=0.0118889215)
     c_s1: float = field(default=0.0563691592)
     c_s2: float = field(default=0.13290157)
     a_f: float = field(default=3.11)
@@ -131,16 +131,16 @@
         sum_lbda = np.zeros_like(u_initial)
 
         for m in range(0, ii - 1):
             x_coord_m = x_coord[:, :, m:m+1]
             y_coord_m = y_coord[:, :, m:m+1]
             z_coord_m = z_coord[:, :, m:m+1]
 
-            # For computing crossplanes, we don't need to compute downstream
-            # turbines from out crossplane position.
+            # For computing cross planes, we don't need to compute downstream
+            # turbines from out cross plane position.
             if x_coord[:, :, m:m+1].size == 0:
                 break
 
             delta_x_m = x - x_coord_m
 
             sigma_i = wake_expansion(
                 delta_x_m,
```

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/empirical_gauss.py` & `FLORIS-3.6/floris/simulation/wake_velocity/empirical_gauss.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
                 increase in wake expansion due to wake-induced mixing.
 
     References:
         .. bibliography:: /references.bib
             :style: unsrt
             :filter: docname in docnames
     """
-    wake_expansion_rates: list = field(default=[0.023, 0.008])
-    breakpoints_D: list = field(default=[10])
+    wake_expansion_rates: list = field(factory=lambda: [0.023, 0.008])
+    breakpoints_D: list = field(factory=lambda: [10])
     sigma_0_D: float = field(default=0.28)
     smoothing_length_D: float = field(default=2.0)
     mixing_gain_velocity: float = field(default=2.0)
 
     def prepare_function(
         self,
         grid: Grid,
@@ -223,15 +223,15 @@
                 ct_i,
                 yaw_angle,
                 tilt_angle_i,
                 rotor_diameter_i,
                 sigma_y0,
                 sigma_z0
             )
-            # Normalize to match end of acuator disk model tube
+            # Normalize to match end of actuator disk model tube
             C_mirr = C_mirr / (8 * self.sigma_0_D**2)
 
             # ASSUME sum-of-squares superposition for the real and mirror wakes
             wake_deficit = np.sqrt(
                 wake_deficit**2 +
                 gaussian_function(C_mirr, r_mirr, 1, np.sqrt(0.5))**2
             )
```

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/gauss.py` & `FLORIS-3.6/floris/simulation/wake_velocity/gauss.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
         # This mask defines the near wake; keeps the areas downstream of xR and upstream of x0
         near_wake_mask = (x > xR + 0.1) * (x < x0)
         far_wake_mask = (x >= x0)
 
         # Compute the velocity deficit in the NEAR WAKE region
         # ONLY If there are points within the near wake boundary
-        # TODO: for the turbinegrid, do we need to do this near wake calculation at all?
+        # TODO: for the TurbineGrid, do we need to do this near wake calculation at all?
         #       same question for any grid with a resolution larger than the near wake region
         if np.sum(near_wake_mask):
 
             # Calculate the wake expansion
 
             # This is a linear ramp from 0 to 1 from the start of the near wake to the start
             # of the far wake.
```

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/jensen.py` & `FLORIS-3.6/floris/simulation/wake_velocity/jensen.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 from typing import Any, Dict
 
 import numexpr as ne
 import numpy as np
-from attrs import define, field
+from attrs import (
+    define,
+    field,
+    fields,
+)
 
 from floris.simulation import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 
 
+NUM_EPS = fields(BaseModel).NUM_EPS.default
+
 @define
 class JensenVelocityDeficit(BaseModel):
     """
     The Jensen model computes the wake velocity deficit based on the classic
     Jensen/Park model :cite:`jvm-jensen1983note`.
 
     -   **we** (*float*): The linear wake decay constant that
@@ -103,15 +109,14 @@
 
         # Numexpr - do not change below without corresponding changes above.
         dx = ne.evaluate("x - x_i")
         dy = ne.evaluate("y - y_i - deflection_field_i")
         dz = ne.evaluate("z - z_i")
 
         we = self.we
-        NUM_EPS = JensenVelocityDeficit.NUM_EPS
 
         # Construct a boolean mask to include all points downstream of the turbine
         downstream_mask = ne.evaluate("dx > 0 + NUM_EPS")
 
         # Construct a boolean mask to include all points within the wake boundary
         # as defined by the Jensen model. This is a linear wake expansion that makes
         # a shape like a cone and starts at the turbine disc.
```

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/none.py` & `FLORIS-3.6/floris/simulation/wake_velocity/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/turbopark.py` & `FLORIS-3.6/floris/simulation/wake_velocity/turbopark.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         # The downstream_mask is used to avoid negative numbers in the sqrt and the
         # subsequent runtime warnings.
         # Here self.NUM_EPS is to avoid precision issues with masking, and is slightly
         # larger than 0.0
         downstream_mask = (x_i - x >= self.NUM_EPS)
         x_dist = (x_i - x) * downstream_mask / rotor_diameters
 
-        # Radial distance between turbine i and the centerlines of wakes from all
+        # Radial distance between turbine i and the center lines of wakes from all
         # real/image turbines
         r_dist = np.sqrt((y_i - (y + deflection_field)) ** 2 + (z_i - z) ** 2)
         r_dist_image = np.sqrt((y_i - (y + deflection_field)) ** 2 + (z_i - (-z)) ** 2)
 
         Cts[:, :, i:, :, :] = 0.00001
 
         # Characteristic wake widths from all turbines relative to turbine i
```

### Comparing `FLORIS-3.5/floris/simulation/wake_velocity/turbopark_lookup_table.mat` & `FLORIS-3.6/floris/simulation/wake_velocity/turbopark_lookup_table.mat`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/__init__.py` & `FLORIS-3.6/floris/tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 Examples:
     >>> import floris.tools
 
     >>> dir(floris.tools)
     ['__builtins__', '__cached__', '__doc__', '__file__', '__loader__',
     '__name__', '__package__', '__path__', '__spec__', 'cut_plane',
-    'floris_interface', 'flow_data',
+    'floris_interface',
     'layout_functions', 'optimization', 'plotting', 'power_rose',
-    'rews', 'sowfa_utilities', 'visualization', 'wind_rose']
+    'rews', 'visualization', 'wind_rose']
 """
 
 from .floris_interface import FlorisInterface
 from .floris_interface_legacy_reader import FlorisInterfaceLegacyV2
 from .parallel_computing_interface import ParallelComputingInterface
 from .uncertainty_interface import UncertaintyInterface
 from .visualization import (
@@ -48,18 +48,16 @@
 )
 from .wind_rose import WindRose
 
 
 # from floris.tools import (
     # cut_plane,
     # floris_interface,
-    # flow_data,
     # interface_utilities,
     # layout_functions,
     # optimization,
     # plotting,
     # power_rose,
     # rews,
-    # sowfa_utilities,
     # visualization,
     # wind_rose,
 # )
```

### Comparing `FLORIS-3.5/floris/tools/cut_plane.py` & `FLORIS-3.6/floris/tools/cut_plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,17 +350,17 @@
 def calculate_wind_speed(cross_plane, x1_loc, x2_loc, R):
     """
     Calculate effective wind speed within specified range of a point.
 
     Args:
         cross_plane (:py:class:`floris.tools.cut_plane.CrossPlane`):
             plane of data.
-        x1_loc (float): x1-coordinate of point of interst.
-        x2_loc (float): x2-coordinate of point of interst.
-        R (float): radius from point of interst to consider
+        x1_loc (float): x1-coordinate of point of interest.
+        x2_loc (float): x2-coordinate of point of interest.
+        R (float): radius from point of interest to consider
 
     Returns:
         (float): effective wind speed
     """
 
     # Temp local copy
     df = cross_plane.df.copy()
@@ -389,16 +389,16 @@
 ):
     """
     Calculate maximum power available in a given cross plane.
 
     Args:
         cross_plane (:py:class:`floris.tools.cut_plane.CrossPlane`):
             plane of data.
-        x1_loc (float): x1-coordinate of point of interst.
-        x2_loc (float): x2-coordinate of point of interst.
+        x1_loc (float): x1-coordinate of point of interest.
+        x2_loc (float): x2-coordinate of point of interest.
         R (float): Radius of wind turbine rotor.
         ws_array (np.array): reference wind speed for cp curve.
         cp_array (np.array): cp curve at reference wind speeds.
         air_density (float, optional): air density. Defaults to 1.225.
 
     Returns:
         float: Power!
```

### Comparing `FLORIS-3.5/floris/tools/floris_interface.py` & `FLORIS-3.6/floris/tools/floris_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,56 +10,65 @@
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 
 from __future__ import annotations
 
+import inspect
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
-from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
 
-from floris.logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 from floris.simulation import Floris, State
 from floris.simulation.turbine import (
     average_velocity,
     axial_induction,
     Ct,
     power,
     rotor_effective_velocity,
 )
 from floris.simulation.turbine_multi_dim import multidim_power_down_select, power_multidim
 from floris.tools.cut_plane import CutPlane
 from floris.type_dec import NDArrayFloat
 
 
-class FlorisInterface(LoggerBase):
+class FlorisInterface(LoggingManager):
     """
     FlorisInterface provides a high-level user interface to many of the
     underlying methods within the FLORIS framework. It is meant to act as a
     single entry-point for the majority of users, simplifying the calls to
     methods on objects within FLORIS.
 
     Args:
-        configuration (:py:obj:`dict`): The Floris configuration dictarionary or YAML file.
+        configuration (:py:obj:`dict`): The Floris configuration dictionary or YAML file.
             The configuration should have the following inputs specified.
                 - **flow_field**: See `floris.simulation.flow_field.FlowField` for more details.
                 - **farm**: See `floris.simulation.farm.Farm` for more details.
                 - **turbine**: See `floris.simulation.turbine.Turbine` for more details.
                 - **wake**: See `floris.simulation.wake.WakeManager` for more details.
                 - **logging**: See `floris.simulation.floris.Floris` for more details.
     """
 
     def __init__(self, configuration: dict | str | Path):
         self.configuration = configuration
 
         if isinstance(self.configuration, (str, Path)):
-            self.floris = Floris.from_file(self.configuration)
+            try:
+                self.floris = Floris.from_file(self.configuration)
+            except FileNotFoundError:
+                # If the file cannot be found, then attempt the configuration path relative to the
+                # file location from which FlorisInterface was attempted to be run. If successful,
+                # update self.configuration to an absolute, working file path and name.
+                base_fn = Path(inspect.stack()[-1].filename).resolve().parent
+                config = (base_fn / self.configuration).resolve()
+                self.floris = Floris.from_file(config)
+                self.configuration = config
 
         elif isinstance(self.configuration, dict):
             self.floris = Floris.from_dict(self.configuration)
 
         else:
             raise TypeError("The Floris `configuration` must be of type 'dict', 'str', or 'Path'.")
 
@@ -580,15 +589,15 @@
         if len(ws) > 1 or len(ws) < 1:
             raise ValueError(
                 "Wind speed input must be of length 1 for visualization. "
                 f"Current length is {len(ws)}."
             )
 
     def get_turbine_powers(self) -> NDArrayFloat:
-        """Calculates the power at each turbine in the windfarm.
+        """Calculates the power at each turbine in the wind farm.
 
         Returns:
             NDArrayFloat: Powers at each turbine.
         """
 
         # Confirm calculate wake has been run
         if self.floris.state is not State.USED:
@@ -606,15 +615,15 @@
             rotor_effective_velocities=self.turbine_effective_velocities,
             power_interp=self.floris.farm.turbine_power_interps,
             turbine_type_map=self.floris.farm.turbine_type_map,
         )
         return turbine_powers
 
     def get_turbine_powers_multidim(self) -> NDArrayFloat:
-        """Calculates the power at each turbine in the windfarm
+        """Calculates the power at each turbine in the wind farm
         when using multi-dimensional Cp/Ct turbine definitions.
 
         Returns:
             NDArrayFloat: Powers at each turbine.
         """
 
         # Confirm calculate wake has been run
@@ -643,30 +652,30 @@
     def get_turbine_Cts(self) -> NDArrayFloat:
         turbine_Cts = Ct(
             velocities=self.floris.flow_field.u,
             yaw_angle=self.floris.farm.yaw_angles,
             tilt_angle=self.floris.farm.tilt_angles,
             ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
             fCt=self.floris.farm.turbine_fCts,
-            tilt_interp=self.floris.farm.turbine_fTilts,
+            tilt_interp=self.floris.farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
             turbine_type_map=self.floris.farm.turbine_type_map,
             average_method=self.floris.grid.average_method,
             cubature_weights=self.floris.grid.cubature_weights,
         )
         return turbine_Cts
 
     def get_turbine_ais(self) -> NDArrayFloat:
         turbine_ais = axial_induction(
             velocities=self.floris.flow_field.u,
             yaw_angle=self.floris.farm.yaw_angles,
             tilt_angle=self.floris.farm.tilt_angles,
             ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
             fCt=self.floris.farm.turbine_fCts,
-            tilt_interp=self.floris.farm.turbine_fTilts,
+            tilt_interp=self.floris.farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
             turbine_type_map=self.floris.farm.turbine_type_map,
             average_method=self.floris.grid.average_method,
             cubature_weights=self.floris.grid.cubature_weights,
         )
         return turbine_ais
 
@@ -685,15 +694,15 @@
             ref_density_cp_ct=self.floris.farm.ref_density_cp_cts,
             velocities=self.floris.flow_field.u,
             yaw_angle=self.floris.farm.yaw_angles,
             tilt_angle=self.floris.farm.tilt_angles,
             ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
             pP=self.floris.farm.pPs,
             pT=self.floris.farm.pTs,
-            tilt_interp=self.floris.farm.turbine_fTilts,
+            tilt_interp=self.floris.farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
             turbine_type_map=self.floris.farm.turbine_type_map,
             average_method=self.floris.grid.average_method,
             cubature_weights=self.floris.grid.cubature_weights
         )
         return rotor_effective_velocities
 
@@ -982,14 +991,138 @@
 
         # Check that x, y, z are all the same length
         if not len(x) == len(y) == len(z):
             raise ValueError("x, y, and z must be the same size")
 
         return self.floris.solve_for_points(x, y, z)
 
+    def sample_velocity_deficit_profiles(
+            self,
+            direction: str = 'cross-stream',
+            downstream_dists: NDArrayFloat | list = None,
+            profile_range: NDArrayFloat | list = None,
+            resolution: int = 100,
+            wind_direction: float = None,
+            homogeneous_wind_speed: float = None,
+            ref_rotor_diameter: float = None,
+            x_start: float = 0.0,
+            y_start: float = 0.0,
+            reference_height: float = None,
+    ) -> list[pd.DataFrame]:
+        """
+        Extract velocity deficit profiles at a set of downstream distances from a starting point
+        (usually a turbine location). For each downstream distance, a profile is sampled along
+        a line in either the cross-stream direction (x2) or the vertical direction (x3).
+        Velocity deficit is here defined as (homogeneous_wind_speed - u)/homogeneous_wind_speed,
+        where u is the wake velocity obtained when wind_shear = 0.0.
+
+        Args:
+            direction: At each downstream location, this is the direction in which to sample the
+                profile. Either `cross-stream` or `vertical`.
+            downstream_dists: A list/array of streamwise locations for where to sample the profiles.
+                Default starting point is (0.0, 0.0, reference_height).
+            profile_range: Determines the extent of the line along which the profiles are sampled.
+                The range is defined about a point which lies some distance directly downstream of
+                the starting point.
+            resolution: Number of sample points in each profile.
+            wind_direction: A single wind direction.
+            homogeneous_wind_speed: A single wind speed. It is called homogeneous since 'wind_shear'
+                is temporarily set to 0.0 in this method.
+            ref_rotor_diameter: A reference rotor diameter which is used to normalize the
+                coordinates.
+            x_start: x-coordinate of starting point.
+            y_start: y-coordinate of starting point.
+            reference_height: If `direction` is cross-stream, then `reference_height` defines the
+                height of the horizontal plane in which the velocity profiles are sampled.
+                If `direction` is vertical, then the velocity is sampled along the vertical
+                direction with the `profile_range` being relative to the `reference_height`.
+        Returns:
+            A list of pandas DataFrame objects where each DataFrame represents one velocity deficit
+            profile.
+        """
+
+        if direction not in ['cross-stream', 'vertical']:
+            raise ValueError("`direction` must be either `cross-stream` or `vertical`.")
+
+        if ref_rotor_diameter is None:
+            unique_rotor_diameters = np.unique(self.floris.farm.rotor_diameters)
+            if len(unique_rotor_diameters) == 1:
+                ref_rotor_diameter = unique_rotor_diameters[0]
+            else:
+                raise ValueError(
+                    "Please provide a `ref_rotor_diameter`. This is needed to normalize the "
+                    "coordinates. Could not select a value automatically since the number of "
+                    "unique rotor diameters in the turbine layout is not 1. "
+                    f"Found the following rotor diameters: {unique_rotor_diameters}."
+                )
+
+        if downstream_dists is None:
+            downstream_dists = ref_rotor_diameter * np.array([3, 5, 7, 9])
+
+        if profile_range is None:
+            profile_range = ref_rotor_diameter * np.array([-2, 2])
+
+        wind_directions_copy = np.array(self.floris.flow_field.wind_directions, copy=True)
+        wind_speeds_copy = np.array(self.floris.flow_field.wind_speeds, copy=True)
+        wind_shear_copy = self.floris.flow_field.wind_shear
+
+        if wind_direction is None:
+            if len(wind_directions_copy) == 1:
+                wind_direction = wind_directions_copy[0]
+            else:
+                raise ValueError(
+                    "Could not determine a wind direction for which to sample the velocity "
+                    "profiles. Either provide a single `wind_direction` as an argument to this "
+                    "method, or initialize the Floris object with a single wind direction."
+                )
+
+        if homogeneous_wind_speed is None:
+            if len(wind_speeds_copy) == 1:
+                homogeneous_wind_speed = wind_speeds_copy[0]
+                self.logger.warning(
+                    "`homogeneous_wind_speed` not provided. Setting it to the following wind speed "
+                    f"found in the current flow field: {wind_speeds_copy[0]} m/s. Note that the "
+                    "inflow is always homogeneous when calculating the velocity deficit profiles. "
+                    "This is done by temporarily setting `wind_shear` to 0.0"
+                )
+            else:
+                raise ValueError(
+                    "Could not determine a wind speed for which to sample the velocity "
+                    "profiles. Provide a single `homogeneous_wind_speed` to this method."
+                )
+
+        if reference_height is None:
+            reference_height = self.floris.flow_field.reference_wind_height
+
+        self.reinitialize(
+            wind_directions=[wind_direction],
+            wind_speeds=[homogeneous_wind_speed],
+            wind_shear=0.0,
+        )
+
+        velocity_deficit_profiles = self.floris.solve_for_velocity_deficit_profiles(
+            direction,
+            downstream_dists,
+            profile_range,
+            resolution,
+            homogeneous_wind_speed,
+            ref_rotor_diameter,
+            x_start,
+            y_start,
+            reference_height,
+        )
+
+        self.reinitialize(
+            wind_directions=wind_directions_copy,
+            wind_speeds=wind_speeds_copy,
+            wind_shear=wind_shear_copy,
+        )
+
+        return velocity_deficit_profiles
+
     @property
     def layout_x(self):
         """
         Wind turbine coordinate information.
 
         Returns:
             np.array: Wind turbine x-coordinate.
@@ -1014,12 +1147,12 @@
             z (bool): When *True*, return lists of x, y, and z coords,
             otherwise, return x and y only. Defaults to *False*.
 
         Returns:
             np.array: lists of x, y, and (optionally) z coordinates of
                 each turbine
         """
-        xcoords, ycoords, zcoords = np.array([c.elements for c in self.floris.farm.coordinates]).T
+        xcoords, ycoords, zcoords = self.floris.farm.coordinates.T
         if z:
             return xcoords, ycoords, zcoords
         else:
             return xcoords, ycoords
```

### Comparing `FLORIS-3.5/floris/tools/floris_interface_legacy_reader.py` & `FLORIS-3.6/floris/tools/floris_interface_legacy_reader.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/interface_utilities.py` & `FLORIS-3.6/floris/tools/interface_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ):
 
     if wake_velocity_model:
         obj = "fi.floris.wake.velocity_model"
         # props = get_props(obj, fi)
         props = fi.floris.wake._asdict()
         # props = props["wake_velocity_parameters"][fi.floris.wake.velocity_model.model_string]
+        # NOTE: _get_model_dict is remove and model.as_dict() should be used instead
         props = fi.floris.wake.velocity_model._get_model_dict()
 
         if verbose:
             print("=".join(["="] * 39))
         else:
             print("=".join(["="] * 19))
         print(
```

### Comparing `FLORIS-3.5/floris/tools/layout_functions.py` & `FLORIS-3.6/floris/tools/layout_functions.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_base.py` & `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import numpy as np
 from shapely.geometry import LineString, Polygon
 
 from floris.tools.optimization.yaw_optimization.yaw_optimizer_geometric import (
     YawOptimizationGeometric,
 )
 
-from ....logging_manager import LoggerBase
+from ....logging_manager import LoggingManager
 
 
-class LayoutOptimization(LoggerBase):
+class LayoutOptimization(LoggingManager):
     def __init__(self, fi, boundaries, min_dist=None, freq=None, enable_geometric_yaw=False):
         self.fi = fi.copy()
         self.boundaries = boundaries
         self.enable_geometric_yaw = enable_geometric_yaw
 
         self._boundary_polygon = Polygon(self.boundaries)
         self._boundary_line = LineString(self.boundaries)
```

### Comparing `FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py` & `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py` & `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py` & `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py` & `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/layout.py` & `FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/optimization.py` & `FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
-from ....logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 
 
-class Optimization(LoggerBase):
+class Optimization(LoggingManager):
     """
     Base optimization class.
 
     Args:
         fi (:py:class:`floris.tools.floris_utilities.FlorisInterface`):
             Interface from FLORIS to the tools package.
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/power_density.py` & `FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/power_density.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/pyoptsparse/yaw.py` & `FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/yaw.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See https://floris.readthedocs.io for documentation
 
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import norm
 
-from ...visualization import visualize_cut_plane
+from floris.tools.visualization import visualize_cut_plane
 
 
 class Yaw:
     """
     Class that performs yaw optimization for a single set of
     inflow conditions. Intended to be used together with an object of the
     :py:class`floris.tools.optimization.optimization.Optimization` class.
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/base_COE.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/base_COE.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/cluster_turbines.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/cluster_turbines.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/layout.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/layout_height.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout_height.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/optimization.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/optimization.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
-import matplotlib.pyplot as plt
 import numpy as np
 
 
-try:
-    from mpi4py.futures import MPIPoolExecutor
-except ImportError:
-    pass
-
-
 class Optimization:
     """
     Optimization is the base optimization class for
     `~.tools.optimization.scipy` subclasses. Contains some common
     methods and properties that can be used by the individual optimization
     classes.
     """
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/power_density.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/power_density_1D.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density_1D.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_clustered.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_clustered.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # See https://floris.readthedocs.io for documentation
 
 import copy
 
 import numpy as np
 import pandas as pd
 
-from ....logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
+
 from .cluster_turbines import cluster_turbines
 from .yaw import YawOptimization
 
 
-class YawOptimizationClustered(YawOptimization, LoggerBase):
+class YawOptimizationClustered(YawOptimization, LoggingManager):
     """
     YawOptimization is a subclass of
     :py:class:`~.tools.optimizationscipy.YawOptimization` that is used to
     perform optimizations of the yaw angles of all or a subset of wind turbines
     in a Floris Farm for a single set of inflow conditions using the scipy
     optimization package. This class facilitates the clusterization of the
     turbines inside seperate subsets in which the turbines witin each subset
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # See https://floris.readthedocs.io for documentation
 
 import copy
 
 import numpy as np
 import pandas as pd
 
-from ....logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
+
 from .cluster_turbines import cluster_turbines
 from .yaw_wind_rose import YawOptimizationWindRose
 
 
-class YawOptimizationWindRoseClustered(YawOptimizationWindRose, LoggerBase):
+class YawOptimizationWindRoseClustered(YawOptimizationWindRose, LoggingManager):
     """
     YawOptimizationWindRose is a subclass of
     :py:class:`~.tools.optimizationscipy.YawOptimizationWindRose` that is used
     to perform optimizations of the yaw angles of all or a subset of wind
     turbines in a Floris Farm for multiple sets of inflow conditions using the
     scipy optimization package. This class facilitates the clusterization of the
     turbines inside seperate subsets in which the turbines witin each subset
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 from itertools import repeat
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import minimize
 
-from ....logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
+
 from .yaw_wind_rose import YawOptimizationWindRose
 
 
-class YawOptimizationWindRoseParallel(YawOptimizationWindRose, LoggerBase):
+class YawOptimizationWindRoseParallel(YawOptimizationWindRose, LoggingManager):
     """
     YawOptimizationWindRose is a subclass of
     :py:class:`~.tools.optimizationscipy.YawOptimizationWindRose` that is used
     to perform parallel computing to optimize the yaw angles of all turbines in
     a Floris Farm for multiple sets of inflow conditions (combinations of wind
     speed, wind direction, and optionally turbulence intensity) using the scipy
     optimize package. Parallel optimization is performed using the
```

### Comparing `FLORIS-3.5/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py` & `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 import copy
 from itertools import repeat
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import minimize
 
-from ....logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
+
 from .yaw_wind_rose_clustered import YawOptimizationWindRoseClustered
 
 
-class YawOptimizationWindRoseParallelClustered(YawOptimizationWindRoseClustered, LoggerBase):
+class YawOptimizationWindRoseParallelClustered(YawOptimizationWindRoseClustered, LoggingManager):
     """
     YawOptimizationWindRoseClustered is a subclass of
     :py:class:`~.tools.optimizationscipy.YawOptimizationWindRoseClustered` that
     is used to perform optimizations of the yaw angles of all turbines in a
     Floris Farm for multiple sets of inflow conditions (combinations of wind
     speed, wind direction, and optionally turbulence intensity) using the scipy
     optimize package. This class additionally facilitates the clusterization of
```

### Comparing `FLORIS-3.5/floris/tools/optimization/other/boundary_grid.py` & `FLORIS-3.6/floris/tools/optimization/other/boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py` & `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import copy
 from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
-from floris.logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 
 from .yaw_optimization_tools import derive_downstream_turbines, find_layout_symmetry
 
 
-class YawOptimization(LoggerBase):
+class YawOptimization(LoggingManager):
     """
     YawOptimization is a subclass of :py:class:`floris.tools.optimization.scipy.
     Optimization` that is used to optimize the yaw angles of all turbines in a Floris
     Farm for a single set of inflow conditions using the SciPy optimize package.
     """
 
     def __init__(
```

### Comparing `FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py` & `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py` & `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py` & `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py` & `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 import copy
 import warnings
 from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
-from floris.logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 
 # from .yaw_optimizer_scipy import YawOptimizationScipy
 from .yaw_optimization_base import YawOptimization
 
 
-class YawOptimizationSR(YawOptimization, LoggerBase):
+class YawOptimizationSR(YawOptimization, LoggingManager):
     def __init__(
         self,
         fi,
         minimum_yaw_angle=0.0,
         maximum_yaw_angle=25.0,
         yaw_angles_baseline=None,
         x0=None,
```

### Comparing `FLORIS-3.5/floris/tools/parallel_computing_interface.py` & `FLORIS-3.6/floris/tools/parallel_computing_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import warnings
 from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
-from floris.logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 from floris.tools.optimization.yaw_optimization.yaw_optimizer_sr import YawOptimizationSR
 from floris.tools.uncertainty_interface import FlorisInterface, UncertaintyInterface
 
 
 def _load_local_floris_object(
     fi_dict,
     unc_pmfs=None,
@@ -62,15 +62,15 @@
     )
 
     # Perform optimization but silence print statements to avoid cluttering
     df_opt = yaw_opt.optimize(print_progress=print_progress)
     return df_opt
 
 
-class ParallelComputingInterface(LoggerBase):
+class ParallelComputingInterface(LoggingManager):
     def __init__(
         self,
         fi,
         max_workers,
         n_wind_direction_splits,
         n_wind_speed_splits=1,
         interface="multiprocessing",  # Options are 'multiprocessing', 'mpi4py' or 'concurrent'
```

### Comparing `FLORIS-3.5/floris/tools/power_rose.py` & `FLORIS-3.6/floris/tools/power_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/rews.py` & `FLORIS-3.6/floris/tools/rews.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/tools/uncertainty_interface.py` & `FLORIS-3.6/floris/tools/uncertainty_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 import copy
 
 import numpy as np
 from scipy.stats import norm
 
-from floris.logging_manager import LoggerBase
+from floris.logging_manager import LoggingManager
 from floris.tools import FlorisInterface
 from floris.utilities import wrap_360
 
 
-class UncertaintyInterface(LoggerBase):
+class UncertaintyInterface(LoggingManager):
     def __init__(
         self,
         configuration,
         unc_options=None,
         unc_pmfs=None,
         fix_yaw_in_relative_frame=False,
     ):
```

### Comparing `FLORIS-3.5/floris/tools/visualization.py` & `FLORIS-3.6/floris/tools/visualization.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 # See https://floris.readthedocs.io for documentation
 from __future__ import annotations
 
 import copy
 import warnings
 from typing import Union
 
+import attrs
 import matplotlib as mpl
 import matplotlib.colors as mplcolors
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from attrs import define, field
 from matplotlib import rcParams
 from scipy.spatial import ConvexHull
 
 from floris.simulation import Floris
 from floris.tools.cut_plane import CutPlane
 from floris.tools.floris_interface import FlorisInterface
+from floris.type_dec import (
+    floris_array_converter,
+    NDArrayFloat,
+)
 from floris.utilities import rotate_coordinates_rel_west, wind_delta
 
 
 def show_plots():
     plt.show()
 
 def plot_turbines(
@@ -302,15 +308,15 @@
 
     # Set the title
     ax.set_title(title)
 
     # Make equal axis
     ax.set_aspect("equal")
 
-    return im
+    return ax
 
 
 def visualize_heterogeneous_cut_plane(
     cut_plane,
     fi,
     ax=None,
     vel_component='u',
@@ -647,19 +653,28 @@
         # Now place the yaw_angles back into yaw_angles
         # to be sure not None
         yaw_angles = fi.floris.farm.yaw_angles
 
         # Grab the turbine layout
         layout_x = copy.deepcopy(fi.layout_x)
         layout_y = copy.deepcopy(fi.layout_y)
+        turbine_types = copy.deepcopy(fi.floris.farm.turbine_type)
         D = fi.floris.farm.rotor_diameters_sorted[0, 0, 0]
 
         # Declare a new layout array with an extra turbine
         layout_x_test = np.append(layout_x,[0])
         layout_y_test = np.append(layout_y,[0])
+
+        # Declare turbine types with an extra turbine in
+        # case of special one type useage
+        if len(layout_x) > 1 and len(turbine_types) == 1:
+            # Convert to list length len(layout_x) + 1
+            turbine_types_test = [turbine_types[0] for i in range(len(layout_x))] + ['nrel_5MW']
+        else:
+            turbine_types_test = np.append(turbine_types, 'nrel_5MW').tolist()
         yaw_angles = np.append(yaw_angles, np.zeros([len(wd), len(ws), 1]), axis=2)
 
         # Get a grid of points test test
         if x_bounds is None:
             x_bounds = (np.min(layout_x) - 2 * D, np.max(layout_x) + 10 * D)
 
         if y_bounds is None:
@@ -684,15 +699,19 @@
                 # Save the x and y results
                 x_results[idx] = x
                 y_results[idx] = y
 
                 # Place the test turbine at this location and calculate wake
                 layout_x_test[-1] = x
                 layout_y_test[-1] = y
-                fi.reinitialize(layout_x = layout_x_test, layout_y = layout_y_test)
+                fi.reinitialize(
+                    layout_x=layout_x_test,
+                    layout_y=layout_y_test,
+                    turbine_type=turbine_types_test
+                )
                 fi.calculate_wake(yaw_angles=yaw_angles)
 
                 # Get the velocity of that test turbines central point
                 center_point = int(np.floor(fi.floris.flow_field.u[0,0,-1].shape[0] / 2.0))
                 u_results[idx] = fi.floris.flow_field.u[0,0,-1,center_point,center_point]
 
                 # Increment index
@@ -708,7 +727,203 @@
             'w':w_results,
         })
 
         # Convert to a cut_plane
         horizontal_plane = CutPlane(df, x_resolution, y_resolution, "z")
 
         return horizontal_plane
+
+@define
+class VelocityProfilesFigure():
+    """
+    Create a figure which displays velocity deficit profiles at several downstream
+    locations of a turbine.
+
+    Args:
+        downstream_dists_D: A list/array of streamwise locations at which the velocity deficit
+            profiles have been sampled. The locations should be normalized by the turbine
+            diameter D.
+        layout: A one- or two-element list defining the direction of the profiles and in which
+            order the directions are plotted. For example, ['cross-stream', 'vertical'] initializes
+            a figure where cross-stream profiles are expected on the top row of Axes in the figure,
+            and vertical profiles are expected on the bottom row.
+        ax_width: Roughly the width of each Axes.
+        ax_height: Roughly the height of each Axes.
+        coordinate_labels: A list of labels for the normalized coordinates.
+
+    """
+    downstream_dists_D: NDArrayFloat = field(converter=floris_array_converter)
+    layout: list[str] = field(default=['cross-stream'])
+    ax_width: float = field(default=2.07)
+    ax_height: float = field(default=3.0)
+    coordinate_labels: list[str] = field(default=['x_1/D', 'x_2/D', 'x_3/D'])
+
+    n_rows: int = field(init=False)
+    n_cols: int = field(init=False)
+    fig: plt.Figure = field(init=False)
+    axs: np.ndarray = field(init=False)
+    deficit_max: float = field(init=False, default=0.0)
+
+    def __attrs_post_init__(self) -> None:
+        self.n_rows = len(self.layout)
+        self.n_cols = len(self.downstream_dists_D)
+        figsize = [0.7 + self.ax_width * self.n_cols, 1.0 + self.ax_height * self.n_rows]
+        self.fig, self.axs = plt.subplots(
+            self.n_rows,
+            self.n_cols,
+            figsize=figsize,
+            layout='tight',
+            sharex='col',
+            sharey='row',
+            squeeze=False,
+        )
+
+        for ax in self.axs[-1]:
+            ax.set_xlabel(r'$\Delta U / U_\infty$', fontsize=14)
+            ax.tick_params('x', labelsize=14)
+
+        for ax, x1_D in zip(self.axs[0], self.downstream_dists_D):
+            ax.set_title(f'${self.coordinate_labels[0]} = {x1_D:.1f}$', fontsize=14)
+
+        for ax, profile_direction in zip(self.axs[:,0], self.layout):
+            if profile_direction == 'cross-stream':
+                ylabel = f'${self.coordinate_labels[1]}$'
+            elif profile_direction == 'vertical':
+                ylabel = f'${self.coordinate_labels[2]}$'
+            ax.set_ylabel(ylabel, fontsize=14)
+            ax.tick_params('y', labelsize=14)
+
+    @layout.validator
+    def layout_validator(self, instance : attrs.Attribute, value : list[str]) -> None:
+        allowed_layouts = [
+            ['cross-stream'],
+            ['vertical'],
+            ['cross-stream', 'vertical'],
+            ['vertical', 'cross-stream'],
+        ]
+        if value not in allowed_layouts:
+            raise ValueError(f"'layout' must be one of the following: {allowed_layouts}.")
+
+    def add_profiles(
+        self,
+        velocity_deficit_profiles: list[pd.DataFrame],
+        **kwargs
+    ) -> None:
+        """
+        Add a list of velocity deficit profiles to the figure. Each profile is represented
+        as a pandas DataFrame. `kwargs` are passed to `ax.plot`.
+        """
+        for df in velocity_deficit_profiles:
+            ax, profile_direction = self.match_profile_to_axes(df)
+            profile_direction_D = f'{profile_direction}/D'
+            ax.plot(df['velocity_deficit'], df[profile_direction_D], **kwargs)
+            self.deficit_max = max(self.deficit_max, df['velocity_deficit'].max())
+
+        margin = 0.05
+        self.set_xlim([0.0 - margin, self.deficit_max + margin])
+
+    def match_profile_to_axes(
+        self,
+        df: pd.DataFrame,
+    ) -> tuple[plt.Axes, str]:
+        x1_D = np.unique(df['x1/D'])
+        if len(x1_D) == 1:
+            x1_D = x1_D[0]
+        else:
+            raise ValueError(
+                "The streamwise location x1/D must be constant for each velocity profile."
+            )
+
+        unique_x2 = np.unique(df['x2/D'])
+        unique_x3 = np.unique(df['x3/D'])
+        if len(unique_x2) == 1:
+            profile_direction = 'x3'
+            profile_direction_name = 'vertical'
+        elif len(unique_x3) == 1:
+            profile_direction = 'x2'
+            profile_direction_name = 'cross-stream'
+        else:
+            raise ValueError(
+                f"Velocity deficit profile at x1/D = {x1_D} is neither in the cross-stream (x2) "
+                "nor the vertical (x3) direction."
+            )
+        row = self.layout.index(profile_direction_name)
+
+        col = None
+        for i in range(self.n_cols):
+            if np.abs(x1_D - self.downstream_dists_D[i]) < 0.001:
+                col = i
+                break
+        if col is None:
+            raise ValueError(
+                "Could not add a velocity deficit profile at downstream distance "
+                f"x1/D = {x1_D}. The downstream distance must be one of the following "
+                "values with which this VelocityProfilesFigure object was initialized: "
+                f"{self.downstream_dists_D}."
+            )
+        return self.axs[row,col], profile_direction
+
+    def set_xlim(
+        self,
+        xlim: list[float] | NDArrayFloat,
+    ) -> None:
+        for ax in self.axs[-1]:
+            ax.set_xlim(xlim)
+
+    def add_ref_lines_x2(
+        self,
+        ref_lines_x2_D: list[float] | NDArrayFloat,
+        **kwargs
+    ) -> None:
+        """
+        Add reference lines to the VelocityProfilesFigure which go along the XAxis.
+        Commonly used to show the extent of the turbine.
+        Args:
+            ref_lines_x2_D: A list of x2-coordinates normalized by the turbine diameter D.
+                One coordinate per reference line.
+            **kwargs: Additional parameters to pass to `ax.plot`.
+        """
+        if 'cross-stream' not in self.layout:
+            raise Exception(
+                "Could not add reference lines to cross-stream (x2) velocity profiles. No "
+                "such profiles exist in the figure."
+            )
+        row_x2 = self.layout.index('cross-stream')
+        self.add_ref_lines(ref_lines_x2_D, row_x2, **kwargs)
+
+    def add_ref_lines_x3(
+        self,
+        ref_lines_x3_D: list[float] | NDArrayFloat,
+        **kwargs
+    ) -> None:
+        """
+        Add reference lines to the VelocityProfilesFigure which go along the XAxis.
+        Commonly used to show the extent of the turbine.
+        Args:
+            ref_lines_x3_D: A list of x3-coordinates normalized by the turbine diameter D.
+                One coordinate per reference line.
+            **kwargs: Additional parameters to pass to `ax.plot`.
+        """
+        if 'vertical' not in self.layout:
+            raise Exception(
+                "Could not add reference lines to vertical (x3) velocity profiles. No "
+                "such profiles exist in the figure."
+            )
+        row_x3 = self.layout.index('vertical')
+        self.add_ref_lines(ref_lines_x3_D, row_x3, **kwargs)
+
+    def add_ref_lines(
+        self,
+        ref_lines_D: list[float] | NDArrayFloat,
+        row: int,
+        **kwargs
+    ) -> None:
+        default_params = {
+                'linestyle': (0, (4, 2)),
+                'color': 'k',
+                'linewidth': 1.1
+        }
+        kwargs = default_params | kwargs
+
+        for ax in self.axs[row]:
+            for coordinate in ref_lines_D:
+                ax.plot([0.0, 1.0], [coordinate, coordinate], **kwargs)
```

### Comparing `FLORIS-3.5/floris/tools/wind_rose.py` & `FLORIS-3.6/floris/tools/wind_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/turbine_library/iea_10MW.yaml` & `FLORIS-3.6/floris/turbine_library/iea_10MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/turbine_library/iea_15MW.yaml` & `FLORIS-3.6/floris/turbine_library/iea_15MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml` & `FLORIS-3.6/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 pP: 1.88
 pT: 1.88
 rotor_diameter: 242.24
 TSR: 8.0
 ref_density_cp_ct: 1.225
 ref_tilt_cp_ct: 6.0
 multi_dimensional_cp_ct: True
-power_thrust_data_file: '../floris/turbine_library/iea_15MW_multi_dim_Tp_Hs.csv'
+power_thrust_data_file: 'iea_15MW_multi_dim_Tp_Hs.csv'
 floating_tilt_table:
   tilt:
     - 5.747296314800103
     - 7.2342400188651068
     - 9.0468701999352397
     - 9.762182013267733
     - 8.795649572299896
     - 8.089078308325314
     - 7.7229584934943614
-  wind_speeds:
+  wind_speed:
     - 4.0
     - 6.0
     - 8.0
     - 10.0
     - 12.0
     - 14.0
     - 16.0
-floating_correct_cp_ct_for_tilt: True
+correct_cp_ct_for_tilt: True
```

### Comparing `FLORIS-3.5/floris/turbine_library/nrel_5MW.yaml` & `FLORIS-3.6/floris/turbine_library/nrel_5MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/turbine_library/turbine_previewer.py` & `FLORIS-3.6/floris/turbine_library/turbine_previewer.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,124 +8,156 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
+from __future__ import annotations
+
 from pathlib import Path
 
 import attrs
 import matplotlib.pyplot as plt
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.simulation.turbine import (
     Ct,
     power,
     Turbine,
 )
-from floris.type_dec import NDArrayFloat
+from floris.simulation.turbine_multi_dim import (
+    Ct_multidim,
+    multidim_Ct_down_select,
+    multidim_power_down_select,
+    power_multidim,
+    TurbineMultiDimensional,
+)
+from floris.type_dec import convert_to_path, NDArrayFloat
 from floris.utilities import (
     load_yaml,
     round_nearest,
     round_nearest_2_or_5,
 )
 
 
 INTERNAL_LIBRARY = Path(__file__).parent
 DEFAULT_WIND_SPEEDS = np.linspace(0, 40, 81)
 
 
 @define(auto_attribs=True)
 class TurbineInterface:
-    turbine: Turbine = field(validator=attrs.validators.instance_of(Turbine))
+    turbine: Turbine | TurbineMultiDimensional = field(
+        validator=attrs.validators.instance_of((Turbine, TurbineMultiDimensional))
+    )
 
     @classmethod
-    def from_internal_library(cls, file_name: str):
-        """Loads the turbine definition from a YAML configuration file located in
-        ``floris/floris/turbine_library/``.
+    def from_library(cls, library_path: str | Path, file_name: str):
+        """Loads the turbine definition from a YAML configuration file located in either the
+        internal turbine library ``floris/floris/turbine_library/``, or a user-specified location.
 
         Args:
-            file_`name : str | Path
-                T`he file name of the turbine configuration file.
+            library_path (:obj:`str` | :obj:`pathlib.Path`): The location of the turbine library;
+                use "internal" to use the FLORIS-provided library.
+            file_name (:obj:`str` | :obj:`pathlib.Path`): The name of the configuration file.
 
         Returns:
             (TurbineInterface): Creates a new ``TurbineInterface`` object.
         """
-        return cls(turbine=Turbine.from_dict(load_yaml(INTERNAL_LIBRARY / file_name)))
+        # Use the pre-mapped internal turbine library or validate the user's library
+        if library_path == "internal":
+            library_path = INTERNAL_LIBRARY
+        else:
+            library_path = convert_to_path(library_path)
+
+        # Add in the library specification if needed, and load from dict
+        turb_dict = load_yaml(library_path / file_name)
+        if turb_dict.get("multi_dimensional_cp_ct", False):
+            turb_dict.setdefault("turbine_library_path", library_path)
+            return cls(turbine=TurbineMultiDimensional.from_dict(turb_dict))
+        return cls(turbine=Turbine.from_dict(turb_dict))
 
     @classmethod
     def from_yaml(cls, file_path: str | Path):
         """Loads the turbine definition from a YAML configuration file.
 
         Args:
             file_path : str | Path
                 The full path and file name of the turbine configuration file.
 
         Returns:
             (TurbineInterface): Creates a new ``TurbineInterface`` object.
         """
-        return cls(turbine=Turbine.from_dict(load_yaml(file_path)))
+        file_path = Path(file_path).resolve()
+
+        # Add in the library specification if needed, and load from dict
+        turb_dict = load_yaml(file_path)
+        if turb_dict.get("multi_dimensional_cp_ct", False):
+            turb_dict.setdefault("turbine_library_path", file_path.parent)
+            return cls(turbine=TurbineMultiDimensional.from_dict(turb_dict))
+        return cls(turbine=Turbine.from_dict(turb_dict))
 
     @classmethod
     def from_turbine_dict(cls, config_dict: dict):
         """Loads the turbine definition from a dictionary.
 
         Args:
             config_dict : dict
                 The ``Turbine`` configuration dictionary.
 
         Returns:
             (`TurbineInterface`): Returns a ``TurbineInterface`` object.
         """
+        if config_dict.get("multi_dimensional_cp_ct", False):
+            return cls(turbine=TurbineMultiDimensional.from_dict(config_dict))
         return cls(turbine=Turbine.from_dict(config_dict))
 
-    def power_curve(
+    def  power_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-    ) -> tuple[NDArrayFloat, NDArrayFloat]:
+    ) -> tuple[NDArrayFloat, NDArrayFloat] | tuple[NDArrayFloat, dict[tuple, NDArrayFloat]]:
         """Produces a plot-ready power curve for the turbine for wind speed vs power (MW), assuming
         no tilt or yaw effects.
 
         Args:
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
 
         Returns:
-            (tuple[NDArrayFloat, NDArrayFloat]): Returns the wind speed array and the power array.
+            (tuple[NDArrayFloat, NDArrayFloat] | tuple[NDArrayFloat, dict[tuple, NDArrayFloat]]):
+                Returns the wind speed array and the power array, or the wind speed array and a
+                dictionary of the multidimensional parameters and their associated power arrays.
         """
         shape = (1, wind_speeds.size, 1)
-        power_mw = power(
-            ref_density_cp_ct=np.full(shape, self.turbine.ref_density_cp_ct),
-            rotor_effective_velocities=wind_speeds.reshape(shape),
-            power_interp={self.turbine.turbine_type: self.turbine.power_interp},
-            turbine_type_map=np.full(shape, self.turbine.turbine_type)
-        ).flatten() / 1e6
+        if self.turbine.multi_dimensional_cp_ct:
+            power_interps = {
+                k: multidim_power_down_select(
+                    np.full(shape, self.turbine.power_interp),
+                    dict(zip(self.turbine.condition_keys, k)),
+                )
+                for k in self.turbine.power_interp
+            }
+            power_mw = {
+                k: power_multidim(
+                    ref_density_cp_ct=np.full(shape, self.turbine.ref_density_cp_ct),
+                    rotor_effective_velocities=wind_speeds.reshape(shape),
+                    power_interp=power_interps[k],
+                ).flatten() / 1e6
+                for k in self.turbine.power_interp
+            }
+        else:
+            power_mw = power(
+                ref_density_cp_ct=np.full(shape, self.turbine.ref_density_cp_ct),
+                rotor_effective_velocities=wind_speeds.reshape(shape),
+                power_interp={self.turbine.turbine_type: self.turbine.power_interp},
+                turbine_type_map=np.full(shape, self.turbine.turbine_type)
+            ).flatten() / 1e6
         return wind_speeds, power_mw
 
-    def Cp_curve(
-        self,
-        wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-    ) -> tuple[NDArrayFloat, NDArrayFloat]:
-        """Produces a plot-ready thrust curve for the turbine for wind speed vs power coefficient
-        assuming no tilt or yaw effects.
-
-        Args:
-        wind_speeds : NDArrayFloat, optional
-            The wind speed conditions to produce the power curve for, by default 0 m/s -> 40 m/s,
-            every 0.5 m/s.
-
-        Returns:
-            tuple[NDArrayFloat, NDArrayFloat]
-                Returns the wind speed array and the power coefficient array.
-        """
-        cp_curve = self.turbine.fCp_interp(wind_speeds)
-        return wind_speeds, cp_curve
-
     def Ct_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
     ) -> tuple[NDArrayFloat, NDArrayFloat]:
         """Produces a plot-ready thrust curve for the turbine for wind speed vs thrust coefficient
         assuming no tilt or yaw effects.
 
@@ -134,173 +166,178 @@
                 0 m/s -> 40 m/s, every 0.5 m/s.
 
         Returns:
             tuple[NDArrayFloat, NDArrayFloat]
                 Returns the wind speed array and the thrust coefficient array.
         """
         shape = (1, wind_speeds.size, 1)
-        ct_curve = Ct(
-            velocities=wind_speeds.reshape(shape),
-            yaw_angle=np.zeros(shape),
-            tilt_angle=np.full(shape, self.turbine.ref_tilt_cp_ct),
-            ref_tilt_cp_ct=np.full(shape, self.turbine.ref_tilt_cp_ct),
-            fCt={self.turbine.turbine_type: self.turbine.fCt_interp},
-            tilt_interp=[(self.turbine.turbine_type, self.turbine.fTilt_interp)],
-            correct_cp_ct_for_tilt=np.zeros(shape, dtype=bool),
-            turbine_type_map=np.full(shape, self.turbine.turbine_type),
-        ).flatten()
+        shape_single = (1, 1, 1)
+        if self.turbine.multi_dimensional_cp_ct:
+            fCt_interps = {
+                k: multidim_Ct_down_select(
+                    np.full(shape, self.turbine.fCt_interp),
+                    dict(zip(self.turbine.condition_keys, k)),
+                )
+                for k in self.turbine.fCt_interp
+            }
+            ct_curve = {
+                k: Ct_multidim(
+                    velocities=wind_speeds.reshape(shape),
+                    yaw_angle=np.zeros(shape),
+                    tilt_angle=np.full(shape, self.turbine.ref_tilt_cp_ct),
+                    ref_tilt_cp_ct=np.full(shape_single, self.turbine.ref_tilt_cp_ct),
+                    fCt=fCt_interps[k],
+                    tilt_interp={self.turbine.turbine_type: self.turbine.tilt_interp},
+                    correct_cp_ct_for_tilt=np.zeros(shape_single, dtype=bool),
+                    turbine_type_map=np.full(shape_single, self.turbine.turbine_type)
+                ).flatten()
+                for k in self.turbine.fCt_interp
+            }
+        else:
+            ct_curve = Ct(
+                velocities=wind_speeds.reshape(shape),
+                yaw_angle=np.zeros(shape),
+                tilt_angle=np.full(shape, self.turbine.ref_tilt_cp_ct),
+                ref_tilt_cp_ct=np.full(shape, self.turbine.ref_tilt_cp_ct),
+                fCt={self.turbine.turbine_type: self.turbine.fCt_interp},
+                tilt_interp={self.turbine.turbine_type: self.turbine.tilt_interp},
+                correct_cp_ct_for_tilt=np.zeros(shape, dtype=bool),
+                turbine_type_map=np.full(shape, self.turbine.turbine_type),
+            ).flatten()
         return wind_speeds, ct_curve
 
     def plot_power_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        plot_kwargs: dict | None =  None,
+        legend_kwargs: dict | None =  None,
         return_fig: bool = False
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots the power curve for a given set of wind speeds.
 
         Args:
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s.
                 Defaults to 0 m/s -> 40 m/s, every 0.5 m/s.
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
+                Defaults to None.
             plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            legend_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.legend()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         wind_speeds, power_mw = self.power_curve(wind_speeds=wind_speeds)
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        plot_kwargs = {} if plot_kwargs is None else plot_kwargs
+        legend_kwargs = {} if legend_kwargs is None else legend_kwargs
+
         # Set the figure defaults if none are provided
         fig_kwargs.setdefault("dpi", 200)
         fig_kwargs.setdefault("figsize", (4, 3))
 
         fig = plt.figure(**fig_kwargs)
         ax = fig.add_subplot(111)
 
         min_windspeed = 0
         max_windspeed = max(wind_speeds)
         min_power = 0
-        max_power = max(power_mw)
-        ax.plot(wind_speeds, power_mw, label=self.turbine.turbine_type, **plot_kwargs)
+        max_power = 0
+        if isinstance(power_mw, dict):
+            for key, _power_mw in power_mw.items():
+                max_power = max(max_power, *_power_mw)
+                _cond = "; ".join((f"{c}: {k}" for c, k in zip(self.turbine.condition_keys, key)))
+                label = f"{self.turbine.turbine_type} - {_cond}"
+                ax.plot(wind_speeds, _power_mw, label=label, **plot_kwargs)
+        else:
+            max_power = max(power_mw)
+            ax.plot(wind_speeds, power_mw, label=self.turbine.turbine_type, **plot_kwargs)
 
         ax.grid()
         ax.set_axisbelow(True)
-        ax.legend()
+        ax.legend(**legend_kwargs)
 
         max_power = round_nearest_2_or_5(max_power)
         ax.set_xlim(min_windspeed, max_windspeed)
         ax.set_ylim(min_power, max_power)
 
         ax.set_xlabel("Wind Speed (m/s)")
         ax.set_ylabel("Power (MW)")
 
         if return_fig:
             return fig, ax
 
         fig.tight_layout()
 
-    def plot_Cp_curve(
-        self,
-        wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
-        return_fig: bool = False
-    ) -> None | tuple[plt.Figure, plt.Axes]:
-        """Plots the power coefficient curve for a given set of wind speeds.
-
-        Args:
-            wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
-                0 m/s -> 40 m/s, every 0.5 m/s.
-            fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
-            plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
-            return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
-                returned. Defaults to False.
-
-        Returns:
-            None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
-                a tuple of the Figure and Axes objects are returned.
-        """
-        wind_speeds, power_c = self.Cp_curve(wind_speeds=wind_speeds)
-
-        # Set the figure defaults if none are provided
-        fig_kwargs.setdefault("dpi", 200)
-        fig_kwargs.setdefault("figsize", (4, 3))
-
-        fig = plt.figure(**fig_kwargs)
-        ax = fig.add_subplot(111)
-
-        min_windspeed = 0
-        max_windspeed = max(wind_speeds)
-        ax.plot(wind_speeds, power_c, label=self.turbine.turbine_type, **plot_kwargs)
-
-        ax.grid()
-        ax.set_axisbelow(True)
-        ax.legend()
-
-        ax.set_xlim(min_windspeed, max_windspeed)
-        ax.set_ylim(0, round_nearest(max(power_c) * 100, base=10) / 100)
-
-        ax.set_xlabel("Wind Speed (m/s)")
-        ax.set_ylabel("Power Coefficient")
-
-        if return_fig:
-            return fig, ax
-
-        fig.tight_layout()
-
     def plot_Ct_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        plot_kwargs: dict | None =  None,
+        legend_kwargs: dict | None =  None,
         return_fig: bool = False
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots the thrust coefficient curve for a given set of wind speeds.
 
         Args:
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
+                Defaults to None.
             plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            legend_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.legend()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         wind_speeds, thrust = self.Ct_curve(wind_speeds=wind_speeds)
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        plot_kwargs = {} if plot_kwargs is None else plot_kwargs
+        legend_kwargs = {} if legend_kwargs is None else legend_kwargs
+
         # Set the figure defaults if none are provided
         fig_kwargs.setdefault("dpi", 200)
         fig_kwargs.setdefault("figsize", (4, 3))
 
         fig = plt.figure(**fig_kwargs)
         ax = fig.add_subplot(111)
 
         min_windspeed = 0
+        max_thrust = 0
         max_windspeed = max(wind_speeds)
-        ax.plot(wind_speeds, thrust, label=self.turbine.turbine_type, **plot_kwargs)
+        if isinstance(thrust, dict):
+            for key, _thrust in thrust.items():
+                max_thrust = max(max_thrust, *_thrust)
+                _cond = "; ".join((f"{c}: {k}" for c, k in zip(self.turbine.condition_keys, key)))
+                label = f"{self.turbine.turbine_type} - {_cond}"
+                ax.plot(wind_speeds, _thrust, label=label, **plot_kwargs)
+        else:
+            max_thrust = max(thrust)
+            ax.plot(wind_speeds, thrust, label=self.turbine.turbine_type, **plot_kwargs)
 
         ax.grid()
         ax.set_axisbelow(True)
-        ax.legend()
+        ax.legend(**legend_kwargs)
 
         ax.set_xlim(min_windspeed, max_windspeed)
-        ax.set_ylim(0, round_nearest(max(thrust) * 100, base=10) / 100)
+        ax.set_ylim(0, round_nearest(max_thrust * 100, base=10) / 100)
 
         ax.set_xlabel("Wind Speed (m/s)")
         ax.set_ylabel("Thrust Coefficient")
 
         if return_fig:
             return fig, ax
 
@@ -374,29 +411,14 @@
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
         """
         self.power_curves = {
             name: t.power_curve(wind_speeds) for name, t in self.turbine_map.items()
         }
 
-    def compute_Cp_curves(
-            self,
-            wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        ) -> None:
-        """Computes the power coefficient curves for each turbine in ``turbine_map`` and sets the
-        ``Ct_curves`` attribute.
-
-        Args:
-            wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
-                0 m/s -> 40 m/s, every 0.5 m/s.
-        """
-        self.Cp_curves = {
-            name: t.Cp_curve(wind_speeds) for name, t in self.turbine_map.items()
-        }
-
     def compute_Ct_curves(
             self,
             wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
         ) -> None:
         """Computes the thrust curves for each turbine in ``turbine_map`` and sets the
         ``Ct_curves`` attribute.
 
@@ -411,16 +433,17 @@
     def plot_power_curves(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
         exclude: list[str] = [],
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
+        fig_kwargs: dict | None = None,
+        plot_kwargs: dict | None = None,
+        legend_kwargs: dict | None = None,
         return_fig: bool = False,
         show: bool = False,
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots each power curve in ``turbine_map`` in a single plot.
 
         Args:
             fig (plt.figure, optional): A pre-made figure where the plot should exist.
@@ -428,31 +451,38 @@
             which (list[str], optional): A list of which turbine types/names to include. Defaults to
                 [].
             exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
                 to [].
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
+                Defaults to None.
             plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            legend_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.legend()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
             show (bool, optional): Indicator if the figure should be automatically displayed.
                 Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         if self.power_curves == {} or wind_speeds is not None:
             self.compute_power_curves(wind_speeds=wind_speeds)
 
         which = [*self.turbine_map] if which == [] else which
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        plot_kwargs = {} if plot_kwargs is None else plot_kwargs
+        legend_kwargs = {} if legend_kwargs is None else legend_kwargs
+
         # Set the figure defaults if none are provided
         if fig is None:
             fig_kwargs.setdefault("dpi", 200)
             fig_kwargs.setdefault("figsize", (4, 3))
 
             fig = plt.figure(**fig_kwargs)
         if ax is None:
@@ -461,120 +491,52 @@
         min_windspeed = 0
         max_windspeed = 0
         min_power = 0
         max_power = 0
         for name, (ws, p) in self.power_curves.items():
             if name in exclude or name not in which:
                 continue
-            max_power = max(p.max(), max_power)
-            max_windspeed = max(ws.max(), max_windspeed)
-            ax.plot(ws, p, label=name, **plot_kwargs)
+            if isinstance(p, dict):
+                max_windspeed = max(ws.max(), max_windspeed)
+                for k, _p in p.items():
+                    max_power = max(_p.max(), max_power)
+                    label = f"{name} - {k}"
+                    ax.plot(ws, _p, label=label, linestyle="--", **plot_kwargs)
+            else:
+                max_power = max(p.max(), max_power)
+                max_windspeed = max(ws.max(), max_windspeed)
+                ax.plot(ws, p, label=name, **plot_kwargs)
 
         ax.grid()
         ax.set_axisbelow(True)
-        ax.legend()
+        ax.legend(**legend_kwargs)
 
         max_power = round_nearest(max_power, base=5)
         ax.set_xlim(min_windspeed, max_windspeed)
         ax.set_ylim(min_power, max_power)
 
         ax.set_xlabel("Wind Speed (m/s)")
         ax.set_ylabel("Power (MW)")
 
         if return_fig:
             return fig, ax
 
         if show:
             fig.tight_layout()
 
-    def plot_Cp_curves(
-        self,
-        fig: plt.Figure | None = None,
-        ax: plt.Axes | None = None,
-        which: list[str] = [],
-        exclude: list[str] = [],
-        wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
-        return_fig: bool = False,
-        show: bool = False,
-    ) -> None | tuple[plt.Figure, plt.Axes]:
-        """Plots each power coefficient curve in ``turbine_map`` in a single plot.
-
-        Args:
-            fig (plt.figure, optional): A pre-made figure where the plot should exist.
-            ax (plt.Axes, optional): A pre-initialized axes object that should be used for the plot.
-            which (list[str], optional): A list of which turbine types/names to include. Defaults to
-                [].
-            exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
-                to [].
-            wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
-                0 m/s -> 40 m/s, every 0.5 m/s.
-            fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
-            plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
-            return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
-                returned. Defaults to False.
-            show (bool, optional): Indicator if the figure should be automatically displayed.
-                Defaults to False.
-
-        Returns:
-            None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
-                a tuple of the Figure and Axes objects are returned.
-        """
-        if self.Cp_curves == {} or wind_speeds is None:
-            self.compute_Cp_curves(wind_speeds=wind_speeds)
-
-        which = [*self.turbine_map] if which == [] else which
-
-        # Set the figure defaults if none are provided
-        if fig is None:
-            fig_kwargs.setdefault("dpi", 200)
-            fig_kwargs.setdefault("figsize", (4, 3))
-
-            fig = plt.figure(**fig_kwargs)
-        if ax is None:
-            ax = fig.add_subplot(111)
-
-        min_windspeed = 0
-        max_windspeed = 0
-        max_power = 0
-        for name, (ws, p) in self.Cp_curves.items():
-            if name in exclude or name not in which:
-                continue
-            max_windspeed = max(ws.max(), max_windspeed)
-            max_power = max(p.max(), max_power)
-            ax.plot(ws, p, label=name, **plot_kwargs)
-
-        ax.grid()
-        ax.set_axisbelow(True)
-        ax.legend()
-
-        ax.set_xlim(min_windspeed, max_windspeed)
-        ax.set_ylim(0, round_nearest(max_power * 100, base=10) / 100)
-
-        ax.set_xlabel("Wind Speed (m/s)")
-        ax.set_ylabel("Power Coefficient")
-
-        if return_fig:
-            return fig, ax
-
-        if show:
-            fig.tight_layout()
-
     def plot_Ct_curves(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
         exclude: list[str] = [],
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        plot_kwargs: dict | None =  None,
+        legend_kwargs: dict | None =  None,
         return_fig: bool = False,
         show: bool = False,
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots each thrust coefficient curve in ``turbine_map`` in a single plot.
 
         Args:
             fig (plt.figure, optional): A pre-made figure where the plot should exist.
@@ -582,31 +544,39 @@
             which (list[str], optional): A list of which turbine types/names to include. Defaults to
                 [].
             exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
                 to [].
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
+                Defaults to None.
             plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.legend()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
             show (bool, optional): Indicator if the figure should be automatically displayed.
                 Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         if self.Ct_curves == {} or wind_speeds is None:
             self.compute_Ct_curves(wind_speeds=wind_speeds)
 
         which = [*self.turbine_map] if which == [] else which
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        plot_kwargs = {} if plot_kwargs is None else plot_kwargs
+        legend_kwargs = {} if legend_kwargs is None else legend_kwargs
+
+
         # Set the figure defaults if none are provided
         if fig is None:
             fig_kwargs.setdefault("dpi", 200)
             fig_kwargs.setdefault("figsize", (4, 3))
 
             fig = plt.figure(**fig_kwargs)
         if ax is None:
@@ -614,21 +584,28 @@
 
         min_windspeed = 0
         max_windspeed = 0
         max_thrust = 0
         for name, (ws, t) in self.Ct_curves.items():
             if name in exclude or name not in which:
                 continue
-            max_windspeed = max(ws.max(), max_windspeed)
-            max_thrust = max(t.max(), max_thrust)
-            ax.plot(ws, t, label=name, **plot_kwargs)
+            if isinstance(t, dict):
+                max_windspeed = max(ws.max(), max_windspeed)
+                for k, _t in t.items():
+                    max_thrust = max(_t.max(), max_thrust)
+                    label = f"{name} - {k}"
+                    ax.plot(ws, _t, label=label, linestyle="--", **plot_kwargs)
+            else:
+                max_windspeed = max(ws.max(), max_windspeed)
+                max_thrust = max(t.max(), max_thrust)
+                ax.plot(ws, t, label=name, **plot_kwargs)
 
         ax.grid()
         ax.set_axisbelow(True)
-        ax.legend()
+        ax.legend(**legend_kwargs)
 
         ax.set_xlim(min_windspeed, max_windspeed)
         ax.set_ylim(0, round_nearest(max_thrust * 100, base=10) / 100)
 
         ax.set_xlabel("Wind Speed (m/s)")
         ax.set_ylabel("Thrust Coefficient")
 
@@ -640,43 +617,47 @@
 
     def plot_rotor_diameters(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
         exclude: list[str] = [],
-        fig_kwargs: dict = {},
-        bar_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        bar_kwargs: dict | None =  None,
         return_fig: bool = False,
         show: bool = False,
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots a bar chart of rotor diameters for each turbine in ``turbine_map``.
 
         Args:
             fig (plt.figure, optional): A pre-made figure where the plot should exist.
             ax (plt.Axes, optional): A pre-initialized axes object that should be used for the plot.
             which (list[str], optional): A list of which turbine types/names to include. Defaults to
                 [].
             exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
                 to [].
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
-            bar_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            bar_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.bar()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
             show (bool, optional): Indicator if the figure should be automatically displayed.
                 Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         which = [*self.turbine_map] if which == [] else which
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        bar_kwargs = {} if bar_kwargs is None else bar_kwargs
+
         # Set the figure defaults if none are provided
         if fig is None:
             fig_kwargs.setdefault("dpi", 200)
             fig_kwargs.setdefault("figsize", (4, 3))
 
             fig = plt.figure(**fig_kwargs)
         if ax is None:
@@ -695,58 +676,62 @@
         ax.grid(axis="y")
         ax.set_axisbelow(True)
 
         ax.set_xlim(-0.5, len(x) - 0.5)
         ax.set_ylim(0, round_nearest(max(y) / 10, base=5) * 10)
 
         ax.set_xticks(x)
-        ax.set_xticklabels(np.array([*subset_map])[ix_sort])
+        ax.set_xticklabels(np.array([*subset_map])[ix_sort], rotation=30, ha="right")
         ax.set_ylabel("Rotor Diameter (m)")
 
         if return_fig:
             return fig, ax
 
         if show:
             fig.tight_layout()
 
     def plot_hub_heights(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
         exclude: list[str] = [],
-        fig_kwargs: dict = {},
-        bar_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        bar_kwargs: dict | None =  None,
         return_fig: bool = False,
         show: bool = False,
     ) -> None | tuple[plt.Figure, plt.Axes]:
         """Plots a bar chart of hub heights for each turbine in ``turbine_map``.
 
         Args:
             fig (plt.figure, optional): A pre-made figure where the plot should exist.
             ax (plt.Axes, optional): A pre-initialized axes object that should be used for the plot.
             which (list[str], optional): A list of which turbine types/names to include. Defaults to
                 [].
             exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
                 to [].
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
-            bar_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
+            bar_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.bar()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
             show (bool, optional): Indicator if the figure should be automatically displayed.
                 Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
         which = [*self.turbine_map] if which == [] else which
 
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        bar_kwargs = {} if bar_kwargs is None else bar_kwargs
+
         # Set the figure defaults if none are provided
         if fig is None:
             fig_kwargs.setdefault("dpi", 200)
             fig_kwargs.setdefault("figsize", (4, 3))
 
             fig = plt.figure(**fig_kwargs)
         if ax is None:
@@ -765,99 +750,100 @@
         ax.grid(axis="y")
         ax.set_axisbelow(True)
 
         ax.set_xlim(-0.5, len(x) - 0.5)
         ax.set_ylim(0, round_nearest(max(y) / 10, base=5) * 10)
 
         ax.set_xticks(x)
-        ax.set_xticklabels(np.array([*subset_map])[ix_sort])
+        ax.set_xticklabels(np.array([*subset_map])[ix_sort], rotation=30, ha="right")
         ax.set_ylabel("Hub Height (m)")
 
         if return_fig:
             return fig, ax
 
         if show:
             fig.tight_layout()
 
     def plot_comparison(
         self,
         which: list[str] = [],
         exclude: list[str] = [],
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
-        fig_kwargs: dict = {},
-        plot_kwargs = {},
-        bar_kwargs = {},
+        fig_kwargs: dict | None =  None,
+        plot_kwargs: dict | None =  None,
+        bar_kwargs: dict | None =  None,
+        legend_kwargs: dict | None =  None,
         return_fig: bool = False
     ) -> None | tuple[plt.Figure, list[plt.Axes]]:
         """Plots each thrust curve in ``turbine_map`` in a single plot.
 
         Args:
             which (list[str], optional): A list of which turbine types/names to include. Defaults to
                 [].
             exclude (list[str], optional): A list of turbine types/names names to exclude. Defaults
                 to [].
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
             fig_kwargs (dict, optional): Any keywords arguments to be passed to ``plt.Figure()``.
-                Defaults to {}.
+                Defaults to None.
             plot_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.plot()``.
-                Defaults to {}.
+                Defaults to None.
             bar_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.bar()``.
-                Defaults to {}.
+                Defaults to None.
+            legend_kwargs (dict, optional): Any keyword arguments to be passed to ``plt.legend()``.
+                Defaults to None.
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, list[plt.Axes]]: None, if :py:attr:`return_fig` is False,
                 otherwise a tuple of the Figure and Axes objects are returned.
         """
+        # Initialize kwargs if None
+        fig_kwargs = {} if fig_kwargs is None else fig_kwargs
+        plot_kwargs = {} if plot_kwargs is None else plot_kwargs
+        bar_kwargs = {} if bar_kwargs is None else bar_kwargs
+        legend_kwargs = {} if legend_kwargs is None else legend_kwargs
+
         # Set the figure defaults if none are provided
         fig_kwargs.setdefault("dpi", 200)
         fig_kwargs.setdefault("figsize", (6, 5))
+        legend_kwargs.setdefault("fontsize", 6)
 
         fig = plt.figure(**fig_kwargs)
         ax1 = fig.add_subplot(321)
         ax2 = fig.add_subplot(322)
         ax3 = fig.add_subplot(323)
         ax4 = fig.add_subplot(324)
-        ax5 = fig.add_subplot(325)
-        ax_list = [ax1, ax2, ax3, ax4, ax5]
+        ax_list = [ax1, ax2, ax3, ax4]
 
         self.plot_power_curves(
             fig,
             ax1,
             which=which,
             exclude=exclude,
             wind_speeds=wind_speeds,
             plot_kwargs=plot_kwargs,
         )
-        self.plot_Cp_curves(
-            fig,
-            ax3,
-            which=which,
-            exclude=exclude,
-            wind_speeds=wind_speeds,
-            plot_kwargs=plot_kwargs,
-        )
         self.plot_Ct_curves(
             fig,
-            ax5,
+            ax3,
             which=which,
             exclude=exclude,
             wind_speeds=wind_speeds,
             plot_kwargs=plot_kwargs,
         )
         self.plot_rotor_diameters(fig, ax2, which=which, exclude=exclude, bar_kwargs=bar_kwargs)
         self.plot_hub_heights(fig, ax4, which=which, bar_kwargs=bar_kwargs)
 
         for ax in ax_list:
             ax.tick_params(axis='both', which='major', labelsize=7)
             ax.xaxis.label.set_size(7)
             ax.yaxis.label.set_size(8)
 
-        for ax in (ax1, ax3, ax5):
-            ax.legend(fontsize=6)
+        for ax in (ax1, ax3):
+            ax.legend(**legend_kwargs)
 
         if return_fig:
             return fig, ax_list
 
         fig.tight_layout()
```

### Comparing `FLORIS-3.5/floris/turbine_library/x_20MW.yaml` & `FLORIS-3.6/floris/turbine_library/x_20MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/floris/type_dec.py` & `FLORIS-3.6/floris/type_dec.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import copy
+import inspect
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Iterable,
     Tuple,
     Union,
@@ -46,14 +47,32 @@
 def floris_array_converter(data: Iterable) -> np.ndarray:
     try:
         a = np.array(data, dtype=floris_float_type)
     except TypeError as e:
         raise TypeError(e.args[0] + f". Data given: {data}")
     return a
 
+def floris_numeric_dict_converter(data: dict) -> dict:
+    try:
+        return {k: floris_array_converter(v) for k, v in data.items()}
+    except TypeError as e:
+        raise TypeError(e.args[0] + f". Data given: {data}")
+
+# def array_field(**kwargs) -> Callable:
+#     """
+#     A wrapper for the :py:func:`attr.field` function that converts the input to a Numpy array,
+#     adds a comparison function specific to Numpy arrays, and passes through all additional
+#     keyword arguments.
+#     """
+#     return field(
+#         converter=floris_array_converter,
+#         eq=cmp_using(eq=np.array_equal),
+#         **kwargs
+#     )
+
 def _attr_serializer(inst: type, field: Attribute, value: Any):
     if isinstance(value, np.ndarray):
         return value.tolist()
     return value
 
 def _attr_floris_filter(inst: Attribute, value: Any) -> bool:
     if inst.init is False:
@@ -62,56 +81,77 @@
         return False
     if isinstance(value, np.ndarray):
         if value.size == 0:
             return False
     return True
 
 def iter_validator(iter_type, item_types: Union[Any, Tuple[Any]]) -> Callable:
-    """Helper function to generate iterable validators that will reduce the amount of
+    """
+    Helper function to generate iterable validators that will reduce the amount of
     boilerplate code.
 
-    Parameters
-    ----------
-    iter_type : any iterable
-        The type of iterable object that should be validated.
-    item_types : Union[Any, Tuple[Any]]
-        The type or types of acceptable item types.
-
-    Returns
-    -------
-    Callable
-        The attr.validators.deep_iterable iterable and instance validator.
+    Args:
+        iter_type (iterable): The type of iterable object that should be validated.
+        item_types (Union[Any, Tuple[Any]]): The type or types of acceptable item types.
+
+    Returns:
+        Callable: The attr.validators.deep_iterable iterable and instance validator.
     """
     validator = attrs.validators.deep_iterable(
         member_validator=attrs.validators.instance_of(item_types),
         iterable_validator=attrs.validators.instance_of(iter_type),
     )
     return validator
 
 def convert_to_path(fn: str | Path) -> Path:
-    """Converts an input string or pathlib.Path object to a fully resolved ``pathlib.Path``
-    object.
+    """
+    Converts an input string or ``pathlib.Path`` object to a fully resolved ``pathlib.Path``
+    object. If the input is a string, it is converted to a pathlib.Path object.
+    The function then checks if the path exists as an absolute path, a relative path from
+    the script, or a relative path from the system location. If the path does not exist in
+    any of these locations, a FileExistsError is raised.
 
     Args:
         fn (str | Path): The user input file path or file name.
 
     Raises:
+        FileExistsError: Raised if :py:attr:`fn` is not able to be found as an absolute path, nor as
+            a relative path.
         TypeError: Raised if :py:attr:`fn` is neither a :py:obj:`str`, nor a :py:obj:`pathlib.Path`.
 
     Returns:
         Path: A resolved pathlib.Path object.
     """
     if isinstance(fn, str):
         fn = Path(fn)
 
+    # Get the base path from where the analysis script was run to determine the relative
+    # path from which `fn` might be based. [1] is where a direct call to this function will be
+    # located (e.g., testing via pytest), and [-1] is where a direct call to the function via an
+    # analysis script will be located (e.g., running an example).
+    base_fn_script = Path(inspect.stack()[-1].filename).resolve().parent
+    base_fn_sys = Path(inspect.stack()[1].filename).resolve().parent
+
     if isinstance(fn, Path):
-        fn.resolve()
-    else:
-        raise TypeError(f"The passed input: {fn} could not be converted to a pathlib.Path object")
-    return fn
+        absolute_fn = fn.resolve()
+        relative_fn_script = (base_fn_script / fn).resolve()
+        relative_fn_sys = (base_fn_sys / fn).resolve()
+        if absolute_fn.exists():
+            return absolute_fn
+        if relative_fn_script.exists():
+            return relative_fn_script
+        if relative_fn_sys.exists():
+            return relative_fn_sys
+        raise FileExistsError(
+            f"{fn} could not be found as either a\n"
+            f"  - relative file path from a script: {relative_fn_script}\n"
+            f"  - relative file path from a system location: {relative_fn_sys}\n"
+            f"  - or absolute file path: {absolute_fn}"
+        )
+    raise TypeError(f"The passed input: {fn} could not be converted to a pathlib.Path object")
 
 
 @define
 class FromDictMixin:
     """
     A Mixin class to allow for kwargs overloading when a data class doesn't
     have a specific parameter defined. This allows passing of larger dictionaries
```

### Comparing `FLORIS-3.5/floris/utilities.py` & `FLORIS-3.6/floris/utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,109 +25,14 @@
 from floris.type_dec import floris_array_converter, NDArrayFloat
 
 
 def pshape(array: np.ndarray, label: str = ""):
     print(label, np.shape(array))
 
 
-@define
-class Vec3:
-    """
-    Contains 3-component vector information. All arithmetic operators are
-    set so that Vec3 objects can operate on and with each other directly.
-
-    Args:
-        components (list(numeric, numeric, numeric), numeric): All three vector
-            components.
-        string_format (str, optional): Format to use in the
-            overloaded __str__ function. Defaults to None.
-    """
-    components: NDArrayFloat = field(converter=floris_array_converter)
-    # NOTE: this does not convert elements to float if they are given as int. Is this ok?
-
-    @components.validator
-    def _check_components(self, attribute, value) -> None:
-        if np.ndim(value) > 1:
-            raise ValueError(
-                f"Vec3 must contain exactly 1 dimension, {np.ndim(value)} were given."
-            )
-        if np.size(value) != 3:
-            raise ValueError(
-                f"Vec3 must contain exactly 3 components, {np.size(value)} were given."
-            )
-
-    def __add__(self, arg):
-        if type(arg) is Vec3:
-            return Vec3(self.components + arg.components)
-        elif type(arg) is int or type(arg) is float:
-            return Vec3(self.components + arg)
-        else:
-            raise ValueError
-
-    def __sub__(self, arg):
-        if type(arg) is Vec3:
-            return Vec3(self.components - arg.components)
-        elif type(arg) is int or type(arg) is float:
-            return Vec3(self.components - arg)
-        else:
-            raise ValueError
-
-    def __mul__(self, arg):
-        if type(arg) is Vec3:
-            return Vec3(self.components * arg.components)
-        elif type(arg) is int or type(arg) is float:
-            return Vec3(self.components * arg)
-        else:
-            raise ValueError
-
-    def __truediv__(self, arg):
-        if type(arg) is Vec3:
-            return Vec3(self.components / arg.components)
-        elif type(arg) is int or type(arg) is float:
-            return Vec3(self.components / arg)
-        else:
-            raise ValueError
-
-    def __eq__(self, arg):
-        return False not in np.isclose([self.x1, self.x2, self.x3], [arg.x1, arg.x2, arg.x3])
-
-    def __hash__(self):
-        return hash((self.x1, self.x2, self.x3))
-
-    @property
-    def x1(self):
-        return self.components[0]
-
-    @x1.setter
-    def x1(self, value):
-        self.components[0] = float(value)
-
-    @property
-    def x2(self):
-        return self.components[1]
-
-    @x2.setter
-    def x2(self, value):
-        self.components[1] = float(value)
-
-    @property
-    def x3(self):
-        return self.components[2]
-
-    @x3.setter
-    def x3(self, value):
-        self.components[2] = float(value)
-
-    @property
-    def elements(self) -> Tuple[float, float, float]:
-        # TODO: replace references to elements with components
-        # and remove this @property
-        return self.components
-
-
 def cosd(angle):
     """
     Cosine of an angle with the angle given in degrees.
 
     Args:
         angle (float): Angle in degrees.
 
@@ -299,17 +204,17 @@
     wind_deviation_from_west = -1.0 * wind_delta(wind_directions)
 
     # Construct the arrays storing the turbine locations
     grid_x_reversed = np.zeros_like(grid_x)
     grid_y_reversed = np.zeros_like(grid_x)
     grid_z_reversed = np.zeros_like(grid_x)
     for wii, angle_rotation in enumerate(wind_deviation_from_west):
-        x_rot = grid_x[wii, :, :, :, :]
-        y_rot = grid_y[wii, :, :, :, :]
-        z_rot = grid_z[wii, :, :, :, :]
+        x_rot = grid_x[wii]
+        y_rot = grid_y[wii]
+        z_rot = grid_z[wii]
 
         # Rotate turbine coordinates about the center
         x_rot_offset = x_rot - x_center_of_rotation
         y_rot_offset = y_rot - y_center_of_rotation
         x = (
             x_rot_offset * cosd(angle_rotation)
             - y_rot_offset * sind(angle_rotation)
@@ -318,17 +223,17 @@
         y = (
             x_rot_offset * sind(angle_rotation)
             + y_rot_offset * cosd(angle_rotation)
             + y_center_of_rotation
         )
         z = z_rot  # Nothing changed in this rotation
 
-        grid_x_reversed[wii, :, :, :, :] = x
-        grid_y_reversed[wii, :, :, :, :] = y
-        grid_z_reversed[wii, :, :, :, :] = z
+        grid_x_reversed[wii] = x
+        grid_y_reversed[wii] = y
+        grid_z_reversed[wii] = z
 
     return grid_x_reversed, grid_y_reversed, grid_z_reversed
 
 
 class Loader(yaml.SafeLoader):
 
     def __init__(self, stream):
```

### Comparing `FLORIS-3.5/pyproject.toml` & `FLORIS-3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.5/setup.py` & `FLORIS-3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,37 +26,37 @@
 AUTHOR = "NREL National Wind Technology Center"
 REQUIRES_PYTHON = ">=3.8.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # simulation
     "attrs",
-    "pyyaml",
-    "numexpr",
-    "numpy>=1.20",
-    "scipy>=1.1",
+    "pyyaml~=6.0",
+    "numexpr~=2.0",
+    "numpy~=1.20",
+    "scipy~=1.1",
 
     # tools
-    "matplotlib>=3",
-    "pandas",
-    "shapely",
+    "matplotlib~=3.0",
+    "pandas~=2.0",
+    "shapely~=2.0",
 
     # utilities
-    "coloredlogs>=10.0",
-    "flatten_dict",
+    "coloredlogs~=10.0",
+    "flatten_dict~=0.0",
 ]
 
 # What packages are optional?
 # To use:
 #   pip install -e ".[docs,develop]"    install both sets of extras in editable install
 #   pip install -e ".[develop]"         installs only developer packages in editable install
 #   pip install "floris[develop]"       installs developer packages in non-editable install
 EXTRAS = {
     "docs": {
-        "jupyter-book<=0.13.3",
+        "jupyter-book",
         "sphinx-book-theme",
         "sphinx-autodoc-typehints",
         "sphinxcontrib-autoyaml",
         "sphinxcontrib.mermaid",
     },
     "develop": {
         "pytest",
```

