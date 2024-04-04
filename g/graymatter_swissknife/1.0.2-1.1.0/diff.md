# Comparing `tmp/graymatter_swissknife-1.0.2.tar.gz` & `tmp/graymatter_swissknife-1.1.0.tar.gz`

## Comparing `graymatter_swissknife-1.0.2.tar` & `graymatter_swissknife-1.1.0.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/images/GM_models_from_GEM.png
--rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/images/gm_swissknife_square_low_res.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/__main__.py
--rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/estimate_model.py
--rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/estimate_model_noiseless.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/find_model.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/microstructure_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/__init__.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/gem.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/gem_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/functions/__init__.py
--rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/classic_constants.txt
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_dot.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_rm.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/smex.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/smex_rm.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/__init__.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/sandi.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/sandi_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/functions/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/__init__.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/sandix.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/acq_parameters.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/mist_parameters.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/save_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/rice_noise/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/rice_noise/rice_mean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/struct_functions/__init__.py
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/nls/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/nls/gridsearch.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/nls/nls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/powderaverage/__init__.py
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/src/graymatter_swissknife/powderaverage/powderaverage.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/generate_phantom.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/test_estimate_model.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/test_estimate_model_noiseless.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/mask.nii.gz
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/phantom.bval
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/phantom.nii.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/phantom.td
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/powderaverage_ref.bval
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/powderaverage_ref.td
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_sigma_ref.nii.gz
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/models/test_nexi_functions.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/models/test_rician_mean.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/LICENSE
--rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/README.md
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9365 2020-02-02 00:00:00.000000 graymatter_swissknife-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/images/GM_models_from_GEM.png
+-rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/images/gm_swissknife_square_low_res.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/__main__.py
+-rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/estimate_model.py
+-rw-r--r--   0        0        0    10845 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/estimate_model_noiseless.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/find_model.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/microstructure_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/gem.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/gem_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/functions/__init__.py
+-rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/__init__.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_dot.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_rm.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/smex.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/smex_rm.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/sandi.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/sandi_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/functions/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/sandix.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/acq_parameters.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/mist_parameters.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/save_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/rice_noise/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/rice_noise/rice_mean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/struct_functions/__init__.py
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/nls/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/nls/gridsearch.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/nls/nls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/powderaverage/__init__.py
+-rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/powderaverage/powderaverage.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/xgboost/define_xgboost_model.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/src/graymatter_swissknife/xgboost/generate_dataset.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/generate_phantom.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/test_estimate_model.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/test_estimate_model_noiseless.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/mask.nii.gz
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/phantom.bval
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/phantom.nii.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/phantom.td
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/powderaverage_ref.bval
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/powderaverage_ref.td
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_sigma_ref.nii.gz
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/models/test_nexi_functions.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/models/test_rician_mean.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.0/PKG-INFO
```

### Comparing `graymatter_swissknife-1.0.2/images/GM_models_from_GEM.png` & `graymatter_swissknife-1.1.0/images/GM_models_from_GEM.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/images/gm_swissknife_square_low_res.png` & `graymatter_swissknife-1.1.0/images/gm_swissknife_square_low_res.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/estimate_model.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/estimate_model_noiseless.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 import os
 import logging
 import argparse
 import numpy as np
-from .powderaverage.powderaverage import powder_average, normalize_sigma, save_data_as_npz
+from .powderaverage.powderaverage import powder_average, save_data_as_npz
 from .models.find_model import find_model
 from .models.parameters.acq_parameters import AcquisitionParameters
 from .models.parameters.save_parameters import save_estimations_as_nifti
 from .nls.nls import nls_parallel
 from .nls.gridsearch import find_nls_initialization
