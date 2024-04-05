# Comparing `tmp/rio_tiler-6.4.4.tar.gz` & `tmp/rio_tiler-6.4.5.tar.gz`

## Comparing `rio_tiler-6.4.4.tar` & `rio_tiler-6.4.5.tar`

### file list

```diff
@@ -1,241 +1,241 @@
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/__init__.py
--rw-r--r--   0        0        0     9755 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/colormap.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/constants.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/errors.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/expression.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/logger.py
--rw-r--r--   0        0        0    28243 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/py.typed
--rw-r--r--   0        0        0    21802 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/reader.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/tasks.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/types.py
--rw-r--r--   0        0        0    26514 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/utils.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/accent.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/accent_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/afmhot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/afmhot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/algae.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/algae_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/amp.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/amp_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/autumn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/autumn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/balance.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/balance_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/binary.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/binary_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/blues.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/blues_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bone.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bone_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/brbg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/brbg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/brg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/brg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bupu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bupu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bwr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/bwr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cfastie.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cividis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cividis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cmrmap.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cmrmap_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cool.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cool_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/coolwarm.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/coolwarm_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/copper.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/copper_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cubehelix.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/cubehelix_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/curl.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/curl_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/dark2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/dark2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/deep.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/deep_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/delta.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/delta_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/dense.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/dense_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/diff.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/diff_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/flag.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/flag_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_earth.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_earth_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_heat.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_heat_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_ncar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_ncar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_stern.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_stern_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_yarg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gist_yarg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/greens.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/greens_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/greys.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/greys_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/haline.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/haline_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/hot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/hot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/hsv.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/hsv_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ice.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ice_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/inferno.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/inferno_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/jet.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/jet_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/magma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/magma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/matter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/matter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/nipy_spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/nipy_spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ocean.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ocean_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/oranges.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/oranges_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/orrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/orrd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/oxy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/oxy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/paired.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/paired_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pastel1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pastel1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pastel2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pastel2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/phase.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/phase_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pink.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pink_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/piyg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/piyg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/plasma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/plasma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/prgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/prgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/prism.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/prism_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pubu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pubu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pubugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/pubugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/puor.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/puor_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/purd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/purd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/purples.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/purples_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdgy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdgy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdpu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdpu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdylbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdylbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rdylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/reds.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/reds_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/rplumbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/schwarzwald.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/seismic.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/seismic_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set3.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/set3_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/solar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/solar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/speed.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/speed_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/spring.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/spring_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/summer.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/summer_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab10.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab10_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20b.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20b_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20c.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tab20c_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tarn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tarn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tempo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/tempo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/terrain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/terrain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/thermal.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/thermal_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/topo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/topo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/turbid.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/turbid_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/turbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/turbo_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/twilight.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_shifted.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_shifted_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/viridis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/viridis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/winter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/winter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/wistia.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/wistia_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylgnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylgnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylorbr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylorbr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylorrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/cmap_data/ylorrd_r.npy
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/io/__init__.py
--rw-r--r--   0        0        0    45260 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/io/base.py
--rw-r--r--   0        0        0    32184 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/io/rasterio.py
--rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/io/stac.py
--rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/io/xarray.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/mosaic/__init__.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/mosaic/reader.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/mosaic/methods/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/mosaic/methods/base.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/rio_tiler/mosaic/methods/defaults.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/.gitignore
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/AUTHORS.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/LICENSE
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/README.md
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/pyproject.toml
--rw-r--r--   0        0        0    11869 2020-02-02 00:00:00.000000 rio_tiler-6.4.4/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/__init__.py
+-rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/colormap.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/constants.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/errors.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/expression.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/logger.py
+-rw-r--r--   0        0        0    28149 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/py.typed
+-rw-r--r--   0        0        0    21610 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/reader.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/tasks.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/types.py
+-rw-r--r--   0        0        0    26532 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/utils.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/accent.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/accent_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/afmhot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/afmhot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/algae.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/algae_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/amp.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/amp_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/autumn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/autumn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/balance.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/balance_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/binary.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/binary_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/blues.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/blues_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bone.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bone_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/brbg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/brbg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/brg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/brg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bupu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bupu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bwr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/bwr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cfastie.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cividis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cividis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cmrmap.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cmrmap_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cool.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cool_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/coolwarm.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/coolwarm_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/copper.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/copper_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cubehelix.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/cubehelix_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/curl.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/curl_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/dark2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/dark2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/deep.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/deep_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/delta.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/delta_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/dense.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/dense_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/diff.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/diff_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/flag.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/flag_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_earth.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_earth_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_heat.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_heat_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_ncar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_ncar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_stern.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_stern_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_yarg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gist_yarg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/greens.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/greens_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/greys.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/greys_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/haline.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/haline_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/hot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/hot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/hsv.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/hsv_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ice.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ice_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/inferno.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/inferno_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/jet.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/jet_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/magma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/magma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/matter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/matter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/nipy_spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/nipy_spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ocean.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ocean_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/oranges.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/oranges_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/orrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/orrd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/oxy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/oxy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/paired.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/paired_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pastel1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pastel1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pastel2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pastel2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/phase.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/phase_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pink.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pink_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/piyg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/piyg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/plasma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/plasma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/prgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/prgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/prism.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/prism_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pubu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pubu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pubugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/pubugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/puor.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/puor_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/purd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/purd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/purples.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/purples_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdgy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdgy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdpu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdpu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdylbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdylbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rdylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/reds.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/reds_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/rplumbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/schwarzwald.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/seismic.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/seismic_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set3.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/set3_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/solar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/solar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/speed.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/speed_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/spring.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/spring_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/summer.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/summer_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab10.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab10_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20b.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20b_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20c.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tab20c_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tarn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tarn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tempo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/tempo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/terrain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/terrain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/thermal.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/thermal_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/topo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/topo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/turbid.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/turbid_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/turbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/turbo_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/twilight.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_shifted.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_shifted_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/viridis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/viridis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/winter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/winter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/wistia.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/wistia_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylgnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylgnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylorbr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylorbr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylorrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/cmap_data/ylorrd_r.npy
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/io/__init__.py
+-rw-r--r--   0        0        0    45246 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/io/base.py
+-rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/io/rasterio.py
+-rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/io/stac.py
+-rw-r--r--   0        0        0    17756 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/io/xarray.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/mosaic/__init__.py
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/mosaic/reader.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/mosaic/methods/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/mosaic/methods/base.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/rio_tiler/mosaic/methods/defaults.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/.gitignore
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/AUTHORS.txt
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/LICENSE
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/README.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/pyproject.toml
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 rio_tiler-6.4.5/PKG-INFO
```

