# Comparing `tmp/matflow_new-0.3.0a98.tar.gz` & `tmp/matflow_new-0.3.0a99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matflow_new-0.3.0a98.tar", max compression
+gzip compressed data, was "matflow_new-0.3.0a99.tar", max compression
```

## Comparing `matflow_new-0.3.0a98.tar` & `matflow_new-0.3.0a99.tar`

### file list

```diff
@@ -1,66 +1,70 @@
--rw-r--r--   0        0        0    41541 2023-11-20 23:26:44.613112 matflow_new-0.3.0a98/README.md
--rw-r--r--   0        0        0     1646 2023-11-20 23:26:44.617112 matflow_new-0.3.0a98/matflow/__init__.py
--rw-r--r--   0        0        0       98 2023-11-20 23:26:44.617112 matflow_new-0.3.0a98/matflow/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      636 2023-11-20 23:26:44.617112 matflow_new-0.3.0a98/matflow/__pyinstaller/hook-matflow.py
--rw-r--r--   0        0        0       25 2023-11-20 23:26:44.617112 matflow_new-0.3.0a98/matflow/_version.py
--rw-r--r--   0        0        0       62 2023-11-20 23:26:44.617112 matflow_new-0.3.0a98/matflow/cli.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/demo_data_manifest/__init__.py
--rw-r--r--   0        0        0      381 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/demo_data_manifest/demo_data_manifest.json
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/__init__.py
--rw-r--r--   0        0        0      617 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/dump_all_yield_stresses.py
--rw-r--r--   0        0        0      276 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/extract_damask_HDF5.py
--rw-r--r--   0        0        0     2505 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/generate_volume_element_voronoi.py
--rw-r--r--   0        0        0      281 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/process_damask_HDF5.py
--rw-r--r--   0        0        0      318 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/read_log.py
--rw-r--r--   0        0        0      940 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/seeds_from_random.py
--rw-r--r--   0        0        0      310 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/viz_damask_HDF5.py
--rw-r--r--   0        0        0      295 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/write_geom.py
--rw-r--r--   0        0        0      573 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/write_load.py
--rw-r--r--   0        0        0      935 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/damask/write_material.py
--rw-r--r--   0        0        0       35 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/demo_script_action.py
--rw-r--r--   0        0        0      146 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/dump_group_data.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/formable/__init__.py
--rw-r--r--   0        0        0     4708 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/formable/fit_single_crystal_parameters.py
--rw-r--r--   0        0        0     3507 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/formable/fit_yield_function.py
--rw-r--r--   0        0        0     1416 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/formable/read_tensile_test_CSV.py
--rw-r--r--   0        0        0      802 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/main_script_test.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/mtex/__init__.py
--rw-r--r--   0        0        0     3919 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/mtex/plot_pole_figures.m
--rw-r--r--   0        0        0     3051 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_CTF.m
--rw-r--r--   0        0        0     1867 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_ODF_mat.m
--rw-r--r--   0        0        0     5579 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_model_ODF.m
--rw-r--r--   0        0        0      120 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/read_my_file.py
--rw-r--r--   0        0        0       53 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/read_t1_outfile_1.py
--rw-r--r--   0        0        0      120 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/write_my_file.py
--rw-r--r--   0        0        0       49 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/scripts/write_t1_infile_1.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/template_components/__init__.py
--rw-r--r--   0        0        0      958 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/template_components/command_files.yaml
--rw-r--r--   0        0        0      288 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/template_components/environments.yaml
--rw-r--r--   0        0        0     3303 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/template_components/parameters.yaml
--rw-r--r--   0        0        0    23375 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/template_components/task_schemas.yaml
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/__init__.py
--rw-r--r--   0        0        0     1751 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/damask_input_files.yaml
--rw-r--r--   0        0        0     2779 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/fit_single_crystal_parameters.yaml
--rw-r--r--   0        0        0     2739 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/fit_yield_funcs.yaml
--rw-r--r--   0        0        0      345 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/read_tensile_test_CSV.yaml
--rw-r--r--   0        0        0      702 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_CTF_file.yaml
--rw-r--r--   0        0        0      573 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_ODF_mat.yaml
--rw-r--r--   0        0        0     1148 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_model_ODF.yaml
--rw-r--r--   0        0        0     3083 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/simulate_yield_surface_2D_brass.yaml
--rw-r--r--   0        0        0     2663 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/tension_DAMASK_Al.yaml
--rw-r--r--   0        0        0     4451 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/data/workflows/tension_DAMASK_Mg.yaml
--rw-r--r--   0        0        0      627 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/__init__.py
--rw-r--r--   0        0        0    33956 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/load.py
--rw-r--r--   0        0        0     7992 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/orientations.py
--rw-r--r--   0        0        0     2978 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/seeds.py
--rw-r--r--   0        0        0     1793 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/single_crystal_parameters.py
--rw-r--r--   0        0        0      762 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/param_classes/utils.py
--rw-r--r--   0        0        0        0 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/__init__.py
--rw-r--r--   0        0        0     1423 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/conftest.py
--rw-r--r--   0        0        0      349 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/param_classes/test_load.py
--rw-r--r--   0        0        0      929 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/param_classes/test_single_crystal_parameters.py
--rw-r--r--   0        0        0      500 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/test_cli.py
--rw-r--r--   0        0        0     1193 2023-11-20 23:26:44.693112 matflow_new-0.3.0a98/matflow/tests/test_utils.py
--rw-r--r--   0        0        0     1511 2023-11-20 23:26:44.697112 matflow_new-0.3.0a98/pyproject.toml
--rw-r--r--   0        0        0    42266 1970-01-01 00:00:00.000000 matflow_new-0.3.0a98/PKG-INFO
+-rw-r--r--   0        0        0    41543 2023-11-21 20:10:42.040203 matflow_new-0.3.0a99/README.md
+-rw-r--r--   0        0        0     1646 2023-11-21 20:10:42.044203 matflow_new-0.3.0a99/matflow/__init__.py
+-rw-r--r--   0        0        0       98 2023-11-21 20:10:42.044203 matflow_new-0.3.0a99/matflow/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      636 2023-11-21 20:10:42.044203 matflow_new-0.3.0a99/matflow/__pyinstaller/hook-matflow.py
+-rw-r--r--   0        0        0       25 2023-11-21 20:10:42.044203 matflow_new-0.3.0a99/matflow/_version.py
+-rw-r--r--   0        0        0       62 2023-11-21 20:10:42.044203 matflow_new-0.3.0a99/matflow/cli.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/demo_data_manifest/__init__.py
+-rw-r--r--   0        0        0      381 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/demo_data_manifest/demo_data_manifest.json
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/__init__.py
+-rw-r--r--   0        0        0      617 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/dump_all_yield_stresses.py
+-rw-r--r--   0        0        0      276 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/extract_damask_HDF5.py
+-rw-r--r--   0        0        0     2505 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/generate_volume_element_voronoi.py
+-rw-r--r--   0        0        0      281 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/process_damask_HDF5.py
+-rw-r--r--   0        0        0      318 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/read_log.py
+-rw-r--r--   0        0        0      940 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/seeds_from_random.py
+-rw-r--r--   0        0        0      310 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/viz_damask_HDF5.py
+-rw-r--r--   0        0        0      295 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/write_geom.py
+-rw-r--r--   0        0        0      573 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/write_load.py
+-rw-r--r--   0        0        0      935 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/damask/write_material.py
+-rw-r--r--   0        0        0       35 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/demo_script_action.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/dream_3D/__init__.py
+-rw-r--r--   0        0        0    46145 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/dream_3D/generate_volume_element_statistics.py
+-rw-r--r--   0        0        0     1741 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/dream_3D/parse_dream_3D_volume_element.py
+-rw-r--r--   0        0        0      146 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/dump_group_data.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/formable/__init__.py
+-rw-r--r--   0        0        0     4708 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/formable/fit_single_crystal_parameters.py
+-rw-r--r--   0        0        0     3507 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/formable/fit_yield_function.py
+-rw-r--r--   0        0        0     1416 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/formable/read_tensile_test_CSV.py
+-rw-r--r--   0        0        0      802 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/main_script_test.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/mtex/__init__.py
+-rw-r--r--   0        0        0     3919 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/mtex/plot_pole_figures.m
+-rw-r--r--   0        0        0     3051 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_CTF.m
+-rw-r--r--   0        0        0     1867 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_ODF_mat.m
+-rw-r--r--   0        0        0     5579 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_model_ODF.m
+-rw-r--r--   0        0        0      120 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/read_my_file.py
+-rw-r--r--   0        0        0       53 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/read_t1_outfile_1.py
+-rw-r--r--   0        0        0      120 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/write_my_file.py
+-rw-r--r--   0        0        0       49 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/scripts/write_t1_infile_1.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/template_components/__init__.py
+-rw-r--r--   0        0        0      749 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/template_components/command_files.yaml
+-rw-r--r--   0        0        0      310 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/template_components/environments.yaml
+-rw-r--r--   0        0        0     3303 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/template_components/parameters.yaml
+-rw-r--r--   0        0        0    24666 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/template_components/task_schemas.yaml
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/__init__.py
+-rw-r--r--   0        0        0     1751 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/damask_input_files.yaml
+-rw-r--r--   0        0        0     2779 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/fit_single_crystal_parameters.yaml
+-rw-r--r--   0        0        0     2739 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/fit_yield_funcs.yaml
+-rw-r--r--   0        0        0      755 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/generate_volume_element_from_statistics.yaml
+-rw-r--r--   0        0        0      345 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/read_tensile_test_CSV.yaml
+-rw-r--r--   0        0        0      702 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_CTF_file.yaml
+-rw-r--r--   0        0        0      573 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_ODF_mat.yaml
+-rw-r--r--   0        0        0     1148 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_model_ODF.yaml
+-rw-r--r--   0        0        0     3083 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/simulate_yield_surface_2D_brass.yaml
+-rw-r--r--   0        0        0     2663 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/tension_DAMASK_Al.yaml
+-rw-r--r--   0        0        0     4451 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/data/workflows/tension_DAMASK_Mg.yaml
+-rw-r--r--   0        0        0      627 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/__init__.py
+-rw-r--r--   0        0        0    33963 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/load.py
+-rw-r--r--   0        0        0     7992 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/orientations.py
+-rw-r--r--   0        0        0     2978 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/seeds.py
+-rw-r--r--   0        0        0     1793 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/single_crystal_parameters.py
+-rw-r--r--   0        0        0      762 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/param_classes/utils.py
+-rw-r--r--   0        0        0        0 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/__init__.py
+-rw-r--r--   0        0        0     1423 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/conftest.py
+-rw-r--r--   0        0        0      349 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/param_classes/test_load.py
+-rw-r--r--   0        0        0      929 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/param_classes/test_single_crystal_parameters.py
+-rw-r--r--   0        0        0      500 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/test_cli.py
+-rw-r--r--   0        0        0     1193 2023-11-21 20:10:42.124203 matflow_new-0.3.0a99/matflow/tests/test_utils.py
+-rw-r--r--   0        0        0     1511 2023-11-21 20:10:42.128203 matflow_new-0.3.0a99/pyproject.toml
+-rw-r--r--   0        0        0    42268 1970-01-01 00:00:00.000000 matflow_new-0.3.0a99/PKG-INFO
```

### Comparing `matflow_new-0.3.0a98/README.md` & `matflow_new-0.3.0a99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 | **generate_volume_element**                                                                                                                                                         |        |                                                                                                                                                                                                                                                                          |
 | ⇒ method: [single_voxel_grains/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L452)                      | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [particle_RVE/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L477)                             | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [dual_phase_ti_alpha_colony](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L486)                      | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [from_damask_input_files](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L495)                         | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [from_dream3d_pipeline](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L505)                           | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [extrusion](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L511)                                       | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