+from .xgboost.define_xgboost_model import define_xgboost_model
+from .xgboost.apply_xgboost_model import apply_xgboost_model
 
 
-def estimate_model(model_name, dwi_path, bvals_path, td_path, small_delta, lowb_noisemap_path, out_path, 
-                   mask_path=None, fixed_parameters=None, adjust_parameter_limits=None, 
-                   n_cores=-1 ,debug=False):
+def estimate_model_noiseless(model_name, dwi_path, bvals_path, td_path, small_delta, out_path, 
+                             mask_path=None, fixed_parameters=None, adjust_parameter_limits=None, 
+                             optimization_method='NLS', xgboost_model_path=None, retrain_xgboost=False,
+                             n_cores=-1, debug=False):
     """
-    Estimate the model parameters for a given set of preprocessed signals,
-    providing the b-values, diffusion times and low b-values noise map. A mask is optional but highly recommended.
+    Estimate the noiseless NEXI model parameters for a given set of preprocessed signals,
+    providing the b-values and diffusion times. A mask is optional but highly recommended.
 
     Parameters
     ----------
     dwi_path : str
         Path to the preprocessed DWI signal.
     bvals_path : str
         Path to the b-values file. b-values must be provided in ms/µm².
     td_path : str
         Path to the diffusion time file. Diffusion time must be provided in ms.
     small_delta : float
         Small delta value in ms. This value is optional for NEXI (NEXI with Narrow Pulse Approximation (NPA)) but is mandatory for other models.
         If using NEXI with NPA, set small_delta to None.
-    lowb_noisemap_path : str
-        Path to the low b-values (b < 2ms/µm²) noise map.
     out_path : str
         Path to the output directory. If the directory does not exist, it will be created.
     mask_path : str, optional
         Path to the mask file. The default is None.
-    fixed_parameters : tuple
+    fixed_parameters : tuple, optional
         Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. 
-        The tuple must have the same length as the number of parameters of the model (with or without noise correction).
+        The tuple must have the same length as the number of parameters of the model.
         Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
-    adjust_parameter_limits : tuple
+    adjust_parameter_limits : tuple, optional
         Allows to adjust the parameter limits for the Non-Linear Least Squares if not set to None. Tuple of adjusted parameter limits for the model.
-        The tuple must have the same length as the number of parameters of the model (with or without noise correction).
+        The tuple must have the same length as the number of parameters of the model.
         Example of use: Adjust the parameter limits for Di to [1.5, 2.5]µm²/ms and De to [0.5, 1.5]µm²/ms in the NEXI model by specifying adjust_parameter_limits=(None, [1.5, 2.5], [0.5, 1.5], None)
+    optimization_method : string, optional
+        Optimization method to use. 'NLS' for Non-Linear Least Squares. 'XGBoost' for XGBoost (Machine Learning). 
+        The default is 'NLS'.
+    xgboost_model_path : string, optional
+        Path to your future or pretrained XGBoost model file. Allowed file extensions are json or ubj.
+        Example: 'yourfolder/cohort_microstructuremodel.ubj'. 
+        The default is None.
+    retrain_xgboost : bool, optional
+        If True, the XGBoost model will be retrained. If False, the XGBoost model will be loaded from the xgboost_model_path.
     n_cores : int, optional
         Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
     debug : bool, optional
         Debug mode. The default is False.
 
     Returns
     -------
@@ -58,114 +68,135 @@
     if not os.path.exists(out_path):
         os.makedirs(out_path)
 
     # Convert into powder average
     powder_average_path, updated_bvals_path, updated_td_path = powder_average(
         dwi_path, bvals_path, td_path, mask_path, out_path, debug=debug
     )
-    # NEXI with Rician Mean correction
-    normalized_sigma_filename = normalize_sigma(dwi_path, lowb_noisemap_path, bvals_path, out_path)
+    # Model without Rician Mean correction
     powder_average_signal_npz_filename = save_data_as_npz(
-        powder_average_path,
-        updated_bvals_path,
-        updated_td_path,
-        out_path,
-        normalized_sigma_filename=normalized_sigma_filename,
-        debug=debug,
+        powder_average_path, updated_bvals_path, updated_td_path, out_path, debug=debug
     )
 
-    # Load the powder average signal, normalized sigma, b-values and diffusion time (acquisition parameters)
+    # Load the powder average signal, b-values and diffusion time (acquisition parameters)
     powder_average_signal_npz = np.load(powder_average_signal_npz_filename)
     signal = powder_average_signal_npz['signal']
     voxel_nb = len(signal)
-    sigma = powder_average_signal_npz['sigma']
     bvals = powder_average_signal_npz['b']
     td = powder_average_signal_npz['td']
     acq_param = AcquisitionParameters(bvals, td, small_delta=small_delta)
 
-    # Estimate the model parameters
+    # Estimate the microstructure model parameters
 
     # Define the parameter limits for the Non-Linear Least Squares
-    microstruct_model = find_model(model_name + 'RiceMean')
-    nls_param_lim = microstruct_model.param_lim
+    microstruct_model = find_model(model_name)
+    parameter_limits = microstruct_model.param_lim
     grid_search_nb_points = microstruct_model.grid_search_nb_points
     max_nls_verif = 1
 
-    # Replace the NLS parameter limits if adjust_parameter_limits if provided
+    # Replace the NLS parameter limits if adjust_parameter_limits is provided
     if adjust_parameter_limits is not None:
         # Assert that the number of parameters in the model and the number of fixed parameters are the same
         assert (len(adjust_parameter_limits) == microstruct_model.n_params - 1) or (len(adjusted_param_limit) == microstruct_model.n_params), "The number of parameters in the model and the length of adjusted_param_limit are different. Set the unchanged parameter limits in the adjusted_param_limit tuple to None."
 
         # Replace the NLS parameter limits for the fixed parameters
         for i, (adjusted_param_limit) in enumerate(adjust_parameter_limits):
             if adjusted_param_limit is not None:
                 assert len(adjusted_param_limit) == 2, "The adjusted parameter limits must be a tuple of two values."
-                nls_param_lim[i] = [adjusted_param_limit[0], adjusted_param_limit[1]]
+                parameter_limits[i] = [adjusted_param_limit[0], adjusted_param_limit[1]]
     
     # Replace the NLS parameter limits for the fixed parameters if provided
     if fixed_parameters is not None:
         # Assert that the number of parameters in the model and the number of fixed parameters are the same
-        assert (len(fixed_parameters) == microstruct_model.n_params - 1) or (len(fixed_parameters) == microstruct_model.n_params), "The number of parameters in the model and the length of fixed_parameters are different. Set the moving parameters in the fixed_parameters tuple to None."
+        assert microstruct_model.n_params == len(fixed_parameters), "The number of parameters in the model and the length of fixed_parameters are different. Set the moving parameters in the fixed_parameters tuple to None."
 
         # Replace the NLS parameter limits for the fixed parameters
         for i, fixed_param in enumerate(fixed_parameters):
             if fixed_param is not None:
-                nls_param_lim[i] = [fixed_param, fixed_param]
-
-    # Compute the initial Ground Truth to start the NLS with if requested
-    initial_grid_search = True
-    initial_gt = None
-    if initial_grid_search:
-        initial_gt = find_nls_initialization(
-            signal, sigma, voxel_nb, acq_param, microstruct_model, nls_param_lim, grid_search_nb_points, debug=debug
+                parameter_limits[i] = [fixed_param, fixed_param]
+    
+    # Update the parameter limits in the microstructure model
+    microstruct_model.param_lim = parameter_limits
+    
+    # Check the optimization method
+    optimization_method = optimization_method.lower()
+    assert optimization_method in ['nls', 'xgboost'], "The optimization method must be 'NLS' or 'XGBoost'."
+
+    if optimization_method == 'nls':
+
+        # Compute the initial Ground Truth to start the NLS with if requested
+        initial_grid_search = True
+        initial_gt = None
+        if initial_grid_search:
+            initial_gt = find_nls_initialization(
+                signal, None, voxel_nb, acq_param, microstruct_model, parameter_limits, grid_search_nb_points, debug=debug
+            )
+
+        # Compute the NLS estimations
+        estimations, estimation_init = nls_parallel(
+            signal,
+            voxel_nb,
+            microstruct_model,
+            acq_param,
+            nls_param_lim=parameter_limits,
+            max_nls_verif=max_nls_verif,
+            initial_gt=initial_gt,
+            n_cores=n_cores
         )
+    
+    elif optimization_method == 'xgboost':
 
-    # Compute the NLS estimations
-    estimations, estimation_init = nls_parallel(
-        signal,
-        voxel_nb,
-        microstruct_model,
-        acq_param,
-        nls_param_lim=nls_param_lim,
-        max_nls_verif=max_nls_verif,
-        initial_gt=initial_gt,
-        n_cores=n_cores
-    )
+        # No initialization in XGBoost
+        estimation_init = None
+
+        # Check if the XGBoost model path is provided
+        assert xgboost_model_path is not None, "The XGBoost model path must be provided, either to save or load the model."
+
+        # Define the XGBoost model from a file or generate and train it
+        n_training_samples = 1000000
+        xgboost_model = define_xgboost_model(xgboost_model_path, retrain_xgboost, 
+                                             microstruct_model, acq_param, n_training_samples, None, n_cores)
+        
+        # Apply the XGBoost model
+        estimations = apply_xgboost_model(xgboost_model, signal, microstruct_model)
+    
+    else:
+        raise ValueError("The optimization method must be 'NLS' or 'XGBoost'.")
 
-    # Save the model parameters
+    # Save the NEXI model parameters
     if debug:
         np.savez_compressed(
             f'{out_path}/{microstruct_model.name.lower()}_estimations.npz',
             estimations=estimations,
             estimation_init=estimation_init,
         )
 
-    # Save the model parameters as nifti
+    # Save the NEXI model parameters as nifti
     save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, mask_path, out_path)
 
 
 if __name__ == '__main__':
     # Parse arguments
     parser = argparse.ArgumentParser(
         description='Estimate the NEXI model parameters for a given set of preprocessed '
         'signals, providing the b-values and diffusion time.'
     )
+    parser.add_argument('model_name', help='microstructure model name between Nexi, Smex, Sandi, Sandix and Gem. NexiDot is also possible.')
     parser.add_argument('dwi_path', help='path to the preprocessed signals')
     # For conversion from b-values in s/µm² to b-values in ms/µm², divide by 1000
     parser.add_argument('bvals_path', help='path to the b-values (in ms/µm²) txt file')
     parser.add_argument('td_path', help='path to the diffusion times (in ms) txt file')
-    parser.add_argument('lowb_noisemap_path', help='path to the lowb noisemap')
     parser.add_argument('out_path', help='path to the output folder')
     # potential arguments
     # Set to None if not provided
     parser.add_argument('--small_delta', help='small delta (in ms)', required=False, type=float, default=None)
     parser.add_argument('--mask_path', help='path to the mask', required=False, default=None)
     parser.add_argument('--fixed_parameters', help='tuple of fixed parameters', required=False, default=None)
     parser.add_argument('--adjust_parameter_limits', help='tuple of adjusted parameter limits', required=False, default=None)
     parser.add_argument('--debug', help='debug mode', required=False, action='store_true')
     args = parser.parse_args()
 
     # estimate_nexi(**vars(parser.parse_args()))
-    estimate_model(model_name=args.model_name, dwi_path=args.dwi_path, bvals_path=args.bvals_path, td_path=args.td_path, 
-                   small_delta=args.small_delta, lowb_noisemap_path=args.lowb_noisemap_path, out_path=args.out_path, 
-                   mask_path=args.mask_path, fixed_parameters=args.fixed_parameters, adjust_parameter_limits=args.adjust_parameter_limits, 
-                   debug=args.debug)
+    estimate_model_noiseless(model_name=args.model_name, dwi_path=args.dwi_path, bvals_path=args.bvals_path, td_path=args.td_path, 
+                             small_delta=args.small_delta, out_path=args.out_path, mask_path=args.mask_path, 
+                             fixed_parameters=args.fixed_parameters, adjust_parameter_limits=args.adjust_parameter_limits, 
+                             debug=args.debug)
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/estimate_model_noiseless.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/estimate_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 import os
 import logging
 import argparse
 import numpy as np
-from .powderaverage.powderaverage import powder_average, save_data_as_npz
+from .powderaverage.powderaverage import powder_average, normalize_sigma, save_data_as_npz
 from .models.find_model import find_model
 from .models.parameters.acq_parameters import AcquisitionParameters
 from .models.parameters.save_parameters import save_estimations_as_nifti
 from .nls.nls import nls_parallel
 from .nls.gridsearch import find_nls_initialization
+from .xgboost.define_xgboost_model import define_xgboost_model
+from .xgboost.apply_xgboost_model import apply_xgboost_model
 
 
-def estimate_model_noiseless(model_name, dwi_path, bvals_path, td_path, small_delta, out_path, 
-                             mask_path=None, fixed_parameters=None, adjust_parameter_limits=None, 
-                             n_cores=-1, debug=False):
+def estimate_model(model_name, dwi_path, bvals_path, td_path, small_delta, lowb_noisemap_path, out_path, 
+                   mask_path=None, fixed_parameters=None, adjust_parameter_limits=None, 
+                   optimization_method='NLS', xgboost_model_path=None, retrain_xgboost=False,
+                   n_cores=-1 ,debug=False):
     """