### Comparing `rio_tiler-6.4.4/rio_tiler/colormap.py` & `rio_tiler-6.4.5/rio_tiler/colormap.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     # Try backported to PY<39 `importlib_resources`.
     from importlib_resources import files as resources_files  # type: ignore
 
 
 EMPTY_COLORMAP: GDALColorMapType = {i: (0, 0, 0, 0) for i in range(256)}
 
 DEFAULT_CMAPS_FILES = {
-    f.stem: str(f) for f in (resources_files(__package__) / "cmap_data").glob("*.npy")  # type: ignore
+    f.stem: str(f)
+    for f in (resources_files(__package__) / "cmap_data").glob("*.npy")  # type: ignore
 }
 
 USER_CMAPS_DIR = os.environ.get("COLORMAP_DIRECTORY", None)
 if USER_CMAPS_DIR:
     DEFAULT_CMAPS_FILES.update(
         {f.stem: str(f) for f in pathlib.Path(USER_CMAPS_DIR).glob("*.npy")}
     )
@@ -119,17 +120,15 @@
     # we cast the output array to Uint8.
     if data.min() >= 0 and data.max() <= 255:
         data = data.astype("uint8")
 
     return data[:-1], data[-1]
 
 
-def apply_discrete_cmap(
-    data: numpy.ndarray, colormap: GDALColorMapType
-) -> DataMaskType:
+def apply_discrete_cmap(data: numpy.ndarray, colormap: GDALColorMapType) -> DataMaskType:
     """Apply discrete colormap.
 
     Args:
         data (numpy.ndarray): 1D image array to translate to RGB.
         color_map (dict): Discrete ColorMap dictionary.
 
     Returns:
@@ -185,15 +184,15 @@
 
             data, mask = apply_intervals_cmap(data, cmap)
             assert data.shape == (3, 256, 256)
 
     """
     res = numpy.zeros((data.shape[1], data.shape[2], 4), dtype=numpy.uint8)
 
