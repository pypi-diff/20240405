# Comparing `tmp/pandeia.engine-3.1.tar.gz` & `tmp/pandeia.engine-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandeia.engine-3.1.tar", last modified: Mon Dec 11 19:45:42 2023, max compression
+gzip compressed data, was "pandeia.engine-3.2.tar", last modified: Fri Apr  5 14:20:28 2024, max compression
```

## Comparing `pandeia.engine-3.1.tar` & `pandeia.engine-3.2.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:42.008201 pandeia.engine-3.1/
--rw-r--r--   0 riedel    (1525)     1031      125 2022-12-08 20:06:08.000000 pandeia.engine-3.1/MANIFEST.in
--rw-r--r--   0 riedel    (1525)     1031     2221 2023-12-11 19:45:42.007590 pandeia.engine-3.1/PKG-INFO
--rw-r--r--   0 riedel    (1525)     1031     1218 2022-11-17 18:41:23.000000 pandeia.engine-3.1/README.md
--rwxr-xr-x   0 riedel    (1525)     1031       62 2022-10-04 19:20:08.000000 pandeia.engine-3.1/clean
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.808946 pandeia.engine-3.1/pandeia/
--rw-r--r--   0 riedel    (1525)     1031      181 2022-10-04 19:20:08.000000 pandeia.engine-3.1/pandeia/__init__.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.851582 pandeia.engine-3.1/pandeia/engine/
--rw-r--r--   0 riedel    (1525)     1031     1509 2022-10-04 19:20:08.000000 pandeia.engine-3.1/pandeia/engine/LICENSE.rst
--rw-r--r--   0 riedel    (1525)     1031     1933 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/__init__.py
--rw-r--r--   0 riedel    (1525)     1031    62923 2023-11-14 22:34:23.000000 pandeia.engine-3.1/pandeia/engine/astro_spectrum.py
--rw-r--r--   0 riedel    (1525)     1031    11639 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/background.py
--rw-r--r--   0 riedel    (1525)     1031     2787 2023-03-01 18:51:17.000000 pandeia.engine-3.1/pandeia/engine/bnc.py
--rw-r--r--   0 riedel    (1525)     1031    12673 2023-06-30 17:11:56.000000 pandeia.engine-3.1/pandeia/engine/calc_utils.py
--rw-r--r--   0 riedel    (1525)     1031     8969 2023-07-06 20:11:51.000000 pandeia.engine-3.1/pandeia/engine/config.py
--rw-r--r--   0 riedel    (1525)     1031     4247 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/constants.py
--rw-r--r--   0 riedel    (1525)     1031    22864 2023-08-24 16:33:27.000000 pandeia.engine-3.1/pandeia/engine/coords.py
--rw-r--r--   0 riedel    (1525)     1031    10514 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/custom_exceptions.py
--rw-r--r--   0 riedel    (1525)     1031     9702 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/debug_utils.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.855207 pandeia.engine-3.1/pandeia/engine/defaults/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-04 19:20:08.000000 pandeia.engine-3.1/pandeia/engine/defaults/__init__.py
--rw-r--r--   0 riedel    (1525)     1031      353 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/defaults/background_defaults.json
--rw-r--r--   0 riedel    (1525)     1031      219 2022-11-17 18:41:23.000000 pandeia.engine-3.1/pandeia/engine/defaults/calculationconfig_defaults.json
--rw-r--r--   0 riedel    (1525)     1031      311 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/defaults/insconfig_defaults.json
--rw-r--r--   0 riedel    (1525)     1031       50 2022-10-04 19:20:08.000000 pandeia.engine-3.1/pandeia/engine/defaults/observation_defaults.json
--rw-r--r--   0 riedel    (1525)     1031    66402 2023-11-30 20:16:22.000000 pandeia.engine-3.1/pandeia/engine/detector.py
--rw-r--r--   0 riedel    (1525)     1031     1136 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/detector_factory.py
--rw-r--r--   0 riedel    (1525)     1031    21209 2023-07-06 20:11:51.000000 pandeia.engine-3.1/pandeia/engine/etc3D.py
--rw-r--r--   0 riedel    (1525)     1031    15562 2023-11-15 18:31:14.000000 pandeia.engine-3.1/pandeia/engine/exposure.py
--rw-r--r--   0 riedel    (1525)     1031     1496 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/exposure_factory.py
--rw-r--r--   0 riedel    (1525)     1031    15074 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/extinction.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.857560 pandeia.engine-3.1/pandeia/engine/helpers/
--rw-r--r--   0 riedel    (1525)     1031       23 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia/engine/helpers/DEVBUILD
--rw-r--r--   0 riedel    (1525)     1031      140 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/README.md
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-04 19:20:08.000000 pandeia.engine-3.1/pandeia/engine/helpers/__init__.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.858655 pandeia.engine-3.1/pandeia/engine/helpers/background/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     6633 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/butler.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.865339 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/__init__.py
--rw-r--r--   0 riedel    (1525)     1031      599 2023-03-15 15:26:19.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky.dat
--rw-r--r--   0 riedel    (1525)     1031    11152 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky.py
--rw-r--r--   0 riedel    (1525)     1031     6595 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky_angles.py
--rw-r--r--   0 riedel    (1525)     1031     1238 2023-03-31 18:46:41.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky_spectrum.py
--rw-r--r--   0 riedel    (1525)     1031     3909 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/util.py
--rw-r--r--   0 riedel    (1525)     1031     3928 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/hst/zodi.dat
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.871519 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     2853 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/accessor_globals.py
--rw-r--r--   0 riedel    (1525)     1031     2030 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/bmg_accessor.py
--rw-r--r--   0 riedel    (1525)     1031     2799 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/mod_healpix_func.py
--rwxr-xr-x   0 riedel    (1525)     1031     7648 2022-10-05 18:17:23.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/sl_accessor_funcs.py
--rw-r--r--   0 riedel    (1525)     1031      203 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/straylight_accessor.py
--rw-r--r--   0 riedel    (1525)     1031      148 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/thermal_accessor.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.885417 pandeia.engine-3.1/pandeia/engine/helpers/bit/
--rw-r--r--   0 riedel    (1525)     1031      986 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/README.md
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/__init__.py
--rwxr-xr-x   0 riedel    (1525)     1031    16191 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/bit.py
--rwxr-xr-x   0 riedel    (1525)     1031     3999 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/bit_regenerate_pweb_peng_jeng.py
--rwxr-xr-x   0 riedel    (1525)     1031     4534 2023-01-20 21:31:05.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/bit_test_query_to_peng.py
--rw-r--r--   0 riedel    (1525)     1031     6612 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/compute.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.896434 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-12-08 20:06:08.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/__init__.py
--rw-r--r--   0 riedel    (1525)     1031      568 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/acs_sbc.dict
--rw-r--r--   0 riedel    (1525)     1031      823 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/acs_wfc.dict
--rw-r--r--   0 riedel    (1525)     1031      499 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/cos_fuv.dict
--rw-r--r--   0 riedel    (1525)     1031      468 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/cos_nuv.dict
--rw-r--r--   0 riedel    (1525)     1031     1072 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/global.dict
--rw-r--r--   0 riedel    (1525)     1031      667 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_ccd.dict
--rw-r--r--   0 riedel    (1525)     1031     1330 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_fuv-mama.dict
--rw-r--r--   0 riedel    (1525)     1031     1265 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_nuv-mama.dict
--rw-r--r--   0 riedel    (1525)     1031      134 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/wfc3_ir.dict
--rw-r--r--   0 riedel    (1525)     1031     1742 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/config/wfc3_uvis.dict
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.898285 pandeia.engine-3.1/pandeia/engine/helpers/bit/etc_web_data/
--rw-r--r--   0 riedel    (1525)     1031     1218 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/etc_web_data/extraction.dat
--rw-r--r--   0 riedel    (1525)     1031    27982 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/etc_web_data/targets.dat
--rw-r--r--   0 riedel    (1525)     1031    10770 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/extraction.py
--rw-r--r--   0 riedel    (1525)     1031    47385 2022-12-08 20:06:08.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/input_conversion.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.902890 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/
--rw-r--r--   0 riedel    (1525)     1031      971 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/README
--rw-r--r--   0 riedel    (1525)     1031     6105 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     4740 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/custom_configuration.py
--rw-r--r--   0 riedel    (1525)     1031     5419 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/data.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.905782 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/
--rw-r--r--   0 riedel    (1525)     1031      708 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/__init__.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.913717 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/
--rw-r--r--   0 riedel    (1525)     1031      659 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/__init__.py
--rw-r--r--   0 riedel    (1525)     1031    33090 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_aperture_fraction.dat
--rw-r--r--   0 riedel    (1525)     1031    11364 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_config.dat
--rw-r--r--   0 riedel    (1525)     1031     1431 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     7561 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_limits.py
--rw-r--r--   0 riedel    (1525)     1031     2990 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_sharpness.dat
--rw-r--r--   0 riedel    (1525)     1031     1320 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/detector_config.dat
--rw-r--r--   0 riedel    (1525)     1031      836 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/instr_functions.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.919964 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     1055 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     9807 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_web.py
--rw-r--r--   0 riedel    (1525)     1031     1503 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_coronography.py
--rw-r--r--   0 riedel    (1525)     1031     1724 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_imaging.py
--rw-r--r--   0 riedel    (1525)     1031     1518 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampcoronography.py
--rw-r--r--   0 riedel    (1525)     1031     1735 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampfilter.py
--rw-r--r--   0 riedel    (1525)     1031     1530 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_spectroscopic.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.926823 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/
--rw-r--r--   0 riedel    (1525)     1031      768 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/__init__.py
--rw-r--r--   0 riedel    (1525)     1031    17734 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_aperture_fraction.dat
--rw-r--r--   0 riedel    (1525)     1031     4001 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_config.dat
--rw-r--r--   0 riedel    (1525)     1031     2182 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     7246 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_limits.py
--rw-r--r--   0 riedel    (1525)     1031     3938 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/custom_config.dat
--rw-r--r--   0 riedel    (1525)     1031     2888 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/detector_config.dat
--rw-r--r--   0 riedel    (1525)     1031    37744 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/instr_functions.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.932413 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     1573 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     3591 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_web.py
--rw-r--r--   0 riedel    (1525)     1031     1781 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_imaging.py
--rw-r--r--   0 riedel    (1525)     1031     1621 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopic.py
--rw-r--r--   0 riedel    (1525)     1031     1647 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopicacq.py
--rw-r--r--   0 riedel    (1525)     1031     1392 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_targetacquisition.py
--rw-r--r--   0 riedel    (1525)     1031      565 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/default.py
--rw-r--r--   0 riedel    (1525)     1031     3148 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/scan_mode.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.939886 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/
--rw-r--r--   0 riedel    (1525)     1031      705 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     3944 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/detector_config.dat
--rw-r--r--   0 riedel    (1525)     1031    22864 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/instr_functions.py
--rw-r--r--   0 riedel    (1525)     1031    30096 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_aperture_fraction.dat
--rw-r--r--   0 riedel    (1525)     1031    13879 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_config.dat
--rw-r--r--   0 riedel    (1525)     1031     1914 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     8214 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_limits.py
--rw-r--r--   0 riedel    (1525)     1031     2281 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_sharpness.dat
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.944187 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     1743 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_imaging.py
--rw-r--r--   0 riedel    (1525)     1031     1967 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_spectroscopic.py
--rw-r--r--   0 riedel    (1525)     1031     1477 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_targetacquisition.py
--rw-r--r--   0 riedel    (1525)     1031      907 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     7284 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_web.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.950631 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/
--rw-r--r--   0 riedel    (1525)     1031      642 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/__init__.py
--rw-r--r--   0 riedel    (1525)     1031      739 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/detector_config.dat
--rw-r--r--   0 riedel    (1525)     1031     2286 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/instr_functions.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.954840 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     1655 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_imaging.py
--rw-r--r--   0 riedel    (1525)     1031     1780 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scimaging.py
--rw-r--r--   0 riedel    (1525)     1031     1581 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scspectroscopic.py
--rw-r--r--   0 riedel    (1525)     1031     1456 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_spectroscopic.py
--rw-r--r--   0 riedel    (1525)     1031      799 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     2587 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_web.py
--rw-r--r--   0 riedel    (1525)     1031    20541 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_aperture_fraction.dat
--rw-r--r--   0 riedel    (1525)     1031     2140 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_config.dat
--rw-r--r--   0 riedel    (1525)     1031     1037 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     4342 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_limits.py
--rw-r--r--   0 riedel    (1525)     1031     1059 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_sharpness.dat
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.962162 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/
--rw-r--r--   0 riedel    (1525)     1031      652 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/__init__.py
--rw-r--r--   0 riedel    (1525)     1031      906 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/detector_config.dat
--rw-r--r--   0 riedel    (1525)     1031     1422 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/instr_functions.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:41.966095 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     1753 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_imaging.py
--rw-r--r--   0 riedel    (1525)     1031     1878 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_scimaging.py
--rw-r--r--   0 riedel    (1525)     1031     1421 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_spectroscopic.py
--rw-r--r--   0 riedel    (1525)     1031      745 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     2587 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_web.py
--rw-r--r--   0 riedel    (1525)     1031   210674 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_aperture_fraction.dat
--rw-r--r--   0 riedel    (1525)     1031     6778 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_config.dat
--rw-r--r--   0 riedel    (1525)     1031      951 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_extraction_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     4946 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_limits.py
--rw-r--r--   0 riedel    (1525)     1031     1736 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_sharpness.dat
--rw-r--r--   0 riedel    (1525)     1031      669 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/telescopes.py
--rw-r--r--   0 riedel    (1525)     1031     9891 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/perform_calculation.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:42.001967 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/
--rw-r--r--   0 riedel    (1525)     1031     2695 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/README
--rw-r--r--   0 riedel    (1525)     1031     2677 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/__init__.py
--rw-r--r--   0 riedel    (1525)     1031     2147 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    17768 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2152 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    17200 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1959 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    15460 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2197 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    16270 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2085 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    16647 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2050 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    16826 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1785 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031    14502 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1144 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/map
--rw-r--r--   0 riedel    (1525)     1031     1108 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     4094 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1114 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     3931 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1141 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     4591 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1141 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_defaults.dat
--rw-r--r--   0 riedel    (1525)     1031     4100 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1123 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/options_map
--rw-r--r--   0 riedel    (1525)     1031     2164 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    17315 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2490 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    23797 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1881 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    15077 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2051 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    16985 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1894 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    14921 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1868 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    14575 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1816 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    14573 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2183 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    18490 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     2021 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    16423 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     1780 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_default_input.dat
--rw-r--r--   0 riedel    (1525)     1031    14839 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_form_options.dat
--rw-r--r--   0 riedel    (1525)     1031     7634 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_util.py
--rw-r--r--   0 riedel    (1525)     1031    11469 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/sky.py
--rw-r--r--   0 riedel    (1525)     1031    16404 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/source.py
--rw-r--r--   0 riedel    (1525)     1031     2097 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/string_constants.py
--rw-r--r--   0 riedel    (1525)     1031    10372 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/helpers/bit/translate.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:42.003510 pandeia.engine-3.1/pandeia/engine/helpers/peng/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-05 18:16:25.000000 pandeia.engine-3.1/pandeia/engine/helpers/peng/__init__.py
--rw-r--r--   0 riedel    (1525)     1031    79567 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/helpers/peng/peng3jeng.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:42.005303 pandeia.engine-3.1/pandeia/engine/helpers/schema/
--rw-r--r--   0 riedel    (1525)     1031        0 2022-10-04 19:20:09.000000 pandeia.engine-3.1/pandeia/engine/helpers/schema/__init__.py
--rw-r--r--   0 riedel    (1525)     1031    37075 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/helpers/schema/messages.py
--rw-r--r--   0 riedel    (1525)     1031    29952 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/hst.py
--rw-r--r--   0 riedel    (1525)     1031    64578 2023-09-19 16:44:39.000000 pandeia.engine-3.1/pandeia/engine/instrument.py
--rw-r--r--   0 riedel    (1525)     1031     2000 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/instrument_factory.py
--rw-r--r--   0 riedel    (1525)     1031    14519 2023-01-24 15:41:58.000000 pandeia.engine-3.1/pandeia/engine/io_utils.py
--rw-r--r--   0 riedel    (1525)     1031    28525 2023-09-19 16:44:14.000000 pandeia.engine-3.1/pandeia/engine/jwst.py
--rw-r--r--   0 riedel    (1525)     1031    12044 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/noise.py
--rw-r--r--   0 riedel    (1525)     1031    18038 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/normalization.py
--rw-r--r--   0 riedel    (1525)     1031     1691 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/observation.py
--rw-r--r--   0 riedel    (1525)     1031     6889 2023-11-13 20:36:41.000000 pandeia.engine-3.1/pandeia/engine/pandeia_warnings.py
--rw-r--r--   0 riedel    (1525)     1031     1728 2023-03-01 18:51:17.000000 pandeia.engine-3.1/pandeia/engine/perform_calculation.py
--rw-r--r--   0 riedel    (1525)     1031    26198 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/profile.py
--rw-r--r--   0 riedel    (1525)     1031     8722 2023-08-03 16:25:50.000000 pandeia.engine-3.1/pandeia/engine/projection.py
--rw-r--r--   0 riedel    (1525)     1031    24272 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/psf_library.py
--rw-r--r--   0 riedel    (1525)     1031    74069 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/report.py
--rw-r--r--   0 riedel    (1525)     1031     4694 2023-11-16 22:20:27.000000 pandeia.engine-3.1/pandeia/engine/roman.py
--rw-r--r--   0 riedel    (1525)     1031     6651 2023-03-07 21:29:39.000000 pandeia.engine-3.1/pandeia/engine/scene.py
--rw-r--r--   0 riedel    (1525)     1031    29620 2023-06-07 18:37:28.000000 pandeia.engine-3.1/pandeia/engine/sed.py
--rw-r--r--   0 riedel    (1525)     1031   101437 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/signal.py
--rw-r--r--   0 riedel    (1525)     1031    15359 2023-07-06 20:11:51.000000 pandeia.engine-3.1/pandeia/engine/source.py
--rw-r--r--   0 riedel    (1525)     1031   213337 2023-11-02 16:28:05.000000 pandeia.engine-3.1/pandeia/engine/strategy.py
--rw-r--r--   0 riedel    (1525)     1031     3172 2023-01-24 15:41:59.000000 pandeia.engine-3.1/pandeia/engine/telescope.py
--rw-r--r--   0 riedel    (1525)     1031     9028 2023-02-08 16:34:29.000000 pandeia.engine-3.1/pandeia/engine/utils.py
-drwxr-xr-x   0 riedel    (1525)     1031        0 2023-12-11 19:45:42.006716 pandeia.engine-3.1/pandeia.engine.egg-info/
--rw-r--r--   0 riedel    (1525)     1031     2221 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia.engine.egg-info/PKG-INFO
--rw-r--r--   0 riedel    (1525)     1031    13493 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia.engine.egg-info/SOURCES.txt
--rw-r--r--   0 riedel    (1525)     1031        1 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia.engine.egg-info/dependency_links.txt
--rw-r--r--   0 riedel    (1525)     1031        1 2022-10-05 14:53:14.000000 pandeia.engine-3.1/pandeia.engine.egg-info/not-zip-safe
--rw-r--r--   0 riedel    (1525)     1031       72 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia.engine.egg-info/requires.txt
--rw-r--r--   0 riedel    (1525)     1031        8 2023-12-11 19:45:41.000000 pandeia.engine-3.1/pandeia.engine.egg-info/top_level.txt
--rw-r--r--   0 riedel    (1525)     1031       38 2023-12-11 19:45:42.008311 pandeia.engine-3.1/setup.cfg
--rw-r--r--   0 riedel    (1525)     1031     3606 2023-12-11 18:50:22.000000 pandeia.engine-3.1/setup.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.699526 pandeia.engine-3.2/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      125 2022-12-15 19:23:09.000000 pandeia.engine-3.2/MANIFEST.in
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2044 2024-04-05 14:20:28.699085 pandeia.engine-3.2/PKG-INFO
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1218 2022-11-23 21:04:59.000000 pandeia.engine-3.2/README.md
+-rwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)       62 2021-04-30 14:42:15.000000 pandeia.engine-3.2/clean
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.549540 pandeia.engine-3.2/pandeia/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      181 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/__init__.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.573460 pandeia.engine-3.2/pandeia/engine/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1509 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/engine/LICENSE.rst
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1933 2023-03-02 14:05:15.000000 pandeia.engine-3.2/pandeia/engine/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    64636 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/astro_spectrum.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    12048 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/background.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2787 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/bnc.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    12673 2023-03-02 14:05:15.000000 pandeia.engine-3.2/pandeia/engine/calc_utils.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     8969 2023-07-18 13:14:53.000000 pandeia.engine-3.2/pandeia/engine/config.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4247 2023-09-20 14:22:49.000000 pandeia.engine-3.2/pandeia/engine/constants.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    26829 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/coords.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    10694 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/custom_exceptions.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     9702 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/debug_utils.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.576122 pandeia.engine-3.2/pandeia/engine/defaults/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/engine/defaults/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      353 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/defaults/background_defaults.json
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      219 2022-11-23 21:04:59.000000 pandeia.engine-3.2/pandeia/engine/defaults/calculationconfig_defaults.json
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      311 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/defaults/insconfig_defaults.json
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)       50 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/engine/defaults/observation_defaults.json
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    73448 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/detector.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1136 2023-11-02 17:41:40.000000 pandeia.engine-3.2/pandeia/engine/detector_factory.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    22198 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/etc3D.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16795 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/exposure.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1496 2023-11-02 17:41:40.000000 pandeia.engine-3.2/pandeia/engine/exposure_factory.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    15309 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/extinction.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.577824 pandeia.engine-3.2/pandeia/engine/helpers/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        9 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia/engine/helpers/DEVBUILD
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      140 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/README.md
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/engine/helpers/__init__.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.578830 pandeia.engine-3.2/pandeia/engine/helpers/background/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     7435 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/butler.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.582735 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      599 2023-03-16 12:48:48.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    11152 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6595 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky_angles.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1238 2023-04-28 16:59:23.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky_spectrum.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3909 2024-02-22 13:54:05.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/util.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3928 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/hst/zodi.dat
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.586725 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2853 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/accessor_globals.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2030 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/bmg_accessor.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2799 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/mod_healpix_func.py
+-rwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)     7648 2024-02-22 16:11:32.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/sl_accessor_funcs.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      203 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/straylight_accessor.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      148 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/thermal_accessor.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.595324 pandeia.engine-3.2/pandeia/engine/helpers/bit/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      986 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/README.md
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/__init__.py
+-rwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)    16191 2023-06-01 12:29:53.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/bit.py
+-rwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)     3999 2023-06-01 12:29:53.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/bit_regenerate_pweb_peng_jeng.py
+-rwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)     4534 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/bit_test_query_to_peng.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6612 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/compute.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.602290 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-12-15 19:23:09.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      568 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/acs_sbc.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      823 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/acs_wfc.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      499 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/cos_fuv.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      468 2023-06-01 12:29:53.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/cos_nuv.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1072 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/global.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      667 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_ccd.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1330 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_fuv-mama.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1265 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_nuv-mama.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      134 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/wfc3_ir.dict
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1742 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/config/wfc3_uvis.dict
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.603516 pandeia.engine-3.2/pandeia/engine/helpers/bit/etc_web_data/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1218 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/etc_web_data/extraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    27982 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/etc_web_data/targets.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    10770 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/extraction.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    47385 2022-12-15 19:23:09.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/input_conversion.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.606770 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      971 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/README
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6105 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4740 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/custom_configuration.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     5419 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/data.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.608737 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      708 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/__init__.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.614373 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      659 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    33090 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_aperture_fraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    11364 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1431 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     7561 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_limits.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2990 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_sharpness.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1320 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/detector_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      836 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/instr_functions.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.619752 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1055 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     9807 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_web.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1503 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_coronography.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1724 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_imaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1518 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampcoronography.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1735 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampfilter.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1530 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_spectroscopic.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.625485 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      768 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    17734 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_aperture_fraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4001 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2182 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     7246 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_limits.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3938 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/custom_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2888 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/detector_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    37744 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/instr_functions.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.630604 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1573 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3591 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_web.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1781 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_imaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1621 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopic.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1647 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopicacq.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1392 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_targetacquisition.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      565 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/default.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3148 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/scan_mode.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.636294 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      705 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3944 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/detector_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    22864 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/instr_functions.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    30096 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_aperture_fraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    13879 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1914 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     8214 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_limits.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2281 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_sharpness.dat
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.640531 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1743 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_imaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1967 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_spectroscopic.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1477 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_targetacquisition.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      907 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     7284 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_web.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.646976 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      642 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      739 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/detector_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2286 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/instr_functions.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.652035 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1655 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_imaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1780 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scimaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1581 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scspectroscopic.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1456 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_spectroscopic.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      799 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2587 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_web.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    20541 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_aperture_fraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2140 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1037 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4342 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_limits.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1059 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_sharpness.dat
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.658704 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      652 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      906 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/detector_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1422 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/instr_functions.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.663469 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1753 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_imaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1878 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_scimaging.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1421 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_spectroscopic.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      745 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2587 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_web.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)   210674 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_aperture_fraction.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6778 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_config.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      951 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_extraction_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4946 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_limits.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1736 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_sharpness.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)      669 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/telescopes.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     9891 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/perform_calculation.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.696320 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2695 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/README
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2677 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2147 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    17768 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2152 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    17200 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1959 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    15460 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2197 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16270 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2085 2023-06-01 12:29:53.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16647 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2050 2023-06-01 12:29:53.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16826 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1785 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    14502 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1144 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/map
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1108 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4094 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1114 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3931 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1141 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4591 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1141 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_defaults.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4100 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1123 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/options_map
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2164 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    17315 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2490 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    23797 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1881 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    15077 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2051 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16985 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1894 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    14921 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1868 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    14575 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1816 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    14573 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2183 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    18490 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2021 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16423 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1780 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_default_input.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    14839 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_form_options.dat
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     7634 2024-02-22 13:54:05.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_util.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    11469 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/sky.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    16404 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/source.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2097 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/string_constants.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    10372 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/helpers/bit/translate.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.697363 pandeia.engine-3.2/pandeia/engine/helpers/peng/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2022-02-17 19:55:03.000000 pandeia.engine-3.2/pandeia/engine/helpers/peng/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    79567 2023-10-04 16:05:23.000000 pandeia.engine-3.2/pandeia/engine/helpers/peng/peng3jeng.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.698352 pandeia.engine-3.2/pandeia/engine/helpers/schema/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        0 2021-04-30 14:42:15.000000 pandeia.engine-3.2/pandeia/engine/helpers/schema/__init__.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    37522 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/helpers/schema/messages.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    33764 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/hst.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    67392 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/instrument.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2000 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/instrument_factory.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    18343 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/io_utils.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    29561 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/jwst.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    12080 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/noise.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    18290 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/normalization.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     1691 2023-03-02 14:05:15.000000 pandeia.engine-3.2/pandeia/engine/observation.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6903 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/pandeia_warnings.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2063 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/perform_calculation.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    28560 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/profile.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    13190 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/projection.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    24272 2023-09-20 14:22:49.000000 pandeia.engine-3.2/pandeia/engine/psf_library.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    76559 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/report.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     4954 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/roman.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     6702 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/scene.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    32268 2024-01-18 13:38:58.000000 pandeia.engine-3.2/pandeia/engine/sed.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)   104933 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/signal.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    15359 2023-07-18 13:14:53.000000 pandeia.engine-3.2/pandeia/engine/source.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)   217796 2024-03-12 19:03:28.000000 pandeia.engine-3.2/pandeia/engine/strategy.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3172 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/telescope.py
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     9028 2023-02-20 17:35:50.000000 pandeia.engine-3.2/pandeia/engine/utils.py
+drwxr-xr-x   0 ispitzer  (2833) STSCI\science  (1031)        0 2024-04-05 14:20:28.552494 pandeia.engine-3.2/pandeia.engine.egg-info/
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     2044 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia.engine.egg-info/PKG-INFO
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)    13493 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia.engine.egg-info/SOURCES.txt
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        1 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia.engine.egg-info/dependency_links.txt
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        1 2021-06-11 13:44:41.000000 pandeia.engine-3.2/pandeia.engine.egg-info/not-zip-safe
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)       72 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia.engine.egg-info/requires.txt
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)        8 2024-04-05 14:20:28.000000 pandeia.engine-3.2/pandeia.engine.egg-info/top_level.txt
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)       38 2024-04-05 14:20:28.699666 pandeia.engine-3.2/setup.cfg
+-rw-r--r--   0 ispitzer  (2833) STSCI\science  (1031)     3606 2024-04-05 14:03:17.000000 pandeia.engine-3.2/setup.py
```

### Comparing `pandeia.engine-3.1/PKG-INFO` & `pandeia.engine-3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: pandeia.engine
-Version: 3.1
+Version: 3.2
 Summary: Pandeia 3D Exposure Time Calculator compute engine
 Home-page: https://jwst.etc.stsci.edu
 Author: Adric Riedel, Isaac Spitzer, Dharini Chittiraibalan, Oi In Tam, Chris Sontag, Ivo Busko, Craig Jones, Tim Pickering, Klaus Pontoppidan
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: numpy>=1.17
-Requires-Dist: scipy>1.6
-Requires-Dist: astropy>=4
-Requires-Dist: photutils
-Requires-Dist: synphot
-Requires-Dist: stsynphot
-Requires-Dist: setuptools
 
 The Pandeia engine is a 'simulation-hybrid' exposure time calculation engine that performs calculations on two-dimensional astronomical scenes created by the user. It uses a pixel-based 3D approach, modeling both the spatial and wavelength dimensions using realistic PSFs for each instrument mode, and handles saturation, correlated read noise, and inter-pixel capacitance. It supports both the James Webb Space Telescope and the Wide-field Imager mode of the Nancy Grace Roman Space Telescope.
 
 Installation and setup instructions (including a required data package) for the Pandeia engine can be found at this Space Telescope Science Institute page: https://outerspace.stsci.edu/display/PEN/Pandeia+Engine+News
 
 See also this page for James Webb Space Telescope (JWST)-specific installation instructions:
 https://jwst-docs.stsci.edu/jwst-exposure-time-calculator-overview/jwst-etc-pandeia-engine-tutorial/installing-pandeia