-    Estimate the noiseless NEXI model parameters for a given set of preprocessed signals,
-    providing the b-values and diffusion times. A mask is optional but highly recommended.
+    Estimate the model parameters for a given set of preprocessed signals,
+    providing the b-values, diffusion times and low b-values noise map. A mask is optional but highly recommended.
 
     Parameters
     ----------
     dwi_path : str
         Path to the preprocessed DWI signal.
     bvals_path : str
         Path to the b-values file. b-values must be provided in ms/µm².
     td_path : str
         Path to the diffusion time file. Diffusion time must be provided in ms.
     small_delta : float
         Small delta value in ms. This value is optional for NEXI (NEXI with Narrow Pulse Approximation (NPA)) but is mandatory for other models.
         If using NEXI with NPA, set small_delta to None.
+    lowb_noisemap_path : str
+        Path to the low b-values (b < 2ms/µm²) noise map.
     out_path : str
         Path to the output directory. If the directory does not exist, it will be created.
     mask_path : str, optional
         Path to the mask file. The default is None.
-    fixed_parameters : tuple
+    fixed_parameters : tuple, optional
         Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. 
-        The tuple must have the same length as the number of parameters of the model.
+        The tuple must have the same length as the number of parameters of the model (with or without noise correction).
         Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
-    adjust_parameter_limits : tuple
+    adjust_parameter_limits : tuple, optional
         Allows to adjust the parameter limits for the Non-Linear Least Squares if not set to None. Tuple of adjusted parameter limits for the model.
-        The tuple must have the same length as the number of parameters of the model.
+        The tuple must have the same length as the number of parameters of the model (with or without noise correction).
         Example of use: Adjust the parameter limits for Di to [1.5, 2.5]µm²/ms and De to [0.5, 1.5]µm²/ms in the NEXI model by specifying adjust_parameter_limits=(None, [1.5, 2.5], [0.5, 1.5], None)