-    for (k, v) in colormap:
+    for k, v in colormap:
         res[(data[0] >= k[0]) & (data[0] < k[1])] = numpy.array(v)
 
     data = numpy.transpose(res, [2, 0, 1])
 
     # If the output data has values between 0-255
     # we cast the output array to Uint8
     if data.min() >= 0 and data.max() <= 255:
@@ -247,15 +246,17 @@
                 r"$"
             )
         else:
             raise InvalidColorFormat(f"Invalid color format: {rgba}")
 
         match = re.match(hex_pattern, rgba)
         rgba = [
-            int(n * factor, 16) for n in match.groupdict().values() if n is not None  # type: ignore
+            int(n * factor, 16)
+            for n in match.groupdict().values()
+            if n is not None  # type: ignore
         ]
 
     if len(rgba) > 4 or len(rgba) < 3:
         raise InvalidColorFormat(f"Invalid color format: {rgba}")
 
     rgba = tuple(rgba)
     if len(rgba) == 3:
```

### Comparing `rio_tiler-6.4.4/rio_tiler/errors.py` & `rio_tiler-6.4.5/rio_tiler/errors.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/expression.py` & `rio_tiler-6.4.5/rio_tiler/expression.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/models.py` & `rio_tiler-6.4.5/rio_tiler/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             data (sequence): sequence of PointData.
 
         """
         if not data:
             raise InvalidPointDataError("Empty PointData list.")
 
         # validate coordinates
-        if all([pt.coordinates or pt.crs or None for pt in data]):
+        if all(pt.coordinates or pt.crs or None for pt in data):
             lon, lat, crs = zip(*[(*(pt.coordinates or []), pt.crs) for pt in data])
             if len(set(lon)) > 1 or len(set(lat)) > 1 or len(set(crs)) > 1:
                 raise InvalidPointDataError(
                     "Cannot concatenate points with different coordinates/CRS."
                 )
 
         arr = numpy.ma.concatenate([pt.array for pt in data])
@@ -241,17 +241,15 @@
         assets = list(
             dict.fromkeys(
                 itertools.chain.from_iterable([pt.assets for pt in data if pt.assets])
             )
         )
 
         band_names = list(
-            itertools.chain.from_iterable(
-                [pt.band_names for pt in data if pt.band_names]
-            )
+            itertools.chain.from_iterable([pt.band_names for pt in data if pt.band_names])
         )
 
         metadata = dict(
             itertools.chain.from_iterable(
                 [pt.metadata.items() for pt in data if pt.metadata]
             )
         )
@@ -435,17 +433,15 @@
 
         """
         h, w = zip(*[(img.height, img.width) for img in data])
 
         # Get cutline mask at highest resolution.
         max_h, max_w = max(h), max(w)
         cutline_mask = next(
-            img.cutline_mask
-            for img in data
-            if img.height == max_h and img.width == max_w
+            img.cutline_mask for img in data if img.height == max_h and img.width == max_w
         )
 
         if len(set(h)) > 1 or len(set(w)) > 1:
             warnings.warn(
                 "Cannot concatenate images with different size. Will resize using max width/heigh",
                 UserWarning,
             )