```

### Comparing `pandeia.engine-3.1/README.md` & `pandeia.engine-3.2/README.md`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/LICENSE.rst` & `pandeia.engine-3.2/pandeia/engine/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/__init__.py` & `pandeia.engine-3.2/pandeia/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/astro_spectrum.py` & `pandeia.engine-3.2/pandeia/engine/astro_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,22 @@
             self.add_spectral_lines()
 
         # Astropy Synphot usage ends here, so convert back to arrays
         self.wave = self.wave.to_value(PANDEIA_WAVEUNITS)
         self.flux = self.flux.to_value(PANDEIA_FLUXUNITS)
 
     def export_to_fits_table(self, fitsfile="source_spectrum.fits"):
+        """
+        Export the source spectrum to a fits file
+
+        Parameters:
+        fitsfile (str, optional): 
+            name of the output file. Defaults to "source_spectrum.fits".
+        """
+
         c1 = fits.Column(array=self.wave, format="D", name="wavelength", unit="micron")
         c2 = fits.Column(array=self.flux, format="D", name="flux", unit="mJy")
         tbhdu = fits.BinTableHDU.from_columns([c1, c2])
         tbhdu.writeto(fitsfile, overwrite=True)
 
     def add_spectral_lines(self):
         """
@@ -342,14 +350,21 @@
         # In wavelength units
         self.wave_width = self.width / cs.c * self.center
 
         # Run the sanity checks to make sure things are kosher.
         self._sanity_checks()
 
     def _sanity_checks(self):
+        """
+        Basic sanity check for lines. Strength must be positive, line width must be
+        positive, center wavelength must be positive.
+
+        Raises:
+            EngineInputError: Useful error for the line parameters checked.
+        """
 
         # Check the center, width and strength
         # Based on Issue #2263#issuecomment-263374621
         if self.center <= 0 or self.width <= 0 or self.strength < 0:
             msg = 'Invalid line configuration'
             if self.name:
                 msg += ' for "' + self.name + '"'
@@ -412,15 +427,15 @@
         sigma = self.wave_width / 2.3548
 
         # normalized to a peak flux density of 1 mJy - note that flux will be unitless
         flux = np.exp(-(wave - self.center) ** 2 / (2. * sigma ** 2))
 
         # input line strength units in 10^-26 erg/cm^2/s (aka mJy)
         # because the flux is unitless and THIS calculation isn't unit-aware, we have to do some manual conversions
-        int_flux = -integ.simps(flux * 1e-26, cs.c / (wave.to(u.m)))
+        int_flux = -integ.simpson(flux * 1e-26, cs.c / (wave.to(u.m)))
 
 
         flux = flux * self.strength / int_flux
 
         return flux
 
     def optical_depth(self, wave):
@@ -570,23 +585,23 @@
         Also compute the filter leak (only valid for image projections), which needs pre- and 
         post-trimming products.
         """
         for i, spectrum in enumerate(spectra):
             if self.instrument.projection_type in ["image", "image_scan"]:
                 # get the pre-trimming filter leak components
                 full_filtered = self.focal_plane_rate(spectrum.flux, spectrum.wave)
-                full = integ.simps(full_filtered, spectrum.wave)
+                full = integ.simpson(full_filtered, spectrum.wave)
 
             # we trim here as an optimization so that we only convolve the section we need of a possibly very large spectrum
             spectrum.trim(wrange['wmin'], wrange['wmax'])
 
             if self.instrument.projection_type in ["image", "image_scan"]:
                 # get the post-trimming filter leak components
                 trim_filtered = self.focal_plane_rate(spectrum.flux, spectrum.wave)
-                trim = integ.simps(trim_filtered, spectrum.wave)
+                trim = integ.simpson(trim_filtered, spectrum.wave)
 
                 # compute filter leak and set warning if applicable
                 filter_leak = (full-trim)/full
                 if filter_leak > self.instrument.max_filter_leak:
                     key = "filter_leak"
                     msg = warning_messages[key].format(filter_leak*100)
                     self.warnings["%s_%s" % (key, i)] = msg
@@ -762,14 +777,44 @@
         # brightest_pixel_rate is now the rate (in e-/s or counts/s) of the source, in its
         # brightest pixel.
 
         return brightest_pixel_rate
 
 
     def get_fov_size(self, pixbuffer=SCENE_FOV_PIXBUFFER):
+        """
+        get_fov_size is the main function that determines the size of the FOV. There are
+        four possible modes: 
+        
+        1. For multiorder (just NIRISS SOSS): Use the size given in the subarray
+        2. If the scene is dynamic, the size is the size of the scene (plus
+           SCENE_FOV_PIXBUFFER) between the minimum and maximum sizes. 
+        3. If the scene is not dynamic, the size is custom_scene_size 
+        4. If custom_scene_size is not set, the size is the PSF dimensions.
+
+        In all cases, the scene is intended to be square. 
+        
+        Parameters
+        ----------
+        pixbuffer : int
+           buffer size around the scene, by default SCENE_FOV_PIXBUFFER. This exists so
+           that a point source at the edge of the scene will not be visibly cut off
+
+        Returns
+        -------
+        fov_size: float
+            The FOV size in arcseconds, for a square scene
+
+        Raises
+        ------
+        DataError
+            If appropriate defaults do not exist in the data
+        EngineInputError
+            If the scene size is larger than max_fov
+        """
         # The scene size is the minimum size containing all sources, but at least as large as the PSF.
 
 
         instrument_name = self.instrument.get_name()
         aperture_name = self.instrument.get_aperture()
         readout_pattern = self.instrument.detector.get("readout_pattern", "default")
         psf_shape = self.instrument.psf_library.get_shape(instrument_name, aperture_name)
@@ -1167,14 +1212,20 @@
         ])
         tbhdu.name = 'WCS-TAB'
         return tbhdu, header
 
     def export_to_fits(self, fitsfile='ModelDetectorCube'):
         """
         Write convolved scene cube to a FITS file
+
+        Parameters
+        ----------
+        fitsfile: str
+            The name of the fits file to write to.
+
         """
         header = self.grid.wcs_info()
         for slice_index,flux_plus_bg in enumerate(self.flux_plus_bg_list):
             fitsfile_slice = '{}{}.fits'.format(fitsfile, str(slice_index).strip())
             t1 = fits.PrimaryHDU(np.moveaxis(flux_plus_bg, [0, 1, 2], [1, 2, 0]))
             c1 = fits.Column(name='wavelength', array=self.wave, format='D')
             t2 = fits.BinTableHDU.from_columns([c1])
```

### Comparing `pandeia.engine-3.1/pandeia/engine/background.py` & `pandeia.engine-3.2/pandeia/engine/background.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,30 +166,46 @@
                     msg += repr(e)
                 raise DataError(value=msg)
 
         self.bg_spec = tot_bg
 
     @property
     def wave(self):
+        """
+        Return the wavelength of the current binned/trimmed background
+
+        Returns
+        -------
+        np.ndarray
+            background wavelength array in PANDEIA_WAVEUNITS
+        """
         return self.bg.waveset.to_value(PANDEIA_WAVEUNITS)
 
     @property
     def MJy_sr(self):
+        """
+        Return the flux of the current binnned/trimmed background
+
+        Returns
+        -------
+        np.ndarray
+            background flux array, converted to MJy/sr.
+        """
         return self.bg(self.bg.waveset, flux_unit=u.MJy).to_value(u.MJy)
 
 
     @property
     def mjy_pix(self):
         """
         Convert background surface brightness in MJy/sr to F_nu per pixel in
         mJy/pixel (self.wave assumed to be in microns)
 
         Returns
         -------
-        i_pix: 1D np.ndarray
+        i_nu_pix: 1D np.ndarray
             Flux per pixel in mJy/pixel
         """
         i_nu = self.bg(self.bg.waveset, flux_unit=PANDEIA_FLUXUNITS).to_value(PANDEIA_FLUXUNITS) * (u.arcsec * u.arcsec).to(u.sr)
 
         i_nu_pix = i_nu * self.aperture_pars['plate_scale'][0] * self.aperture_pars['plate_scale'][1]
         return i_nu_pix
```

### Comparing `pandeia.engine-3.1/pandeia/engine/bnc.py` & `pandeia.engine-3.2/pandeia/engine/bnc.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/calc_utils.py` & `pandeia.engine-3.2/pandeia/engine/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/config.py` & `pandeia.engine-3.2/pandeia/engine/config.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/constants.py` & `pandeia.engine-3.2/pandeia/engine/constants.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/coords.py` & `pandeia.engine-3.2/pandeia/engine/coords.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,23 +63,33 @@
         # flip Y axis because we use Y increasing from bottom to top
         self.pixel_col = pixel_yvals[::-1]
 
     @property
     def shape(self):
         """
         Provides array-like .shape functionality
+
+        Returns
+        -------
+        sh: tuple
+            shape-like tuple
         """
         sh = (self.ny, self.nx)
         return sh
 
     def as_dict(self):
         """
         Create engine API format dict containing the properties of the Grid instance. The half-pixel
         offsets are due to the pixel coordinates being referenced to pixel centers. Thus the edges of the
         Grid are a half-pixel above and to the left of the Grid index origin.
+
+        Returns
+        -------
+        transform: dict
+            All necessary information about this coordinate grid, in dict form.
         """
 
         transform = {}
         transform['x_refpix'] = 0
         transform['x_refval'] = self.x[0][0]
         transform['x_max'] = self.x.max() + 0.5 * self.xsamp
         transform['x_min'] = self.x.min() - 0.5 * self.xsamp
@@ -118,14 +128,19 @@
             'cname2': 'Y',
         }
         return header
 
     def __len__(self):
         """
         Provide array-like len() functionality
+
+        Returns
+        -------
+        l: int
+           the full size of the grid, in (sub)pixels
         """
         l = self.x.shape[0] * self.x.shape[1]
         return l
 
     def __getitem__(self, val):
         """
         Provide array-like indexing functionality.
@@ -141,31 +156,62 @@
             Elements are floats in the case of specific indicies and arrays in
             the cases of slice()'s.
         """
         section = [self.y[val], self.x[val]]
         return section
 
     def bounds(self):
+        """
+        Return boundary information
+
+        Returns
+        -------
+        dict
+            grid boundary information
+        """
         return {'xmin': np.min(self.x),
                 'xmax': np.max(self.x),
                 'ymin': np.min(self.y),
                 'ymax': np.max(self.y)}
 
     def dist(self, xcen=0.0, ycen=0.0):
         """
         Return a distance array where each element contains its distance from
         the center of the grid.
+
+        Parameters
+        ----------
+        xcen, ycen: float, optional
+            offset position from which to compute distance
+
+        Returns
+        -------
+        d: np.ndarray
+            2D grid of distances from (xcen, ycen)
+
         """
         d = np.sqrt((self.x - xcen) ** 2 + (self.y - ycen) ** 2)
         return d
 
     def dist_xy(self, xcen=0.0, ycen=0.0):
         """
-        Return a directional distance array where each element contains its (x,y) distance from
+        Return directional distance arrays where each element contains its (x,y) distance from
         the center of the grid.
+
+        Parameters
+        ----------
+        xcen, ycen: float, optional
+            offset position from which to compute distance
+
+        Returns
+        -------
+        dx: np.ndarray
+            2D grid of x-dimension distances from xcen
+        dy: np.ndarray
+            2D grid of y-dimension distances from ycen
         """
         dx = self.x - xcen
         dy = self.y - ycen
         return dx,dy
 
     def world_to_image(self, y, x):
         """
@@ -257,14 +303,19 @@
         xsh_rot = xsh * np.cos(pa_radians) + ysh * np.sin(pa_radians)
         ysh_rot = -xsh * np.sin(pa_radians) + ysh * np.cos(pa_radians)
         return ysh_rot, xsh_rot
 
     def get_aperture(self):
         """
         Return Grid parameters as an aperture specification
+
+        Returns
+        -------
+        ap: dict
+            Pandeia Aperture specficiation dictionary
         """
         ap = {'width': self.nx * self.xsamp, 'height': self.ny * self.ysamp, 'offset': (0, 0)}
         return ap
 
     def rectangular_mask(self, width=None, height=None, xoff=0.0, yoff=0.0, transparency=1.0, pixels=False):
         """
         Define a rectangular mask within the Grid of specfied width and height and offset by xoff/yoff.
@@ -319,42 +370,80 @@
         # if width and/or height are not specified, set them encompass the size of the Grid.
         # add two pixels to make sure the masking does not interpolate the edges.
         if width is None:
             width = maxx - minx + 2 * xsamp
         if height is None:
             height = maxy - miny + 2 * ysamp
 
+
+        # The min and max values are either the bounds of the FOV or one pixel outside the
+        # rectangle, whichever is further from center. (JETC-4064) In all other cases, we
+        # want to straddle the edge of the rectangle by +/- 0.5 of the sampling.
         mask_x = np.array(
             [
-                minx,
+                np.min((minx, xcen - (width + xsamp) / 2.0 + xoff - xsamp)),
                 xcen - (width + xsamp) / 2.0 + xoff,
                 xcen - (width - xsamp) / 2.0 + xoff,
                 xcen + (width - xsamp) / 2.0 + xoff,
                 xcen + (width + xsamp) / 2.0 + xoff,
-                maxx
+                np.max((maxx, xcen + (width + xsamp) / 2.0 + xoff + xsamp)),
             ]
         )
         mask_y = np.array(
             [
-                miny,
+                np.min((miny, ycen - (height + ysamp) / 2.0 + yoff - ysamp)),
                 ycen - (height + ysamp) / 2.0 + yoff,
                 ycen - (height - ysamp) / 2.0 + yoff,
                 ycen + (height - ysamp) / 2.0 + yoff,
                 ycen + (height + ysamp) / 2.0 + yoff,
-                maxy
+                np.max((maxy, ycen + (height + ysamp) / 2.0 + yoff + ysamp)),
             ]
         )
 
+        # There are 4 edge cases to be concerned with:
+        # 1. Rectangle is taller/wider than 1 pixel 
+        #    - do not renormalize
+        # 2. Rectangle is shorter/narrower than 1 pixel 
+        #    - renormalize to the height/width
+        # 3. Rectangle is shorter/narrower than 1 pixel but offset completely off the edge
+        #    - do not renormalize
+        # 4. Rectangle is shorter/narrower than 1 pixel but offset partially off the edge
+        #    - renormalize to the fraction still within the FOV.
+        missingheight = np.max(((yoff+height/2) - maxy, miny - (yoff - height/2)))-1
+        missingwidth = np.max(((xoff+width/2)- maxx, minx - (xoff - width/2))) -1
+        orig_width = width
+        orig_height = height
+
+        # Note that thought we're potentially altering the height here, it will still do
+        # the right thing with larger rectangles (anything with more than a pixel remaining will
+        # be unaffected; anything larger but with less than a pixel remaining will be altered but correct)
+        if missingheight > 0:
+            height -= missingheight
+        if missingwidth > 0:
+            width -= missingwidth
+
+        # Pixels are judged as being at the middle of a bin. Therefore, half a pixel
+        # outside the rectangle will be fully off, half a pixel inside the rectangle will
+        # be fully on. However, in the case of an aperture smaller than one pixel, elements
+        # 3 and 4 of the mask arrays above will be flipped, resulting in a non-monotonic 
+        # array. The array needs to be monotonic, and scaled to the correct value, so we sort
+        # and scale if it's smaller than a pixel. (JETC-4064)
         mask_pix = np.array([0.0, 0.0, 1.0, 1.0, 0.0, 0.0])
         if pixels:
-            x_mask_int = np.interp(self.pixel_row, mask_x, mask_pix)
-            y_mask_int = np.interp(self.pixel_col, mask_y, mask_pix)
+            x_mask_int = np.interp(self.pixel_row, sorted(mask_x), mask_pix)
+            y_mask_int = np.interp(self.pixel_col, sorted(mask_y), mask_pix)
         else:
-            x_mask_int = np.interp(self.row, mask_x, mask_pix)
-            y_mask_int = np.interp(self.col, mask_y, mask_pix)
+            x_mask_int = np.interp(self.row, sorted(mask_x), mask_pix)
+            y_mask_int = np.interp(self.col, sorted(mask_y), mask_pix)
+        if orig_width/xsamp <= 1 and np.sum(x_mask_int) > 0: # only if the rectangle is less than a pixel wide; don't do this if the rectangle is entirely not in the FOV.
+            # normalize and then correct to the width relative to a pixel
+            x_mask_int = x_mask_int / np.sum(x_mask_int) * width/xsamp
+        if orig_height/ysamp <= 1 and np.sum(y_mask_int) > 0:
+            # normalize and then correct to the height relative to a pixel
+            y_mask_int = y_mask_int / np.sum(y_mask_int) * height/ysamp
         x_mask = x_mask_int.reshape((1, self.nx))
         y_mask = y_mask_int.reshape((self.ny, 1))
         mask = y_mask * x_mask * transparency
         return mask
 
     def circular_mask(self, radius, xoff=0.0, yoff=0.0, use_exact=1, subsampling=1, transparency=1.0, pixels=False):
         """
@@ -364,17 +453,17 @@
         use_exact=0 will sub-sample the pixels by the specfied subsampling parameter
         to estimate the subtended area.
 
         Parameters
         ----------
         radius: float
             Radius of the circular mask
-        xoff: float
+        xoff: float (default: 0.0)
             X position of the center of the mask
-        yoff: float
+        yoff: float, (default: 0.0)
             Y position of the center of the mask
         use_exact: int (default: 1)
             If 1, then use exact geometrical calculation to weight pixels partially covered by mask.
             This parameter is passed directly on to photutils.geometry.circular_overlap_grid()
         subsampling: int (default: 1)
             If use_exact=0, then subsample pixels by this factor to calculate area of each pixel subtended
             by the mask. The default value of 1 will force no partial pixels to be included in the mask.
@@ -444,19 +533,19 @@
 
         Parameters
         ----------
         major: float
             Semi-major axis of the elliptical mask
         minor: float
             Semi-minor axis of the mask
-        pa: float
+        pa: float (default: 0.0)
             Position angle of the ellipse in degrees measured clockwise (positive in +X direction)
-        xoff: float
+        xoff: float (default: 0.0)
             X position of the center of the mask
-        yoff: float
+        yoff: float (default: 0.0)
             Y position of the center of the mask
         use_exact: int (default: 1)
             If 1, then use exact geometrical calculation to weight pixels partially covered by mask.
             This parameter is passed directly on to photutils.geometry.circular_overlap_grid()
         subsampling: int (default: 1)
             If use_exact=0, then subsample pixels by this factor to calculate area of each pixel subtended
             by the mask. The default value of 1 will force no partial pixels to be included in the mask.
@@ -504,17 +593,17 @@
         a.) the lower left pixel of the 2x2 box,
         b.) the proportion of flux that spills into that and the other three pixels (as long as they're not off the edge
             of the grid)
         c.) and then return an image, scaled appropriately.
 
         Parameters
         ----------
-        xoff: float
+        xoff: float (default: 0.0)
             X position of point source
-        yoff: float
+        yoff: float (default: 0.0)
             Y position of point source
 
         Returns
         -------
         im: 2D np.ndarray
             Image containing point source with flux scaled to 1.0.
         """
```

### Comparing `pandeia.engine-3.1/pandeia/engine/custom_exceptions.py` & `pandeia.engine-3.2/pandeia/engine/custom_exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -260,14 +260,20 @@
 
     def __init__(self, value='Background Error', debug=None):
         BackgroundError.__init__(self, value, debug)
         self.name = value
 
 
 class DatelessBGError(BackgroundError):
+    """
+    Handles all cases where a dateless background nevertheless has an error.
+
+    Usage:
+        raise engine.custom_exceptions.DatelessBGError('descriptive text')
+    """
 
     def __init__(self, value='Dateless Background Error', debug=None):
         BackgroundError.__init__(self, value, debug)
         self.name = value
 
 
 class BMGError(BackgroundError):
```

### Comparing `pandeia.engine-3.1/pandeia/engine/debug_utils.py` & `pandeia.engine-3.2/pandeia/engine/debug_utils.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/detector.py` & `pandeia.engine-3.2/pandeia/engine/detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 class Detector:
 
     def __init__(self, config, webapp=False):
         """
         All functions that are detector-specific will live under children of this class
 
-        DetectorNoise will use the this class (or rather, its detector-specific subclasses) to produce noise.
+        DetectorNoise will use the this class (or rather, its detector-specific
+        subclasses) to produce noise.
         """
         self.webapp = webapp
         self.detector_config = config["detector_config"]
         self.subarray_config = config["subarray_config"]
         self.readout_pattern_config = config["readout_pattern_config"]
         self.input_detector = config["input_detector"]
 
@@ -54,42 +55,132 @@
             "readout_pattern": self.readout_pattern_config, "detector_config": self.detector_config}
 
         exposure_spec = ExposureFactory(self.det_type, config=exp_conf, webapp=self.webapp)
 
         return exposure_spec
 
     def set_saturation(self, flag):
-        # this function turns saturation on and off - if the flag is True, we 
-        # compute saturation. If toggle is False, we do not.
+        """
+        Set saturation flag. 
+
+        This method turns saturation on and off - if the flag is True, we compute
+        saturation. If toggle is False, we do not.
+
+        The use of this API is preferred over ignoring the saturation map or setting it to
+        all zeros after the fact.
+
+        Parameters
+        ----------
+        flag: bool
+            Boolean to toggle saturation
+        """
+
         if not flag:
             self.fullwell = np.inf
 
     def set_readnoise(self, flag):
-        # this function turns readnoise on and off - if the flag is False,
-        # we set the readnoise to 0.
+        """
+        Set readnoise flag
+
+        This method turns readnoise on and off. If the flag is True, we use the
+        readnoise from the config.json file. If False, it is set to zero.
+
+        Parameters
+        ----------
+        flag : bool
+            Boolean to toggle readnoise
+        """
         if not flag:
             self.rn = 0
 
     def set_excess(self, flag):
-        # this function turns the various excess noise components on and off - if the flag is False,
-        # we set var_fudge, excessp1, and excessp2 to 0.
+        """
+        Set Excess Noise flag
+
+        This method turns the various excess noise components on and off - if the flag
+        is False, we set var_fudge, excessp1, and excessp2 to 0.
+
+        Parameters
+        ----------
+        flag : bool
+            Boolean to toggle excess noise
+        """
+
         if not flag:
             self.var_fudge = 1
             self.excessp1 = 0
             self.excessp2 = 0
 
     def get_slope_variance(self, rate, unsat):
+        """
+        Hook allowing different slope variance behaviors. Multiaccum will override this
+        method to provide unique slope variance functions for regular and TA observations.
+
+        Parameters
+        ----------
+        rate : dict
+            dictionary of source rates (generally variance, with background)
+        unsat : np.ndarray
+            2D array map of the number of unsaturated groups, per pixel.
+
+        Returns
+        -------
+        slope_var: np.ndarray
+            2D array of the total noise.
+        slope_rn_var: np.ndarray
+            2D array of the readnoise component only.
+        """
         # This function allows different slope variance functions (used for MULTIACCUM TA)
         slope_var, slope_rn_var = self.slope_variance(rate, unsat)
         return slope_var, slope_rn_var
 
     def scale_exposure_time(self, extracted):
+        """
+        Scale exposure time
+
+        For reverse calculations, the computation is first done for t=1s, and then the SNR
+        equation is worked in reverse to determine the appropriate time to achieve that
+        SNR. 
+        
+        This will only be defined for detectors where reverse calculation is meaningfully
+        possible (SingleAccum)
+
+        Parameters
+        ----------
+        extracted : dict
+            Dictionary of extracted products, needed to get the SNR, mask, and other
+            extracted properties for the 1s calculation
+
+        Raises
+        ------
+        NotImplementedError
+            Error for detectors where reverse calculation is not supported.
+        """
         raise NotImplementedError("Reverse ETC calculations for {} are not implemented.".format(type(self)))
 
     def set_time(self, new_time):
+        """
+        Set exposure time
+
+        In a reverse calculation, the 1s initial exposure time must be replaced with the
+        final scaled time (see scale_exposure_time) and the signal and noise recomputed.
+
+        This will only be defined for detectors where reverse calculation is meaningfully
+        possible (SingleAccum)
+
+        Parameters
+        ----------
+        new_time : float
+            The new exposure time, in seconds.
+
+        Raises
+        ------
+        NotImplementedError
+            Error for detectors where reverse calculation is not supported.
+        """
         raise NotImplementedError("Reverse ETC calculations for {} are not implemented.".format(type(self)))
 
     def to_resels_scalar(self, wave, values, refwave, squared=False):
         """
         Extract scalar value from array in resels.
         Requires an array, a resel (read from the detector), and the reference wavelength
         Uses astropy 1D box model to apply the resel value.
@@ -260,34 +351,36 @@
         else:
             var_fudge = 1
         
         return var_fudge * np.ones(len(wave))
 
     def get_before_sat(self, slope):
         """
-        This method returns a map of the maximum number of groups each pixel can be exposed to, before saturation.
-        The formula is calculated by equating the time-to-saturation to the saturation time formula and isolating
-        ngroup. The resulting fractional value is then rounded down to an integer.
-
-        These equations are derived by setting saturation_time = time_to_saturation in equation 7 (for NIR H2RG
-        detectors) or equation 6 (for MIR SiAs detectors, now out of the timing document revision, JWST-STScI-006013-A)
-        of the timing document, Valenti et al. 2017, JWST-STScI-006013, and solving for n_groups.
-
-        Technically speaking, we are getting the groups BEFORE saturation by rounding the number of groups down to the
-        nearest integer. If groups_before_sat is EXACTLY an integer (which is unlikely), we will get one partially
-        saturated pixel.
+        This method returns a map of the maximum number of groups each pixel can be
+        exposed to, before saturation. The formula is calculated by equating the
+        time-to-saturation to the saturation time formula and isolating ngroup. The
+        resulting fractional value is then rounded down to an integer.
+
+        These equations are derived by setting saturation_time = time_to_saturation in
+        equation 7 (for NIR H2RG detectors) or equation 6 (for MIR SiAs detectors, now out
+        of the timing document revision, JWST-STScI-006013-A) of the timing document,
+        Valenti et al. 2017, JWST-STScI-006013, and solving for n_groups.
+
+        Technically speaking, we are getting the groups BEFORE saturation by rounding the
+        number of groups down to the nearest integer. If groups_before_sat is EXACTLY an
+        integer (which is unlikely), we will get one partially saturated pixel.
 
         Parameters
         ----------
         slope: ndarray
             The measured slope of the ramp (ie, the rate) per pixel
 
         fullwell: positive integer