+    optimization_method : string, optional
+        Optimization method to use. 'NLS' for Non-Linear Least Squares. 'XGBoost' for XGBoost (Machine Learning). 
+        The default is 'NLS'.
+    xgboost_model_path : string, optional
+        Path to your future or pretrained XGBoost model file. Allowed file extensions are json or ubj.
+        Example: 'yourfolder/cohort_microstructuremodel.ubj'. 
+        The default is None.
+    retrain_xgboost : bool, optional
+        If True, the XGBoost model will be retrained. If False, the XGBoost model will be loaded from the xgboost_model_path.
     n_cores : int, optional
         Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
     debug : bool, optional
         Debug mode. The default is False.
 
     Returns
     -------
@@ -56,107 +70,142 @@
     if not os.path.exists(out_path):
         os.makedirs(out_path)
 
     # Convert into powder average
     powder_average_path, updated_bvals_path, updated_td_path = powder_average(
         dwi_path, bvals_path, td_path, mask_path, out_path, debug=debug
     )
-    # Model without Rician Mean correction
+    # NEXI with Rician Mean correction
+    normalized_sigma_filename = normalize_sigma(dwi_path, lowb_noisemap_path, bvals_path, out_path)
     powder_average_signal_npz_filename = save_data_as_npz(
-        powder_average_path, updated_bvals_path, updated_td_path, out_path, debug=debug
+        powder_average_path,
+        updated_bvals_path,
+        updated_td_path,
+        out_path,
+        normalized_sigma_filename=normalized_sigma_filename,
+        debug=debug,
     )
 
-    # Load the powder average signal, b-values and diffusion time (acquisition parameters)
+    # Load the powder average signal, normalized sigma, b-values and diffusion time (acquisition parameters)
     powder_average_signal_npz = np.load(powder_average_signal_npz_filename)
     signal = powder_average_signal_npz['signal']
     voxel_nb = len(signal)
+    sigma = powder_average_signal_npz['sigma']
     bvals = powder_average_signal_npz['b']
     td = powder_average_signal_npz['td']
     acq_param = AcquisitionParameters(bvals, td, small_delta=small_delta)
 
-    # Estimate the microstructure model parameters
+    # Estimate the model parameters
 
     # Define the parameter limits for the Non-Linear Least Squares
-    microstruct_model = find_model(model_name)
-    nls_param_lim = microstruct_model.param_lim
+    microstruct_model = find_model(model_name + 'RiceMean')
+    parameter_limits = microstruct_model.param_lim
     grid_search_nb_points = microstruct_model.grid_search_nb_points
     max_nls_verif = 1
 
-    # Replace the NLS parameter limits if adjust_parameter_limits is provided
+    # Replace the NLS parameter limits if adjust_parameter_limits if provided
     if adjust_parameter_limits is not None:
         # Assert that the number of parameters in the model and the number of fixed parameters are the same
         assert (len(adjust_parameter_limits) == microstruct_model.n_params - 1) or (len(adjusted_param_limit) == microstruct_model.n_params), "The number of parameters in the model and the length of adjusted_param_limit are different. Set the unchanged parameter limits in the adjusted_param_limit tuple to None."
 
         # Replace the NLS parameter limits for the fixed parameters
         for i, (adjusted_param_limit) in enumerate(adjust_parameter_limits):
             if adjusted_param_limit is not None:
                 assert len(adjusted_param_limit) == 2, "The adjusted parameter limits must be a tuple of two values."
-                nls_param_lim[i] = [adjusted_param_limit[0], adjusted_param_limit[1]]
+                parameter_limits[i] = [adjusted_param_limit[0], adjusted_param_limit[1]]
     
     # Replace the NLS parameter limits for the fixed parameters if provided
     if fixed_parameters is not None:
         # Assert that the number of parameters in the model and the number of fixed parameters are the same
-        assert microstruct_model.n_params == len(fixed_parameters), "The number of parameters in the model and the length of fixed_parameters are different. Set the moving parameters in the fixed_parameters tuple to None."
+        assert (len(fixed_parameters) == microstruct_model.n_params - 1) or (len(fixed_parameters) == microstruct_model.n_params), "The number of parameters in the model and the length of fixed_parameters are different. Set the moving parameters in the fixed_parameters tuple to None."
 
         # Replace the NLS parameter limits for the fixed parameters
         for i, fixed_param in enumerate(fixed_parameters):
             if fixed_param is not None:
-                nls_param_lim[i] = [fixed_param, fixed_param]
-
-    # Compute the initial Ground Truth to start the NLS with if requested
-    initial_grid_search = True
-    initial_gt = None
-    if initial_grid_search:
-        initial_gt = find_nls_initialization(
-            signal, None, voxel_nb, acq_param, microstruct_model, nls_param_lim, grid_search_nb_points, debug=debug
+                parameter_limits[i] = [fixed_param, fixed_param]
+    
+    # Update the parameter limits in the microstructure model
+    microstruct_model.param_lim = parameter_limits
+    
+    # Check the optimization method
+    optimization_method = optimization_method.lower()
+    assert optimization_method in ['nls', 'xgboost'], "The optimization method must be 'NLS' or 'XGBoost'."
+
+    if optimization_method == 'nls':
+
+        # Compute the initial Ground Truth to start the NLS with if requested
+        initial_grid_search = True
+        initial_gt = None
+        if initial_grid_search:
+            initial_gt = find_nls_initialization(
+                signal, sigma, voxel_nb, acq_param, microstruct_model, parameter_limits, grid_search_nb_points, debug=debug
+            )
+
+        # Compute the NLS estimations
+        estimations, estimation_init = nls_parallel(
+            signal,
+            voxel_nb,
+            microstruct_model,
+            acq_param,
+            nls_param_lim=parameter_limits,
+            max_nls_verif=max_nls_verif,
+            initial_gt=initial_gt,
+            n_cores=n_cores
         )
 
-    # Compute the NLS estimations
-    estimations, estimation_init = nls_parallel(
-        signal,
-        voxel_nb,
-        microstruct_model,
-        acq_param,
-        nls_param_lim=nls_param_lim,
-        max_nls_verif=max_nls_verif,
-        initial_gt=initial_gt,
-        n_cores=n_cores
-    )
+    elif optimization_method == 'xgboost':
 
-    # Save the NEXI model parameters
+        # No initialization in XGBoost
+        estimation_init = None
+
+        # Check if the XGBoost model path is provided
+        assert xgboost_model_path is not None, "The XGBoost model path must be provided, either to save or load the model."
+
+        # Define the XGBoost model from a file or generate and train it
+        n_training_samples = 1000000
+        xgboost_model = define_xgboost_model(xgboost_model_path, retrain_xgboost, 
+                                             microstruct_model, acq_param, n_training_samples, sigma, n_cores)
+        
+        # Apply the XGBoost model
+        estimations = apply_xgboost_model(xgboost_model, signal, microstruct_model)
+    
+    else:
+        raise ValueError("The optimization method must be 'NLS' or 'XGBoost'.")
+    
+    # Save the model parameters
     if debug:
         np.savez_compressed(
             f'{out_path}/{microstruct_model.name.lower()}_estimations.npz',
             estimations=estimations,
             estimation_init=estimation_init,
         )
 
-    # Save the NEXI model parameters as nifti
+    # Save the model parameters as nifti
     save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, mask_path, out_path)
 
 
 if __name__ == '__main__':
     # Parse arguments
     parser = argparse.ArgumentParser(
         description='Estimate the NEXI model parameters for a given set of preprocessed '
         'signals, providing the b-values and diffusion time.'
     )