-| ⇒ method: [from_statistics/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L525)                         | ❌      | [PR pending](https://github.com/hpcflow/matflow-new/pull/179)                                                                                                                                                                                                            |
+| ⇒ method: [from_statistics/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L525)                         | ✅/❌    | `generate_volume_element/from_statistics` - Not yet tested with `orientations` input                                                                                                                                                                                     |
 | ⇒ method: [from_statistics_dual_phase_orientations/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L568) | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [random_voronoi/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L624)                           | ✅      | [generate_volume_element/from_voronoi](https://docs.matflow.io/stable/reference/template_components/task_schemas.html#generate-volume-element)                                                                                                                           |
 | ⇒ method: [random_voronoi/neper](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L647)                            | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [random_voronoi_from_orientations](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L686)                | ✅      | Use [generate_volume_element/from_voronoi](https://docs.matflow.io/stable/reference/template_components/task_schemas.html#generate-volume-element)                                                                                                                       |
 | ⇒ method: [random_voronoi_from_dual_phase_orientations](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L716)     | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | **modify_volume_element**                                                                                                                                                           |        |                                                                                                                                                                                                                                                                          |
 | ⇒ method: [add_buffer_zones/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L760)                         | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
```

### Comparing `matflow_new-0.3.0a98/matflow/__init__.py` & `matflow_new-0.3.0a99/matflow/__init__.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/__pyinstaller/hook-matflow.py` & `matflow_new-0.3.0a99/matflow/__pyinstaller/hook-matflow.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/damask/dump_all_yield_stresses.py` & `matflow_new-0.3.0a99/matflow/data/scripts/damask/dump_all_yield_stresses.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/damask/generate_volume_element_voronoi.py` & `matflow_new-0.3.0a99/matflow/data/scripts/damask/generate_volume_element_voronoi.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/damask/seeds_from_random.py` & `matflow_new-0.3.0a99/matflow/data/scripts/damask/seeds_from_random.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/damask/write_load.py` & `matflow_new-0.3.0a99/matflow/data/scripts/damask/write_load.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/damask/write_material.py` & `matflow_new-0.3.0a99/matflow/data/scripts/damask/write_material.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/formable/fit_single_crystal_parameters.py` & `matflow_new-0.3.0a99/matflow/data/scripts/formable/fit_single_crystal_parameters.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/formable/fit_yield_function.py` & `matflow_new-0.3.0a99/matflow/data/scripts/formable/fit_yield_function.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/formable/read_tensile_test_CSV.py` & `matflow_new-0.3.0a99/matflow/data/scripts/formable/read_tensile_test_CSV.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/main_script_test.py` & `matflow_new-0.3.0a99/matflow/data/scripts/main_script_test.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/mtex/plot_pole_figures.m` & `matflow_new-0.3.0a99/matflow/data/scripts/mtex/plot_pole_figures.m`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_CTF.m` & `matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_CTF.m`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_ODF_mat.m` & `matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_ODF_mat.m`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/scripts/mtex/sample_texture_model_ODF.m` & `matflow_new-0.3.0a99/matflow/data/scripts/mtex/sample_texture_model_ODF.m`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/template_components/command_files.yaml` & `matflow_new-0.3.0a99/matflow/data/template_components/command_files.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -22,26 +22,16 @@
     is_regex: true
 - label: mtex_pole_figures
   name:
     name: pole_figure.png
 - label: mtex_IPF_figure
   name:
     name: IPF_key.png
-# - label: lammps_atoms_file
-#   name:
-#     name: atoms.lammps
-# - label: lammps_input_script
-#   name:
-#     name: in.lammps
-# - label: lammps_dump_files
-#   name:
-#     name: (dump.\d+.txt)
-#     is_regex: true
-# - label: t1_outfile_1
-#   name:
-#     name: t1_outfile_1.txt
-# - label: t1_infile_1
-#   name:
-#     name: t1_infile_1.txt
-# - label: my_file
-#   name:
-#     name: my_file.txt
+- label: dream_3D_pipeline
+  name:
+    name: pipeline.json
+- label: dream_3D_hdf5_file
+  name:
+    name: pipeline.dream3d
+- label: dream_3D_XDMF_file
+  name:
+    name: pipeline.xdmf
```

### Comparing `matflow_new-0.3.0a98/matflow/data/template_components/parameters.yaml` & `matflow_new-0.3.0a99/matflow/data/template_components/parameters.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/template_components/task_schemas.yaml` & `matflow_new-0.3.0a99/matflow/data/template_components/task_schemas.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -847,7 +847,51 @@
 #         damask_geom_file:
 #           from_inputs: [material, RVE]
 #       output_file_parsers:
 #         RVE_response:
 #           from_files: [damask_hdf5_file, damask_stdout]
 #       commands:
 #         - command: DAMASK_grid --load <<input_file:damask_load_file>> --geom <<input_file:damask_geom_file>>
+
+- objective: generate_volume_element
+  method: from_statistics
+  inputs:
+    - parameter: grid_size
+    - parameter: phase_statistics
+    - parameter: resolution
+      default_value: null
+    - parameter: size
+      default_value: null
+    - parameter: origin
+      default_value: null
+    - parameter: periodic
+      default_value: true
+    - parameter: precipitates
+      default_value: null
+    - parameter: orientations
+      default_value: null
+  outputs:
+    - parameter: volume_element
+  actions:
+    - environments:
+        - scope:
+            type: any
+          environment: dream_3D_env
+      input_file_generators:
+        - input_file: dream_3D_pipeline
+          from_inputs:
+            - grid_size
+            - resolution
+            - size
+            - origin
+            - periodic
+            - phase_statistics
+            - precipitates
+            - orientations
+          script: <<script:dream_3D/generate_volume_element_statistics.py>>
+      commands:
+        - command: <<executable:dream_3D_runner>> --pipeline ${PWD}/pipeline.json
+      output_file_parsers:
+        volume_element:
+          from_files: [dream_3D_hdf5_file]
+          save_files: [dream_3D_hdf5_file, dream_3D_XDMF_file]
+          script: <<script:dream_3D/parse_dream_3D_volume_element.py>>
```

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/damask_input_files.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/damask_input_files.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/fit_single_crystal_parameters.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/fit_single_crystal_parameters.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/fit_yield_funcs.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/fit_yield_funcs.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_CTF_file.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_CTF_file.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_ODF_mat.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_ODF_mat.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/sample_texture_model_ODF.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/sample_texture_model_ODF.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/simulate_yield_surface_2D_brass.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/simulate_yield_surface_2D_brass.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/tension_DAMASK_Al.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/tension_DAMASK_Al.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/data/workflows/tension_DAMASK_Mg.yaml` & `matflow_new-0.3.0a99/matflow/data/workflows/tension_DAMASK_Mg.yaml`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/__init__.py` & `matflow_new-0.3.0a99/matflow/param_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/load.py` & `matflow_new-0.3.0a99/matflow/param_classes/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
 
         obj = cls(
             direction=direction,
             total_time=total_time,
             num_increments=num_increments,
             target_def_grad=def_grad,
             target_def_grad_rate=def_grad_rate,
-            vel_grad=vel_grad,
+            target_vel_grad=vel_grad,
             stress=stress_arr,
             dump_frequency=dump_frequency,
         )
         obj._method_name = _method_name
         obj._method_name = _method_args
         return obj
```

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/orientations.py` & `matflow_new-0.3.0a99/matflow/param_classes/orientations.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/seeds.py` & `matflow_new-0.3.0a99/matflow/param_classes/seeds.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/single_crystal_parameters.py` & `matflow_new-0.3.0a99/matflow/param_classes/single_crystal_parameters.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/param_classes/utils.py` & `matflow_new-0.3.0a99/matflow/param_classes/utils.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/tests/conftest.py` & `matflow_new-0.3.0a99/matflow/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/tests/param_classes/test_single_crystal_parameters.py` & `matflow_new-0.3.0a99/matflow/tests/param_classes/test_single_crystal_parameters.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/matflow/tests/test_utils.py` & `matflow_new-0.3.0a99/matflow/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `matflow_new-0.3.0a98/pyproject.toml` & `matflow_new-0.3.0a99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matflow-new"
-version = "0.3.0a98"
+version = "0.3.0a99"
 description = "Computational workflows for materials science"
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "matflow" }
 ]
@@ -47,15 +47,15 @@
 matflow = 'matflow.cli:cli'
 
 [tool.poetry.plugins.pyinstaller40]
 hook-dirs = "matflow.__pyinstaller:get_hook_dirs"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0a98"
+version = "0.3.0a99"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "matflow/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `matflow_new-0.3.0a98/PKG-INFO` & `matflow_new-0.3.0a99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matflow-new
-Version: 0.3.0a98
+Version: 0.3.0a99
 Summary: Computational workflows for materials science
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,15 +55,15 @@
 | **generate_volume_element**                                                                                                                                                         |        |                                                                                                                                                                                                                                                                          |
 | ⇒ method: [single_voxel_grains/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L452)                      | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [particle_RVE/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L477)                             | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [dual_phase_ti_alpha_colony](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L486)                      | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [from_damask_input_files](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L495)                         | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [from_dream3d_pipeline](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L505)                           | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [extrusion](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L511)                                       | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
-| ⇒ method: [from_statistics/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L525)                         | ❌      | [PR pending](https://github.com/hpcflow/matflow-new/pull/179)                                                                                                                                                                                                            |
+| ⇒ method: [from_statistics/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L525)                         | ✅/❌    | `generate_volume_element/from_statistics` - Not yet tested with `orientations` input                                                                                                                                                                                     |
 | ⇒ method: [from_statistics_dual_phase_orientations/Dream3D](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L568) | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [random_voronoi/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L624)                           | ✅      | [generate_volume_element/from_voronoi](https://docs.matflow.io/stable/reference/template_components/task_schemas.html#generate-volume-element)                                                                                                                           |
 | ⇒ method: [random_voronoi/neper](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L647)                            | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | ⇒ method: [random_voronoi_from_orientations](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L686)                | ✅      | Use [generate_volume_element/from_voronoi](https://docs.matflow.io/stable/reference/template_components/task_schemas.html#generate-volume-element)                                                                                                                       |
 | ⇒ method: [random_voronoi_from_dual_phase_orientations](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L716)     | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
 | **modify_volume_element**                                                                                                                                                           |        |                                                                                                                                                                                                                                                                          |
 | ⇒ method: [add_buffer_zones/damask](https://github.com/LightForm-group/UoM-CSF-matflow/blob/569fa7bdc7006d04bd6ed2d4e4b6a114df23492e/task_schemas.yml#L760)                         | ❌      | Unimplemented                                                                                                                                                                                                                                                            |
```