-            The number of electrons defining a full well (beyond which the pixel reads become unusable for science
-            due to saturation).
+            The number of electrons defining a full well (beyond which the pixel reads
+            become unusable for science due to saturation).
         """
         # we clip to 1e-10 to avoid division by zero errors even if the slope is tiny.
         time_to_saturation = self.fullwell / slope.clip(MIN_CLIP, np.max([MIN_CLIP, np.max(slope)]))
 
         groups_before_sat = self._get_groups_before_sat(time_to_saturation)
 
         # The groups_before_sat value should never be less than 0 - that would imply saturation before we started
@@ -482,15 +575,16 @@
         if self.excessp1 != 0.0 or self.excessp2 != 0.0:
             excess_variance = (12.0 * (n-1)/(n+1) * self.excessp1**2 - self.excessp2/np.sqrt(m)) / ((1 - n) * tgroup)**2
             var_rn += excess_variance
         return var_rn
 
     def _get_saturation_mask(self, rate):
         """
-        Compute a numpy array indicating pixels with full saturation (2), partial saturation (1) and no saturation (0).
+        Compute a numpy array indicating pixels with full saturation (2), partial
+        saturation (1) and no saturation (0).
 
         Parameters
         ----------
         rate: None or 2D np.ndarray
             Detector plane rate image used to build saturation map from
 
         Returns
@@ -504,36 +598,39 @@
         saturation_mask[(unsat_ngroups < self.exposure_spec.ngroup)] = 1
         saturation_mask[(unsat_ngroups < self.mingroups)] = 2
 
         return saturation_mask
 
     def calc_cr_loss(self, ngroups, pix_cr_rate):
         """
-        Calculate the effective loss of exposure time due to cosmic rays. This uses the cosmic ray (CR) event rate
-        that is contained within the telescope configuration to calculate the odds of a cosmic rays
-        hitting a pixel. Pixels that are hit by cosmic rays are assumed to have ramps that are valid before the
-        CR, but not after. The exposure specification is used to adjust the expectation value of the exposure
+        Calculate the effective loss of exposure time due to cosmic rays. This uses the
+        cosmic ray (CR) event rate that is contained within the telescope configuration to
+        calculate the odds of a cosmic rays hitting a pixel. Pixels that are hit by cosmic
+        rays are assumed to have ramps that are valid before the CR, but not after. The
+        exposure specification is used to adjust the expectation value of the exposure
         time (i.e. ngroups) for a CR-truncated ramp.
 
         See discussion and links in:
 
         - https://confluence.stsci.edu/pages/viewpage.action?spaceKey=JWST&title=2014-11-10+Effect+of+CRs+on+SNR
         - Robberto (2010) Technical Report JWST-STScI-001928
 
         for more information on implementation and the numbers used.
 
         Parameters
         ----------
         ngroups: int
-            Number of groups over which to calculate CR losses.  This will usually be number of unsaturated groups.
+            Number of groups over which to calculate CR losses.  This will usually be
+            number of unsaturated groups.
 
         Returns
         -------
         cr_ngroups: float
-            This is the input ngroups scaled by the mean loss of time due to cosmic ray events.
+            This is the input ngroups scaled by the mean loss of time due to cosmic ray
+            events.
         """
 
         # this is the average fraction of the ramp that is lost upon a CR event
         if ngroups < self.mingroups:
             # if for some reason (e.g. using single read noise model) ngroup is less than the minimum needed
             # to get a good ramp fit, then the whole ramp is lost upon a CR event
             ramp_frac = 1.0
@@ -550,28 +647,71 @@
         # the unsaturated groups. We now simplify this (the difference is minimal and would add some complex logic now that the time
         # formulae are detector type dependent). This is simple.
         cr_ngroups = (1.0 - ramp_frac * pix_cr_rate * self.exposure_spec.saturation_time) * ngroups
 
         return cr_ngroups
 
     def get_slope_variance(self, rate, unsat):
+        """
+        Get Slope Variance
+
+        Hook allowing different slope variance behaviors. Multiaccum overrides this method
+        to provide unique slope variance functions for regular and TA observations.
+
+        Parameters
+        ----------
+        rate : dict
+            dictionary of source rates (generally variance, with background)
+        unsat : np.ndarray
+            2D array map of the number of unsaturated groups, per pixel.
+
+        Returns
+        -------
+        slope_var: np.ndarray
+            2D array of the total noise.
+        slope_rn_var: np.ndarray
+            2D array of the readnoise component only.
+
+        Raises
+        ------
+        DataConfigurationError
+            If the slopemode is not a recognized option
+        """
         # We allow alternate ways to derive a signal from a detector slope,
         # but multiaccum is the default if no mode is provided. Slopemode
         # must be matched with a corresponding slope_variance function.
         if self.slopemode == "target_acq":
             slope_var, slope_rn_var = self.slope_variance_ta(rate, unsat)
         elif self.slopemode == "multiaccum":
             slope_var, slope_rn_var = self.slope_variance(rate, unsat)
         else:
             msg = "{} is not a valid slope mode.".format(self.slopemode)
             raise DataConfigurationError(value=msg)
             
         return slope_var, slope_rn_var
 
     def _get_groups_before_sat(self, time_to_saturation):
+        """
+        The computation of groups before saturation is broken out because H2RG and SiAs
+        detectors at one point had different calculations.
+
+        The output is a 2D array of values, essentially the translation of a time into a
+        number of groups (float). 
+
+        Parameters
+        ----------
+        time_to_saturation : np.ndarray
+            2D array of the basic time to saturate (the raw version, merely fullwell/rate)
+            on a per-pixel basis.
+
+        Returns
+        -------
+        np.ndarray
+            2D array of per-pixel groups before saturation.
+        """
         return ((time_to_saturation / self.exposure_spec.tframe) - self.exposure_spec.nframe - self.exposure_spec.ndrop1) / \
                 (self.exposure_spec.nframe + self.exposure_spec.ndrop2) + 1 
 
 class Detector_UnevenMultiAccum(Detector_MultiAccum):
 
     def _power_value(self, snr):
         """
@@ -702,14 +842,32 @@
         mask = self._get_saturation_mask(rate['fp_pix_variance'])
         slope_var[mask==2] = np.nan 
         slope_rn_var[mask==2] = np.nan
 
         return slope_var, slope_rn_var
 
     def weightcalc(self, uns, w_ij, tmean ):
+        """
+        The calculation for multiaccum resultant weights, as a function of the unsaturated
+        number of resultants, tabulated weight, and mean time. Computed per-pixel.
+
+        Parameters
+        ----------
+        uns : float
+            the number of unsaturated resultants, for this pixel.
+        w_ij : np.ndarray
+            1D array of the tabulated weight for each resultant for this pixel.
+        tmean : np.ndarray
+            1D array of the mean time for each resultant.
+
+        Returns
+        -------
+        k_i: np.ndarray
+            1D array of the coefficients for each resultant for this piel
+        """
 
         # Calculate the auxiliary quantities W*t^0, W*t^1, W*t^2, and denomenator.
         # Casertano+22 eq 35
         # except in these arrays, the extra dimension is for unsat_resultants
         # these are resultants+1 because cosmic rays make this short by 1.
         f_0 = np.sum(w_ij[:uns], axis=0)
         f_1 = np.sum(w_ij[:uns] * tmean[:uns], axis=0)
@@ -832,14 +990,32 @@
         # total_frames is really 1D, but it doesn't matter as the broadcasting shape is
         # valid and k_i implicitly handles all resultants that were saturated
         var_rn = np.sum(k_i ** 2 / total_frames, axis = 0) * self.rn**2
 
         return var_rn
 
     def get_slope_variance(self, rate, unsat):
+        """
+        Hook allowing different slope variance behaviors. Multiaccum will override this
+        method to provide unique slope variance functions for regular and TA observations.
+
+        Parameters
+        ----------
+        rate : dict
+            dictionary of source rates (generally variance, with background)
+        unsat : np.ndarray
+            2D array map of the number of unsaturated groups, per pixel.
+
+        Returns
+        -------
+        slope_var: np.ndarray
+            2D array of the total noise.
+        slope_rn_var: np.ndarray
+            2D array of the readnoise component only.
+        """
         slope_var, slope_rn_var = self.slope_variance(rate, unsat)
 
         return slope_var, slope_rn_var
     
     def _frames_before_sat(self, slope):
         """
         To do the actual math of how many resultants we can have, we actually need the
@@ -923,15 +1099,15 @@
 
         Returns
         -------
         unsat_nframes: np.ndarray 
             2D array of unsaturated frames remaining after cosmic ray hits.
         """
         # this is the average fraction of the ramp that is lost upon a CR event
-        if nframes < self.mingroups:
+        if nframes <= self.mingroups:
             # if for some reason (e.g. using single read noise model) ngroup is less than the minimum needed
             # to get a good ramp fit, then the whole ramp is lost upon a CR event
             ramp_frac = 1.0
         else:
             # the more groups you have per ramp, the less of the ramp you lose to CRs on average.
             # this formalism takes into account that there's always a fraction that's totally lost.
             # in the limit of infinite reads this converges on half the ramp since CRs are evenly
@@ -978,26 +1154,45 @@
         return m, tframe
 
 class H4RG(Detector_UnevenMultiAccum):
     """
     Detector properties for H4RG detectors (Roman WFI).
     """
     def set_excess(self, flag):
-        # this function turns excess noise on and off. H4RG detectors do not use excess noise parameters. Warn
-        # if a user tries to turn it on.
+        """
+        Set Excess Noise flag
+
+        H4RG detectors do not use excess noise parameters. Warn if a user tries to turn it
+        on (the values in config.json should be set to 0, so this will do nothing.)
+
+        Parameters
+        ----------
+        flag : bool
+            Boolean to toggle excess noise
+        """
         if flag:
             warnings.warn(f"{type(self).__name__} detectors do not have excess noise parameters, they cannot be turned on.")
 
 #------------ Single accum ------------------
 
 class Detector_SingleAccum(Detector):
 
     def set_excess(self, flag):
-        # this function turns excess noise on and off. SingleAccum detectors do not use H2RG-style excess
-        # noise parameters. Warn if a user tries to turn them on.
+        """
+        Set Excess Noise flag
+
+        SingleAccum detectors do not use H2RG-style excess noise parameters. Warn if a
+        user tries to turn it on (the values in config.json should be set to 0, so this
+        will do nothing.)
+
+        Parameters
+        ----------
+        flag : bool
+            Boolean to toggle excess noise
+        """
         if flag:
             warnings.warn(f"{type(self).__name__} detectors do not have excess noise parameters, they cannot be turned on.")
 
     def postflash_as_rate(self):
         """
         Postflash will not always be defined (and is only valid for some CCDs)
 
@@ -1080,14 +1275,28 @@
         saturation_fraction = self.get_saturation_fraction(rate)
 
         saturation_mask[(saturation_fraction > 1)] = 2
 
         return saturation_mask
 
     def get_unsaturated(self, rate):
+        """
+        Get a map of the 2D pixels that are not saturated.
+
+        Parameters
+        ----------
+        rate : dict
+            dictionary of rate (source flux) products
+
+        Returns
+        -------
+        unsat: ndarray
+            A 2D array, of the same shape as rate, where all pixels whose saturation
+            fraction > 1 have been masked.
+        """
 
         saturation_fraction = self.get_saturation_fraction(rate)
 
         unsat = ma.masked_greater(saturation_fraction, 1)
 
         return unsat
 
@@ -1238,14 +1447,27 @@
         ----------
         wave: 1D numpy.ndarray
             Wavelengths to interpolate chromatic variance over
         """
         return np.ones(len(wave))
 
     def set_time(self, new_time):
+        """
+        Set exposure time
+
+        In a reverse calculation, the 1s initial exposure time must be replaced with the
+        final scaled time (see scale_exposure_time) and the signal and noise recomputed.
+
+        Parameters
+        ----------
+        new_time : float
+            The new exposure time, in seconds.
+
+        """
+
         # See also ExposureSpec.get_times()
 
         # measurement time is the time from the first measurement to the last read of the
         # exposure. HST has no skipped or dropped frames; this is simply the time for one
         # frame.
         self.exposure_spec.measurement_time = new_time / self.exposure_spec.nsplit
 
@@ -1339,15 +1561,15 @@
         wave_index = 0
         wave_pix = extracted['wavelength'] # at worst, this will be backwards from the actual wavelength grid
                                            # but we explicitly use min and max, so this should be fine.
         if len(wave_pix) > 1:
             wref = (wave_pix.max()+wave_pix.min())/2.
             user_wave = calc_input['strategy']['reference_wavelength']
             if user_wave is not None:
-                if user_wave >= wave_pix.min() or user_wave <= wave_pix.max():
+                if user_wave >= wave_pix.min() and user_wave <= wave_pix.max():
                     wref = user_wave
                 # the Report version of this conditional produces a warning here (bad_waveref), but we won't 
                 # bother now and let the Report produce it later.
 
             sbdpr = self.to_resels_scalar(wave_pix, extracted['extracted_flux_plus_bg_all'], wref) # (source + background + dark + postflash) rate
             sr = self.to_resels_scalar(wave_pix, extracted['extracted_flux'], wref) # source rate
             ns = self.to_resels_scalar(wave_pix, extracted['extracted_source_noise'], wref)
@@ -1420,18 +1642,41 @@
         refer to a non-existent concept of read noise)
         """
         Detector_SingleAccum.__init__(self, config, webapp=False)
 
         self.rn_correlation = False
 
     def set_saturation(self, toggle):
+        """
+        Set saturation flag. 
+
+        This method turns saturation on and off. MAMA detectors do not have saturation,
+        and do not run any of the code that sets saturation; this method is therefore
+        superfluous.
+
+        Parameters
+        ----------
+        flag: bool
+            Boolean to toggle saturation
+        """
         # MAMA detector has no concept of saturation, so this is irrelevant.
         pass
 
     def set_readnoise(self, flag):
+        """
+        Set readnoise flag
+
+        This method turns readnoise on and off. MAMA detectors do not have readnoise, so
+        it is always off and the user should be warned if they try to turn it on.
+
+        Parameters
+        ----------
+        flag : bool
+            Boolean to toggle readnoise
+        """
         # this function turns readnoise on and off, but MAMAs do not have readnoise to turn on. Warn if a user
         # tries to turn it on.
         if flag:
             warnings.warn(f"{type(self).__name__} detectors do not have readnoise, it cannot be turned on.")
 
     def get_saturation_fraction(self, rate):
         """
```

### Comparing `pandeia.engine-3.1/pandeia/engine/detector_factory.py` & `pandeia.engine-3.2/pandeia/engine/detector_factory.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/etc3D.py` & `pandeia.engine-3.2/pandeia/engine/etc3D.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # pyfftw.interfaces.cache.enable()
 
 def setup(calc_input, webapp=False, validate=False):
     """
     This generic portion of the code unpacks the input dictionary and uses the 
     pieces to configure the class instances that will perform the calculation.
 
+    Parameters
+    ----------
     calc_input: dict
         Formatted hierarchical calculation input dictionary
     webapp: bool
         Determines whether extra API checks are done
     validate: bool
         Keyword controlling whether intermediate products are saved for validation.
 
@@ -63,14 +65,43 @@
         scene_configuration = build_empty_scene()
 
     strategy = StrategyFactory(instrument, config=strategy_configuration, webapp=webapp, validate=validate)
 
     return calc_config, instrument, strategy, scene_configuration, background, background_level, warnings
 
 def make_observation(calc_config, instrument, strategy, scene, background, background_level, webapp=False, validate=False):
+    """
+    Make Observation
+
+    Principally, this function comprises the generic parts of setting up and making an observation.
+
+    Parameters
+    ----------
+    calc_config: CalculationConfig
+        CalculationConfig instance
+    instrument: Instrument
+        Configured Instrument instance
+    strategy: Strategy
+        Configured Strategy instance
+    scene: Scene
+        Configured Scene instance
+    background: str or list
+        string (as key to background) or list of numpy ndarrays
+    background_level: str
+        String describing background level
+    webapp : bool, optional
+        Flag controlling whether we are in strict API mode, by default False
+    validate : bool, optional
+        Flag controlling whether intermediate products are saved for validation purposes, by default False
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
     # set up the observation and then do S/N calculation...
     obs = observation.Observation(
         scene=scene,
         instrument=instrument,
         strategy=strategy,
         background=background,
         background_level=background_level,
@@ -195,19 +226,20 @@
     Parameters
     ----------
     calc_input: dict
         Engine API format dictionary containing the information required to perform the calculation.
     webapp: bool
         Keyword activating strict checking of API items
     validate: bool
-        Keyword controlling whether intermediate validation products are saved for validation.
+        Keyword controlling whether intermediate products are saved for validation purposes.
 
     Returns
     -------
-    report.Report instance
+    report: Report
+        A filled Report instance
     """
 
     calc_config, instrument, strategy, scene_configuration, background, background_level, warnings = setup(calc_input, webapp=webapp, validate=validate)
 
     # strategies can have different figures of interest that need to be calculated.
     # in most cases, S/N is what is desired. However, for coronagraphy the figure of interest
     # is sometimes the contrast that can be achieved. In this case, strategy.calc_type will be
@@ -276,15 +308,16 @@
     warnings: dict
         A dictionary of warnings produced within all preceeding code.
     webapp: bool
         Control whether we are running in webapp (strict API) mode, or not.
 
     Returns
     -------
-    report.Report instance
+    report: Report
+        A filled Report instance
     """
 
     # We need a regular S/N of the target source
     extracted_sn_list = strategy.extract(my_detector_signal_list, my_detector_noise_list)
     warnings.update(extracted_sn_list[0]['warnings'])
 
     # Use the strategy to get the extracted contrast products
@@ -337,19 +370,20 @@
     Parameters
     ----------
     calc_input: dict
         Dictionary containing the information required to perform the calculation.
     webapp: bool
         Keyword activating strict checking of API items
     validate: bool
-        Keyword controlling whether intermediate products are saved for validation.
+        Keyword controlling whether intermediate products are saved for validation purposes.
 
     Returns
     -------
-    report.Report instance
+    report: Report
+        A filled Report instance
     """
     calc_config, instrument, strategy, scene_configuration, background, background_level, warnings = setup(calc_input, webapp=webapp, validate=validate)
     # do a forward calculation with time=1
     # this sets the time in the calculation 
     instrument.the_detector.set_time(1.0)
 
     # strategies can have different figures of interest that need to be calculated.
```

### Comparing `pandeia.engine-3.1/pandeia/engine/exposure.py` & `pandeia.engine-3.2/pandeia/engine/exposure.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,23 +109,25 @@
         self.get_times()
 
         # Derived quantities
         self.nramps = self.nint * self.nexp
 
     def get_times(self):
         """
-        The time formulae are defined in Holler et al. 2021, JWST-STScI-006013-A. Note that we have to subtract the
-        groups that are rejected (by the pipeline) from the measurement time (nprerej+npostrej). The saturation time
-        conservatively considers the ramp saturated even if saturation occurs in a rejected frame.
-
-        Also note that these equations are generic, suitable for both H2RG and SiAs detectors.
-
-        The equations in this method are duplicated in the front-end
-        (workbook.js, update_detector_time_labels function). Please ensure
-        that changes to these equations are reflected there.
+        The time formulae are defined in Holler et al. 2021, JWST-STScI-006013-A. Note
+        that we have to subtract the groups that are rejected (by the pipeline) from the
+        measurement time (nprerej+npostrej). The saturation time conservatively considers
+        the ramp saturated even if saturation occurs in a rejected frame.
+
+        Also note that these equations are generic, suitable for both H2RG and SiAs
+        detectors.
+
+        The equations in this method are duplicated in the front-end (workbook.js,
+        update_detector_time_labels function). Please ensure that changes to these
+        equations are reflected there.
         """
 
         self.tgroup = self.tframe * (self.nframe + self.ndrop2)
 
         # MIRI measurement time for ngroups < 5 is now handled with dropframes
         # This reduces to Equation 3 for H2RG detectors and Equation 5 for SiAs detectors.
         self.measurement_time = self.nint * self.tframe * (self.ngroup - 1 - self.nprerej - self.npostrej) * (self.nframe + self.ndrop2)
@@ -151,14 +153,19 @@
 
     pass
 
 
 class ExposureSpec_SiAs(ExposureSpec_MultiAccum):
 
     def get_times(self):
+        """
+        SiAs detectors obey the time formulae defined in Holler et al. 2021,
+        JWST-STScI-006013-A. They need two additional values defined, which we compute
+        here.
+        """
         super().get_times()
 
         # This is where we adjust values so we can still use the same
         # MULTIACCUM formula as for the NIR detectors. We need the effective
         # "average time per sample" for MIRI.
         self.tsample = self.tframe / (self.nsample + self.nsample_skip)
         # 'nsample_total' for MIRI is the total number of non-skipped samples X number of averaged frames.
@@ -168,15 +175,15 @@
         self.nsample_total = self.nframe * self.nsample
 
 
 class ExposureSpec_UnevenMultiAccum(ExposureSpec):
 
     def __init__(self, config={}, webapp=False, **kwargs):
         """
-        Create a generic Exposure Specification.
+        Create a generic UnevenMultiAccum Exposure Specification.
 
         Inputs
         ------
         config: dict
             dictionary of detector configuration setups
 
         webapp: bool
@@ -208,15 +215,15 @@
         self.min_resultants = self.ma_table["min_resultants"]
         # Allow a simple "maximum number of resultants" option
         if self.nresultants == -1:
             self.nresultants = self.max_resultants
         # Check, otherwise, for invalid resultant values.
         if self.nresultants > self.max_resultants:
             raise EngineInputError(f"MA Table {self.ma_table_name} supports a maximum of {self.max_resultants} resultants.")
-        if self.nresultants < self.min_resultants:
+        if self.nresultants < 1:
             raise EngineInputError(f"MA Table {self.ma_table_name} supports a minimum of {self.min_resultants} resultants.")
 
         # we've read the full table, now consider only out to the requested stopping
         # point.
         try:
             self.readout_pattern = self._enumerate_pattern()[:self.nresultants]
         except TypeError:
@@ -249,29 +256,42 @@
             frames = frame_counter + resultant["pre_resultant_skips"] + np.arange(resultant["read_frames"])
             readout_pattern.append(list(frames))
             frame_counter += resultant["pre_resultant_skips"] + resultant["read_frames"]
         
         return readout_pattern
 
     def get_times(self):
+        """
+        UnevenMultiaccum detectors follow the multiaccum table definitions specified in the Roman PRD
+        (Roman-STScI-000058 revision J, section 4.6.2) with the addition of the saturation time (utilizing the fact
+        that the detector IS exposing on-sky during the reference read, S. Gomez private
+        communication) which is not precisely the total_accumulated_exposure_time
+        
+        The equations in this method are duplicated in the front-end (workbook.js,
+        update_detector_time_labels function). Please ensure that changes to these
+        equations are reflected there.
+        """
 
         # The frame-based time between the middle of the first and middle of the last readout
+        # Equivalent to total_effective_exposure_time in the PRD (4.6.2, 2.1.14.6)
         if self.nreference > 0:
             self.measurement_time = (self.nreference/2 + np.sum(self.ntotal[0:-1]) + self.ntotal[-1]/2) * self.tframe
         else:
             self.measurement_time = (self.ntotal[0] + np.sum(self.ntotal[1:-1]) + self.ntotal[-1]/2) * self.tframe
 
         # The total time spent on one exposure, including resets
         # Total number of frames + optional reference read + reset read
-        self.exposure_time = 1 * self.treset + self.nreference * self.tframe + self.readout_pattern[-1][-1] * self.tframe
+        # Equivalent to total_integration_duration in the PRD (4.6.2, 2.1.14.7)
+        self.exposure_time = self.nreset * self.treset + self.nreference * self.tframe + self.readout_pattern[-1][-1] * self.tframe
 
         # The total time spent exposing this observation (exposure time, times number of exposures)
         self.total_exposure_time = self.exposure_time * self.nexp
 
         # The time that's important for computing saturation; the time spent collecting photons.
+        # This is the total_accumulated_exposure_time (4.6.2, 2.1.14.5) plus the reference read.
         self.saturation_time = self.nreference * self.tframe + self.readout_pattern[-1][-1] * self.tframe
 
         self.duty_cycle = self.saturation_time/self.exposure_time
         self.nramps = self.nexp
         self.exposures = self.nexp
         self.total_integrations = self.nexp
 
@@ -313,16 +333,20 @@
 
         self.get_times()
 
         # Derived quantities needed for the generic noise equation
         self.nramps = 1
 
     def get_times(self):
-        # See also SingleAccum.set_time()
+        """
+        The following times are defined for use in Pandeia to parallel JWST usage.
 
+
+        See also ExposureSpec_SingleAccum.set_time()
+        """
         # measurement time is the time from the first measurement to the last read of the
         # exposure. HST has no skipped or dropped frames; this is simply the time for one
         # frame.
         self.measurement_time = self.time / self.nsplit
 
         # exposure time is the total time of one exposure (including any skipped reads,
         # reset reads, and the like - HST doesn’t have them.)
```

### Comparing `pandeia.engine-3.1/pandeia/engine/exposure_factory.py` & `pandeia.engine-3.2/pandeia/engine/exposure_factory.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/extinction.py` & `pandeia.engine-3.2/pandeia/engine/extinction.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,22 @@
         if self.webapp:
             self._api_checks(all_config)
 
         # load the extinction curve, i.e. extinction cross section versus wavelength
         self.extinction_wave, self.extinction_curve = self._load_curve()
 
     def _sanity_checks(self):
+        """
+        Check that the input data is valid and usable for this setup.
+
+        Raises
+        ------
+        EngineInputError
+            Invalid extinction unit or invalid extinction bandpass given
+        """
         # make sure we're using a valid unit
         if self.unit not in self.units:
             msg = "Invalid extinction unit, %s, specified ." % self.unit
             raise EngineInputError(value=msg)
 
         # make sure if we're using a bandpass, we have it defined
         if self.unit == "mag":
@@ -137,15 +145,15 @@
         data: dict-like
             Data columns read from extinction data file.
         """
         curve_config = self.laws[self.law]
         filename = os.path.join(default_refdata_directory, "extinction", "curves", curve_config['filename'])
         data = ascii.read(
             filename,
-            Reader=ascii.FixedWidth,
+            format="fixed_width",
             data_start=curve_config['data_start'],
             names=curve_config['names'],
             col_starts=curve_config['col_starts'],
             col_ends=curve_config['col_ends'],
             guess=False
         )
         # make sure the data is sorted in order of increasing wavelength. 'data' is an astropy.table.Table object so has
@@ -263,23 +271,24 @@
 
         return wave, c_ext
 
 
 class Chapman09(Extinction):
 
     """
-    This class implements the extinction law model of Chapman et al. 2009, ApJ, 690, 496.  It is most appropriate for dense
-    molecular clouds and has been derived using mid-IR observations of a set of three molecular clouds: Ophiuchus, Perseus,
-    and Serpens.
+    This class implements the extinction law model of Chapman et al. 2009, ApJ, 690, 496.
+    It is most appropriate for dense molecular clouds and has been derived using mid-IR
+    observations of a set of three molecular clouds: Ophiuchus, Perseus, and Serpens.
     """
 
     def _load_curve(self):
         """
-        The Chapman et al. (2009) model provides the absorption and scattering cross sections separately. These need to be
-        combined and then converted from cm^2/g to cm^2/H.
+        The Chapman et al. (2009) model provides the absorption and scattering cross
+        sections separately. These need to be combined and then converted from cm^2/g to
+        cm^2/H.
 
         Returns
         -------
         wave: np.array
             Wavelength vector of extinction curve
         c_ext: np.array
             Extinction curve
@@ -295,73 +304,75 @@
         # times the dust/ice mass fraction of 1.5 => 3.3e-26 g/H
         c_ext = (3.3e-26 * (ca + cs)) << PANDEIA_FLUXUNITS
 
         return wave, c_ext
 
 class MWRV31(WD2001):
     """