-    parser.add_argument('model_name', help='microstructure model name between Nexi, Smex, Sandi, Sandix and Gem. NexiDot is also possible.')
     parser.add_argument('dwi_path', help='path to the preprocessed signals')
     # For conversion from b-values in s/µm² to b-values in ms/µm², divide by 1000
     parser.add_argument('bvals_path', help='path to the b-values (in ms/µm²) txt file')
     parser.add_argument('td_path', help='path to the diffusion times (in ms) txt file')
+    parser.add_argument('lowb_noisemap_path', help='path to the lowb noisemap')
     parser.add_argument('out_path', help='path to the output folder')
     # potential arguments
     # Set to None if not provided
     parser.add_argument('--small_delta', help='small delta (in ms)', required=False, type=float, default=None)
     parser.add_argument('--mask_path', help='path to the mask', required=False, default=None)
     parser.add_argument('--fixed_parameters', help='tuple of fixed parameters', required=False, default=None)
     parser.add_argument('--adjust_parameter_limits', help='tuple of adjusted parameter limits', required=False, default=None)
     parser.add_argument('--debug', help='debug mode', required=False, action='store_true')
     args = parser.parse_args()
 
     # estimate_nexi(**vars(parser.parse_args()))
-    estimate_model_noiseless(model_name=args.model_name, dwi_path=args.dwi_path, bvals_path=args.bvals_path, td_path=args.td_path, 
-                             small_delta=args.small_delta, out_path=args.out_path, mask_path=args.mask_path, 
-                             fixed_parameters=args.fixed_parameters, adjust_parameter_limits=args.adjust_parameter_limits, 
-                             debug=args.debug)
+    estimate_model(model_name=args.model_name, dwi_path=args.dwi_path, bvals_path=args.bvals_path, td_path=args.td_path, 
+                   small_delta=args.small_delta, lowb_noisemap_path=args.lowb_noisemap_path, out_path=args.out_path, 
+                   mask_path=args.mask_path, fixed_parameters=args.fixed_parameters, adjust_parameter_limits=args.adjust_parameter_limits, 
+                   debug=args.debug)
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/find_model.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/find_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/microstructure_models.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/microstructure_models.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/gem.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/gem.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     # Class attributes
     n_params = 7
     param_names = ["t_exs", "t_exd", "Dd", "De", "fn", "radius", "fsn"]
     classic_limits = np.array([[1, 150], [1, 150], [0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5]])
     grid_search_nb_points = [5, 5, 5, 5, 5, 5, 5]  # Optimal would be [12, 8, 5, 5, 5, 5, 5], but it will depends on how much time your machine takes
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='GEM')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[2] < param[3]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/gem_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/gem_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     n_params = 8
     param_names = ["t_exs", "t_exd", "Dd", "De", "fn", "radius", "fsn", "sigma"]
     classic_limits = np.array([[1, 150], [1, 150], [0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5], [0, 100]])
     grid_search_nb_points = [5, 5, 5, 5, 5, 5, 5]  # Optimal would be [12, 8, 5, 5, 5, 5, 5], but it will depends on how much time your machine takes
     has_rician_mean_correction = True
     non_corrected_model = Gem()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='GEM_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[2] < param[3]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     # Class attributes
     n_params = 4
     param_names = ["t_ex", "Di", "De", "f"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9]])
     grid_search_nb_points = [15, 12, 8, 8]
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='NEXI')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_dot.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/sandi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-import numpy as np
 from ...models.microstructure_models import MicroStructModel
-from .functions.scipy_nexi_dot import nexi_dot_signal_from_vector, \
-    nexi_dot_jacobian_from_vector, nexi_dot_optimized_mse_jacobian
+from .functions.scipy_sandi import sandi_signal_from_vector, sandi_jacobian_from_vector, sandi_optimized_mse_jacobian
+# from models.SANDI.functions.torch_sandi import torch_sandi_signal_from_vector
+import numpy as np
 
 
-class NexiDot(MicroStructModel):
-    """Neurite Exchange Imaging model ( Narrow Pulse approximation) with an additional dot compartment for diffusion MRI."""
+class Sandi(MicroStructModel):
+    """Soma And Neurite Density Imaging model for diffusion MRI."""
 
     # Class attributes
     n_params = 5
-    param_names = ["t_ex", "Di", "De", "f", "f_dot"]
-    classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9], [0.0, 0.3]])
-    grid_search_nb_points = [15, 12, 8, 8, 6]
+    param_names = ["Di", "De", "f", "rs", "fs"]
+    classic_limits = np.array([[0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5]])
+    grid_search_nb_points = [15, 8, 8, 12, 8]
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
-        super().__init__(name='NEXI_dot')
+    def __init__(self, param_lim=classic_limits):
+        super().__init__(name='SANDI')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
-            if param[1] < param[2]:
+            if param[0] < param[1]:
                 # exchange them
-                param[1], param[2] = param[2], param[1]
+                param[0], param[1] = param[1], param[0]
         elif np.array(param).ndim == 2:
             # Put Di>De
             for iset in range(len(param)):
                 # if Di < De of the set iset
-                if param[iset, 1] < param[iset, 2]:
+                if param[iset, 0] < param[iset, 1]:
                     # exchange them
