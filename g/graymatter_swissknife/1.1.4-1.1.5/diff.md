# Comparing `tmp/graymatter_swissknife-1.1.4.tar.gz` & `tmp/graymatter_swissknife-1.1.5.tar.gz`

## Comparing `graymatter_swissknife-1.1.4.tar` & `graymatter_swissknife-1.1.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/images/GM_models_from_GEM.png
--rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/images/gm_swissknife_square_low_res.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/__main__.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/estimate_model.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/estimate_model_noiseless.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/find_model.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/microstructure_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/gem.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/gem_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/functions/__init__.py
--rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/__init__.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_dot.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_rm.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/smex.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/smex_rm.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/sandi.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/sandi_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/functions/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/sandix.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/acq_parameters.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/mist_parameters.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/save_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/rice_noise/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/rice_noise/rice_mean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/struct_functions/__init__.py
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/nls/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/nls/gridsearch.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/nls/nls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/powderaverage/__init__.py
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/powderaverage/powderaverage.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/define_xgboost_model.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/generate_dataset.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/generate_phantom.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/test_estimate_model.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/test_estimate_model_noiseless.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/mask.nii.gz
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/phantom.bval
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/phantom.nii.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/phantom.td
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/powderaverage_ref.bval
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/powderaverage_ref.td
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_sigma_ref.nii.gz
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/models/test_nexi_functions.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/models/test_rician_mean.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/LICENSE
--rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/README.md
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/images/GM_models_from_GEM.png
+-rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/images/gm_swissknife_square_low_res.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/__main__.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/estimate_model.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/estimate_model_noiseless.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/find_model.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/microstructure_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/gem.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/gem_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/functions/__init__.py
+-rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/__init__.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_dot.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_rm.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/smex.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/smex_rm.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/sandi.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/sandi_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/functions/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/sandix.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/acq_parameters.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/mist_parameters.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/save_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/rice_noise/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/rice_noise/rice_mean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/struct_functions/__init__.py
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/nls/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/nls/gridsearch.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/nls/nls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/powderaverage/__init__.py
+-rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/powderaverage/powderaverage.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/define_xgboost_model.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/generate_dataset.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/generate_phantom.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/test_estimate_model.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/test_estimate_model_noiseless.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/mask.nii.gz
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/phantom.bval
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/phantom.nii.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/phantom.td
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/powderaverage_ref.bval
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/powderaverage_ref.td
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_sigma_ref.nii.gz
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/models/test_nexi_functions.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/models/test_rician_mean.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/.gitignore
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/LICENSE
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.5/PKG-INFO
```

### Comparing `graymatter_swissknife-1.1.4/images/GM_models_from_GEM.png` & `graymatter_swissknife-1.1.5/images/GM_models_from_GEM.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/images/gm_swissknife_square_low_res.png` & `graymatter_swissknife-1.1.5/images/gm_swissknife_square_low_res.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/estimate_model.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/estimate_model_noiseless.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/find_model.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/find_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/microstructure_models.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/microstructure_models.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/gem.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/gem_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/gem_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_dot.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/nexi_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/nexi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/smex.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/smex_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/smex_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/sandi.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/sandi_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/sandi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/sandix.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/sandix_rm.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/sandix_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/acq_parameters.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/acq_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/mist_parameters.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/mist_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/parameters/save_parameters.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/parameters/save_parameters.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         mask = (mask > mask_threshold).astype(bool)
         mask = mask & (~np.isnan(powder_average))
     else:
         mask = ~np.isnan(powder_average)
     param_map_shape = mask.shape
 
     param_names = model.param_names
+    # Remove the last parameter (sigma) from the parameter names if the model has a Rician mean correction
+    if model.has_rician_mean_correction:
+        param_names = param_names[:-1]
     for i, param_name in enumerate(param_names):
         param_map = np.zeros(param_map_shape)
         param_map[mask] = estimations[:, i]
         param_map_nifti = nib.Nifti1Image(param_map, aff, hdr)
         if optimization_method == 'nls':
             nib.save(param_map_nifti, f'{out_path}/{model.name.lower()}_{param_name.lower()}.nii.gz')
             logging.info(f'{model.name.lower()}_{param_name.lower()}.nii.gz saved in {out_path}')
```

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/rice_noise/rice_mean.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/rice_noise/rice_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/nls/gridsearch.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/nls/gridsearch.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/nls/nls.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/nls/nls.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/powderaverage/powderaverage.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/powderaverage/powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/apply_xgboost_model.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/apply_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/define_xgboost_model.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/define_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/src/graymatter_swissknife/xgboost/generate_dataset.py` & `graymatter_swissknife-1.1.5/src/graymatter_swissknife/xgboost/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/generate_phantom.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/generate_phantom.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/test_estimate_model.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/test_estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/test_estimate_model_noiseless.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/test_estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/phantom.nii.gz` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/phantom.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/models/test_nexi_functions.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/models/test_nexi_functions.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/models/test_rician_mean.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/models/test_rician_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/powderaverage/test_powderaverage.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/powderaverage/test_powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/tests/graymatter_swissknife/xgboost/test_generate_dataset.py` & `graymatter_swissknife-1.1.5/tests/graymatter_swissknife/xgboost/test_generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/.gitignore` & `graymatter_swissknife-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/LICENSE` & `graymatter_swissknife-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/README.md` & `graymatter_swissknife-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/pyproject.toml` & `graymatter_swissknife-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.4/PKG-INFO` & `graymatter_swissknife-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graymatter_swissknife
-Version: 1.1.4
+Version: 1.1.5
 Summary: Gray Matter Swiss Knife : Generalized Exchange Model estimators for diffusion MRI
 Project-URL: Documentation, https://github.com/QuentinUhl/graymatter_swissknife#readme
 Project-URL: Issues, https://github.com/QuentinUhl/graymatter_swissknife/issues
 Project-URL: Source, https://github.com/QuentinUhl/graymatter_swissknife
 Author-email: Quentin Uhl <quentin.uhl@gmail.com>, "Ileana O. Jelescu" <ileana.jelescu@chuv.ch>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