-    This class wraps the md_rv_31 extinction law that is derived from the Weingartner & Draine model for Milky Way
-    extinction with R_V = 3.1
+    This class wraps the md_rv_31 extinction law that is derived from the Weingartner &
+    Draine model for Milky Way extinction with R_V = 3.1
     """
     pass
 
 
 class MWRV40(WD2001):
     """
-    This class wraps the md_rv_40 extinction law that is derived from the Weingartner & Draine model for Milky Way
-    extinction with R_V = 4.0
+    This class wraps the md_rv_40 extinction law that is derived from the Weingartner &
+    Draine model for Milky Way extinction with R_V = 4.0
     """
     pass
 
 
 class MWRV55(WD2001):
     """
-    This class wraps the md_rv_55 extinction law that is derived from the Weingartner & Draine model for Milky Way
-    extinction with R_V = 5.5
+    This class wraps the md_rv_55 extinction law that is derived from the Weingartner &
+    Draine model for Milky Way extinction with R_V = 5.5
     """
     pass
 
 
 class HD210121(WD2001):
     """
-    This class wraps the hd210121 extinction law that is derived from the Weingartner & Draine model for extinction along
-    the line of sight to the high latitude molecular cloud HD 210121.
+    This class wraps the hd210121 extinction law that is derived from the Weingartner &
+    Draine model for extinction along the line of sight to the high latitude molecular
+    cloud HD 210121.
     """
     pass
 
 
 class LMCavg(WD2001):
     """
-    This class wraps the lmc_avg extinction law that is derived from the Weingartner & Draine model for average extinction
-    within the LMC.
+    This class wraps the lmc_avg extinction law that is derived from the Weingartner &
+    Draine model for average extinction within the LMC.
     """
     pass
 
 
 class LMC2(WD2001):
     """
-    This class wraps the lmc_2 extinction law that is derived from the Weingartner & Draine model for a modified versions
-    of the LMC extinction model with C/H = b_C = 10 ppm in log-normal size distributions.
+    This class wraps the lmc_2 extinction law that is derived from the Weingartner &
+    Draine model for a modified versions of the LMC extinction model with C/H = b_C = 10
+    ppm in log-normal size distributions.
     """
     pass
 
 
 class SMCbar(WD2001):
     """
-    This class wraps the smc_bar extinction law that is derived from the Weingartner & Draine model for extinction within
-    the bar region of the SMC.
+    This class wraps the smc_bar extinction law that is derived from the Weingartner &
+    Draine model for extinction within the bar region of the SMC.
     """
     pass
 
 
 def ExtinctionFactory(webapp=False, config={}, **kwargs):
 
     """
-    Function to take extinction configuration data and build/return a configured instance of the appropriate
-    subclass of Extinction.
+    Function to take extinction configuration data and build/return a configured instance
+    of the appropriate subclass of Extinction.
 
     Parameters
     ----------
     webapp: bool
         Switch to toggle strict API checking
     config: dict
         Configuration data in engine API dict format
```

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/butler.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/butler.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,21 +45,22 @@
 
 
 def call_butler(ra, dec, date, level, ra_dec_str, date_str):
 
     if date is not None:
         # dated
 
-        # stray light
-        try:
-            sl_wave, sl_bg = get_stray_light_bg(ra, dec, date, ra_dec_str, date_str)
-        except (StraylightPositionError, StraylightDataError):
-            raise
-        except Exception as e:
-            raise BackgroundError('Error calculating stray light background.', e)
+        if telescope != 'roman':
+            # stray light.  Roman has no stray light.
+            try:
+                sl_wave, sl_bg = get_stray_light_bg(ra, dec, date, ra_dec_str, date_str)
+            except (StraylightPositionError, StraylightDataError):
+                raise
+            except Exception as e:
+                raise BackgroundError('Error calculating stray light background.', e)
 
         # thermal
         try:
             thermal_wave, thermal_bg = get_thermal_bg()
         except Exception as e:
             raise BackgroundError('Error calculating thermal background.', e)
 
@@ -72,46 +73,67 @@
             if "timed out" in str(e):
                 raise BackgroundError("Error calculating infield background: dated background is currently unavailable.  Try again later or switch to low/medium/high")
             else:
                 raise BackgroundError('Error calculating infield background: %s' % e)
 
         # merge wavelengths
         # wave = syn.units.merge_wavelengths(thermal_wave, if_wave)
-        wave = if_wave
+        if telescope == "roman":
+            wave = thermal_wave
+            if_bg = bg_resample(wave, if_wave, if_bg)
+        else:
+            wave = if_wave
+            thermal_bg = bg_resample(wave, thermal_wave, thermal_bg)
 
     else:
 
         # get all components via special get_dateless_bg route if no date given
         try:
             unused_iday, wave, if_bg, sl_bg, thermal_wave, thermal_bg = get_dateless_bg(ra, dec, level)
+            if telescope == "roman":
+                if_bg = bg_resample(thermal_wave, wave, if_bg)
+                wave = thermal_wave
+            else:
+                thermal_bg = bg_resample(wave, thermal_wave, thermal_bg)
+
             # the get_dateless_bg() API returns iday (int day of yr) which we don't currently use
         except (DatelessBGError, StraylightPositionError, StraylightDataError):
             raise
         except Exception as e:
             raise BackgroundError('Error calculating dateless background.', e)
         # wave stands for both if_wave (infield) and sl_wave (straylight)
 
     # resample the flux for each onto the new set
-    if date is not None:
+    if date is not None and telescope != 'roman':
         sl_bg = bg_resample(wave, sl_wave, sl_bg)
-    thermal_bg = bg_resample(wave, thermal_wave, thermal_bg)
-    # if_bg = bg_resample(wave, if_wave, if_bg)
 
     # then sum the backgrounds
     combined_bg = list(map(add, thermal_bg, if_bg))
-    combined_bg = list(map(add, combined_bg, sl_bg))
+
+    if telescope != 'roman':
+        # Don't add straylight for Roman.  It doesn't have any.
+        combined_bg = list(map(add, combined_bg, sl_bg))
 
     # this will be written to a .npz file
-    data_to_save = dict(
-        straylight=sl_bg,
-        thermal=thermal_bg,
-        infield=if_bg,
-        background=combined_bg,
-        wavelength=wave
-    )
+    if telescope == 'roman':
+        # Omit straylight for Roman
+        data_to_save = dict(
+            thermal=thermal_bg,
+            infield=if_bg,
+            background=combined_bg,
+            wavelength=wave
+        )
+    else:
+        data_to_save = dict(
+            straylight=sl_bg,
+            thermal=thermal_bg,
+            infield=if_bg,
+            background=combined_bg,
+            wavelength=wave
+        )
 
     return [list(wave), combined_bg], data_to_save
 
 
 def get_jwst_background(background):
     data_to_save = None
```

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky_angles.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky_angles.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/sky_spectrum.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/sky_spectrum.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/util.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     """
     Safely evaluate an expression node or a string containing a Python
     expression.  The string or node provided may only consist of the following
     Python literal structures: strings, numbers, tuples, lists, dicts, booleans,
     and None.
     """
     _safe_names = {'None': None, 'True': True, 'False': False,
-                   'nan':nan, 'NaN':np.NaN,
-                   'inf':inf, 'Inf':np.Inf}
+                   'nan':nan, 'NaN':np.nan,
+                   'inf':inf, 'Inf':np.inf}
     if isinstance(node_or_string, str):
         node_or_string = ast.parse(node_or_string, mode='eval')
     if isinstance(node_or_string, ast.Expression):
         node_or_string = node_or_string.body
     def _convert(node):
         # Old code used to return instances of ast.Dict. 
         # New code sometimes retuns dicts disguised as lists
```

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/hst/zodi.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/background/hst/zodi.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/accessor_globals.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/accessor_globals.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/bmg_accessor.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/bmg_accessor.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/mod_healpix_func.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/mod_healpix_func.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/background/jwst/sl_accessor_funcs.py` & `pandeia.engine-3.2/pandeia/engine/helpers/background/jwst/sl_accessor_funcs.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/README.md` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/README.md`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/bit.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/bit.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/bit_regenerate_pweb_peng_jeng.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/bit_regenerate_pweb_peng_jeng.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/bit_test_query_to_peng.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/bit_test_query_to_peng.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/compute.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/compute.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/acs_sbc.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/acs_sbc.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/acs_wfc.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/acs_wfc.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/global.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/global.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_ccd.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_ccd.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_fuv-mama.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_fuv-mama.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/stis_nuv-mama.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/stis_nuv-mama.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/config/wfc3_uvis.dict` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/config/wfc3_uvis.dict`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/etc_web_data/extraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/etc_web_data/extraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/etc_web_data/targets.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/etc_web_data/targets.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/extraction.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/extraction.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/input_conversion.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/input_conversion.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/README` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/README`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/custom_configuration.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/custom_configuration.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/data.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/data.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_aperture_fraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_aperture_fraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_limits.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_limits.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/acs_sharpness.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/acs_sharpness.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/detector_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/detector_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/instr_functions.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/instr_functions.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_web.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/acs_web.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_coronography.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_coronography.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_imaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_imaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampcoronography.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampcoronography.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampfilter.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_rampfilter.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_spectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/acs/web/form_fields_acs_spectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_aperture_fraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_aperture_fraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/cos_limits.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/cos_limits.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/custom_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/custom_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/detector_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/detector_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/instr_functions.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/instr_functions.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_web.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/cos_web.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_imaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_imaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopicacq.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_spectroscopicacq.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_targetacquisition.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/cos/web/form_fields_cos_targetacquisition.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/default.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/default.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/scan_mode.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/scan_mode.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/detector_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/detector_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/instr_functions.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/instr_functions.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_aperture_fraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_aperture_fraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_limits.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_limits.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/stis_sharpness.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/stis_sharpness.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_imaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_imaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_spectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_spectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_targetacquisition.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/form_fields_stis_targetacquisition.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_web.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/stis/web/stis_web.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/detector_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/detector_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/instr_functions.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/instr_functions.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_imaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_imaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scimaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scimaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scspectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_scspectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_spectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/form_fields_wfc3ir_spectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_web.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/web/wfc3ir_web.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_aperture_fraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_aperture_fraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_limits.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_limits.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_sharpness.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3ir/wfc3ir_sharpness.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/detector_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/detector_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/instr_functions.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/instr_functions.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_imaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_imaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_scimaging.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_scimaging.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_spectroscopic.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/form_fields_wfc3uvis_spectroscopic.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_web.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/web/wfc3uvis_web.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_aperture_fraction.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_aperture_fraction.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_config.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_config.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_extraction_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_extraction_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_limits.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_limits.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_sharpness.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/hst/wfc3uvis/wfc3uvis_sharpness.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/instruments/telescopes.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/instruments/telescopes.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/perform_calculation.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/perform_calculation.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/README` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/README`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/__init__.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/__init__.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_rampfilter_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/acs_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_specacq_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/cos_targetacquisition_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/map` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/map`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/miri_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nircam_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_defaults.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_defaults.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/nirspec_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/options_map` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/options_map`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/stis_target_acq_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scimaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_scspectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_ir_spectroscopic_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_imaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_scimaging_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_default_input.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_default_input.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_form_options.dat` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_form_defaults/wfc3_uvis_spectroscopy_form_options.dat`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/pyetc_util.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/pyetc_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
     """
     Safely evaluate an expression node or a string containing a Python
     expression.  The string or node provided may only consist of the following
     Python literal structures: strings, numbers, tuples, lists, dicts, booleans,
     and None.
     """
     _safe_names = {'None': None, 'True': True, 'False': False,
-                   'nan':nan, 'NaN':np.NaN,
-                   'inf':inf, 'Inf':np.Inf}
+                   'nan':nan, 'NaN':np.nan,
+                   'inf':inf, 'Inf':np.inf}
     if isinstance(node_or_string, str):
         node_or_string = ast.parse(node_or_string, mode='eval')
     if isinstance(node_or_string, ast.Expression):
         node_or_string = node_or_string.body
     def _convert(node):
         # Old code used to return instances of ast.Dict.
         # New code sometimes retuns dicts disguised as lists
```

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/sky.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/sky.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/source.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/source.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/string_constants.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/string_constants.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/bit/translate.py` & `pandeia.engine-3.2/pandeia/engine/helpers/bit/translate.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/peng/peng3jeng.py` & `pandeia.engine-3.2/pandeia/engine/helpers/peng/peng3jeng.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/helpers/schema/messages.py` & `pandeia.engine-3.2/pandeia/engine/helpers/schema/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     'type': 'object',
     'required': ['bandpass','norm_flux','norm_fluxunit','type'],
     'additionalProperties': False,
     'properties': {
         'bandpass':      {'type': 'string'},
         'norm_flux':     {'type': 'number'},
         'norm_fluxunit': {'type': 'string', 'enum': ['flam','fnu','abmag','vegamag','mjy','ujy','njy','jy','MJy']},
-        'type':          {'type': 'string', 'enum': ['hst','jwst','photsys']},
+        'type':          {'type': 'string', 'enum': ['hst','jwst','photsys','roman']},
     },
 }
 
 an_sed_none = {
     'type': 'object',
     'required': ['sed_type'],
     'additionalProperties': False,
@@ -709,17 +709,29 @@
         'ngroup':          {'type': 'number'},
         'nint':            {'type': 'number'},
         'readout_pattern': {'type': 'string'},
         'subarray':        {'type': 'string'}, # optional
     },
 }
 