-                    param[iset, 1], param[iset, 2] = param[iset, 2], param[iset, 1]
+                    param[iset, 0], param[iset, 1] = param[iset, 1], param[iset, 0]
         else:
             raise ValueError('Wrong dimension of parameters')
         return param
 
     def set_param_lim(self, param_lim):
         self.param_lim = param_lim
 
     @classmethod
     def get_signal(cls, parameters, acq_parameters):
         """Get signal from single Ground Truth."""
-        return nexi_dot_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td)
+        return sandi_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
 
     @classmethod
     def get_jacobian(cls, parameters, acq_parameters):
         """Get jacobian from single Ground Truth."""
-        return nexi_dot_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td)
+        signal, jacobian = sandi_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td,
+                                                      acq_parameters.small_delta)
+        return jacobian
 
     @classmethod
     def get_hessian(cls, parameters, acq_parameters):
         """Get hessian from single Ground Truth."""
-        return None  # KM_dot_vec_hess(parameters, acq_parameters.b, acq_parameters.td)
+        return None
 
     # Optimized methods for Non-linear Least Squares
     @classmethod
     def get_mse_jacobian(cls, parameters, acq_parameters, signal_gt):
         """Get signal from single Ground Truth."""
-        return nexi_dot_optimized_mse_jacobian(parameters, acq_parameters.b, acq_parameters.td, signal_gt, acq_parameters.ndim)
+        return sandi_optimized_mse_jacobian(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta,
+                                            signal_gt, acq_parameters.ndim)
+
+
+    # @classmethod
+    # def get_torch_signal(cls, parameters, acq_parameters):
+    #     """Get signal from single Ground Truth."""
+    #     return torch_sandi_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     n_params = 6
     param_names = ["t_ex", "Di", "De", "f", "f_dot", "sigma"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9], [0.0, 0.3], [0, 100]])
     grid_search_nb_points = [15, 12, 8, 8, 6]
     has_rician_mean_correction = True
     non_corrected_model = NexiDot()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='Nexi_Dot_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/nexi_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     n_params = 5
     param_names = ["t_ex", "Di", "De", "f", "sigma"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9], [0, 100]])
     grid_search_nb_points = [15, 12, 8, 8]
     has_rician_mean_correction = True
     non_corrected_model = Nexi()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='NEXI_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/smex.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/smex.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,17 @@
     # Class attributes
     n_params = 4
     param_names = ["t_ex", "Di", "De", "f"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9]])
     grid_search_nb_points = [15, 12, 8, 8]
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='SMEX')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/smex_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/smex_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     n_params = 5
     param_names = ["t_ex", "Di", "De", "f", "sigma"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9], [0, 100]])
     grid_search_nb_points = [15, 12, 8, 8]
     has_rician_mean_correction = True
     non_corrected_model = Smex()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='SMEX_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/sandi.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/sandix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,62 @@
-from ...models.microstructure_models import MicroStructModel
-from .functions.scipy_sandi import sandi_signal_from_vector, sandi_jacobian_from_vector, sandi_optimized_mse_jacobian
-# from models.SANDI.functions.torch_sandi import torch_sandi_signal_from_vector
 import numpy as np
+from ...models.microstructure_models import MicroStructModel
+from .functions.scipy_sandix import (sandix_signal_from_vector,
+                                                                sandix_jacobian_from_vector,
+                                                                sandix_optimized_mse_jacobian)
 
 
-class Sandi(MicroStructModel):
-    """Soma And Neurite Density Imaging model for diffusion MRI."""
+class Sandix(MicroStructModel):
+    """Soma And Neurite Density Imaging model with Exchange for diffusion MRI."""
 
     # Class attributes
-    n_params = 5
-    param_names = ["Di", "De", "f", "rs", "fs"]
-    classic_limits = np.array([[0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5]])
-    grid_search_nb_points = [15, 8, 8, 12, 8]
+    n_params = 6
+    param_names = ["t_ex", "Di", "De", "f", "rs", "fs"]
+    classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5]])
+    grid_search_nb_points = [7, 5, 5, 5, 5, 5]  # Optimal would be [12, 8, 5, 5, 5, 5], but it will depends on how much time your machine takes
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
-        super().__init__(name='SANDI')
+    def __init__(self, param_lim=classic_limits):
+        super().__init__(name='SANDIX')
         self.param_lim = param_lim
-        self.invert_tex = False
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
-            if param[0] < param[1]:
+            if param[1] < param[2]:
                 # exchange them
-                param[0], param[1] = param[1], param[0]
+                param[1], param[2] = param[2], param[1]
         elif np.array(param).ndim == 2:
             # Put Di>De
             for iset in range(len(param)):
                 # if Di < De of the set iset
-                if param[iset, 0] < param[iset, 1]:
+                if param[iset, 1] < param[iset, 2]:
                     # exchange them
-                    param[iset, 0], param[iset, 1] = param[iset, 1], param[iset, 0]
+                    param[iset, 1], param[iset, 2] = param[iset, 2], param[iset, 1]
         else:
             raise ValueError('Wrong dimension of parameters')
         return param
 
     def set_param_lim(self, param_lim):
         self.param_lim = param_lim
 
     @classmethod
     def get_signal(cls, parameters, acq_parameters):
         """Get signal from single Ground Truth."""
-        return sandi_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
+        return sandix_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
 
     @classmethod
     def get_jacobian(cls, parameters, acq_parameters):
         """Get jacobian from single Ground Truth."""
-        signal, jacobian = sandi_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td,
-                                                      acq_parameters.small_delta)
-        return jacobian
+        return sandix_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
 
     @classmethod
     def get_hessian(cls, parameters, acq_parameters):
-        """Get hessian from single Ground Truth."""
         return None
 
     # Optimized methods for Non-linear Least Squares
     @classmethod
     def get_mse_jacobian(cls, parameters, acq_parameters, signal_gt):