@@ -458,17 +454,15 @@
                 )
                 img.array = arr
 
         arr = numpy.ma.concatenate([img.array for img in data])
 
         assets = list(
             dict.fromkeys(
-                itertools.chain.from_iterable(
-                    [img.assets for img in data if img.assets]
-                )
+                itertools.chain.from_iterable([img.assets for img in data if img.assets])
             )
         )
 
         bounds_values = [img.bounds for img in data if img.bounds]
         bounds = bounds_values[0] if bounds_values else None
 
         crs_values = [img.crs for img in data if img.crs]
@@ -623,17 +617,17 @@
         self,
         height: int,
         width: int,
         resampling_method: RIOResampling = "nearest",
     ) -> "ImageData":
         """Resize data and mask."""
         data = resize_array(self.array.data, height, width, resampling_method)
-        mask = resize_array(
-            self.array.mask * 1, height, width, resampling_method
-        ).astype("bool")
+        mask = resize_array(self.array.mask * 1, height, width, resampling_method).astype(
+            "bool"
+        )
 
         return ImageData(
             numpy.ma.MaskedArray(data, mask=mask),
             assets=self.assets,
             crs=self.crs,
             bounds=self.bounds,
             band_names=self.band_names,
```

### Comparing `rio_tiler-6.4.4/rio_tiler/profiles.py` & `rio_tiler-6.4.5/rio_tiler/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/reader.py` & `rio_tiler-6.4.5/rio_tiler/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """rio-tiler.reader: low level reader."""
 
 import contextlib
 import math
 import warnings
-from enum import IntEnum
 from typing import Callable, Dict, Optional, Tuple, TypedDict, Union
 
 import numpy
 from affine import Affine
 from rasterio import windows
 from rasterio.crs import CRS
-from rasterio.enums import ColorInterp, MaskFlags, Resampling
+from rasterio.enums import ColorInterp, Resampling
 from rasterio.io import DatasetReader, DatasetWriter
 from rasterio.transform import array_bounds
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import transform as transform_coords
 from rasterio.warp import transform_bounds
 
 from rio_tiler.constants import WGS84_CRS
@@ -93,17 +92,15 @@
     window: Optional[windows.Window] = None,
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
     resampling_method: RIOResampling = "nearest",
     reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
-    post_process: Optional[
-        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
-    ] = None,
+    post_process: Optional[Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]] = None,
 ) -> ImageData:
     """Low level read function.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         dst_crs (rasterio.crs.CRS, optional): Target coordinate reference system.
         height (int, optional): Output height of the image.
@@ -192,17 +189,15 @@
 
             # Read Data and Mask separately
             # Special case (see https://github.com/rasterio/rasterio/issues/2798)
             if dataset.dtypes[alpha_idx - 1] != dataset.dtypes[indexes[0] - 1]:
                 values = dataset.read(
                     indexes=indexes,
                     window=window,
-                    out_shape=(len(indexes), height, width)
-                    if height and width
-                    else None,
+                    out_shape=(len(indexes), height, width) if height and width else None,
                     resampling=io_resampling,
                     boundless=boundless,
                 )
                 mask = dataset.read(
                     indexes=(alpha_idx,),
                     window=window,
                     out_shape=(1, height, width) if height and width else None,
@@ -242,17 +237,15 @@
                     data.mask = numpy.isnan(data.data)
                 else:
                     data.mask = data.data == nodata
 
         stats = []
         for ix in indexes:
             tags = dataset.tags(ix)
-            if all(
-                stat in tags for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]
-            ):
+            if all(stat in tags for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]):
                 stat_min = float(tags.get("STATISTICS_MINIMUM"))
                 stat_max = float(tags.get("STATISTICS_MAXIMUM"))
                 stats.append((stat_min, stat_max))
 
         # We only add dataset statistics if we have them for all the indexes
         dataset_statistics = stats if len(stats) == len(indexes) else None
 
@@ -298,17 +291,15 @@
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
     align_bounds_with_dataset: bool = False,
     resampling_method: RIOResampling = "nearest",
     reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
-    post_process: Optional[
-        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
-    ] = None,
+    post_process: Optional[Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]] = None,
 ) -> ImageData:
     """Read part of a dataset.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         bounds (tuple): Output bounds (left, bottom, right, top). By default the coordinates are considered to be in either the dataset CRS or in the `dst_crs` if set. Use `bounds_crs` to set a specific CRS.
         height (int, optional): Output height of the image.