+a_detector_roman = {
+    'type': 'object',
+    'required': ['ma_table_name','nexp','nresultants','subarray'],
+    'additionalProperties': False,
+    'properties': {
+        'ma_table_name':   {'type': 'string'},
+        'nexp':            {'type': 'number'},
+        'nresultants':     {'type': 'number'},
+        'subarray':        {'type': 'string'},
+    },
+}
+
 a_detector_for_st = {
     'type': 'object',
-    'oneOf': [a_detector_hst, a_detector_jwst],
+    'oneOf': [a_detector_hst, a_detector_jwst, a_detector_roman],
 }
 
 a_camera_config = {
     'type': 'object',
     'required': ['detector','instrument'],
     'additionalProperties': False,
     'properties': {
@@ -894,14 +906,15 @@
         'a_scene':                      a_scene,
         'a_source':                     a_source,
 
         # config
         'a_detector_for_st':            a_detector_for_st,
         'a_detector_hst':               a_detector_hst,
         'a_detector_jwst':              a_detector_jwst,
+        'a_detector_roman':             a_detector_roman,
         'a_camera_config':              a_camera_config,
         'an_instrument_name':           an_instrument_name,
         'an_instrument_name_hst':       an_instrument_name_hst,
         'an_instrument_name_jwst':      an_instrument_name_jwst,
 
         # calculations
         'a_calculation':                a_calculation,
```

### Comparing `pandeia.engine-3.1/pandeia/engine/hst.py` & `pandeia.engine-3.2/pandeia/engine/hst.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,22 @@
         self.api_ignore = ['dynamic_scene', 'max_scene_size', 'scene_size']
         Instrument.__init__(self, telescope=telescope, mode=mode, config=config, **kwargs)
         # avoid doing the complex obsmode calculations multiple times
         self.obsmode = self.get_obsmode()
         self.rpower, self.dlds, self.dispwave = self.get_dispersion_products()
 
     def get_obsmode(self):
+        """
+        Obtain the correct obsmode string based on the name of the mode.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         if "imagingacq" in self.instrument['mode']:
             obsmode = self._obsmode_ta()
         elif "imaging" in self.instrument['mode']:
             obsmode = self._obsmode_imaging()
         elif "specacq" in self.instrument['mode']:
             obsmode = self._obsmode_specacq()
         elif "spec" in self.instrument['mode']:
@@ -64,21 +72,31 @@
 
         return obsmode
 
     def _obsmode_imaging(self):
         """
         Temporary function for basic imaging obsmodes, to be replaced as we work modes.
         These are likely not correct and not complete, but they should be functional.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
         """
         return "{},{},{}".format(self.instrument['instrument'], self.instrument['detector'], self.instrument['filter'])
 
     def _obsmode_spec(self):
         """
         Temporary function for basic spectroscopic obsmodes, to be replaced as we work modes.
         These are likely not correct and not complete, but they should be functional.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
         """
         if "cenwave" in self.instrument:
             return "{},{},{},{}".format(self.instrument['instrument'], self.instrument['detector'], self.instrument['disperser'], self.instrument['cenwave'])
         else:
             return "{},{},{}".format(self.instrument['instrument'], self.instrument['detector'], self.instrument['disperser'])
 
     def _obsmode_specacq(self):
@@ -337,14 +355,25 @@
             except KeyError as e:
                 msg = "Configuration for slit {} not specified".format(slit)
                 raise DataError(value=msg)
             self.segments = self.read_config_param(slit_config, "range")
         self._loadpsfs()
 
     def get_wave_range(self):
+        """
+        Special replacement function for COS segmented wavelength range definitions.
+
+        Due to API limitations, this function does not and cannot note wavelengths within
+        the detector gaps as unavailable for science.
+
+        Returns
+        -------
+        range_dict: dict
+            Dictionary of wavelength range information
+        """
         if self.projection_type != "image":
             # get the wavelength range from the segments configuration
             disperser = self.instrument['disperser']
             cenwave = self.instrument['cenwave']
             segments = self.segments[disperser][cenwave]
             wmin = None
             wmax = None
@@ -362,30 +391,51 @@
         range_dict = {'wmin': wmin, 'wmax': wmax}
         return range_dict
 
     def _get_psf_key(self):
         """
         The COS PSFs differ greatly by focus position, and we thus need to 
         know lifetime position (currently only LP4), disperser, and cenwave.
+
+        Returns
+        -------
+        psf_key: str
+            String containing the correct PSF key for the instrument setup
         """
         psf_key = self.instrument['aperture']
 
         if self.instrument['mode'] in ["fuv_spec","fuv_specacq", "nuv_spec", "nuv_specacq"]:
             psf_key = "{}{}{}".format(self.instrument['aperture'], self.instrument['disperser'], self.instrument['cenwave'])
         elif self.instrument['mode'] in ["nuv_imaging","nuv_imagingacq"]:
             psf_key = self.instrument['aperture']+self.instrument['slit']
 
         return psf_key
 
     def _obsmode_imaging(self):
+        """
+        Proper format for COS NUV Imaging and ImagingAcq modes, where slit is the final entry.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         items = ['cos',self.instrument['aperture'],self.instrument['detector'], self.instrument['slit']]
         obsmode = ",".join(items)
         return obsmode
 
     def _obsmode_spec(self):
+        """
+        Proper format for COS NUV Spec, FUV Spec, NUV SpecAcq, and FUV SpecAcq modes.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         items = ['cos',self.instrument['detector'],self.instrument['disperser'],str(self.instrument['cenwave']),self.instrument['slit']]
         obsmode = ",".join(items)
         return obsmode
 
     # specacq mode returns the same obsmode as spec - rely on base class directly
     def get_segment_indicies(self, wave):
         """
@@ -521,18 +571,34 @@
     """
     def __init__(self, mode=None, config={}, webapp=False, **kwargs):
 
         HSTInstrument.__init__(self, mode=mode, config=config, webapp=webapp, **kwargs)
         self._loadpsfs()
 
     def _obsmode_imaging(self):
+        """
+        Construct appropriate Obsmode string for UVIS Imaging, IR Imaging, and scan imaging modes.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         obsmode = ",".join(["wfc3",self.instrument['detector'],self.instrument['filter']])
         return obsmode
 
     def _obsmode_spec(self):
+        """
+        Construct appropriate Obsmode string for UVIS Spec, IR Spec, and scan spec modes.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         obsmode = ",".join(["wfc3",self.instrument['detector'],self.instrument['disperser']])
         return obsmode
 
     def add_thermal(self):
         """
         This WFC3-specific functionality adds thermal background if the detector is the WFC3 IR
         detector.
@@ -582,31 +648,50 @@
     def __init__(self, mode=None, config={}, webapp=False, **kwargs):
 
         HSTInstrument.__init__(self, mode=mode, config=config, webapp=webapp, **kwargs)
         self._loadpsfs()
 
     def _obsmode_imaging(self):
         """
-        Polarimeter options are already comma-separated and within the filter keyword.
+        Construct appropriate Obsmode string for ACS WFC Imaging and SBC Imaging modes.
+        Polarimetry is already included in the filter keyword.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for
+            stsynphot.spectrum.band()
         """
         obsmode = "{},{}".format(self.instrument['instrument'], self.instrument['detector'])
         if self.instrument['filter'] != "clear":
             obsmode += ",{}".format(self.instrument['filter'])
         return obsmode
 
     def _obsmode_spec(self):
         """
-        Polarimeter options are already comma-separated and within the disperser keyword.
+        Construct appropriate Obsmode string for ACS WFC Spec and SBC Spec modes.
+        Polarimetry is already included in the disperser keyword.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for
+            stsynphot.spectrum.band()
         """
         obsmode = "{},{},{}".format(self.instrument['instrument'], self.instrument['detector'], self.instrument['disperser'])
         return obsmode
     
     def _obsmode_ramp(self):
         """
-        Polarimeter options are already comma-separated and within the disperser keyword.
+        Construct appropriate Obsmode string for ACS Ramp, including the specification of the Ramp wavelength
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
         """
         obsmode = "{},{},{}#{}".format(self.instrument['instrument'], self.instrument['detector'], self.instrument['filter'], int(self.instrument['wavelength']*10000))
         return obsmode
 
 
 class STIS(HSTInstrument):
 
@@ -643,32 +728,55 @@
         proj_type = super().projection_type
         if proj_type in ("spec", "slitless"):
             if self.instrument['slit'] in self.slitless_slits:
                 proj_type = "slitless"
         return proj_type
 
     def _obsmode_imaging(self):
+        """
+        Construct appropriate Obsmode string for STIS CCD, FUVMAMA, and NUVMAMA Imaging.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         items = ['stis',self.instrument['detector'], 'mirror']
         if self.instrument['filter'] is not None:
             items.append(self.instrument['filter'])
         obsmode = ",".join(items)
         return obsmode
     
     def _obsmode_ta(self):
+        """
+        Construct appropriate Obsmode string for STIS CCD TA. This can optionally include a slit (or filtered slit).
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
+        """
         items = ['stis',self.instrument['detector'], 'mirror']
         if self.instrument['slit'] is not None:
             items.append(self.instrument['slit'])
         obsmode = ",".join(items)
         return obsmode
 
     def _obsmode_spec(self):
         """
-        Much of the PyETC version of this code has to deal with the fact that the web interface
+        Construct appropriate Obsmode string for STIS CCD, FUVMAMA, and NUVMAMA Spec, and the echelle modes.
+
+        Much of the Pyetc version of this code has to deal with the fact that the web interface
         does not contain the prefix character (i or c). In pandeia, the names of the cenwaves include
         the prefix.
+
+        Returns
+        -------
+        obsmode: str
+            Formatted string describing instrument setup, suitable for stsynphot.spectrum.band()
         """
         disperser = self.instrument['disperser']
         detector = self.instrument['detector']
         obsmode = ",".join(['stis', detector, disperser])
 
         cenwave = self.instrument.get('cenwave',None)
         if cenwave != None:
@@ -747,17 +855,21 @@
     def apply_scattering(self, extracted_list):
         """
         Compute and apply the echelle scattered light parameter Will not affect any configuration that does
         not have defined echelle scattering 
 
         Parameters
         ----------
-        wave: numpy.ndarray
-            Wavelength vector to interpolate throughput onto
-        rate: extracted target rate
+        extracted_list: list
+            List of extracted product dictionaries
+        
+        Returns
+        -------
+        extracted_list: list
+            List of extracted product dictionaries, with echelle scattering added to the noise
 
         """
         if hasattr(self.the_detector, "echelle_scattering"):
             for idx in range(len(extracted_list)):
 
                 scatter_rate = self.the_detector.compute_scattering_factor(extracted_list[idx]["wavelength"]) * extracted_list[idx]["extracted_source_noise"]
 
@@ -765,19 +877,24 @@
                 # term.
                 extracted_list[idx]["extracted_noise"] = np.sqrt(extracted_list[idx]["extracted_noise"]**2 + scatter_rate / self.the_detector.exposure_spec.total_exposure_time)
 
         return extracted_list
 
     def get_global_scattering(self):
         """
-        Return the global scattering rate, scattered portion as defined in the data
+        Extract and return the global scattering rate, scattered portion as defined in the data
+
+        Returns
+        -------
+        scatter_rate: float
+            The rate (in counts/s) of the global scattering noise.
         """
         cenwave = self.instrument.get('cenwave', None)
 
-        # No cenwave or cenwave = all will give no detector scattering, but PyETC doesn't make that option
+        # No cenwave or cenwave = all will give no detector scattering, but Pyetc doesn't make that option
         # possible.
         scatter_rate = 0
         if hasattr(self.the_detector, "echelle_global"):
             if cenwave in self.the_detector.echelle_global:
                 scatter_rate = self.the_detector.echelle_global[cenwave] - 1
 
         return scatter_rate
```

### Comparing `pandeia.engine-3.1/pandeia/engine/instrument.py` & `pandeia.engine-3.2/pandeia/engine/instrument.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,32 @@
     There are two reserved words that must not show up as keys:
     * $threshold: The threshold value that triggers the warning.
     * $subthreshold: The fraction of the threshold value that triggers the subthreshold warning (converted to
       a percentage for output)
     Using these in warning messages should help enforce consistency: we don't have to update the message
     every time the number is changed, nor do we have to worry about copy&paste errors.
 
-    :param warnings_list: list of warnings to check for and add to the warnings list
-    :param warnings: warnings dict that is updated by the function with new warnings
-    :param input_dict: input as passed into the function
-    :param value_lookup: dict with lookup lists for each thing we want to check against the warning parameters
-    :param sub_word: str to prefix warning with so that subreports can independently report values
-    :param sub_str: string prefix for warning message
-    :return:
+    Parameters
+    ----------
+    warnings_list: list
+        list of warnings to check for and add to the warnings list
+    warnings: dict 
+        warnings dict that is updated by the function with new warnings
+    input_dict: dict
+        input as passed into the function
+    value_lookup: dict
+        dict with lookup lists for each thing we want to check against the warning parameters
+    sub_word: str 
+        str to prefix warning with so that subreports can independently report values
+    sub_str: str
+        string prefix for warning message
+    
+    Returns
+    -------
+    None. relies on the warnings dictionary attribute being updated in memory.
     """
 
     # Run through each warning in the warnings_list to see if we need to return it.
     for warning in warnings_list:
 
         # Run through all the parameters for this warning to see if all are true
         need_warning = True
@@ -180,15 +191,15 @@
     """
     This is a trivial top-level class for now. It overrides TelescopeConfig._get_config() to get the configuration
     information from a different place, currently under $pandeia_refdata/<tel_name>/<inst_name>
     """
 
     def _get_config(self):
         """
-        Read default source configuration from JSON
+        Read default source configuration from instrument JSON files
 
         Returns
         -------
         config: dict
             All desired class attributes should have defaults defined in the config file
         """
         # use this trick to key the configuration file name off the name of the instantiated subclass
@@ -314,14 +325,31 @@
                 'readout_pattern': ['detector', 'readout_pattern'],
                 'subarray': ['detector', 'subarray']
             }
 
             check_warnings(all_config, self.warnings, self.warning_list_input, value_lookup)
 
     def _nested_api_checks(self, conf, webapp=False):
+        """
+        Function to check API compliance of an input instrument configuration. A missing
+        section is always an error, individual missing keys are only warnings if we are
+        operating in webapp mode. 
+
+        Parameters
+        ----------
+        conf : dict
+            Instrument configuration dictionary
+        webapp : bool, optional
+            Flag to trigger additional API strictness, by default False
+
+        Raises
+        ------
+        DataError
+            Raised if an entire section of instrument configuration is missing.
+        """
         for section in self.instrument_pars:
             for p in self.instrument_pars[section]:
                 # if parameter is not already set, then it's a DataError since config file should have set it to a default.
                 if p not in getattr(self, section):
                     msg = "Missing required %s parameter %s from default configuration for %s." % (
                         section,
                         p,
@@ -349,41 +377,71 @@
         This is only done by JWST and Roman, whose classes will override this function.  For HST, nothing will be done."""
         pass
 
     def _get_psf_key(self):
         """
         Get the PSF key for the current instrument configuration.  Generally, this is just the aperture, but other
         instruments use more complicated logic (COS, NIRCam coronagraphy, etc.).
+
+        Returns
+        -------
+        str
+            the default psf_key is the value of instrument["aperture"]
         """
         return self.instrument['aperture']
 
     def _loadpsfs(self):
         """
         Load the PSF library for the current instrument configuration.  In most cases, this is based on the aperture.
         In some cases (e.g. NIRCam coronagraphy with bar-shaped masks), other configuration parameters come into play.
         """
         self.psf_library = self._load_psf_library(self._get_psf_key())
 
-    def _load_psf_library(self,psf_key):
+    def _load_psf_library(self, psf_key):
+        """
+        Create and return a PSFLibrary instance, based on a psf_key.
+
+        Parameters
+        ----------
+        psf_key : str
+            Key corresponding to a valid PSF sequence for use with a particular instrument configuration
+
+        Returns
+        -------
+        library: PSFLibrary
+            A configured PSFLibrary instance.
+        """
 
         psf_path = os.path.join(self.ref_dir, "psfs")
         library = PSFLibrary(self.get_wave_range(), path=psf_path, psf_key=psf_key)
 
         return library
 
     @property
     def qe_key(self):
         """
-        set default qe_key for looking up QE reference data. MIRI different from others and overloads this.
+        set default qe_key for looking up QE reference data. MIRI operates differently
+        from others and overloads this.
+
+        Returns
+        -------
+        str
+            The default QE keyword
         """
         return 'qe'
 
     def get_detector_pars(self):
         """
-        Create the_detector (and Exposure_Spec) by passing in the appropriate detector_config, subarray_config, and readout_pattern_config options
+        Create and return a Detector instance (and in turn, ExposureSpec instance) by
+        assembling the required configuration parameters from data and user input. 
+        
+        Returns
+        -------
+        the_detector: Detector
+            A configured Detector instance
         """
 
         # this det_dict has been parsed down to key: value pairs for a single detector; self.detector_config is the complete unparsed tree.
         det_dict = self.read_detector_pars() 
 
         detector_config = {"detector_config": det_dict, "subarray_config": self.subarray_config, 
             "readout_pattern_config": self.readout_pattern_config, "input_detector": self.detector}
@@ -434,42 +492,62 @@
             raise ValueError('Only one of rn_fudge or excessp1/p2 maybe used, not both.')
 
         return det_dict
 
     def get_name(self):
         """
         Return instrument's name
+
+        Returns
+        -------
+        str
+            Instrument name
         """
         return self.inst_name
 
     def get_aperture(self):
         """
         Return configured aperture
+
+        Returns
+        -------
+        str
+            Aperture name
         """
         return self.instrument['aperture']
 
     def get_spatial_binning(self):
         """
         Return the spatial-dimension binning values. 
         
         Binning will be an integer or 1 if not present
+
+        Returns
+        -------
+        bin_spatial: int
+            The preconfigured value of spatial binning for this setup
         """
 
         if (("bin_spatial" in self.detector) and not self.the_detector.detector_config.get("has_binning", False)):
             raise EngineInputError(f"Detector does not support pixel binning.")
         bin_spatial = self.detector.get("bin_spatial", 1)
         if (not isinstance(bin_spatial, int)) or (bin_spatial < 1):
             raise EngineInputError(f"Spatial binning value {bin_spatial} invalid. Must be positive integer.")
         return bin_spatial
 
     def get_dispersion_binning(self):
         """
         Return the dispersion-direction binning values. 
         
         Binning will be an integer or 1 if not present
+
+        Returns
+        -------
+        bin_dispersion: int
+            The preconfigured value of dispersion-direction binning for this setup
         """
 
         if (("bin_dispersion" in self.detector) and not self.the_detector.detector_config.get("has_binning", False)):
             raise EngineInputError(f"Detector does not support pixel binning.")
         bin_dispersion = self.detector.get("bin_dispersion", 1)
         if (not isinstance(bin_dispersion, int)) or (bin_dispersion < 1):
             raise EngineInputError(f"Dispersion binning value {bin_dispersion} invalid. Must be positive integer.")
@@ -659,36 +737,38 @@
         fano_factor = (3.0 * q_yield - q_yield**2. - 2.) / q_yield  # two level model, valid for quantum yield between 1 and ~2.
         return q_yield, fano_factor
 
     def apply_scattering(self, extracted):
         """
         Compute additional scattered light term
 
-        This function is overridden when used.
+        This method is a stub that's overridden when used.
         """
 
         return extracted
 
     def get_global_scattering(self):
         """
         Get the global scattering term
 
-        This function is overridden when used.
+        This method is a stub that's overridden when used.
         """
 
         return 0.0
 
     def get_total_eff(self, wave, full_throughput=False):
         """
         Calculate combined throughput of entire telescope/instrument/detector system
 
         Parameters
         ----------
         wave: numpy.ndarray
             Wavelength vector to interpolate throughput onto
+        full_throughput: bool, optional
+            Controls whether certain instrument-specific variants use special behavior. Defaults to false.
 
         Returns
         -------
         eff: numpy.ndarray or float
             Total system throughput as a function of wave
         """
         ote_int = self.telescope.get_ote_eff(wave)
@@ -871,14 +951,18 @@
         to produce that output.
         (NIRSpec does the same thing but with identical detectors that do not have
         health and safety concerns)
 
         Thus, we have both the complete dimensions of the chip (in pixel space) and the 
         portion of the computed spectrum on that chip to consider.
 
+        Returns
+        -------
+        dimensions: list
+            List of chip dimension dictionaries.
         """
         nx = self.the_detector.pixels_x
         ny = self.the_detector.pixels_y
 
         dimensions = [{"name": self.instrument.get("detector","default"), 
                         "size":{"x": nx, "y": ny}, "bounds": {"x": slice(-1), "y": slice(-1)}}]
         return dimensions
@@ -914,14 +998,19 @@
         chromatic so needs to accept an array of wavelengths to interpolate over. By default this returns
         a 1's array the same length as wave scaled by the 'var_fudge' scalar value defined in detector_config.
 
         Parameters
         ----------
         wave: 1D numpy.ndarray
             Wavelengths to interpolate chromatic variance over
+
+        Returns
+        -------
+        variance_fudge: np.ndarray
+            The variance fudge value at the requested wavelengths
         """
         return self.the_detector._get_variance_fudge(wave)
 
     def get_readnoise_correlation_matrix(self, shape):
         """
         Grab correlated readnoise data out of reference file and build a correlation
         matrix out of it.
@@ -998,19 +1087,25 @@
             "rn": {
     			"default": 16.8,
     			"key_format": ["aperture"],
     			"sw": 17
     		},
             "rn_correlation": true
         }
+
+        Parameters
+        ----------
         item: dict
             Dictionary within which we need to search for the correct detector configuration parameter.
         parameter_key: string
             The parameter we want to search for
-        returns: string, int, float, or bool
+
+        Returns
+        -------
+        parameter_value: string, int, float, or bool
              The value of parameter_key for the given instrument and detector setup.
         """
 
         value_lookup = {
             "detector": self.instrument["detector"],
             "aperture": self.instrument["aperture"],
             "disperser": self.instrument["disperser"],
@@ -1073,14 +1168,27 @@
                 raise DataError("Improperly formatted parameter {}".format(item))
         else:
             raise DataError("There is no {} key in {}".format(parameter_key, item))
 
         return parameter_value
 
     def slitlet_grid(self,slitlet):
+        """
+        From a key, look up a slitlet grid definition and translate into a list of actual slitlet positions in slitlet units.
+        
+        Parameters
+        ----------
+        slitlet: str
+            Lookup key for slitlet defined in data
+            
+        Returns
+        -------
+        positions: list
+            List of slitlet positions in the grid of interest
+        """
         nx = self.slitlet_config[slitlet]["nx"]
         ny = self.slitlet_config[slitlet]["ny"]
         xstep = self.slitlet_config[slitlet]["xstep"]
         ystep = self.slitlet_config[slitlet]["ystep"]
         positions = []
         startx = -(nx - 1) / 2.0 * xstep
         stopx = (nx - 1) / 2.0 * xstep
@@ -1179,15 +1287,14 @@
         Collect instrument aperture parameters into a dict and return it
 
         Returns
         -------
         aperture_dict: dict
             Contains the following parameters describing the instrument aperture:
                 pix - pixel scale in arcsec/pixel
-                detector - which detector it goes with
                 plate_scale - pixel scale, y and x dimensions. Should match PSFs. 
                     Defaults to match (pix, pix) if not specified, which may happen when pixels
                     are truly square.
         """
         aperture = self.get_aperture()
         pix = self.aperture_config[aperture]["pix"]
         plate_scale = (self.aperture_config[aperture].get("plate_scale_y", pix), self.aperture_config[aperture].get("plate_scale_x", pix))
@@ -1284,19 +1391,23 @@
         range_dict = {"wmin": wmin, "wmax": wmax}
         return range_dict
 
     @property
     def projection_type(self):
         """
         Determine the appropriate projection type based on the configured instrument mode
+        and tabulated in the telescope configuration.
+
+        Valid options are currently one of "slitless", 'slitless_scan', 'spec', 'image',
+        or 'image_scan'.
 
         Returns
         -------
         proj_type: str
-            The projection type, currently one of 'slitless', 'slitless_scan', 'spec', 'image', or 'image_scan'.
+            The projection type
         """
         mode = self.mode
         slitless_modes = self.telescope.slitless_modes
         spec_modes = self.telescope.spec_modes
         image_modes = self.telescope.image_modes
         if hasattr(self.telescope, 'multiorder_modes'):
             multiorder_modes = self.telescope.multiorder_modes
```

### Comparing `pandeia.engine-3.1/pandeia/engine/instrument_factory.py` & `pandeia.engine-3.2/pandeia/engine/instrument_factory.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/io_utils.py` & `pandeia.engine-3.2/pandeia/engine/io_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 """
 io_utils - commonly used I/O routines for JSON, FITS, and possibly other formats.
 """
 
 import os
 import json
 import errno
+import warnings
 import numpy as np
 import astropy.io.fits as fits
 import astropy.units as u
+from astropy.utils.exceptions import AstropyUserWarning
+import synphot as syn
 
 from .custom_exceptions import EngineInputError, DataError
 from .constants import PANDEIA_WAVEUNITS, PANDEIA_FLUXUNITS, UNIT_MAP
 
 
 class NumPyArangeEncoder(json.JSONEncoder):
 
@@ -262,14 +265,95 @@
                 # recurse !
                 convert_nd2list_in_place(obj[key])
             else:
                 pass # leave this key of dict untouched
     else:
         pass
 
+# This is a copy of the synphot.specio.read_fits_spec function with the following modifications:
+# 1. imports modified to match pandeia
+# 2. Can read in nonstandard FITS files (like SOSS trace files) where the wavelength is not in column 1
+#   and the data of interest is not in column 2
+# 3. Filters out duplicate wavelengths
+# 4. Every file is read in with dimensionless_unscaled as the "flux" unit
+def read_fits_spec(filename, ext=1, wave_col='WAVELENGTH', flux_col='FLUX',
+                   wave_unit=u.AA, flux_unit=u.dimensionless_unscaled):
+    """Read FITS spectrum.
+
+    Wavelength and flux units are extracted from ``TUNIT1`` and ``TUNIT2``
+    keywords, respectively, from data table (not primary) header.
+    If these keywords are not present, units are taken from
+    ``wave_unit`` and ``flux_unit`` instead.
+
+    Parameters
+    ----------
+    filename : str or file pointer
+        Spectrum file name or pointer.
+
+    ext: int
+        FITS extension with table data. Default is 1.
+
+    wave_col, flux_col : str
+        Wavelength and flux column names (case-insensitive).
+
+    wave_unit, flux_unit : str or `~astropy.units.Unit`
+        Wavelength and flux units, which default to Angstrom and FLAM,
+        respectively. These are *only* used if ``TUNIT1`` and ``TUNIT2``
+        keywords are not present in table (not primary) header.
+
+    Returns
+    -------
+    header : dict
+        Primary header only. Extension header is discarded.
+
+    wavelengths, fluxes : `~astropy.units.quantity.Quantity`
+        Wavelength and flux of the spectrum.
+
+    """
+    try:
+        fs = fits.open(filename)
+        header = dict(fs[str('PRIMARY')].header)
+        wave_field = [name.lower() for name in fs[ext].data.names].index(wave_col.lower())
+        flux_field = [name.lower() for name in fs[ext].data.names].index(flux_col.lower())
+        wave_dat = fs[ext].data.field(wave_col).copy()
+        flux_dat = fs[ext].data.field(flux_col).copy()
+        dummy, good = np.unique(wave_dat, return_index=True)
+        wave_dat = wave_dat[good]
+        flux_dat = flux_dat[good]
+        fits_wave_unit = fs[ext].header.get(f'TUNIT{wave_field+1}')
+        fits_flux_unit = fs[ext].header.get(f'TUNIT{flux_field+1}')
+
+        if fits_wave_unit is not None:
+            try:
+                wave_unit = syn.units.validate_unit(fits_wave_unit)
+            except (syn.exceptions.SynphotError, ValueError) as e:  # pragma: no cover  # noqa: E501
+                warnings.warn(
+                    '{0} from FITS header is not valid wavelength unit, using '
+                    '{1}: {2}'.format(fits_wave_unit, wave_unit, e),
+                    AstropyUserWarning)
+
+        if fits_flux_unit is not None:
+            try:
+                flux_unit = syn.units.validate_unit(fits_flux_unit)
+            except (syn.exceptions.SynphotError, ValueError) as e:  # pragma: no cover  # noqa: E501
+                warnings.warn(
+                    '{0} from FITS header is not valid flux unit, using '
+                    '{1}: {2}'.format(fits_flux_unit, flux_unit, e),
+                    AstropyUserWarning)
+
+        wave_unit = syn.units.validate_unit(wave_unit)
+        flux_unit = syn.units.validate_unit(flux_unit)
+
+        wavelengths = wave_dat << wave_unit
+        fluxes = flux_dat << u.dimensionless_unscaled
+    finally:
+        if isinstance(filename, str):
+            fs.close()
+
+    return header, wavelengths, fluxes
 
 def ref_data_interp(filename, wave, colname=None):
     """
     Read reference data from a FITS file and interpolate it to a provided wavelength array
 
     Parameters
     ----------
@@ -281,36 +365,39 @@
         Name of column within the reference file to read and interpolate
 
     Returns
     -------
     interp_col: numpy.ndarray
         Vector containing reference data interpolated onto wave
     """
+    microns_upper = u.def_unit('MICRONS', u.micron)
+    microns = u.def_unit('microns', u.micron)
+    resolution = u.def_unit('resolution', u.dimensionless_unscaled)
+    electronsphoton = u.def_unit('electrons/photon', u.electron/u.photon)
+    u.add_enabled_units([microns, microns_upper, electronsphoton, resolution])
     if colname is None:
         raise EngineInputError(value="Must specify name of column to read from reference file.")
+
     try:
-        data = fits.getdata(filename)
+        # this is a mini version of syn.spectrum.SpectralElement.from_file(), assuming
+        # it's always going to be a .fits file, and that negative values are always
+        # allowed.
+        header, wavelengths, fluxes = read_fits_spec(filename, flux_col=colname)
+        # not everything read in with this function is actually a unitless SpectralElement
+        # (resolving power R, dl/ds, quantum yield, SOSS trace) but SourceSpectrum can't handle
+        # any of them as it requires the "flux" unit to be one of PHOTLAM, FLAM, PHOTNU, FNU, or Jy.
+        data = syn.spectrum.SpectralElement(syn.models.Empirical1D, points=wavelengths, lookup_table=fluxes,
+                keep_neg=True, meta={'header': header})
+
     except IOError as e:
         error_msg = "Error reading reference file: " + filename
         raise DataError(value=error_msg)
-    if np.any(np.diff(data['wavelength']) < 0):
-        indices = np.where(np.diff(data['wavelength']) < 0)[0]
-        error_msg = "Wavelengths must be increasing in reference file: %s\n" % (filename)
-        error_msg += "Out-of-order indices: %s" % repr(indices)
-        raise DataError(value=error_msg)
-    try:
-        columns = set(k.name.lower() for k in data.columns)
-        if colname.lower() not in columns:
-            msg = "Column %s not found in %s" % (colname, filename)
-            raise DataError(value=msg)
-        interp_col = np.interp(wave, data['wavelength'], data[colname])
-    except Exception as e:
-        error_msg = "Error interpolating reference file: %s : %s" % (filename, type(e))
-        raise DataError(value=error_msg)
-    return interp_col
+    interp_col = data(wave << u.micron)
+
+    return interp_col.value
 
 
 def ref_data_column(filename, colname=None, error_msg="Error loading reference file."):
     """
     Read reference data from a FITS file and provide it directly with no interpolation
 
     Parameters
```

### Comparing `pandeia.engine-3.1/pandeia/engine/jwst.py` & `pandeia.engine-3.2/pandeia/engine/jwst.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,18 @@
             self.api_ignore.extend(['dynamic_scene', 'max_scene_size', 'scene_size'])
         else:
             self.api_ignore = ['dynamic_scene', 'max_scene_size', 'scene_size']
 
         Instrument.__init__(self, telescope=telescope, mode=mode, config=config, webapp=webapp, **kwargs)
 
     def read_detector(self):
-        """Read in the detector keyword from the aperture parameter in the config json file.
-           Put the detector keyword in self.instrument['detector']."""
+        """
+        Read in the detector keyword from the aperture parameter in the config json file.
+        Put the detector keyword in self.instrument['detector'].
+        """
         if "slit" in self.aperture_config[self.get_aperture()]:
             self.instrument['slit'] = self.aperture_config[self.get_aperture()]['slit']
         if "detector" not in self.instrument:
             self.instrument['detector'] = self.aperture_config[self.get_aperture()]['detector']
 
 class NIRSpec(JWSTInstrument):
 
@@ -190,14 +192,17 @@
         This also multiplies the internal efficiency by the correction
         factor that showed up after commissioning.
 
         Parameters
         ----------
         wave: numpy.ndarray
             Wavelength vector to interpolate throughput onto
+        full_throughput: bool, optional
+            Specifies whether special throughput handling should be used. 
+            Not active here, only used by methods that override this (HST)
 
         Returns
         -------
         eff: numpy.ndarray or float
             Internal throughput as a function of wave
         """
         if self.mode in ["ifu", "ifu_ver"]:
@@ -213,15 +218,15 @@
         # generate a valid key only for the 3 modes that support correction factors
         # (this will change when more cf files are delivered)
         str_mode = "Nomode" # causes a fall thru to np.ones correction factor
         if "ifu" in self.mode:
             str_mode = "ifu"
         if "fixed_slit" in self.mode or "bots" in self.mode:
             str_mode = "fs"
-        elif "mos" in self.mode:
+        elif "msa" in self.mode:
             str_mode = "mos"
 
         disperser = self.instrument['disperser']
         if disperser is None:
             disperser = 'prism'
         filter = self.instrument['filter']
         if filter is None:
@@ -370,15 +375,15 @@
         ----------
         x: float
             X position (arcsec) in field of view
 
         Returns
         ------
         width: float
-            Width of bar at X in arcsec
+            Width of bar at X, in arcsec
         """
         filt = self.instrument["filter"]
         if "paired_filter" in self.instrument:
             filt = self.instrument["paired_filter"]
         if filt not in self.bar_offsets:
             msg = "Invalid filter, %s, for MASKLWB/MASKSWB." % filt
             raise DataError(value=msg)
@@ -396,14 +401,24 @@
             raise EngineInputError(value=msg)
         return width
 
     def get_detector_qe(self, wave):
         """
         Need to over-ride get_detector_qe() to handle the two different detectors. Which one to use is keyed off
         of the configured aperture.
+
+        Parameters
+        ----------
+        wave: numpy.ndarray
+            wavelengths at which the quantum efficiency is desired, in microns
+
+        Returns
+        -------
+        qe: numpy.ndarray
+            the quantum efficiency of the detector at the input wavelengths
         """
         try:
             detector = self.instrument['detector']
         except KeyError as e:
             msg = "NIRCam aperture configuration must include which detector the aperture belongs to, sw or lw. (%s)" % e
             raise DataError(value=msg)
         qe = self._get_throughput(wave, 'qe_{}'.format(detector))
@@ -490,14 +505,19 @@
 
     def _get_psf_key(self):
         """
         Short-wavelength filters need PSFs that have the CLEAR pupil mask (0.79-2.26 microns)
         Long-wavelength filters need PSFs that have the CLEARP mask (2.37-5.04 microns)
         (See https://jwst-docs.stsci.edu/display/JTI/NIRISS+Overview, Table 2)
         Because the ranges overlap when put on a grid, we need to switch between PSF libraries.
+
+        Returns
+        -------
+        psf_key: str
+            String containing the appropriate psf keyword for this NIRISS observation
         """
         psf_key = self.instrument['aperture']
         if self.instrument['aperture'] == 'imager':
             if self.instrument['filter'] in self.lw_pupil:
                 psf_key = "%s%s" % (self.instrument['aperture'], 'lw')
             else:
                 psf_key = "%s%s" % (self.instrument['aperture'], 'sw')
@@ -578,14 +598,19 @@
         self._loadpsfs()
 
     def _get_psf_key(self):
         """
         The MIRI coronagraphic target acquisition modes use a tiny box that does not include any of the obscuration, and
         only on filters that do not have the coronagraphic occulters included. Therefore, we're using different PSFs
         for them, with aperture names "fqpm1065ta", and similar.
+
+        Returns
+        -------
+        psf_key: str
+            A properly-formatted PSF Keyword for this MIRI observation
         """
         psf_key = self.instrument['aperture']
         
         if (self.instrument['mode'] in ('target_acq')) and (self.instrument['aperture'] in ('fqpm1065', 'fqpm1140',
                                                                                             'fqpm1550', 'lyot2300')):
             psf_key = '{0:}ta'.format(self.instrument['aperture'])            
 
@@ -609,14 +634,24 @@
     def get_variance_fudge(self, wave):
         """
         In addition to a scalar fudge factor, MIRI also has a chromatic variance fudge that correlates with
         the quantum yield. The information posted in Issue #2167 suggests that they want the noise scaled by an extra
         factor of the quantum yield so that the SNR scales inversely with quantum yield. The MIRI team has been asked
         to provide the chromatic fudge factor they want as a separate reference file. Until that's delivered, we'll
         use the quantum yield squared to achieve the desired effect.
+
+        Parameters
+        ----------
+        wave: np.ndarray
+            The wavelength array used in the observation, in microns
+
+        Returns
+        -------
+        var_fudge: np.ndarray
+            The scalar fudge factor sampled at the wavelengths of the observation
         """
         scalar_fudge = self.the_detector._get_variance_fudge(wave)
         q_yield, fano_factor = self.get_quantum_yield(wave)
         var_fudge = scalar_fudge * q_yield**2
 
         return var_fudge
 
@@ -699,18 +734,20 @@
         return disp_axis
 
 def name_mapper(name=None):
     """
     General Purpose name remapping function
     If not fed a name, it returns the mapping dictionary
     If fed a name, it returns either the mapped name or the name (if no mapping is defined)
+
     Parameters
     ----------
     name: string
         The name of a JWST object
+    
     Returns
     -------
     dictionary or string
         Either the remapped string (where necessary) or the complete mapping dictionary.
     """
     short_str_mappings = {
         'nircam ssgrism':  'nircam lw_tsgrism',
```

### Comparing `pandeia.engine-3.1/pandeia/engine/noise.py` & `pandeia.engine-3.2/pandeia/engine/noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         if self.validate:
             self.var_pix, self.stdev_pix, self.var_rn_pix, self.ff_pix = self.on_detector()
         else:
             self.var_pix, self.stdev_pix, self.var_rn_pix = self.on_detector()
 
 
-    def on_detector(self, ff_pix=None):
+    def on_detector(self):
         """
         Calculates the detector plane noise products
 
         Returns
         -------
         products: tuple
             detector_var - numpy.ndarray
@@ -123,16 +123,16 @@
 
         return tuple(output)
 
     def basic_source_noise(self, obs_signal):
         """
         Calculate the noise using the full pixelated flux cube.
 
-        Inputs
-        ------
+        Parameters
+        ----------
         obs_signal: DetectorSignal/CombinedSignal class instance
             Class containing the detector flux plane or plane cube
 
         Returns
         -------
         var_pix_list: List of ndarrays
             The detector variance plane or plane cube
@@ -194,23 +194,22 @@
             products = var_pix_list, stdev_pix_list, rn_var_pix_list, ffnoise_pix_list
         else:
             products = var_pix_list, stdev_pix_list, rn_var_pix_list
         return products
 
     def get_slope_variance(self, rate):
         """
-        Compute the slope variance, based on detector properties and
-        exposure specifications.
+        Compute the slope variance, based on detector properties and exposure
+        specifications.
 
-        Inputs
-        ------
-        rate_per_pix: ndarray
-           The measured slope of the ramp (ie, the rate) per pixel
-           This can be a one-dimensional wavelength spectrum (for a 1D ETC)
-        or a three-dimensional cube ([wave,x,y] for a 3D ETC).
+        Parameters
+        ----------
+        rate: dict
+           dictionary of ramp rate products, usually with all non-target flux sources
+           included.
 
         Returns
         -------
         slope_var: ndarray
            The associated variance of the measured slope
         slope_rn_var: ndarray
            The associated variance of the readnoise only
@@ -233,25 +232,29 @@
 
         slope_var, slope_rn_var = self.the_detector.get_slope_variance(rate, unsat_ngroups)
 
         return slope_var, slope_rn_var
 
     def get_readnoise_slope_variance(self, rate):
         """
-        Compute the variance of the read noise only, excluding all other noise contributions.
+        Compute the variance of the read noise only, excluding all other noise
+        contributions.
 
-        Inputs
-        ------
-        none
+        Parameters
+        ----------
+        rate: dict
+            dictionary of ramp rate products, usually with all non-target flux sources
+            included.
 
         Returns
         -------
         var_rn: ndarray
-            The variance of the readnoise given the current detector slope parameters. Note that
-            if the readnoise is switched off, the associated variance will of course be zero.
+            The variance of the readnoise given the current detector slope parameters.
+            Note that if the readnoise is switched off, the associated variance will of
+            course be zero.
         """
 
         unsat_ngroups = self.the_detector.get_unsaturated(rate['fp_pix_no_ipc'],
                                                         full_saturation=self.the_detector.mingroups)
         # scale the unsaturated ngroups by the CR loss.
         # if (a if condition else b)
         # if the calculation_config value is True or False (edited by user), use True or False. If it's none, use the instrument-team-defined default from detector_config
```

### Comparing `pandeia.engine-3.1/pandeia/engine/normalization.py` & `pandeia.engine-3.2/pandeia/engine/normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         scaled_wave, scaled_flux: 1D np.ndarrays
             Wavelength and scaled flux vectors in pandeia units, microns and mJy
         """
 
         sp = syn.spectrum.SourceSpectrum(Empirical1D, points=wave, lookup_table=flux)
         bp = self._get_bandpass(wave)
         # Check if the flux is less than 1e-10 mJy
-        if integ.trapz(sp(bp.waveset, flux_unit=PANDEIA_FLUXUNITS).value) < MIN_CLIP:
+        if integ.trapezoid(sp(bp.waveset, flux_unit=PANDEIA_FLUXUNITS).value) < MIN_CLIP:
             key = 'normalized_to_zero_flux_bandpass'
             self.warnings[key] = warning_messages[key]
             sp_rn = sp
         else:
             try:
                 sp_rn = sp.normalize(self.norm_flux, band=bp, vegaspec=syn.spectrum.SourceSpectrum.from_vega())
             except Exception as e:
@@ -390,14 +390,24 @@
                 msg += "(%s)" % type(e)
             else:
                 msg += repr(e)
             raise SynphotError(value=msg)
         return bp
 
 
+class NormalizeRoman(NormalizeJwst):
+    """
+    Subclass to normalize a spectrum using Roman filter bandpasses.
+
+    This class functions identically to NormalizeJwst; it uses the Instrument class to get
+    a throughput curve.
+    """
+    pass
+
+
 class NormalizeNone(Normalization):
 
     """
     Subclass to make no normalization look like the other methods.
     """
 
     def normalize(self, wave, flux):
```

### Comparing `pandeia.engine-3.1/pandeia/engine/observation.py` & `pandeia.engine-3.2/pandeia/engine/observation.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/pandeia_warnings.py` & `pandeia.engine-3.2/pandeia/engine/pandeia_warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # warning messages for the instrument class
 instrument_warning_messages = {
     "missing_instrument_api": "Missing {:s} API parameter {:s} for {:s}. Using default value of {:s}.",
     "spectral_resampling_too_small": "Spectrum for source {:s} has been resampled to a spacing " \
                                  "of {} microns for performance reasons. This is smaller " \
                                  "than the minimum spectral resolution {}.",
-    "roman_max_resultants": "Using maximum number of resultants for this MA table ({})"
+    "roman_min_resultants": "Requested number of resultants {} is below the recommended minimum ({})"
 }
 
 source_warning_messages = {
     "source_parameters_missing": "Missing list of required API parameters for source {:s}.",
     "source_parameter_missing": "Source {} configuration missing API parameter, {}. Using the default value of {}."
 }
```

### Comparing `pandeia.engine-3.1/pandeia/engine/perform_calculation.py` & `pandeia.engine-3.2/pandeia/engine/perform_calculation.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,13 +39,28 @@
     if dict_report:
         return report.as_dict()
     else:
         return report
 
 
 def perform_fake_exceptions(calc_input):
+    """
+    Generate fake exceptions for testing
+
+    Parameters
+    ----------
+    calc_input : dict
+        A heirarchical calculation input dictionary
+
+    Raises
+    ------
+    custom_exceptions.PandeiaException
+        Testing exception for custom Pandeia errors
+    Exception
+        Testing exception for generic errors
+    """
     i = calc_input['fake_exception']
     if 'pandeia' in i:
         from . import custom_exceptions
         raise custom_exceptions.PandeiaException("fake pandeia exception for testing")
     if 'exception' in i:
         raise Exception("fake abnormal exception for testing")
```

### Comparing `pandeia.engine-3.1/pandeia/engine/profile.py` & `pandeia.engine-3.2/pandeia/engine/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,49 +102,120 @@
         self.yrot = yrot
         self.pix_area_sqarcsec = src.grid.xsamp * src.grid.ysamp
         self.norm_method = src.shape['norm_method']
         self.geometry = src.shape['geometry']
         self.psf_upsamp = psf_upsamp
 
     def pixelscale(self):
+        """
+        Return a per-pixel normalization factor for the appropriate area unit.
+
+        Returns
+        -------
+        normfactor: float
+            Normalization factor, unitless
+
+        Raises
+        ------
+        EngineInputError
+            Raised on invalid area unit
+        """
         if self.surf_area_units in ['sr']:
             arcsec2 = u.arcsec * u.arcsec
             normfactor = self.pix_area_sqarcsec / u.sr.to(arcsec2)  # convert area in steradians to area in pixels
         elif self.surf_area_units in ['arcsec^2', None]: # 'None' should be an option because integrated flux
                                                         # shouldn't have units (internally, the grid is arcsec)
             normfactor = self.pix_area_sqarcsec
         else:
             msg = "Unsupported surface area unit: %s" % self.surf_area_units
             raise EngineInputError(value=msg)
 
         return normfactor
+    
     def normalize(self):
+        """
+        Normalization chooser
+        """
         options = {'integ_infinity': self.integrate_infinity, 'surf_scale': self.surface_scale,
                        'surf_center': self.surface_center}
         options[self.norm_method]()
 
     def integrate_infinity(self):
+        """
+        Stub method for normalization to total sum
+
+        Raises
+        ------
+        EngineInputError
+            Default not-implemented error
+        """
         msg = "Normalization method {0:} not supported for profile type {1:}".format(self.norm_method, self.geometry)
         raise EngineInputError(value=msg)
 
     def surface_scale(self):
+        """
+        Stub method for normalization at scale radius
+
+        Raises
+        ------
+        EngineInputError
+            Default not-implemented error
+        """
         msg = "Normalization method {0:} not supported for profile type {1:}".format(self.norm_method, self.geometry)
         raise EngineInputError(value=msg)
 
     def surface_center(self):
+        """
+        Stub method for normalization to center/max flux
+
+        Raises
+        ------
+        EngineInputError
+            Default not-implemented error
+        """
         msg = "Normalization method {0:} not supported for profile type {1:}".format(self.norm_method, self.geometry)
         raise EngineInputError(value=msg)
 
     def normalized(self):
+        """
+        Return the normalized profile. If norm_val is set properly (elsewhere) this is all
+        that's needed.
+
+        Returns
+        -------
+        2D numpy.ndarray
+            grid filled with normalized profile
+        """
         return self.prof * self.norm_val
 
     def raw(self):
+        """
+        Return the raw, un-normalized profile. 
+
+        Returns
+        -------
+        2D numpy.ndarray
+            grid filled with raw profile
+        """
         return self.prof
     
     def brightest(self):
+        """
+        Return brightest pixel of profile
+
+        In order to make this independent of offsets, we create a centered but otherwise
+        identical profile on a one-(detector)-pixel grid, and normalize it.
+
+        Returns
+        -------
+        brightest: float
+            The value of the brightest pixel if the profile were centered
+        extemded: bool
+            Whether the source is extended, which triggers different brightest-pixel behavior
+        """
         # make a new 1-pixel grid, shift the source back to center
         self.xoff = 0
         self.yoff = 0
         self.grid = Grid(self.grid.xsamp, self.grid.ysamp, self.psf_upsamp, self.psf_upsamp)
         self.generate()
         norm_prof = self.normalized()
         return np.sum(norm_prof), self.extended
@@ -179,16 +250,19 @@
         self.base_center = 1.0
         self.psf_upsamp = psf_upsamp
         self.grid = src.grid
 
         self.generate()
 
     def generate(self):
-        # This function both creates and fills the point source profile. It should
-        # eventually be refactored to work the same way as other sources
+        """
+        This method both creates and fills the point source profile. It should eventually
+        be refactored to work the same way as other profile types.
+        """
+
         self.prof = self.grid.point_source(xoff=self.xoff, yoff=self.yoff)
 
         self.norm_val = 1
         self.extended = False
 
 class SersicDistribution(Distribution):
     """
@@ -250,26 +324,32 @@
         self.b = sp.gammaincinv(2*self.sersic_index,0.5)
         self.extended = True
         self.base_center = np.e**(self.b)
 
         self.generate()
 
     def generate(self):
+        """
+        Do the work of actually creating the profile and populating the attributes.
+        """
         self.sersic_generator()
 
         self.normalize()
 
     def sersic_generator(self):
         '''
         Generic function to create a properly normalized sersic, taking into account:
-         * Subpixel positioning (off-screen and on) by replicating some of the grid.point_source functionality
-         * Realistic peak counts, by creating a highly oversampled grid covering just the central pixel
-
-        NB: Subclasses should override sersic_func to specify the appropriate equation for the desired distribution.
-        This method will rely on the subclass's sersic_func method.
+         * Subpixel positioning (off-screen and on) by replicating some of the
+           grid.point_source functionality
+         * Realistic peak counts, by creating a highly oversampled grid covering just the
+           central pixel
+
+        NB: Subclasses should override sersic_func to specify the appropriate equation for
+        the desired distribution. This method will rely on the subclass's sersic_func
+        method.
 
         '''
         # oversample the central pixel to compute an actual flux for what may be an extremely tiny peak
         center_grid = Grid(self.grid.xsamp/(SERSIC_OVERSAMPLE-1), self.grid.ysamp/(SERSIC_OVERSAMPLE-1),
                            SERSIC_OVERSAMPLE, SERSIC_OVERSAMPLE)
         yrot,xrot = center_grid.shift_rotate(0, 0, self.pa)
         center_pixel = self.sersic_func(yrot,xrot,self.major,self.minor,self.sersic_index)
@@ -311,24 +391,33 @@
                     xy = np.intersect1d(xvals,yvals)
                     xval = xy // self.grid.shape[1]
                     yval = xy % self.grid.shape[1]
                     partial[xval, yval] = self.center_flux
                 self.prof += partial * frac
 
     def integrate_infinity(self):
+        """
+        Sersic version of normalizing to the entire integrated flux
+        """
         # integrate the Sersic profile to get the total flux for normalization, including flux outside the FOV
         # http://ned.ipac.caltech.edu/level5/March05/Graham/Graham2.html
         integral = self.major * self.minor * 2 * np.pi * self.sersic_index * np.exp(self.b)/(self.b**(2*self.sersic_index))* sp.gamma(2 * self.sersic_index)
         self.norm_val = self.pixelscale() / integral
 
     def surface_scale(self):
+        """
+        Sersic-specific version of normalizing to the scale radius
+        """
         # for the base sersic profile, the flux at R=Re is 1. e^(-b* (1-1))
         self.norm_val = self.pixelscale()
 
     def surface_center(self):
+        """
+        Sersic-specific version of normalizing to the center/max flux
+        """
         # for the base sersic profile, the flux at R=0 is e**b, so we must multiply by e**-b
         self.norm_val = self.pixelscale() * np.e**(-1*self.b)
 
     def sersic_func(self, y, x, major, minor, index):
         """
         Implement the Sersic intensity profile as a function to actually fill the grid with the profile.
         This is Equation 1 of Graham & Driver (2005) 2005PASA...22..118G
@@ -359,57 +448,59 @@
         profile = np.exp( -self.b * (dist**(1.0 / index) - 1) )
 
         return profile
 
 
 class SersicScaleDistribution(SersicDistribution):
     """
-    Create a 2-dimensional elliptical source on the current grid. The intensity
-    profile is described by a Sersic profile, I(r) = I(0) * exp(-(r/r_scale)**(1/n)),
-    where r_scale is the scale length where I(r) = I(0)/e and n is the Sersic index.
-    The ellipticity is governed by specifying major and minor axis scale lengths
-    separately.
-    This is Equation 14 of Graham & Driver (2005) 2005PASA...22..118G
+    Create a 2-dimensional elliptical source on the current grid. The intensity profile is
+    described by a Sersic profile, I(r) = I(0) * exp(-(r/r_scale)**(1/n)), where r_scale
+    is the scale length where I(r) = I(0)/e and n is the Sersic index. The ellipticity is
+    governed by specifying major and minor axis scale lengths separately. This is Equation
+    14 of Graham & Driver (2005) 2005PASA...22..118G
 
 
-    This was the original implementation of the Sersic profile in pandeia, up through version 1.2.2. However, based on
-    community feedback, it was replaced by the above SersicDistribution class. This class was retained but renamed to
-    permit backwards compatibility in the web app.
+    This was the original implementation of the Sersic profile in pandeia, up through
+    version 1.2.2. However, based on community feedback, it was replaced by the above
+    SersicDistribution class. This class was retained but renamed to permit backwards
+    compatibility in the web app.
 
 
     Parameters
     ----------
     src: dict
-        Details of the source geometry to generate, from the Source block of the input files.
+        Details of the source geometry to generate, from the Source block of the input
+        files.
 
     Attributes
     ----------
     minor: float
         Minor axis scale length
     major: float
         Major axis scale length
     pa: float
         Position angle in degrees of major axis measured positive in +X direction
     xoff: float
         Offset in X direction
     yoff: float
         Offset in Y direction
     sersic_index: float
-        Sersic profile shape parameter. 0.5 => gaussian, 1.0 => exponential, 4.0 => de Vaucouleurs
+        Sersic profile shape parameter. 0.5 => gaussian, 1.0 => exponential, 4.0 => de
+        Vaucouleurs
     prof: np.ndarray
         raw 2D profile in detector units
     norm_prof: np.ndarray
         normalized 2D profile in detector units
 
     Methods
     -------
     _integrate_infinity():
         We use an analytical function to represent the integration of the sersic function
-        from -Inf to +Inf in both axes. This will account for flux that falls
-        outside of the FOV.
+        from -Inf to +Inf in both axes. This will account for flux that falls outside of
+        the FOV.
     _surface_center():
         Normalization is to the surface brightness of the center of the profile. This
         formulation is already normalized at that point.
     _surface_scale():
         Normalization is to the surface brightness of a point at the e-folding radius of
         this profile, where intensity is 1/e of the central intensity.
     """
@@ -422,32 +513,33 @@
         self.sersic_index = src.shape['sersic_index']
         self.surf_area_units = src.shape['surf_area_units']
         self.extended = True
         self.base_center = 1.0
 
         self.generate()
 
-    def generate(self):
-
-        # The sersic_generator is inherited from the parent SersicDistribution class, but will correctly use this
-        # class's own sersic_func(), which contains the appropriate equation.
-        self.sersic_generator()
-
-        self.normalize()
-
     def integrate_infinity(self):
+        """
+        Sersic-scale version of normalizing to the entire integrated flux
+        """
         # integrate the Sersic profile to get the total flux for normalization, including flux outside the FOV
         # http://ned.ipac.caltech.edu/level5/March05/Graham/Graham2.html
         integral = self.major * self.minor * 2 * np.pi * self.sersic_index * sp.gamma(2*self.sersic_index)
         self.norm_val = self.pixelscale() / integral
 
     def surface_scale(self):
+        """
+        Sersic-scale version of normalizing to the scale (e-folding) radius
+        """
         self.norm_val = np.e * self.pixelscale()
 
     def surface_center(self):
+        """
+        Sersic-scale vesion of normalizing to the center/max flux
+        """
         self.norm_val = self.pixelscale()
 
     def sersic_func(self, y, x, major, minor, index):
         """
         Implement the Sersic_scale intensity profile as a function to actually fill the grid with the profile.
 
         This distribution function is also replicated in client/js/scenepage.js and should be kept in sync with any
@@ -512,22 +604,14 @@
         self.sersic_index=0.5
         self.surf_area_units = src.shape['surf_area_units']
         self.extended = True
         self.base_center = 1.0
 
         self.generate()
 
-    def generate(self):
-        # The sersic_generator is inherited from the parent SersicDistribution class, but will correctly use
-        # this class's (SersicScaleDistribution) own sersic_func() which contains the appropriate equation for
-        # a gaussian2d function.
-        self.sersic_generator()
-
-        self.normalize()
-
 
 class FlatDistribution(Distribution):
     """
     Implement a source with a constant surface brightness as an ellipse, i.e. a tilted disc.
 
     Parameters
     ----------
@@ -569,23 +653,32 @@
         self.surf_area_units = src.shape['surf_area_units']
         self.extended = True
         self.base_center = 1.0
 
         self.generate()
 
     def generate(self):
+        """
+        Method to generate a flat profile source
+        """
 
         self.prof = self.grid.elliptical_mask(self.major, self.minor, pa=self.pa, xoff=self.xoff, yoff=self.yoff)
 
         self.normalize()
 
     def integrate_infinity(self):
+        """
+        Flat source version of normalizing to the entire integrated flux of the source
+        """
         self.norm_val = self.pixelscale() / (np.pi * self.major * self.minor)
 
     def surface_center(self):
+        """
+        Flat source specific version of normalizing to the central flux
+        """
         self.norm_val = self.pixelscale()
 
 
 class PowerDistribution(Distribution):
     """
     Create a 2-dimensional power law distribution on the current grid. I(r) = I(0) * r**-k
     There is only one configurable parameter, k, which must be positive.
@@ -627,26 +720,32 @@
             raise ValueError('Power Law Index must be positive, not {}'.format(self.power_index))
         self.extended = True
         self.base_center = 1.0
 
         self.generate()
 
     def generate(self):
+        """
+        Method to generate a power-law profile
+        """
 
         self.prof = self.exponential_func(self.yrot, self.xrot, self.r_core, self.power_index)
 
         self.normalize()
 
     #def integrate_infinity(self):
     #    # integrate the Power Law profile to get the total flux for normalization, including flux outside the FOV
     #    # This is two integrations: One over the central circle; one for the exponential profile outside of that.
     #    integral = np.pi * self.r_core**2 + 2* np.pi * self.r_core**2/(self.power_index - 2)
     #    self.norm_prof = self.prof / integral * self.pixelscale()
 
     def surface_center(self):
+        """
+        Power-law-specific version of normalizing to the central flux
+        """
         # the profile comes pre-normalized to 1 at the center.
         self.norm_val = self.pixelscale()
 
     def exponential_func(self, y, x, r_core, index):
         """
         Implement an exponential function. This isn't a pure exponential, because the real one is infinite at dist=0
         but this shares the same basic properties.
```

### Comparing `pandeia.engine-3.1/pandeia/engine/projection.py` & `pandeia.engine-3.2/pandeia/engine/projection.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,14 +43,26 @@
 
     """
 
     def __init__(self):
         pass
 
     def _2d(self, extracted, saturation, signal):
+        """
+        2-D results from a generic projection
+
+        Parameters
+        ----------
+        extracted : dict
+            A Strategy output dictionary
+        saturation : np.ndarray
+            A 2d saturation bitmap
+        signal : DetectorSignal
+            DetectorSignal instance
+        """
 
         self.signal = signal
 
         # Signal and noise in 2D. Get from extracted products
         s = extracted['detector_signal']
         n = extracted['detector_noise']
         t = extracted['detector_saturation']
@@ -68,28 +80,83 @@
         self.saturation = t
         self.ngroups_map = extracted['detector_ngroups']
 
 
 class ImageProjection(Projection):
 
     def _2d(self, extracted, saturation, signal):
+        """
+        Create the Imaging projection 2D products
+
+        Parameters
+        ----------
+        extracted : dict
+            A Strategy extraction dictionary
+        saturation : np.ndarray
+            2D saturation bitmap
+        signal : DetectorSignal
+            A DetectorSignal instance
+
+        Returns
+        -------
+        dict
+            Dict of 2D projection results
+        """
         Projection._2d(self,extracted,saturation,signal)
 
         return {'detector': self.detector_signal, 'snr': self.detector_sn, 'saturation': self.saturation, \
                 'ngroups_map': self.ngroups_map}, self.bg_pix
 
     def _project(self, signal, extracted):
+        """
+        Return the Imaging projection products
+
+        Parameters
+        ----------
+        signal : DetectorSignal
+            A DetectorSignal object
+        extracted : dict
+            A Strategy extraction dictionary
+
+        Returns
+        -------
+        grid: CoordinateGrid or IrregularGrid
+            The observation's *Grid instance
+        wave_pix: np.ndarray
+            The observation's detector wavelength grid
+        pixgrid: CoordinateGrid or IrregularGrid
+            The pixel grid instance.
+        """
 
         return signal.grid, signal.wave_pix, signal.pixgrid_list[0]
 
 class Image_ScanProjection(ImageProjection):
     pass
 class SpecProjection(Projection):
 
     def _2d(self, extracted, saturation, signal):
+        """
+        Create the Spec projection 2D products. Y-dispersed spectra will need to be
+        rotated into the X-axis; X-dispersed spectra merely need to be mirrored vertically
+        to the correct orientation.
+
+        Parameters
+        ----------
+        extracted : dict
+            A Strategy extraction dictionary
+        saturation : np.ndarray
+            2D saturation bitmap
+        signal : DetectorSignal
+            A DetectorSignal instance
+
+        Returns
+        -------
+        dict
+            Dict of 2D projection results
+        """
         Projection._2d(self,extracted,saturation,signal)
 
         if self.signal.dispersion_axis == 'y' and self.signal.current_instrument.instrument["disperser"] != "p750l":  
             # where projection is slitless and axis is y (and not the MIRI p750l disperser)
             # need to rotate these 90 deg clockwise to match our normal axis orientation. np.rot90 only works CCW
             # so we need to rotate 3 times.
             det_sn = np.rot90(self.detector_sn, 3)
@@ -104,21 +171,59 @@
 
         return {'detector_unrotated': self.detector_signal, 'snr_unrotated': self.detector_sn, \
                 'saturation_unrotated': self.saturation, 'ngroups_map_unrotated': self.ngroups_map, \
                 'detector':det_signal, 'snr':det_sn, 'saturation':det_sat, 'ngroups_map': det_groups}, \
                self.bg_pix
 
     def _project(self, signal, extracted):
+        """
+        Return the Spec projection products
+
+        Parameters
+        ----------
+        signal : DetectorSignal
+            A DetectorSignal object
+        extracted : dict
+            A Strategy extraction dictionary
+
+        Returns
+        -------
+        grid: CoordinateGrid or IrregularGrid
+            The observation's *Grid instance
+        extracted_wavelength: np.ndarray
+            The observation's detector wavelength grid
+        pixgrid: CoordinateGrid or IrregularGrid
+            The output pixel grid instance.
+        """
 
         return signal.grid, extracted['wavelength'], signal.pixgrid_list[0]
 
 
 class SlitlessProjection(Projection):
 
     def _2d(self, extracted, saturation, signal):
+        """
+        Create the Slitless projection 2D products. Y-dispersed spectra
+        will need to be rotated into the X-axis; X-dispersed spectra merely need to be
+        mirrored vertically to the correct orientation.
+
+        Parameters
+        ----------
+        extracted : dict
+            A Strategy extraction dictionary
+        saturation : np.ndarray
+            2D saturation bitmap
+        signal : DetectorSignal
+            A DetectorSignal instance
+
+        Returns
+        -------
+        dict
+            Dict of 2D projection results
+        """
 
         Projection._2d(self,extracted,saturation,signal)
 
         if self.signal.dispersion_axis == 'y':
             if self.signal.current_instrument.instrument["disperser"] == "p750l":
                 # y-dispersed spectra need to be flipped vertically.
                 det_signal = self.detector_signal[::-1,:]
@@ -145,15 +250,31 @@
                self.bg_pix
 
     def _project(self, signal, extracted):
         '''
         This function handles (almost) all projection-type dependent factors (which are independent of strategy)
         This primarily includes wave_pix and pix_grid.
 
-        The 2D projection types for slitless and multiorder are handled in _2d()
+        The 2D projection types for slitless are handled in _2d()
+
+        Parameters
+        ----------
+        signal : DetectorSignal
+            A DetectorSignal object
+        extracted : dict
+            A Strategy extraction dictionary
+
+        Returns
+        -------
+        grid: CoordinateGrid or IrregularGrid
+            The observation's *Grid instance
+        wave_pix: np.ndarray
+            The observation's detector wavelength grid
+        pix_grid: CoordinateGrid or IrregularGrid
+            The output pixel grid instance.
         '''
         # this is the spatial grid for the calculation. It needs to be added as an attribute for the
         # common/scene/coordinates tests to work.
         grid = signal.grid
         wave_pix = extracted['wavelength']
         if signal.dispersion_axis == 'y':
             wave_pix = wave_pix[::-1]
@@ -170,27 +291,62 @@
 
 class Slitless_ScanProjection(SlitlessProjection):
     pass
 
 class MultiorderProjection(SlitlessProjection):
 
     def _2d(self, extracted, saturation, signal):
+        """
+        Create the Multiorder projection 2D products. Y-dispersed spectra will need to be
+        rotated into the X-axis but the rotation is different from slitless. We currently
+        have no X-dispersed multiorder spectra.
+
+        Parameters
+        ----------
+        extracted : dict
+            A Strategy extraction dictionary
+        saturation : np.ndarray
+            2D saturation bitmap
+        signal : DetectorSignal
+            A DetectorSignal instance
+
+        Returns
+        -------
+        dict
+            Dict of 2D projection results
+        """
         Projection._2d(self,extracted,saturation,signal)
         
         return {'detector_unrotated': self.detector_signal, 'snr_unrotated': self.detector_sn, \
                 'saturation_unrotated': self.saturation, 'ngroups_map_unrotated': self.ngroups_map, \
                 'detector':np.rot90(self.detector_signal), 'snr':np.rot90(self.detector_sn),
                 'saturation':np.rot90(self.saturation), 'ngroups_map': np.rot90(self.ngroups_map)}, self.bg_pix
 
     def _project(self, signal, extracted):
         '''
         This function handles (almost) all projection-type dependent factors (which are independent of strategy)
         This primarily includes wave_pix and pix_grid.
 
-        The 2D projection types for slitless and multiorder are handled in _2d()
+        The 2D projection types for multiorder are handled in _2d()
+
+        Parameters
+        ----------
+        signal : DetectorSignal
+            A DetectorSignal object
+        extracted : dict
+            A Strategy extraction dictionary
+
+        Returns
+        -------
+        grid: CoordinateGrid or IrregularGrid
+            The observation's *Grid instance
+        wave_pix: np.ndarray
+            The observation's detector wavelength grid
+        pix_grid: CoordinateGrid or IrregularGrid
+            The output pixel grid instance.
         '''
         # this is the spatial grid for the calculation. It needs to be added as an attribute for the
         # common/scene/coordinates tests to work.
         grid = signal.grid
         # this is the wavelength sampling on the detector.
         wave_pix = extracted['wavelength']  # this is already a 1D np.array
```

### Comparing `pandeia.engine-3.1/pandeia/engine/psf_library.py` & `pandeia.engine-3.2/pandeia/engine/psf_library.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/report.py` & `pandeia.engine-3.2/pandeia/engine/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,28 @@
                 if "filter_leak" not in warning:
                     self.r["warnings"][warning] = warnings[warning]
 
         # this must be run last, after the rest of the report has been filled.
         self._web_report()
 
     def _check_output_warnings(self, warning_list_output, sub_word=None, sub_str=''):
+        """
+        Data-driven output warnings. The bulk of the code is handled by instrument.py
+        check_warnings, but we still need to supply the value lookup table that connects
+        the keywords to specific input and output products.
+
+        Parameters
+        ----------
+        warning_list_output : list
+            List of warning definition dictionaries to check against
+        sub_word : int, optional
+            the subreport number, so that subreports can produce individual warnings, by default None
+        sub_str : str, optional
+            Accompanying prefix string for subreports, by default ''
+        """
 
         # merge together input and results dictionaries so the check_warnings
         # function can find everything it needs.
         merged_dict = copy.deepcopy(self.input)
         merged_dict.update(self.r)
 
         # Each thing we want to be able to get the value of in the merged dictionary
@@ -301,14 +315,28 @@
             'max_saturated_pixels': ["scalar", "max_saturated_pixels"],
             'min_snr_threshold': ["scalar", "min_snr_threshold"]
         }
 
         check_warnings(merged_dict, self.warnings, warning_list_output, value_lookup, sub_word=sub_word, sub_str=sub_str)
 
     def _check_output_warnings_bop(self, warning_list_output_bop, sub_word=None, sub_str=''):
+        """
+        Unique health and safety output warnings. Given the different listings, a
+        different value lookup tables are needed.
+
+        Parameters
+        ----------
+        warning_list_output : list
+            List of warning definition dictionaries to check against
+        sub_word : int, optional
+            the subreport number, so that subreports can produce individual warnings, by
+            default None
+        sub_str : str, optional
+            Accompanying prefix string for subreports, by default ''
+        """
 
         # merge together input and results dictionaries so the check_warnings
         # function can find everything it needs.
         merged_dict = copy.deepcopy(self.input)
         merged_dict.update(self.r)
 
         # Each thing we want to be able to get the value of in the merged dictionary
@@ -423,15 +451,16 @@
                 self.warnings["no_waveref"] = warning_messages["no_waveref"].format(self.rw)
         if not hasattr(self.signal.the_detector, "pixels_per_resel"):
             wave_index = (np.abs(self.wave_pix - self.rw)).argmin()
             self.rw = self.wave_pix[wave_index]
 
     def _3dfits(self):
         """
-        Format 3D outputs into fits headers.
+        Format 3D scene cubes into fits headers.
+        Modes that produce 3D outputs (IFUs) override this function.
         """
         for k in ['flux', 'flux_plus_background']:
             self.f['3d'][k] = []
             for i in range(len(self.s['3d'][k])):
                 # the cube data coming out of pandeia.engine is ordered wavelength,x,y which is
                 # backwards from the numpy convention of ordering axes from slowest to fastest.
                 # it is set up this way because we need to broadcast 1D vectors (e.g. throughput
@@ -637,18 +666,20 @@
         max_bright_pixel_rate = max(self.signal.brightest_pixel_rate.values(), key = operator.itemgetter(0))[0]
         self.r['bop']['max_bright_pixel_rate'] = max_bright_pixel_rate
         self.r['bop']['max_bright_pixel_count'] = max_bright_pixel_rate * time
         self.r['bop']['max_total_detector_rate'] = max(self.signal.detector_total_rate.values())
 
     def _3d(self):
         """
-        Compute 3D data products
+        Compute 3D data products. These are the generated scene cubes (not converted to
+        photons, with no telescope throughputs); any mode that produces 3D outputs (IFUs)
+        overrides this method.
         """
 
-        # this is the data cube of the input signal (not converted to photons, with no telescope throughputs)
+        # this is the data cube of the input signal 
         self.flux = self.signal.flux_cube_list
         self.flux_plus_bg = self.signal.flux_plus_bg_list
         self.r['3d']['flux'] = self.flux
 
         # this is the data cube of the input signal plus background
         self.r['3d']['flux_plus_background'] = self.flux_plus_bg
 
@@ -790,16 +821,20 @@
         self.r['scalar']['cr_ramp_rate'] = self.noise.pix_cr_rate * self.r['information']['exposure_specification'][
             'saturation_time']
 
     def _warnings(self, sub_words={'': None, '1':'Dither','2':'Dither', '3': 'Dither'}):
         """
         Collect warnings, and generate saturation warnings
 
-        This module contains both the collected warnings from elsewhere in the program, and also the saturation
-        warnings (which are, currently, the only warnings that may be different between subreports)
+        This module contains both the collected warnings from elsewhere in the program,
+        and also the saturation warnings (which are, currently, the only warnings that may
+        be different between subreports)
+
+        For the duration of generating warnings only, we put some values into the scalar
+        results dict so they can be used in warning checking/generation
 
         Parameters
         -----------
         sub_words : dict
             dict of strings to use when differentiating warning subreports
         """
 
@@ -957,33 +992,40 @@
                     insertion_list = [insertion]
                 category_dict["items"].extend(insertion_list)
             self.r["web_report"].append(category_dict)
 
 
     def _get_report_config(self):
         """
-        Set up formatting for this calculation
+        Set up formatting for this calculation. The order of precedence of report items is:
+          1. Mode-specific section of the inst configuration
+          2. Inst-specific config
+          3. Telescope default
+        
+        Individual modes can remove entries with a special keyword
+
+        Returns
+        -------
+        report_config: dict
+            The full report dictionary to be filled
+        inst_precision: int
+            The floating point precision with which to render values
         """
         tel_config_path = os.path.join(default_refdata_directory, self.tel, "telescope", "report_config.json")
         inst_config_path = os.path.join(default_refdata_directory, self.tel, self.inst, "report_config.json")
         tel_config = read_json(tel_config_path, raise_except=True)
         inst_config = read_json(inst_config_path, raise_except=True)
 
         inst_precision = tel_config["precision"]
         if "precision" in inst_config:
             inst_precision = inst_config["precision"]
             del inst_config["precision"]
         report_config = {category: tel_config[category]['default'] for category in tel_config if category not in ["precision", "-delivered-for-version-"]}
 
         # Order of precedence: (on a section-by-section basis)
-        # 1. Mode-specific section of the inst configuration
-        # 2. Inst-specific config
-        # 3. Telescope default
-        #
-        # Individual modes can remove entries with a special keyword
         for category in inst_config:
             if self.mode in inst_config[category]:
                 report_config[category] = inst_config[category][self.mode]
                 if "delete" in report_config[category]:
                     del report_config[category]
             elif "default" in inst_config[category]:
                 report_config[category] = inst_config[category]["default"]
@@ -992,14 +1034,18 @@
         return report_config, inst_precision
 
     def _key_walk(self, keys, unit, precision):
         """
         Actually walk through the report dictionary to find the value and format it.
         Some very basic processing can be done here.
 
+        Returns
+        -------
+        val: str, list
+            The processed stringified value
         """
         # https://stackoverflow.com/questions/9320335/accessing-python-dict-with-multiple-key-lookup-string
         try:
             val = reduce(dict.get, keys, self.r)
         except TypeError: # Failures to find the key result in a TypeError, not a KeyError.
             val = None
 
@@ -1009,14 +1055,21 @@
 
         val = self._value_process(val, precision)
         return val
 
     def _value_process(self, val, precision, spacing=True):
         """
         Process a value into a string according to what it is
+
+        This method is meant to be run recursively on iterables.
+
+        Returns
+        -------
+        val: str, list
+            The processed value ready for display
         """
         if isinstance(val, (float, np.floating)):
             if val != 0.0 and np.log(abs(val)) < -1*precision:
                 # I put a format string in our format string so we can format our format
                 val = format(val, f" .{precision}e")
             else:
                 val = format(val, f" .{precision}f")
@@ -1063,14 +1116,17 @@
         """
         Report._1d(self)
         # Coronagraphy always has contrast curves
         self.r['1d']['contrast'] = self.extracted['contrast_curve']
         self.curves['contrast'] = self.extracted['contrast_curve']
 
     def _1dfits(self):
+        """
+        Coronagraphy-specific 1D fits values, specifically contrast.
+        """
         Report._1dfits(self)
         # contrast is NOT like the other 1D products and must be handled separately (overwritten).
         tbhdu = fits.BinTableHDU.from_columns([
             fits.Column(name='SEPARATION',
                         unit='arcsec',
                         format="1D",
                         array=self.s['1d']['contrast'][0]),
@@ -1125,24 +1181,30 @@
             contrast_separation = self.input['strategy']['contrast_separation']
             self.r['scalar']['contrast_separation'] = contrast_separation
             self.r['scalar']['contrast_azimuth'] = self.input['strategy']['contrast_azimuth']
             self.r['scalar']['contrast'] = np.interp(contrast_separation, self.extracted['contrast_curve'][0],
                                                 self.extracted['contrast_curve'][1])
 
     def _warnings(self):
+        """
+        Customize the warning strings for coronagraphy
+        """
         Report._warnings(self, sub_words={'': None, '1':'Science Scene', '2':'PSF Subtraction Source', '3':'Contrast Observation'})
 
 class SpecApPhotReport(Report):
     """
     This report class is specifically for Aperture Spectral Extraction
 
     Parameters are read in through Report.__init__
 
     """
     def _scalar(self):
+        """
+        Custom scalar products for SpecApPhot. Specifically, HST instruments should report extraction width and height.
+        """
         Report._scalar(self)
         if isinstance(self.signal.current_instrument, HSTInstrument) and 'extraction_width' in self.extracted and 'extraction_height' in self.extracted:
             self.r['scalar']['extraction_width'] = self.extracted['extraction_width']
             self.r['scalar']['extraction_height'] = self.extracted['extraction_height']
 
 class SpecSegmentedPhotReport(SpecApPhotReport):
     pass
@@ -1199,49 +1261,51 @@
 
     """
 
     def _information(self):
         """
         IFU Aperture Photometry-specific information.
 
-        IFU modes are computed as spectroscopy, but reported as imaging (reconstructed data cubes)
+        IFU modes are computed as spectroscopy, but reported as imaging (reconstructed
+        data cubes)
         """
         Report._information(self)
         # this is used by the UI to decide how to make the plots. even though IFUs are spectroscopic,
         # they're plotted as 2D spatial images. they could be shown as either single planes from the
         # reconstructed cubes or some combination of multiple planes.
         self.r['information']['calc_type'] = "image"
 
     def _projection(self):
         """
         IFU Aperture Photometry-specific projection.
 
-        IFU modes use extracted properties for their projection, and also require wavelength setting in a
-        fashion similar to Aperture Spectral Extraction.
+        IFU modes use extracted properties for their projection, and also require
+        wavelength setting in a fashion similar to Aperture Spectral Extraction.
         """
         self.grid = self.signal.grid
         # for IFUs we want the reconstructed image plane that's build by the strategy
         self.pix_grid = self.extracted['plane_grid']
         self.wave_pix = self.extracted['wavelength']
 
     def _2d(self):
         """
         IFU Aperture Photometry-specific 2D products.
 
-        For IFU modes, all of the 2d outputs of IFUs are linked to the 3D cubes and defined there.
+        For IFU modes, all of the 2d outputs of IFUs are linked to the 3D cubes and
+        defined there.
         """
         pass
 
 
     def _3d(self):
         """
         IFU Aperture Photometry-specific 3D and 2D products.
 
-        IFU modes report 3D data cubes, in addition to the input model cubes all other strategies report. The
-        2D IFU data is taken from slices of these 3D cubes.
+        IFU modes report 3D data cubes, in addition to the input model cubes all other
+        strategies report. The 2D IFU data is taken from slices of these 3D cubes.
         """
         Report._3d(self)
 
         # adding a np.random.randn() instance here operating on self.extracted['detector_signal'], before it's run for
         # cube_sim, will get the same random numbers as the v1.2 and earlier version of Report.py
         # Signal and noise. Get from extracted products
 
@@ -1293,19 +1357,14 @@
             self.f['3d'][key] = o
 
     def _warnings(self):
         """
         Collect warnings for the IFU mode, and generate saturation warnings. This does not call to
         Report._warnings() because ALL of the saturation warnings for IFU modes are different from anywhere
         else.
-
-        Parameters
-        -----------
-        sub_words : dict
-            dict of strings to use when differentiating warning subreports
         """
         sub_words = {'': None, '1': 'Nod 1', '2': 'Nod 2'}
         self.r['warnings'] = self.warnings
         sat_obj = self.cube_saturation[self.wave_index]
 
         self.r['scalar']['n_partial_saturated'] = (sat_obj == 1).sum()
         self.r['scalar']['n_full_saturated'] = (sat_obj == 2).sum()
@@ -1410,14 +1469,20 @@
     """
     This report class is specifically for Spectral Target Acqusition (and its derivatives) 
     
     Parameters are read in through Report.__init__
 
     """
     def _1d(self):
+        """
+        TASpec custom 1D products
+
+        Some TASpec modes require printing out the combined AND individual subreport
+        values, organized by names. For now, those names are hardcoded. 
+        """
         Report._1d(self)
 
         if self.sub_str == "":
             if "acq_mode" in self.input["strategy"] and self.input["strategy"]["acq_mode"] == "acq_peakxd":
                 if "stripe" in self.input["strategy"]:
                     report_mapping = {"a": 0, "b": 1, "c": 2}
                     subreport = report_mapping[self.input["strategy"]["stripe"]]
@@ -1444,15 +1509,15 @@
                     noise = self.signal.the_detector.to_resels_scalar(self.wave_pix, self.extracts[subreport]['extracted_noise'], self.rw)
                     self.r['scalar'][f'sn_per_stripe'][mapping_report[subreport]] =  signal/noise
                     self.r['scalar'][f'time_per_stripe'][mapping_report[subreport]] = self.extracts[subreport]['all_dithers_time']
                     self.r['scalar'][f'reference_wavelength_stripe'][mapping_report[subreport]] = self.extracts[subreport]['wavelength']
 
     def _bop(self):
         """
-        Compute HST's Bright Object Protection (Health and Safety) quantities
+        Compute HST's Bright Object Protection (Health and Safety) quantities for TASpec
         """
         if self.sub_str == "":
             if "acq_mode" in self.input["strategy"] and self.input["strategy"]["acq_mode"] != "acq_peakxd" or "stripe" not in self.input["strategy"]:
                 Report._bop(self)
             else:
                 if "stripe" in self.input["strategy"]:
                     report_mapping = {0: "nuv-a", 1: "nuv-b", 2: "nuv-c"} # this maps stripe names to the subreport we should read them from
```

### Comparing `pandeia.engine-3.1/pandeia/engine/roman.py` & `pandeia.engine-3.2/pandeia/engine/roman.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,29 @@
 
         # these are required for calculation, but ok to live with config file defaults
         self.api_ignore = ['dynamic_scene', 'max_scene_size', 'scene_size']
 
         Instrument.__init__(self, telescope=telescope, mode=mode, config=config, **kwargs)
 
     def read_detector(self):
-        """Read in the detector keyword from the aperture parameter in the config json file.
-           Put the detector keyword in self.instrument['detector']."""
+        """
+        Read in the detector keyword from the aperture parameter in the config json file.
+        Put the detector keyword in self.instrument['detector'].
+        """
         self.instrument['detector'] = self.aperture_config[self.get_aperture()]['detector']
 
 
 class WFI(RomanInstrument):
 
     """
-    Currently, the Roman WFI requires only one method beyond those provided by the generic Instrument class
+    Currently, the Roman WFI requires only one method beyond those provided by the generic
+    Instrument class
+
+    This is also the optimal place to check agreement of MA table and mode, and to
+    implement the nresultants=-1 special behavior.
     """
     def __init__(self, mode=None, config={}, webapp=False, **kwargs):
 
         # We will stick with our own terminology, but allow for someone simply using "optical_element"
         # If present, it supercedes filter and disperser.
         if "optical_element" in config["instrument"]:
             if config["instrument"]["mode"] == "imaging":
@@ -54,28 +60,28 @@
             elif config["instrument"]["mode"] == "spectroscopy":
                 config["instrument"]["disperser"] = config["instrument"]["optical_element"]
                 config["instrument"]["filter"] = None
 
         RomanInstrument.__init__(self, mode=mode, config=config, webapp=webapp, **kwargs)
         self._loadpsfs()
 
-        if config["detector"]["nresultants"] == -1:
-            key = "roman_max_resultants"
-            self.warnings[key] = instrument_warning_messages[key].format(self.the_detector.exposure_spec.max_resultants)
-
         if config["instrument"]["mode"] == "imaging" and config["instrument"]["filter"] not in self.filters:
             raise EngineInputError(f'Invalid filter: {config["instrument"]["filter"]}')
         elif config["instrument"]["mode"] == "spectroscopy" and config["instrument"]["disperser"] not in self.dispersers:
             raise EngineInputError(f'Invalid disperser: {config["instrument"]["disperser"]}')
 
         # Mixing the MA tables will not be allowed, so it should error.
         if self.instrument["mode"] == "imaging" and self.the_detector.exposure_spec.ma_table["observing_mode"] != "WIM":
             raise EngineInputError(f"Invalid MA table {self.the_detector.exposure_spec.ma_table_name} for imaging.")
         if self.instrument["mode"] == "spectroscopy" and self.the_detector.exposure_spec.ma_table["observing_mode"] != "WSM":
             raise EngineInputError(f"Invalid MA table {self.the_detector.exposure_spec.ma_table_name} for spectroscopy.")
+        
+        if self.the_detector.exposure_spec.nresultants < self.the_detector.exposure_spec.min_resultants:
+            key = "roman_min_resultants"
+            self.warnings[key] = instrument_warning_messages[key].format(self.the_detector.exposure_spec.nresultants, self.the_detector.exposure_spec.min_resultants)
 
     def _loadpsfs(self):
         """
         Short-wavelength filters need PSFs with the skinny pupil mask.
         Long-wavelength filters (just f184 and f213 for now) need the wide pupil mask.
         The grism and prism both have their own pupil masks.
         Because the ranges overlap, we need to switch between PSF libraries.
```

### Comparing `pandeia.engine-3.1/pandeia/engine/scene.py` & `pandeia.engine-3.2/pandeia/engine/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,17 @@
     def set_pixsamp(self, xsamp=1.0, ysamp=1.0):
         """
         Set the pixel sampling to apply to the scene
 
         Parameters
         ----------
         xsamp: float
-            Pixel size along the X axis
+            Pixel size along the X axis (default: 1.0)
         ysamp: float
-            Pixel size along the Y axis
+            Pixel size along the Y axis (default: 1.0)
         """
         for s in self.sources:
             s.shape['xsamp'] = xsamp
             s.shape['ysamp'] = ysamp
 
     def get_size(self):
         """
@@ -156,15 +156,15 @@
         Parameters
         ----------
         None
 
         Returns
         -------
         size: float
-            Size of the scene
+            Size of the scene in world coordinates
         """
 
         # The scene size is the maximum (or minimum) x or y offset.
         # It is multiplied by 2 because the 0 position is referenced to the center of the FOV.
         size = 2.0 * np.max([np.max(np.abs([s.position['x_offset'], s.position['y_offset']])) for s in self.sources])
 
         return size
```

### Comparing `pandeia.engine-3.1/pandeia/engine/sed.py` & `pandeia.engine-3.2/pandeia/engine/sed.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         # we need to run the API checks here after merging in the SED type-specific defaults
         if self.webapp:
             all_config = merge_data(config, dict(**kwargs))
             self._api_checks(all_config)
 
     def _get_config(self):
         """
-        Read default configuration from JSON
+        Read default configuration from SED JSON file
 
         Returns
         -------
         config: dict
             All desired class attributes should have defaults defined in the config file
         """
         # use this trick to key the configuration file name off the name of the instantiated subclass
@@ -192,14 +192,28 @@
 
         for par in ["wmin", "wmax", "sampling", "z"]:
             if not hasattr(self, par):
                 msg = "%s spectrum missing %s." % (self.__class__.__name__, par)
                 raise DataConfigurationError(value=msg)
 
     def create_wave(self):
+        """
+        Create an appropriate wavelength grid. Default sampling information is read in
+        from the sed JSON file in a different method.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            The wavelength array in microns
+
+        Raises
+        ------
+        EngineInputError
+            If the grid cannot be created with the input values.
+        """
         # Create a wavelength grid with constant lambda/delta_lambda
         try:
             k = -self.sampling * np.log(self.wmin)
             nw = int(self.sampling * np.log(self.wmax) + k)
             # nw + 1 almost spans the wavelength range, while nw + 2 guarantees 
             # the highest wavelength will be above the requested range and
             # therefore never require any extrapolation.
@@ -211,14 +225,22 @@
                 self.sampling,
                 e
             )
             raise EngineInputError(value=msg)
         return wave << PANDEIA_WAVEUNITS
 
     def create_flux(self):
+        """
+        Create an empty flux array
+
+        Returns
+        -------
+        flux: astropy.units.Quantity
+            (Empty) flux array
+        """
         flux = np.zeros(len(self.wave))
         return flux << PANDEIA_FLUXUNITS
 
 
 class Powerlaw(Analytic):
 
     """
@@ -231,14 +253,28 @@
         """
         for par in ['unit', 'units', 'index']:
             if not hasattr(self, par):
                 msg = "Missing required parameter %s for %s." % (par, self.__class__.__name__)
                 raise DataConfigurationError(value=msg)
 
     def create_flux(self):
+        """
+        Create the flux array. We do this numerically and then convert the result to a
+        Synphot spectrum with the appropriate units.
+
+        Returns
+        -------
+        flux: astropy.units.Quantity
+            The resulting generated spectrum, converted to PANDEIA_FLUXUNITS
+
+        Raises
+        ------
+        SynphotError
+            If conversion to a spectrum in flam or fnu units fails
+        """
         # effectively normalize to 1 mJy at 1 micron and use Normalize() to scale from there
         flux = self.wave.value ** self.index
         if self.unit == 'flam':
             try:
                 # This will be normalized anyway, so the change in units won't matter
                 sp = syn.spectrum.SourceSpectrum(Empirical1D, points=self.wave << PANDEIA_WAVEUNITS, lookup_table=flux << syn.units.FLAM)
                 flux = sp(sp.waveset).value
@@ -281,14 +317,30 @@
                 raise DataConfigurationError(value=msg)
 
         if self.unit not in self.units:
             msg = "Unsupported unit, %s, for %s." % (par, self.__class__.__name__)
             raise EngineInputError(value=msg)
 
     def create_flux(self):
+        """
+        Create a flat source.
+
+        Normally, we could simply use the ConstFlux1D model to have constant flux, but the
+        rest of Pandeia relies on integrated flux at gridded wavelengths.
+
+        Returns
+        -------
+        flux: astropy.units.Quantity
+            The flux array, in PANDEIA_FLUXUNITS
+
+        Raises
+        ------
+        SynphotError
+            If conversion to a spectrum in flam or fnu units fails
+        """
         if self.unit == 'flam':
             try:
                 # Make sure this spectrum is created in FLAM units
                 sp = syn.spectrum.SourceSpectrum(ConstFlux1D, amplitude=1*syn.units.FLAM)
                 flux = sp(self.wave)
             except Exception as e:
                 msg = "Error converting flam units to Pandeia flux units via Synphot for Flat spectrum. "
@@ -325,14 +377,23 @@
         """
         Analytic._sanity_checks(self)
         if not hasattr(self, 'temp'):
             msg = "Missing required parameter 'temp' for %s." % self.__class__.__name__
             raise DataConfigurationError(value=msg)
 
     def create_flux(self):
+        """
+        Create a blackbody flux array. Synphot can create an object, but the rest of
+        Pandeia requires a sampled array.
+
+        Returns
+        -------
+        flux: astropy.units.Quantity
+            The flux array, in normalizeable units.
+        """
         # use astropy analytic function and astropy.units to specify microns and K.
         # flux is in erg cm-2 s-1 hz-1 sr-1, but will be scaled by normalization.
         bb = Black_Body(temperature=self.temp * u.K)
         flux = bb(self.wave)
         # because it's in units that include steradian, we need to multiply by steradian to take them out
         # This will be normalized anyway.
         return flux * u.sr
@@ -412,14 +473,21 @@
         Parameterized.__init__(self, webapp=webapp, config=config, **kwargs)
 
     def get_spectrum(self):
         """
         Use stsynphot.grid_to_spec() to calculate spectrum and convert to microns/mJy.  If
         self.key is defined, use key to look up a specified set of parameters.  Otherwise,
         get them from the configured attributes.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            Wavelength of the spectrum.
+        flux: astropy.units.Quantity
+            Flux of the spectrum, in PANDEIA_FLUXUNITS
         """
         if hasattr(self, "teff"):
             m = self.metallicity
             t = self.teff
             g = self.log_g
         else:
             if self.key not in self.spectra:
@@ -467,14 +535,21 @@
         Parameterized.__init__(self, webapp=webapp, config=config, **kwargs)
 
     def get_spectrum(self):
         """
         Use stsynphot.grid_to_spec() to calculate spectrum and convert to microns/mJy.  If
         self.webapp=True, use key to look up a specified set of parameters.  Otherwise,
         get them from the configured attributes.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            Wavelength of the spectrum.
+        flux: astropy.units.Quantity
+            Flux of the spectrum, in PANDEIA_FLUXUNITS
         """
         if hasattr(self, "teff") and hasattr(self, "log_g"):
             m = 0
             t = self.teff
             g = self.log_g
         else:
             if self.key not in self.spectra:
@@ -520,16 +595,23 @@
             self.api_ignore = ["spectrum_id", "key",  "comment", "display_string", "spectra", "z"]
 
         Parameterized.__init__(self, webapp=webapp, config=config, **kwargs)
 
     def get_spectrum(self):
         """
         Use stsynphot.grid_to_spec() to calculate spectrum and convert to microns/mJy.  If
-        self.webapp=True, use key to look up a specified set of parameters.  Otherwise,
+        self.webapp=True, use key to look up a specified set of parameters. Otherwise,
         get them from the configured attributes.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            Wavelength of the spectrum.
+        flux: astropy.units.Quantity
+            Flux of the spectrum, in PANDEIA_FLUXUNITS
         """
         if hasattr(self, "teff") and hasattr(self, "log_g"):
             m = 0
             t = self.teff
             g = self.log_g
         else:
             if self.key not in self.spectra:
@@ -576,24 +658,30 @@
         self.spectra = read_json(spectra_file)
         self.wave, self.flux = self.get_spectrum()
         self.wmin = self.wave.min()
         self.wmax = self.wave.max()
 
     def _sanity_checks(self):
         """
-        Make sure a key is provided
+        Make sure a lookup key is provided
         """
         if not hasattr(self, "key"):
             msg = "Must provide a key for looking up a SED."
             raise DataConfigurationError(value=msg)
 
     def get_spectrum(self):
         """
         Use self.key to grab filename out of self.spectra and load data using Synphot.
-        Return wave and flux in microns and mJy.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            Wavelength of the spectrum.
+        flux: astropy.units.Quantity
+            Flux of the spectrum, in PANDEIA_FLUXUNITS
         """
         if self.key not in self.spectra:
             msg = "Provided SED key, %s, not supported." % self.key
             raise EngineInputError(value=msg)
 
         filepath = os.path.join(default_refdata_directory,
                                 "sed",
@@ -619,15 +707,21 @@
     """
     Class implementing SED's that are looked-up from CDBS via an input 'key' and loaded from a file.
     """
 
     def get_spectrum(self):
         """
         Use self.key to grab filename out of self.spectra and load data using Synphot.
-        Return wave and flux in microns and mJy.
+
+        Returns
+        -------
+        wave: astropy.units.Quantity
+            Wavelength of the spectrum.
+        flux: astropy.units.Quantity
+            Flux of the spectrum, in PANDEIA_FLUXUNITS
         """
         if self.key not in self.spectra:
             msg = "Provided SED key, %s, not supported." % self.key
             raise EngineInputError(value=msg)
 
         filepath = os.path.join(os.environ['PYSYN_CDBS'],
                                 self.spectra[self.key]['filename'])
@@ -789,16 +883,16 @@
     """
 
     pass
 
 
 def SEDFactory(webapp=False, config={}, **kwargs):
     """
-    Function to take configuration data and build/return an appropriately configured instance
-    of the desired SED class.
+    Function to take configuration data and build/return an appropriately configured
+    instance of the desired SED class.
 
     Parameters
     ----------
     webapp: bool
         Switch to toggle strict API checking
     config: dict
         Configuration data in engine API dict format
```

### Comparing `pandeia.engine-3.1/pandeia/engine/signal.py` & `pandeia.engine-3.2/pandeia/engine/signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,23 +140,24 @@
 
         # now compute the products of the 2D projection 
         self.signal_products()
 
 
     def slice_products(self, projected_rate, projected_rate_plus_bg):
         """
-        Compute per-slice products from the projected 2D slice with post-projection detector effects added
+        Compute per-slice products from the projected 2D slice with post-projection
+        detector effects added
         
         Parameters
         ----------
         projected_rate: dict
             A dictionary of 2D-projected signal from the rate cube.
         projected_rate_plus_bg: dict
-            A dictionary of 2D-projected signal+background from the rate_plus_bg cube that will contain all
-            other effects.
+            A dictionary of 2D-projected signal+background from the rate_plus_bg cube that
+            will contain all other effects.
         """
         # apply detector effects to the projected products for this slice
         slice_rate = self.apply_detector_effects(projected_rate, add_flux_sources=False)
         slice_rate_plus_bg = self.apply_detector_effects(projected_rate_plus_bg, add_flux_sources=True)
         # Saturation map for the slice
         slice_saturation = self.the_detector._get_saturation_mask(slice_rate_plus_bg['fp_pix_no_ipc_unbinned'])
         slice_group = self.the_detector.get_before_sat(slice_rate_plus_bg['fp_pix_unbinned'])
@@ -172,15 +173,16 @@
         self.rate_plus_bg_list.append(slice_rate_plus_bg)
         self.saturation_list.append(slice_saturation)
         self.groups_list.append(slice_group)
         self.pixgrid_list.append(slice_pixgrid)
 
     def signal_products(self):
         """
-        Compute per-signal products from the projected 2D slice with post-projection detector effects added
+        Compute per-signal products from the projected 2D slice with post-projection
+        detector effects (dark current, postflash, wfc3 thermal) added.
         These will constitute the main interface and products used in DetectorSignal.
         
         """
         # Initialize slice lists
         self.rate_list = []
         self.rate_plus_bg_list = []
         self.saturation_list = []
@@ -412,15 +414,28 @@
             detector[i * aperture_sh[0]:(i + 1) * aperture_sh[0], :] = rate[product_name]
             i += 1
 
         return detector
 
     def get_pix_grid(self, rate):
         """
-        Generate the coordinate grid of the detector plane
+        Generate the coordinate grid of the detector plane. This is useful for
+        spectroscopic projections, where up until this point the grid has been that of the
+        2D scene, not its spectroscopic projection.
+
+        Parameters
+        ----------
+        rate: dict
+            Rate product dictionary
+
+        Returns
+        -------
+        grid: IrregularGrid
+            An IrregularGrid instance
+
         """
         if self.projection_type in ('image', 'image_scan'):
             grid = self.grid
         elif self.projection_type in ('spec', 'slitless', 'slitless_scan', 'multiorder'):
             nw = rate['wave_pix'].shape[0]
             if self.dispersion_axis == 'x':
                 # for slitless calculations, the dispersion axis is longer than the spectrum being dispersed
@@ -464,16 +479,16 @@
             raise EngineOutputError("Focal Plane Rate Cube unavailable. Recompute with validate=True.")
 
     def _build_dark_array(self, wave, size_y):
         '''
         Builds the dark current array, in case there is more than one value of dark current. Case in point:
         segmented detectors such as COS FUV.
 
-        This operates by replacing the dark_current value in the detector instance, originally a dict, with a
-        2D array with the proper dark values filling their corresponding slices on the array.
+        This operates by replacing the dark_current value in the detector instance, originally a float, with a
+        2D array where the proper dark values fill their corresponding slices on the array.
 
         Parameters
         ----------
         wave: numpy.ndarray
             Wavelength array.
         size_y: int
             Size of array in the Y direction
@@ -781,25 +796,25 @@
             first element - electron rate per pixel
             second element - photon rate per pixel (no quantum yield)
             third element - variance of electron rate per pixel
         '''
         q_yield, fano_factor = self.current_instrument.get_quantum_yield(self.wave)
 
         # convert the photon rate to electron rate by multiplying by the quantum yield which is a function of wavelength
-        electron_rate_pix = integrate.trapz(rate * q_yield, self.wave)
-        image_rate_no_qyield = integrate.trapz(rate, self.wave)
+        electron_rate_pix = integrate.trapezoid(rate * q_yield, self.wave)
+        image_rate_no_qyield = integrate.trapezoid(rate, self.wave)
 
         # to meet IDT expectations, some instruments require a possibly chromatic fudge factor to be applied
         # to the per-pixel electron rate variance.
         var_fudge = self.current_instrument.get_variance_fudge(self.wave)
 
         # the variance in the electron rate, Ve, is also scaled by the quantum yield plus a fano factor which is
         # analytic in the simple 1 or 2 electron case: Ve = (qy + fano) * Re.  since Re is the photon rate
         # scaled by the quantum yield, Re = qy * Rp, we get: Ve = qy * (qy + fano) * Rp
-        electron_variance_pix = integrate.trapz(rate * q_yield * (q_yield + fano_factor) * var_fudge, self.wave)
+        electron_variance_pix = integrate.trapezoid(rate * q_yield * (q_yield + fano_factor) * var_fudge, self.wave)
 
         # bin the instrument wavelength grid in pixels
         bin_x = self.current_instrument.get_spatial_binning()
         bin_y = self.current_instrument.get_spatial_binning()
         self.binning = DetectorBinning(electron_rate_pix, bin_x, bin_y, self.grid)
 
         products = electron_rate_pix, image_rate_no_qyield, electron_variance_pix
@@ -1025,14 +1040,16 @@
 
 
     def observation_scan(self, product, bgvals, add_extended_background=True):
         '''
         Calculate the scan effect. We build up the actual detector plane by shifting and adding an appropriate 
         amount of the previously-projected image, and then rebuild the Grid.
 
+        Scans are only ever done along the 0 degree line.
+
         How this works:
         1. We calculate the scan properties
         2. We calculate the actual scan length in pixels.
         3. We divide the existing products by that length, as it will be divided out into those pixels.
         4. We shift and add the product to the new array
         5. If add_extended_background = True, we add the background to the parts of the new array not covered 
            by the shifted product.
@@ -1151,17 +1168,17 @@
                                           kind='linear', assume_sorted=True, copy=False)
         bg_fp_rate_pix = int_bg_fp_rate(wave_pix)
         q_yield, fano_factor = self.current_instrument.get_quantum_yield(wave_pix)
         # To meet IDT expectations, some instruments require a possibly chromatic fudge factor to be applied
         # To the per-pixel electron rate variance.
         var_fudge = self.current_instrument.get_variance_fudge(wave_pix)
         # Calculate electron rate and variance due to background (per wavelength -> scalar)
-        bg_electron_rate = integrate.trapz(bg_fp_rate_pix * q_yield, wave_pix)
-        bg_rate_no_qyield = integrate.trapz(bg_fp_rate_pix, wave_pix)
-        bg_electron_variance = integrate.trapz(bg_fp_rate_pix * q_yield * (q_yield + fano_factor) * var_fudge, wave_pix)
+        bg_electron_rate = integrate.trapezoid(bg_fp_rate_pix * q_yield, wave_pix)
+        bg_rate_no_qyield = integrate.trapezoid(bg_fp_rate_pix, wave_pix)
+        bg_electron_variance = integrate.trapezoid(bg_fp_rate_pix * q_yield * (q_yield + fano_factor) * var_fudge, wave_pix)
 
         # Scan the projection.
         fp_pix_rate = self.observation_scan(fp_pix_rate, bg_electron_rate, add_extended_background=add_extended_background)
         fp_pix_no_qyield = self.observation_scan(fp_pix_no_qyield, bg_rate_no_qyield, add_extended_background=add_extended_background)
         fp_pix_variance = self.observation_scan(fp_pix_variance, bg_electron_variance, add_extended_background=add_extended_background)
 
         # Expand the grid so we can extract a box that tall.
@@ -1225,17 +1242,17 @@
         bg_fp_rate_pix = int_bg_fp_rate(self.wave)
 
         q_yield, fano_factor = self.current_instrument.get_quantum_yield(self.wave)
         # To meet IDT expectations, some instruments require a possibly chromatic fudge factor to be applied
         # To the per-pixel electron rate variance.
         var_fudge = self.current_instrument.get_variance_fudge(self.wave)
         # Calculate electron rate and variance due to background (per wavelength -> scalar)
-        bg_electron_rate = integrate.trapz(bg_fp_rate_pix * q_yield, self.wave)
-        bg_rate_no_qyield = integrate.trapz(bg_fp_rate_pix, self.wave)
-        bg_electron_variance = integrate.trapz(bg_fp_rate_pix * q_yield * (q_yield + fano_factor) * var_fudge, self.wave)
+        bg_electron_rate = integrate.trapezoid(bg_fp_rate_pix * q_yield, self.wave)
+        bg_rate_no_qyield = integrate.trapezoid(bg_fp_rate_pix, self.wave)
+        bg_electron_variance = integrate.trapezoid(bg_fp_rate_pix * q_yield * (q_yield + fano_factor) * var_fudge, self.wave)
 
         # Scan the projection.
         fp_pix_rate = self.observation_scan(fp_pix_rate, bg_electron_rate, add_extended_background=add_extended_background)
         fp_pix_no_qyield = self.observation_scan(fp_pix_no_qyield, bg_rate_no_qyield, add_extended_background=add_extended_background)
         fp_pix_variance = self.observation_scan(fp_pix_variance, bg_electron_variance, add_extended_background=add_extended_background)
  
         # Expand the grid so we can extract a box that tall.
@@ -1253,14 +1270,23 @@
         self.binning = DetectorBinning(fp_pix_rate, bin_x, bin_y, self.grid)
 
         products = wave_pix, fp_pix_rate, fp_pix_no_qyield, fp_pix_variance
 
         return products
 
     def wave_eff(self, rate):
+        """
+        Compute the effective wavelength of the observation. This is a different
+        calculation from the one done by Synphot.
+
+        Returns
+        -------
+        wave_eff_arr: np.ndarray
+            The effective wavelength as a single-element ndarray
+        """
         if len(rate.shape) > 1:
             rate_tot = np.nansum(rate, axis=0)
         else:
             rate_tot = rate
         a = np.sum(rate_tot * self.wave)
         b = np.sum(rate_tot)
 
@@ -1268,17 +1294,40 @@
             wave_eff = a / b
         else:
             wave_eff = self.wave.mean()
         wave_eff_arr = np.array([wave_eff])
         return wave_eff_arr
 
     def get_projection_type(self):
+        """
+        Return the projection type of the calculation
+
+        Returns
+        -------
+        projection_type: str
+            string describing the projection type
+        """
         return self.projection_type
 
     def ipc_convolve(self, rate, kernel):
+        """
+        Introduce inter-pixel communication effect via convolution of the rate image.
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+        kernel : np.ndarray
+            appropriate IPC kernel given the number of groups
+
+        Returns
+        -------
+        fp_pix_ipc: np.ndarray
+            2D rate array with IPC effect added
+        """
         fp_pix_ipc = sg.fftconvolve(rate, kernel, mode='same')
 
         debug_utils.debugarrays.store('signal', 'ipc_convolve',
                                       {
                                           'rate': rate,
                                           'kernel': kernel,
                                           'fp_pix_ipc': fp_pix_ipc,
@@ -1595,46 +1644,121 @@
         # create a new array that starts in the middle of the first pixel and goes to the middle of the last pixel
         gridyvals = np.linspace(start_y + 0.5 * newsampy, start_y + newsampy * (self.newshape[0] - 0.5), self.newshape[0])[::-1]
         gridxvals = np.linspace(start_x + 0.5 * newsampx, start_x + newsampx * (self.newshape[1] - 0.5), self.newshape[1])
 
         self.grid = coords.IrregularGrid(gridyvals, gridxvals)
 
     def sum(self, rate):
+        """
+        Bin an array by summing. The input array is first cropped to the nearest lower
+        multiple of the binning factor (already computed)
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+
+        Returns
+        -------
+        croprate: np.ndarray
+            Cropped and binned 2D rate array
+        """
         # this MUST be sliced in numpy notation ([x,y]) rather than sequentially [x][y]) 
         croprate = rate[self.end_y:self.end_y+self.cropshape[0], self.start_x:self.start_x+self.cropshape[1]]
 
         # rebin the 2D array
         sh = int(self.newshape[0]), int(self.cropshape[0] // self.newshape[0]), int(self.newshape[1]), int(self.cropshape[1] // self.newshape[1])
         return croprate.reshape(sh).sum(-1).sum(1)
 
     def mean(self, rate):
+        """
+        Bin an array by taking the mean. The input array is first cropped to the nearest lower
+        multiple of the binning factor (already computed)
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+
+        Returns
+        -------
+        croprate: np.ndarray
+            Cropped and binned 2D rate array
+        """
         # this MUST be sliced in numpy notation ([x,y]) rather than sequentially [x][y]) 
         croprate = rate[self.end_y:self.end_y+self.cropshape[0], self.start_x:self.start_x+self.cropshape[1]]
 
         # rebin the 2D array
         sh = int(self.newshape[0]), int(self.cropshape[0] // self.newshape[0]), int(self.newshape[1]), int(self.cropshape[1] // self.newshape[1])
         return croprate.reshape(sh).mean(-1).mean(1)
 
     def min(self, rate):
+        """
+        Bin an array and take the minimum. The input array is first cropped to the nearest lower
+        multiple of the binning factor (already computed)
+
+        Used, for instance, in ngroups_before_saturation, where the lowest number wins
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+
+        Returns
+        -------
+        croprate: np.ndarray
+            Cropped and binned 2D rate array
+        """
         # this MUST be sliced in numpy notation ([x,y]) rather than sequentially [x][y]) 
         croprate = rate[self.end_y:self.end_y+self.cropshape[0], self.start_x:self.start_x+self.cropshape[1]]
 
         # rebin the 2D array
         sh = int(self.newshape[0]), int(self.cropshape[0] // self.newshape[0]), int(self.newshape[1]), int(self.cropshape[1] // self.newshape[1])
         return croprate.reshape(sh).min(-1).min(1)
 
     def max(self, rate):
+        """
+        Bin an array and take the maximum. The input array is first cropped to the nearest
+        lower multiple of the binning factor (already computed)
+
+        Used, for instance, in binning saturation maps, where an already-saturated pixel
+        knocks out the whole superpixel.
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+
+        Returns
+        -------
+        croprate: np.ndarray
+            Cropped and binned 2D rate array
+        """
         # this MUST be sliced in numpy notation ([x,y]) rather than sequentially [x][y]) 
         croprate = rate[self.end_y:self.end_y+self.cropshape[0], self.start_x:self.start_x+self.cropshape[1]]
 
         # rebin the 2D array
         sh = int(self.newshape[0]), int(self.cropshape[0] // self.newshape[0]), int(self.newshape[1]), int(self.cropshape[1] // self.newshape[1])
         return croprate.reshape(sh).max(-1).max(1)
 
     def dispersion(self, wave):
+        """
+        Bin a dispersed spectroscopic array using the mean. The input array is first
+        cropped to the nearest lower multiple of the binning factor (already computed)
+
+        Parameters
+        ----------
+        rate : np.ndarray
+            2D rate array
+
+        Returns
+        -------
+        croprate: np.ndarray
+            Cropped and binned 2D rate array
+        """
         if hasattr(self, "start_wave"):
             # We have now set up the cropping required.
             cropwave = wave[self.start_wave:self.start_wave+self.cropwaveshape]
             # rebin the wavelength array
             wavesh = int(self.newwaveshape), int(self.cropwaveshape // self.newwaveshape)
             # we take the mean rather than the sum, because we want the new midpoint
             # wavelength arrays generally aren't linear, so some info is lost here.
```

### Comparing `pandeia.engine-3.1/pandeia/engine/source.py` & `pandeia.engine-3.2/pandeia/engine/source.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/strategy.py` & `pandeia.engine-3.2/pandeia/engine/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,27 +277,44 @@
         my_detector_noise_list : List of DetectorNoise instances
 
         Returns
         -------
         products : Dictionary of strategy products.
                     detector_signal - 2D image of pixel count rates on detector plane
                     detector_noise - 2D image of pixel count rate standard deviations on detector plane
+                    detector_saturation - 2D map of saturated and partially saturated pixels
+                    detector_ngroups - 2D map of the number of groups/resultants before saturation
                     wavelength - either a wavelength vector for spectroscopic modes or the effective wavelength
                                  for imaging modes.
                     extracted_flux - The flux extracted by the strategy from the input detector pixel plane(s). This is always
                                      background-subtracted either via a background extracted from another aperture or an
                                      ideal noiseless sky background.
                     extracted_noise - The noise extracted by the strategy from the input detector pixel plane(s).
                     extracted_flux_plus_bg - The flux extracted by the strategy from the input detector pixel plane(s) with
-                                             sky background included in signal.  If background subtraction is done via an
-                                             aperture, this will be the same as 'extracted_flux'.  If an ideal background is
-                                             assumed, then this will include the flux from the sky background as well.
+                                             sky background and dark current included in signal.  If background subtraction 
+                                             is done via an aperture, this will be the same as 'extracted_flux'.  If an ideal 
+                                             background is assumed, then this will include the flux from the sky background as well.
+                    extracted_bg_total - The total flux through the background aperture, including target wings and other targets
+                    extracted_bg_only - The flux through the background aperture of specifically non-scene objects (background,
+                                        dark current, etc)
+                    reconstructed - Optional. Reconstructed detector plane product (relevant for dithered or IFU calculations)
+                    warnings - the combined warnings dictionaries of every step along the computational chain
+
+                    Products for technical purposes
                     source_flux_in_fov - The total sum of all source flux within the scene field of view (no background).
-                    source_flux_in_fov_plus_bg - The total sum of all flux within the scene, including the background.
-                    reconstructed - Reconstructed detector plane product (relevant for dithered or IFU calculations)
+                    extracted_flux_plus_bg_all - The total target flux through both target aperture and background aperture
+                    extracted_source_noise - The target extracted through the square of the target aperture
+                    plane_grid - Grid instance
+                    aperture_size - Target Aperture size in input units
+                    extraction_area - Target Aperture size in pixels^2
+                    background_area - Sky Annulus size in pixels^2 (0 if an ideal background is assumed)
+                    mask_products - Target Aperture mask array
+                    saturation_products - Dictionary of saturated pixel products
+                    aperture_sizes_arcsec - Optional. If aperture_size is pixels, aperture_sizes_arcsec is in arcseconds.
+                    source_flux_in_fov_plus_bg - Optional. The total sum of all flux within the scene, including the background.
         """
 
         # We calculate the weights for all the dithers first, because each dither may have different weights, depending
         # on the strategy. These differences between dithers are not known to the general extract method, but only to the
         # specific _createWeightMatrix methods, which are redefined for each strategy.
         a_ij_list, product_subscripts_list = self._create_weight_matrix(my_detector_signal_list, my_detector_noise_list)
 
@@ -997,21 +1014,44 @@
             # if the sources are extended, they need to be rotated
             if s.shape['geometry'] != "point":
                 sources[i].position['orientation'] = (sources[i].position['orientation'] + self.scene_rotation) % 360.0
 
         return sources
 
     def is_pixel_units(self):
+        """
+        Simple check for whether the extraction strategy units are pixels or arcseconds
+
+        Returns
+        -------
+        is_pixels: bool
+            Bool describing whether we are using pixel units
+        """
         is_pixels = False
         if hasattr(self, "units") and 'pixel' == self.units:
             is_pixels = True
         
         return is_pixels
 
     def convert_extraction_units(self, units_in, units_to):
+        """
+        Generic function to convert units. Typically used when units_in is pixels, and units_to is arcsec.
+
+        Parameters
+        ----------
+        units_in : str
+            A valid astropy unit name
+        units_to : str
+            A valid astropy unit name
+
+        Raises
+        ------
+        EngineInputError
+            If the units are not recognized
+        """
         # Verify that the user specified units are supported.
         if self.units not in self.permitted_units:
             msg = "Unsupported unit type, %s, in strategy %s" % (self.units, self.__class__.__name__)
             raise EngineInputError(value=msg)
 
         # If aperture_size is a list, make sure we convert each axis with the correct pixel scale.
         if isinstance(self.aperture_size, list):
@@ -1102,19 +1142,45 @@
                 message = "Number of on_target designations must equal number of dithers for %s." % self.__class__.__name__
                 raise EngineInputError(value=message)
         else:
             self.on_target = [True]
             self.dithers = [{"x": 0.0, "y": 0.0}]
 
     def _check_aperture_size(self):
+        """
+        Sanity check: Aperture radius must be positive
+
+        Raises
+        ------
+        EngineInputError
+            If the check fails
+        """
         if self.aperture_size <= 0.0:
             msg = "%s error: aperture radius must be > 0.0." % self.__class__.__name__
             raise EngineInputError(value=msg)
         
     def _check_circular_annulus_limits(self, aperture):
+        """
+        If the sky_annulus exists and realistic subtraction, background_subtraction=True,
+        is being done: Make sure the inner radius is greater than the outer radius Make
+        sure the inner radius is larger than the target aperture
+
+        Neither of these actually prevent the same pixels from being identified as part of
+        the sky annulus and target aperture, but it reduces the possibiilty of confusion.
+
+        Parameters
+        ----------
+        aperture : float
+            The target aperture, in units.
+
+        Raises
+        ------
+        EngineInputError
+            If either tested condition fails
+        """
         if self.background_subtraction:
             # check source and background regions to make sure they don't overlap
             if isinstance(aperture, (np.ndarray, list)):
                 ap = np.max(aperture)
             else:
                 ap = aperture
             bk_inner = self.sky_annulus[0]
@@ -1222,14 +1288,42 @@
             extraction_area_pix = aper_area_pix
         if n_aper < 0.9 * extraction_area_pix and ap_outside_fov is False:
             loss_pct = 100.0 * (1.0 - n_aper / aper_area_pix)
             key = 'extraction_aperture_undersampled'
             self.warnings[key] = warning_messages[key] % loss_pct
 
     def _get_aperture_size(self, wavelengths):
+        """
+        Implement Encircled Energy Extraction.
+
+        This function takes in a wavelength and loads and reads the corresponding EE table
+        from the fits file.
+
+        Then it does 2D (bilinear) interpolation into the EE table for the correct
+        wavelength and EE percentage. The resulting value is the size in arcseconds,
+        preserved as aperture_sizes_arcsec.
+
+        Parameters
+        ----------
+        wavelengths : np.ndarray
+            The wavelength(s) at which the encircled energy is desired.
+
+        Returns
+        -------
+        aperture_size: np.ndarray
+            The aperture size in arcseconds
+
+        Raises
+        ------
+        NotImplementedError
+            Only HST is allowed to run EE extraction at present.
+        EngineInputError
+            Encircled Energy value outside file bounds.
+        """
+
         if hasattr(self, "is_aperture_ee") and self.is_aperture_ee:
 
             # TODO: Temporary code to disable EE extraction for all telescopes other than
             # HST (JETC-3624, JETC-3626) due to concerns about appropriate use of
             # subpixels and WebbPSF flux distribution issues.
             if not self.instrument.telescope.tel_name == "hst":
                 raise NotImplementedError(f"Encircled Energy is not supported for {self.instrument.telescope.tel_name}")
@@ -2021,15 +2115,15 @@
             # wavelength array will too low by x wavelength elements.
             # 1. Get fractional part of wave_off_pix - this is the fraction of wavelength elements
             #    the array will be off by.
             wave_off_subpix = wave_off_pix % 1
             if wave_off_subpix != 0.0:
                 # 2. Set up the wavelength grid in wavelength elements
                 wave_elements = np.arange(nw)
-                # bounds_error=False fills pixels outside of the interpolation range with np.NaN, rather than crashing
+                # bounds_error=False fills pixels outside of the interpolation range with np.nan, rather than crashing
                 interpolator = sc.interpolate.interp1d(wave_elements, wave_pix, bounds_error=False)
                 # 3. Now find the offset wavelength elements.
                 wave_off_elements = wave_elements-wave_off_subpix
                 wave_pix = interpolator(wave_off_elements)
 
                 # trim the wavelength array and shorten it
                 nw = nw - 1
@@ -2328,15 +2422,15 @@
             # wavelength array will too low by x wavelength elements.
             # 1. Get fractional part of wave_off_pix - this is the fraction of wavelength elements
             #    the array will be off by.
             wave_off_subpix = wave_off_pix % 1
             if wave_off_subpix != 0.0:
                 # 2. Set up the wavelength grid in wavelength elements
                 wave_elements = np.arange(nw)
-                # bounds_error=False fills pixels outside of the interpolation range with np.NaN, rather than crashing
+                # bounds_error=False fills pixels outside of the interpolation range with np.nan, rather than crashing
                 interpolator = sc.interpolate.interp1d(wave_elements, wave_pix, bounds_error=False)
                 # 3. Now find the offset wavelength elements.
                 wave_off_elements = wave_elements-wave_off_subpix
                 wave_pix = interpolator(wave_off_elements)
 
                 # trim the wavelength array and shorten it
                 nw = nw - 1
@@ -2392,14 +2486,18 @@
         if len(waves) < nw:
             msg = "Extraction aperture out of range in dispersion direction."
             raise EngineInputError(value=msg)
 
         return weight_matrix, product_subscripts
 
     def _error_sum(self, a_ij, product_subscripts, my_detector_signal, my_detector_noise):
+        """
+        Special customizations for SpecSegmentedPhot: Run through the ImagingApPhot
+        _error_sum, not SpecApPhot's customized version.
+        """
         exposure_products = ImagingApPhot._error_sum(self, a_ij, product_subscripts, my_detector_signal, my_detector_noise)
 
         return exposure_products
 
     def _sanity_checks(self):
         """
         The SpecSegmentedPhot checks require information from the DetectorSignal, and thus
@@ -2484,14 +2582,30 @@
             # Add the API parameters specific to this strategy
             self.api_parameters = ["method", "units", "target_xy", "scan_extraction_length",
                                    "background_subtraction", "reference_wavelength"]
 
         SpecApPhot.__init__(self, instrument=instrument, config=config, webapp=webapp, **kwargs)
 
     def _create_weight_matrix(self, my_detector_signal_list, my_detector_noise_list):
+        """
+        SpecScanApPhot weight matrix is a regular SpecApPhot weight matrix with either
+        one-pixel height or scan length height.
+
+        Parameters
+        ----------
+        my_detector_signal_list : list
+            A list of DetectorSignal instances
+        my_detector_noise_list : list
+            A list of DetectorNoise instances
+
+        Returns
+        -------
+        products
+            Return ordinary SpecApPhot weight matrix products
+        """
         # Set up the extraction box.  Set up aperture_size, then the computation should match SpecApPhot.
         # aperture_size should either be 1 pixel converted to arcsecs, or the scan length (already in arcsec).
         # aperture_size (as used in SpecApPhot) is a radius, so it will be double.
         self.aperture_size = self.instrument.get_scan_length()
 
         if self.scan_extraction_length == 'pixel':
             # WFC3IR has rectangular pixels, so we need to get the right pixel size based on the dispersion direction.
```

### Comparing `pandeia.engine-3.1/pandeia/engine/telescope.py` & `pandeia.engine-3.2/pandeia/engine/telescope.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia/engine/utils.py` & `pandeia.engine-3.2/pandeia/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/pandeia.engine.egg-info/PKG-INFO` & `pandeia.engine-3.2/pandeia.engine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: pandeia.engine
-Version: 3.1
+Version: 3.2
 Summary: Pandeia 3D Exposure Time Calculator compute engine
 Home-page: https://jwst.etc.stsci.edu
 Author: Adric Riedel, Isaac Spitzer, Dharini Chittiraibalan, Oi In Tam, Chris Sontag, Ivo Busko, Craig Jones, Tim Pickering, Klaus Pontoppidan
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: numpy>=1.17
-Requires-Dist: scipy>1.6
-Requires-Dist: astropy>=4
-Requires-Dist: photutils
-Requires-Dist: synphot
-Requires-Dist: stsynphot
-Requires-Dist: setuptools
 
 The Pandeia engine is a 'simulation-hybrid' exposure time calculation engine that performs calculations on two-dimensional astronomical scenes created by the user. It uses a pixel-based 3D approach, modeling both the spatial and wavelength dimensions using realistic PSFs for each instrument mode, and handles saturation, correlated read noise, and inter-pixel capacitance. It supports both the James Webb Space Telescope and the Wide-field Imager mode of the Nancy Grace Roman Space Telescope.
 
 Installation and setup instructions (including a required data package) for the Pandeia engine can be found at this Space Telescope Science Institute page: https://outerspace.stsci.edu/display/PEN/Pandeia+Engine+News
 
 See also this page for James Webb Space Telescope (JWST)-specific installation instructions:
 https://jwst-docs.stsci.edu/jwst-exposure-time-calculator-overview/jwst-etc-pandeia-engine-tutorial/installing-pandeia
```

### Comparing `pandeia.engine-3.1/pandeia.engine.egg-info/SOURCES.txt` & `pandeia.engine-3.2/pandeia.engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandeia.engine-3.1/setup.py` & `pandeia.engine-3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         out.write(DEVBUILD)
 except (subprocess.CalledProcessError, FileNotFoundError) as err:
     print(err)
 
 setup(
     # The package
     name="pandeia.engine",
-    version="3.1",
+    version="3.2",
     packages=["pandeia",
               "pandeia.engine",
               "pandeia.engine.defaults",
               "pandeia.engine.helpers",
               "pandeia.engine.helpers.bit",
               "pandeia.engine.helpers.bit.config",
               "pandeia.engine.helpers.bit.etc_web_data",
```