-        """Get signal from single Ground Truth."""
-        return sandi_optimized_mse_jacobian(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta,
-                                            signal_gt, acq_parameters.ndim)
-
-
-    # @classmethod
-    # def get_torch_signal(cls, parameters, acq_parameters):
-    #     """Get signal from single Ground Truth."""
-    #     return torch_sandi_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
+        """Get jacobian of Mean Square Error from single Ground Truth."""
+        return sandix_optimized_mse_jacobian(parameters, acq_parameters, signal_gt)
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/sandi_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/sandi_rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     n_params = 6
     param_names = ["Di", "De", "f", "rs", "fs", "sigma"]
     classic_limits = np.array([[0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5], [0, 100]])
     grid_search_nb_points = [15, 8, 8, 12, 8]
     has_rician_mean_correction = True
     non_corrected_model = Sandi()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='SANDI_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = False
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[0] < param[1]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/sandix.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/NEXI/nexi_dot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import numpy as np
 from ...models.microstructure_models import MicroStructModel
-from .functions.scipy_sandix import (sandix_signal_from_vector,
-                                                                sandix_jacobian_from_vector,
-                                                                sandix_optimized_mse_jacobian)
+from .functions.scipy_nexi_dot import nexi_dot_signal_from_vector, \
+    nexi_dot_jacobian_from_vector, nexi_dot_optimized_mse_jacobian
 
 
-class Sandix(MicroStructModel):
-    """Soma And Neurite Density Imaging model with Exchange for diffusion MRI."""
+class NexiDot(MicroStructModel):
+    """Neurite Exchange Imaging model ( Narrow Pulse approximation) with an additional dot compartment for diffusion MRI."""
 
     # Class attributes
-    n_params = 6
-    param_names = ["t_ex", "Di", "De", "f", "rs", "fs"]
-    classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5]])
-    grid_search_nb_points = [7, 5, 5, 5, 5, 5]  # Optimal would be [12, 8, 5, 5, 5, 5], but it will depends on how much time your machine takes
+    n_params = 5
+    param_names = ["t_ex", "Di", "De", "f", "f_dot"]
+    classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.1, 0.9], [0.0, 0.3]])
+    grid_search_nb_points = [15, 12, 8, 8, 6]
     has_rician_mean_correction = False
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
-        super().__init__(name='SANDIX')
+    def __init__(self, param_lim=classic_limits):
+        super().__init__(name='NEXI_dot')
         self.param_lim = param_lim
-        self.invert_tex = invert_tex
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[1] < param[2]:
@@ -41,23 +39,24 @@
 
     def set_param_lim(self, param_lim):
         self.param_lim = param_lim
 
     @classmethod
     def get_signal(cls, parameters, acq_parameters):
         """Get signal from single Ground Truth."""
-        return sandix_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
+        return nexi_dot_signal_from_vector(parameters, acq_parameters.b, acq_parameters.td)
 
     @classmethod
     def get_jacobian(cls, parameters, acq_parameters):
         """Get jacobian from single Ground Truth."""
-        return sandix_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td, acq_parameters.small_delta)
+        return nexi_dot_jacobian_from_vector(parameters, acq_parameters.b, acq_parameters.td)
 
     @classmethod
     def get_hessian(cls, parameters, acq_parameters):
-        return None
+        """Get hessian from single Ground Truth."""
+        return None  # KM_dot_vec_hess(parameters, acq_parameters.b, acq_parameters.td)
 
     # Optimized methods for Non-linear Least Squares
     @classmethod
     def get_mse_jacobian(cls, parameters, acq_parameters, signal_gt):
-        """Get jacobian of Mean Square Error from single Ground Truth."""
-        return sandix_optimized_mse_jacobian(parameters, acq_parameters, signal_gt)
+        """Get signal from single Ground Truth."""
+        return nexi_dot_optimized_mse_jacobian(parameters, acq_parameters.b, acq_parameters.td, signal_gt, acq_parameters.ndim)
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/sandix_rm.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/sandix_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     n_params = 7
     param_names = ["t_ex", "Di", "De", "f", "rs", "fs", "sigma"]
     classic_limits = np.array([[1, 150], [0.1, 3.5], [0.1, 3.5], [0.05, 0.95], [1, 30], [0.05, 0.5], [0, 100]])
     grid_search_nb_points = [7, 5, 5, 5, 5, 5]  # Optimal would be [12, 8, 5, 5, 5, 5], but it will depends on how much time your machine takes
     has_rician_mean_correction = True
     non_corrected_model = Sandix()
 
-    def __init__(self, param_lim=classic_limits, invert_tex=False):
+    def __init__(self, param_lim=classic_limits):
         super().__init__(name='SANDIX_Rice_Mean')
         self.param_lim = param_lim
-        self.invert_tex = False
         self.constraints = [self.constr_on_diffusivities]
 
     @staticmethod
     def constr_on_diffusivities(param):
         if np.array(param).ndim == 1:
             # Put Di>De
             if param[0] < param[1]:
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/acq_parameters.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/acq_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/mist_parameters.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/mist_parameters.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,36 +10,36 @@
         # number of parameters
         self.n_params = mist_model.n_params
         # parameter names
         self.names = mist_model.param_names
         # parameters
         self.param = param
 
-    def initialize_fixed_parameters(self, n_set, ground_truth_params):
-        # parameters
-        param = np.empty([n_set, self.n_params])
-        for param_index in range(self.n_params):
-            param[:, param_index] = np.ones(n_set) * ground_truth_params[param_index]
-        self.param = param
-        return param
-
     def initialize_random_parameters(self, n_set, microstruct_model):
         # parameters
-        param = np.empty([n_set, self.n_params])
+        param = np.zeros([n_set, self.n_params])
         for param_index in range(microstruct_model.n_params):
             param[:, param_index] = (
                 np.random.rand(n_set)
                 * (microstruct_model.param_lim[param_index][1] - microstruct_model.param_lim[param_index][0])
                 + microstruct_model.param_lim[param_index][0]
             )
         if microstruct_model.constraints is not None:
             for constr in microstruct_model.constraints:
+                normalized_param = constr(normalized_param)
                 param = constr(param)
+        # Compute the normalized parameters
+        normalized_param = np.zeros([n_set, self.n_params])
+        for param_index in range(microstruct_model.n_params):
+            if microstruct_model.param_lim[param_index][1] != microstruct_model.param_lim[param_index][0]:
+                normalized_param[:, param_index] = (
+                    param[:, param_index] - microstruct_model.param_lim[param_index][0]
+                ) / (microstruct_model.param_lim[param_index][1] - microstruct_model.param_lim[param_index][0])
         self.param = param
-        return param
+        return param, normalized_param
 
 
 class MIcroSTructureParametersException(Exception):
     """Handle exceptions related to microstructure parameters."""
 
     pass