@@ -348,20 +339,16 @@
     if bounds_crs and bounds_crs != dst_crs:
         bounds = transform_bounds(bounds_crs, dst_crs, *bounds, densify_pts=21)
 
     if minimum_overlap:
         src_bounds = transform_bounds(
             src_dst.crs, dst_crs, *src_dst.bounds, densify_pts=21
         )
-        x_overlap = max(
-            0, min(src_bounds[2], bounds[2]) - max(src_bounds[0], bounds[0])
-        )
-        y_overlap = max(
-            0, min(src_bounds[3], bounds[3]) - max(src_bounds[1], bounds[1])
-        )
+        x_overlap = max(0, min(src_bounds[2], bounds[2]) - max(src_bounds[0], bounds[0]))
+        y_overlap = max(0, min(src_bounds[3], bounds[3]) - max(src_bounds[1], bounds[1]))
         cover_ratio = (x_overlap * y_overlap) / (
             (bounds[2] - bounds[0]) * (bounds[3] - bounds[1])
         )
 
         if cover_ratio < minimum_overlap:
             raise TileOutsideBounds(
                 "Dataset covers less than {:.0f}% of tile".format(cover_ratio * 100)
@@ -496,17 +483,15 @@
     coord_crs: CRS = WGS84_CRS,
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
     resampling_method: RIOResampling = "nearest",
     reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
-    post_process: Optional[
-        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
-    ] = None,
+    post_process: Optional[Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]] = None,
 ) -> PointData:
     """Read a pixel value for a point.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         coordinates (tuple): Coordinates in form of (X, Y).
         indexes (sequence of int or int, optional): Band indexes.
```

### Comparing `rio_tiler-6.4.4/rio_tiler/tasks.py` & `rio_tiler-6.4.5/rio_tiler/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Yields:
         Task results.
 
     """
     if allowed_exceptions is None:
         allowed_exceptions = ()
 
-    for (future, asset) in tasks:
+    for future, asset in tasks:
         try:
             if isinstance(future, futures.Future):
                 yield future.result(), asset
             else:
                 yield future(), asset
         except allowed_exceptions as err:
             logger.info(err)
@@ -48,17 +48,15 @@
         with futures.ThreadPoolExecutor(max_workers=threads) as executor:
             return [
                 (executor.submit(reader, asset, *args, **kwargs), asset)
                 for asset in asset_list
             ]
     else:
         logger.debug(f"Running tasks outside ThreadsPool (max_workers={threads})")
-        return [
-            (partial(reader, asset, *args, **kwargs), asset) for asset in asset_list
-        ]
+        return [(partial(reader, asset, *args, **kwargs), asset) for asset in asset_list]
 
 
 def multi_arrays(
     asset_list: Sequence,
     reader: Callable[..., ImageData],
     *args: Any,
     threads: int = MAX_THREADS,
```

### Comparing `rio_tiler-6.4.4/rio_tiler/types.py` & `rio_tiler-6.4.5/rio_tiler/types.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/utils.py` & `rio_tiler-6.4.5/rio_tiler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,17 +108,20 @@
     if len(data.shape) < 3:
         data = numpy.ma.expand_dims(data, axis=0)
 
     output: List[Dict[Any, Any]] = []
     percentiles_names = [f"percentile_{int(p)}" for p in percentiles]
 
     if coverage is not None:
-        assert coverage.shape == (
-            data.shape[1],
-            data.shape[2],
+        assert (
+            coverage.shape
+            == (
+                data.shape[1],
+                data.shape[2],
+            )
         ), f"Invalid shape ({coverage.shape}) for Coverage, expected {(data.shape[1], data.shape[2])}"
 
     else:
         coverage = numpy.ones((data.shape[1], data.shape[2]))
 
     # Avoid non masked nan/inf values
     numpy.ma.fix_invalid(data, copy=False)
@@ -391,28 +394,26 @@
 
     return vrt_transform, vrt_width, vrt_height
 
 
 def has_alpha_band(src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT]) -> bool:
     """Check for alpha band or mask in source."""
     if (
-        any([MaskFlags.alpha in flags for flags in src_dst.mask_flag_enums])
+        any(MaskFlags.alpha in flags for flags in src_dst.mask_flag_enums)
         or ColorInterp.alpha in src_dst.colorinterp
     ):
         return True
     return False
 
 
 def has_mask_band(src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT]) -> bool:
     """Check for mask band in source."""
     if any(
-        [
-            (MaskFlags.per_dataset in flags and MaskFlags.alpha not in flags)
-            for flags in src_dst.mask_flag_enums
-        ]
+        (MaskFlags.per_dataset in flags and MaskFlags.alpha not in flags)
+        for flags in src_dst.mask_flag_enums
     ):
         return True
     return False
 
 
 def non_alpha_indexes(src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT]) -> Tuple:
     """Return indexes of non-alpha bands."""