```

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/parameters/save_parameters.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/parameters/save_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/rice_noise/rice_mean.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/rice_noise/rice_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/nls/gridsearch.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/nls/gridsearch.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/nls/nls.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/nls/nls.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/src/graymatter_swissknife/powderaverage/powderaverage.py` & `graymatter_swissknife-1.1.0/src/graymatter_swissknife/powderaverage/powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/generate_phantom.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/generate_phantom.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/test_estimate_model.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/test_estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/test_estimate_model_noiseless.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/test_estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/phantom.nii.gz` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/phantom.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/models/test_nexi_functions.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/models/test_nexi_functions.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/models/test_rician_mean.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/models/test_rician_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/tests/graymatter_swissknife/powderaverage/test_powderaverage.py` & `graymatter_swissknife-1.1.0/tests/graymatter_swissknife/powderaverage/test_powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/.gitignore` & `graymatter_swissknife-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/LICENSE` & `graymatter_swissknife-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.0.2/README.md` & `graymatter_swissknife-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Gray Matter Microstructure models estimator for gray matter diffusion MRI
+# Gray Matter Microstructure models estimator for diffusion MRI
 
 [![PyPI - Version](https://img.shields.io/pypi/v/graymatter_swissknife.svg)](https://pypi.org/project/graymatter_swissknife)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/graymatter_swissknife)](#)
 [![GitHub](https://img.shields.io/github/license/QuentinUhl/graymatter_swissknife)](#)
 [![GitHub top language](https://img.shields.io/github/languages/top/QuentinUhl/graymatter_swissknife?color=lightgray)](#)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graymatter_swissknife.svg)](https://pypi.org/project/graymatter_swissknife)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -51,24 +51,34 @@
 
 `lowb_noisemap_path`: The path to the noisemap calculated using only the small b-values (b < 2 ms/µm²) and Marchenko-Pastur principal component analysis (MP-PCA) denoising. This noisemap is used to calculate the signal-to-noise ratio (SNR) of the data.
 
 `out_path`: The folder where the estimated parameters will be saved as output.
 
 **Additional options:**
 
-`mask_path`: The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
+`mask_path` (Recommended): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
 
-`fixed_parameters`: Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
+`fixed_parameters` (Optional): Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
 
-`adjust_parameter_limits`: Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
+`adjust_parameter_limits` (Optional): Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
 
 `n_cores`: Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
 
 `debug`: Debug mode. The default is False.
 
+## Fast XGBoost Estimation:
+
+The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. To analyze large cohorts, we could recommend training an XGBoost model to learn the model on the given parameter limits, then applying this trained model to the entire cohort. To achieve this, we use the following arguments:
+
+`optimization_method`: To use XGBoost, set this setting to `'xgboost'`. The default is `'nls'`.
+
+`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it will be saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
+
+`retrain_xgboost` (Optional): Boolean to indicate if you wish to overwrite the model already trained and saved at the address indicated in xgboost_model_path. The default and recommended setting is False. The safest way is to delete the saved file yourself.
+
 ### Gray Matter microstructure models description from the Generalized Exchange Model
 
 ![](images/GM_models_from_GEM.png)
 
 ## Prerequisites
 
 ### Data Acquisition
```

### Comparing `graymatter_swissknife-1.0.2/pyproject.toml` & `graymatter_swissknife-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 dependencies = [
   "numpy",
   "nibabel",
   "tqdm",
   "joblib",
   "scipy",
   "coverage[toml]>=6.5",
-  "pytest"
+  "pytest",
+  "xgboost",
+  "scikit-learn"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `graymatter_swissknife-1.0.2/PKG-INFO` & `graymatter_swissknife-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graymatter_swissknife
-Version: 1.0.2
+Version: 1.1.0
 Summary: Gray Matter Swiss Knife : Generalized Exchange Model estimators for diffusion MRI
 Project-URL: Documentation, https://github.com/QuentinUhl/graymatter_swissknife#readme
 Project-URL: Issues, https://github.com/QuentinUhl/graymatter_swissknife/issues
 Project-URL: Source, https://github.com/QuentinUhl/graymatter_swissknife
 Author-email: Quentin Uhl <quentin.uhl@gmail.com>, "Ileana O. Jelescu" <ileana.jelescu@chuv.ch>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Gray Matter Microstructure models estimator for gray matter diffusion MRI
+# Gray Matter Microstructure models estimator for diffusion MRI
 
 [![PyPI - Version](https://img.shields.io/pypi/v/graymatter_swissknife.svg)](https://pypi.org/project/graymatter_swissknife)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/graymatter_swissknife)](#)
 [![GitHub](https://img.shields.io/github/license/QuentinUhl/graymatter_swissknife)](#)
 [![GitHub top language](https://img.shields.io/github/languages/top/QuentinUhl/graymatter_swissknife?color=lightgray)](#)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graymatter_swissknife.svg)](https://pypi.org/project/graymatter_swissknife)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -74,24 +74,34 @@
 
 `lowb_noisemap_path`: The path to the noisemap calculated using only the small b-values (b < 2 ms/µm²) and Marchenko-Pastur principal component analysis (MP-PCA) denoising. This noisemap is used to calculate the signal-to-noise ratio (SNR) of the data.
 
 `out_path`: The folder where the estimated parameters will be saved as output.
 
 **Additional options:**
 
-`mask_path`: The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
+`mask_path` (Recommended): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
 
-`fixed_parameters`: Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
+`fixed_parameters` (Optional): Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
 
-`adjust_parameter_limits`: Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
+`adjust_parameter_limits` (Optional): Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
 
 `n_cores`: Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
 
 `debug`: Debug mode. The default is False.
 
+## Fast XGBoost Estimation:
+
+The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. To analyze large cohorts, we could recommend training an XGBoost model to learn the model on the given parameter limits, then applying this trained model to the entire cohort. To achieve this, we use the following arguments:
+
+`optimization_method`: To use XGBoost, set this setting to `'xgboost'`. The default is `'nls'`.
+
+`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it will be saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
+
+`retrain_xgboost` (Optional): Boolean to indicate if you wish to overwrite the model already trained and saved at the address indicated in xgboost_model_path. The default and recommended setting is False. The safest way is to delete the saved file yourself.
+
 ### Gray Matter microstructure models description from the Generalized Exchange Model
 
 ![](images/GM_models_from_GEM.png)
 
 ## Prerequisites
 
 ### Data Acquisition
```