```

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/__init__.py` & `rio_tiler-6.4.5/rio_tiler/cmap_data/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/accent.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/accent.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/accent_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/accent_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/afmhot.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/afmhot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/afmhot_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/afmhot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/algae.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/algae.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/algae_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/algae_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/amp.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/amp.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/amp_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/amp_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/autumn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/autumn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/autumn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/autumn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/balance.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/balance.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/balance_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/balance_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/binary.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/binary.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/binary_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/binary_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/blues.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/blues.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/blues_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/blues_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bone.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bone.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bone_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bone_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/brbg.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/brbg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/brbg_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/brbg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/brg.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/brg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/brg_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/brg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bugn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bugn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bupu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bupu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bupu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bupu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bwr.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bwr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/bwr_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/bwr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cfastie.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cfastie.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cividis.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cividis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cividis_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cividis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cmrmap.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cmrmap.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cmrmap_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cmrmap_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cool.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cool.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cool_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cool_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/coolwarm.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/coolwarm.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/coolwarm_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/coolwarm_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/copper.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/copper.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/copper_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/copper_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cubehelix.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cubehelix.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/cubehelix_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/cubehelix_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/curl.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/curl.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/curl_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/curl_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/dark2.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/dark2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/dark2_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/dark2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/deep.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/deep.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/deep_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/deep_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/delta.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/delta.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/delta_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/delta_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/dense.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/dense.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/dense_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/dense_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/diff.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/diff.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/diff_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/diff_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/flag.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/flag.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/flag_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/flag_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_earth.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_earth.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_earth_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_earth_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_gray.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_gray_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_heat.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_heat.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_heat_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_heat_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_ncar.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_ncar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_ncar_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_ncar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_rainbow.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_rainbow_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_stern.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_stern.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_stern_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_stern_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_yarg.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_yarg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gist_yarg_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gist_yarg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnbu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnbu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot2.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot2_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gnuplot_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gnuplot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gray.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/gray_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/greens.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/greens.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/greens_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/greens_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/greys.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/greys.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/greys_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/greys_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/haline.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/haline.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/haline_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/haline_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/hot.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/hot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/hot_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/hot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/hsv.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/hsv.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/hsv_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/hsv_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ice.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ice.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ice_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ice_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/inferno.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/inferno.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/inferno_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/inferno_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/jet.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/jet.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/jet_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/jet_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/magma.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/magma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/magma_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/magma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/matter.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/matter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/matter_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/matter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/nipy_spectral.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/nipy_spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/nipy_spectral_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/nipy_spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ocean.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ocean.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ocean_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ocean_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/oranges.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/oranges.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/oranges_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/oranges_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/orrd.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/orrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/orrd_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/orrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/oxy.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/oxy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/oxy_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/oxy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/paired.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/paired.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/paired_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/paired_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pastel1.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pastel1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pastel1_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pastel1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pastel2.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pastel2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pastel2_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pastel2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/phase.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/phase.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/phase_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/phase_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pink.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pink.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pink_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pink_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/piyg.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/piyg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/piyg_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/piyg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/plasma.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/plasma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/plasma_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/plasma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/prgn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/prgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/prgn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/prgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/prism.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/prism.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/prism_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/prism_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pubu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pubu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pubu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pubu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pubugn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pubugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/pubugn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/pubugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/puor.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/puor.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/puor_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/puor_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/purd.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/purd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/purd_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/purd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/purples.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/purples.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/purples_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/purples_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rain.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rain_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rainbow.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rainbow_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdbu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdbu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdgy.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdgy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdgy_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdgy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdpu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdpu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdpu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdpu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdylbu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdylbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdylbu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdylbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdylgn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rdylgn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rdylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/reds.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/reds.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/reds_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/reds_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/rplumbo.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/rplumbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/schwarzwald.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/schwarzwald.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/seismic.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/seismic.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/seismic_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/seismic_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set1.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set1_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set2.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set2_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set3.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set3.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/set3_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/set3_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/solar.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/solar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/solar_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/solar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/spectral.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/spectral_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/speed.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/speed.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/speed_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/speed_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/spring.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/spring.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/spring_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/spring_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/summer.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/summer.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/summer_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/summer_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab10.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab10.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab10_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab10_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20b.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20b.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20b_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20b_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20c.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20c.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tab20c_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tab20c_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tarn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tarn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tarn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tarn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tempo.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tempo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/tempo_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/tempo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/terrain.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/terrain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/terrain_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/terrain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/thermal.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/thermal.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/thermal_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/thermal_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/topo.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/topo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/topo_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/topo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/turbid.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/turbid.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/turbid_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/turbid_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/turbo.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/turbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/turbo_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/turbo_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/twilight.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/twilight.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_shifted.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_shifted.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/twilight_shifted_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/twilight_shifted_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/viridis.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/viridis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/viridis_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/viridis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/winter.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/winter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/winter_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/winter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/wistia.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/wistia.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/wistia_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/wistia_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylgn.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylgn_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylgnbu.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylgnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylgnbu_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylgnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylorbr.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylorbr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylorbr_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylorbr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylorrd.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylorrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/cmap_data/ylorrd_r.npy` & `rio_tiler-6.4.5/rio_tiler/cmap_data/ylorrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/io/base.py` & `rio_tiler-6.4.5/rio_tiler/io/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,17 +897,15 @@
         if not bands:
             raise InvalidExpression(
                 f"Could not find any valid bands in '{expression}' expression."
             )
 
         return bands
 
-    def info(
-        self, bands: Union[Sequence[str], str] = None, *args, **kwargs: Any
-    ) -> Info:
+    def info(self, bands: Union[Sequence[str], str] = None, *args, **kwargs: Any) -> Info:
         """Return metadata from multiple bands.
 
         Args:
             bands (sequence of str or str, optional): band names to fetch info from. Required keyword argument.
 
         Returns:
             dict: Multiple bands info in form of {"band1": rio_tile.models.Info}.
```

### Comparing `rio_tiler-6.4.4/rio_tiler/io/rasterio.py` & `rio_tiler-6.4.5/rio_tiler/io/rasterio.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,17 +271,15 @@
                 {"scale": self.dataset.scales[0], "offset": self.dataset.offsets[0]}
             )
 
         if self.colormap:
             meta.update({"colormap": self.colormap})
 
         if nodata_type == "Nodata":
-            meta.update(
-                {"nodata_value": self.options.get("nodata", self.dataset.nodata)}
-            )
+            meta.update({"nodata_value": self.options.get("nodata", self.dataset.nodata)})
 
         return Info(**meta)
 
     def statistics(
         self,
         categorical: bool = False,
         categories: Optional[List[float]] = None,
```

### Comparing `rio_tiler-6.4.4/rio_tiler/io/stac.py` & `rio_tiler-6.4.5/rio_tiler/io/stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,17 +260,15 @@
                 include=self.include_assets,
                 exclude=self.exclude_assets,
                 include_asset_types=self.include_asset_types,
                 exclude_asset_types=self.exclude_asset_types,
             )
         )
         if not self.assets:
-            raise MissingAssets(
-                "No valid asset found. Asset's media types not supported"
-            )
+            raise MissingAssets("No valid asset found. Asset's media types not supported")
 
     @minzoom.default
     def _minzoom(self):
         return self.tms.minzoom
 
     @maxzoom.default
     def _maxzoom(self):
```

### Comparing `rio_tiler-6.4.4/rio_tiler/io/xarray.py` & `rio_tiler-6.4.5/rio_tiler/io/xarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """rio_tiler.io.xarray: Xarray Reader."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional
 
 import attr
 from morecantile import Tile, TileMatrixSet
@@ -227,17 +228,15 @@
             warnings.warn(
                 "`resampling_method` is deprecated and will be removed in rio-tiler 7.0, please use `reproject_method`",
                 DeprecationWarning,
             )
             reproject_method = resampling_method
 
         if not self.tile_exists(tile_x, tile_y, tile_z):
-            raise TileOutsideBounds(
-                f"Tile {tile_z}/{tile_x}/{tile_y} is outside bounds"
-            )
+            raise TileOutsideBounds(f"Tile {tile_z}/{tile_x}/{tile_y} is outside bounds")
 
         ds = self.input
         if nodata is not None:
             ds = ds.rio.write_nodata(nodata)
 
         tile_bounds = self.tms.xy_bounds(Tile(x=tile_x, y=tile_y, z=tile_z))
         dst_crs = self.tms.rasterio_crs
```

### Comparing `rio_tiler-6.4.4/rio_tiler/mosaic/reader.py` & `rio_tiler-6.4.5/rio_tiler/mosaic/reader.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/mosaic/methods/__init__.py` & `rio_tiler-6.4.5/rio_tiler/mosaic/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/mosaic/methods/base.py` & `rio_tiler-6.4.5/rio_tiler/mosaic/methods/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/rio_tiler/mosaic/methods/defaults.py` & `rio_tiler-6.4.5/rio_tiler/mosaic/methods/defaults.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/.gitignore` & `rio_tiler-6.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/LICENSE` & `rio_tiler-6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/README.md` & `rio_tiler-6.4.5/README.md`

 * *Files identical despite different names*

### Comparing `rio_tiler-6.4.4/pyproject.toml` & `rio_tiler-6.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "attrs",
     "cachetools",
     "httpx",
@@ -125,20 +126,27 @@
 ]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
 no_strict_optional = true
 
 [tool.ruff]
+line-length = 90
+
+[tool.ruff.lint]
 select = [
     "D1",  # pydocstyle errors
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # flake8
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
+    "B028",
 ]
+
+[tool.ruff.lint.mccabe]
+max-complexity = 14
```

### Comparing `rio_tiler-6.4.4/PKG-INFO` & `rio_tiler-6.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-tiler
-Version: 6.4.4
+Version: 6.4.5
 Summary: User friendly Rasterio plugin to read raster datasets.
 Project-URL: Homepage, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Documentation, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Issues, https://github.com/cogeotiff/rio-tiler/issues
 Project-URL: Source, https://github.com/cogeotiff/rio-tiler
 Project-URL: Changelog, https://cogeotiff.github.io/rio-tiler/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
@@ -43,14 +43,15 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: cachetools
 Requires-Dist: color-operations
 Requires-Dist: httpx
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
```

